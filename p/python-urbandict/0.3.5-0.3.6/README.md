# Comparing `tmp/python_urbandict-0.3.5.tar.gz` & `tmp/python_urbandict-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_urbandict-0.3.5.tar", max compression
+gzip compressed data, was "python_urbandict-0.3.6.tar", max compression
```

## Comparing `python_urbandict-0.3.5.tar` & `python_urbandict-0.3.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1066 2024-04-17 19:02:38.144085 python_urbandict-0.3.5/LICENSE
--rw-r--r--   0        0        0     2325 2024-04-17 19:02:38.144085 python_urbandict-0.3.5/README.md
--rw-r--r--   0        0        0      954 2024-04-17 19:02:38.144085 python_urbandict-0.3.5/pyproject.toml
--rw-r--r--   0        0        0       77 2024-04-17 19:02:38.144085 python_urbandict-0.3.5/pyurbandict/__init__.py
--rw-r--r--   0        0        0     1211 2024-04-17 19:02:38.144085 python_urbandict-0.3.5/pyurbandict/parse.py
--rw-r--r--   0        0        0     3272 1970-01-01 00:00:00.000000 python_urbandict-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-21 11:49:04.902449 python_urbandict-0.3.6/LICENSE
+-rw-r--r--   0        0        0     2325 2024-05-21 11:49:04.902449 python_urbandict-0.3.6/README.md
+-rw-r--r--   0        0        0      944 2024-05-21 11:49:04.902449 python_urbandict-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0       79 2024-05-21 11:49:04.902449 python_urbandict-0.3.6/pyurbandict/__init__.py
+-rw-r--r--   0        0        0     1211 2024-05-21 11:49:04.906449 python_urbandict-0.3.6/pyurbandict/parse.py
+-rw-r--r--   0        0        0     3262 1970-01-01 00:00:00.000000 python_urbandict-0.3.6/PKG-INFO
```

### Comparing `python_urbandict-0.3.5/LICENSE` & `python_urbandict-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `python_urbandict-0.3.5/README.md` & `python_urbandict-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `python_urbandict-0.3.5/pyproject.toml` & `python_urbandict-0.3.6/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [tool.flake8]
 max-line-length = 88
 
 [tool.poetry]
 name = "python-urbandict"
-version = "0.3.5"
+version = "0.3.6"
 description = "Python wrapper for the Urban Dictionary API."
-authors = ["atbuy <contact.atbuy@gmail.com>"]
+authors = ["atbuy <buy@atbuy.dev>"]
 license = "MIT"
 homepage = "https://github.com/atbuy/pyurbandict"
 repository = "https://github.com/atbuy/pyurbandict"
 keywords = ["urban", "dictionary", "api", "wrapper", "python"]
 include = ["README.md"]
 readme = "README.md"
 packages = [
     {include = "pyurbandict"}
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-requests = "^2.31.0"
+requests = "^2.32.0"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/atbuy/pyurbandict/issues"
 "Source Code" = "https://github.com/atbuy/pyurbandict"
 "CI/CD" = "https://github.com/atbuy/pyurbandict/actions"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `python_urbandict-0.3.5/pyurbandict/parse.py` & `python_urbandict-0.3.6/pyurbandict/parse.py`

 * *Files identical despite different names*

### Comparing `python_urbandict-0.3.5/PKG-INFO` & `python_urbandict-0.3.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: python-urbandict
-Version: 0.3.5
+Version: 0.3.6
 Summary: Python wrapper for the Urban Dictionary API.
 Home-page: https://github.com/atbuy/pyurbandict
 License: MIT
 Keywords: urban,dictionary,api,wrapper,python
 Author: atbuy
-Author-email: contact.atbuy@gmail.com
+Author-email: buy@atbuy.dev
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: requests (>=2.32.0,<3.0.0)
 Project-URL: Bug Tracker, https://github.com/atbuy/pyurbandict/issues
 Project-URL: CI/CD, https://github.com/atbuy/pyurbandict/actions
 Project-URL: Repository, https://github.com/atbuy/pyurbandict
 Project-URL: Source Code, https://github.com/atbuy/pyurbandict
 Description-Content-Type: text/markdown
 
 # python-urbandict
```

