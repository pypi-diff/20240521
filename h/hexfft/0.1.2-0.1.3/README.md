# Comparing `tmp/hexfft-0.1.2.tar.gz` & `tmp/hexfft-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hexfft-0.1.2.tar", last modified: Mon May  6 04:12:34 2024, max compression
+gzip compressed data, was "hexfft-0.1.3.tar", last modified: Tue May 21 06:29:34 2024, max compression
```

## Comparing `hexfft-0.1.2.tar` & `hexfft-0.1.3.tar`

### file list

```diff
@@ -1,29 +1,32 @@
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2024-05-06 04:12:34.803244 hexfft-0.1.2/
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2024-05-06 04:12:34.793331 hexfft-0.1.2/.github/
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2024-05-06 04:12:34.795053 hexfft-0.1.2/.github/workflows/
--rw-r--r--   0 chris      (501) staff       (20)     1094 2024-04-24 02:26:15.000000 hexfft-0.1.2/.github/workflows/python-package-conda.yml
--rw-r--r--   0 chris      (501) staff       (20)     1078 2024-04-06 16:16:22.000000 hexfft-0.1.2/LICENSE
--rw-r--r--   0 chris      (501) staff       (20)      954 2024-05-06 04:12:34.802992 hexfft-0.1.2/PKG-INFO
--rw-r--r--   0 chris      (501) staff       (20)      691 2024-05-06 04:06:16.000000 hexfft-0.1.2/README.md
--rw-r--r--   0 chris      (501) staff       (20)       55 2024-04-25 02:06:04.000000 hexfft-0.1.2/environment.yml
--rw-r--r--   0 chris      (501) staff       (20)      359 2024-05-06 04:11:25.000000 hexfft-0.1.2/pyproject.toml
--rw-r--r--   0 chris      (501) staff       (20)       22 2024-04-25 02:06:20.000000 hexfft-0.1.2/requirements.txt
--rw-r--r--   0 chris      (501) staff       (20)       38 2024-05-06 04:12:34.803290 hexfft-0.1.2/setup.cfg
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2024-05-06 04:12:34.793542 hexfft-0.1.2/src/
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2024-05-06 04:12:34.798412 hexfft-0.1.2/src/hexfft/
--rw-r--r--   0 chris      (501) staff       (20)       84 2024-04-25 00:42:25.000000 hexfft-0.1.2/src/hexfft/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)     4435 2024-05-03 01:21:02.000000 hexfft-0.1.2/src/hexfft/array.py
--rw-r--r--   0 chris      (501) staff       (20)     2245 2024-05-05 20:31:48.000000 hexfft-0.1.2/src/hexfft/grids.py
--rw-r--r--   0 chris      (501) staff       (20)    21129 2024-05-06 04:00:00.000000 hexfft-0.1.2/src/hexfft/hexfft.py
--rw-r--r--   0 chris      (501) staff       (20)     3722 2024-04-26 04:17:34.000000 hexfft-0.1.2/src/hexfft/plot.py
--rw-r--r--   0 chris      (501) staff       (20)     2896 2024-05-06 04:04:31.000000 hexfft-0.1.2/src/hexfft/reference.py
--rw-r--r--   0 chris      (501) staff       (20)     3841 2024-04-25 02:21:17.000000 hexfft-0.1.2/src/hexfft/utils.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2024-05-06 04:12:34.802693 hexfft-0.1.2/src/hexfft.egg-info/
--rw-r--r--   0 chris      (501) staff       (20)      954 2024-05-06 04:12:34.000000 hexfft-0.1.2/src/hexfft.egg-info/PKG-INFO
--rw-r--r--   0 chris      (501) staff       (20)      450 2024-05-06 04:12:34.000000 hexfft-0.1.2/src/hexfft.egg-info/SOURCES.txt
--rw-r--r--   0 chris      (501) staff       (20)        1 2024-05-06 04:12:34.000000 hexfft-0.1.2/src/hexfft.egg-info/dependency_links.txt
--rw-r--r--   0 chris      (501) staff       (20)        7 2024-05-06 04:12:34.000000 hexfft-0.1.2/src/hexfft.egg-info/top_level.txt
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2024-05-06 04:12:34.802274 hexfft-0.1.2/tests/
--rw-r--r--   0 chris      (501) staff       (20)     4025 2024-05-03 02:57:35.000000 hexfft-0.1.2/tests/test_api.py
--rw-r--r--   0 chris      (501) staff       (20)     9893 2024-05-06 04:04:02.000000 hexfft-0.1.2/tests/test_hexfft.py
--rw-r--r--   0 chris      (501) staff       (20)     3180 2024-04-25 02:31:28.000000 hexfft-0.1.2/tests/test_utils.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2024-05-21 06:29:34.616022 hexfft-0.1.3/
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2024-05-21 06:29:34.606299 hexfft-0.1.3/.github/
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2024-05-21 06:29:34.608215 hexfft-0.1.3/.github/workflows/
+-rw-r--r--   0 chris      (501) staff       (20)     1094 2024-04-24 02:26:15.000000 hexfft-0.1.3/.github/workflows/python-package-conda.yml
+-rw-r--r--   0 chris      (501) staff       (20)     1078 2024-04-06 16:16:22.000000 hexfft-0.1.3/LICENSE
+-rw-r--r--   0 chris      (501) staff       (20)      954 2024-05-21 06:29:34.615778 hexfft-0.1.3/PKG-INFO
+-rw-r--r--   0 chris      (501) staff       (20)      691 2024-05-06 04:06:16.000000 hexfft-0.1.3/README.md
+-rw-r--r--   0 chris      (501) staff       (20)       55 2024-04-25 02:06:04.000000 hexfft-0.1.3/environment.yml
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2024-05-21 06:29:34.609444 hexfft-0.1.3/examples/
+-rw-r--r--   0 chris      (501) staff       (20)   193281 2024-05-03 04:00:19.000000 hexfft-0.1.3/examples/HexArray.ipynb
+-rw-r--r--   0 chris      (501) staff       (20)   662246 2024-05-21 06:26:15.000000 hexfft-0.1.3/examples/RectangularPeriodicity.ipynb
+-rw-r--r--   0 chris      (501) staff       (20)      359 2024-05-21 06:26:25.000000 hexfft-0.1.3/pyproject.toml
+-rw-r--r--   0 chris      (501) staff       (20)       22 2024-04-25 02:06:20.000000 hexfft-0.1.3/requirements.txt
+-rw-r--r--   0 chris      (501) staff       (20)       38 2024-05-21 06:29:34.616066 hexfft-0.1.3/setup.cfg
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2024-05-21 06:29:34.606620 hexfft-0.1.3/src/
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2024-05-21 06:29:34.613556 hexfft-0.1.3/src/hexfft/
+-rw-r--r--   0 chris      (501) staff       (20)       84 2024-04-25 00:42:25.000000 hexfft-0.1.3/src/hexfft/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)     4431 2024-05-10 01:09:34.000000 hexfft-0.1.3/src/hexfft/array.py
+-rw-r--r--   0 chris      (501) staff       (20)     2245 2024-05-05 20:31:48.000000 hexfft-0.1.3/src/hexfft/grids.py
+-rw-r--r--   0 chris      (501) staff       (20)    21129 2024-05-08 01:41:54.000000 hexfft-0.1.3/src/hexfft/hexfft.py
+-rw-r--r--   0 chris      (501) staff       (20)     3722 2024-04-26 04:17:34.000000 hexfft-0.1.3/src/hexfft/plot.py
+-rw-r--r--   0 chris      (501) staff       (20)     2896 2024-05-08 01:06:26.000000 hexfft-0.1.3/src/hexfft/reference.py
+-rw-r--r--   0 chris      (501) staff       (20)     4563 2024-05-10 01:13:12.000000 hexfft-0.1.3/src/hexfft/utils.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2024-05-21 06:29:34.615489 hexfft-0.1.3/src/hexfft.egg-info/
+-rw-r--r--   0 chris      (501) staff       (20)      954 2024-05-21 06:29:34.000000 hexfft-0.1.3/src/hexfft.egg-info/PKG-INFO
+-rw-r--r--   0 chris      (501) staff       (20)      512 2024-05-21 06:29:34.000000 hexfft-0.1.3/src/hexfft.egg-info/SOURCES.txt
+-rw-r--r--   0 chris      (501) staff       (20)        1 2024-05-21 06:29:34.000000 hexfft-0.1.3/src/hexfft.egg-info/dependency_links.txt
+-rw-r--r--   0 chris      (501) staff       (20)        7 2024-05-21 06:29:34.000000 hexfft-0.1.3/src/hexfft.egg-info/top_level.txt
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2024-05-21 06:29:34.615155 hexfft-0.1.3/tests/
+-rw-r--r--   0 chris      (501) staff       (20)     4025 2024-05-03 02:57:35.000000 hexfft-0.1.3/tests/test_api.py
+-rw-r--r--   0 chris      (501) staff       (20)     9893 2024-05-06 04:04:02.000000 hexfft-0.1.3/tests/test_hexfft.py
+-rw-r--r--   0 chris      (501) staff       (20)     3180 2024-04-25 02:31:28.000000 hexfft-0.1.3/tests/test_utils.py
```

### Comparing `hexfft-0.1.2/.github/workflows/python-package-conda.yml` & `hexfft-0.1.3/.github/workflows/python-package-conda.yml`

 * *Files identical despite different names*

### Comparing `hexfft-0.1.2/LICENSE` & `hexfft-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hexfft-0.1.2/PKG-INFO` & `hexfft-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hexfft
-Version: 0.1.2
+Version: 0.1.3
 Summary: Hexagonal FFTs in Python
 Author-email: Chris Langfield <christopher.langfield@gmail.com>
 Keywords: hexagonal,dsp,fft
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `hexfft-0.1.2/README.md` & `hexfft-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `hexfft-0.1.2/src/hexfft/array.py` & `hexfft-0.1.3/src/hexfft/array.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import numpy as np
 from hexfft.grids import heshgrid, skew_heshgrid
 
 
