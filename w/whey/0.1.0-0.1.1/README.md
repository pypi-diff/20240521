# Comparing `tmp/whey-0.1.0.tar.gz` & `tmp/whey-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whey-0.1.0.tar", last modified: Mon Apr  8 21:45:33 2024, max compression
+gzip compressed data, was "whey-0.1.1.tar", last modified: Tue May 21 09:28:06 2024, max compression
```

## Comparing `whey-0.1.0.tar` & `whey-0.1.1.tar`

### file list

```diff
@@ -1,39 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:45:33.356426 whey-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-08 21:45:04.000000 whey-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-08 21:45:04.000000 whey-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9704 2024-04-08 21:45:33.356426 whey-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5982 2024-04-08 21:45:04.000000 whey-0.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-08 21:45:04.000000 whey-0.1.0/__pkginfo__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5558 2024-04-08 21:45:04.000000 whey-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-08 21:45:04.000000 whey-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-08 21:45:33.356426 whey-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-08 21:45:04.000000 whey-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:45:33.352426 whey-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    43090 2024-04-08 21:45:04.000000 whey-0.1.0/tests/test_build.py
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-04-08 21:45:04.000000 whey-0.1.0/tests/test_builder_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)    21136 2024-04-08 21:45:04.000000 whey-0.1.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    28981 2024-04-08 21:45:04.000000 whey-0.1.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8303 2024-04-08 21:45:04.000000 whey-0.1.0/tests/test_foreman.py
--rw-r--r--   0 runner    (1001) docker     (127)    11785 2024-04-08 21:45:04.000000 whey-0.1.0/tests/test_pep517_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-04-08 21:45:04.000000 whey-0.1.0/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:45:33.352426 whey-0.1.0/whey/
--rw-r--r--   0 runner    (1001) docker     (127)     4678 2024-04-08 21:45:04.000000 whey-0.1.0/whey/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5150 2024-04-08 21:45:04.000000 whey-0.1.0/whey/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-08 21:45:04.000000 whey-0.1.0/whey/_editable.py
--rw-r--r--   0 runner    (1001) docker     (127)     7682 2024-04-08 21:45:04.000000 whey-0.1.0/whey/additional_files.py
--rw-r--r--   0 runner    (1001) docker     (127)    27105 2024-04-08 21:45:04.000000 whey-0.1.0/whey/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:45:33.356426 whey-0.1.0/whey/config/
--rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-04-08 21:45:04.000000 whey-0.1.0/whey/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-04-08 21:45:04.000000 whey-0.1.0/whey/config/pep621.py
--rw-r--r--   0 runner    (1001) docker     (127)    12864 2024-04-08 21:45:04.000000 whey-0.1.0/whey/config/whey.py
--rw-r--r--   0 runner    (1001) docker     (127)     4014 2024-04-08 21:45:04.000000 whey-0.1.0/whey/foreman.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 21:45:04.000000 whey-0.1.0/whey/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-04-08 21:45:04.000000 whey-0.1.0/whey/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:45:33.356426 whey-0.1.0/whey.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9704 2024-04-08 21:45:33.000000 whey-0.1.0/whey.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-08 21:45:33.000000 whey-0.1.0/whey.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 21:45:33.000000 whey-0.1.0/whey.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-08 21:45:33.000000 whey-0.1.0/whey.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 21:45:33.000000 whey-0.1.0/whey.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-08 21:45:33.000000 whey-0.1.0/whey.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-08 21:45:33.000000 whey-0.1.0/whey.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:28:06.955716 whey-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-21 09:27:42.000000 whey-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-21 09:27:42.000000 whey-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9008 2024-05-21 09:28:06.955716 whey-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5982 2024-05-21 09:27:42.000000 whey-0.1.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-21 09:27:42.000000 whey-0.1.1/__pkginfo__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5505 2024-05-21 09:27:42.000000 whey-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-21 09:27:42.000000 whey-0.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-05-21 09:28:06.955716 whey-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-21 09:27:42.000000 whey-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:28:06.955716 whey-0.1.1/whey/
+-rw-r--r--   0 runner    (1001) docker     (127)     4678 2024-05-21 09:27:42.000000 whey-0.1.1/whey/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5150 2024-05-21 09:27:42.000000 whey-0.1.1/whey/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-05-21 09:27:42.000000 whey-0.1.1/whey/_editable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7682 2024-05-21 09:27:42.000000 whey-0.1.1/whey/additional_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27105 2024-05-21 09:27:42.000000 whey-0.1.1/whey/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:28:06.955716 whey-0.1.1/whey/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-05-21 09:27:42.000000 whey-0.1.1/whey/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-05-21 09:27:42.000000 whey-0.1.1/whey/config/pep621.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12864 2024-05-21 09:27:42.000000 whey-0.1.1/whey/config/whey.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4014 2024-05-21 09:27:42.000000 whey-0.1.1/whey/foreman.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:27:42.000000 whey-0.1.1/whey/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-05-21 09:27:42.000000 whey-0.1.1/whey/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:28:06.955716 whey-0.1.1/whey.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9008 2024-05-21 09:28:06.000000 whey-0.1.1/whey.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-21 09:28:06.000000 whey-0.1.1/whey.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 09:28:06.000000 whey-0.1.1/whey.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-21 09:28:06.000000 whey-0.1.1/whey.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 09:28:06.000000 whey-0.1.1/whey.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-21 09:28:06.000000 whey-0.1.1/whey.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-21 09:28:06.000000 whey-0.1.1/whey.egg-info/top_level.txt
```

### Comparing `whey-0.1.0/LICENSE` & `whey-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `whey-0.1.0/PKG-INFO` & `whey-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whey
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple Python wheel builder for simple projects.
 Home-page: https://github.com/repo-helper/whey
 Author: Dominic Davis-Foster
 Author-email: Dominic Davis-Foster <dominic@davis-foster.co.uk>
 License: Copyright (c) 2021 Dominic Davis-Foster
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -51,35 +51,18 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Archiving :: Packaging
 Classifier: Typing :: Typed
 Requires-Python: >=3.6.1
 Description-Content-Type: text/x-rst
-License-File: LICENSE
-Requires-Dist: attrs>=22.2.0
-Requires-Dist: click>=7.1.2
-Requires-Dist: consolekit>=1.4.1
-Requires-Dist: dist-meta>=0.1.0
-Requires-Dist: dom-toml>=2.0.0
-Requires-Dist: domdf-python-tools>=2.8.0
-Requires-Dist: handy-archives>=0.2.0
-Requires-Dist: natsort>=7.1.1
-Requires-Dist: packaging>=20.9
-Requires-Dist: pyproject-parser>=0.11.0
-Requires-Dist: shippinglabel>=0.16.0
 Provides-Extra: readme
-Requires-Dist: docutils>=0.16; extra == "readme"
-Requires-Dist: pyproject-parser[readme]>=0.11.0b1; extra == "readme"
 Provides-Extra: editable
-Requires-Dist: editables>=0.2; extra == "editable"
 Provides-Extra: all
-Requires-Dist: docutils>=0.16; extra == "all"
-Requires-Dist: editables>=0.2; extra == "all"
-Requires-Dist: pyproject-parser[readme]>=0.11.0b1; extra == "all"
+License-File: LICENSE
 
 #####
 whey
 #####
 
 .. start short_desc
 
@@ -194,15 +177,15 @@
 .. |license| image:: https://img.shields.io/github/license/repo-helper/whey
 	:target: https://github.com/repo-helper/whey/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/repo-helper/whey
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/whey/v0.1.0
+.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/whey/v0.1.1
 	:target: https://github.com/repo-helper/whey/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/repo-helper/whey
 	:target: https://github.com/repo-helper/whey/commit/master
 	:alt: GitHub last commit
```

