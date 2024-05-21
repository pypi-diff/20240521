# Comparing `tmp/shippinglabel-1.7.1.tar.gz` & `tmp/shippinglabel-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shippinglabel-1.7.1.tar", last modified: Wed Jan 10 14:03:57 2024, max compression
+gzip compressed data, was "shippinglabel-1.7.2.tar", last modified: Tue May 21 09:27:01 2024, max compression
```

## Comparing `shippinglabel-1.7.1.tar` & `shippinglabel-1.7.2.tar`

### file list

```diff
@@ -1,43 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 14:03:57.948133 shippinglabel-1.7.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-01-10 14:03:32.000000 shippinglabel-1.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-01-10 14:03:32.000000 shippinglabel-1.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8488 2024-01-10 14:03:57.948133 shippinglabel-1.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-01-10 14:03:32.000000 shippinglabel-1.7.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5262 2024-01-10 14:03:32.000000 shippinglabel-1.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-01-10 14:03:32.000000 shippinglabel-1.7.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-01-10 14:03:57.948133 shippinglabel-1.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-01-10 14:03:32.000000 shippinglabel-1.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 14:03:57.944133 shippinglabel-1.7.1/shippinglabel/
--rw-r--r--   0 runner    (1001) docker     (127)     5295 2024-01-10 14:03:32.000000 shippinglabel-1.7.1/shippinglabel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 14:03:57.944133 shippinglabel-1.7.1/shippinglabel/_vendor/
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-01-10 14:03:32.000000 shippinglabel-1.7.1/shippinglabel/_vendor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-01-10 14:03:32.000000 shippinglabel-1.7.1/shippinglabel/_vendor/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 14:03:57.944133 shippinglabel-1.7.1/shippinglabel/_vendor/trove_classifiers/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-01-10 14:03:32.000000 shippinglabel-1.7.1/shippinglabel/_vendor/trove_classifiers/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    38727 2024-01-10 14:03:32.000000 shippinglabel-1.7.1/shippinglabel/_vendor/trove_classifiers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-01-10 14:03:32.000000 shippinglabel-1.7.1/shippinglabel/_vendor/trove_classifiers/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 14:03:32.000000 shippinglabel-1.7.1/shippinglabel/_vendor/trove_classifiers/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     4929 2024-01-10 14:03:32.000000 shippinglabel-1.7.1/shippinglabel/checksum.py
--rw-r--r--   0 runner    (1001) docker     (127)     4851 2024-01-10 14:03:32.000000 shippinglabel-1.7.1/shippinglabel/classifiers.py
--rw-r--r--   0 runner    (1001) docker     (127)     8539 2024-01-10 14:03:32.000000 shippinglabel-1.7.1/shippinglabel/conda.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 14:03:32.000000 shippinglabel-1.7.1/shippinglabel/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    10753 2024-01-10 14:03:32.000000 shippinglabel-1.7.1/shippinglabel/pypi.py
--rw-r--r--   0 runner    (1001) docker     (127)    22506 2024-01-10 14:03:32.000000 shippinglabel-1.7.1/shippinglabel/requirements.py
--rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-01-10 14:03:32.000000 shippinglabel-1.7.1/shippinglabel/sdist.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 14:03:57.948133 shippinglabel-1.7.1/shippinglabel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8488 2024-01-10 14:03:57.000000 shippinglabel-1.7.1/shippinglabel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-01-10 14:03:57.000000 shippinglabel-1.7.1/shippinglabel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-10 14:03:57.000000 shippinglabel-1.7.1/shippinglabel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-10 14:03:57.000000 shippinglabel-1.7.1/shippinglabel.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-01-10 14:03:57.000000 shippinglabel-1.7.1/shippinglabel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-01-10 14:03:57.000000 shippinglabel-1.7.1/shippinglabel.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 14:03:57.948133 shippinglabel-1.7.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-01-10 14:03:32.000000 shippinglabel-1.7.1/tests/test_checksum.py
--rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-01-10 14:03:32.000000 shippinglabel-1.7.1/tests/test_classifiers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7786 2024-01-10 14:03:32.000000 shippinglabel-1.7.1/tests/test_conda.py
--rw-r--r--   0 runner    (1001) docker     (127)    12774 2024-01-10 14:03:32.000000 shippinglabel-1.7.1/tests/test_pypi.py
--rw-r--r--   0 runner    (1001) docker     (127)    20056 2024-01-10 14:03:32.000000 shippinglabel-1.7.1/tests/test_requirements.py
--rw-r--r--   0 runner    (1001) docker     (127)     4705 2024-01-10 14:03:32.000000 shippinglabel-1.7.1/tests/test_requirements_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-01-10 14:03:32.000000 shippinglabel-1.7.1/tests/test_requirements_win.py
--rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-01-10 14:03:32.000000 shippinglabel-1.7.1/tests/test_sdist.py
--rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-01-10 14:03:32.000000 shippinglabel-1.7.1/tests/test_shippinglabel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:27:01.399535 shippinglabel-1.7.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-21 09:26:39.000000 shippinglabel-1.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-21 09:26:39.000000 shippinglabel-1.7.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8208 2024-05-21 09:27:01.399535 shippinglabel-1.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-05-21 09:26:39.000000 shippinglabel-1.7.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5209 2024-05-21 09:26:39.000000 shippinglabel-1.7.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-21 09:26:39.000000 shippinglabel-1.7.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-21 09:27:01.399535 shippinglabel-1.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-21 09:26:39.000000 shippinglabel-1.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:27:01.395535 shippinglabel-1.7.2/shippinglabel/
+-rw-r--r--   0 runner    (1001) docker     (127)     5295 2024-05-21 09:26:39.000000 shippinglabel-1.7.2/shippinglabel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:27:01.395535 shippinglabel-1.7.2/shippinglabel/_vendor/
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-21 09:26:39.000000 shippinglabel-1.7.2/shippinglabel/_vendor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-21 09:26:39.000000 shippinglabel-1.7.2/shippinglabel/_vendor/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:27:01.399535 shippinglabel-1.7.2/shippinglabel/_vendor/trove_classifiers/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-21 09:26:39.000000 shippinglabel-1.7.2/shippinglabel/_vendor/trove_classifiers/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    38727 2024-05-21 09:26:39.000000 shippinglabel-1.7.2/shippinglabel/_vendor/trove_classifiers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-21 09:26:39.000000 shippinglabel-1.7.2/shippinglabel/_vendor/trove_classifiers/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:26:39.000000 shippinglabel-1.7.2/shippinglabel/_vendor/trove_classifiers/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     4929 2024-05-21 09:26:39.000000 shippinglabel-1.7.2/shippinglabel/checksum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4851 2024-05-21 09:26:39.000000 shippinglabel-1.7.2/shippinglabel/classifiers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8539 2024-05-21 09:26:39.000000 shippinglabel-1.7.2/shippinglabel/conda.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:26:39.000000 shippinglabel-1.7.2/shippinglabel/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    10753 2024-05-21 09:26:39.000000 shippinglabel-1.7.2/shippinglabel/pypi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22506 2024-05-21 09:26:39.000000 shippinglabel-1.7.2/shippinglabel/requirements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-05-21 09:26:39.000000 shippinglabel-1.7.2/shippinglabel/sdist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:27:01.395535 shippinglabel-1.7.2/shippinglabel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8208 2024-05-21 09:27:01.000000 shippinglabel-1.7.2/shippinglabel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-21 09:27:01.000000 shippinglabel-1.7.2/shippinglabel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 09:27:01.000000 shippinglabel-1.7.2/shippinglabel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 09:27:01.000000 shippinglabel-1.7.2/shippinglabel.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-21 09:27:01.000000 shippinglabel-1.7.2/shippinglabel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-21 09:27:01.000000 shippinglabel-1.7.2/shippinglabel.egg-info/top_level.txt
```

### Comparing `shippinglabel-1.7.1/LICENSE` & `shippinglabel-1.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `shippinglabel-1.7.1/PKG-INFO` & `shippinglabel-1.7.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shippinglabel
-Version: 1.7.1
+Version: 1.7.2
 Summary: Utilities for handling packages.
 Home-page: https://github.com/domdfcoding/shippinglabel
 Author: Dominic Davis-Foster
 Author-email: Dominic Davis-Foster <dominic@davis-foster.co.uk>
 License: Copyright (c) 2020-2022 Dominic Davis-Foster
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -50,22 +50,14 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Archiving :: Packaging
 Classifier: Typing :: Typed
 Requires-Python: >=3.6.1
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: apeye>=1.0.0
-Requires-Dist: deprecation-alias>=0.3.2
-Requires-Dist: dist-meta>=0.1.2
-Requires-Dist: dom-toml>=0.2.2
-Requires-Dist: domdf-python-tools>=3.1.0
-Requires-Dist: packaging>=20.9
-Requires-Dist: platformdirs>=2.3.0
-Requires-Dist: typing-extensions>=3.7.4.3
 
 #############
 shippinglabel
 #############
 
 .. start short_desc
 
@@ -161,15 +153,15 @@
 .. |license| image:: https://img.shields.io/github/license/domdfcoding/shippinglabel
 	:target: https://github.com/domdfcoding/shippinglabel/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/domdfcoding/shippinglabel
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/shippinglabel/v1.7.1
+.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/shippinglabel/v1.7.2
 	:target: https://github.com/domdfcoding/shippinglabel/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/domdfcoding/shippinglabel
 	:target: https://github.com/domdfcoding/shippinglabel/commit/master
 	:alt: GitHub last commit
```

