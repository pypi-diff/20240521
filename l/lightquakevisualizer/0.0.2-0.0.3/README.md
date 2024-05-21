# Comparing `tmp/lightquakevisualizer-0.0.2.tar.gz` & `tmp/lightquakevisualizer-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightquakevisualizer-0.0.2.tar", last modified: Thu May 16 17:18:34 2024, max compression
+gzip compressed data, was "lightquakevisualizer-0.0.3.tar", last modified: Tue May 21 12:05:29 2024, max compression
```

## Comparing `lightquakevisualizer-0.0.2.tar` & `lightquakevisualizer-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 ulrich    (1000) ulrich    (1000)        0 2024-05-16 17:18:34.076333 lightquakevisualizer-0.0.2/
--rw-rw-r--   0 ulrich    (1000) ulrich    (1000)     1074 2024-05-14 14:46:16.000000 lightquakevisualizer-0.0.2/LICENSE
--rw-r--r--   0 ulrich    (1000) ulrich    (1000)     2507 2024-05-16 17:18:34.076333 lightquakevisualizer-0.0.2/PKG-INFO
--rw-rw-r--   0 ulrich    (1000) ulrich    (1000)     1847 2024-05-16 17:17:10.000000 lightquakevisualizer-0.0.2/README.md
-drwxrwxr-x   0 ulrich    (1000) ulrich    (1000)        0 2024-05-16 17:18:34.076333 lightquakevisualizer-0.0.2/lightquakevisualizer/
--rw-rw-r--   0 ulrich    (1000) ulrich    (1000)        0 2024-05-16 12:02:30.000000 lightquakevisualizer-0.0.2/lightquakevisualizer/__init__.py
--rwxrwxr-x   0 ulrich    (1000) ulrich    (1000)     6047 2024-05-16 12:47:50.000000 lightquakevisualizer-0.0.2/lightquakevisualizer/generateColorBar.py
--rwxrwxr-x   0 ulrich    (1000) ulrich    (1000)     2600 2024-05-16 12:47:50.000000 lightquakevisualizer-0.0.2/lightquakevisualizer/imageCombiner.py
--rw-rw-r--   0 ulrich    (1000) ulrich    (1000)     2787 2024-05-16 12:47:50.000000 lightquakevisualizer-0.0.2/lightquakevisualizer/imageCombinernew.py
--rwxrwxr-x   0 ulrich    (1000) ulrich    (1000)    23119 2024-05-16 16:52:14.000000 lightquakevisualizer-0.0.2/lightquakevisualizer/lightQuakeVisualizer.py
-drwxrwxr-x   0 ulrich    (1000) ulrich    (1000)        0 2024-05-16 17:18:34.076333 lightquakevisualizer-0.0.2/lightquakevisualizer.egg-info/
--rw-r--r--   0 ulrich    (1000) ulrich    (1000)     2507 2024-05-16 17:18:34.000000 lightquakevisualizer-0.0.2/lightquakevisualizer.egg-info/PKG-INFO
--rw-rw-r--   0 ulrich    (1000) ulrich    (1000)      496 2024-05-16 17:18:34.000000 lightquakevisualizer-0.0.2/lightquakevisualizer.egg-info/SOURCES.txt
--rw-rw-r--   0 ulrich    (1000) ulrich    (1000)        1 2024-05-16 17:18:34.000000 lightquakevisualizer-0.0.2/lightquakevisualizer.egg-info/dependency_links.txt
--rw-rw-r--   0 ulrich    (1000) ulrich    (1000)      211 2024-05-16 17:18:34.000000 lightquakevisualizer-0.0.2/lightquakevisualizer.egg-info/entry_points.txt
--rw-rw-r--   0 ulrich    (1000) ulrich    (1000)       73 2024-05-16 17:18:34.000000 lightquakevisualizer-0.0.2/lightquakevisualizer.egg-info/requires.txt
--rw-rw-r--   0 ulrich    (1000) ulrich    (1000)       21 2024-05-16 17:18:34.000000 lightquakevisualizer-0.0.2/lightquakevisualizer.egg-info/top_level.txt
--rw-rw-r--   0 ulrich    (1000) ulrich    (1000)      921 2024-05-16 16:53:49.000000 lightquakevisualizer-0.0.2/pyproject.toml
--rw-rw-r--   0 ulrich    (1000) ulrich    (1000)       38 2024-05-16 17:18:34.076333 lightquakevisualizer-0.0.2/setup.cfg
+drwxrwxr-x   0 ulrich    (1000) ulrich    (1000)        0 2024-05-21 12:05:29.638175 lightquakevisualizer-0.0.3/
+-rw-rw-r--   0 ulrich    (1000) ulrich    (1000)     1074 2024-05-14 14:46:16.000000 lightquakevisualizer-0.0.3/LICENSE
+-rw-r--r--   0 ulrich    (1000) ulrich    (1000)     2507 2024-05-21 12:05:29.638175 lightquakevisualizer-0.0.3/PKG-INFO
+-rw-rw-r--   0 ulrich    (1000) ulrich    (1000)     1847 2024-05-16 17:17:10.000000 lightquakevisualizer-0.0.3/README.md
+drwxrwxr-x   0 ulrich    (1000) ulrich    (1000)        0 2024-05-21 12:05:29.638175 lightquakevisualizer-0.0.3/lightquakevisualizer/
+-rw-rw-r--   0 ulrich    (1000) ulrich    (1000)        0 2024-05-16 12:02:30.000000 lightquakevisualizer-0.0.3/lightquakevisualizer/__init__.py
+-rwxrwxr-x   0 ulrich    (1000) ulrich    (1000)     6047 2024-05-16 12:47:50.000000 lightquakevisualizer-0.0.3/lightquakevisualizer/generateColorBar.py
+-rwxrwxr-x   0 ulrich    (1000) ulrich    (1000)     2600 2024-05-16 12:47:50.000000 lightquakevisualizer-0.0.3/lightquakevisualizer/imageCombiner.py
+-rw-rw-r--   0 ulrich    (1000) ulrich    (1000)     2787 2024-05-16 12:47:50.000000 lightquakevisualizer-0.0.3/lightquakevisualizer/imageCombinernew.py
+-rwxrwxr-x   0 ulrich    (1000) ulrich    (1000)    23211 2024-05-21 12:02:59.000000 lightquakevisualizer-0.0.3/lightquakevisualizer/lightQuakeVisualizer.py
+drwxrwxr-x   0 ulrich    (1000) ulrich    (1000)        0 2024-05-21 12:05:29.638175 lightquakevisualizer-0.0.3/lightquakevisualizer.egg-info/
+-rw-r--r--   0 ulrich    (1000) ulrich    (1000)     2507 2024-05-21 12:05:29.000000 lightquakevisualizer-0.0.3/lightquakevisualizer.egg-info/PKG-INFO
+-rw-rw-r--   0 ulrich    (1000) ulrich    (1000)      496 2024-05-21 12:05:29.000000 lightquakevisualizer-0.0.3/lightquakevisualizer.egg-info/SOURCES.txt
+-rw-rw-r--   0 ulrich    (1000) ulrich    (1000)        1 2024-05-21 12:05:29.000000 lightquakevisualizer-0.0.3/lightquakevisualizer.egg-info/dependency_links.txt
+-rw-rw-r--   0 ulrich    (1000) ulrich    (1000)      211 2024-05-21 12:05:29.000000 lightquakevisualizer-0.0.3/lightquakevisualizer.egg-info/entry_points.txt
+-rw-rw-r--   0 ulrich    (1000) ulrich    (1000)       73 2024-05-21 12:05:29.000000 lightquakevisualizer-0.0.3/lightquakevisualizer.egg-info/requires.txt
+-rw-rw-r--   0 ulrich    (1000) ulrich    (1000)       21 2024-05-21 12:05:29.000000 lightquakevisualizer-0.0.3/lightquakevisualizer.egg-info/top_level.txt
+-rw-rw-r--   0 ulrich    (1000) ulrich    (1000)      921 2024-05-21 12:05:06.000000 lightquakevisualizer-0.0.3/pyproject.toml
+-rw-rw-r--   0 ulrich    (1000) ulrich    (1000)       38 2024-05-21 12:05:29.638175 lightquakevisualizer-0.0.3/setup.cfg
```

### Comparing `lightquakevisualizer-0.0.2/LICENSE` & `lightquakevisualizer-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lightquakevisualizer-0.0.2/PKG-INFO` & `lightquakevisualizer-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightquakevisualizer
-Version: 0.0.2
+Version: 0.0.3
 Summary: A collection of scripts to visualize SeisSol output using pyvista
 Author: Thomas Ulrich
 License: MIT
 Project-URL: Repository, https://github.com/Thomas-Ulrich/light-quake-visualizer.git
 Keywords: pyvista,SeisSol
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `lightquakevisualizer-0.0.2/README.md` & `lightquakevisualizer-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `lightquakevisualizer-0.0.2/lightquakevisualizer/generateColorBar.py` & `lightquakevisualizer-0.0.3/lightquakevisualizer/generateColorBar.py`

 * *Files identical despite different names*

### Comparing `lightquakevisualizer-0.0.2/lightquakevisualizer/imageCombiner.py` & `lightquakevisualizer-0.0.3/lightquakevisualizer/imageCombiner.py`

 * *Files identical despite different names*

### Comparing `lightquakevisualizer-0.0.2/lightquakevisualizer/imageCombinernew.py` & `lightquakevisualizer-0.0.3/lightquakevisualizer/imageCombinernew.py`

 * *Files identical despite different names*

### Comparing `lightquakevisualizer-0.0.2/lightquakevisualizer/lightQuakeVisualizer.py` & `lightquakevisualizer-0.0.3/lightquakevisualizer/lightQuakeVisualizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import numpy as np
 import seissolxdmf
 import pyvista as pv
 import matplotlib.pyplot as plt
 import matplotlib.colors as mcolors
 import os
 import importlib
