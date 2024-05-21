# Comparing `tmp/accelbyte_py_sdk_all-0.5.0.tar.gz` & `tmp/accelbyte_py_sdk_all-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accelbyte_py_sdk_all-0.5.0.tar", last modified: Tue May  7 06:31:33 2024, max compression
+gzip compressed data, was "accelbyte_py_sdk_all-0.6.0.tar", last modified: Tue May 21 03:50:52 2024, max compression
```

## Comparing `accelbyte_py_sdk_all-0.5.0.tar` & `accelbyte_py_sdk_all-0.6.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:31:33.311907 accelbyte_py_sdk_all-0.5.0/
--rw-r--r--   0 root         (0) root         (0)    43234 2024-05-07 06:31:33.311907 accelbyte_py_sdk_all-0.5.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)    41526 2024-05-07 06:31:24.000000 accelbyte_py_sdk_all-0.5.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:31:33.311907 accelbyte_py_sdk_all-0.5.0/accelbyte_py_sdk_all.egg-info/
--rw-r--r--   0 root         (0) root         (0)    43234 2024-05-07 06:31:33.000000 accelbyte_py_sdk_all-0.5.0/accelbyte_py_sdk_all.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      243 2024-05-07 06:31:33.000000 accelbyte_py_sdk_all-0.5.0/accelbyte_py_sdk_all.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-07 06:31:33.000000 accelbyte_py_sdk_all-0.5.0/accelbyte_py_sdk_all.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1064 2024-05-07 06:31:33.000000 accelbyte_py_sdk_all-0.5.0/accelbyte_py_sdk_all.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-07 06:31:33.000000 accelbyte_py_sdk_all-0.5.0/accelbyte_py_sdk_all.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)     1599 2024-05-07 06:24:47.000000 accelbyte_py_sdk_all-0.5.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-07 06:31:33.311907 accelbyte_py_sdk_all-0.5.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:50:52.052263 accelbyte_py_sdk_all-0.6.0/
+-rw-r--r--   0 root         (0) root         (0)    43234 2024-05-21 03:50:52.052263 accelbyte_py_sdk_all-0.6.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)    41526 2024-05-21 03:50:43.000000 accelbyte_py_sdk_all-0.6.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:50:52.052263 accelbyte_py_sdk_all-0.6.0/accelbyte_py_sdk_all.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    43234 2024-05-21 03:50:52.000000 accelbyte_py_sdk_all-0.6.0/accelbyte_py_sdk_all.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      243 2024-05-21 03:50:52.000000 accelbyte_py_sdk_all-0.6.0/accelbyte_py_sdk_all.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 03:50:52.000000 accelbyte_py_sdk_all-0.6.0/accelbyte_py_sdk_all.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1064 2024-05-21 03:50:52.000000 accelbyte_py_sdk_all-0.6.0/accelbyte_py_sdk_all.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 03:50:52.000000 accelbyte_py_sdk_all-0.6.0/accelbyte_py_sdk_all.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)     1599 2024-05-21 03:44:14.000000 accelbyte_py_sdk_all-0.6.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-21 03:50:52.052263 accelbyte_py_sdk_all-0.6.0/setup.cfg
```

### Comparing `accelbyte_py_sdk_all-0.5.0/PKG-INFO` & `accelbyte_py_sdk_all-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: accelbyte-py-sdk-all
-Version: 0.5.0
+Version: 0.6.0
 Summary: AccelByte Python SDK - All
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: accelbyte-py-sdk-core
 Requires-Dist: accelbyte-py-sdk-feat-auth
 Requires-Dist: accelbyte-py-sdk-feat-token-validation
 Requires-Dist: accelbyte-py-sdk-service-achievement
```

### Comparing `accelbyte_py_sdk_all-0.5.0/README.md` & `accelbyte_py_sdk_all-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_all-0.5.0/accelbyte_py_sdk_all.egg-info/PKG-INFO` & `accelbyte_py_sdk_all-0.6.0/accelbyte_py_sdk_all.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: accelbyte-py-sdk-all
-Version: 0.5.0
+Version: 0.6.0
 Summary: AccelByte Python SDK - All
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: accelbyte-py-sdk-core
 Requires-Dist: accelbyte-py-sdk-feat-auth
 Requires-Dist: accelbyte-py-sdk-feat-token-validation
 Requires-Dist: accelbyte-py-sdk-service-achievement
```

### Comparing `accelbyte_py_sdk_all-0.5.0/accelbyte_py_sdk_all.egg-info/requires.txt` & `accelbyte_py_sdk_all-0.6.0/accelbyte_py_sdk_all.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_all-0.5.0/pyproject.toml` & `accelbyte_py_sdk_all-0.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "accelbyte-py-sdk-all"
 readme = "README.md"
-version = "0.5.0"
+version = "0.6.0"
 description = "AccelByte Python SDK - All"
 requires-python = ">=3.9"
 dependencies = [
     "accelbyte-py-sdk-core",
     # Features
     "accelbyte-py-sdk-feat-auth",
     "accelbyte-py-sdk-feat-token-validation",
```

