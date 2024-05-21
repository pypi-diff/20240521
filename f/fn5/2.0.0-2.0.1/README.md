# Comparing `tmp/fn5-2.0.0.tar.gz` & `tmp/fn5-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fn5-2.0.0.tar", last modified: Mon May 20 14:54:24 2024, max compression
+gzip compressed data, was "fn5-2.0.1.tar", last modified: Mon May 20 15:16:33 2024, max compression
```

## Comparing `fn5-2.0.0.tar` & `fn5-2.0.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:54:24.538692 fn5-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     5730 2024-05-20 14:53:36.000000 fn5-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-05-20 14:54:24.538692 fn5-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5732 2024-05-20 14:53:36.000000 fn5-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:54:24.538692 fn5-2.0.0/fn5.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-05-20 14:54:24.000000 fn5-2.0.0/fn5.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-20 14:54:24.000000 fn5-2.0.0/fn5.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 14:54:24.000000 fn5-2.0.0/fn5.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 14:53:59.000000 fn5-2.0.0/fn5.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-20 14:54:24.000000 fn5-2.0.0/fn5.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-20 14:53:36.000000 fn5-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 14:54:24.538692 fn5-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-05-20 14:53:36.000000 fn5-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:54:24.538692 fn5-2.0.0/src/
--rw-r--r--   0 runner    (1001) docker     (127)    21409 2024-05-20 14:53:36.000000 fn5-2.0.0/src/comparisons.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5815 2024-05-20 14:53:36.000000 fn5-2.0.0/src/fn5_python.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:54:24.538692 fn5-2.0.0/src/include/
--rw-r--r--   0 runner    (1001) docker     (127)     5357 2024-05-20 14:53:36.000000 fn5-2.0.0/src/include/comparisons.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5357 2024-05-20 14:53:36.000000 fn5-2.0.0/src/include/sample.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    14308 2024-05-20 14:53:36.000000 fn5-2.0.0/src/sample.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:54:24.538692 fn5-2.0.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-05-20 14:53:36.000000 fn5-2.0.0/test/test_outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-05-20 14:53:36.000000 fn5-2.0.0/test/test_py_bindings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:16:32.997971 fn5-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     5730 2024-05-20 15:15:56.000000 fn5-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-05-20 15:16:32.997971 fn5-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5732 2024-05-20 15:15:56.000000 fn5-2.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:16:32.997971 fn5-2.0.1/fn5.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-05-20 15:16:32.000000 fn5-2.0.1/fn5.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-20 15:16:32.000000 fn5-2.0.1/fn5.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 15:16:32.000000 fn5-2.0.1/fn5.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 15:16:09.000000 fn5-2.0.1/fn5.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-20 15:16:32.000000 fn5-2.0.1/fn5.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-20 15:15:56.000000 fn5-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 15:16:32.997971 fn5-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-05-20 15:15:56.000000 fn5-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:16:32.997971 fn5-2.0.1/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    21409 2024-05-20 15:15:56.000000 fn5-2.0.1/src/comparisons.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5815 2024-05-20 15:15:56.000000 fn5-2.0.1/src/fn5_python.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:16:32.997971 fn5-2.0.1/src/include/
+-rw-r--r--   0 runner    (1001) docker     (127)     5357 2024-05-20 15:15:56.000000 fn5-2.0.1/src/include/comparisons.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5357 2024-05-20 15:15:56.000000 fn5-2.0.1/src/include/sample.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    14308 2024-05-20 15:15:56.000000 fn5-2.0.1/src/sample.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:16:32.997971 fn5-2.0.1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-05-20 15:15:56.000000 fn5-2.0.1/test/test_outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-05-20 15:15:56.000000 fn5-2.0.1/test/test_py_bindings.py
```

### Comparing `fn5-2.0.0/LICENSE` & `fn5-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fn5-2.0.0/PKG-INFO` & `fn5-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fn5
-Version: 2.0.0
+Version: 2.0.1
 Summary: Fast, scalable SNP distance calculation from disk.
 Home-page: https://github.com/oxfordmmm/FN5
 Author: Jeremy Westhead
 Author-email: jeremy.westhead@ndm.ox.ac.uk
 License: University of Oxford, see LICENSE
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `fn5-2.0.0/README.md` & `fn5-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `fn5-2.0.0/fn5.egg-info/PKG-INFO` & `fn5-2.0.1/fn5.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fn5
-Version: 2.0.0
+Version: 2.0.1
 Summary: Fast, scalable SNP distance calculation from disk.
 Home-page: https://github.com/oxfordmmm/FN5
 Author: Jeremy Westhead
 Author-email: jeremy.westhead@ndm.ox.ac.uk
 License: University of Oxford, see LICENSE
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `fn5-2.0.0/setup.py` & `fn5-2.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Based on example https://github.com/pybind/python_example
 from pybind11.setup_helpers import Pybind11Extension
 from setuptools import setup
 from pathlib import Path
 import os
 
-__version__ = "v2.0.0"
+__version__ = "v2.0.1"
 
 try:
     this_directory = Path(__file__).parent
     long_description = (this_directory / "PYTHON_README.md").read_text()
 except FileNotFoundError:
     # Issues around packaging other readme means we can just skip on install
     long_description = "Fast, scalable SNP distance calculation from disk."
```

### Comparing `fn5-2.0.0/src/comparisons.cpp` & `fn5-2.0.1/src/comparisons.cpp`

 * *Files identical despite different names*

### Comparing `fn5-2.0.0/src/fn5_python.cpp` & `fn5-2.0.1/src/fn5_python.cpp`

 * *Files identical despite different names*

### Comparing `fn5-2.0.0/src/include/comparisons.hpp` & `fn5-2.0.1/src/include/comparisons.hpp`

 * *Files identical despite different names*

### Comparing `fn5-2.0.0/src/include/sample.hpp` & `fn5-2.0.1/src/include/sample.hpp`

 * *Files identical despite different names*

### Comparing `fn5-2.0.0/src/sample.cpp` & `fn5-2.0.1/src/sample.cpp`

 * *Files identical despite different names*

### Comparing `fn5-2.0.0/test/test_outputs.py` & `fn5-2.0.1/test/test_outputs.py`

 * *Files identical despite different names*

### Comparing `fn5-2.0.0/test/test_py_bindings.py` & `fn5-2.0.1/test/test_py_bindings.py`

 * *Files identical despite different names*

