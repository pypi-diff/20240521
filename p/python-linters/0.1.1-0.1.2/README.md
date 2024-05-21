# Comparing `tmp/python_linters-0.1.1.tar.gz` & `tmp/python_linters-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_linters-0.1.1.tar", max compression
+gzip compressed data, was "python_linters-0.1.2.tar", max compression
```

## Comparing `python_linters-0.1.1.tar` & `python_linters-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     8595 2024-03-17 16:01:25.101519 python_linters-0.1.1/README.md
--rw-r--r--   0        0        0     1018 2024-03-17 16:01:34.993464 python_linters-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2960 2024-03-17 16:01:25.101519 python_linters-0.1.1/python_linters/.flake8
--rw-r--r--   0        0        0        0 2024-03-17 16:01:25.101519 python_linters-0.1.1/python_linters/__init__.py
--rw-r--r--   0        0        0      859 2024-03-17 16:01:25.101519 python_linters-0.1.1/python_linters/add_noqa.py
--rw-r--r--   0        0        0      758 2024-03-17 16:01:25.101519 python_linters-0.1.1/python_linters/fix_code.py
--rw-r--r--   0        0        0      531 2024-03-17 16:01:25.101519 python_linters-0.1.1/python_linters/parse_rules.py
--rw-r--r--   0        0        0     7153 2024-03-17 16:01:25.101519 python_linters-0.1.1/python_linters/ruff.toml
--rw-r--r--   0        0        0     1647 2024-03-17 16:01:25.101519 python_linters-0.1.1/python_linters/ruff_rule_categories.py
--rw-r--r--   0        0        0    75528 2024-03-17 16:01:25.101519 python_linters-0.1.1/python_linters/ruff_rules.txt
--rw-r--r--   0        0        0     3466 2024-03-17 16:01:25.101519 python_linters-0.1.1/python_linters/run_linters.py
--rw-r--r--   0        0        0     9430 1970-01-01 00:00:00.000000 python_linters-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-05-21 06:39:18.689597 python_linters-0.1.2/LICENSE
+-rw-r--r--   0        0        0     8928 2024-05-21 06:39:18.689597 python_linters-0.1.2/README.md
+-rw-r--r--   0        0        0      963 2024-05-21 06:39:30.665487 python_linters-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2960 2024-05-21 06:39:18.689597 python_linters-0.1.2/python_linters/.flake8
+-rw-r--r--   0        0        0        0 2024-05-21 06:39:18.689597 python_linters-0.1.2/python_linters/__init__.py
+-rw-r--r--   0        0        0      859 2024-05-21 06:39:18.689597 python_linters-0.1.2/python_linters/add_noqa.py
+-rw-r--r--   0        0        0      758 2024-05-21 06:39:18.689597 python_linters-0.1.2/python_linters/fix_code.py
+-rw-r--r--   0        0        0      531 2024-05-21 06:39:18.689597 python_linters-0.1.2/python_linters/parse_rules.py
+-rw-r--r--   0        0        0     7364 2024-05-21 06:39:18.689597 python_linters-0.1.2/python_linters/ruff.toml
+-rw-r--r--   0        0        0     1647 2024-05-21 06:39:18.689597 python_linters-0.1.2/python_linters/ruff_rule_categories.py
+-rw-r--r--   0        0        0    75528 2024-05-21 06:39:18.689597 python_linters-0.1.2/python_linters/ruff_rules.txt
+-rw-r--r--   0        0        0     3466 2024-05-21 06:39:18.689597 python_linters-0.1.2/python_linters/run_linters.py
+-rw-r--r--   0        0        0     9763 1970-01-01 00:00:00.000000 python_linters-0.1.2/PKG-INFO
```

### Comparing `python_linters-0.1.1/README.md` & `python_linters-0.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+![pypi](https://github.com/dertilo/python-linters/actions/workflows/release.yml/badge.svg)
+[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
+[![bear-ified](https://raw.githubusercontent.com/beartype/beartype-assets/main/badge/bear-ified.svg)](https://beartype.readthedocs.io)
 # python-linters
 - bundles flake8, black, isort, ruff into a single poetry-script
 - project independent linter configuration (via `ruff.toml`,`.flake8`) -> one config to rule them all
 ### use-cases:
 1. interactively learning python code quality standards via ruff+flake8, see [local development workflow](#2-local-development-workflow-before-pushing-to-ci-pipeline)
 2. enforcing minimal quality-standards via a "lint-stage" in a ci-pipeline, see [setup for ci-pipeline](#3-setup-for-ci-pipeline)
```

### Comparing `python_linters-0.1.1/pyproject.toml` & `python_linters-0.1.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 [tool.poetry]
 name = "python-linters"
-version = "0.1.1"
+version = "0.1.2"
 description = "bundling config files for linters like ruff and flake8"
 authors = ["Tilo Himmelsbach <dertilo@gmail.com>"]
 readme = "README.md"
-homepage = "https://github.com/dertilo/python-linters"
 repository = "https://github.com/dertilo/python-linters"
 packages = [{ include = "python_linters" }]
 
 include=["python_linters/.flake8","python_linters/ruff.toml"]
 
 [tool.poetry.scripts]
 pythonlinter = 'python_linters.run_linters:main'
```

### Comparing `python_linters-0.1.1/python_linters/.flake8` & `python_linters-0.1.2/python_linters/.flake8`

 * *Files identical despite different names*

### Comparing `python_linters-0.1.1/python_linters/add_noqa.py` & `python_linters-0.1.2/python_linters/add_noqa.py`

 * *Files identical despite different names*

### Comparing `python_linters-0.1.1/python_linters/fix_code.py` & `python_linters-0.1.2/python_linters/fix_code.py`

 * *Files identical despite different names*

### Comparing `python_linters-0.1.1/python_linters/parse_rules.py` & `python_linters-0.1.2/python_linters/parse_rules.py`

 * *Files identical despite different names*

### Comparing `python_linters-0.1.1/python_linters/ruff.toml` & `python_linters-0.1.2/python_linters/ruff.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 target-version = "py310"
+[lint.isort]
+profile = "black"
 # Exclude a variety of commonly ignored directories. see https://beta.ruff.rs/docs/configuration/#using-pyprojecttoml
 [lint]
 exclude = [
     ".bzr",
     ".direnv",
     ".eggs",
     ".git",
@@ -106,18 +108,20 @@
     "E741",# SIM118 	in-dict-keys -> fully disagree! "for k in d.keys()" is way better than "for k in d" -> implicit is bad!
     "N806", # this one disallows the "constant-variable-convention" within functions, leaving you without any convention!
     "N802",# N802: I want test-names like this: "test_ASRInferDecoder" that contain the actual class-name! with camelcase!
     "N803", # to allow names with abbreviations, like: max_SNR, cause it is more understandable than "max_snr"
     "RET505", # encurages bad practice of ommitting the "else"-clause
     "RUF100", # RUF100 unused-noqa: ruff does not know about flake8 codes
     "UP008", # see: https://stackoverflow.com/questions/73268995/typeerror-when-calling-super-in-dataclassslots-true-subclass
+    "RET506", # looks like a false-positive
+    "SLF001", # everybody knows about the _-conventin, if one still accesses "protected" attributes one has their reasons!
 ]
 
 [lint.mccabe]
-# Flag errors (`C901`) whenever the complexity level exceeds 5.
+# Flag errors (`C901`) whenever the complexity level exceeds some threshold.
 # ruffs default is 10
 # PyCQA default seems to be 7: https://github.com/PyCQA/mccabe/blob/60cf21c21f8e5880f9907561c53732e80d1be400/mccabe.py#L273
 # flake8's default is 10: https://flake8.pycqa.org/en/2.5.5/
 # radon: cc<=5 is A ; 5<cc<=10 is B ; see: https://radon.readthedocs.io/en/latest/commandline.html#the-cc-command
 max-complexity = 7 # seven is a "magical" number!
 
 [lint.pylint]
```

### Comparing `python_linters-0.1.1/python_linters/ruff_rule_categories.py` & `python_linters-0.1.2/python_linters/ruff_rule_categories.py`

 * *Files identical despite different names*

### Comparing `python_linters-0.1.1/python_linters/ruff_rules.txt` & `python_linters-0.1.2/python_linters/ruff_rules.txt`

 * *Files identical despite different names*

### Comparing `python_linters-0.1.1/python_linters/run_linters.py` & `python_linters-0.1.2/python_linters/run_linters.py`

 * *Files identical despite different names*

### Comparing `python_linters-0.1.1/PKG-INFO` & `python_linters-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-linters
-Version: 0.1.1
+Version: 0.1.2
 Summary: bundling config files for linters like ruff and flake8
 Home-page: https://github.com/dertilo/python-linters
 Author: Tilo Himmelsbach
 Author-email: dertilo@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -15,14 +15,17 @@
 Requires-Dist: flake8-newspaper-style (>=0.4.3,<0.5.0)
 Requires-Dist: ruff (>=0.0.291)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: wemake-python-styleguide (>=0.18.0,<0.19.0)
 Project-URL: Repository, https://github.com/dertilo/python-linters
 Description-Content-Type: text/markdown
 
+![pypi](https://github.com/dertilo/python-linters/actions/workflows/release.yml/badge.svg)
+[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
+[![bear-ified](https://raw.githubusercontent.com/beartype/beartype-assets/main/badge/bear-ified.svg)](https://beartype.readthedocs.io)
 # python-linters
 - bundles flake8, black, isort, ruff into a single poetry-script
 - project independent linter configuration (via `ruff.toml`,`.flake8`) -> one config to rule them all
 ### use-cases:
 1. interactively learning python code quality standards via ruff+flake8, see [local development workflow](#2-local-development-workflow-before-pushing-to-ci-pipeline)
 2. enforcing minimal quality-standards via a "lint-stage" in a ci-pipeline, see [setup for ci-pipeline](#3-setup-for-ci-pipeline)
```

