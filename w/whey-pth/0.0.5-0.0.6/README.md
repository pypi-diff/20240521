# Comparing `tmp/whey-pth-0.0.5.tar.gz` & `tmp/whey-pth-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whey-pth-0.0.5.tar", last modified: Thu Apr 20 14:10:15 2023, max compression
+gzip compressed data, was "whey-pth-0.0.6.tar", last modified: Tue May 21 09:29:46 2024, max compression
```

## Comparing `whey-pth-0.0.5.tar` & `whey-pth-0.0.6.tar`

### file list

```diff
@@ -1,22 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 14:10:15.795812 whey-pth-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (122)     1064 2023-04-20 14:09:44.000000 whey-pth-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      121 2023-04-20 14:09:44.000000 whey-pth-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     8323 2023-04-20 14:10:15.795812 whey-pth-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5417 2023-04-20 14:09:44.000000 whey-pth-0.0.5/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)     5110 2023-04-20 14:09:44.000000 whey-pth-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       29 2023-04-20 14:09:44.000000 whey-pth-0.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1609 2023-04-20 14:10:15.795812 whey-pth-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      589 2023-04-20 14:09:44.000000 whey-pth-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 14:10:15.791812 whey-pth-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (122)    12145 2023-04-20 14:09:44.000000 whey-pth-0.0.5/tests/test_whey_pth.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 14:10:15.795812 whey-pth-0.0.5/whey_pth/
--rw-r--r--   0 runner    (1001) docker     (122)     5307 2023-04-20 14:09:44.000000 whey-pth-0.0.5/whey_pth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 14:09:44.000000 whey-pth-0.0.5/whey_pth/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 14:10:15.795812 whey-pth-0.0.5/whey_pth.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     8323 2023-04-20 14:10:15.000000 whey-pth-0.0.5/whey_pth.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      368 2023-04-20 14:10:15.000000 whey-pth-0.0.5/whey_pth.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-20 14:10:15.000000 whey-pth-0.0.5/whey_pth.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       57 2023-04-20 14:10:15.000000 whey-pth-0.0.5/whey_pth.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-20 14:10:15.000000 whey-pth-0.0.5/whey_pth.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       29 2023-04-20 14:10:15.000000 whey-pth-0.0.5/whey_pth.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-04-20 14:10:15.000000 whey-pth-0.0.5/whey_pth.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:29:46.181174 whey-pth-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-21 09:29:20.000000 whey-pth-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-21 09:29:20.000000 whey-pth-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8374 2024-05-21 09:29:46.181174 whey-pth-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5417 2024-05-21 09:29:20.000000 whey-pth-0.0.6/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5111 2024-05-21 09:29:20.000000 whey-pth-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-21 09:29:20.000000 whey-pth-0.0.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-05-21 09:29:46.181174 whey-pth-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-21 09:29:20.000000 whey-pth-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:29:46.181174 whey-pth-0.0.6/whey_pth/
+-rw-r--r--   0 runner    (1001) docker     (127)     5567 2024-05-21 09:29:20.000000 whey-pth-0.0.6/whey_pth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:29:20.000000 whey-pth-0.0.6/whey_pth/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:29:46.181174 whey-pth-0.0.6/whey_pth.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8374 2024-05-21 09:29:46.000000 whey-pth-0.0.6/whey_pth.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-21 09:29:46.000000 whey-pth-0.0.6/whey_pth.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 09:29:46.000000 whey-pth-0.0.6/whey_pth.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-21 09:29:46.000000 whey-pth-0.0.6/whey_pth.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 09:29:46.000000 whey-pth-0.0.6/whey_pth.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-21 09:29:46.000000 whey-pth-0.0.6/whey_pth.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-21 09:29:46.000000 whey-pth-0.0.6/whey_pth.egg-info/top_level.txt
```

### Comparing `whey-pth-0.0.5/LICENSE` & `whey-pth-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `whey-pth-0.0.5/PKG-INFO` & `whey-pth-0.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whey-pth
-Version: 0.0.5
+Version: 0.0.6
 Summary: Extension to whey to support .pth files.
 Home-page: https://github.com/repo-helper/whey-pth
 Author: Dominic Davis-Foster
 Author-email: Dominic Davis-Foster <dominic@davis-foster.co.uk>
 License: Copyright (c) 2021 Dominic Davis-Foster
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -42,14 +42,15 @@
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
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Archiving :: Packaging
 Classifier: Typing :: Typed
 Requires-Python: >=3.6.1
@@ -155,23 +156,23 @@
 .. |license| image:: https://img.shields.io/github/license/repo-helper/whey-pth
 	:target: https://github.com/repo-helper/whey-pth/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/repo-helper/whey-pth
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/whey-pth/v0.0.5
+.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/whey-pth/v0.0.6
 	:target: https://github.com/repo-helper/whey-pth/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/repo-helper/whey-pth
 	:target: https://github.com/repo-helper/whey-pth/commit/master
 	:alt: GitHub last commit
 
-.. |maintained| image:: https://img.shields.io/maintenance/yes/2023
+.. |maintained| image:: https://img.shields.io/maintenance/yes/2024
 	:alt: Maintenance
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/whey-pth
 	:target: https://pypi.org/project/whey-pth/
 	:alt: PyPI - Downloads
 
 .. end shields
```

