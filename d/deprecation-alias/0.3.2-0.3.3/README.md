# Comparing `tmp/deprecation-alias-0.3.2.tar.gz` & `tmp/deprecation-alias-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deprecation-alias-0.3.2.tar", last modified: Tue May 23 15:55:02 2023, max compression
+gzip compressed data, was "deprecation-alias-0.3.3.tar", last modified: Tue May 21 09:33:49 2024, max compression
```

## Comparing `deprecation-alias-0.3.2.tar` & `deprecation-alias-0.3.3.tar`

### file list

```diff
@@ -1,21 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 15:55:02.863628 deprecation-alias-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (122)    10898 2023-05-23 15:54:35.000000 deprecation-alias-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      139 2023-05-23 15:54:35.000000 deprecation-alias-0.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    19145 2023-05-23 15:55:02.863628 deprecation-alias-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5057 2023-05-23 15:54:35.000000 deprecation-alias-0.3.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 15:55:02.863628 deprecation-alias-0.3.2/deprecation_alias/
--rw-r--r--   0 runner    (1001) docker     (122)     7753 2023-05-23 15:54:35.000000 deprecation-alias-0.3.2/deprecation_alias/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 15:54:35.000000 deprecation-alias-0.3.2/deprecation_alias/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 15:55:02.863628 deprecation-alias-0.3.2/deprecation_alias.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    19145 2023-05-23 15:55:02.000000 deprecation-alias-0.3.2/deprecation_alias.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      408 2023-05-23 15:55:02.000000 deprecation-alias-0.3.2/deprecation_alias.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-23 15:55:02.000000 deprecation-alias-0.3.2/deprecation_alias.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-23 15:55:02.000000 deprecation-alias-0.3.2/deprecation_alias.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       35 2023-05-23 15:55:02.000000 deprecation-alias-0.3.2/deprecation_alias.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-05-23 15:55:02.000000 deprecation-alias-0.3.2/deprecation_alias.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2676 2023-05-23 15:54:35.000000 deprecation-alias-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       35 2023-05-23 15:54:35.000000 deprecation-alias-0.3.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1383 2023-05-23 15:55:02.863628 deprecation-alias-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      639 2023-05-23 15:54:35.000000 deprecation-alias-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 15:55:02.863628 deprecation-alias-0.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     4961 2023-05-23 15:54:35.000000 deprecation-alias-0.3.2/tests/test_deprecation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:33:49.756632 deprecation-alias-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    10898 2024-05-21 09:33:25.000000 deprecation-alias-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-21 09:33:25.000000 deprecation-alias-0.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    19196 2024-05-21 09:33:49.756632 deprecation-alias-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5057 2024-05-21 09:33:25.000000 deprecation-alias-0.3.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:33:49.756632 deprecation-alias-0.3.3/deprecation_alias/
+-rw-r--r--   0 runner    (1001) docker     (127)     7753 2024-05-21 09:33:25.000000 deprecation-alias-0.3.3/deprecation_alias/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:33:25.000000 deprecation-alias-0.3.3/deprecation_alias/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:33:49.756632 deprecation-alias-0.3.3/deprecation_alias.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19196 2024-05-21 09:33:49.000000 deprecation-alias-0.3.3/deprecation_alias.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-21 09:33:49.000000 deprecation-alias-0.3.3/deprecation_alias.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 09:33:49.000000 deprecation-alias-0.3.3/deprecation_alias.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 09:33:49.000000 deprecation-alias-0.3.3/deprecation_alias.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-21 09:33:49.000000 deprecation-alias-0.3.3/deprecation_alias.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-21 09:33:49.000000 deprecation-alias-0.3.3/deprecation_alias.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-05-21 09:33:25.000000 deprecation-alias-0.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-21 09:33:25.000000 deprecation-alias-0.3.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-21 09:33:49.756632 deprecation-alias-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-21 09:33:25.000000 deprecation-alias-0.3.3/setup.py
```

### Comparing `deprecation-alias-0.3.2/LICENSE` & `deprecation-alias-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `deprecation-alias-0.3.2/PKG-INFO` & `deprecation-alias-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deprecation-alias
-Version: 0.3.2
+Version: 0.3.3
 Summary: A wrapper around 'deprecation' providing support for deprecated aliases.
 Home-page: https://github.com/domdfcoding/deprecation-alias
 Author: Dominic Davis-Foster
 Author-email: Dominic Davis-Foster <dominic@davis-foster.co.uk>
 License: Apache License
         Version 2.0, January 2004
         http://www.apache.org/licenses/
@@ -228,14 +228,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: >=3.6.1
 Description-Content-Type: text/x-rst
 License-File: LICENSE
@@ -329,23 +330,23 @@
 .. |license| image:: https://img.shields.io/github/license/domdfcoding/deprecation-alias
 	:target: https://github.com/domdfcoding/deprecation-alias/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/domdfcoding/deprecation-alias
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/deprecation-alias/v0.3.2
+.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/deprecation-alias/v0.3.3
 	:target: https://github.com/domdfcoding/deprecation-alias/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/domdfcoding/deprecation-alias
 	:target: https://github.com/domdfcoding/deprecation-alias/commit/master
 	:alt: GitHub last commit
 
-.. |maintained| image:: https://img.shields.io/maintenance/yes/2023
+.. |maintained| image:: https://img.shields.io/maintenance/yes/2024
 	:alt: Maintenance
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/deprecation-alias
 	:target: https://pypi.org/project/deprecation-alias/
 	:alt: PyPI - Downloads
 
 .. end shields
```

