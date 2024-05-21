# Comparing `tmp/pyrheed-1.0.8rc0.tar.gz` & `tmp/pyrheed-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrheed-1.0.8rc0.tar", last modified: Tue May 21 05:22:04 2024, max compression
+gzip compressed data, was "pyrheed-1.0.9.tar", last modified: Tue May 21 05:24:54 2024, max compression
```

## Comparing `pyrheed-1.0.8rc0.tar` & `pyrheed-1.0.9.tar`

### file list

```diff
@@ -1,44 +1,52 @@
-drwxr-xr-x   0 yuuxiang   (504) staff       (20)        0 2024-05-21 05:22:04.575470 pyrheed-1.0.8rc0/
--rw-r--r--   0 yuuxiang   (504) staff       (20)     1059 2024-05-19 00:11:40.000000 pyrheed-1.0.8rc0/LICENSE
--rw-r--r--   0 yuuxiang   (504) staff       (20)     8458 2024-05-21 05:22:04.575098 pyrheed-1.0.8rc0/PKG-INFO
--rw-r--r--   0 yuuxiang   (504) staff       (20)     7352 2024-05-21 03:40:07.000000 pyrheed-1.0.8rc0/README.md
--rw-r--r--   0 yuuxiang   (504) staff       (20)      952 2024-05-21 05:21:57.000000 pyrheed-1.0.8rc0/pyproject.toml
--rw-r--r--   0 yuuxiang   (504) staff       (20)       38 2024-05-21 05:22:04.575548 pyrheed-1.0.8rc0/setup.cfg
-drwxr-xr-x   0 yuuxiang   (504) staff       (20)        0 2024-05-21 05:22:04.561960 pyrheed-1.0.8rc0/src/
-drwxr-xr-x   0 yuuxiang   (504) staff       (20)        0 2024-05-21 05:22:04.572516 pyrheed-1.0.8rc0/src/PyRHEED.egg-info/
--rw-r--r--   0 yuuxiang   (504) staff       (20)     8458 2024-05-21 05:22:04.000000 pyrheed-1.0.8rc0/src/PyRHEED.egg-info/PKG-INFO
--rw-r--r--   0 yuuxiang   (504) staff       (20)     1036 2024-05-21 05:22:04.000000 pyrheed-1.0.8rc0/src/PyRHEED.egg-info/SOURCES.txt
--rw-r--r--   0 yuuxiang   (504) staff       (20)        1 2024-05-21 05:22:04.000000 pyrheed-1.0.8rc0/src/PyRHEED.egg-info/dependency_links.txt
--rw-r--r--   0 yuuxiang   (504) staff       (20)      305 2024-05-21 05:22:04.000000 pyrheed-1.0.8rc0/src/PyRHEED.egg-info/requires.txt
--rw-r--r--   0 yuuxiang   (504) staff       (20)        8 2024-05-21 05:22:04.000000 pyrheed-1.0.8rc0/src/PyRHEED.egg-info/top_level.txt
-drwxr-xr-x   0 yuuxiang   (504) staff       (20)        0 2024-05-21 05:22:04.572066 pyrheed-1.0.8rc0/src/pyrheed/
--rw-r--r--   0 yuuxiang   (504) staff       (20)        0 2024-05-21 04:49:27.000000 pyrheed-1.0.8rc0/src/pyrheed/__init__.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)     9719 2024-05-21 05:21:52.000000 pyrheed-1.0.8rc0/src/pyrheed/__main__.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)     5666 2024-05-21 04:53:36.000000 pyrheed-1.0.8rc0/src/pyrheed/bar_chart.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)     7381 2024-05-21 03:38:01.000000 pyrheed-1.0.8rc0/src/pyrheed/boundary_statistics.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)    44314 2024-05-21 04:55:03.000000 pyrheed-1.0.8rc0/src/pyrheed/broadening.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)     1725 2024-05-21 03:38:01.000000 pyrheed-1.0.8rc0/src/pyrheed/browser.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)    27635 2024-05-21 03:38:01.000000 pyrheed-1.0.8rc0/src/pyrheed/canvas.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)     2833 2024-05-21 03:38:01.000000 pyrheed-1.0.8rc0/src/pyrheed/configuration.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)     2261 2024-05-21 03:38:01.000000 pyrheed-1.0.8rc0/src/pyrheed/cursor.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)    36281 2024-05-21 04:55:45.000000 pyrheed-1.0.8rc0/src/pyrheed/generate_report.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)    65774 2024-05-21 04:58:41.000000 pyrheed-1.0.8rc0/src/pyrheed/gmm.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)    22311 2024-05-21 03:38:01.000000 pyrheed-1.0.8rc0/src/pyrheed/graph_3D_surface.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)    27121 2024-05-21 04:59:20.000000 pyrheed-1.0.8rc0/src/pyrheed/kikuchi.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)    17671 2024-05-21 04:59:42.000000 pyrheed-1.0.8rc0/src/pyrheed/manual_fit.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)    50948 2024-05-21 03:38:01.000000 pyrheed-1.0.8rc0/src/pyrheed/my_widgets.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)    18518 2024-05-21 03:38:01.000000 pyrheed-1.0.8rc0/src/pyrheed/plot_chart.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)    12078 2024-05-21 03:38:01.000000 pyrheed-1.0.8rc0/src/pyrheed/preference.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)   102534 2024-05-21 05:00:41.000000 pyrheed-1.0.8rc0/src/pyrheed/process.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)     3481 2024-05-21 03:38:01.000000 pyrheed-1.0.8rc0/src/pyrheed/process_monitor.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)    17718 2024-05-21 05:00:51.000000 pyrheed-1.0.8rc0/src/pyrheed/profile_chart.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)    15838 2024-05-21 03:38:01.000000 pyrheed-1.0.8rc0/src/pyrheed/properties.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)    33571 2024-05-21 05:01:10.000000 pyrheed-1.0.8rc0/src/pyrheed/reciprocal_space_mapping.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)     2508 2024-05-21 03:38:01.000000 pyrheed-1.0.8rc0/src/pyrheed/regularization.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)    24148 2024-05-21 05:02:29.000000 pyrheed-1.0.8rc0/src/pyrheed/scenario.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)     7759 2024-05-21 03:38:01.000000 pyrheed-1.0.8rc0/src/pyrheed/scipy_test.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)   147826 2024-05-21 05:03:10.000000 pyrheed-1.0.8rc0/src/pyrheed/simulate_RHEED.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)    21784 2024-05-21 05:03:18.000000 pyrheed-1.0.8rc0/src/pyrheed/statistical_factor.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)     7998 2024-05-21 05:03:34.000000 pyrheed-1.0.8rc0/src/pyrheed/translational_antiphase_domain.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)    47989 2024-05-21 05:04:15.000000 pyrheed-1.0.8rc0/src/pyrheed/window.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)     4087 2024-05-21 03:38:01.000000 pyrheed-1.0.8rc0/src/pyrheed/write_scenario.py
+drwxr-xr-x   0 yuuxiang   (504) staff       (20)        0 2024-05-21 05:24:54.245382 pyrheed-1.0.9/
+-rw-r--r--   0 yuuxiang   (504) staff       (20)     1059 2024-05-19 00:11:40.000000 pyrheed-1.0.9/LICENSE
+-rw-r--r--   0 yuuxiang   (504) staff       (20)     8455 2024-05-21 05:24:54.245029 pyrheed-1.0.9/PKG-INFO
+-rw-r--r--   0 yuuxiang   (504) staff       (20)     7352 2024-05-21 03:40:07.000000 pyrheed-1.0.9/README.md
+-rw-r--r--   0 yuuxiang   (504) staff       (20)      951 2024-05-21 05:24:47.000000 pyrheed-1.0.9/pyproject.toml
+-rw-r--r--   0 yuuxiang   (504) staff       (20)       38 2024-05-21 05:24:54.245451 pyrheed-1.0.9/setup.cfg
+drwxr-xr-x   0 yuuxiang   (504) staff       (20)        0 2024-05-21 05:24:54.232293 pyrheed-1.0.9/src/
+drwxr-xr-x   0 yuuxiang   (504) staff       (20)        0 2024-05-21 05:24:54.244658 pyrheed-1.0.9/src/PyRHEED.egg-info/
+-rw-r--r--   0 yuuxiang   (504) staff       (20)     8455 2024-05-21 05:24:54.000000 pyrheed-1.0.9/src/PyRHEED.egg-info/PKG-INFO
+-rw-r--r--   0 yuuxiang   (504) staff       (20)     1173 2024-05-21 05:24:54.000000 pyrheed-1.0.9/src/PyRHEED.egg-info/SOURCES.txt
+-rw-r--r--   0 yuuxiang   (504) staff       (20)        1 2024-05-21 05:24:54.000000 pyrheed-1.0.9/src/PyRHEED.egg-info/dependency_links.txt
+-rw-r--r--   0 yuuxiang   (504) staff       (20)      305 2024-05-21 05:24:54.000000 pyrheed-1.0.9/src/PyRHEED.egg-info/requires.txt
+-rw-r--r--   0 yuuxiang   (504) staff       (20)        8 2024-05-21 05:24:54.000000 pyrheed-1.0.9/src/PyRHEED.egg-info/top_level.txt
+drwxr-xr-x   0 yuuxiang   (504) staff       (20)        0 2024-05-21 05:24:54.243229 pyrheed-1.0.9/src/pyrheed/
+-rw-r--r--   0 yuuxiang   (504) staff       (20)        0 2024-05-21 04:49:27.000000 pyrheed-1.0.9/src/pyrheed/__init__.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)     9719 2024-05-21 05:21:52.000000 pyrheed-1.0.9/src/pyrheed/__main__.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)     5666 2024-05-21 04:53:36.000000 pyrheed-1.0.9/src/pyrheed/bar_chart.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)     7381 2024-05-21 03:38:01.000000 pyrheed-1.0.9/src/pyrheed/boundary_statistics.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)    44314 2024-05-21 04:55:03.000000 pyrheed-1.0.9/src/pyrheed/broadening.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)     1725 2024-05-21 03:38:01.000000 pyrheed-1.0.9/src/pyrheed/browser.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)    27635 2024-05-21 03:38:01.000000 pyrheed-1.0.9/src/pyrheed/canvas.py
+drwxr-xr-x   0 yuuxiang   (504) staff       (20)        0 2024-05-21 05:24:54.243507 pyrheed-1.0.9/src/pyrheed/configuration/
+-rw-r--r--   0 yuuxiang   (504) staff       (20)        0 2024-05-21 05:23:11.000000 pyrheed-1.0.9/src/pyrheed/configuration/__init__.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)     2833 2024-05-21 03:38:01.000000 pyrheed-1.0.9/src/pyrheed/configuration.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)     2261 2024-05-21 03:38:01.000000 pyrheed-1.0.9/src/pyrheed/cursor.py
+drwxr-xr-x   0 yuuxiang   (504) staff       (20)        0 2024-05-21 05:24:54.243743 pyrheed-1.0.9/src/pyrheed/data/
+-rw-r--r--   0 yuuxiang   (504) staff       (20)        0 2024-05-21 05:23:09.000000 pyrheed-1.0.9/src/pyrheed/data/__init__.py
+drwxr-xr-x   0 yuuxiang   (504) staff       (20)        0 2024-05-21 05:24:54.243987 pyrheed-1.0.9/src/pyrheed/data/files/
+-rw-r--r--   0 yuuxiang   (504) staff       (20)        0 2024-05-21 05:23:13.000000 pyrheed-1.0.9/src/pyrheed/data/files/__init__.py
+drwxr-xr-x   0 yuuxiang   (504) staff       (20)        0 2024-05-21 05:24:54.244219 pyrheed-1.0.9/src/pyrheed/data/icons/
+-rw-r--r--   0 yuuxiang   (504) staff       (20)        0 2024-05-21 05:23:15.000000 pyrheed-1.0.9/src/pyrheed/data/icons/__init__.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)    36281 2024-05-21 04:55:45.000000 pyrheed-1.0.9/src/pyrheed/generate_report.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)    65774 2024-05-21 04:58:41.000000 pyrheed-1.0.9/src/pyrheed/gmm.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)    22311 2024-05-21 03:38:01.000000 pyrheed-1.0.9/src/pyrheed/graph_3D_surface.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)    27121 2024-05-21 04:59:20.000000 pyrheed-1.0.9/src/pyrheed/kikuchi.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)    17671 2024-05-21 04:59:42.000000 pyrheed-1.0.9/src/pyrheed/manual_fit.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)    50948 2024-05-21 03:38:01.000000 pyrheed-1.0.9/src/pyrheed/my_widgets.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)    18518 2024-05-21 03:38:01.000000 pyrheed-1.0.9/src/pyrheed/plot_chart.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)    12078 2024-05-21 03:38:01.000000 pyrheed-1.0.9/src/pyrheed/preference.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)   102534 2024-05-21 05:00:41.000000 pyrheed-1.0.9/src/pyrheed/process.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)     3481 2024-05-21 03:38:01.000000 pyrheed-1.0.9/src/pyrheed/process_monitor.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)    17718 2024-05-21 05:00:51.000000 pyrheed-1.0.9/src/pyrheed/profile_chart.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)    15838 2024-05-21 03:38:01.000000 pyrheed-1.0.9/src/pyrheed/properties.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)    33571 2024-05-21 05:01:10.000000 pyrheed-1.0.9/src/pyrheed/reciprocal_space_mapping.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)     2508 2024-05-21 03:38:01.000000 pyrheed-1.0.9/src/pyrheed/regularization.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)    24148 2024-05-21 05:02:29.000000 pyrheed-1.0.9/src/pyrheed/scenario.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)     7759 2024-05-21 03:38:01.000000 pyrheed-1.0.9/src/pyrheed/scipy_test.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)   147826 2024-05-21 05:03:10.000000 pyrheed-1.0.9/src/pyrheed/simulate_RHEED.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)    21784 2024-05-21 05:03:18.000000 pyrheed-1.0.9/src/pyrheed/statistical_factor.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)     7998 2024-05-21 05:03:34.000000 pyrheed-1.0.9/src/pyrheed/translational_antiphase_domain.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)    47989 2024-05-21 05:04:15.000000 pyrheed-1.0.9/src/pyrheed/window.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)     4087 2024-05-21 03:38:01.000000 pyrheed-1.0.9/src/pyrheed/write_scenario.py
```

### Comparing `pyrheed-1.0.8rc0/LICENSE` & `pyrheed-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrheed-1.0.8rc0/PKG-INFO` & `pyrheed-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyRHEED
-Version: 1.0.8rc0
+Version: 1.0.9
 Summary: A python package for RHEED data analysis and simulation
 Author-email: Yu Xiang <yux1991@gmail.com>
 Project-URL: Homepage, https://github.com/yux1991/PyRHEED
 Project-URL: Issues, https://github.com/yux1991/PyRHEED/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyrheed-1.0.8rc0/README.md` & `pyrheed-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pyrheed-1.0.8rc0/pyproject.toml` & `pyrheed-1.0.9/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "PyRHEED"