### Comparing `whey-pth-0.0.5/README.rst` & `whey-pth-0.0.6/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -97,23 +97,23 @@
 .. |license| image:: https://img.shields.io/github/license/repo-helper/whey-pth
 	:target: https://github.com/repo-helper/whey-pth/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/repo-helper/whey-pth
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/whey-pth/v0.0.5
+.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/whey-pth/v0.0.6
 	:target: https://github.com/repo-helper/whey-pth/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/repo-helper/whey-pth
 	:target: https://github.com/repo-helper/whey-pth/commit/master
 	:alt: GitHub last commit
 
-.. |maintained| image:: https://img.shields.io/maintenance/yes/2023
+.. |maintained| image:: https://img.shields.io/maintenance/yes/2024
 	:alt: Maintenance
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/whey-pth
 	:target: https://pypi.org/project/whey-pth/
 	:alt: PyPI - Downloads
 
 .. end shields
```

### Comparing `whey-pth-0.0.5/pyproject.toml` & `whey-pth-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = [ "setuptools!=61.*,>=40.6.0", "wheel>=0.34.2",]
+requires = [ "setuptools!=61.*,<=67.1.0,>=40.6.0", "wheel>=0.34.2",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "whey-pth"
-version = "0.0.5"
+version = "0.0.6"
 description = "Extension to whey to support .pth files."
 readme = "README.rst"
 requires-python = ">=3.6.1"
 keywords = [ "build", "distribution", "packaging", "wheel", "whey",]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Environment :: Console",
@@ -19,37 +19,40 @@
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
 Homepage = "https://github.com/repo-helper/whey-pth"
 "Issue Tracker" = "https://github.com/repo-helper/whey-pth/issues"
 "Source Code" = "https://github.com/repo-helper/whey-pth"
 Documentation = "https://whey-pth.readthedocs.io/en/latest"
 
+[project.entry-points."whey.builder"]
+whey_pth_wheel = "whey_pth:PthWheelBuilder"
+
 [tool.mkrecipe]
 conda-channels = [ "conda-forge", "domdfcoding",]
 extras = "all"
 license-key = "MIT"
 package = "whey_pth"
 
 [tool.sphinx-pyproject]
@@ -69,28 +72,26 @@
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
     "configconfig.autoconfig",
     "sphinx_toolbox.more_autosummary.column_widths",
     "sphinx_packaging.peps",
     "sphinx_packaging.toml",
 ]
-sphinxemoji_style = "twemoji"
 gitstamp_fmt = "%d %b %Y"
 templates_path = [ "_templates",]
 html_static_path = [ "_static",]
 source_suffix = ".rst"
 master_doc = "index"
 suppress_warnings = [ "image.nonlocal_uri",]
 pygments_style = "default"
@@ -141,15 +142,15 @@
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Build Tools",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: System :: Archiving :: Packaging",
     "Typing :: Typed",
 ]
-python-versions = [ "3.6", "3.7", "3.8", "3.9", "3.10", "3.11",]
+python-versions = [ "3.6", "3.7", "3.8", "3.9", "3.10", "3.11", "3.12",]
 python-implementations = [ "CPython", "PyPy",]
 platforms = [ "Windows", "macOS", "Linux",]
 license-key = "MIT"
 package = "whey_pth"
 
 [tool.mypy]
 python_version = "3.6"
@@ -158,35 +159,32 @@
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
 
-[project.entry-points."whey.builder"]
-whey_pth_wheel = "whey_pth:PthWheelBuilder"
-
 [tool.dependency-dash."requirements.txt"]
 order = 10
 
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

