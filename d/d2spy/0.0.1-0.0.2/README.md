# Comparing `tmp/d2spy-0.0.1.tar.gz` & `tmp/d2spy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "d2spy-0.0.1.tar", max compression
+gzip compressed data, was "d2spy-0.0.2.tar", max compression
```

## Comparing `d2spy-0.0.1.tar` & `d2spy-0.0.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1084 2024-05-09 20:06:12.014917 d2spy-0.0.1/LICENSE
--rw-r--r--   0        0        0      478 2024-01-18 19:30:36.339127 d2spy-0.0.1/README.md
--rw-r--r--   0        0        0        0 2024-01-17 21:48:38.275883 d2spy-0.0.1/d2spy/__init__.py
--rw-r--r--   0        0        0     1817 2024-05-07 13:55:31.781965 d2spy-0.0.1/d2spy/api_client.py
--rw-r--r--   0        0        0     3600 2024-05-06 20:48:37.124090 d2spy-0.0.1/d2spy/auth.py
--rw-r--r--   0        0        0        0 2024-01-18 15:04:09.678821 d2spy-0.0.1/d2spy/extras/__init__.py
--rw-r--r--   0        0        0       22 2024-04-30 20:19:08.531894 d2spy-0.0.1/d2spy/extras/third_party/tusclient/__init__.py
--rw-r--r--   0        0        0     2625 2024-05-20 17:38:39.522943 d2spy-0.0.1/d2spy/extras/third_party/tusclient/client.py
--rw-r--r--   0        0        0     1088 2024-04-30 20:19:08.531894 d2spy-0.0.1/d2spy/extras/third_party/tusclient/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-30 20:19:08.531894 d2spy-0.0.1/d2spy/extras/third_party/tusclient/py.typed
--rw-r--r--   0        0        0     2989 2024-05-20 17:38:49.419440 d2spy-0.0.1/d2spy/extras/third_party/tusclient/request.py
--rw-r--r--   0        0        0       74 2024-05-20 17:39:31.182126 d2spy-0.0.1/d2spy/extras/third_party/tusclient/uploader/__init__.py
--rw-r--r--   0        0        0     9162 2024-05-20 17:39:22.605600 d2spy-0.0.1/d2spy/extras/third_party/tusclient/uploader/baseuploader.py
--rw-r--r--   0        0        0     3291 2024-05-20 17:39:11.582443 d2spy-0.0.1/d2spy/extras/third_party/tusclient/uploader/uploader.py
--rw-r--r--   0        0        0      335 2024-01-18 15:34:18.855544 d2spy-0.0.1/d2spy/extras/utils.py
--rw-r--r--   0        0        0       94 2024-05-06 20:42:46.950593 d2spy-0.0.1/d2spy/models/__init__.py
--rw-r--r--   0        0        0      616 2024-05-07 14:49:56.705546 d2spy-0.0.1/d2spy/models/data_product.py
--rw-r--r--   0        0        0     6126 2024-05-20 12:44:38.255877 d2spy-0.0.1/d2spy/models/flight.py
--rw-r--r--   0        0        0      851 2024-04-19 18:47:50.184569 d2spy-0.0.1/d2spy/models/job.py
--rw-r--r--   0        0        0      117 2024-04-19 20:46:18.130984 d2spy-0.0.1/d2spy/models/location.py
--rw-r--r--   0        0        0     4278 2024-05-07 14:51:25.410151 d2spy-0.0.1/d2spy/models/project.py
--rw-r--r--   0        0        0      645 2024-01-18 18:35:29.909248 d2spy-0.0.1/d2spy/models/user.py
--rw-r--r--   0        0        0       94 2024-05-06 20:45:45.998842 d2spy-0.0.1/d2spy/schemas/__init__.py
--rw-r--r--   0        0        0     1004 2024-05-07 14:49:35.999348 d2spy-0.0.1/d2spy/schemas/data_product.py
--rw-r--r--   0        0        0     1100 2024-05-06 20:51:28.504068 d2spy-0.0.1/d2spy/schemas/flight.py
--rw-r--r--   0        0        0      317 2024-01-18 18:52:49.119350 d2spy-0.0.1/d2spy/schemas/geojson.py
--rw-r--r--   0        0        0     1121 2024-05-06 20:51:16.960785 d2spy-0.0.1/d2spy/schemas/project.py
--rw-r--r--   0        0        0      472 2024-05-20 12:48:06.155912 d2spy-0.0.1/d2spy/schemas/stac_properties.py
--rw-r--r--   0        0        0     3336 2024-05-07 15:10:23.991650 d2spy-0.0.1/d2spy/workspace.py
--rw-r--r--   0        0        0     1154 2024-05-20 12:42:11.422108 d2spy-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1309 1970-01-01 00:00:00.000000 d2spy-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1084 2024-05-09 20:06:12.014917 d2spy-0.0.2/LICENSE
+-rw-r--r--   0        0        0      668 2024-05-21 13:44:06.545032 d2spy-0.0.2/README.md
+-rw-r--r--   0        0        0        0 2024-01-17 21:48:38.275883 d2spy-0.0.2/d2spy/__init__.py
+-rw-r--r--   0        0        0     1817 2024-05-07 13:55:31.781965 d2spy-0.0.2/d2spy/api_client.py
+-rw-r--r--   0        0        0     3600 2024-05-06 20:48:37.124090 d2spy-0.0.2/d2spy/auth.py
+-rw-r--r--   0        0        0        0 2024-01-18 15:04:09.678821 d2spy-0.0.2/d2spy/extras/__init__.py
+-rw-r--r--   0        0        0       22 2024-04-30 20:19:08.531894 d2spy-0.0.2/d2spy/extras/third_party/tusclient/__init__.py
+-rw-r--r--   0        0        0     2625 2024-05-20 17:38:39.522943 d2spy-0.0.2/d2spy/extras/third_party/tusclient/client.py
+-rw-r--r--   0        0        0     1088 2024-04-30 20:19:08.531894 d2spy-0.0.2/d2spy/extras/third_party/tusclient/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-30 20:19:08.531894 d2spy-0.0.2/d2spy/extras/third_party/tusclient/py.typed
+-rw-r--r--   0        0        0     2989 2024-05-20 17:38:49.419440 d2spy-0.0.2/d2spy/extras/third_party/tusclient/request.py
+-rw-r--r--   0        0        0       74 2024-05-20 17:39:31.182126 d2spy-0.0.2/d2spy/extras/third_party/tusclient/uploader/__init__.py
+-rw-r--r--   0        0        0     9162 2024-05-20 17:39:22.605600 d2spy-0.0.2/d2spy/extras/third_party/tusclient/uploader/baseuploader.py
+-rw-r--r--   0        0        0     3291 2024-05-20 17:39:11.582443 d2spy-0.0.2/d2spy/extras/third_party/tusclient/uploader/uploader.py
+-rw-r--r--   0        0        0      335 2024-01-18 15:34:18.855544 d2spy-0.0.2/d2spy/extras/utils.py
+-rw-r--r--   0        0        0       94 2024-05-06 20:42:46.950593 d2spy-0.0.2/d2spy/models/__init__.py
+-rw-r--r--   0        0        0      616 2024-05-07 14:49:56.705546 d2spy-0.0.2/d2spy/models/data_product.py
+-rw-r--r--   0        0        0     6126 2024-05-20 12:44:38.255877 d2spy-0.0.2/d2spy/models/flight.py
+-rw-r--r--   0        0        0      851 2024-04-19 18:47:50.184569 d2spy-0.0.2/d2spy/models/job.py
+-rw-r--r--   0        0        0      117 2024-04-19 20:46:18.130984 d2spy-0.0.2/d2spy/models/location.py
+-rw-r--r--   0        0        0     4278 2024-05-07 14:51:25.410151 d2spy-0.0.2/d2spy/models/project.py
+-rw-r--r--   0        0        0      645 2024-01-18 18:35:29.909248 d2spy-0.0.2/d2spy/models/user.py
+-rw-r--r--   0        0        0       94 2024-05-06 20:45:45.998842 d2spy-0.0.2/d2spy/schemas/__init__.py
+-rw-r--r--   0        0        0     1004 2024-05-07 14:49:35.999348 d2spy-0.0.2/d2spy/schemas/data_product.py
+-rw-r--r--   0        0        0     1100 2024-05-06 20:51:28.504068 d2spy-0.0.2/d2spy/schemas/flight.py
+-rw-r--r--   0        0        0      317 2024-01-18 18:52:49.119350 d2spy-0.0.2/d2spy/schemas/geojson.py
+-rw-r--r--   0        0        0     1121 2024-05-06 20:51:16.960785 d2spy-0.0.2/d2spy/schemas/project.py
+-rw-r--r--   0        0        0      472 2024-05-20 12:48:06.155912 d2spy-0.0.2/d2spy/schemas/stac_properties.py
+-rw-r--r--   0        0        0     3336 2024-05-07 15:10:23.991650 d2spy-0.0.2/d2spy/workspace.py
+-rw-r--r--   0        0        0     1154 2024-05-21 13:48:30.735918 d2spy-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1499 1970-01-01 00:00:00.000000 d2spy-0.0.2/PKG-INFO
```

### Comparing `d2spy-0.0.1/LICENSE` & `d2spy-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `d2spy-0.0.1/d2spy/api_client.py` & `d2spy-0.0.2/d2spy/api_client.py`

 * *Files identical despite different names*

