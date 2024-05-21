# Comparing `tmp/geogif-0.1.5.tar.gz` & `tmp/geogif-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geogif-0.1.5.tar", max compression
+gzip compressed data, was "geogif-0.2.tar", max compression
```

## Comparing `geogif-0.1.5.tar` & `geogif-0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1067 2021-05-01 05:47:29.391768 geogif-0.1.5/LICENSE
--rw-r--r--   0        0        0     1829 2023-02-10 04:19:12.431810 geogif-0.1.5/README.md
--rw-r--r--   0        0        0      321 2022-03-17 03:06:09.675312 geogif-0.1.5/geogif/__init__.py
--rw-r--r--   0        0        0    16117 2023-07-23 19:04:01.315151 geogif-0.1.5/geogif/gif.py
--rw-r--r--   0        0        0     1141 2023-07-23 19:04:01.317492 geogif-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2608 1970-01-01 00:00:00.000000 geogif-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1067 2021-05-01 05:47:29.391768 geogif-0.2/LICENSE
+-rw-r--r--   0        0        0     1829 2023-02-10 04:19:12.431810 geogif-0.2/README.md
+-rw-r--r--   0        0        0      321 2022-03-17 03:06:09.675312 geogif-0.2/geogif/__init__.py
+-rw-r--r--   0        0        0    19511 2024-05-21 15:50:36.550096 geogif-0.2/geogif/gif.py
+-rw-r--r--   0        0        0     1160 2024-05-21 15:54:37.715679 geogif-0.2/pyproject.toml
+-rw-r--r--   0        0        0     2661 1970-01-01 00:00:00.000000 geogif-0.2/PKG-INFO
```

### Comparing `geogif-0.1.5/LICENSE` & `geogif-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `geogif-0.1.5/README.md` & `geogif-0.2/README.md`

 * *Files identical despite different names*

### Comparing `geogif-0.1.5/geogif/gif.py` & `geogif-0.2/geogif/gif.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
 
 def _validate_arr_for_gif(
     arr: xr.DataArray,
     cmap: str | matplotlib.colors.Colormap | None,
     date_format: str | None,
     date_position: Literal["ul", "ur", "ll", "lr"],
+    date_size: int | float,
 ) -> tuple[xr.DataArray, matplotlib.colors.Colormap | None]:
     if arr.ndim not in (3, 4):
         raise ValueError(
             f"Array must only have the dimensions 'time', 'y', 'x', and optionally 'band', not {arr.dims!r}"
         )
     if arr.ndim == 3:
         arr = arr.expand_dims("band", axis=1)
@@ -56,37 +57,93 @@
         try:
             time_coord.dt.strftime
         except (TypeError, AttributeError):
             raise TypeError(
                 f"Coordinates for the {time_coord.name} dimension are not datetimes, or don't support `strftime`. "
                 "Set `date_format=False`"
             )
