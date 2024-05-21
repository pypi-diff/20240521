# Comparing `tmp/ccft_pymarkdown-1.1.0.tar.gz` & `tmp/ccft_pymarkdown-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccft_pymarkdown-1.1.0.tar", max compression
+gzip compressed data, was "ccft_pymarkdown-1.1.1.tar", max compression
```

## Comparing `ccft_pymarkdown-1.1.0.tar` & `ccft_pymarkdown-1.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11357 2024-05-16 17:31:40.444703 ccft_pymarkdown-1.1.0/LICENSE
--rw-r--r--   0        0        0     3298 2024-05-16 17:31:40.444703 ccft_pymarkdown-1.1.0/README.adoc
--rw-r--r--   0        0        0      706 2024-05-16 17:31:48.436737 ccft_pymarkdown-1.1.0/ccft_pymarkdown/__init__.py
--rw-r--r--   0        0        0      232 2024-05-16 17:31:40.444703 ccft_pymarkdown-1.1.0/ccft_pymarkdown/__main__.py
--rw-r--r--   0        0        0     2246 2024-05-16 17:31:40.444703 ccft_pymarkdown-1.1.0/ccft_pymarkdown/clean_custom_formatted_tables.py
--rw-r--r--   0        0        0     5096 2024-05-16 17:31:40.444703 ccft_pymarkdown-1.1.0/ccft_pymarkdown/console.py
--rw-r--r--   0        0        0      880 2024-05-16 17:31:40.444703 ccft_pymarkdown-1.1.0/ccft_pymarkdown/context_manager.py
--rw-r--r--   0        0        0     1088 2024-05-16 17:31:40.444703 ccft_pymarkdown-1.1.0/ccft_pymarkdown/restore_files.py
--rw-r--r--   0        0        0     1102 2024-05-16 17:31:40.444703 ccft_pymarkdown-1.1.0/ccft_pymarkdown/utils/__init__.py
--rw-r--r--   0        0        0     3977 2024-05-16 17:31:48.436737 ccft_pymarkdown-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     4480 1970-01-01 00:00:00.000000 ccft_pymarkdown-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-21 20:50:16.556413 ccft_pymarkdown-1.1.1/LICENSE
+-rw-r--r--   0        0        0     3298 2024-05-21 20:50:16.556413 ccft_pymarkdown-1.1.1/README.adoc
+-rw-r--r--   0        0        0      706 2024-05-21 20:50:24.220681 ccft_pymarkdown-1.1.1/ccft_pymarkdown/__init__.py
+-rw-r--r--   0        0        0      232 2024-05-21 20:50:16.556413 ccft_pymarkdown-1.1.1/ccft_pymarkdown/__main__.py
+-rw-r--r--   0        0        0     2246 2024-05-21 20:50:16.556413 ccft_pymarkdown-1.1.1/ccft_pymarkdown/clean_custom_formatted_tables.py
+-rw-r--r--   0        0        0     5096 2024-05-21 20:50:16.556413 ccft_pymarkdown-1.1.1/ccft_pymarkdown/console.py
+-rw-r--r--   0        0        0      880 2024-05-21 20:50:16.556413 ccft_pymarkdown-1.1.1/ccft_pymarkdown/context_manager.py
+-rw-r--r--   0        0        0     1088 2024-05-21 20:50:16.556413 ccft_pymarkdown-1.1.1/ccft_pymarkdown/restore_files.py
+-rw-r--r--   0        0        0     1102 2024-05-21 20:50:16.556413 ccft_pymarkdown-1.1.1/ccft_pymarkdown/utils/__init__.py
+-rw-r--r--   0        0        0     3977 2024-05-21 20:50:24.224681 ccft_pymarkdown-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4480 1970-01-01 00:00:00.000000 ccft_pymarkdown-1.1.1/PKG-INFO
```

### Comparing `ccft_pymarkdown-1.1.0/LICENSE` & `ccft_pymarkdown-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ccft_pymarkdown-1.1.0/README.adoc` & `ccft_pymarkdown-1.1.1/README.adoc`

 * *Files identical despite different names*

### Comparing `ccft_pymarkdown-1.1.0/ccft_pymarkdown/__init__.py` & `ccft_pymarkdown-1.1.1/ccft_pymarkdown/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 __all__: Sequence[str] = (
     "run",
     "restore_all_markdown_files",
     "clean_custom_formatted_tables_from_all_files",
     "clean_custom_formatted_tables_from_single_file",
     "CleanCustomFormattedTables",
 )
