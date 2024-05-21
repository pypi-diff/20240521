# Comparing `tmp/pillory-1.1.3.tar.gz` & `tmp/pillory-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pillory-1.1.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pillory-1.1.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pillory-1.1.3.tar` & `pillory-1.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      797 2024-05-16 22:32:59.828446 pillory-1.1.3/.circleci/config.yml
--rw-r--r--   0        0        0       50 2024-05-16 22:32:59.828446 pillory-1.1.3/.gitignore
--rw-r--r--   0        0        0      359 2024-05-16 22:32:59.828446 pillory-1.1.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0     9161 2024-05-16 22:32:59.828446 pillory-1.1.3/LICENSE
--rw-r--r--   0        0        0      354 2024-05-16 22:32:59.828446 pillory-1.1.3/Makefile
--rw-r--r--   0        0        0     4793 2024-05-16 22:32:59.828446 pillory-1.1.3/README.md
--rw-r--r--   0        0        0     1372 2024-05-16 22:32:59.828446 pillory-1.1.3/dev-requirements.txt
--rw-r--r--   0        0        0       41 2024-05-16 22:32:59.828446 pillory-1.1.3/example/__init__.py
--rw-r--r--   0        0        0      311 2024-05-16 22:32:59.828446 pillory-1.1.3/example/definition.py
--rw-r--r--   0        0        0      180 2024-05-16 22:32:59.828446 pillory-1.1.3/example/empty/README.txt
--rw-r--r--   0        0        0      649 2024-05-16 22:32:59.828446 pillory-1.1.3/example/test_use.py
--rw-r--r--   0        0        0      222 2024-05-16 22:32:59.828446 pillory-1.1.3/example/use.py
--rwxr-xr-x   0        0        0    10614 2024-05-16 22:32:59.828446 pillory-1.1.3/pillory.py
--rw-r--r--   0        0        0     1093 2024-05-16 22:32:59.828446 pillory-1.1.3/pyproject.toml
--rw-r--r--   0        0        0     1245 2024-05-16 22:32:59.828446 pillory-1.1.3/test_example.py
--rw-r--r--   0        0        0     2768 2024-05-16 22:32:59.828446 pillory-1.1.3/test_pillory.py
--rw-r--r--   0        0        0     5376 1970-01-01 00:00:00.000000 pillory-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0      797 2024-05-21 10:47:45.530701 pillory-1.1.4/.circleci/config.yml
+-rw-r--r--   0        0        0       50 2024-05-21 10:47:45.530701 pillory-1.1.4/.gitignore
+-rw-r--r--   0        0        0      359 2024-05-21 10:47:45.530701 pillory-1.1.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     9161 2024-05-21 10:47:45.530701 pillory-1.1.4/LICENSE
+-rw-r--r--   0        0        0      354 2024-05-21 10:47:45.534701 pillory-1.1.4/Makefile
+-rw-r--r--   0        0        0     5320 2024-05-21 10:47:45.534701 pillory-1.1.4/README.md
+-rw-r--r--   0        0        0     1372 2024-05-21 10:47:45.534701 pillory-1.1.4/dev-requirements.txt
+-rw-r--r--   0        0        0       41 2024-05-21 10:47:45.534701 pillory-1.1.4/example/__init__.py
+-rw-r--r--   0        0        0      311 2024-05-21 10:47:45.534701 pillory-1.1.4/example/definition.py
+-rw-r--r--   0        0        0      180 2024-05-21 10:47:45.534701 pillory-1.1.4/example/empty/README.txt
+-rw-r--r--   0        0        0      649 2024-05-21 10:47:45.534701 pillory-1.1.4/example/test_use.py
+-rw-r--r--   0        0        0      222 2024-05-21 10:47:45.534701 pillory-1.1.4/example/use.py
+-rwxr-xr-x   0        0        0    10614 2024-05-21 10:47:45.534701 pillory-1.1.4/pillory.py
+-rw-r--r--   0        0        0     1093 2024-05-21 10:47:45.534701 pillory-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1245 2024-05-21 10:47:45.534701 pillory-1.1.4/test_example.py
+-rw-r--r--   0        0        0     2768 2024-05-21 10:47:45.534701 pillory-1.1.4/test_pillory.py
+-rw-r--r--   0        0        0     5903 1970-01-01 00:00:00.000000 pillory-1.1.4/PKG-INFO
```

### Comparing `pillory-1.1.3/.circleci/config.yml` & `pillory-1.1.4/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `pillory-1.1.3/LICENSE` & `pillory-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pillory-1.1.3/README.md` & `pillory-1.1.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,22 @@
 
 Install from PyPI with pip:
 
 ```
 pip install pillory
 ```
 
+Pillory needs to be able to find your code and its dependencies _as if_ it were
+importing it (but it doesn’t actually import it). This means you need to install
+any other dependencies and set up your environment as if you were going to run
+your tests. How you do this can vary between projects, but could include making
+a virtualenv, `pip install -r requirements.txt`, and `pip install -e .`. If you
+don’t do this pillory will find fewer errors than it should, or maybe find
+no errors at all, a misleading positive result.
+
 Run pillory on the current directory:
 
 ```
 python -m pillory
 ```
 
 Or give a specific file, directory, or glob:
@@ -27,20 +35,20 @@
 ```
 
 ### Rules
 
 **PM101 patched implementation**
 : You patched the implementation of a class or function instead of where it is
 imported to in the module under test. e.g. "parsers.Parser" where Parser is