### Comparing `shippinglabel-1.7.1/README.rst` & `shippinglabel-1.7.2/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 .. |license| image:: https://img.shields.io/github/license/domdfcoding/shippinglabel
 	:target: https://github.com/domdfcoding/shippinglabel/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/domdfcoding/shippinglabel
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/shippinglabel/v1.7.1
+.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/shippinglabel/v1.7.2
 	:target: https://github.com/domdfcoding/shippinglabel/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/domdfcoding/shippinglabel
 	:target: https://github.com/domdfcoding/shippinglabel/commit/master
 	:alt: GitHub last commit
```

### Comparing `shippinglabel-1.7.1/pyproject.toml` & `shippinglabel-1.7.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = [ "setuptools!=61.*,>=40.6.0", "wheel>=0.34.2",]
+requires = [ "setuptools!=61.*,<=67.1.0,>=40.6.0", "wheel>=0.34.2",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "shippinglabel"
-version = "1.7.1"
+version = "1.7.2"
 description = "Utilities for handling packages."
 readme = "README.rst"
 requires-python = ">=3.6.1"
 keywords = [ "conda", "packaging", "pypi", "requirements",]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
@@ -27,22 +27,21 @@
     "Programming Language :: Python :: Implementation :: PyPy",
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
 Homepage = "https://github.com/domdfcoding/shippinglabel"
 "Issue Tracker" = "https://github.com/domdfcoding/shippinglabel/issues"
 "Source Code" = "https://github.com/domdfcoding/shippinglabel"
 Documentation = "https://shippinglabel.readthedocs.io/en/latest"
 
 [tool.mkrecipe]
@@ -67,28 +66,26 @@
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
     "sphinx_toolbox.more_autosummary.column_widths",
     "sphinx_packaging.peps",
     "sphinx_toolbox_experimental.missing_xref",
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
@@ -154,14 +151,24 @@
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
 [tool.vendoring]
 destination = "shippinglabel/_vendor/"
 requirements = "shippinglabel/_vendor/requirements.txt"
 namespace = "shippinglabel._vendor"
 protected-files = [ "__init__.py", "README.rst", "requirements.txt",]
 
 [tool.setuptools]
@@ -175,17 +182,7 @@
 [tool.dependency-dash."tests/requirements.txt"]
 order = 20
 include = false
 
 [tool.dependency-dash."doc-source/requirements.txt"]
 order = 30
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

### Comparing `shippinglabel-1.7.1/setup.cfg` & `shippinglabel-1.7.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = shippinglabel
-version = 1.7.1
+version = 1.7.2
 author = Dominic Davis-Foster
 author_email = dominic@davis-foster.co.uk
 license = MIT License
 keywords = packaging, requirements, pypi, conda
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 platforms = Windows, macOS, Linux
```

### Comparing `shippinglabel-1.7.1/setup.py` & `shippinglabel-1.7.2/setup.py`

 * *Files identical despite different names*

### Comparing `shippinglabel-1.7.1/shippinglabel/__init__.py` & `shippinglabel-1.7.2/shippinglabel/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 		"read_pyvenv",
 		"get_project_links",
 		]
 
 __author__: str = "Dominic Davis-Foster"
 __copyright__: str = "2020 Dominic Davis-Foster"
 __license__: str = "MIT License"
