# Comparing `tmp/remla24_team8_lib_version-0.3.1.tar.gz` & `tmp/remla24_team8_lib_version-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remla24_team8_lib_version-0.3.1.tar", max compression
+gzip compressed data, was "remla24_team8_lib_version-0.3.2.tar", max compression
```

## Comparing `remla24_team8_lib_version-0.3.1.tar` & `remla24_team8_lib_version-0.3.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1067 2024-05-19 11:21:28.973728 remla24_team8_lib_version-0.3.1/README.md
--rw-r--r--   0        0        0      631 2024-05-19 11:21:28.973728 remla24_team8_lib_version-0.3.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-19 11:21:28.973728 remla24_team8_lib_version-0.3.1/src/lib_version/__init__.py
--rw-r--r--   0        0        0      571 2024-05-19 11:21:28.973728 remla24_team8_lib_version-0.3.1/src/lib_version/versioning.py
--rw-r--r--   0        0        0     1512 1970-01-01 00:00:00.000000 remla24_team8_lib_version-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-05-21 17:08:03.326503 remla24_team8_lib_version-0.3.2/README.md
+-rw-r--r--   0        0        0      631 2024-05-21 17:22:16.072798 remla24_team8_lib_version-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-16 16:22:43.564527 remla24_team8_lib_version-0.3.2/src/lib_version/__init__.py
+-rw-r--r--   0        0        0      660 2024-05-21 16:56:44.925177 remla24_team8_lib_version-0.3.2/src/lib_version/versioning.py
+-rw-r--r--   0        0        0     1508 1970-01-01 00:00:00.000000 remla24_team8_lib_version-0.3.2/PKG-INFO
```

### Comparing `remla24_team8_lib_version-0.3.1/README.md` & `remla24_team8_lib_version-0.3.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,14 @@
 ```
 
 ## Usage
 
 To get the current version include the following lines:
 
 ```python
-from lib_version import Version_Util
+import lib_version.versioning as versioning
 util = VersionUtil()
-print(util.get_version_from_setup())
+print(util.get_version())
 ```
```

### Comparing `remla24_team8_lib_version-0.3.1/pyproject.toml` & `remla24_team8_lib_version-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "remla24-team8-lib-version"
-version = "0.3.1"
+version = "0.3.2"
 description = "A version-aware library that can can be asked for the version of the library"
 authors = [
     "Tip ten Brink <T.M.tenBrink@student.tudelft.nl>", 
     "Felipe Bononi Bello <bello2001felipe@gmail.com>", 
     "Dielof van Loon <d.i.vanloon@student.tudelft.nl>", 
     "Sayf El Kaddouri <sayfgmaul@gmail.com>"
 ]
```

### Comparing `remla24_team8_lib_version-0.3.1/PKG-INFO` & `remla24_team8_lib_version-0.3.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remla24-team8-lib-version
-Version: 0.3.1
+Version: 0.3.2
 Summary: A version-aware library that can can be asked for the version of the library
 Author: Tip ten Brink
 Author-email: T.M.tenBrink@student.tudelft.nl
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: importlib-resources (>=6.4.0,<7.0.0)
@@ -29,15 +29,15 @@
 ```
 
 ## Usage
 
 To get the current version include the following lines:
 
 ```python
-from lib_version import Version_Util
+import lib_version.versioning as versioning
 util = VersionUtil()
-print(util.get_version_from_setup())
+print(util.get_version())
 ```
```