-def _generate_indices(shape, pattern):
+def generate_indices(shape, pattern):
     N1, N2 = shape
     n1, n2 = np.meshgrid(np.arange(N1), np.arange(N2))
 
     # convert offset indices to oblique for internal representation
     if pattern == "offset":
         row_shift = np.repeat(np.arange(N1), 2)[1 : N1 + 1]
         n2 += row_shift
 
     return n1, n2
 
 
-def _generate_grid(shape, pattern):
+def generate_grid(shape, pattern):
     if pattern == "oblique":
         return skew_heshgrid(shape)
     elif pattern == "offset":
         return heshgrid(shape)
 
 
 class HexArray(np.ndarray):
@@ -49,16 +49,16 @@
 
         if pattern not in ["oblique", "offset"]:
             raise ValueError(
                 f"Coordinate system {pattern} is not implemented or unknown."
             )
 
         obj.pattern = pattern
-        obj.indices = _generate_indices(arr.shape[-2:], pattern)
-        obj.grid = _generate_grid(arr.shape[-2:], pattern)
+        obj.indices = generate_indices(arr.shape[-2:], pattern)
+        obj.grid = generate_grid(arr.shape[-2:], pattern)
 
         return obj
 
     # np.ndarray subclass boilerplate
     def __array_finalize__(self, obj):
         if obj is None:
             return
