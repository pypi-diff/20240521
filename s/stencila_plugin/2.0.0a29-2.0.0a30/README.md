# Comparing `tmp/stencila_plugin-2.0.0a29.tar.gz` & `tmp/stencila_plugin-2.0.0a30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stencila_plugin-2.0.0a29.tar", last modified: Tue Mar 26 03:59:23 2024, max compression
+gzip compressed data, was "stencila_plugin-2.0.0a30.tar", last modified: Tue May 21 01:57:31 2024, max compression
```

## Comparing `stencila_plugin-2.0.0a29.tar` & `stencila_plugin-2.0.0a30.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      890 2024-03-26 01:26:24.321915 stencila_plugin-2.0.0a29/README.md
--rw-r--r--   0        0        0     1865 2024-03-26 03:59:23.455186 stencila_plugin-2.0.0a29/pyproject.toml
--rw-r--r--   0        0        0       86 2024-03-26 01:26:24.322882 stencila_plugin-2.0.0a29/src/stencila_plugin/__init__.py
--rw-r--r--   0        0        0     5721 2024-03-26 03:21:24.057751 stencila_plugin-2.0.0a29/src/stencila_plugin/kernel.py
--rw-r--r--   0        0        0    10468 2024-03-26 03:23:40.306616 stencila_plugin-2.0.0a29/src/stencila_plugin/plugin.py
--rw-r--r--   0        0        0     8224 2024-03-26 01:26:24.323664 stencila_plugin-2.0.0a29/src/stencila_plugin/testing.py
--rw-r--r--   0        0        0        0 2024-03-26 01:26:24.323733 stencila_plugin-2.0.0a29/tests/__init__.py
--rw-r--r--   0        0        0      875 2024-03-26 01:26:24.323815 stencila_plugin-2.0.0a29/tests/conftest.py
--rw-r--r--   0        0        0      723 2024-03-26 01:26:24.324045 stencila_plugin-2.0.0a29/tests/plugin_example.py
--rw-r--r--   0        0        0     1775 2024-03-26 01:26:24.324265 stencila_plugin-2.0.0a29/tests/test_plugin.py
--rw-r--r--   0        0        0     1744 1970-01-01 00:00:00.000000 stencila_plugin-2.0.0a29/PKG-INFO
+-rw-r--r--   0        0        0      890 2024-03-26 01:26:24.321915 stencila_plugin-2.0.0a30/README.md
+-rw-r--r--   0        0        0     1865 2024-05-21 01:57:31.072257 stencila_plugin-2.0.0a30/pyproject.toml
+-rw-r--r--   0        0        0       86 2024-05-20 23:13:11.799305 stencila_plugin-2.0.0a30/src/stencila_plugin/__init__.py
+-rw-r--r--   0        0        0     5721 2024-03-26 03:21:24.057751 stencila_plugin-2.0.0a30/src/stencila_plugin/kernel.py
+-rw-r--r--   0        0        0    10468 2024-05-20 23:13:11.799623 stencila_plugin-2.0.0a30/src/stencila_plugin/plugin.py
+-rw-r--r--   0        0        0     8224 2024-03-26 01:26:24.323664 stencila_plugin-2.0.0a30/src/stencila_plugin/testing.py
+-rw-r--r--   0        0        0        0 2024-03-26 01:26:24.323733 stencila_plugin-2.0.0a30/tests/__init__.py
+-rw-r--r--   0        0        0      875 2024-03-26 01:26:24.323815 stencila_plugin-2.0.0a30/tests/conftest.py
+-rw-r--r--   0        0        0      723 2024-05-20 23:13:11.799874 stencila_plugin-2.0.0a30/tests/plugin_example.py
+-rw-r--r--   0        0        0     1775 2024-05-20 23:13:11.800071 stencila_plugin-2.0.0a30/tests/test_plugin.py
+-rw-r--r--   0        0        0     1744 1970-01-01 00:00:00.000000 stencila_plugin-2.0.0a30/PKG-INFO
```

### Comparing `stencila_plugin-2.0.0a29/README.md` & `stencila_plugin-2.0.0a30/README.md`

 * *Files identical despite different names*

### Comparing `stencila_plugin-2.0.0a29/pyproject.toml` & `stencila_plugin-2.0.0a30/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "stencila_plugin"
-version = "2.0.0a29"
+version = "2.0.0a30"
 description = "Library for building Stencila Plugins"
 readme = "README.md"
 authors = [
     { name = "Nokome Bentley", email = "nokome@stencila.io" },
     { name = "Brett Calcott", email = "brett@dragonfly.co.nz" },
 ]
 dependencies = [
```

### Comparing `stencila_plugin-2.0.0a29/src/stencila_plugin/kernel.py` & `stencila_plugin-2.0.0a30/src/stencila_plugin/kernel.py`

 * *Files identical despite different names*

### Comparing `stencila_plugin-2.0.0a29/src/stencila_plugin/plugin.py` & `stencila_plugin-2.0.0a30/src/stencila_plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `stencila_plugin-2.0.0a29/src/stencila_plugin/testing.py` & `stencila_plugin-2.0.0a30/src/stencila_plugin/testing.py`

 * *Files identical despite different names*

### Comparing `stencila_plugin-2.0.0a29/tests/conftest.py` & `stencila_plugin-2.0.0a30/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `stencila_plugin-2.0.0a29/tests/plugin_example.py` & `stencila_plugin-2.0.0a30/tests/plugin_example.py`

 * *Files identical despite different names*

### Comparing `stencila_plugin-2.0.0a29/tests/test_plugin.py` & `stencila_plugin-2.0.0a30/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `stencila_plugin-2.0.0a29/PKG-INFO` & `stencila_plugin-2.0.0a30/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: stencila_plugin
-Version: 2.0.0a29
+Version: 2.0.0a30
 Summary: Library for building Stencila Plugins
-Keywords: programmable reproducible interactive documents python SDK
+Keywords: programmable,reproducible,interactive,documents,python,SDK
 Author-Email: Nokome Bentley <nokome@stencila.io>, Brett Calcott <brett@dragonfly.co.nz>
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
 Classifier: Topic :: Software Development
```

