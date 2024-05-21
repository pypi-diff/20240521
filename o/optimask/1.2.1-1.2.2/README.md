# Comparing `tmp/optimask-1.2.1.tar.gz` & `tmp/optimask-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optimask-1.2.1.tar", last modified: Tue May 21 14:51:10 2024, max compression
+gzip compressed data, was "optimask-1.2.2.tar", last modified: Tue May 21 16:51:27 2024, max compression
```

## Comparing `optimask-1.2.1.tar` & `optimask-1.2.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:51:10.620873 optimask-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-21 14:50:57.000000 optimask-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-21 14:50:57.000000 optimask-1.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-05-21 14:51:10.620873 optimask-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-05-21 14:50:57.000000 optimask-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:51:10.620873 optimask-1.2.1/optimask/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-21 14:50:57.000000 optimask-1.2.1/optimask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-21 14:50:57.000000 optimask-1.2.1/optimask/_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     7017 2024-05-21 14:50:57.000000 optimask-1.2.1/optimask/_optimask.py
--rw-r--r--   0 runner    (1001) docker     (127)   427048 2024-05-21 14:51:10.000000 optimask-1.2.1/optimask/optimask_cython.c
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-21 14:50:57.000000 optimask-1.2.1/optimask/optimask_cython.pyx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:51:10.620873 optimask-1.2.1/optimask.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-05-21 14:51:10.000000 optimask-1.2.1/optimask.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-21 14:51:10.000000 optimask-1.2.1/optimask.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 14:51:10.000000 optimask-1.2.1/optimask.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-21 14:51:10.000000 optimask-1.2.1/optimask.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-21 14:51:10.000000 optimask-1.2.1/optimask.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 14:51:10.620873 optimask-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-05-21 14:50:57.000000 optimask-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:51:10.620873 optimask-1.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-21 14:50:57.000000 optimask-1.2.1/tests/test_optimask.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 16:51:27.237502 optimask-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-21 16:51:14.000000 optimask-1.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-21 16:51:14.000000 optimask-1.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-05-21 16:51:27.237502 optimask-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-05-21 16:51:14.000000 optimask-1.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 16:51:27.237502 optimask-1.2.2/optimask/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-21 16:51:14.000000 optimask-1.2.2/optimask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-21 16:51:14.000000 optimask-1.2.2/optimask/_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7017 2024-05-21 16:51:14.000000 optimask-1.2.2/optimask/_optimask.py
+-rw-r--r--   0 runner    (1001) docker     (127)   425891 2024-05-21 16:51:26.000000 optimask-1.2.2/optimask/optimask_cython.c
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-21 16:51:14.000000 optimask-1.2.2/optimask/optimask_cython.pyx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 16:51:27.237502 optimask-1.2.2/optimask.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-05-21 16:51:27.000000 optimask-1.2.2/optimask.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-21 16:51:27.000000 optimask-1.2.2/optimask.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 16:51:27.000000 optimask-1.2.2/optimask.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-21 16:51:27.000000 optimask-1.2.2/optimask.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-21 16:51:27.000000 optimask-1.2.2/optimask.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 16:51:27.237502 optimask-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-21 16:51:14.000000 optimask-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 16:51:27.237502 optimask-1.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-21 16:51:14.000000 optimask-1.2.2/tests/test_optimask.py
```

### Comparing `optimask-1.2.1/LICENSE` & `optimask-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `optimask-1.2.1/PKG-INFO` & `optimask-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: optimask
-Version: 1.2.1
+Version: 1.2.2
 Summary: OptiMask: extracting the largest (non-contiguous) submatrix without NaN
 Home-page: https://github.com/CyrilJl/optimask
 Author: Cyril Joly
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: pandas
-Requires-Dist: cython
 
 # <img src="https://raw.githubusercontent.com/CyrilJl/OptiMask/main/docs/source/_static/icon.svg" alt="Logo OptiMask" width="35" height="35"> OptiMask: Efficient NaN Data Removal in Python
 
 [![PyPI Version](https://img.shields.io/pypi/v/optimask.svg)](https://pypi.org/project/optimask/) [![Conda Version](https://img.shields.io/conda/vn/conda-forge/optimask.svg)](https://anaconda.org/conda-forge/optimask)
 
 ## Introduction
```

### Comparing `optimask-1.2.1/README.md` & `optimask-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `optimask-1.2.1/optimask/_misc.py` & `optimask-1.2.2/optimask/_misc.py`

 * *Files identical despite different names*

### Comparing `optimask-1.2.1/optimask/_optimask.py` & `optimask-1.2.2/optimask/_optimask.py`

 * *Files identical despite different names*

### Comparing `optimask-1.2.1/optimask/optimask_cython.c` & `optimask-1.2.2/optimask/optimask_cython.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,37 +1,9 @@
 /* Generated by Cython 3.0.10 */
 
-/* BEGIN: Cython Metadata
-{
-    "distutils": {
-        "depends": [
-            "/opt/hostedtoolcache/Python/3.12.3/x64/lib/python3.12/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/opt/hostedtoolcache/Python/3.12.3/x64/lib/python3.12/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/opt/hostedtoolcache/Python/3.12.3/x64/lib/python3.12/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/opt/hostedtoolcache/Python/3.12.3/x64/lib/python3.12/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/opt/hostedtoolcache/Python/3.12.3/x64/lib/python3.12/site-packages/numpy/core/include/numpy/ufuncobject.h"
-        ],
-        "extra_compile_args": [
-            "-std=c99"
-        ],
-        "extra_link_args": [
-            "-std=c99"
-        ],
-        "include_dirs": [
-            "/opt/hostedtoolcache/Python/3.12.3/x64/lib/python3.12/site-packages/numpy/core/include"
-        ],
-        "name": "optimask.optimask_cython",
-        "sources": [
-            "optimask/optimask_cython.pyx"
-        ]
-    },
-    "module_name": "optimask.optimask_cython"
-}
-END: Cython Metadata */
-
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #if defined(CYTHON_LIMITED_API) && 0
   #ifndef Py_LIMITED_API
     #if CYTHON_LIMITED_API+0 > 0x03030000
       #define Py_LIMITED_API CYTHON_LIMITED_API
```

### Comparing `optimask-1.2.1/optimask/optimask_cython.pyx` & `optimask-1.2.2/optimask/optimask_cython.pyx`

 * *Files identical despite different names*

### Comparing `optimask-1.2.1/optimask.egg-info/PKG-INFO` & `optimask-1.2.2/optimask.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: optimask
-Version: 1.2.1
+Version: 1.2.2
 Summary: OptiMask: extracting the largest (non-contiguous) submatrix without NaN
 Home-page: https://github.com/CyrilJl/optimask
 Author: Cyril Joly
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: pandas
-Requires-Dist: cython
 
 # <img src="https://raw.githubusercontent.com/CyrilJl/OptiMask/main/docs/source/_static/icon.svg" alt="Logo OptiMask" width="35" height="35"> OptiMask: Efficient NaN Data Removal in Python
 
 [![PyPI Version](https://img.shields.io/pypi/v/optimask.svg)](https://pypi.org/project/optimask/) [![Conda Version](https://img.shields.io/conda/vn/conda-forge/optimask.svg)](https://anaconda.org/conda-forge/optimask)
 
 ## Introduction
```

### Comparing `optimask-1.2.1/tests/test_optimask.py` & `optimask-1.2.2/tests/test_optimask.py`

 * *Files identical despite different names*