```

### Comparing `hexfft-0.1.2/src/hexfft/grids.py` & `hexfft-0.1.3/src/hexfft/grids.py`

 * *Files identical despite different names*

### Comparing `hexfft-0.1.2/src/hexfft/hexfft.py` & `hexfft-0.1.3/src/hexfft/hexfft.py`

 * *Files identical despite different names*

### Comparing `hexfft-0.1.2/src/hexfft/plot.py` & `hexfft-0.1.3/src/hexfft/plot.py`

 * *Files identical despite different names*

### Comparing `hexfft-0.1.2/src/hexfft/reference.py` & `hexfft-0.1.3/src/hexfft/reference.py`

 * *Files identical despite different names*

### Comparing `hexfft-0.1.2/src/hexfft/utils.py` & `hexfft-0.1.3/src/hexfft/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import numpy as np
-from hexfft.array import HexArray, _generate_indices
+from hexfft.array import HexArray, generate_indices
 from hexfft.grids import heshgrid, skew_heshgrid
 
 
 def hsupport(N, pattern="oblique"):
     """
     Return a boolean mask of the hexagonally periodic
     region inscribed in the square or parallelopiped region
     defined by h. h must have square dimensions with even
     side length. If h is NxN then the area of the mask
     is always 3 * N**2 / 4
 
     :param h: a HexArray
     """
     # assert N1 % 2 == 0, "Side length must be even."