### Comparing `whey-0.1.0/README.rst` & `whey-0.1.1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -115,15 +115,15 @@
 .. |license| image:: https://img.shields.io/github/license/repo-helper/whey
 	:target: https://github.com/repo-helper/whey/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/repo-helper/whey
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/whey/v0.1.0
+.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/whey/v0.1.1
 	:target: https://github.com/repo-helper/whey/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/repo-helper/whey
 	:target: https://github.com/repo-helper/whey/commit/master
 	:alt: GitHub last commit
```

### Comparing `whey-0.1.0/pyproject.toml` & `whey-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = [ "setuptools!=61.*,>=40.6.0", "wheel>=0.34.2",]
+requires = [ "setuptools!=61.*,<=67.1.0,>=40.6.0", "wheel>=0.34.2",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "whey"
-version = "0.1.0"
+version = "0.1.1"
 description = "A simple Python wheel builder for simple projects."
 readme = "README.rst"
 requires-python = ">=3.6.1"
 keywords = [ "build", "distribution", "packaging", "pep517", "pep621", "sdist", "wheel",]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Environment :: Console",
@@ -29,31 +29,34 @@
     "Topic :: Software Development :: Build Tools",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: System :: Archiving :: Packaging",
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
 Homepage = "https://github.com/repo-helper/whey"
 "Issue Tracker" = "https://github.com/repo-helper/whey/issues"
 "Source Code" = "https://github.com/repo-helper/whey"
 Documentation = "https://whey.readthedocs.io/en/latest"
 
 [project.scripts]
 whey = "whey.__main__:main"
 
+[project.entry-points."whey.builder"]
+whey_sdist = "whey.builder:SDistBuilder"
+whey_wheel = "whey.builder:WheelBuilder"
+
 [project.optional-dependencies]
 readme = [ "docutils>=0.16", "pyproject-parser[readme]>=0.11.0b1",]
 editable = [ "editables>=0.2",]
 all = [ "docutils>=0.16", "editables>=0.2", "pyproject-parser[readme]>=0.11.0b1",]
 
 [tool.mkrecipe]
 conda-channels = [ "conda-forge", "domdfcoding",]
@@ -77,30 +80,28 @@
     "sphinxcontrib.toctree_plus",
     "sphinx_toolbox.tweaks.latex_layout",
     "sphinx_toolbox.tweaks.latex_toc",
     "sphinx.ext.intersphinx",
     "sphinx.ext.mathjax",
     "sphinxcontrib.extras_require",
     "sphinx.ext.todo",
-    "sphinxemoji.sphinxemoji",
     "notfound.extension",
     "sphinx_copybutton",
     "sphinxcontrib.default_values",
     "sphinx_debuginfo",
     "sphinx_licenseinfo",
     "seed_intersphinx_mapping",
     "html_section",
     "cli_extension",
     "sphinx_toolbox.more_autosummary.column_widths",
     "sphinx_toolbox_experimental.download_icon",
     "sphinx_packaging",
     "attr_utils.autoattrs",
     "local_extension",
 ]
