# Comparing `tmp/stencila_plugin-2.0.0a31.tar.gz` & `tmp/stencila_plugin-2.0.0a32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stencila_plugin-2.0.0a31.tar", last modified: Tue May 21 03:32:05 2024, max compression
+gzip compressed data, was "stencila_plugin-2.0.0a32.tar", last modified: Tue May 21 04:49:25 2024, max compression
```

## Comparing `stencila_plugin-2.0.0a31.tar` & `stencila_plugin-2.0.0a32.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      890 2024-03-26 01:26:24.321915 stencila_plugin-2.0.0a31/README.md
--rw-r--r--   0        0        0     1865 2024-05-21 03:32:05.556001 stencila_plugin-2.0.0a31/pyproject.toml
--rw-r--r--   0        0        0      319 2024-05-21 03:23:15.043705 stencila_plugin-2.0.0a31/src/stencila_plugin/__init__.py
--rw-r--r--   0        0        0     4085 2024-05-21 03:23:15.043904 stencila_plugin-2.0.0a31/src/stencila_plugin/assistant.py
--rw-r--r--   0        0        0     5721 2024-03-26 03:21:24.057751 stencila_plugin-2.0.0a31/src/stencila_plugin/kernel.py
--rw-r--r--   0        0        0    12223 2024-05-21 03:23:15.044355 stencila_plugin-2.0.0a31/src/stencila_plugin/plugin.py
--rw-r--r--   0        0        0     8224 2024-03-26 01:26:24.323664 stencila_plugin-2.0.0a31/src/stencila_plugin/testing.py
--rw-r--r--   0        0        0        0 2024-03-26 01:26:24.323733 stencila_plugin-2.0.0a31/tests/__init__.py
--rw-r--r--   0        0        0      875 2024-03-26 01:26:24.323815 stencila_plugin-2.0.0a31/tests/conftest.py
--rw-r--r--   0        0        0     1126 2024-05-21 03:23:15.044616 stencila_plugin-2.0.0a31/tests/plugin_example.py
--rw-r--r--   0        0        0     3261 2024-05-21 03:23:15.045065 stencila_plugin-2.0.0a31/tests/test_plugin.py
--rw-r--r--   0        0        0     1744 1970-01-01 00:00:00.000000 stencila_plugin-2.0.0a31/PKG-INFO
+-rw-r--r--   0        0        0      890 2024-03-26 01:26:24.321915 stencila_plugin-2.0.0a32/README.md
+-rw-r--r--   0        0        0     1865 2024-05-21 04:49:25.040264 stencila_plugin-2.0.0a32/pyproject.toml
+-rw-r--r--   0        0        0      319 2024-05-21 03:23:15.043705 stencila_plugin-2.0.0a32/src/stencila_plugin/__init__.py
+-rw-r--r--   0        0        0     4085 2024-05-21 03:23:15.043904 stencila_plugin-2.0.0a32/src/stencila_plugin/assistant.py
+-rw-r--r--   0        0        0     5721 2024-03-26 03:21:24.057751 stencila_plugin-2.0.0a32/src/stencila_plugin/kernel.py
+-rw-r--r--   0        0        0    12223 2024-05-21 03:23:15.044355 stencila_plugin-2.0.0a32/src/stencila_plugin/plugin.py
+-rw-r--r--   0        0        0     8224 2024-03-26 01:26:24.323664 stencila_plugin-2.0.0a32/src/stencila_plugin/testing.py
+-rw-r--r--   0        0        0        0 2024-03-26 01:26:24.323733 stencila_plugin-2.0.0a32/tests/__init__.py
+-rw-r--r--   0        0        0      875 2024-03-26 01:26:24.323815 stencila_plugin-2.0.0a32/tests/conftest.py
+-rw-r--r--   0        0        0     1126 2024-05-21 03:23:15.044616 stencila_plugin-2.0.0a32/tests/plugin_example.py
+-rw-r--r--   0        0        0     3261 2024-05-21 03:23:15.045065 stencila_plugin-2.0.0a32/tests/test_plugin.py
+-rw-r--r--   0        0        0     1744 1970-01-01 00:00:00.000000 stencila_plugin-2.0.0a32/PKG-INFO
```

### Comparing `stencila_plugin-2.0.0a31/README.md` & `stencila_plugin-2.0.0a32/README.md`

 * *Files identical despite different names*

### Comparing `stencila_plugin-2.0.0a31/pyproject.toml` & `stencila_plugin-2.0.0a32/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [project]
 name = "stencila_plugin"
-version = "2.0.0a31"
+version = "2.0.0a32"
 description = "Library for building Stencila Plugins"
 readme = "README.md"
 authors = [
     { name = "Nokome Bentley", email = "nokome@stencila.io" },
     { name = "Brett Calcott", email = "brett@dragonfly.co.nz" },
 ]
 dependencies = [
     "aiohttp>=3.9.3",
-    "stencila-types>=2.0.0a26",
+    "stencila-types>=2.0.0a29",
 ]
 requires-python = ">=3.10"
 keywords = [
     "programmable",
     "reproducible",
     "interactive",
     "documents",
```

### Comparing `stencila_plugin-2.0.0a31/src/stencila_plugin/assistant.py` & `stencila_plugin-2.0.0a32/src/stencila_plugin/assistant.py`

 * *Files identical despite different names*

### Comparing `stencila_plugin-2.0.0a31/src/stencila_plugin/kernel.py` & `stencila_plugin-2.0.0a32/src/stencila_plugin/kernel.py`

 * *Files identical despite different names*

### Comparing `stencila_plugin-2.0.0a31/src/stencila_plugin/plugin.py` & `stencila_plugin-2.0.0a32/src/stencila_plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `stencila_plugin-2.0.0a31/src/stencila_plugin/testing.py` & `stencila_plugin-2.0.0a32/src/stencila_plugin/testing.py`

 * *Files identical despite different names*

### Comparing `stencila_plugin-2.0.0a31/tests/conftest.py` & `stencila_plugin-2.0.0a32/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `stencila_plugin-2.0.0a31/tests/plugin_example.py` & `stencila_plugin-2.0.0a32/tests/plugin_example.py`

 * *Files identical despite different names*

### Comparing `stencila_plugin-2.0.0a31/tests/test_plugin.py` & `stencila_plugin-2.0.0a32/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `stencila_plugin-2.0.0a31/PKG-INFO` & `stencila_plugin-2.0.0a32/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: stencila_plugin
-Version: 2.0.0a31
+Version: 2.0.0a32
 Summary: Library for building Stencila Plugins
 Keywords: programmable,reproducible,interactive,documents,python,SDK
 Author-Email: Nokome Bentley <nokome@stencila.io>, Brett Calcott <brett@dragonfly.co.nz>
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
 Classifier: Topic :: Software Development
 Classifier: License :: OSI Approved :: Apache Software License
 Project-URL: Homepage, https://github.com/stencila/stencila/tree/main/python#readme
 Project-URL: Repository, https://github.com/stencila/stencila
 Requires-Python: >=3.10
 Requires-Dist: aiohttp>=3.9.3
-Requires-Dist: stencila-types>=2.0.0a26
+Requires-Dist: stencila-types>=2.0.0a29
 Description-Content-Type: text/markdown
 
 # Stencila Plugin
 
 [![stencila_plugin](https://img.shields.io/pypi/v/stencila_plugin.svg?logo=python&label=stencila_plugin&style=for-the-badge&color=1d3bd1&logoColor=66ff66&labelColor=3219a8)](https://pypi.org/project/stencila_plugin/)
 
 ## Introduction
```

