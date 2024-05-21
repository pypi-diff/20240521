# Comparing `tmp/hyjinx-0.29.0.tar.gz` & `tmp/hyjinx-0.29.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyjinx-0.29.0.tar", last modified: Tue May 21 09:08:02 2024, max compression
+gzip compressed data, was "hyjinx-0.29.1.tar", last modified: Tue May 21 09:31:04 2024, max compression
```

## Comparing `hyjinx-0.29.0.tar` & `hyjinx-0.29.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 user      (1001) users      (100)        0 2024-05-21 09:08:02.069175 hyjinx-0.29.0/
--rw-r--r--   0 user      (1001) users      (100)       38 2024-02-06 15:19:38.000000 hyjinx-0.29.0/AUTHORS
--rw-r--r--   0 user      (1001) users      (100)     1070 2024-02-06 14:37:46.000000 hyjinx-0.29.0/LICENSE
--rw-r--r--   0 user      (1001) users      (100)     4622 2024-05-21 09:08:02.045175 hyjinx-0.29.0/PKG-INFO
--rw-r--r--   0 user      (1001) users      (100)     1957 2024-05-08 11:47:39.000000 hyjinx-0.29.0/README.md
-drwxr-xr-x   0 user      (1001) users      (100)        0 2024-05-21 09:08:01.750175 hyjinx-0.29.0/hyjinx/
--rw-r--r--   0 user      (1001) users      (100)     2179 2024-05-21 09:06:03.000000 hyjinx-0.29.0/hyjinx/__init__.py
--rw-r--r--   0 user      (1001) users      (100)    16082 2024-05-08 14:16:43.000000 hyjinx-0.29.0/hyjinx/beautify.hy
--rw-r--r--   0 user      (1001) users      (100)     2294 2024-02-05 12:57:36.000000 hyjinx-0.29.0/hyjinx/crypto.hy
--rw-r--r--   0 user      (1001) users      (100)     2538 2024-05-08 11:51:44.000000 hyjinx-0.29.0/hyjinx/docs.hy
--rw-r--r--   0 user      (1001) users      (100)     2738 2024-05-04 00:22:53.000000 hyjinx-0.29.0/hyjinx/hyrc.hy
--rw-r--r--   0 user      (1001) users      (100)    11310 2024-05-06 19:45:02.000000 hyjinx-0.29.0/hyjinx/inspect.py
--rw-r--r--   0 user      (1001) users      (100)    10309 2024-04-30 10:37:49.000000 hyjinx-0.29.0/hyjinx/lib.hy
--rw-r--r--   0 user      (1001) users      (100)    15848 2024-05-04 19:06:11.000000 hyjinx-0.29.0/hyjinx/llm.hy
--rw-r--r--   0 user      (1001) users      (100)     3829 2024-04-29 10:47:04.000000 hyjinx-0.29.0/hyjinx/macros.hy
--rw-r--r--   0 user      (1001) users      (100)      888 2024-04-09 13:50:23.000000 hyjinx-0.29.0/hyjinx/mail.hy
--rw-r--r--   0 user      (1001) users      (100)     3979 2024-04-29 10:55:33.000000 hyjinx-0.29.0/hyjinx/mat.hy
--rw-r--r--   0 user      (1001) users      (100)    16648 2024-05-07 21:18:58.000000 hyjinx-0.29.0/hyjinx/reader.py
--rw-r--r--   0 user      (1001) users      (100)     3026 2024-04-02 12:27:35.000000 hyjinx-0.29.0/hyjinx/screen.hy
--rw-r--r--   0 user      (1001) users      (100)     8926 2024-05-07 14:02:21.000000 hyjinx-0.29.0/hyjinx/source.hy
--rw-r--r--   0 user      (1001) users      (100)     1168 2024-02-18 19:01:10.000000 hyjinx-0.29.0/hyjinx/wire.hy
--rw-r--r--   0 user      (1001) users      (100)     1178 2024-02-18 19:01:43.000000 hyjinx-0.29.0/hyjinx/zmq_client.hy
--rw-r--r--   0 user      (1001) users      (100)     1960 2024-05-21 09:03:49.000000 hyjinx-0.29.0/hyjinx/zmq_server.hy
-drwxr-xr-x   0 user      (1001) users      (100)        0 2024-05-21 09:08:01.993175 hyjinx-0.29.0/hyjinx.egg-info/
--rw-r--r--   0 user      (1001) users      (100)     4622 2024-05-21 09:08:00.000000 hyjinx-0.29.0/hyjinx.egg-info/PKG-INFO
--rw-r--r--   0 user      (1001) users      (100)      507 2024-05-21 09:08:00.000000 hyjinx-0.29.0/hyjinx.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1001) users      (100)        1 2024-05-21 09:08:00.000000 hyjinx-0.29.0/hyjinx.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1001) users      (100)       94 2024-05-21 09:08:00.000000 hyjinx-0.29.0/hyjinx.egg-info/entry_points.txt
--rw-r--r--   0 user      (1001) users      (100)      194 2024-05-21 09:08:00.000000 hyjinx-0.29.0/hyjinx.egg-info/requires.txt
--rw-r--r--   0 user      (1001) users      (100)        7 2024-05-21 09:08:00.000000 hyjinx-0.29.0/hyjinx.egg-info/top_level.txt
--rw-r--r--   0 user      (1001) users      (100)     1544 2024-05-06 15:23:59.000000 hyjinx-0.29.0/pyproject.toml
--rw-r--r--   0 user      (1001) users      (100)       38 2024-05-21 09:08:02.076175 hyjinx-0.29.0/setup.cfg
+drwxr-xr-x   0 user      (1001) users      (100)        0 2024-05-21 09:31:04.489644 hyjinx-0.29.1/
+-rw-r--r--   0 user      (1001) users      (100)       38 2024-02-06 15:19:38.000000 hyjinx-0.29.1/AUTHORS
+-rw-r--r--   0 user      (1001) users      (100)     1070 2024-02-06 14:37:46.000000 hyjinx-0.29.1/LICENSE
+-rw-r--r--   0 user      (1001) users      (100)     4622 2024-05-21 09:31:04.466644 hyjinx-0.29.1/PKG-INFO
+-rw-r--r--   0 user      (1001) users      (100)     1957 2024-05-08 11:47:39.000000 hyjinx-0.29.1/README.md
+drwxr-xr-x   0 user      (1001) users      (100)        0 2024-05-21 09:31:04.170644 hyjinx-0.29.1/hyjinx/
+-rw-r--r--   0 user      (1001) users      (100)     2179 2024-05-21 09:30:07.000000 hyjinx-0.29.1/hyjinx/__init__.py
+-rw-r--r--   0 user      (1001) users      (100)    16082 2024-05-08 14:16:43.000000 hyjinx-0.29.1/hyjinx/beautify.hy
+-rw-r--r--   0 user      (1001) users      (100)     2294 2024-02-05 12:57:36.000000 hyjinx-0.29.1/hyjinx/crypto.hy
+-rw-r--r--   0 user      (1001) users      (100)     2538 2024-05-08 11:51:44.000000 hyjinx-0.29.1/hyjinx/docs.hy
+-rw-r--r--   0 user      (1001) users      (100)     2738 2024-05-04 00:22:53.000000 hyjinx-0.29.1/hyjinx/hyrc.hy
+-rw-r--r--   0 user      (1001) users      (100)    11310 2024-05-06 19:45:02.000000 hyjinx-0.29.1/hyjinx/inspect.py
+-rw-r--r--   0 user      (1001) users      (100)    10309 2024-04-30 10:37:49.000000 hyjinx-0.29.1/hyjinx/lib.hy
+-rw-r--r--   0 user      (1001) users      (100)    15848 2024-05-04 19:06:11.000000 hyjinx-0.29.1/hyjinx/llm.hy
+-rw-r--r--   0 user      (1001) users      (100)     3829 2024-04-29 10:47:04.000000 hyjinx-0.29.1/hyjinx/macros.hy
+-rw-r--r--   0 user      (1001) users      (100)      888 2024-04-09 13:50:23.000000 hyjinx-0.29.1/hyjinx/mail.hy
+-rw-r--r--   0 user      (1001) users      (100)     3979 2024-04-29 10:55:33.000000 hyjinx-0.29.1/hyjinx/mat.hy
+-rw-r--r--   0 user      (1001) users      (100)    16648 2024-05-07 21:18:58.000000 hyjinx-0.29.1/hyjinx/reader.py
+-rw-r--r--   0 user      (1001) users      (100)     3026 2024-04-02 12:27:35.000000 hyjinx-0.29.1/hyjinx/screen.hy
+-rw-r--r--   0 user      (1001) users      (100)     8926 2024-05-07 14:02:21.000000 hyjinx-0.29.1/hyjinx/source.hy
+-rw-r--r--   0 user      (1001) users      (100)     1168 2024-02-18 19:01:10.000000 hyjinx-0.29.1/hyjinx/wire.hy
+-rw-r--r--   0 user      (1001) users      (100)     1178 2024-02-18 19:01:43.000000 hyjinx-0.29.1/hyjinx/zmq_client.hy
+-rw-r--r--   0 user      (1001) users      (100)     1960 2024-05-21 09:03:49.000000 hyjinx-0.29.1/hyjinx/zmq_server.hy
+drwxr-xr-x   0 user      (1001) users      (100)        0 2024-05-21 09:31:04.413644 hyjinx-0.29.1/hyjinx.egg-info/
+-rw-r--r--   0 user      (1001) users      (100)     4622 2024-05-21 09:31:03.000000 hyjinx-0.29.1/hyjinx.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1001) users      (100)      507 2024-05-21 09:31:03.000000 hyjinx-0.29.1/hyjinx.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1001) users      (100)        1 2024-05-21 09:31:03.000000 hyjinx-0.29.1/hyjinx.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1001) users      (100)       94 2024-05-21 09:31:03.000000 hyjinx-0.29.1/hyjinx.egg-info/entry_points.txt
+-rw-r--r--   0 user      (1001) users      (100)      194 2024-05-21 09:31:03.000000 hyjinx-0.29.1/hyjinx.egg-info/requires.txt
+-rw-r--r--   0 user      (1001) users      (100)        7 2024-05-21 09:31:03.000000 hyjinx-0.29.1/hyjinx.egg-info/top_level.txt
+-rw-r--r--   0 user      (1001) users      (100)     1544 2024-05-21 09:29:35.000000 hyjinx-0.29.1/pyproject.toml
+-rw-r--r--   0 user      (1001) users      (100)       38 2024-05-21 09:31:04.496644 hyjinx-0.29.1/setup.cfg
```

### Comparing `hyjinx-0.29.0/LICENSE` & `hyjinx-0.29.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hyjinx-0.29.0/PKG-INFO` & `hyjinx-0.29.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyjinx
-Version: 0.29.0
+Version: 0.29.1
 Summary: A minimal Hy utility library, using mostly the standard libraries.
 Author-email: Ati Sharma <ati+hyjinx@agalmic.ltd>
 License: MIT License
         
         Copyright (c) 2024 the authors.
         
         Permission is hereby granted, free of charge, to any person obtaining a