### Comparing `d2spy-0.0.1/d2spy/auth.py` & `d2spy-0.0.2/d2spy/auth.py`

 * *Files identical despite different names*

### Comparing `d2spy-0.0.1/d2spy/extras/third_party/tusclient/client.py` & `d2spy-0.0.2/d2spy/extras/third_party/tusclient/client.py`

 * *Files identical despite different names*

### Comparing `d2spy-0.0.1/d2spy/extras/third_party/tusclient/exceptions.py` & `d2spy-0.0.2/d2spy/extras/third_party/tusclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `d2spy-0.0.1/d2spy/extras/third_party/tusclient/request.py` & `d2spy-0.0.2/d2spy/extras/third_party/tusclient/request.py`

 * *Files identical despite different names*

### Comparing `d2spy-0.0.1/d2spy/extras/third_party/tusclient/uploader/baseuploader.py` & `d2spy-0.0.2/d2spy/extras/third_party/tusclient/uploader/baseuploader.py`

 * *Files identical despite different names*

### Comparing `d2spy-0.0.1/d2spy/extras/third_party/tusclient/uploader/uploader.py` & `d2spy-0.0.2/d2spy/extras/third_party/tusclient/uploader/uploader.py`

 * *Files identical despite different names*

### Comparing `d2spy-0.0.1/d2spy/models/data_product.py` & `d2spy-0.0.2/d2spy/models/data_product.py`

 * *Files identical despite different names*

