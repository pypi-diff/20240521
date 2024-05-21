# Comparing `tmp/python_urbandict-0.3.6.tar.gz` & `tmp/python_urbandict-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_urbandict-0.3.6.tar", max compression
+gzip compressed data, was "python_urbandict-0.3.7.tar", max compression
```

## Comparing `python_urbandict-0.3.6.tar` & `python_urbandict-0.3.7.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1066 2024-05-21 11:49:04.902449 python_urbandict-0.3.6/LICENSE
--rw-r--r--   0        0        0     2325 2024-05-21 11:49:04.902449 python_urbandict-0.3.6/README.md
--rw-r--r--   0        0        0      944 2024-05-21 11:49:04.902449 python_urbandict-0.3.6/pyproject.toml
--rw-r--r--   0        0        0       79 2024-05-21 11:49:04.902449 python_urbandict-0.3.6/pyurbandict/__init__.py
--rw-r--r--   0        0        0     1211 2024-05-21 11:49:04.906449 python_urbandict-0.3.6/pyurbandict/parse.py
--rw-r--r--   0        0        0     3262 1970-01-01 00:00:00.000000 python_urbandict-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-21 16:57:34.553958 python_urbandict-0.3.7/LICENSE
+-rw-r--r--   0        0        0     2307 2024-05-21 16:57:34.553958 python_urbandict-0.3.7/README.md
+-rw-r--r--   0        0        0      944 2024-05-21 16:57:34.553958 python_urbandict-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0       79 2024-05-21 16:57:34.553958 python_urbandict-0.3.7/pyurbandict/__init__.py
+-rw-r--r--   0        0        0     1211 2024-05-21 16:57:34.553958 python_urbandict-0.3.7/pyurbandict/parse.py
+-rw-r--r--   0        0        0     3244 1970-01-01 00:00:00.000000 python_urbandict-0.3.7/PKG-INFO
```

### Comparing `python_urbandict-0.3.6/LICENSE` & `python_urbandict-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `python_urbandict-0.3.6/README.md` & `python_urbandict-0.3.7/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # python-urbandict
 
 [![version](https://img.shields.io/pypi/v/python-urbandict.svg)](https://pypi.org/project/python-urbandict/)
 [![versions](https://img.shields.io/pypi/pyversions/python-urbandict.svg)](https://pypi.org/project/python-urbandict/)
-[![Python package](https://github.com/Vitaman02/pyurbandict/actions/workflows/python-package.yml/badge.svg)](https://github.com/Vitaman02/pyurbandict/actions/workflows/python-package.yml)
-[![codecov](https://codecov.io/gh/Vitaman02/pyurbandict/branch/main/graph/badge.svg?token=A244XBTUVH)](https://codecov.io/gh/Vitaman02/pyurbandict)
+[![Python package](https://github.com/atbuy/pyurbandict/actions/workflows/python-package.yml/badge.svg)(https://github.com/atbuy/pyurbandict/actions/workflows/python-package.yml)
+[![codecov](https://codecov.io/gh/atbuy/pyurbandict/branch/main/graph/badge.svg?token=A244XBTUVH)(https://codecov.io/gh/atbuy/pyurbandict)
 
 This is a python project, that fetches definitions of words from urban dictionary's public API.
 
 Future additions. PRs are always welcome :)
 * Calculate ratio of `thumbs_up` and `thumbs_down` and decide the probability of a correct definition.
 
 # Installation
```

### Comparing `python_urbandict-0.3.6/pyproject.toml` & `python_urbandict-0.3.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.flake8]
 max-line-length = 88
 
 [tool.poetry]
 name = "python-urbandict"
-version = "0.3.6"
+version = "0.3.7"
 description = "Python wrapper for the Urban Dictionary API."
 authors = ["atbuy <buy@atbuy.dev>"]
 license = "MIT"
 homepage = "https://github.com/atbuy/pyurbandict"
 repository = "https://github.com/atbuy/pyurbandict"
 keywords = ["urban", "dictionary", "api", "wrapper", "python"]
 include = ["README.md"]
```

### Comparing `python_urbandict-0.3.6/pyurbandict/parse.py` & `python_urbandict-0.3.7/pyurbandict/parse.py`

 * *Files identical despite different names*

### Comparing `python_urbandict-0.3.6/PKG-INFO` & `python_urbandict-0.3.7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-urbandict
-Version: 0.3.6
+Version: 0.3.7
 Summary: Python wrapper for the Urban Dictionary API.
 Home-page: https://github.com/atbuy/pyurbandict
 License: MIT
 Keywords: urban,dictionary,api,wrapper,python
 Author: atbuy
 Author-email: buy@atbuy.dev
 Requires-Python: >=3.9,<4.0
@@ -21,16 +21,16 @@
 Project-URL: Source Code, https://github.com/atbuy/pyurbandict
 Description-Content-Type: text/markdown
 
 # python-urbandict
 
 [![version](https://img.shields.io/pypi/v/python-urbandict.svg)](https://pypi.org/project/python-urbandict/)
 [![versions](https://img.shields.io/pypi/pyversions/python-urbandict.svg)](https://pypi.org/project/python-urbandict/)
-[![Python package](https://github.com/Vitaman02/pyurbandict/actions/workflows/python-package.yml/badge.svg)](https://github.com/Vitaman02/pyurbandict/actions/workflows/python-package.yml)
-[![codecov](https://codecov.io/gh/Vitaman02/pyurbandict/branch/main/graph/badge.svg?token=A244XBTUVH)](https://codecov.io/gh/Vitaman02/pyurbandict)
+[![Python package](https://github.com/atbuy/pyurbandict/actions/workflows/python-package.yml/badge.svg)(https://github.com/atbuy/pyurbandict/actions/workflows/python-package.yml)
+[![codecov](https://codecov.io/gh/atbuy/pyurbandict/branch/main/graph/badge.svg?token=A244XBTUVH)(https://codecov.io/gh/atbuy/pyurbandict)
 
 This is a python project, that fetches definitions of words from urban dictionary's public API.
 
 Future additions. PRs are always welcome :)
 * Calculate ratio of `thumbs_up` and `thumbs_down` and decide the probability of a correct definition.
 
 # Installation
```

