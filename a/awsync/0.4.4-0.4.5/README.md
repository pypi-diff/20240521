# Comparing `tmp/awsync-0.4.4.tar.gz` & `tmp/awsync-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "awsync-0.4.4.tar", max compression
+gzip compressed data, was "awsync-0.4.5.tar", max compression
```

## Comparing `awsync-0.4.4.tar` & `awsync-0.4.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    11357 2024-05-19 03:51:25.858388 awsync-0.4.4/LICENSE
--rw-r--r--   0        0        0     1841 2024-05-19 03:51:25.858388 awsync-0.4.4/README.md
--rw-r--r--   0        0        0        0 2024-05-19 03:51:25.858388 awsync-0.4.4/awsync/__init__.py
--rw-r--r--   0        0        0      592 2024-05-19 03:51:25.858388 awsync-0.4.4/awsync/__main__.py
--rw-r--r--   0        0        0     6960 2024-05-19 03:51:25.858388 awsync-0.4.4/awsync/client.py
--rw-r--r--   0        0        0        0 2024-05-19 03:51:25.858388 awsync-0.4.4/awsync/models/__init__.py
--rw-r--r--   0        0        0     3062 2024-05-19 03:51:25.858388 awsync-0.4.4/awsync/models/aws.py
--rw-r--r--   0        0        0     1433 2024-05-19 03:51:25.858388 awsync-0.4.4/awsync/models/http.py
--rw-r--r--   0        0        0      282 2024-05-19 03:51:25.858388 awsync-0.4.4/awsync/models/strenum.py
--rw-r--r--   0        0        0        0 2024-05-19 03:51:25.858388 awsync-0.4.4/awsync/py.typed
--rw-r--r--   0        0        0    10212 2024-05-19 03:51:25.858388 awsync-0.4.4/awsync/request.py
--rw-r--r--   0        0        0     1672 2024-05-19 03:51:25.862388 awsync-0.4.4/pyproject.toml
--rw-r--r--   0        0        0     2870 1970-01-01 00:00:00.000000 awsync-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-20 23:51:27.733074 awsync-0.4.5/LICENSE
+-rw-r--r--   0        0        0     2029 2024-05-20 23:51:27.733074 awsync-0.4.5/README.md
+-rw-r--r--   0        0        0        0 2024-05-20 23:51:27.733074 awsync-0.4.5/awsync/__init__.py
+-rw-r--r--   0        0        0      592 2024-05-20 23:51:27.733074 awsync-0.4.5/awsync/__main__.py
+-rw-r--r--   0        0        0     6960 2024-05-20 23:51:27.737074 awsync-0.4.5/awsync/client.py
+-rw-r--r--   0        0        0        0 2024-05-20 23:51:27.737074 awsync-0.4.5/awsync/models/__init__.py
+-rw-r--r--   0        0        0     3062 2024-05-20 23:51:27.737074 awsync-0.4.5/awsync/models/aws.py
+-rw-r--r--   0        0        0     1433 2024-05-20 23:51:27.737074 awsync-0.4.5/awsync/models/http.py
+-rw-r--r--   0        0        0      282 2024-05-20 23:51:27.737074 awsync-0.4.5/awsync/models/strenum.py
+-rw-r--r--   0        0        0        0 2024-05-20 23:51:27.737074 awsync-0.4.5/awsync/py.typed
+-rw-r--r--   0        0        0    10212 2024-05-20 23:51:27.737074 awsync-0.4.5/awsync/request.py
+-rw-r--r--   0        0        0     1672 2024-05-20 23:51:27.737074 awsync-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0     3058 1970-01-01 00:00:00.000000 awsync-0.4.5/PKG-INFO
```

### Comparing `awsync-0.4.4/LICENSE` & `awsync-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `awsync-0.4.4/README.md` & `awsync-0.4.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # awsync
 
 ![CICD](https://github.com/JKCT/awsync/actions/workflows/cicd.yaml/badge.svg)
 
 An asynchronous, fully-typed AWS API library with a focus on being understandable, reliable, and maintainable.
 
-Read [the documentation](https://jkct.github.io/awsync/).
+## Getting Started
+
+📖 Read [the documentation](https://jkct.github.io/awsync/)!
 
 **NOTE: Currently a work in progress!**
 Only a few API methods currently implemented for testing and development.
 
 ## Usage
 
 ```python
