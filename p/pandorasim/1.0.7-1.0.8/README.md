# Comparing `tmp/pandorasim-1.0.7.tar.gz` & `tmp/pandorasim-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandorasim-1.0.7.tar", max compression
+gzip compressed data, was "pandorasim-1.0.8.tar", max compression
```

## Comparing `pandorasim-1.0.7.tar` & `pandorasim-1.0.8.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1073 2022-08-04 17:51:49.568934 pandorasim-1.0.7/LICENSE
--rw-r--r--   0        0        0      229 2024-05-21 18:28:50.344224 pandorasim-1.0.7/pyproject.toml
--rw-r--r--   0        0        0      419 2024-05-21 18:28:53.132220 pandorasim-1.0.7/src/pandorasim/__init__.py
--rw-r--r--   0        0        0     4727 2024-05-21 02:31:51.097149 pandorasim-1.0.7/src/pandorasim/docstrings.py
--rw-r--r--   0        0        0    14831 2024-05-21 17:26:05.474937 pandorasim-1.0.7/src/pandorasim/nirsim.py
--rw-r--r--   0        0        0     6847 2024-05-21 18:28:55.178433 pandorasim-1.0.7/src/pandorasim/sim.py
--rw-r--r--   0        0        0    10482 2024-05-21 02:31:51.097745 pandorasim-1.0.7/src/pandorasim/utils.py
--rw-r--r--   0        0        0    20137 2024-05-21 18:28:18.250051 pandorasim-1.0.7/src/pandorasim/visiblesim.py
--rw-r--r--   0        0        0      485 1970-01-01 00:00:00.000000 pandorasim-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1073 2022-08-04 17:51:49.568934 pandorasim-1.0.8/LICENSE
+-rw-r--r--   0        0        0      229 2024-05-21 18:35:24.282281 pandorasim-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0      419 2024-05-21 18:35:22.949906 pandorasim-1.0.8/src/pandorasim/__init__.py
+-rw-r--r--   0        0        0     4727 2024-05-21 02:31:51.097149 pandorasim-1.0.8/src/pandorasim/docstrings.py
+-rw-r--r--   0        0        0    14831 2024-05-21 17:26:05.474937 pandorasim-1.0.8/src/pandorasim/nirsim.py
+-rw-r--r--   0        0        0     6847 2024-05-21 18:28:55.178433 pandorasim-1.0.8/src/pandorasim/sim.py
+-rw-r--r--   0        0        0    10482 2024-05-21 02:31:51.097745 pandorasim-1.0.8/src/pandorasim/utils.py
+-rw-r--r--   0        0        0    20270 2024-05-21 18:33:51.359940 pandorasim-1.0.8/src/pandorasim/visiblesim.py
+-rw-r--r--   0        0        0      485 1970-01-01 00:00:00.000000 pandorasim-1.0.8/PKG-INFO
```

### Comparing `pandorasim-1.0.7/LICENSE` & `pandorasim-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pandorasim-1.0.7/src/pandorasim/docstrings.py` & `pandorasim-1.0.8/src/pandorasim/docstrings.py`

 * *Files identical despite different names*

### Comparing `pandorasim-1.0.7/src/pandorasim/nirsim.py` & `pandorasim-1.0.8/src/pandorasim/nirsim.py`

 * *Files identical despite different names*

### Comparing `pandorasim-1.0.7/src/pandorasim/sim.py` & `pandorasim-1.0.8/src/pandorasim/sim.py`

 * *Files identical despite different names*

### Comparing `pandorasim-1.0.7/src/pandorasim/utils.py` & `pandorasim-1.0.8/src/pandorasim/utils.py`

 * *Files identical despite different names*

### Comparing `pandorasim-1.0.7/src/pandorasim/visiblesim.py` & `pandorasim-1.0.8/src/pandorasim/visiblesim.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,17 +164,20 @@
         # Apply poisson (shot) noise, ffi now has shape  (nrows, ncolumns), units of electrons
         ffi = np.random.poisson(self.scene.model(source_flux)[0])
         if hasattr(self.detector, "fieldstop"):
             ffi *= self.detector.fieldstop.astype(int)
 
         if noise:
             # Apply background to every read, units of electrons
-            ffi += np.random.poisson(
+            bkg = np.random.poisson(
                 (self.background_rate * int_time).value, size=ffi.shape
             ).astype(int)
+            if hasattr(self.detector, "fieldstop"):
+                bkg *= self.detector.fieldstop.astype(int)
+            ffi += bkg
 
             # # Apply a bias to every read which is a Gaussian with mean = bias * nreads value and std = (nreads * (read noise)**2)**0.5
             # We actually do this as a sum because otherwise the integer math doesn't work out...!?
 
             test_distribution = (
                 np.random.normal(
                     loc=self.detector.bias.value,
```