@@ -34,16 +34,16 @@
 Classifier: Programming Language :: Lisp
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
-Requires-Dist: hy==0.28.0
-Requires-Dist: hyrule==0.5.0
+Requires-Dist: hy==0.29.0
+Requires-Dist: hyrule==0.6.0
 Requires-Dist: cytoolz
 Requires-Dist: more-itertools
 Requires-Dist: pansi
 Requires-Dist: platformdirs
 Requires-Dist: pygments
 Requires-Dist: multimethod
 Provides-Extra: zmq
```

### Comparing `hyjinx-0.29.0/README.md` & `hyjinx-0.29.1/README.md`

 * *Files identical despite different names*

### Comparing `hyjinx-0.29.0/hyjinx/__init__.py` & `hyjinx-0.29.1/hyjinx/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 except ModuleNotFoundError:
     pass
 
 # require all the macros
 hy.macros.require('hyjinx.macros', None, assignments = 'ALL', prefix = '')
 
 # set the package version
-__version__ = "0.29.0"
+__version__ = "0.29.1"
 __version_info__ = __version__.split(".")
 
 
 def __cli_grind_files():
     """Pretty-print hy files from the shell."""
     # The first arg is script name, ignore it.
     import sys
```

### Comparing `hyjinx-0.29.0/hyjinx/beautify.hy` & `hyjinx-0.29.1/hyjinx/beautify.hy`

 * *Files identical despite different names*

### Comparing `hyjinx-0.29.0/hyjinx/crypto.hy` & `hyjinx-0.29.1/hyjinx/crypto.hy`

 * *Files identical despite different names*

### Comparing `hyjinx-0.29.0/hyjinx/docs.hy` & `hyjinx-0.29.1/hyjinx/docs.hy`

 * *Files identical despite different names*

### Comparing `hyjinx-0.29.0/hyjinx/hyrc.hy` & `hyjinx-0.29.1/hyjinx/hyrc.hy`

 * *Files identical despite different names*

### Comparing `hyjinx-0.29.0/hyjinx/inspect.py` & `hyjinx-0.29.1/hyjinx/inspect.py`

 * *Files identical despite different names*

### Comparing `hyjinx-0.29.0/hyjinx/lib.hy` & `hyjinx-0.29.1/hyjinx/lib.hy`

 * *Files identical despite different names*

### Comparing `hyjinx-0.29.0/hyjinx/llm.hy` & `hyjinx-0.29.1/hyjinx/llm.hy`

 * *Files identical despite different names*

### Comparing `hyjinx-0.29.0/hyjinx/macros.hy` & `hyjinx-0.29.1/hyjinx/macros.hy`

 * *Files identical despite different names*

### Comparing `hyjinx-0.29.0/hyjinx/mail.hy` & `hyjinx-0.29.1/hyjinx/mail.hy`

 * *Files identical despite different names*

### Comparing `hyjinx-0.29.0/hyjinx/mat.hy` & `hyjinx-0.29.1/hyjinx/mat.hy`

 * *Files identical despite different names*

### Comparing `hyjinx-0.29.0/hyjinx/reader.py` & `hyjinx-0.29.1/hyjinx/reader.py`

 * *Files identical despite different names*

### Comparing `hyjinx-0.29.0/hyjinx/screen.hy` & `hyjinx-0.29.1/hyjinx/screen.hy`

 * *Files identical despite different names*

### Comparing `hyjinx-0.29.0/hyjinx/source.hy` & `hyjinx-0.29.1/hyjinx/source.hy`

 * *Files identical despite different names*

### Comparing `hyjinx-0.29.0/hyjinx/wire.hy` & `hyjinx-0.29.1/hyjinx/wire.hy`

 * *Files identical despite different names*

### Comparing `hyjinx-0.29.0/hyjinx/zmq_client.hy` & `hyjinx-0.29.1/hyjinx/zmq_client.hy`

 * *Files identical despite different names*

### Comparing `hyjinx-0.29.0/hyjinx/zmq_server.hy` & `hyjinx-0.29.1/hyjinx/zmq_server.hy`

 * *Files identical despite different names*

### Comparing `hyjinx-0.29.0/hyjinx.egg-info/PKG-INFO` & `hyjinx-0.29.1/hyjinx.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyjinx
-Version: 0.29.0
+Version: 0.29.1
 Summary: A minimal Hy utility library, using mostly the standard libraries.
 Author-email: Ati Sharma <ati+hyjinx@agalmic.ltd>
 License: MIT License
         
         Copyright (c) 2024 the authors.
         
         Permission is hereby granted, free of charge, to any person obtaining a
@@ -34,16 +34,16 @@
 Classifier: Programming Language :: Lisp
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
-Requires-Dist: hy==0.28.0
-Requires-Dist: hyrule==0.5.0
+Requires-Dist: hy==0.29.0
+Requires-Dist: hyrule==0.6.0
 Requires-Dist: cytoolz
 Requires-Dist: more-itertools
 Requires-Dist: pansi
 Requires-Dist: platformdirs
 Requires-Dist: pygments
 Requires-Dist: multimethod
 Provides-Extra: zmq
```

### Comparing `hyjinx-0.29.0/pyproject.toml` & `hyjinx-0.29.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -20,16 +20,16 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Lisp",
     "Topic :: Software Development :: Libraries",
     "Topic :: Utilities"
 ]
 dependencies = [
-    "hy==0.28.0",
-    "hyrule==0.5.0",
+    "hy==0.29.0",
+    "hyrule==0.6.0",
     "cytoolz",
     "more-itertools",
     "pansi",
     "platformdirs",
     "pygments",
     "multimethod"
 ]
```