-__version__: str = "1.7.1"
+__version__: str = "1.7.2"
 __email__: str = "dominic@davis-foster.co.uk"
 
 
 def no_dev_versions(versions: Iterable[str]) -> List[str]:
 	"""
 	Returns the subset of ``versions`` which does not end with ``-dev``.
```

### Comparing `shippinglabel-1.7.1/shippinglabel/_vendor/trove_classifiers/LICENSE` & `shippinglabel-1.7.2/shippinglabel/_vendor/trove_classifiers/LICENSE`

 * *Files identical despite different names*

### Comparing `shippinglabel-1.7.1/shippinglabel/_vendor/trove_classifiers/__init__.py` & `shippinglabel-1.7.2/shippinglabel/_vendor/trove_classifiers/__init__.py`

 * *Files identical despite different names*

### Comparing `shippinglabel-1.7.1/shippinglabel/checksum.py` & `shippinglabel-1.7.2/shippinglabel/checksum.py`

 * *Files identical despite different names*

### Comparing `shippinglabel-1.7.1/shippinglabel/classifiers.py` & `shippinglabel-1.7.2/shippinglabel/classifiers.py`

 * *Files identical despite different names*

### Comparing `shippinglabel-1.7.1/shippinglabel/conda.py` & `shippinglabel-1.7.2/shippinglabel/conda.py`

 * *Files identical despite different names*

### Comparing `shippinglabel-1.7.1/shippinglabel/pypi.py` & `shippinglabel-1.7.2/shippinglabel/pypi.py`

 * *Files identical despite different names*

### Comparing `shippinglabel-1.7.1/shippinglabel/requirements.py` & `shippinglabel-1.7.2/shippinglabel/requirements.py`

 * *Files identical despite different names*

### Comparing `shippinglabel-1.7.1/shippinglabel/sdist.py` & `shippinglabel-1.7.2/shippinglabel/sdist.py`

 * *Files identical despite different names*

### Comparing `shippinglabel-1.7.1/shippinglabel.egg-info/PKG-INFO` & `shippinglabel-1.7.2/shippinglabel.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shippinglabel
-Version: 1.7.1
+Version: 1.7.2
 Summary: Utilities for handling packages.
 Home-page: https://github.com/domdfcoding/shippinglabel
 Author: Dominic Davis-Foster
 Author-email: Dominic Davis-Foster <dominic@davis-foster.co.uk>
 License: Copyright (c) 2020-2022 Dominic Davis-Foster
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -50,22 +50,14 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Archiving :: Packaging
 Classifier: Typing :: Typed
 Requires-Python: >=3.6.1
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: apeye>=1.0.0
-Requires-Dist: deprecation-alias>=0.3.2
-Requires-Dist: dist-meta>=0.1.2
-Requires-Dist: dom-toml>=0.2.2
-Requires-Dist: domdf-python-tools>=3.1.0
-Requires-Dist: packaging>=20.9
-Requires-Dist: platformdirs>=2.3.0
-Requires-Dist: typing-extensions>=3.7.4.3
 
 #############
 shippinglabel
 #############
 
 .. start short_desc
 
@@ -161,15 +153,15 @@
 .. |license| image:: https://img.shields.io/github/license/domdfcoding/shippinglabel
 	:target: https://github.com/domdfcoding/shippinglabel/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/domdfcoding/shippinglabel
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/shippinglabel/v1.7.1
+.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/shippinglabel/v1.7.2
 	:target: https://github.com/domdfcoding/shippinglabel/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/domdfcoding/shippinglabel
 	:target: https://github.com/domdfcoding/shippinglabel/commit/master
 	:alt: GitHub last commit
```

### Comparing `shippinglabel-1.7.1/shippinglabel.egg-info/SOURCES.txt` & `shippinglabel-1.7.2/shippinglabel.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -20,17 +20,8 @@
 shippinglabel.egg-info/requires.txt
 shippinglabel.egg-info/top_level.txt
 shippinglabel/_vendor/__init__.py
 shippinglabel/_vendor/requirements.txt
 shippinglabel/_vendor/trove_classifiers/LICENSE
 shippinglabel/_vendor/trove_classifiers/__init__.py
 shippinglabel/_vendor/trove_classifiers/__main__.py
-shippinglabel/_vendor/trove_classifiers/py.typed
-tests/test_checksum.py
-tests/test_classifiers.py
-tests/test_conda.py
-tests/test_pypi.py
-tests/test_requirements.py
-tests/test_requirements_manager.py
-tests/test_requirements_win.py
-tests/test_sdist.py
-tests/test_shippinglabel.py
+shippinglabel/_vendor/trove_classifiers/py.typed
```

