# Comparing `tmp/constructor-io-1.8.0.tar.gz` & `tmp/constructor-io-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "constructor-io-1.8.0.tar", last modified: Fri Apr 12 15:22:08 2024, max compression
+gzip compressed data, was "constructor-io-1.8.1.tar", last modified: Tue May 21 20:52:27 2024, max compression
```

## Comparing `constructor-io-1.8.0.tar` & `constructor-io-1.8.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 enes       (502) staff       (20)        0 2024-04-12 15:22:08.429680 constructor-io-1.8.0/
--rw-r--r--   0 enes       (502) staff       (20)     1086 2021-09-21 17:57:12.000000 constructor-io-1.8.0/LICENSE
--rw-r--r--   0 enes       (502) staff       (20)     2562 2024-04-12 15:22:08.429479 constructor-io-1.8.0/PKG-INFO
--rw-r--r--   0 enes       (502) staff       (20)     2198 2022-10-03 13:13:47.000000 constructor-io-1.8.0/README.md
-drwxr-xr-x   0 enes       (502) staff       (20)        0 2024-04-12 15:22:08.424511 constructor-io-1.8.0/constructor_io/
--rw-r--r--   0 enes       (502) staff       (20)       41 2024-04-12 15:21:54.000000 constructor-io-1.8.0/constructor_io/__init__.py
--rw-r--r--   0 enes       (502) staff       (20)     2324 2023-06-08 14:52:00.000000 constructor-io-1.8.0/constructor_io/constructor_io.py
-drwxr-xr-x   0 enes       (502) staff       (20)        0 2024-04-12 15:22:08.426334 constructor-io-1.8.0/constructor_io/helpers/
--rw-r--r--   0 enes       (502) staff       (20)        0 2021-11-18 19:33:38.000000 constructor-io-1.8.0/constructor_io/helpers/__init__.py
--rw-r--r--   0 enes       (502) staff       (20)      481 2021-11-18 19:33:38.000000 constructor-io-1.8.0/constructor_io/helpers/exception.py
--rw-r--r--   0 enes       (502) staff       (20)     4795 2023-05-10 19:05:41.000000 constructor-io-1.8.0/constructor_io/helpers/utils.py
-drwxr-xr-x   0 enes       (502) staff       (20)        0 2024-04-12 15:22:08.429097 constructor-io-1.8.0/constructor_io/modules/
--rw-r--r--   0 enes       (502) staff       (20)        0 2021-11-18 19:33:38.000000 constructor-io-1.8.0/constructor_io/modules/__init__.py
--rw-r--r--   0 enes       (502) staff       (20)     4767 2024-04-12 15:21:14.000000 constructor-io-1.8.0/constructor_io/modules/autocomplete.py
--rw-r--r--   0 enes       (502) staff       (20)    14881 2022-10-03 13:13:47.000000 constructor-io-1.8.0/constructor_io/modules/browse.py
--rw-r--r--   0 enes       (502) staff       (20)    17262 2022-10-21 17:16:45.000000 constructor-io-1.8.0/constructor_io/modules/catalog.py
--rw-r--r--   0 enes       (502) staff       (20)     6762 2023-04-13 18:25:13.000000 constructor-io-1.8.0/constructor_io/modules/quizzes.py
--rw-r--r--   0 enes       (502) staff       (20)     4167 2022-10-03 13:13:47.000000 constructor-io-1.8.0/constructor_io/modules/recommendations.py
--rw-r--r--   0 enes       (502) staff       (20)     4164 2023-05-10 18:53:45.000000 constructor-io-1.8.0/constructor_io/modules/search.py
--rw-r--r--   0 enes       (502) staff       (20)     3880 2023-06-21 16:51:54.000000 constructor-io-1.8.0/constructor_io/modules/tasks.py
-drwxr-xr-x   0 enes       (502) staff       (20)        0 2024-04-12 15:22:08.425672 constructor-io-1.8.0/constructor_io.egg-info/
--rw-r--r--   0 enes       (502) staff       (20)     2562 2024-04-12 15:22:08.000000 constructor-io-1.8.0/constructor_io.egg-info/PKG-INFO
--rw-r--r--   0 enes       (502) staff       (20)      660 2024-04-12 15:22:08.000000 constructor-io-1.8.0/constructor_io.egg-info/SOURCES.txt
--rw-r--r--   0 enes       (502) staff       (20)        1 2024-04-12 15:22:08.000000 constructor-io-1.8.0/constructor_io.egg-info/dependency_links.txt
--rw-r--r--   0 enes       (502) staff       (20)       15 2024-04-12 15:22:08.000000 constructor-io-1.8.0/constructor_io.egg-info/requires.txt
--rw-r--r--   0 enes       (502) staff       (20)       15 2024-04-12 15:22:08.000000 constructor-io-1.8.0/constructor_io.egg-info/top_level.txt
--rw-r--r--   0 enes       (502) staff       (20)       38 2024-04-12 15:22:08.429762 constructor-io-1.8.0/setup.cfg
--rw-r--r--   0 enes       (502) staff       (20)      745 2022-01-10 22:25:09.000000 constructor-io-1.8.0/setup.py
+drwxr-xr-x   0 enes       (502) staff       (20)        0 2024-05-21 20:52:27.130428 constructor-io-1.8.1/
+-rw-r--r--   0 enes       (502) staff       (20)     1086 2021-09-21 17:57:12.000000 constructor-io-1.8.1/LICENSE
+-rw-r--r--   0 enes       (502) staff       (20)     2562 2024-05-21 20:52:27.130245 constructor-io-1.8.1/PKG-INFO
+-rw-r--r--   0 enes       (502) staff       (20)     2198 2022-10-03 13:13:47.000000 constructor-io-1.8.1/README.md
+drwxr-xr-x   0 enes       (502) staff       (20)        0 2024-05-21 20:52:27.124750 constructor-io-1.8.1/constructor_io/
+-rw-r--r--   0 enes       (502) staff       (20)       41 2024-05-21 20:52:17.000000 constructor-io-1.8.1/constructor_io/__init__.py
+-rw-r--r--   0 enes       (502) staff       (20)     2324 2023-06-08 14:52:00.000000 constructor-io-1.8.1/constructor_io/constructor_io.py
+drwxr-xr-x   0 enes       (502) staff       (20)        0 2024-05-21 20:52:27.126436 constructor-io-1.8.1/constructor_io/helpers/
+-rw-r--r--   0 enes       (502) staff       (20)        0 2021-11-18 19:33:38.000000 constructor-io-1.8.1/constructor_io/helpers/__init__.py
+-rw-r--r--   0 enes       (502) staff       (20)      481 2021-11-18 19:33:38.000000 constructor-io-1.8.1/constructor_io/helpers/exception.py
+-rw-r--r--   0 enes       (502) staff       (20)     4795 2023-05-10 19:05:41.000000 constructor-io-1.8.1/constructor_io/helpers/utils.py
+drwxr-xr-x   0 enes       (502) staff       (20)        0 2024-05-21 20:52:27.129838 constructor-io-1.8.1/constructor_io/modules/
+-rw-r--r--   0 enes       (502) staff       (20)        0 2021-11-18 19:33:38.000000 constructor-io-1.8.1/constructor_io/modules/__init__.py
+-rw-r--r--   0 enes       (502) staff       (20)     4767 2024-04-12 15:21:14.000000 constructor-io-1.8.1/constructor_io/modules/autocomplete.py
+-rw-r--r--   0 enes       (502) staff       (20)    14881 2022-10-03 13:13:47.000000 constructor-io-1.8.1/constructor_io/modules/browse.py
+-rw-r--r--   0 enes       (502) staff       (20)    17262 2022-10-21 17:16:45.000000 constructor-io-1.8.1/constructor_io/modules/catalog.py
+-rw-r--r--   0 enes       (502) staff       (20)     6762 2023-04-13 18:25:13.000000 constructor-io-1.8.1/constructor_io/modules/quizzes.py
+-rw-r--r--   0 enes       (502) staff       (20)     4167 2022-10-03 13:13:47.000000 constructor-io-1.8.1/constructor_io/modules/recommendations.py
+-rw-r--r--   0 enes       (502) staff       (20)     4164 2023-05-10 18:53:45.000000 constructor-io-1.8.1/constructor_io/modules/search.py
+-rw-r--r--   0 enes       (502) staff       (20)     3880 2023-06-21 16:51:54.000000 constructor-io-1.8.1/constructor_io/modules/tasks.py
+drwxr-xr-x   0 enes       (502) staff       (20)        0 2024-05-21 20:52:27.125801 constructor-io-1.8.1/constructor_io.egg-info/
+-rw-r--r--   0 enes       (502) staff       (20)     2562 2024-05-21 20:52:27.000000 constructor-io-1.8.1/constructor_io.egg-info/PKG-INFO
+-rw-r--r--   0 enes       (502) staff       (20)      660 2024-05-21 20:52:27.000000 constructor-io-1.8.1/constructor_io.egg-info/SOURCES.txt
+-rw-r--r--   0 enes       (502) staff       (20)        1 2024-05-21 20:52:27.000000 constructor-io-1.8.1/constructor_io.egg-info/dependency_links.txt
+-rw-r--r--   0 enes       (502) staff       (20)       15 2024-05-21 20:52:27.000000 constructor-io-1.8.1/constructor_io.egg-info/requires.txt
+-rw-r--r--   0 enes       (502) staff       (20)       15 2024-05-21 20:52:27.000000 constructor-io-1.8.1/constructor_io.egg-info/top_level.txt
+-rw-r--r--   0 enes       (502) staff       (20)       38 2024-05-21 20:52:27.130483 constructor-io-1.8.1/setup.cfg
+-rw-r--r--   0 enes       (502) staff       (20)      745 2022-01-10 22:25:09.000000 constructor-io-1.8.1/setup.py
```

### Comparing `constructor-io-1.8.0/LICENSE` & `constructor-io-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `constructor-io-1.8.0/PKG-INFO` & `constructor-io-1.8.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: constructor-io
-Version: 1.8.0
+Version: 1.8.1
 Summary: Constructor.IO Python Client
 Home-page: https://www.constructor.io
 Author: Constructor.io
 Author-email: info@constructor.io
 License: MIT
-Download-URL: https://github.com/Constructor-io/constructor-io/tarball/1.8.0
+Download-URL: https://github.com/Constructor-io/constructor-io/tarball/1.8.1
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Constructor.io Python Client
 
 [![Version](https://img.shields.io/pypi/v/constructor-io.svg)](https://pypi.python.org/pypi/constructor-io)
```

