# Comparing `tmp/ridgeplot_py-0.2.5.tar.gz` & `tmp/ridgeplot_py-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ridgeplot_py-0.2.5.tar", max compression
+gzip compressed data, was "ridgeplot_py-0.2.7.tar", max compression
```

## Comparing `ridgeplot_py-0.2.5.tar` & `ridgeplot_py-0.2.7.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11357 2024-05-10 05:09:27.876379 ridgeplot_py-0.2.5/LICENSE
--rw-r--r--   0        0        0     2960 2024-05-10 05:09:27.876379 ridgeplot_py-0.2.5/README.md
--rw-r--r--   0        0        0     1465 2024-05-10 05:09:40.904313 ridgeplot_py-0.2.5/pyproject.toml
--rw-r--r--   0        0        0       73 2024-05-10 05:09:27.876379 ridgeplot_py-0.2.5/ridgeplot/__init__.py
--rw-r--r--   0        0        0     8754 2024-05-10 05:09:27.876379 ridgeplot_py-0.2.5/ridgeplot/colors.py
--rw-r--r--   0        0        0     2174 2024-05-10 05:09:27.876379 ridgeplot_py-0.2.5/ridgeplot/dotted_heatmap.py
--rw-r--r--   0        0        0     3299 2024-05-10 05:09:27.876379 ridgeplot_py-0.2.5/ridgeplot/ridge_plot.py
--rw-r--r--   0        0        0      687 2024-05-10 05:09:27.876379 ridgeplot_py-0.2.5/ridgeplot/stats.py
--rw-r--r--   0        0        0     3741 1970-01-01 00:00:00.000000 ridgeplot_py-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-10 05:28:19.487476 ridgeplot_py-0.2.7/LICENSE
+-rw-r--r--   0        0        0     2960 2024-05-10 05:28:19.487476 ridgeplot_py-0.2.7/README.md
+-rw-r--r--   0        0        0     1465 2024-05-10 05:28:34.991564 ridgeplot_py-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0       73 2024-05-10 05:28:19.491476 ridgeplot_py-0.2.7/ridgeplot/__init__.py
+-rw-r--r--   0        0        0     8818 2024-05-10 05:28:19.491476 ridgeplot_py-0.2.7/ridgeplot/colors.py
+-rw-r--r--   0        0        0     2168 2024-05-10 05:28:19.491476 ridgeplot_py-0.2.7/ridgeplot/dotted_heatmap.py
+-rw-r--r--   0        0        0     3354 2024-05-10 05:28:19.491476 ridgeplot_py-0.2.7/ridgeplot/ridge_plot.py
+-rw-r--r--   0        0        0      687 2024-05-10 05:28:19.491476 ridgeplot_py-0.2.7/ridgeplot/stats.py
+-rw-r--r--   0        0        0     3741 1970-01-01 00:00:00.000000 ridgeplot_py-0.2.7/PKG-INFO
```

### Comparing `ridgeplot_py-0.2.5/LICENSE` & `ridgeplot_py-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ridgeplot_py-0.2.5/README.md` & `ridgeplot_py-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `ridgeplot_py-0.2.5/pyproject.toml` & `ridgeplot_py-0.2.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ridgeplot-py"
-version = "0.2.5"                                   # managed by poetry-dynamic-versioning
+version = "0.2.7"                                   # managed by poetry-dynamic-versioning
 description = "Plotting ridgeplots with matplotlib"
 authors = ["Douglas Wu <wckdouglas@gmail.com>"]
 license = "MIT"
 packages = [{ "include" = "ridgeplot" }]
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `ridgeplot_py-0.2.5/ridgeplot/colors.py` & `ridgeplot_py-0.2.7/ridgeplot/colors.py`

 * *Files 5% similar despite different names*

```diff
@@ -137,14 +137,15 @@
 
 class ColorEncoder:
     """
     color-encoding a categoric vector
 
     Example:
         ```
+        >>> from ridgeplot.colors import ColorEncoder, ColorPalette
         >>> categorical_vector = ['group a','group b','group c','group a']
         >>> colors = ColorPalette["okabeito"]
         >>> ce = ColorEncoder()
         >>> ce.fit(categorical_vector, colors)
         >>> ce.encoder
         OrderedDict([('group a', '#E69F00'),
              ('group b', '#56B4E9'),
@@ -275,12 +276,15 @@
         return lgd
 
 
 def get_cmap_color_values(cmap_name: str) -> Tuple[str, str]:
     """
     Get color values for the min and max color in a color map
 
