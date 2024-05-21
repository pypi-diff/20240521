# Comparing `tmp/sipmessage-0.2.0.tar.gz` & `tmp/sipmessage-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sipmessage-0.2.0.tar", last modified: Thu May 16 23:03:06 2024, max compression
+gzip compressed data, was "sipmessage-0.2.1.tar", last modified: Tue May 21 11:05:35 2024, max compression
```

## Comparing `sipmessage-0.2.0.tar` & `sipmessage-0.2.1.tar`

### file list

```diff
@@ -1,32 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 23:03:06.841922 sipmessage-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-16 23:02:58.000000 sipmessage-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-16 23:02:58.000000 sipmessage-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-05-16 23:02:58.000000 sipmessage-0.2.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-05-16 23:03:06.841922 sipmessage-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-16 23:02:58.000000 sipmessage-0.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 23:03:06.837922 sipmessage-0.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-16 23:02:58.000000 sipmessage-0.2.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-16 23:02:58.000000 sipmessage-0.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-16 23:02:58.000000 sipmessage-0.2.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-05-16 23:02:58.000000 sipmessage-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 23:03:06.841922 sipmessage-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 23:02:58.000000 sipmessage-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 23:03:06.837922 sipmessage-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 23:03:06.837922 sipmessage-0.2.0/src/sipmessage/
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-16 23:02:58.000000 sipmessage-0.2.0/src/sipmessage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-16 23:02:58.000000 sipmessage-0.2.0/src/sipmessage/address.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-16 23:02:58.000000 sipmessage-0.2.0/src/sipmessage/parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-16 23:02:58.000000 sipmessage-0.2.0/src/sipmessage/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-05-16 23:02:58.000000 sipmessage-0.2.0/src/sipmessage/uri.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 23:03:06.841922 sipmessage-0.2.0/src/sipmessage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-05-16 23:03:06.000000 sipmessage-0.2.0/src/sipmessage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-16 23:03:06.000000 sipmessage-0.2.0/src/sipmessage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 23:03:06.000000 sipmessage-0.2.0/src/sipmessage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-16 23:03:06.000000 sipmessage-0.2.0/src/sipmessage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-16 23:03:06.000000 sipmessage-0.2.0/src/sipmessage.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 23:03:06.841922 sipmessage-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 23:02:58.000000 sipmessage-0.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-05-16 23:02:58.000000 sipmessage-0.2.0/tests/test_address.py
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-16 23:02:58.000000 sipmessage-0.2.0/tests/test_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-16 23:02:58.000000 sipmessage-0.2.0/tests/test_public_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-05-16 23:02:58.000000 sipmessage-0.2.0/tests/test_uri.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:05:35.550305 sipmessage-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-21 11:05:26.000000 sipmessage-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-21 11:05:26.000000 sipmessage-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-05-21 11:05:26.000000 sipmessage-0.2.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-05-21 11:05:35.550305 sipmessage-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-21 11:05:26.000000 sipmessage-0.2.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:05:35.546305 sipmessage-0.2.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-21 11:05:26.000000 sipmessage-0.2.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-21 11:05:26.000000 sipmessage-0.2.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-21 11:05:26.000000 sipmessage-0.2.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-05-21 11:05:26.000000 sipmessage-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 11:05:35.550305 sipmessage-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 11:05:26.000000 sipmessage-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:05:35.542305 sipmessage-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:05:35.546305 sipmessage-0.2.1/src/sipmessage/
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-21 11:05:26.000000 sipmessage-0.2.1/src/sipmessage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-21 11:05:26.000000 sipmessage-0.2.1/src/sipmessage/address.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-21 11:05:26.000000 sipmessage-0.2.1/src/sipmessage/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-21 11:05:26.000000 sipmessage-0.2.1/src/sipmessage/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-05-21 11:05:26.000000 sipmessage-0.2.1/src/sipmessage/uri.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-21 11:05:26.000000 sipmessage-0.2.1/src/sipmessage/via.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:05:35.550305 sipmessage-0.2.1/src/sipmessage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-05-21 11:05:35.000000 sipmessage-0.2.1/src/sipmessage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-21 11:05:35.000000 sipmessage-0.2.1/src/sipmessage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 11:05:35.000000 sipmessage-0.2.1/src/sipmessage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-21 11:05:35.000000 sipmessage-0.2.1/src/sipmessage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-21 11:05:35.000000 sipmessage-0.2.1/src/sipmessage.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:05:35.546305 sipmessage-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:05:26.000000 sipmessage-0.2.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-05-21 11:05:26.000000 sipmessage-0.2.1/tests/test_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-21 11:05:26.000000 sipmessage-0.2.1/tests/test_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-21 11:05:26.000000 sipmessage-0.2.1/tests/test_public_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-05-21 11:05:26.000000 sipmessage-0.2.1/tests/test_uri.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-21 11:05:26.000000 sipmessage-0.2.1/tests/test_via.py
```

### Comparing `sipmessage-0.2.0/LICENSE` & `sipmessage-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sipmessage-0.2.0/Makefile` & `sipmessage-0.2.1/Makefile`

 * *Files identical despite different names*

### Comparing `sipmessage-0.2.0/PKG-INFO` & `sipmessage-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sipmessage
-Version: 0.2.0
+Version: 0.2.1
 Summary: Pure python parsing of SIP messages and headers
 Author-email: Spacinov Engineering <opensource@spacinov.com>
 License: BSD License
 Project-URL: Homepage, https://sipmessage.readthedocs.io/
 Project-URL: Documentation, https://sipmessage.readthedocs.io/
 Project-URL: Repository, https://github.com/spacinov/sipmessage
 Project-URL: Issues, https://github.com/spacinov/sipmessage/issues
