# Comparing `tmp/pyrheed-1.0.1.tar.gz` & `tmp/pyrheed-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrheed-1.0.1.tar", last modified: Tue May 21 04:08:25 2024, max compression
+gzip compressed data, was "pyrheed-1.0.2.tar", last modified: Tue May 21 04:21:55 2024, max compression
```

## Comparing `pyrheed-1.0.1.tar` & `pyrheed-1.0.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 yuuxiang   (504) staff       (20)        0 2024-05-21 04:08:25.994844 pyrheed-1.0.1/
--rw-r--r--   0 yuuxiang   (504) staff       (20)     1059 2024-05-19 00:11:40.000000 pyrheed-1.0.1/LICENSE
--rw-r--r--   0 yuuxiang   (504) staff       (20)     8455 2024-05-21 04:08:25.994452 pyrheed-1.0.1/PKG-INFO
--rw-r--r--   0 yuuxiang   (504) staff       (20)     7352 2024-05-21 03:40:07.000000 pyrheed-1.0.1/README.md
--rw-r--r--   0 yuuxiang   (504) staff       (20)      951 2024-05-21 04:07:45.000000 pyrheed-1.0.1/pyproject.toml
--rw-r--r--   0 yuuxiang   (504) staff       (20)       38 2024-05-21 04:08:25.994900 pyrheed-1.0.1/setup.cfg
-drwxr-xr-x   0 yuuxiang   (504) staff       (20)        0 2024-05-21 04:08:25.978538 pyrheed-1.0.1/src/
-drwxr-xr-x   0 yuuxiang   (504) staff       (20)        0 2024-05-21 04:08:25.993946 pyrheed-1.0.1/src/PyRHEED.egg-info/
--rw-r--r--   0 yuuxiang   (504) staff       (20)     8455 2024-05-21 04:08:25.000000 pyrheed-1.0.1/src/PyRHEED.egg-info/PKG-INFO
--rw-r--r--   0 yuuxiang   (504) staff       (20)     1032 2024-05-21 04:08:25.000000 pyrheed-1.0.1/src/PyRHEED.egg-info/SOURCES.txt
--rw-r--r--   0 yuuxiang   (504) staff       (20)        1 2024-05-21 04:08:25.000000 pyrheed-1.0.1/src/PyRHEED.egg-info/dependency_links.txt
--rw-r--r--   0 yuuxiang   (504) staff       (20)      305 2024-05-21 04:08:25.000000 pyrheed-1.0.1/src/PyRHEED.egg-info/requires.txt
--rw-r--r--   0 yuuxiang   (504) staff       (20)        8 2024-05-21 04:08:25.000000 pyrheed-1.0.1/src/PyRHEED.egg-info/top_level.txt
-drwxr-xr-x   0 yuuxiang   (504) staff       (20)        0 2024-05-21 04:08:25.993422 pyrheed-1.0.1/src/pyrheed/
--rw-r--r--   0 yuuxiang   (504) staff       (20)        0 2024-05-21 03:38:01.000000 pyrheed-1.0.1/src/pyrheed/__init__.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)     5658 2024-05-21 03:38:01.000000 pyrheed-1.0.1/src/pyrheed/bar_chart.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)     7381 2024-05-21 03:38:01.000000 pyrheed-1.0.1/src/pyrheed/boundary_statistics.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)    44251 2024-05-21 03:38:01.000000 pyrheed-1.0.1/src/pyrheed/broadening.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)     1725 2024-05-21 03:38:01.000000 pyrheed-1.0.1/src/pyrheed/browser.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)    27635 2024-05-21 03:38:01.000000 pyrheed-1.0.1/src/pyrheed/canvas.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)     2833 2024-05-21 03:38:01.000000 pyrheed-1.0.1/src/pyrheed/configuration.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)     2261 2024-05-21 03:38:01.000000 pyrheed-1.0.1/src/pyrheed/cursor.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)    36260 2024-05-21 03:38:01.000000 pyrheed-1.0.1/src/pyrheed/generate_report.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)    65698 2024-05-21 03:38:01.000000 pyrheed-1.0.1/src/pyrheed/gmm.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)    22311 2024-05-21 03:38:01.000000 pyrheed-1.0.1/src/pyrheed/graph_3D_surface.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)    27092 2024-05-21 03:38:01.000000 pyrheed-1.0.1/src/pyrheed/kikuchi.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)     9696 2024-05-21 03:38:01.000000 pyrheed-1.0.1/src/pyrheed/main.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)    17629 2024-05-21 03:38:01.000000 pyrheed-1.0.1/src/pyrheed/manual_fit.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)    50948 2024-05-21 03:38:01.000000 pyrheed-1.0.1/src/pyrheed/my_widgets.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)    18518 2024-05-21 03:38:01.000000 pyrheed-1.0.1/src/pyrheed/plot_chart.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)    12078 2024-05-21 03:38:01.000000 pyrheed-1.0.1/src/pyrheed/preference.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)   102526 2024-05-21 03:38:01.000000 pyrheed-1.0.1/src/pyrheed/process.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)     3481 2024-05-21 03:38:01.000000 pyrheed-1.0.1/src/pyrheed/process_monitor.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)    17710 2024-05-21 03:38:01.000000 pyrheed-1.0.1/src/pyrheed/profile_chart.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)    15838 2024-05-21 03:38:01.000000 pyrheed-1.0.1/src/pyrheed/properties.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)    33550 2024-05-21 03:38:01.000000 pyrheed-1.0.1/src/pyrheed/reciprocal_space_mapping.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)     2508 2024-05-21 03:38:01.000000 pyrheed-1.0.1/src/pyrheed/regularization.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)    24229 2024-05-21 03:38:01.000000 pyrheed-1.0.1/src/pyrheed/scenario.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)     7759 2024-05-21 03:38:01.000000 pyrheed-1.0.1/src/pyrheed/scipy_test.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)   147797 2024-05-21 03:38:01.000000 pyrheed-1.0.1/src/pyrheed/simulate_RHEED.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)    21776 2024-05-21 03:38:01.000000 pyrheed-1.0.1/src/pyrheed/statistical_factor.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)     7969 2024-05-21 03:38:01.000000 pyrheed-1.0.1/src/pyrheed/translational_antiphase_domain.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)    47928 2024-05-21 03:38:01.000000 pyrheed-1.0.1/src/pyrheed/window.py
--rw-r--r--   0 yuuxiang   (504) staff       (20)     4087 2024-05-21 03:38:01.000000 pyrheed-1.0.1/src/pyrheed/write_scenario.py
+drwxr-xr-x   0 yuuxiang   (504) staff       (20)        0 2024-05-21 04:21:55.218740 pyrheed-1.0.2/
+-rw-r--r--   0 yuuxiang   (504) staff       (20)     1059 2024-05-19 00:11:40.000000 pyrheed-1.0.2/LICENSE
+-rw-r--r--   0 yuuxiang   (504) staff       (20)     8455 2024-05-21 04:21:55.218415 pyrheed-1.0.2/PKG-INFO
+-rw-r--r--   0 yuuxiang   (504) staff       (20)     7352 2024-05-21 03:40:07.000000 pyrheed-1.0.2/README.md
+-rw-r--r--   0 yuuxiang   (504) staff       (20)      951 2024-05-21 04:21:46.000000 pyrheed-1.0.2/pyproject.toml
+-rw-r--r--   0 yuuxiang   (504) staff       (20)       38 2024-05-21 04:21:55.218796 pyrheed-1.0.2/setup.cfg
+drwxr-xr-x   0 yuuxiang   (504) staff       (20)        0 2024-05-21 04:21:55.207761 pyrheed-1.0.2/src/
+drwxr-xr-x   0 yuuxiang   (504) staff       (20)        0 2024-05-21 04:21:55.218028 pyrheed-1.0.2/src/PyRHEED.egg-info/
+-rw-r--r--   0 yuuxiang   (504) staff       (20)     8455 2024-05-21 04:21:55.000000 pyrheed-1.0.2/src/PyRHEED.egg-info/PKG-INFO
+-rw-r--r--   0 yuuxiang   (504) staff       (20)     1036 2024-05-21 04:21:55.000000 pyrheed-1.0.2/src/PyRHEED.egg-info/SOURCES.txt
+-rw-r--r--   0 yuuxiang   (504) staff       (20)        1 2024-05-21 04:21:55.000000 pyrheed-1.0.2/src/PyRHEED.egg-info/dependency_links.txt
+-rw-r--r--   0 yuuxiang   (504) staff       (20)      305 2024-05-21 04:21:55.000000 pyrheed-1.0.2/src/PyRHEED.egg-info/requires.txt
+-rw-r--r--   0 yuuxiang   (504) staff       (20)        8 2024-05-21 04:21:55.000000 pyrheed-1.0.2/src/PyRHEED.egg-info/top_level.txt
+drwxr-xr-x   0 yuuxiang   (504) staff       (20)        0 2024-05-21 04:21:55.217527 pyrheed-1.0.2/src/pyrheed/
+-rw-r--r--   0 yuuxiang   (504) staff       (20)        0 2024-05-21 03:38:01.000000 pyrheed-1.0.2/src/pyrheed/__init__.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)     9696 2024-05-21 03:38:01.000000 pyrheed-1.0.2/src/pyrheed/__main__.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)     5658 2024-05-21 03:38:01.000000 pyrheed-1.0.2/src/pyrheed/bar_chart.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)     7381 2024-05-21 03:38:01.000000 pyrheed-1.0.2/src/pyrheed/boundary_statistics.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)    44251 2024-05-21 03:38:01.000000 pyrheed-1.0.2/src/pyrheed/broadening.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)     1725 2024-05-21 03:38:01.000000 pyrheed-1.0.2/src/pyrheed/browser.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)    27635 2024-05-21 03:38:01.000000 pyrheed-1.0.2/src/pyrheed/canvas.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)     2833 2024-05-21 03:38:01.000000 pyrheed-1.0.2/src/pyrheed/configuration.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)     2261 2024-05-21 03:38:01.000000 pyrheed-1.0.2/src/pyrheed/cursor.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)    36260 2024-05-21 03:38:01.000000 pyrheed-1.0.2/src/pyrheed/generate_report.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)    65698 2024-05-21 03:38:01.000000 pyrheed-1.0.2/src/pyrheed/gmm.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)    22311 2024-05-21 03:38:01.000000 pyrheed-1.0.2/src/pyrheed/graph_3D_surface.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)    27092 2024-05-21 03:38:01.000000 pyrheed-1.0.2/src/pyrheed/kikuchi.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)    17629 2024-05-21 03:38:01.000000 pyrheed-1.0.2/src/pyrheed/manual_fit.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)    50948 2024-05-21 03:38:01.000000 pyrheed-1.0.2/src/pyrheed/my_widgets.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)    18518 2024-05-21 03:38:01.000000 pyrheed-1.0.2/src/pyrheed/plot_chart.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)    12078 2024-05-21 03:38:01.000000 pyrheed-1.0.2/src/pyrheed/preference.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)   102526 2024-05-21 03:38:01.000000 pyrheed-1.0.2/src/pyrheed/process.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)     3481 2024-05-21 03:38:01.000000 pyrheed-1.0.2/src/pyrheed/process_monitor.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)    17710 2024-05-21 03:38:01.000000 pyrheed-1.0.2/src/pyrheed/profile_chart.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)    15838 2024-05-21 03:38:01.000000 pyrheed-1.0.2/src/pyrheed/properties.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)    33550 2024-05-21 03:38:01.000000 pyrheed-1.0.2/src/pyrheed/reciprocal_space_mapping.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)     2508 2024-05-21 03:38:01.000000 pyrheed-1.0.2/src/pyrheed/regularization.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)    24229 2024-05-21 03:38:01.000000 pyrheed-1.0.2/src/pyrheed/scenario.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)     7759 2024-05-21 03:38:01.000000 pyrheed-1.0.2/src/pyrheed/scipy_test.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)   147797 2024-05-21 03:38:01.000000 pyrheed-1.0.2/src/pyrheed/simulate_RHEED.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)    21776 2024-05-21 03:38:01.000000 pyrheed-1.0.2/src/pyrheed/statistical_factor.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)     7969 2024-05-21 03:38:01.000000 pyrheed-1.0.2/src/pyrheed/translational_antiphase_domain.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)    47928 2024-05-21 03:38:01.000000 pyrheed-1.0.2/src/pyrheed/window.py
+-rw-r--r--   0 yuuxiang   (504) staff       (20)     4087 2024-05-21 03:38:01.000000 pyrheed-1.0.2/src/pyrheed/write_scenario.py
```

### Comparing `pyrheed-1.0.1/LICENSE` & `pyrheed-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrheed-1.0.1/PKG-INFO` & `pyrheed-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyRHEED
-Version: 1.0.1
+Version: 1.0.2
 Summary: A python package for RHEED data analysis and simulation
 Author-email: Yu Xiang <yux1991@gmail.com>
 Project-URL: Homepage, https://github.com/yux1991/PyRHEED
 Project-URL: Issues, https://github.com/yux1991/PyRHEED/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyrheed-1.0.1/README.md` & `pyrheed-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pyrheed-1.0.1/pyproject.toml` & `pyrheed-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "PyRHEED"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="Yu Xiang", email="yux1991@gmail.com" },
 ]
 description = "A python package for RHEED data analysis and simulation"
 readme = "README.md"
 requires-python = ">=3.12"
 classifiers = [
```

### Comparing `pyrheed-1.0.1/src/PyRHEED.egg-info/PKG-INFO` & `pyrheed-1.0.2/src/PyRHEED.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyRHEED
-Version: 1.0.1
+Version: 1.0.2
 Summary: A python package for RHEED data analysis and simulation
 Author-email: Yu Xiang <yux1991@gmail.com>
 Project-URL: Homepage, https://github.com/yux1991/PyRHEED
 Project-URL: Issues, https://github.com/yux1991/PyRHEED/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyrheed-1.0.1/src/PyRHEED.egg-info/SOURCES.txt` & `pyrheed-1.0.2/src/PyRHEED.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 pyproject.toml
 src/PyRHEED.egg-info/PKG-INFO
 src/PyRHEED.egg-info/SOURCES.txt
 src/PyRHEED.egg-info/dependency_links.txt
 src/PyRHEED.egg-info/requires.txt
 src/PyRHEED.egg-info/top_level.txt
 src/pyrheed/__init__.py
+src/pyrheed/__main__.py
 src/pyrheed/bar_chart.py
 src/pyrheed/boundary_statistics.py
 src/pyrheed/broadening.py
 src/pyrheed/browser.py
 src/pyrheed/canvas.py
 src/pyrheed/configuration.py
 src/pyrheed/cursor.py
 src/pyrheed/generate_report.py
 src/pyrheed/gmm.py
 src/pyrheed/graph_3D_surface.py
 src/pyrheed/kikuchi.py
-src/pyrheed/main.py
 src/pyrheed/manual_fit.py
 src/pyrheed/my_widgets.py
 src/pyrheed/plot_chart.py
 src/pyrheed/preference.py
 src/pyrheed/process.py
 src/pyrheed/process_monitor.py
 src/pyrheed/profile_chart.py
```

### Comparing `pyrheed-1.0.1/src/pyrheed/bar_chart.py` & `pyrheed-1.0.2/src/pyrheed/bar_chart.py`

 * *Files identical despite different names*

### Comparing `pyrheed-1.0.1/src/pyrheed/boundary_statistics.py` & `pyrheed-1.0.2/src/pyrheed/boundary_statistics.py`

 * *Files identical despite different names*

### Comparing `pyrheed-1.0.1/src/pyrheed/broadening.py` & `pyrheed-1.0.2/src/pyrheed/broadening.py`

 * *Files identical despite different names*

### Comparing `pyrheed-1.0.1/src/pyrheed/browser.py` & `pyrheed-1.0.2/src/pyrheed/browser.py`

 * *Files identical despite different names*

### Comparing `pyrheed-1.0.1/src/pyrheed/canvas.py` & `pyrheed-1.0.2/src/pyrheed/canvas.py`

 * *Files identical despite different names*

### Comparing `pyrheed-1.0.1/src/pyrheed/configuration.py` & `pyrheed-1.0.2/src/pyrheed/configuration.py`

 * *Files identical despite different names*

### Comparing `pyrheed-1.0.1/src/pyrheed/cursor.py` & `pyrheed-1.0.2/src/pyrheed/cursor.py`

 * *Files identical despite different names*

### Comparing `pyrheed-1.0.1/src/pyrheed/generate_report.py` & `pyrheed-1.0.2/src/pyrheed/generate_report.py`

 * *Files identical despite different names*

### Comparing `pyrheed-1.0.1/src/pyrheed/gmm.py` & `pyrheed-1.0.2/src/pyrheed/gmm.py`

 * *Files identical despite different names*

### Comparing `pyrheed-1.0.1/src/pyrheed/graph_3D_surface.py` & `pyrheed-1.0.2/src/pyrheed/graph_3D_surface.py`

 * *Files identical despite different names*

### Comparing `pyrheed-1.0.1/src/pyrheed/kikuchi.py` & `pyrheed-1.0.2/src/pyrheed/kikuchi.py`

 * *Files identical despite different names*

### Comparing `pyrheed-1.0.1/src/pyrheed/main.py` & `pyrheed-1.0.2/src/pyrheed/__main__.py`

 * *Files identical despite different names*

### Comparing `pyrheed-1.0.1/src/pyrheed/manual_fit.py` & `pyrheed-1.0.2/src/pyrheed/manual_fit.py`

 * *Files identical despite different names*

### Comparing `pyrheed-1.0.1/src/pyrheed/my_widgets.py` & `pyrheed-1.0.2/src/pyrheed/my_widgets.py`

 * *Files identical despite different names*

### Comparing `pyrheed-1.0.1/src/pyrheed/plot_chart.py` & `pyrheed-1.0.2/src/pyrheed/plot_chart.py`

 * *Files identical despite different names*

### Comparing `pyrheed-1.0.1/src/pyrheed/preference.py` & `pyrheed-1.0.2/src/pyrheed/preference.py`

 * *Files identical despite different names*

### Comparing `pyrheed-1.0.1/src/pyrheed/process.py` & `pyrheed-1.0.2/src/pyrheed/process.py`

 * *Files identical despite different names*

### Comparing `pyrheed-1.0.1/src/pyrheed/process_monitor.py` & `pyrheed-1.0.2/src/pyrheed/process_monitor.py`

 * *Files identical despite different names*

### Comparing `pyrheed-1.0.1/src/pyrheed/profile_chart.py` & `pyrheed-1.0.2/src/pyrheed/profile_chart.py`

 * *Files identical despite different names*

### Comparing `pyrheed-1.0.1/src/pyrheed/properties.py` & `pyrheed-1.0.2/src/pyrheed/properties.py`

 * *Files identical despite different names*

### Comparing `pyrheed-1.0.1/src/pyrheed/reciprocal_space_mapping.py` & `pyrheed-1.0.2/src/pyrheed/reciprocal_space_mapping.py`

 * *Files identical despite different names*

### Comparing `pyrheed-1.0.1/src/pyrheed/regularization.py` & `pyrheed-1.0.2/src/pyrheed/regularization.py`

 * *Files identical despite different names*

### Comparing `pyrheed-1.0.1/src/pyrheed/scenario.py` & `pyrheed-1.0.2/src/pyrheed/scenario.py`

 * *Files identical despite different names*

### Comparing `pyrheed-1.0.1/src/pyrheed/scipy_test.py` & `pyrheed-1.0.2/src/pyrheed/scipy_test.py`

 * *Files identical despite different names*

### Comparing `pyrheed-1.0.1/src/pyrheed/simulate_RHEED.py` & `pyrheed-1.0.2/src/pyrheed/simulate_RHEED.py`

 * *Files identical despite different names*

### Comparing `pyrheed-1.0.1/src/pyrheed/statistical_factor.py` & `pyrheed-1.0.2/src/pyrheed/statistical_factor.py`

 * *Files identical despite different names*

### Comparing `pyrheed-1.0.1/src/pyrheed/translational_antiphase_domain.py` & `pyrheed-1.0.2/src/pyrheed/translational_antiphase_domain.py`

 * *Files identical despite different names*

### Comparing `pyrheed-1.0.1/src/pyrheed/window.py` & `pyrheed-1.0.2/src/pyrheed/window.py`

 * *Files identical despite different names*

### Comparing `pyrheed-1.0.1/src/pyrheed/write_scenario.py` & `pyrheed-1.0.2/src/pyrheed/write_scenario.py`

 * *Files identical despite different names*