-    :param str cmap_name: color map name (e.g. viridis)
-    :return Tuple[str, str]: hex code for the min and max color
+    Args:
+        cmap_name: color map name (e.g. viridis)
+
+    Returns:
+        hex code for the min and max color
     """
     cmap = get_cmap(cmap_name)
     return to_hex(cmap(0.0)), to_hex(cmap(1.0))
```

### Comparing `ridgeplot_py-0.2.5/ridgeplot/dotted_heatmap.py` & `ridgeplot_py-0.2.7/ridgeplot/dotted_heatmap.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,29 +22,31 @@
 ):
     """
     Plotting dotted heatmap
 
     Example:
         ```
         >>> import matplotlib.pyplot as plt
+        >>> from ridgeplot.dotted_heatmap import dotted_heatmap
         >>> fig = plt.figure()
         >>> ax = fig.add_subplot(111)
         >>> data = pd.DataFrame(
         ...    np.random.randn(n, n),
         ...    index=[f"feature{i}" for i in range(n)],
         ...    columns=[f"sample{i}" for i in range(n)],
         ... )
         >>> dotted_heatmap(data=data,ax=ax, cmap="viridis")
         ```
 
-    :param pd.DataFrame data: data to plot
-    :param matplotlib.axes ax: matplotlib ax object
-    :param str cmap: cmap value, defaults to "cividis"
-    :param Optional[float] circle_size: raidus of the circles,
-        if None, we will use relaive sizes, defaults to None
+    Args:
+        data: data to plot
+        ax: matplotlib ax object
+        cmap: cmap value, defaults to "cividis"
+        circle_size: raidus of the circles,
+            if None, we will use relaive sizes, defaults to None
     """
     nrows, ncols = data.shape
     x, y = np.meshgrid(np.arange(ncols), np.arange(nrows))
     radii = data.values / 2 / data.values.max()
     # radius is relative if circle_size is None
     circles = [
         plt.Circle((j, i), radius=circle_size if circle_size is not None else r)
@@ -60,9 +62,8 @@
 
     ax.set_xticks(np.arange(ncols + 1) - 0.5, minor=True)
     ax.set_yticks(np.arange(nrows + 1) - 0.5, minor=True)
     ax.grid(which="minor", alpha=0.5, color="white")
     ax.tick_params(left=False, bottom=False)
     for d in ["top", "bottom", "left", "right"]:
         ax.spines[d].set(alpha=0.5)
-    cbar = plt.colorbar(col)
-    return cbar
+    plt.colorbar(col)
```

### Comparing `ridgeplot_py-0.2.5/ridgeplot/ridge_plot.py` & `ridgeplot_py-0.2.7/ridgeplot/ridge_plot.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     """
     plotting a ridgeplot
 
     Example:
         ```
         >>> import numpy as np
         >>> import matplotlib.pyplot as plt
+        >>> from ridgeplot.ridge_plot import ridgeplot
 
         >>> data = {}
         >>> for i in range(10):
         >>>    data['data_{}'.format(i)] = np.random.randn(100) * (i+1)
 
         >>> fig = plt.figure()
         >>> ax = fig.add_subplot(111)
```

### Comparing `ridgeplot_py-0.2.5/ridgeplot/stats.py` & `ridgeplot_py-0.2.7/ridgeplot/stats.py`

 * *Files identical despite different names*

### Comparing `ridgeplot_py-0.2.5/PKG-INFO` & `ridgeplot_py-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ridgeplot-py
-Version: 0.2.5
+Version: 0.2.7
 Summary: Plotting ridgeplots with matplotlib
 License: MIT
 Author: Douglas Wu
 Author-email: wckdouglas@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ridgeplot-py Version: 0.2.5 Summary: Plotting
+Metadata-Version: 2.1 Name: ridgeplot-py Version: 0.2.7 Summary: Plotting
 ridgeplots with matplotlib License: MIT Author: Douglas Wu Author-email:
 wckdouglas@gmail.com Requires-Python: >=3.9,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Requires-Dist: matplotlib
 (>=3.8,<4.0) Requires-Dist: more-itertools (>=8.9.0,<9.0.0) Requires-Dist:
```