```

### Comparing `sipmessage-0.2.0/README.rst` & `sipmessage-0.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `sipmessage-0.2.0/docs/Makefile` & `sipmessage-0.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sipmessage-0.2.0/docs/conf.py` & `sipmessage-0.2.1/docs/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,19 @@
 author = "Spacinov Engineering"
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = [
     "sphinx.ext.autodoc",
+    "sphinx.ext.intersphinx",
 ]
+intersphinx_mapping = {
+    "python": ("https://docs.python.org/3", None),
+}
 
 templates_path = ["_templates"]
 exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
 
 # -- Options for HTML output -------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
```

### Comparing `sipmessage-0.2.0/docs/index.rst` & `sipmessage-0.2.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `sipmessage-0.2.0/pyproject.toml` & `sipmessage-0.2.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 # Version
 name = "sipmessage"
-version = "0.2.0"
+version = "0.2.1"
 
 # Dependencies
 dependencies = []
 requires-python = ">= 3.10"
 
 # Development
 authors = [
```

### Comparing `sipmessage-0.2.0/src/sipmessage/address.py` & `sipmessage-0.2.1/src/sipmessage/address.py`

 * *Files identical despite different names*

### Comparing `sipmessage-0.2.0/src/sipmessage/parameters.py` & `sipmessage-0.2.1/src/sipmessage/parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (C) Spacinov SAS
 # Distributed under the 2-clause BSD license
 #
 
 
 class Parameters(dict[str, str | None]):
     """
-    A dictionary of :class:`Address` or :class:`URI` parameters.
+    A dictionary of :class:`Address`, :class:`URI` or :class:`Via` parameters.
     """
 
     @classmethod
     def parse(cls, val: str) -> "Parameters":
         """
         Parse the given string into a :class:`Parameters` instance.
         """
```

### Comparing `sipmessage-0.2.0/src/sipmessage/uri.py` & `sipmessage-0.2.1/src/sipmessage/uri.py`

 * *Files identical despite different names*

### Comparing `sipmessage-0.2.0/src/sipmessage.egg-info/PKG-INFO` & `sipmessage-0.2.1/src/sipmessage.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sipmessage
-Version: 0.2.0
+Version: 0.2.1
 Summary: Pure python parsing of SIP messages and headers
 Author-email: Spacinov Engineering <opensource@spacinov.com>
 License: BSD License
 Project-URL: Homepage, https://sipmessage.readthedocs.io/
 Project-URL: Documentation, https://sipmessage.readthedocs.io/
 Project-URL: Repository, https://github.com/spacinov/sipmessage
 Project-URL: Issues, https://github.com/spacinov/sipmessage/issues
```

### Comparing `sipmessage-0.2.0/src/sipmessage.egg-info/SOURCES.txt` & `sipmessage-0.2.1/src/sipmessage.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -8,17 +8,19 @@
 docs/conf.py
 docs/index.rst
 src/sipmessage/__init__.py
 src/sipmessage/address.py
 src/sipmessage/parameters.py
 src/sipmessage/py.typed
 src/sipmessage/uri.py
+src/sipmessage/via.py
 src/sipmessage.egg-info/PKG-INFO
 src/sipmessage.egg-info/SOURCES.txt
 src/sipmessage.egg-info/dependency_links.txt
 src/sipmessage.egg-info/requires.txt
 src/sipmessage.egg-info/top_level.txt
 tests/__init__.py
 tests/test_address.py
 tests/test_parameters.py
 tests/test_public_api.py
-tests/test_uri.py
+tests/test_uri.py
+tests/test_via.py
```

### Comparing `sipmessage-0.2.0/tests/test_address.py` & `sipmessage-0.2.1/tests/test_address.py`

 * *Files identical despite different names*

### Comparing `sipmessage-0.2.0/tests/test_parameters.py` & `sipmessage-0.2.1/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `sipmessage-0.2.0/tests/test_uri.py` & `sipmessage-0.2.1/tests/test_uri.py`

 * *Files identical despite different names*