### Comparing `whey-pth-0.0.5/setup.cfg` & `whey-pth-0.0.6/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = whey-pth
-version = 0.0.5
+version = 0.0.6
 author = Dominic Davis-Foster
 author_email = dominic@davis-foster.co.uk
 license = MIT License
 keywords = whey, build, wheel, packaging, distribution
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 platforms = Windows, macOS, Linux
@@ -23,14 +23,15 @@
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
 	Topic :: Software Development :: Build Tools
 	Topic :: Software Development :: Libraries :: Python Modules
 	Topic :: System :: Archiving :: Packaging
 	Typing :: Typed
```

### Comparing `whey-pth-0.0.5/setup.py` & `whey-pth-0.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `whey-pth-0.0.5/whey_pth/__init__.py` & `whey-pth-0.0.6/whey_pth/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,20 +28,21 @@
 
 # stdlib
 from typing import Dict, List
 
 # 3rd party
 import dom_toml
 from dom_toml.parser import TOML_TYPES, AbstractConfigParser, BadConfigError
+from whey import additional_files
 from whey.builder import WheelBuilder
 
 __author__: str = "Dominic Davis-Foster"
 __copyright__: str = "2021 Dominic Davis-Foster"
 __license__: str = "MIT License"
-__version__: str = "0.0.5"
+__version__: str = "0.0.6"
 __email__: str = "dominic@davis-foster.co.uk"
 
 __all__ = ["PthWheelBuilder", "WheyPthParser"]
 
 
 class PthWheelBuilder(WheelBuilder):
 	"""
@@ -117,30 +118,40 @@
 
 		pth_content = config["pth-content"]
 
 		self.assert_type(pth_content, str, ["tool", "whey-pth", "pth-content"])
 
 		return pth_content
 
-	def parse_additional_wheel_files(self, config: Dict[str, TOML_TYPES]) -> List[str]:
+	def parse_additional_wheel_files(
+			self,
+			config: Dict[str, TOML_TYPES],
+			) -> List[additional_files.AdditionalFilesEntry]:
 		"""
 		Parse the ``additional-wheel-files`` key.
 
 		The value is a list of `MANIFEST.in <https://packaging.python.org/guides/using-manifest-in/>`_-style
 		entries for additional files to include in the wheel.
 
 		:param config: The unparsed TOML config for the ``[tool.whey-pth]`` table.
 		"""
 
-		additional_files = config["additional-wheel-files"]
+		entries = config["additional-wheel-files"]
 
-		for idx, file in enumerate(additional_files):
+		for idx, file in enumerate(entries):
 			self.assert_indexed_type(file, str, ["tool", "whey", "additional-wheel-files"], idx=idx)
 
-		return additional_files
+		parsed_additional_files = []
+
+		for entry in entries:
+			parsed_entry = additional_files.from_entry(entry)
+			if parsed_entry is not None:
+				parsed_additional_files.append(parsed_entry)
+
+		return parsed_additional_files
 
 	@property
 	def keys(self) -> List[str]:
 		"""
 		The keys to parse from the TOML file.
 		"""
```

### Comparing `whey-pth-0.0.5/whey_pth.egg-info/PKG-INFO` & `whey-pth-0.0.6/whey_pth.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whey-pth
-Version: 0.0.5
+Version: 0.0.6
 Summary: Extension to whey to support .pth files.
 Home-page: https://github.com/repo-helper/whey-pth
 Author: Dominic Davis-Foster
 Author-email: Dominic Davis-Foster <dominic@davis-foster.co.uk>
 License: Copyright (c) 2021 Dominic Davis-Foster
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -42,14 +42,15 @@
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
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Archiving :: Packaging
 Classifier: Typing :: Typed
 Requires-Python: >=3.6.1
@@ -155,23 +156,23 @@
 .. |license| image:: https://img.shields.io/github/license/repo-helper/whey-pth
 	:target: https://github.com/repo-helper/whey-pth/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/repo-helper/whey-pth
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/whey-pth/v0.0.5
+.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/whey-pth/v0.0.6
 	:target: https://github.com/repo-helper/whey-pth/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/repo-helper/whey-pth
 	:target: https://github.com/repo-helper/whey-pth/commit/master
 	:alt: GitHub last commit
 
-.. |maintained| image:: https://img.shields.io/maintenance/yes/2023
+.. |maintained| image:: https://img.shields.io/maintenance/yes/2024
 	:alt: Maintenance
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/whey-pth
 	:target: https://pypi.org/project/whey-pth/
 	:alt: PyPI - Downloads
 
 .. end shields
```

