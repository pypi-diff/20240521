# Comparing `tmp/pandorasim-1.0.6.tar.gz` & `tmp/pandorasim-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandorasim-1.0.6.tar", max compression
+gzip compressed data, was "pandorasim-1.0.7.tar", max compression
```

## Comparing `pandorasim-1.0.6.tar` & `pandorasim-1.0.7.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1073 2022-08-04 17:51:49.568934 pandorasim-1.0.6/LICENSE
--rw-r--r--   0        0        0      229 2024-05-21 18:23:51.531185 pandorasim-1.0.6/pyproject.toml
--rw-r--r--   0        0        0      419 2024-05-21 18:23:54.389496 pandorasim-1.0.6/src/pandorasim/__init__.py
--rw-r--r--   0        0        0     4727 2024-05-21 02:31:51.097149 pandorasim-1.0.6/src/pandorasim/docstrings.py
--rw-r--r--   0        0        0    14831 2024-05-21 17:26:05.474937 pandorasim-1.0.6/src/pandorasim/nirsim.py
--rw-r--r--   0        0        0     6728 2024-05-21 18:17:42.134196 pandorasim-1.0.6/src/pandorasim/sim.py
--rw-r--r--   0        0        0    10482 2024-05-21 02:31:51.097745 pandorasim-1.0.6/src/pandorasim/utils.py
--rw-r--r--   0        0        0    20149 2024-05-21 18:22:50.230081 pandorasim-1.0.6/src/pandorasim/visiblesim.py
--rw-r--r--   0        0        0      485 1970-01-01 00:00:00.000000 pandorasim-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1073 2022-08-04 17:51:49.568934 pandorasim-1.0.7/LICENSE
+-rw-r--r--   0        0        0      229 2024-05-21 18:28:50.344224 pandorasim-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0      419 2024-05-21 18:28:53.132220 pandorasim-1.0.7/src/pandorasim/__init__.py
+-rw-r--r--   0        0        0     4727 2024-05-21 02:31:51.097149 pandorasim-1.0.7/src/pandorasim/docstrings.py
+-rw-r--r--   0        0        0    14831 2024-05-21 17:26:05.474937 pandorasim-1.0.7/src/pandorasim/nirsim.py
+-rw-r--r--   0        0        0     6847 2024-05-21 18:28:55.178433 pandorasim-1.0.7/src/pandorasim/sim.py
+-rw-r--r--   0        0        0    10482 2024-05-21 02:31:51.097745 pandorasim-1.0.7/src/pandorasim/utils.py
+-rw-r--r--   0        0        0    20137 2024-05-21 18:28:18.250051 pandorasim-1.0.7/src/pandorasim/visiblesim.py
+-rw-r--r--   0        0        0      485 1970-01-01 00:00:00.000000 pandorasim-1.0.7/PKG-INFO
```

### Comparing `pandorasim-1.0.6/LICENSE` & `pandorasim-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pandorasim-1.0.6/src/pandorasim/docstrings.py` & `pandorasim-1.0.7/src/pandorasim/docstrings.py`

 * *Files identical despite different names*

### Comparing `pandorasim-1.0.6/src/pandorasim/nirsim.py` & `pandorasim-1.0.7/src/pandorasim/nirsim.py`

 * *Files identical despite different names*

### Comparing `pandorasim-1.0.6/src/pandorasim/sim.py` & `pandorasim-1.0.7/src/pandorasim/sim.py`

 * *Files 5% similar despite different names*

```diff
@@ -121,20 +121,27 @@
         """
 
         # This is fixed for visda, for now
         if hasattr(self.detector, "subarray_size"):
             shape = self.detector.subarray_size
         else:
             shape = self.detector.shape
-        
+
         radius = np.hypot(*np.asarray(shape) // 2)
         radius = ((radius * u.pixel) * self.detector.pixel_scale).to(u.deg).value
         # If there is a fieldstop, we can stop finding sources at that radius
-        if hasattr(self.detector.fieldstop_radius):
-            fieldstop_radius = ((self.detector.fieldstop_radius / self.detector.pixel_size) * self.detector.pixel_scale).to(u.deg).value
+        if hasattr(self.detector, "fieldstop_radius"):
+            fieldstop_radius = (
+                (
+                    (self.detector.fieldstop_radius / self.detector.pixel_size)
+                    * self.detector.pixel_scale
+                )
+                .to(u.deg)
+                .value
+            )
             if fieldstop_radius < radius:
                 radius = fieldstop_radius
 
         # Get location and magnitude data
         cat = ps.utils.get_sky_catalog(
             self.ra, self.dec, radius=radius * u.deg, **kwargs
         )
```

### Comparing `pandorasim-1.0.6/src/pandorasim/utils.py` & `pandorasim-1.0.7/src/pandorasim/utils.py`

 * *Files identical despite different names*

### Comparing `pandorasim-1.0.6/src/pandorasim/visiblesim.py` & `pandorasim-1.0.7/src/pandorasim/visiblesim.py`

 * *Files 0% similar despite different names*

```diff
@@ -159,17 +159,17 @@
         ).value.astype(int)
 
         # FFI has shape (nrows, ncolumns), in units of electrons.
         ffi = self.scene.model(source_flux)
 
         # Apply poisson (shot) noise, ffi now has shape  (nrows, ncolumns), units of electrons
         ffi = np.random.poisson(self.scene.model(source_flux)[0])
-        if hasattr(self.detector, 'fieldstop'):
+        if hasattr(self.detector, "fieldstop"):
             ffi *= self.detector.fieldstop.astype(int)
-            
+
         if noise:
             # Apply background to every read, units of electrons
             ffi += np.random.poisson(
                 (self.background_rate * int_time).value, size=ffi.shape
             ).astype(int)
 
             # # Apply a bias to every read which is a Gaussian with mean = bias * nreads value and std = (nreads * (read noise)**2)**0.5
```