-version = "1.0.8c"
+version = "1.0.9"
 authors = [
   { name="Yu Xiang", email="yux1991@gmail.com" },
 ]
 description = "A python package for RHEED data analysis and simulation"
 readme = "README.md"
 requires-python = ">=3.12"
 classifiers = [
```

### Comparing `pyrheed-1.0.8rc0/src/PyRHEED.egg-info/PKG-INFO` & `pyrheed-1.0.9/src/PyRHEED.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyRHEED
-Version: 1.0.8rc0
+Version: 1.0.9
 Summary: A python package for RHEED data analysis and simulation
 Author-email: Yu Xiang <yux1991@gmail.com>
 Project-URL: Homepage, https://github.com/yux1991/PyRHEED
 Project-URL: Issues, https://github.com/yux1991/PyRHEED/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyrheed-1.0.8rc0/src/PyRHEED.egg-info/SOURCES.txt` & `pyrheed-1.0.9/src/PyRHEED.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -31,8 +31,12 @@
 src/pyrheed/regularization.py
 src/pyrheed/scenario.py
 src/pyrheed/scipy_test.py
 src/pyrheed/simulate_RHEED.py
 src/pyrheed/statistical_factor.py
 src/pyrheed/translational_antiphase_domain.py
 src/pyrheed/window.py
-src/pyrheed/write_scenario.py
+src/pyrheed/write_scenario.py
+src/pyrheed/configuration/__init__.py
+src/pyrheed/data/__init__.py
+src/pyrheed/data/files/__init__.py
+src/pyrheed/data/icons/__init__.py
```

### Comparing `pyrheed-1.0.8rc0/src/pyrheed/__main__.py` & `pyrheed-1.0.9/src/pyrheed/__main__.py`

 * *Files identical despite different names*

### Comparing `pyrheed-1.0.8rc0/src/pyrheed/bar_chart.py` & `pyrheed-1.0.9/src/pyrheed/bar_chart.py`

 * *Files identical despite different names*

### Comparing `pyrheed-1.0.8rc0/src/pyrheed/boundary_statistics.py` & `pyrheed-1.0.9/src/pyrheed/boundary_statistics.py`

 * *Files identical despite different names*

### Comparing `pyrheed-1.0.8rc0/src/pyrheed/broadening.py` & `pyrheed-1.0.9/src/pyrheed/broadening.py`

 * *Files identical despite different names*

### Comparing `pyrheed-1.0.8rc0/src/pyrheed/browser.py` & `pyrheed-1.0.9/src/pyrheed/browser.py`

 * *Files identical despite different names*

### Comparing `pyrheed-1.0.8rc0/src/pyrheed/canvas.py` & `pyrheed-1.0.9/src/pyrheed/canvas.py`

 * *Files identical despite different names*

### Comparing `pyrheed-1.0.8rc0/src/pyrheed/configuration.py` & `pyrheed-1.0.9/src/pyrheed/configuration.py`

 * *Files identical despite different names*

### Comparing `pyrheed-1.0.8rc0/src/pyrheed/cursor.py` & `pyrheed-1.0.9/src/pyrheed/cursor.py`

 * *Files identical despite different names*

### Comparing `pyrheed-1.0.8rc0/src/pyrheed/generate_report.py` & `pyrheed-1.0.9/src/pyrheed/generate_report.py`

 * *Files identical despite different names*

### Comparing `pyrheed-1.0.8rc0/src/pyrheed/gmm.py` & `pyrheed-1.0.9/src/pyrheed/gmm.py`

 * *Files identical despite different names*

### Comparing `pyrheed-1.0.8rc0/src/pyrheed/graph_3D_surface.py` & `pyrheed-1.0.9/src/pyrheed/graph_3D_surface.py`

 * *Files identical despite different names*

### Comparing `pyrheed-1.0.8rc0/src/pyrheed/kikuchi.py` & `pyrheed-1.0.9/src/pyrheed/kikuchi.py`

 * *Files identical despite different names*

### Comparing `pyrheed-1.0.8rc0/src/pyrheed/manual_fit.py` & `pyrheed-1.0.9/src/pyrheed/manual_fit.py`

 * *Files identical despite different names*

### Comparing `pyrheed-1.0.8rc0/src/pyrheed/my_widgets.py` & `pyrheed-1.0.9/src/pyrheed/my_widgets.py`

 * *Files identical despite different names*

### Comparing `pyrheed-1.0.8rc0/src/pyrheed/plot_chart.py` & `pyrheed-1.0.9/src/pyrheed/plot_chart.py`

 * *Files identical despite different names*

### Comparing `pyrheed-1.0.8rc0/src/pyrheed/preference.py` & `pyrheed-1.0.9/src/pyrheed/preference.py`

 * *Files identical despite different names*

### Comparing `pyrheed-1.0.8rc0/src/pyrheed/process.py` & `pyrheed-1.0.9/src/pyrheed/process.py`

 * *Files identical despite different names*

### Comparing `pyrheed-1.0.8rc0/src/pyrheed/process_monitor.py` & `pyrheed-1.0.9/src/pyrheed/process_monitor.py`

 * *Files identical despite different names*

### Comparing `pyrheed-1.0.8rc0/src/pyrheed/profile_chart.py` & `pyrheed-1.0.9/src/pyrheed/profile_chart.py`

 * *Files identical despite different names*

### Comparing `pyrheed-1.0.8rc0/src/pyrheed/properties.py` & `pyrheed-1.0.9/src/pyrheed/properties.py`

 * *Files identical despite different names*

### Comparing `pyrheed-1.0.8rc0/src/pyrheed/reciprocal_space_mapping.py` & `pyrheed-1.0.9/src/pyrheed/reciprocal_space_mapping.py`

 * *Files identical despite different names*

### Comparing `pyrheed-1.0.8rc0/src/pyrheed/regularization.py` & `pyrheed-1.0.9/src/pyrheed/regularization.py`

 * *Files identical despite different names*

### Comparing `pyrheed-1.0.8rc0/src/pyrheed/scenario.py` & `pyrheed-1.0.9/src/pyrheed/scenario.py`

 * *Files identical despite different names*

### Comparing `pyrheed-1.0.8rc0/src/pyrheed/scipy_test.py` & `pyrheed-1.0.9/src/pyrheed/scipy_test.py`

 * *Files identical despite different names*

### Comparing `pyrheed-1.0.8rc0/src/pyrheed/simulate_RHEED.py` & `pyrheed-1.0.9/src/pyrheed/simulate_RHEED.py`

 * *Files identical despite different names*

### Comparing `pyrheed-1.0.8rc0/src/pyrheed/statistical_factor.py` & `pyrheed-1.0.9/src/pyrheed/statistical_factor.py`

 * *Files identical despite different names*

### Comparing `pyrheed-1.0.8rc0/src/pyrheed/translational_antiphase_domain.py` & `pyrheed-1.0.9/src/pyrheed/translational_antiphase_domain.py`

 * *Files identical despite different names*

### Comparing `pyrheed-1.0.8rc0/src/pyrheed/window.py` & `pyrheed-1.0.9/src/pyrheed/window.py`

 * *Files identical despite different names*

### Comparing `pyrheed-1.0.8rc0/src/pyrheed/write_scenario.py` & `pyrheed-1.0.9/src/pyrheed/write_scenario.py`

 * *Files identical despite different names*