-__version__ = "v1.1.0"
+__version__ = "v1.1.1"
 
 
 from ccft_pymarkdown.clean_custom_formatted_tables import (
     clean_custom_formatted_tables_from_all_files,
     clean_custom_formatted_tables_from_single_file,
 )
 from ccft_pymarkdown.console import run
```

### Comparing `ccft_pymarkdown-1.1.0/ccft_pymarkdown/clean_custom_formatted_tables.py` & `ccft_pymarkdown-1.1.1/ccft_pymarkdown/clean_custom_formatted_tables.py`

 * *Files identical despite different names*

### Comparing `ccft_pymarkdown-1.1.0/ccft_pymarkdown/console.py` & `ccft_pymarkdown-1.1.1/ccft_pymarkdown/console.py`

 * *Files identical despite different names*

### Comparing `ccft_pymarkdown-1.1.0/ccft_pymarkdown/context_manager.py` & `ccft_pymarkdown-1.1.1/ccft_pymarkdown/context_manager.py`

 * *Files identical despite different names*

### Comparing `ccft_pymarkdown-1.1.0/ccft_pymarkdown/restore_files.py` & `ccft_pymarkdown-1.1.1/ccft_pymarkdown/restore_files.py`

 * *Files identical despite different names*

### Comparing `ccft_pymarkdown-1.1.0/ccft_pymarkdown/utils/__init__.py` & `ccft_pymarkdown-1.1.1/ccft_pymarkdown/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ccft_pymarkdown-1.1.0/pyproject.toml` & `ccft_pymarkdown-1.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "CCFT-PyMarkdown"
-version = "v1.1.0"
+version = "v1.1.1"
 license = "Apache-2.0"
 description = "A Python wrapper around jackdewinter's PyMarkdown linter to suppress errors, caused by custom-formatted tables in Markdown files"
 authors = ["Matt Norton <matt@carrotmanmatt.com>"]
 readme = "README.adoc"
 repository = "https://github.com/CarrotManMatt/ccft-pymarkdown.git"
 keywords = ["markdown", "linter", "static analysis"]
 classifiers = [
@@ -29,15 +29,15 @@
 ccft-pymarkdown = "ccft_pymarkdown.console:run"
 
 
 [tool.poetry.dependencies]
 python = "^3.12"
 pymarkdownlnt = "^0.9"
 gitpython = "^3.1"
-setuptools = "^69.5"
+setuptools = "^70.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.2"
 ruff = "^0.4"
 pre-commit = "^3.7"
 mypy = "^1.10"
 yamllint = "^1.35"
```

### Comparing `ccft_pymarkdown-1.1.0/PKG-INFO` & `ccft_pymarkdown-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CCFT-PyMarkdown
-Version: 1.1.0
+Version: 1.1.1
 Summary: A Python wrapper around jackdewinter's PyMarkdown linter to suppress errors, caused by custom-formatted tables in Markdown files
 Home-page: https://github.com/CarrotManMatt/ccft-pymarkdown.git
 License: Apache-2.0
 Keywords: markdown,linter,static analysis
 Author: Matt Norton
 Author-email: matt@carrotmanmatt.com
 Requires-Python: >=3.12,<4.0
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Text Processing :: Markup :: Markdown
 Classifier: Typing :: Typed
 Requires-Dist: gitpython (>=3.1,<4.0)
 Requires-Dist: pymarkdownlnt (>=0.9,<0.10)
-Requires-Dist: setuptools (>=69.5,<70.0)
+Requires-Dist: setuptools (>=70.0,<71.0)
 Project-URL: Repository, https://github.com/CarrotManMatt/ccft-pymarkdown.git
 Description-Content-Type: text/plain
 
 = CCFT-PyMarkdown
 Matthew Norton <matt@carrotmanmatt.com>
 v1.0, 02/05/2024
```

