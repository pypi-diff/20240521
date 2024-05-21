# Comparing `tmp/gdtransform-0.0.6.tar.gz` & `tmp/gdtransform-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdtransform-0.0.6.tar", last modified: Fri May 17 14:18:30 2024, max compression
+gzip compressed data, was "gdtransform-0.0.7.tar", last modified: Tue May 21 11:02:07 2024, max compression
```

## Comparing `gdtransform-0.0.6.tar` & `gdtransform-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-17 14:18:30.798302 gdtransform-0.0.6/
--rw-rw-r--   0 mayank    (1000) mayank    (1000)    34523 2024-05-17 10:41:53.000000 gdtransform-0.0.6/LICENSE
--rw-r--r--   0 mayank    (1000) mayank    (1000)      715 2024-05-17 14:18:30.798302 gdtransform-0.0.6/PKG-INFO
--rw-rw-r--   0 mayank    (1000) mayank    (1000)       91 2024-05-17 10:41:53.000000 gdtransform-0.0.6/README.md
--rw-rw-r--   0 mayank    (1000) mayank    (1000)      733 2024-05-17 14:13:06.000000 gdtransform-0.0.6/pyproject.toml
--rw-rw-r--   0 mayank    (1000) mayank    (1000)       38 2024-05-17 14:18:30.798302 gdtransform-0.0.6/setup.cfg
-drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-17 14:18:30.798302 gdtransform-0.0.6/src/
-drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-17 14:18:30.798302 gdtransform-0.0.6/src/gdtransform/
--rw-rw-r--   0 mayank    (1000) mayank    (1000)        0 2024-05-17 11:56:25.000000 gdtransform-0.0.6/src/gdtransform/__init__.py
--rw-rw-r--   0 mayank    (1000) mayank    (1000)      107 2024-05-17 13:46:47.000000 gdtransform-0.0.6/src/gdtransform/constants.py
--rw-rw-r--   0 mayank    (1000) mayank    (1000)      679 2024-05-17 14:17:14.000000 gdtransform-0.0.6/src/gdtransform/introspect.py
--rw-rw-r--   0 mayank    (1000) mayank    (1000)      484 2024-05-17 14:17:37.000000 gdtransform-0.0.6/src/gdtransform/transform.py
-drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-17 14:18:30.798302 gdtransform-0.0.6/src/gdtransform.egg-info/
--rw-r--r--   0 mayank    (1000) mayank    (1000)      715 2024-05-17 14:18:30.000000 gdtransform-0.0.6/src/gdtransform.egg-info/PKG-INFO
--rw-rw-r--   0 mayank    (1000) mayank    (1000)      304 2024-05-17 14:18:30.000000 gdtransform-0.0.6/src/gdtransform.egg-info/SOURCES.txt
--rw-rw-r--   0 mayank    (1000) mayank    (1000)        1 2024-05-17 14:18:30.000000 gdtransform-0.0.6/src/gdtransform.egg-info/dependency_links.txt
--rw-rw-r--   0 mayank    (1000) mayank    (1000)       12 2024-05-17 14:18:30.000000 gdtransform-0.0.6/src/gdtransform.egg-info/top_level.txt
+drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-21 11:02:07.739599 gdtransform-0.0.7/
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)    34523 2024-05-17 10:41:53.000000 gdtransform-0.0.7/LICENSE
+-rw-r--r--   0 mayank    (1000) mayank    (1000)      715 2024-05-21 11:02:07.739599 gdtransform-0.0.7/PKG-INFO
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)       91 2024-05-17 10:41:53.000000 gdtransform-0.0.7/README.md
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)      733 2024-05-21 10:58:52.000000 gdtransform-0.0.7/pyproject.toml
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)       38 2024-05-21 11:02:07.739599 gdtransform-0.0.7/setup.cfg
+drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-21 11:02:07.739599 gdtransform-0.0.7/src/
+drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-21 11:02:07.739599 gdtransform-0.0.7/src/gdtransform/
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)        0 2024-05-17 11:56:25.000000 gdtransform-0.0.7/src/gdtransform/__init__.py
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)      107 2024-05-17 13:46:47.000000 gdtransform-0.0.7/src/gdtransform/constants.py
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)      679 2024-05-17 14:17:14.000000 gdtransform-0.0.7/src/gdtransform/introspect.py
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)     2185 2024-05-21 10:56:13.000000 gdtransform-0.0.7/src/gdtransform/test.py
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)      484 2024-05-17 14:17:37.000000 gdtransform-0.0.7/src/gdtransform/transform.py
+drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-21 11:02:07.739599 gdtransform-0.0.7/src/gdtransform.egg-info/
+-rw-r--r--   0 mayank    (1000) mayank    (1000)      715 2024-05-21 11:02:07.000000 gdtransform-0.0.7/src/gdtransform.egg-info/PKG-INFO
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)      347 2024-05-21 11:02:07.000000 gdtransform-0.0.7/src/gdtransform.egg-info/SOURCES.txt
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)        1 2024-05-21 11:02:07.000000 gdtransform-0.0.7/src/gdtransform.egg-info/dependency_links.txt
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)       12 2024-05-21 11:02:07.000000 gdtransform-0.0.7/src/gdtransform.egg-info/top_level.txt
+drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-21 11:02:07.739599 gdtransform-0.0.7/tests/
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)     1654 2024-05-21 10:57:42.000000 gdtransform-0.0.7/tests/test_test.py
```

### Comparing `gdtransform-0.0.6/LICENSE` & `gdtransform-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gdtransform-0.0.6/PKG-INFO` & `gdtransform-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdtransform
-Version: 0.0.6
+Version: 0.0.7
 Summary: Transformation library to build transformations for Godel Grid data platform
 Author-email: Mayank Bhargava <mbhargava.gd@gmail.com>
 Project-URL: Homepage, https://www.godelgrid.com
 Project-URL: Documentation, https://www.godelgrid.com/docs
 Project-URL: Repository, https://github.com/godelgrid/gdtransform
 Project-URL: Issues, https://github.com/godelgrid/gdtransform/issues
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `gdtransform-0.0.6/pyproject.toml` & `gdtransform-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [project]
 name = "gdtransform"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
     { name = "Mayank Bhargava", email = "mbhargava.gd@gmail.com" },
 ]
 description = "Transformation library to build transformations for Godel Grid data platform"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `gdtransform-0.0.6/src/gdtransform/introspect.py` & `gdtransform-0.0.7/src/gdtransform/introspect.py`

 * *Files identical despite different names*

### Comparing `gdtransform-0.0.6/src/gdtransform.egg-info/PKG-INFO` & `gdtransform-0.0.7/src/gdtransform.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdtransform
-Version: 0.0.6
+Version: 0.0.7
 Summary: Transformation library to build transformations for Godel Grid data platform
 Author-email: Mayank Bhargava <mbhargava.gd@gmail.com>
 Project-URL: Homepage, https://www.godelgrid.com
 Project-URL: Documentation, https://www.godelgrid.com/docs
 Project-URL: Repository, https://github.com/godelgrid/gdtransform
 Project-URL: Issues, https://github.com/godelgrid/gdtransform/issues
 Classifier: Programming Language :: Python :: 3.10
```