@@ -42,23 +44,27 @@
 
 Requirements:
 
 - [mise](https://mise.jdx.dev/)
 - [python](https://www.python.org/) 3.8 or greater
 - [poetry](https://python-poetry.org/)
 
+[Install mise](https://mise.jdx.dev/getting-started.html) then run `mise run init` to setup python, poetry, and install dependencies.
+
 ### Repository Mangement
 
 This repository uses [mise](https://mise.jdx.dev/) for tool and task management.
 
 List all available commands with `mise tasks`.
 
+Run all pull request checks locally with `mise run pr`
+
 ### Package Management
 
 This repository uses [poetry](https://python-poetry.org/) for python package management.
 
-- `poetry install --sync` install/update dependencies, aliased to `mise run init`.
+- `poetry install --sync` install/update dependencies.
 - `poetry add` add a dependency ie. `poetry add black`.
 - `poetry add -D` add a development dependency ie. `poetry add -D black`.
 - `poetry remove` remove a dependency ie. `poetry remove black`.
 - `poetry shell` activate the python virtual environment for access to installed packages.
 - `exit` exit the python virtual environment.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `awsync-0.4.4/awsync/__main__.py` & `awsync-0.4.5/awsync/__main__.py`

 * *Files identical despite different names*

### Comparing `awsync-0.4.4/awsync/client.py` & `awsync-0.4.5/awsync/client.py`

 * *Files identical despite different names*

### Comparing `awsync-0.4.4/awsync/models/aws.py` & `awsync-0.4.5/awsync/models/aws.py`

 * *Files identical despite different names*

### Comparing `awsync-0.4.4/awsync/models/http.py` & `awsync-0.4.5/awsync/models/http.py`

 * *Files identical despite different names*

### Comparing `awsync-0.4.4/awsync/request.py` & `awsync-0.4.5/awsync/request.py`

 * *Files identical despite different names*

### Comparing `awsync-0.4.4/pyproject.toml` & `awsync-0.4.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "awsync"
-version = "0.4.4"
+version = "0.4.5"
 description = "An asynchronous, fully-typed AWS API library with a focus on being understandable, reliable, and maintainable."
 license = "Apache-2.0"
 authors = ["JKCT <jkct@visceralfx.com>"]
 readme = "README.md"
 packages = [{include = "awsync"}]
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `awsync-0.4.4/PKG-INFO` & `awsync-0.4.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awsync
-Version: 0.4.4
+Version: 0.4.5
 Summary: An asynchronous, fully-typed AWS API library with a focus on being understandable, reliable, and maintainable.
 Home-page: https://github.com/JKCT/awsync
 License: Apache-2.0
 Keywords: aws,async,boto,request,sdk,typed
 Author: JKCT
 Author-email: jkct@visceralfx.com
 Requires-Python: >=3.8,<4.0
@@ -25,15 +25,17 @@
 
 # awsync
 
 ![CICD](https://github.com/JKCT/awsync/actions/workflows/cicd.yaml/badge.svg)
 
 An asynchronous, fully-typed AWS API library with a focus on being understandable, reliable, and maintainable.
 
-Read [the documentation](https://jkct.github.io/awsync/).
+## Getting Started
+
+📖 Read [the documentation](https://jkct.github.io/awsync/)!
 
 **NOTE: Currently a work in progress!**
 Only a few API methods currently implemented for testing and development.
 
 ## Usage
 
 ```python
@@ -67,24 +69,28 @@
 
 Requirements:
 
 - [mise](https://mise.jdx.dev/)
 - [python](https://www.python.org/) 3.8 or greater
 - [poetry](https://python-poetry.org/)
 
+[Install mise](https://mise.jdx.dev/getting-started.html) then run `mise run init` to setup python, poetry, and install dependencies.
+
 ### Repository Mangement
 
 This repository uses [mise](https://mise.jdx.dev/) for tool and task management.
 
 List all available commands with `mise tasks`.
 
+Run all pull request checks locally with `mise run pr`
+
 ### Package Management
 
 This repository uses [poetry](https://python-poetry.org/) for python package management.
 
-- `poetry install --sync` install/update dependencies, aliased to `mise run init`.
+- `poetry install --sync` install/update dependencies.
 - `poetry add` add a dependency ie. `poetry add black`.
 - `poetry add -D` add a development dependency ie. `poetry add -D black`.
 - `poetry remove` remove a dependency ie. `poetry remove black`.
 - `poetry shell` activate the python virtual environment for access to installed packages.
 - `exit` exit the python virtual environment.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

