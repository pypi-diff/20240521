# Comparing `tmp/responsibleai_tabular_automl-0.8.0.tar.gz` & `tmp/responsibleai_tabular_automl-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "responsibleai_tabular_automl-0.8.0.tar", last modified: Fri Oct 20 18:33:12 2023, max compression
+gzip compressed data, was "responsibleai_tabular_automl-0.9.0.tar", last modified: Wed Dec  6 22:24:35 2023, max compression
```

## Comparing `responsibleai_tabular_automl-0.8.0.tar` & `responsibleai_tabular_automl-0.9.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-10-20 18:33:12.279820 responsibleai_tabular_automl-0.8.0/
--rw-rw-rw-   0        0        0      728 2023-10-20 18:33:12.278785 responsibleai_tabular_automl-0.8.0/PKG-INFO
--rw-rw-rw-   0        0        0      134 2023-01-18 23:36:24.000000 responsibleai_tabular_automl-0.8.0/README.md
-drwxrwxrwx   0        0        0        0 2023-10-20 18:33:12.224298 responsibleai_tabular_automl-0.8.0/responsibleai_tabular_automl/
--rw-rw-rw-   0        0        0      284 2023-10-20 18:30:18.000000 responsibleai_tabular_automl-0.8.0/responsibleai_tabular_automl/__init__.py
--rw-rw-rw-   0        0        0     6060 2023-10-20 18:30:18.000000 responsibleai_tabular_automl-0.8.0/responsibleai_tabular_automl/_loggerfactory.py
--rw-rw-rw-   0        0        0    12436 2023-10-20 18:30:18.000000 responsibleai_tabular_automl-0.8.0/responsibleai_tabular_automl/automl_inference_run.py
--rw-rw-rw-   0        0        0    11073 2023-10-20 18:30:18.000000 responsibleai_tabular_automl-0.8.0/responsibleai_tabular_automl/rai_automl.py
--rw-rw-rw-   0        0        0      210 2023-10-20 18:30:18.000000 responsibleai_tabular_automl-0.8.0/responsibleai_tabular_automl/version.py
-drwxrwxrwx   0        0        0        0 2023-10-20 18:33:12.270786 responsibleai_tabular_automl-0.8.0/responsibleai_tabular_automl.egg-info/
--rw-rw-rw-   0        0        0      728 2023-10-20 18:33:11.000000 responsibleai_tabular_automl-0.8.0/responsibleai_tabular_automl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      526 2023-10-20 18:33:12.000000 responsibleai_tabular_automl-0.8.0/responsibleai_tabular_automl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-10-20 18:33:11.000000 responsibleai_tabular_automl-0.8.0/responsibleai_tabular_automl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-10-20 18:33:11.000000 responsibleai_tabular_automl-0.8.0/responsibleai_tabular_automl.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2023-10-20 18:33:11.000000 responsibleai_tabular_automl-0.8.0/responsibleai_tabular_automl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-10-20 18:33:12.280788 responsibleai_tabular_automl-0.8.0/setup.cfg
--rw-rw-rw-   0        0        0     1350 2023-08-31 22:22:38.000000 responsibleai_tabular_automl-0.8.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-10-20 18:33:12.273781 responsibleai_tabular_automl-0.8.0/tests/
--rw-rw-rw-   0        0        0     1654 2023-10-20 18:30:18.000000 responsibleai_tabular_automl-0.8.0/tests/test_rai_automl.py
+drwxrwxrwx   0        0        0        0 2023-12-06 22:24:35.969268 responsibleai_tabular_automl-0.9.0/
+-rw-rw-rw-   0        0        0      728 2023-12-06 22:24:35.969268 responsibleai_tabular_automl-0.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0      134 2023-12-06 22:23:14.000000 responsibleai_tabular_automl-0.9.0/README.md
+drwxrwxrwx   0        0        0        0 2023-12-06 22:24:35.900065 responsibleai_tabular_automl-0.9.0/responsibleai_tabular_automl/
+-rw-rw-rw-   0        0        0      284 2023-12-06 22:23:14.000000 responsibleai_tabular_automl-0.9.0/responsibleai_tabular_automl/__init__.py
+-rw-rw-rw-   0        0        0     6060 2023-12-06 22:23:14.000000 responsibleai_tabular_automl-0.9.0/responsibleai_tabular_automl/_loggerfactory.py
+-rw-rw-rw-   0        0        0    12436 2023-12-06 22:23:14.000000 responsibleai_tabular_automl-0.9.0/responsibleai_tabular_automl/automl_inference_run.py
+-rw-rw-rw-   0        0        0    11073 2023-12-06 22:23:14.000000 responsibleai_tabular_automl-0.9.0/responsibleai_tabular_automl/rai_automl.py
+-rw-rw-rw-   0        0        0      210 2023-12-06 22:23:14.000000 responsibleai_tabular_automl-0.9.0/responsibleai_tabular_automl/version.py
+drwxrwxrwx   0        0        0        0 2023-12-06 22:24:35.954259 responsibleai_tabular_automl-0.9.0/responsibleai_tabular_automl.egg-info/
+-rw-rw-rw-   0        0        0      728 2023-12-06 22:24:35.000000 responsibleai_tabular_automl-0.9.0/responsibleai_tabular_automl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      526 2023-12-06 22:24:35.000000 responsibleai_tabular_automl-0.9.0/responsibleai_tabular_automl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-12-06 22:24:35.000000 responsibleai_tabular_automl-0.9.0/responsibleai_tabular_automl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-12-06 22:24:35.000000 responsibleai_tabular_automl-0.9.0/responsibleai_tabular_automl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2023-12-06 22:24:35.000000 responsibleai_tabular_automl-0.9.0/responsibleai_tabular_automl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-12-06 22:24:35.970270 responsibleai_tabular_automl-0.9.0/setup.cfg
+-rw-rw-rw-   0        0        0     1350 2023-12-06 22:23:14.000000 responsibleai_tabular_automl-0.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-12-06 22:24:35.967274 responsibleai_tabular_automl-0.9.0/tests/
+-rw-rw-rw-   0        0        0     1654 2023-12-06 22:23:14.000000 responsibleai_tabular_automl-0.9.0/tests/test_rai_automl.py
```

### Comparing `responsibleai_tabular_automl-0.8.0/PKG-INFO` & `responsibleai_tabular_automl-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: responsibleai_tabular_automl
-Version: 0.8.0
+Version: 0.9.0
 Summary: SDK for computing RAI insights for AutoML models.
 Home-page: 
 Author: Gaurav Gupta, Ke Xu
 Author-email: raiwidgets-maintain@microsoft.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `responsibleai_tabular_automl-0.8.0/responsibleai_tabular_automl/_loggerfactory.py` & `responsibleai_tabular_automl-0.9.0/responsibleai_tabular_automl/_loggerfactory.py`

 * *Files identical despite different names*