### Comparing `d2spy-0.0.1/d2spy/models/flight.py` & `d2spy-0.0.2/d2spy/models/flight.py`

 * *Files identical despite different names*

### Comparing `d2spy-0.0.1/d2spy/models/job.py` & `d2spy-0.0.2/d2spy/models/job.py`

 * *Files identical despite different names*

### Comparing `d2spy-0.0.1/d2spy/models/project.py` & `d2spy-0.0.2/d2spy/models/project.py`

 * *Files identical despite different names*

### Comparing `d2spy-0.0.1/d2spy/models/user.py` & `d2spy-0.0.2/d2spy/models/user.py`

 * *Files identical despite different names*

### Comparing `d2spy-0.0.1/d2spy/schemas/data_product.py` & `d2spy-0.0.2/d2spy/schemas/data_product.py`

 * *Files identical despite different names*

### Comparing `d2spy-0.0.1/d2spy/schemas/flight.py` & `d2spy-0.0.2/d2spy/schemas/flight.py`

 * *Files identical despite different names*

### Comparing `d2spy-0.0.1/d2spy/schemas/project.py` & `d2spy-0.0.2/d2spy/schemas/project.py`

 * *Files identical despite different names*

### Comparing `d2spy-0.0.1/d2spy/workspace.py` & `d2spy-0.0.2/d2spy/workspace.py`

 * *Files identical despite different names*

### Comparing `d2spy-0.0.1/pyproject.toml` & `d2spy-0.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "d2spy"
-version = "0.0.1"
+version = "0.0.2"
 license = "MIT License"
 description = "Python package for interacting with a Data to Science instance."
 authors = ["Ben Hancock <hancocb@purdue.edu>"]
 readme = "README.md"
 keywords = ["python", "data to science", "uas"]
 classifiers = [
     "Development Status :: 3 - Alpha",
```

