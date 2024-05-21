# Comparing `tmp/okipy-1.0.0.tar.gz` & `tmp/okipy-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "okipy-1.0.0.tar", last modified: Tue May 21 01:30:42 2024, max compression
+gzip compressed data, was "okipy-1.0.1.tar", last modified: Tue May 21 01:36:58 2024, max compression
```

## Comparing `okipy-1.0.0.tar` & `okipy-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 mb        (1000) users      (984)        0 2024-05-21 01:30:42.059766 okipy-1.0.0/
--rw-r--r--   0 mb        (1000) users      (984)     1069 2024-05-20 22:29:12.000000 okipy-1.0.0/LICENCE
--rw-r--r--   0 mb        (1000) users      (984)     1268 2024-05-21 01:30:42.059766 okipy-1.0.0/PKG-INFO
--rw-r--r--   0 mb        (1000) users      (984)      712 2024-05-20 23:22:04.000000 okipy-1.0.0/README.md
--rw-r--r--   0 mb        (1000) users      (984)      735 2024-05-21 00:12:48.000000 okipy-1.0.0/pyproject.toml
--rw-r--r--   0 mb        (1000) users      (984)       38 2024-05-21 01:30:42.059766 okipy-1.0.0/setup.cfg
-drwxr-xr-x   0 mb        (1000) users      (984)        0 2024-05-21 01:30:42.057766 okipy-1.0.0/src/
-drwxr-xr-x   0 mb        (1000) users      (984)        0 2024-05-21 01:30:42.058766 okipy-1.0.0/src/okipy/
--rw-r--r--   0 mb        (1000) users      (984)       95 2024-05-21 00:13:23.000000 okipy-1.0.0/src/okipy/__init__.py
--rw-r--r--   0 mb        (1000) users      (984)      265 2024-05-20 21:58:32.000000 okipy-1.0.0/src/okipy/colors.py
--rw-r--r--   0 mb        (1000) users      (984)     3952 2024-05-21 00:32:05.000000 okipy-1.0.0/src/okipy/lib.py
--rwxr-xr-x   0 mb        (1000) users      (984)     1192 2024-05-21 01:07:48.000000 okipy-1.0.0/src/okipy/main.py
--rw-r--r--   0 mb        (1000) users      (984)       63 2024-05-20 23:01:00.000000 okipy-1.0.0/src/okipy/py.typed
--rw-r--r--   0 mb        (1000) users      (984)      583 2024-05-20 21:40:57.000000 okipy-1.0.0/src/okipy/utils.py
-drwxr-xr-x   0 mb        (1000) users      (984)        0 2024-05-21 01:30:42.058766 okipy-1.0.0/src/okipy.egg-info/
--rw-r--r--   0 mb        (1000) users      (984)     1268 2024-05-21 01:30:42.000000 okipy-1.0.0/src/okipy.egg-info/PKG-INFO
--rw-r--r--   0 mb        (1000) users      (984)      315 2024-05-21 01:30:42.000000 okipy-1.0.0/src/okipy.egg-info/SOURCES.txt
--rw-r--r--   0 mb        (1000) users      (984)        1 2024-05-21 01:30:42.000000 okipy-1.0.0/src/okipy.egg-info/dependency_links.txt
--rw-r--r--   0 mb        (1000) users      (984)       35 2024-05-21 01:30:42.000000 okipy-1.0.0/src/okipy.egg-info/entry_points.txt
--rw-r--r--   0 mb        (1000) users      (984)        6 2024-05-21 01:30:42.000000 okipy-1.0.0/src/okipy.egg-info/top_level.txt
+drwxr-xr-x   0 mb        (1000) users      (984)        0 2024-05-21 01:36:58.526451 okipy-1.0.1/
+-rw-r--r--   0 mb        (1000) users      (984)     1069 2024-05-20 22:29:12.000000 okipy-1.0.1/LICENCE
+-rw-r--r--   0 mb        (1000) users      (984)     1559 2024-05-21 01:36:58.526451 okipy-1.0.1/PKG-INFO
+-rw-r--r--   0 mb        (1000) users      (984)     1003 2024-05-21 01:36:07.000000 okipy-1.0.1/README.md
+-rw-r--r--   0 mb        (1000) users      (984)      735 2024-05-21 01:36:36.000000 okipy-1.0.1/pyproject.toml
+-rw-r--r--   0 mb        (1000) users      (984)       38 2024-05-21 01:36:58.526451 okipy-1.0.1/setup.cfg
+drwxr-xr-x   0 mb        (1000) users      (984)        0 2024-05-21 01:36:58.524451 okipy-1.0.1/src/
+drwxr-xr-x   0 mb        (1000) users      (984)        0 2024-05-21 01:36:58.525451 okipy-1.0.1/src/okipy/
+-rw-r--r--   0 mb        (1000) users      (984)       95 2024-05-21 00:13:23.000000 okipy-1.0.1/src/okipy/__init__.py
+-rw-r--r--   0 mb        (1000) users      (984)      265 2024-05-20 21:58:32.000000 okipy-1.0.1/src/okipy/colors.py
+-rw-r--r--   0 mb        (1000) users      (984)     3952 2024-05-21 00:32:05.000000 okipy-1.0.1/src/okipy/lib.py
+-rwxr-xr-x   0 mb        (1000) users      (984)     1192 2024-05-21 01:07:48.000000 okipy-1.0.1/src/okipy/main.py
+-rw-r--r--   0 mb        (1000) users      (984)       63 2024-05-20 23:01:00.000000 okipy-1.0.1/src/okipy/py.typed
+-rw-r--r--   0 mb        (1000) users      (984)      583 2024-05-20 21:40:57.000000 okipy-1.0.1/src/okipy/utils.py
+drwxr-xr-x   0 mb        (1000) users      (984)        0 2024-05-21 01:36:58.526451 okipy-1.0.1/src/okipy.egg-info/
+-rw-r--r--   0 mb        (1000) users      (984)     1559 2024-05-21 01:36:58.000000 okipy-1.0.1/src/okipy.egg-info/PKG-INFO
+-rw-r--r--   0 mb        (1000) users      (984)      315 2024-05-21 01:36:58.000000 okipy-1.0.1/src/okipy.egg-info/SOURCES.txt
+-rw-r--r--   0 mb        (1000) users      (984)        1 2024-05-21 01:36:58.000000 okipy-1.0.1/src/okipy.egg-info/dependency_links.txt
+-rw-r--r--   0 mb        (1000) users      (984)       35 2024-05-21 01:36:58.000000 okipy-1.0.1/src/okipy.egg-info/entry_points.txt
+-rw-r--r--   0 mb        (1000) users      (984)        6 2024-05-21 01:36:58.000000 okipy-1.0.1/src/okipy.egg-info/top_level.txt
```

### Comparing `okipy-1.0.0/LICENCE` & `okipy-1.0.1/LICENCE`

 * *Files identical despite different names*

### Comparing `okipy-1.0.0/README.md` & `okipy-1.0.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -29,8 +29,24 @@
             raise Exception("Expected failure.")
 
     suite.run()
 ```
 
 Results in this output when run :
 
-![test output screenshot](./assets/output.png)
+![test suite output screenshot](https://git.barnulf.net/mb/okipy/media/branch/master/assets/output.png)
+
+It is also possible to write inline tests :
+
+```py
+
+def add(a, b):
+    return a + b
+
+
+@test()
+def it_works(ctx):
+    pass
+
+```
+
+![test inline output screenshot](https://git.barnulf.net/mb/okipy/media/branch/master/assets/inline.png)
```

### Comparing `okipy-1.0.0/pyproject.toml` & `okipy-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [project]
 name = "okipy"
-version = "1.0.0"
+version = "1.0.1"
 description = "Minimal, typed, functional and dynamic test library."
 keywords = ["test", "functional", "library", "testing", "dynamic", "minimal"]
 
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `okipy-1.0.0/src/okipy/lib.py` & `okipy-1.0.1/src/okipy/lib.py`

 * *Files identical despite different names*

### Comparing `okipy-1.0.0/src/okipy/main.py` & `okipy-1.0.1/src/okipy/main.py`

 * *Files identical despite different names*

### Comparing `okipy-1.0.0/src/okipy/utils.py` & `okipy-1.0.1/src/okipy/utils.py`

 * *Files identical despite different names*