### Comparing `responsibleai_tabular_automl-0.8.0/responsibleai_tabular_automl/automl_inference_run.py` & `responsibleai_tabular_automl-0.9.0/responsibleai_tabular_automl/automl_inference_run.py`

 * *Files identical despite different names*

### Comparing `responsibleai_tabular_automl-0.8.0/responsibleai_tabular_automl/rai_automl.py` & `responsibleai_tabular_automl-0.9.0/responsibleai_tabular_automl/rai_automl.py`

 * *Files identical despite different names*

### Comparing `responsibleai_tabular_automl-0.8.0/responsibleai_tabular_automl.egg-info/PKG-INFO` & `responsibleai_tabular_automl-0.9.0/responsibleai_tabular_automl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: responsibleai-tabular-automl
-Version: 0.8.0
+Version: 0.9.0
 Summary: SDK for computing RAI insights for AutoML models.
 Home-page: 
 Author: Gaurav Gupta, Ke Xu
 Author-email: raiwidgets-maintain@microsoft.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `responsibleai_tabular_automl-0.8.0/responsibleai_tabular_automl.egg-info/SOURCES.txt` & `responsibleai_tabular_automl-0.9.0/responsibleai_tabular_automl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `responsibleai_tabular_automl-0.8.0/setup.py` & `responsibleai_tabular_automl-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `responsibleai_tabular_automl-0.8.0/tests/test_rai_automl.py` & `responsibleai_tabular_automl-0.9.0/tests/test_rai_automl.py`

 * *Files identical despite different names*