### Comparing `deprecation-alias-0.3.2/README.rst` & `deprecation-alias-0.3.3/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -87,23 +87,23 @@
 .. |license| image:: https://img.shields.io/github/license/domdfcoding/deprecation-alias
 	:target: https://github.com/domdfcoding/deprecation-alias/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/domdfcoding/deprecation-alias
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/deprecation-alias/v0.3.2
+.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/deprecation-alias/v0.3.3
 	:target: https://github.com/domdfcoding/deprecation-alias/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/domdfcoding/deprecation-alias
 	:target: https://github.com/domdfcoding/deprecation-alias/commit/master
 	:alt: GitHub last commit
 
-.. |maintained| image:: https://img.shields.io/maintenance/yes/2023
+.. |maintained| image:: https://img.shields.io/maintenance/yes/2024
 	:alt: Maintenance
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/deprecation-alias
 	:target: https://pypi.org/project/deprecation-alias/
 	:alt: PyPI - Downloads
 
 .. end shields
```

### Comparing `deprecation-alias-0.3.2/deprecation_alias/__init__.py` & `deprecation-alias-0.3.3/deprecation_alias/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 # 3rd party
 import deprecation  # type: ignore
 from packaging import version
 
 __author__: str = "Dominic Davis-Foster"
 __copyright__: str = "2020 Dominic Davis-Foster"
 __license__: str = "Apache Software License"