-    n1, n2 = _generate_indices((N, N), pattern)
+    n1, n2 = generate_indices((N, N), pattern)
     M = N // 2
     if pattern == "offset":
         n2 = n2 - N // 4
 
     G = (0 <= n1) & (n1 < 2 * M)
     H = (0 <= n2) & (n2 < 2 * M)
     I = (-M <= n1 - n2) & (n1 - n2 < M)
@@ -107,14 +107,43 @@
         h = HexArray(np.zeros((N, N), p.dtype), pattern)
         h[support_below] = p[pgram_left]
         h[support_above] = p[pgram_right]
 
     return HexArray(h, pattern)
 
 
+def filter_shift(x):
+    """
+    Shift the quadrants of a HexArray to move the origin to/from
+    the center of the grid. Useful if a filter kernel is easier to define
+    the origin at the center of the grid.
+    """
+    if not isinstance(x, HexArray):
+        x = HexArray(x)
+
+    N1, N2 = x.shape
+    out = HexArray(np.zeros_like(x), x.pattern)
+
+    regI = x[N1 // 2 :, : N2 // 2]
+    regII = x[N1 // 2 :, N2 // 2 :]
+    regIII = x[: N1 // 2, : N2 // 2]
+    regIV = x[: N1 // 2, N2 // 2 :]
+
+    # II to I
+    out[: N1 // 2, : N2 // 2] = regII
+    # I to IV
+    out[: N1 // 2, N2 // 2 :] = regI
+    # III to II
+    out[N1 // 2 :, N2 // 2 :] = regIII
+    # IV to III
+    out[N1 // 2 :, : N2 // 2] = regIV
+
+    return out
+
+
 def nice_test_function(shape, hcrop=True, pattern="oblique"):
     h = HexArray(np.zeros(shape), pattern)
     N1, N2 = shape
     n1, n2 = np.meshgrid(np.arange(N1), np.arange(N2), indexing="ij")
     if hcrop:
         m = hsupport(N1, pattern)
     else:
```

### Comparing `hexfft-0.1.2/src/hexfft.egg-info/PKG-INFO` & `hexfft-0.1.3/src/hexfft.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hexfft
-Version: 0.1.2
+Version: 0.1.3
 Summary: Hexagonal FFTs in Python
 Author-email: Chris Langfield <christopher.langfield@gmail.com>
 Keywords: hexagonal,dsp,fft
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `hexfft-0.1.2/tests/test_api.py` & `hexfft-0.1.3/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `hexfft-0.1.2/tests/test_hexfft.py` & `hexfft-0.1.3/tests/test_hexfft.py`

 * *Files identical despite different names*

### Comparing `hexfft-0.1.2/tests/test_utils.py` & `hexfft-0.1.3/tests/test_utils.py`

 * *Files identical despite different names*

