# Comparing `tmp/optimask-1.2.tar.gz` & `tmp/optimask-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optimask-1.2.tar", last modified: Tue May 21 14:31:13 2024, max compression
+gzip compressed data, was "optimask-1.2.1.tar", last modified: Tue May 21 14:51:10 2024, max compression
```

## Comparing `optimask-1.2.tar` & `optimask-1.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:31:13.729851 optimask-1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-21 14:31:00.000000 optimask-1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-21 14:31:00.000000 optimask-1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-05-21 14:31:13.729851 optimask-1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-05-21 14:31:00.000000 optimask-1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:31:13.725851 optimask-1.2/optimask/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-21 14:31:00.000000 optimask-1.2/optimask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-21 14:31:00.000000 optimask-1.2/optimask/_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     6983 2024-05-21 14:31:00.000000 optimask-1.2/optimask/_optimask.py
--rw-r--r--   0 runner    (1001) docker     (127)   427048 2024-05-21 14:31:13.000000 optimask-1.2/optimask/optimask_cython.c
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-21 14:31:00.000000 optimask-1.2/optimask/optimask_cython.pyx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:31:13.729851 optimask-1.2/optimask.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-05-21 14:31:13.000000 optimask-1.2/optimask.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-21 14:31:13.000000 optimask-1.2/optimask.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 14:31:13.000000 optimask-1.2/optimask.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-21 14:31:13.000000 optimask-1.2/optimask.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-21 14:31:13.000000 optimask-1.2/optimask.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 14:31:13.729851 optimask-1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-21 14:31:00.000000 optimask-1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:31:13.729851 optimask-1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-21 14:31:00.000000 optimask-1.2/tests/test_optimask.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:51:10.620873 optimask-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-21 14:50:57.000000 optimask-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-21 14:50:57.000000 optimask-1.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-05-21 14:51:10.620873 optimask-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-05-21 14:50:57.000000 optimask-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:51:10.620873 optimask-1.2.1/optimask/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-21 14:50:57.000000 optimask-1.2.1/optimask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-21 14:50:57.000000 optimask-1.2.1/optimask/_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7017 2024-05-21 14:50:57.000000 optimask-1.2.1/optimask/_optimask.py
+-rw-r--r--   0 runner    (1001) docker     (127)   427048 2024-05-21 14:51:10.000000 optimask-1.2.1/optimask/optimask_cython.c
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-21 14:50:57.000000 optimask-1.2.1/optimask/optimask_cython.pyx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:51:10.620873 optimask-1.2.1/optimask.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-05-21 14:51:10.000000 optimask-1.2.1/optimask.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-21 14:51:10.000000 optimask-1.2.1/optimask.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 14:51:10.000000 optimask-1.2.1/optimask.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-21 14:51:10.000000 optimask-1.2.1/optimask.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-21 14:51:10.000000 optimask-1.2.1/optimask.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 14:51:10.620873 optimask-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-05-21 14:50:57.000000 optimask-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:51:10.620873 optimask-1.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-21 14:50:57.000000 optimask-1.2.1/tests/test_optimask.py
```

### Comparing `optimask-1.2/LICENSE` & `optimask-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `optimask-1.2/PKG-INFO` & `optimask-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimask
-Version: 1.2
+Version: 1.2.1
 Summary: OptiMask: extracting the largest (non-contiguous) submatrix without NaN
 Home-page: https://github.com/CyrilJl/optimask
 Author: Cyril Joly
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `optimask-1.2/README.md` & `optimask-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `optimask-1.2/optimask/_misc.py` & `optimask-1.2.1/optimask/_misc.py`

 * *Files identical despite different names*

### Comparing `optimask-1.2/optimask/_optimask.py` & `optimask-1.2.1/optimask/_optimask.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,16 +74,16 @@
         return i0, heights[i0], areas[i0]
 
     @classmethod
     def _is_pareto_ordered(cls, hx, hy):
         return is_decreasing(hx) and is_decreasing(hy)
 
     def _trial(self, rng, m_nan, n_nan, iy, ix, m, n):
-        p_rows = rng.permutation(m_nan)
-        p_cols = rng.permutation(n_nan)
+        p_rows = rng.permutation(m_nan).astype(np.int64)
+        p_cols = rng.permutation(n_nan).astype(np.int64)
         iy_trial = permutation_index(p_rows)[iy]
         ix_trial = permutation_index(p_cols)[ix]
 
         step = 0
         h0, h1 = groupby_max(iy_trial, ix_trial, m_nan), groupby_max(ix_trial, iy_trial, n_nan)
         while (not self._is_pareto_ordered(h0, h1)) and (step < self.max_steps):
             axis = (step % 2)
```

### Comparing `optimask-1.2/optimask/optimask_cython.c` & `optimask-1.2.1/optimask/optimask_cython.c`

 * *Files identical despite different names*

### Comparing `optimask-1.2/optimask/optimask_cython.pyx` & `optimask-1.2.1/optimask/optimask_cython.pyx`

 * *Files identical despite different names*

### Comparing `optimask-1.2/optimask.egg-info/PKG-INFO` & `optimask-1.2.1/optimask.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimask
-Version: 1.2
+Version: 1.2.1
 Summary: OptiMask: extracting the largest (non-contiguous) submatrix without NaN
 Home-page: https://github.com/CyrilJl/optimask
 Author: Cyril Joly
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `optimask-1.2/setup.py` & `optimask-1.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import Extension, find_packages, setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='optimask',
-    version='1.2',
+    version='1.2.1',
     packages=find_packages(),
     install_requires=['numpy', 'pandas', 'cython'],
     description="OptiMask: extracting the largest (non-contiguous) submatrix without NaN",
     long_description_content_type='text/markdown',
     long_description=long_description,
     author='Cyril Joly',
     license='MIT',
```

### Comparing `optimask-1.2/tests/test_optimask.py` & `optimask-1.2.1/tests/test_optimask.py`

 * *Files identical despite different names*