+import h5py
 
 pv.global_theme.nan_color = "white"
 
 
 class seissolxdmfExtended(seissolxdmf.seissolxdmf):
     def ComputeTimeIndices(self, at_times: list[str]) -> list[int]:
         """Retrieve list of time indices in file that match the given string.
@@ -523,18 +524,19 @@
             basename = f"{mod_prefix}{spvcc}{svar}_{mytime}"
         return f"output/{basename}.png"
 
     if fnames[0].endswith("xdmf"):
         sx = seissolxdmfExtended(fnames[0])
         time_indices = sx.ComputeTimeIndices(args.time[0].split(";"))
         output_times = sx.ReadTimes()
-    elif fname.endswith("hdf"):
+    elif fnames[0].endswith("hdf"):
         print("reading a hdf file, no time information available")
+        with h5py.File(fnames[0], "r") as f:
+            output_times = f["VTKHDF/FieldData/Time"][()]
         time_indices = [0]
-        output_times = [0]
     else:
         raise NotImplementedError("only supported files are xdmf and hdf")
     filtered_list = []
     n_output_times = len(output_times)
     for x in time_indices:
         if -n_output_times <= x < n_output_times:
             filtered_list.append(x)
```

### Comparing `lightquakevisualizer-0.0.2/lightquakevisualizer.egg-info/PKG-INFO` & `lightquakevisualizer-0.0.3/lightquakevisualizer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightquakevisualizer
-Version: 0.0.2
+Version: 0.0.3
 Summary: A collection of scripts to visualize SeisSol output using pyvista
 Author: Thomas Ulrich
 License: MIT
 Project-URL: Repository, https://github.com/Thomas-Ulrich/light-quake-visualizer.git
 Keywords: pyvista,SeisSol
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `lightquakevisualizer-0.0.2/pyproject.toml` & `lightquakevisualizer-0.0.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lightquakevisualizer"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
     {name = "Thomas Ulrich"},
 ]
 description = "A collection of scripts to visualize SeisSol output using pyvista"
 readme = "README.md"
 requires-python = ">=3.10"
 keywords = ["pyvista", "SeisSol"]
```