-        assert date_position in (
-            "ul",
-            "ur",
-            "ll",
-            "lr",
+        assert (
+            date_position
+            in (
+                "ul",
+                "ur",
+                "ll",
+                "lr",
+            )
         ), f"date_position must be one of ('ul', 'ur', 'll', 'lr'), not {date_position}."
 
+        if isinstance(date_size, int):
+            assert date_size > 0, f"date_size must be >0, not {date_size}"
+        elif isinstance(date_size, float):
+            assert (
+                0 < date_size < 1
+            ), f"date_size must be greater than 0 and less than 1, not {date_size}"
+        else:
+            raise TypeError(
+                f"date_size must be int or float, not {type(date_size)}: {date_size}"
+            )
+
     return (arr, cmap)
 
 
+def _get_font(
+    date_size: int | float, labels: list[str], image_width: int
+) -> ImageFont.ImageFont | ImageFont.FreeTypeFont:
+    """
+    Get an appropriately-sized font for the requested ``date_size``
+
+    When ``date_size`` is a float, figure out a font size that will make the width of the
+    text that fraction of the width of the image.
+    """
+    if isinstance(date_size, int):
+        # absolute font size
+        return ImageFont.load_default(size=date_size)
+
+    target_width = date_size * image_width
+    test_label = max(labels, key=len)
+
+    fnt = ImageFont.load_default(size=5)
+    if isinstance(fnt, ImageFont.FreeTypeFont):
+        # NOTE: if Pillow doesn't have FreeType support, we won't get a font
+        # with adjustable size. So trying to increase the size would just
+        # loop infinitely.
+
+        def text_width(font) -> int:
+            bbox = font.getbbox(test_label)
+            return bbox[2] - bbox[0]
+
+        if text_width(fnt) > 0:
+            # check for zero-width so we don't loop forever.
+            # (could happen if `test_label` is an empty string or non-printable character)
+
+            # increment font until you get large enough text
+            while text_width(fnt) <= target_width:
+                try:
+                    size = fnt.size + 1
+                    fnt = ImageFont.load_default(size)
+                except OSError as e:
+                    raise RuntimeError(f"Invalid font size: {size}") from e
+
+    return fnt
+
+
 def gif(
     arr: xr.DataArray,
     *,
     to: str | Path | BinaryIO | None = None,
     fps: int = 16,
     robust: bool = True,
     vmin: float | None = None,
     vmax: float | None = None,
     cmap: str | matplotlib.colors.Colormap | None = None,
     date_format: str | None = "%Y-%m-%d",
     date_position: Literal["ul", "ur", "ll", "lr"] = "ul",
     date_color: tuple[int, int, int] = (255, 255, 255),
     date_bg: tuple[int, int, int] | None = (0, 0, 0),
+    date_size: int | float = 0.15,
 ) -> IPython.display.Image | None:
     """
     Render a `~xarray.DataArray` timestack (``time``, ``band``, ``y``, ``x``) into a GIF.
 
     If the `~xarray.DataArray` contains a `dask.array.Array`, use `dgif` (delayed-GIF) instead.
 
     The `~xarray.DataArray` must have 1 or 3 bands.
@@ -136,14 +193,22 @@
         ``"lr"`` (lower-right), default ``"ul"``.
     date_color:
         Color for the timestamp font, as an RGB 3-tuple. Default: ``(255, 255, 255)``
         (white).
     date_bg:
         Fill color to draw behind the timestamp (for legibility), as an RGB 3-tuple.
         Default: ``(0, 0, 0)`` (black). Set to None to disable.
+    date_size:
+        If a float, make the label this fraction of the width of the image.
+        If an int, use this absolute font size for the label.
+        Default: 0.15 (so the label is 15% of the image width).
+
+        Note that if Pillow does not have FreeType support, the font size
+        cannot be adjusted, and the text will be whatever size Pillow's
+        default basic font is (usually rather small).
 
     Returns
     -------
     IPython.display.Image or None
         If ``to`` is None, returns an `IPython.display.Image`, which will display the
         GIF in a Jupyter Notebook. (You can also get the GIF data as bytes from the Image's
         ``.data`` attribute.)
@@ -163,15 +228,15 @@
     >>> stackstac.gif(
     ...     arr.sel(band="ndvi"), cmap="YlGn", date_color=(0, 0, 0), date_bg=None
     ... )
     """
     if isinstance(arr.data, da.Array):
         raise TypeError("DataArray contains delayed data; use `dgif` instead.")
 
-    arr, cmap = _validate_arr_for_gif(arr, cmap, date_format, date_position)
+    arr, cmap = _validate_arr_for_gif(arr, cmap, date_format, date_position, date_size)
 
     # Rescale
     if arr.dtype.kind == "b":
         data = arr.data.astype("uint8", copy=False)
     else:
         if not robust and vmin is None and vmax is None:
             vmin = np.nanmin(arr)
@@ -203,15 +268,15 @@
     imgs = [Image.fromarray(frame) for frame in frames]
 
     # Write timestamps onto each frame
     if date_format:
         time_coord = arr[arr.dims[0]]
         labels = time_coord.dt.strftime(date_format).data
 
-        fnt = ImageFont.load_default()
+        fnt = _get_font(date_size, labels, imgs[0].size[0])
         for label, img in zip(labels, imgs):
             # get a drawing context
             d = ImageDraw.Draw(img)
             d = cast(ImageDraw.ImageDraw, d)
 
             width, height = img.size
             t_bbox = fnt.getbbox(label)
@@ -226,29 +291,38 @@
 
             if date_position[1] == "l":
                 x = offset
             else:
                 x = width - t_width - offset
 
             if date_bg:
-                d.rectangle((x, y, x + t_width, y + t_height), fill=date_bg)
-            # draw text
-            d.multiline_text((x, y), label, font=fnt, fill=date_color)
+                pad = 0.1 * t_height  # looks nicer
+                d.rectangle(
+                    (x - pad, y - pad, x + t_width + pad, y + t_height + pad),
+                    fill=date_bg,
+                )
+
+            # NOTE: sometimes the text seems to incorporate its own internal offset.
+            # This will show up in the first two coordinates of `t_bbox`, so we
+            # "de-offset" by these to make the rectangle and text align.
+            d.multiline_text(
+                (x - t_bbox[0], y - t_bbox[1]), label, font=fnt, fill=date_color
+            )
 
     out = to if to is not None else io.BytesIO()
     imgs[0].save(
         out,
         format="gif",
         save_all=True,
         append_images=imgs[1:],
         duration=1 / fps * 1000,  # ms
         loop=False,
     )
     if to is None and isinstance(out, io.BytesIO):
-        # second `isinstace` is just for the typechecker
+        # second `isinstance` is just for the typechecker
         try:
             import IPython.display
         except ImportError:
             raise ImportError(
                 "Cannot return an Image to display in a notebook, since IPython is not installed. "
                 "Pass a path or file to save the GIF to as the `to=` argument. "
                 "To get the GIF data as bytes, pass an instance of `io.BytesIO()`.\n"
@@ -270,23 +344,24 @@
 _dgif = dask.delayed(_gif, pure=True)
 
 
 def dgif(
     arr: xr.DataArray,
     *,
     bytes=False,
-    fps: int = 10,
+    fps: int = 16,
     robust: bool = True,
     vmin: float | None = None,
     vmax: float | None = None,
     cmap: str | matplotlib.colors.Colormap | None = None,
     date_format: str | None = "%Y-%m-%d",
     date_position: Literal["ul", "ur", "ll", "lr"] = "ul",
     date_color: tuple[int, int, int] = (255, 255, 255),
     date_bg: tuple[int, int, int] | None = (0, 0, 0),
+    date_size: int | float = 0.15,
 ) -> Delayed:
     """
     Turn a dask-backed `~xarray.DataArray` timestack into a GIF, as a `~dask.delayed.Delayed` object.
 
     The `~xarray.DataArray` must have 1 or 3 bands, and dimensions in
     (``time``, [optional ``band``], ``y``, ``x``) order.
 
@@ -346,14 +421,22 @@
         ``"lr"`` (lower-right), default ``"ul"``.
     date_color:
         Color for the timestamp font, as an RGB 3-tuple. Default: ``(255, 255, 255)``
         (white).
     date_bg:
         Fill color to draw behind the timestamp (for legibility), as an RGB 3-tuple.
         Default: ``(0, 0, 0)`` (black). Set to None to disable.
+    date_size:
+        If a float, make the label this fraction of the width of the image.
+        If an int, use this absolute font size for the label.
+        Default: 0.15 (so the label is 15% of the image width).
+
+        Note that if Pillow does not have FreeType support, the font size
+        cannot be adjusted, and the text will be whatever size Pillow's
+        default basic font is (usually rather small).
 
     Returns
     -------
     dask.Delayed
         Delayed object which, when computed, resolves to either an `IPython.display.Image`,
         or `bytes`.
 
@@ -377,15 +460,15 @@
 
     if not isinstance(arr.data, da.Array):
         raise TypeError(
             "DataArray does not contain delayed (Dask) data; use `gif` instead to render a GIF locally."
         )
 
     # Do some quick sanity checks to save you a lot of compute
-    _validate_arr_for_gif(arr, cmap, date_format, date_position)
+    _validate_arr_for_gif(arr, cmap, date_format, date_position, date_size)
 
     if not bytes:
         try:
             import IPython.display  # noqa: F401
         except ImportError:
             raise ImportError(
                 "Cannot return an Image to display in a notebook, since IPython is not installed "
@@ -410,8 +493,9 @@
         vmin=vmin,
         vmax=vmax,
         cmap=cmap,
         date_format=date_format,
         date_position=date_position,
         date_color=date_color,
         date_bg=date_bg,
+        date_size=date_size,
     )
```

### Comparing `geogif-0.1.5/pyproject.toml` & `geogif-0.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 [tool.poetry]
 name = "geogif"
-version = "0.1.5"
+version = "0.2"
 description = "Render xarray timestacks into GIFs"
 authors = ["Gabe Joseph <gjoseph92@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/gjoseph92/geogif"
 homepage = "https://geogif.readthedocs.io/en/latest/index.html"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 dask = {extras = ["delayed"], version = ">= 2021.4.1"}
 numpy = "^1.20.2"
-Pillow = "^10"
+Pillow = "^10.1"
 matplotlib = "^3.4.1"
 xarray = ">=0.18"
 
 [tool.poetry.group.dev.dependencies]
 jupyterlab = "^3.0.14"
 ipython = "^7.23.0"
-black = "^21.4b2"
+black = "^24.4.2"
 flake8 = "^3.9.1"
 shed = "^0.3.4"
 sphinx-autobuild = "^2021.3.14"
 Bottleneck = "^1.3.2"
 keyring = "^23.0.1"
 twine = "^3.4.1"
+netcdf4 = "^1.6.5"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^6.2.3"
 hypothesis = "^6.10.1"
 ipython = "^7.23.0"
```

### Comparing `geogif-0.1.5/PKG-INFO` & `geogif-0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: geogif
-Version: 0.1.5
+Version: 0.2
 Summary: Render xarray timestacks into GIFs
 Home-page: https://geogif.readthedocs.io/en/latest/index.html
 Author: Gabe Joseph
 Author-email: gjoseph92@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: Pillow (>=10,<11)
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: Pillow (>=10.1,<11.0)
 Requires-Dist: dask[delayed] (>=2021.4.1)
 Requires-Dist: matplotlib (>=3.4.1,<4.0.0)
 Requires-Dist: numpy (>=1.20.2,<2.0.0)
 Requires-Dist: xarray (>=0.18)
 Project-URL: Repository, https://github.com/gjoseph92/geogif
 Description-Content-Type: text/markdown
```