### Comparing `constructor-io-1.8.0/README.md` & `constructor-io-1.8.1/README.md`

 * *Files identical despite different names*

### Comparing `constructor-io-1.8.0/constructor_io/constructor_io.py` & `constructor-io-1.8.1/constructor_io/constructor_io.py`

 * *Files identical despite different names*

### Comparing `constructor-io-1.8.0/constructor_io/helpers/utils.py` & `constructor-io-1.8.1/constructor_io/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `constructor-io-1.8.0/constructor_io/modules/autocomplete.py` & `constructor-io-1.8.1/constructor_io/modules/autocomplete.py`

 * *Files identical despite different names*

### Comparing `constructor-io-1.8.0/constructor_io/modules/browse.py` & `constructor-io-1.8.1/constructor_io/modules/browse.py`

 * *Files identical despite different names*

### Comparing `constructor-io-1.8.0/constructor_io/modules/catalog.py` & `constructor-io-1.8.1/constructor_io/modules/catalog.py`

 * *Files identical despite different names*

### Comparing `constructor-io-1.8.0/constructor_io/modules/quizzes.py` & `constructor-io-1.8.1/constructor_io/modules/quizzes.py`

 * *Files identical despite different names*

### Comparing `constructor-io-1.8.0/constructor_io/modules/recommendations.py` & `constructor-io-1.8.1/constructor_io/modules/recommendations.py`

 * *Files identical despite different names*

