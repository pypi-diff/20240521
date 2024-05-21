# Comparing `tmp/optimask-1.1.1b0.tar.gz` & `tmp/optimask-1.1.1rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optimask-1.1.1b0.tar", last modified: Tue May 21 09:58:43 2024, max compression
+gzip compressed data, was "optimask-1.1.1rc0.tar", last modified: Tue May 21 10:07:01 2024, max compression
```

## Comparing `optimask-1.1.1b0.tar` & `optimask-1.1.1rc0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:58:43.455798 optimask-1.1.1b0/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-21 09:58:24.000000 optimask-1.1.1b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-05-21 09:58:43.455798 optimask-1.1.1b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-05-21 09:58:24.000000 optimask-1.1.1b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:58:43.451798 optimask-1.1.1b0/optimask/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-21 09:58:24.000000 optimask-1.1.1b0/optimask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-21 09:58:24.000000 optimask-1.1.1b0/optimask/_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     7028 2024-05-21 09:58:24.000000 optimask-1.1.1b0/optimask/_optimask.py
--rw-r--r--   0 runner    (1001) docker     (127)  1134944 2024-05-21 09:58:37.000000 optimask-1.1.1b0/optimask/optimask_cython.c
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-21 09:58:24.000000 optimask-1.1.1b0/optimask/optimask_cython.pyx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:58:43.455798 optimask-1.1.1b0/optimask.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-05-21 09:58:43.000000 optimask-1.1.1b0/optimask.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-21 09:58:43.000000 optimask-1.1.1b0/optimask.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 09:58:43.000000 optimask-1.1.1b0/optimask.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-21 09:58:43.000000 optimask-1.1.1b0/optimask.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-21 09:58:43.000000 optimask-1.1.1b0/optimask.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 09:58:43.455798 optimask-1.1.1b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-21 09:58:24.000000 optimask-1.1.1b0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:58:43.455798 optimask-1.1.1b0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-21 09:58:24.000000 optimask-1.1.1b0/tests/test_optimask.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:07:01.170715 optimask-1.1.1rc0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-21 10:06:38.000000 optimask-1.1.1rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-05-21 10:07:01.170715 optimask-1.1.1rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-05-21 10:06:38.000000 optimask-1.1.1rc0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:07:01.166715 optimask-1.1.1rc0/optimask/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-21 10:06:38.000000 optimask-1.1.1rc0/optimask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-21 10:06:38.000000 optimask-1.1.1rc0/optimask/_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7028 2024-05-21 10:06:38.000000 optimask-1.1.1rc0/optimask/_optimask.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1134944 2024-05-21 10:06:54.000000 optimask-1.1.1rc0/optimask/optimask_cython.c
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-21 10:06:38.000000 optimask-1.1.1rc0/optimask/optimask_cython.pyx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:07:01.170715 optimask-1.1.1rc0/optimask.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-05-21 10:07:01.000000 optimask-1.1.1rc0/optimask.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-21 10:07:01.000000 optimask-1.1.1rc0/optimask.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 10:07:01.000000 optimask-1.1.1rc0/optimask.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-21 10:07:01.000000 optimask-1.1.1rc0/optimask.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-21 10:07:01.000000 optimask-1.1.1rc0/optimask.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 10:07:01.170715 optimask-1.1.1rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-21 10:06:38.000000 optimask-1.1.1rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:07:01.170715 optimask-1.1.1rc0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-21 10:06:38.000000 optimask-1.1.1rc0/tests/test_optimask.py
```

### Comparing `optimask-1.1.1b0/LICENSE` & `optimask-1.1.1rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `optimask-1.1.1b0/PKG-INFO` & `optimask-1.1.1rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimask
-Version: 1.1.1b0
+Version: 1.1.1rc0
 Summary: OptiMask: extracting the largest (non-contiguous) submatrix without NaN
 Home-page: https://github.com/CyrilJl/optimask
 Author: Cyril Joly
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `optimask-1.1.1b0/README.md` & `optimask-1.1.1rc0/README.md`

 * *Files identical despite different names*

### Comparing `optimask-1.1.1b0/optimask/_misc.py` & `optimask-1.1.1rc0/optimask/_misc.py`

 * *Files identical despite different names*

### Comparing `optimask-1.1.1b0/optimask/_optimask.py` & `optimask-1.1.1rc0/optimask/_optimask.py`

 * *Files identical despite different names*

### Comparing `optimask-1.1.1b0/optimask/optimask_cython.c` & `optimask-1.1.1rc0/optimask/optimask_cython.c`

 * *Files identical despite different names*

### Comparing `optimask-1.1.1b0/optimask/optimask_cython.pyx` & `optimask-1.1.1rc0/optimask/optimask_cython.pyx`

 * *Files identical despite different names*

### Comparing `optimask-1.1.1b0/optimask.egg-info/PKG-INFO` & `optimask-1.1.1rc0/optimask.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimask
-Version: 1.1.1b0
+Version: 1.1.1rc0
 Summary: OptiMask: extracting the largest (non-contiguous) submatrix without NaN
 Home-page: https://github.com/CyrilJl/optimask
 Author: Cyril Joly
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `optimask-1.1.1b0/setup.py` & `optimask-1.1.1rc0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import numpy as np
 from setuptools import Extension, find_packages, setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name='optimask',
-      version='1.1.1b',
+      version='1.1.1c',
       packages=find_packages(),
       install_requires=['numpy', 'pandas'],
       description="OptiMask: extracting the largest (non-contiguous) submatrix without NaN",
       long_description_content_type='text/markdown',
       long_description=long_description,
       author='Cyril Joly',
       license='MIT',
       url='https://github.com/CyrilJl/optimask',
       classifiers=['License :: OSI Approved :: MIT License'],
       ext_modules=[Extension("optimask.optimask_cython",
                              sources=["optimask/optimask_cython.pyx"],
                              include_dirs=[np.get_include()])],
-      package_data={'optimask': ['*.pxd', '*.pyx', '*.c']}
+      package_data={'optimask': ['*.pxd', '*.pyx', '*.c']},
+      extra_compile_args=["-std=c99"]
       )
```

### Comparing `optimask-1.1.1b0/tests/test_optimask.py` & `optimask-1.1.1rc0/tests/test_optimask.py`

 * *Files identical despite different names*