-defined instead of "__main__.Parser" where it is used. This means you may not
+defined instead of "app.Parser" where it is used. This means you may not
 have affected the module under test at all, or you have replaced the target in a
 way which will affect other code that uses it, which is bad for test isolation
-(making sure tests don't affect other tests, and that each test tests what is
-intended and don't change how other parts of the code work). There is a warning
-about not affecting the right module in the [Python Standard Library
+(making sure tests don't affect other tests, each test tests only what it
+intends to, and doesn’t rely on how other parts of the code work). There is a
+warning about not affecting the right module in the [Python Standard Library
 docs][stdlibdocs], but there is an [even better article by Ned
 Batchelder][nedbat] explaining how it works and the additional problems with
 test isolation.
 
 **PM102 patched is not a top level module attribute**
 : You patched something like a method on a class. Because class methods can't be
 imported by themselves, this means all uses of the class will be affected, not
```

### Comparing `pillory-1.1.3/dev-requirements.txt` & `pillory-1.1.4/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `pillory-1.1.3/example/test_use.py` & `pillory-1.1.4/example/test_use.py`

 * *Files identical despite different names*

### Comparing `pillory-1.1.3/pillory.py` & `pillory-1.1.4/pillory.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """A linter to scrutinize how you are using mocks in Python."""
 
-__version__ = "1.1.3"
+__version__ = "1.1.4"
 
 # pyright: strict
 
 import ast
 import functools
 import logging
 import pathlib
```

### Comparing `pillory-1.1.3/pyproject.toml` & `pillory-1.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pillory-1.1.3/test_example.py` & `pillory-1.1.4/test_example.py`

 * *Files identical despite different names*

### Comparing `pillory-1.1.3/test_pillory.py` & `pillory-1.1.4/test_pillory.py`

 * *Files identical despite different names*

### Comparing `pillory-1.1.3/PKG-INFO` & `pillory-1.1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pillory
-Version: 1.1.3
+Version: 1.1.4
 Summary: A linter to scrutinize how you are using mocks in Python.
 Author-email: Fergal Armstrong <patio.algebra0i@icloud.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: coverage~=7.5 ; extra == "dev"
 Requires-Dist: flit~=3.9 ; extra == "dev"
 Requires-Dist: pip-tools~=7.4 ; extra == "dev"
@@ -25,14 +25,22 @@
 
 Install from PyPI with pip:
 
 ```
 pip install pillory
 ```
 
+Pillory needs to be able to find your code and its dependencies _as if_ it were
+importing it (but it doesn’t actually import it). This means you need to install
+any other dependencies and set up your environment as if you were going to run
+your tests. How you do this can vary between projects, but could include making
+a virtualenv, `pip install -r requirements.txt`, and `pip install -e .`. If you
+don’t do this pillory will find fewer errors than it should, or maybe find
+no errors at all, a misleading positive result.
+
 Run pillory on the current directory:
 
 ```
 python -m pillory
 ```
 
 Or give a specific file, directory, or glob:
@@ -42,20 +50,20 @@
 ```
 
 ### Rules
 
 **PM101 patched implementation**
 : You patched the implementation of a class or function instead of where it is
 imported to in the module under test. e.g. "parsers.Parser" where Parser is
-defined instead of "__main__.Parser" where it is used. This means you may not
+defined instead of "app.Parser" where it is used. This means you may not
 have affected the module under test at all, or you have replaced the target in a
 way which will affect other code that uses it, which is bad for test isolation
-(making sure tests don't affect other tests, and that each test tests what is
-intended and don't change how other parts of the code work). There is a warning
-about not affecting the right module in the [Python Standard Library
+(making sure tests don't affect other tests, each test tests only what it
+intends to, and doesn’t rely on how other parts of the code work). There is a
+warning about not affecting the right module in the [Python Standard Library
 docs][stdlibdocs], but there is an [even better article by Ned
 Batchelder][nedbat] explaining how it works and the additional problems with
 test isolation.
 
 **PM102 patched is not a top level module attribute**
 : You patched something like a method on a class. Because class methods can't be
 imported by themselves, this means all uses of the class will be affected, not
```