-sphinxemoji_style = "twemoji"
 gitstamp_fmt = "%d %b %Y"
 templates_path = [ "_templates",]
 html_static_path = [ "_static",]
 source_suffix = ".rst"
 master_doc = "index"
 suppress_warnings = [ "image.nonlocal_uri",]
 pygments_style = "default"
@@ -167,41 +168,37 @@
 warn_unused_ignores = true
 no_implicit_optional = true
 show_error_codes = true
 
 [tool.snippet-fmt]
 directives = [ "code-block",]
 
+[tool.snippet-fmt.languages.python]
+reformat = true
+
+[tool.snippet-fmt.languages.toml]
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
 
-[project.entry-points."whey.builder"]
-whey_sdist = "whey.builder:SDistBuilder"
-whey_wheel = "whey.builder:WheelBuilder"
-
 [tool.dependency-dash."requirements.txt"]
 order = 10
 
 [tool.dependency-dash."tests/requirements.txt"]
 order = 20
 include = false
 
 [tool.dependency-dash."doc-source/requirements.txt"]
 order = 30
 include = false
 
 [tool.dep_checker.name_mapping]
 attrs = "attr"
-
-[tool.snippet-fmt.languages.python]
-reformat = true
-
-[tool.snippet-fmt.languages.toml]
-
-[tool.snippet-fmt.languages.TOML]
-reformat = true
-
-[tool.snippet-fmt.languages.ini]
-
-[tool.snippet-fmt.languages.json]
```

### Comparing `whey-0.1.0/setup.cfg` & `whey-0.1.1/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = whey
-version = 0.1.0
+version = 0.1.1
 author = Dominic Davis-Foster
 author_email = dominic@davis-foster.co.uk
 license = MIT License
 keywords = pep517, pep621, build, sdist, wheel, packaging, distribution
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 platforms = Windows, macOS, Linux
```

### Comparing `whey-0.1.0/setup.py` & `whey-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `whey-0.1.0/whey/__init__.py` & `whey-0.1.1/whey/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 # stdlib
 import os
 
 __author__: str = "Dominic Davis-Foster"
 __copyright__: str = "2021 Dominic Davis-Foster"
 __license__: str = "MIT License"
-__version__: str = "0.1.0"
+__version__: str = "0.1.1"
 __email__: str = "dominic@davis-foster.co.uk"
 
 __all__ = ("build_sdist", "build_wheel")
 
 
 def build_wheel(wheel_directory, config_settings=None, metadata_directory=None) -> str:  # noqa: MAN001
 	"""
```