### Comparing `constructor-io-1.8.0/constructor_io/modules/search.py` & `constructor-io-1.8.1/constructor_io/modules/search.py`

 * *Files identical despite different names*

### Comparing `constructor-io-1.8.0/constructor_io/modules/tasks.py` & `constructor-io-1.8.1/constructor_io/modules/tasks.py`

 * *Files identical despite different names*

### Comparing `constructor-io-1.8.0/constructor_io.egg-info/PKG-INFO` & `constructor-io-1.8.1/constructor_io.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: constructor-io
-Version: 1.8.0
+Version: 1.8.1
 Summary: Constructor.IO Python Client
 Home-page: https://www.constructor.io
 Author: Constructor.io
 Author-email: info@constructor.io
 License: MIT
-Download-URL: https://github.com/Constructor-io/constructor-io/tarball/1.8.0
+Download-URL: https://github.com/Constructor-io/constructor-io/tarball/1.8.1
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Constructor.io Python Client
 
 [![Version](https://img.shields.io/pypi/v/constructor-io.svg)](https://pypi.python.org/pypi/constructor-io)
```

### Comparing `constructor-io-1.8.0/constructor_io.egg-info/SOURCES.txt` & `constructor-io-1.8.1/constructor_io.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `constructor-io-1.8.0/setup.py` & `constructor-io-1.8.1/setup.py`

 * *Files identical despite different names*