-__version__: str = "0.3.2"
+__version__: str = "0.3.3"
 __email__: str = "dominic@davis-foster.co.uk"
 
 __all__ = ["deprecated"]
 
 
 def deprecated(
 		deprecated_in: Optional[str] = None,
```

### Comparing `deprecation-alias-0.3.2/deprecation_alias.egg-info/PKG-INFO` & `deprecation-alias-0.3.3/deprecation_alias.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deprecation-alias
-Version: 0.3.2
+Version: 0.3.3
 Summary: A wrapper around 'deprecation' providing support for deprecated aliases.
 Home-page: https://github.com/domdfcoding/deprecation-alias
 Author: Dominic Davis-Foster
 Author-email: Dominic Davis-Foster <dominic@davis-foster.co.uk>
 License: Apache License
         Version 2.0, January 2004
         http://www.apache.org/licenses/
@@ -228,14 +228,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: >=3.6.1
 Description-Content-Type: text/x-rst
 License-File: LICENSE
@@ -329,23 +330,23 @@
 .. |license| image:: https://img.shields.io/github/license/domdfcoding/deprecation-alias
 	:target: https://github.com/domdfcoding/deprecation-alias/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/domdfcoding/deprecation-alias
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/deprecation-alias/v0.3.2
+.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/deprecation-alias/v0.3.3
 	:target: https://github.com/domdfcoding/deprecation-alias/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/domdfcoding/deprecation-alias
 	:target: https://github.com/domdfcoding/deprecation-alias/commit/master
 	:alt: GitHub last commit
 
-.. |maintained| image:: https://img.shields.io/maintenance/yes/2023
+.. |maintained| image:: https://img.shields.io/maintenance/yes/2024
 	:alt: Maintenance
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/deprecation-alias
 	:target: https://pypi.org/project/deprecation-alias/
 	:alt: PyPI - Downloads
 
 .. end shields
```

### Comparing `deprecation-alias-0.3.2/pyproject.toml` & `deprecation-alias-0.3.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = [ "setuptools!=61.*,>=40.6.0", "wheel>=0.34.2",]
+requires = [ "setuptools!=61.*,<=67.1.0,>=40.6.0", "wheel>=0.34.2",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "deprecation-alias"
-version = "0.3.2"
+version = "0.3.3"
 description = "A wrapper around 'deprecation' providing support for deprecated aliases."
 readme = "README.rst"
 requires-python = ">=3.6.1"
 keywords = [ "deprecation",]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
@@ -18,29 +18,29 @@
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Typing :: Typed",
 ]
 dynamic = [ "dependencies",]
 
+[project.license]
+file = "LICENSE"
+
 [[project.authors]]
 name = "Dominic Davis-Foster"
 email = "dominic@davis-foster.co.uk"
 
-
-[project.license]
-file = "LICENSE"
-
 [project.urls]
 Homepage = "https://github.com/domdfcoding/deprecation-alias"
 "Issue Tracker" = "https://github.com/domdfcoding/deprecation-alias/issues"
 "Source Code" = "https://github.com/domdfcoding/deprecation-alias"
 
 [tool.mkrecipe]
 conda-channels = [ "conda-forge", "domdfcoding",]
@@ -51,15 +51,15 @@
 [tool.whey]
 base-classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Typing :: Typed",
 ]
-python-versions = [ "3.6", "3.7", "3.8", "3.9", "3.10", "3.11",]
+python-versions = [ "3.6", "3.7", "3.8", "3.9", "3.10", "3.11", "3.12",]
 python-implementations = [ "CPython", "PyPy",]
 platforms = [ "Windows", "macOS", "Linux",]
 license-key = "Apache-2.0"
 package = "deprecation_alias"
 
 [tool.mypy]
 python_version = "3.8"
@@ -68,28 +68,28 @@
 warn_unused_ignores = true
 no_implicit_optional = true
 show_error_codes = true
 
 [tool.snippet-fmt]
 directives = [ "code-block",]
 
+[tool.snippet-fmt.languages.python]
+reformat = true
+
+[tool.snippet-fmt.languages.TOML]
+reformat = true
+
+[tool.snippet-fmt.languages.ini]
+
+[tool.snippet-fmt.languages.json]
+
 [tool.setuptools]
 zip-safe = false
 include-package-data = true
 platforms = [ "Windows", "macOS", "Linux",]
 
 [tool.dependency-dash."requirements.txt"]
 order = 10
 
 [tool.dependency-dash."tests/requirements.txt"]
 order = 20
 include = false
-
-[tool.snippet-fmt.languages.python]
-reformat = true
-
-[tool.snippet-fmt.languages.TOML]
-reformat = true
-
-[tool.snippet-fmt.languages.ini]
-
-[tool.snippet-fmt.languages.json]
```

### Comparing `deprecation-alias-0.3.2/setup.cfg` & `deprecation-alias-0.3.3/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = deprecation-alias
-version = 0.3.2
+version = 0.3.3
 author = Dominic Davis-Foster
 author_email = dominic@davis-foster.co.uk
 license = Apache Software License
 keywords = deprecation
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 platforms = Windows, macOS, Linux
@@ -21,14 +21,15 @@
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 	Programming Language :: Python :: Implementation :: CPython
 	Programming Language :: Python :: Implementation :: PyPy
 	Topic :: Software Development :: Libraries :: Python Modules
 	Typing :: Typed
 
 [options]
 python_requires = >=3.6.1
```

### Comparing `deprecation-alias-0.3.2/setup.py` & `deprecation-alias-0.3.3/setup.py`

 * *Files identical despite different names*