### Comparing `whey-0.1.0/whey/__main__.py` & `whey-0.1.1/whey/__main__.py`

 * *Files identical despite different names*

### Comparing `whey-0.1.0/whey/_editable.py` & `whey-0.1.1/whey/_editable.py`

 * *Files identical despite different names*

### Comparing `whey-0.1.0/whey/additional_files.py` & `whey-0.1.1/whey/additional_files.py`

 * *Files identical despite different names*

### Comparing `whey-0.1.0/whey/builder.py` & `whey-0.1.1/whey/builder.py`

 * *Files identical despite different names*

### Comparing `whey-0.1.0/whey/config/__init__.py` & `whey-0.1.1/whey/config/__init__.py`

 * *Files identical despite different names*

### Comparing `whey-0.1.0/whey/config/pep621.py` & `whey-0.1.1/whey/config/pep621.py`

 * *Files identical despite different names*

### Comparing `whey-0.1.0/whey/config/whey.py` & `whey-0.1.1/whey/config/whey.py`

 * *Files identical despite different names*

### Comparing `whey-0.1.0/whey/foreman.py` & `whey-0.1.1/whey/foreman.py`

 * *Files identical despite different names*

### Comparing `whey-0.1.0/whey/utils.py` & `whey-0.1.1/whey/utils.py`

 * *Files identical despite different names*

### Comparing `whey-0.1.0/whey.egg-info/PKG-INFO` & `whey-0.1.1/whey.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whey
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple Python wheel builder for simple projects.
 Home-page: https://github.com/repo-helper/whey
 Author: Dominic Davis-Foster
 Author-email: Dominic Davis-Foster <dominic@davis-foster.co.uk>
 License: Copyright (c) 2021 Dominic Davis-Foster
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -51,35 +51,18 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Archiving :: Packaging
 Classifier: Typing :: Typed
 Requires-Python: >=3.6.1
 Description-Content-Type: text/x-rst
-License-File: LICENSE
-Requires-Dist: attrs>=22.2.0
-Requires-Dist: click>=7.1.2
-Requires-Dist: consolekit>=1.4.1
-Requires-Dist: dist-meta>=0.1.0
-Requires-Dist: dom-toml>=2.0.0
-Requires-Dist: domdf-python-tools>=2.8.0
-Requires-Dist: handy-archives>=0.2.0
-Requires-Dist: natsort>=7.1.1
-Requires-Dist: packaging>=20.9
-Requires-Dist: pyproject-parser>=0.11.0
-Requires-Dist: shippinglabel>=0.16.0
 Provides-Extra: readme
-Requires-Dist: docutils>=0.16; extra == "readme"
-Requires-Dist: pyproject-parser[readme]>=0.11.0b1; extra == "readme"
 Provides-Extra: editable
-Requires-Dist: editables>=0.2; extra == "editable"
 Provides-Extra: all
-Requires-Dist: docutils>=0.16; extra == "all"
-Requires-Dist: editables>=0.2; extra == "all"
-Requires-Dist: pyproject-parser[readme]>=0.11.0b1; extra == "all"
+License-File: LICENSE
 
 #####
 whey
 #####
 
 .. start short_desc
 
@@ -194,15 +177,15 @@
 .. |license| image:: https://img.shields.io/github/license/repo-helper/whey
 	:target: https://github.com/repo-helper/whey/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/repo-helper/whey
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/whey/v0.1.0
+.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/whey/v0.1.1
 	:target: https://github.com/repo-helper/whey/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/repo-helper/whey
 	:target: https://github.com/repo-helper/whey/commit/master
 	:alt: GitHub last commit
```

