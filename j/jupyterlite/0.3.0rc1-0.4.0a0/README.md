# Comparing `tmp/jupyterlite-0.3.0rc1.tar.gz` & `tmp/jupyterlite-0.4.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Mon Mar 18 13:20:32 2024, max compression
+gzip compressed data, last modified: Tue May 21 06:19:07 2024, max compression
```

## Comparing `jupyterlite-0.3.0rc1.tar` & `jupyterlite-0.4.0a0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       57 2024-03-18 13:20:32.000000 jupyterlite-0.3.0rc1/jupyterlite/__init__.py
--rw-r--r--   0        0        0       81 2024-03-18 13:20:32.000000 jupyterlite-0.3.0rc1/jupyterlite/__main__.py
--rw-r--r--   0        0        0      354 2024-03-18 13:20:32.000000 jupyterlite-0.3.0rc1/jupyterlite/constants.py
--rw-r--r--   0        0        0      331 2024-03-18 13:20:32.000000 jupyterlite-0.3.0rc1/jupyterlite/addons/base.py
--rw-r--r--   0        0        0     2189 2024-03-18 13:20:32.000000 jupyterlite-0.3.0rc1/.gitignore
--rw-r--r--   0        0        0     1524 2024-03-18 13:20:32.000000 jupyterlite-0.3.0rc1/LICENSE
--rw-r--r--   0        0        0     5688 2024-03-18 13:20:32.000000 jupyterlite-0.3.0rc1/README.md
--rw-r--r--   0        0        0     1996 2024-03-18 13:20:32.000000 jupyterlite-0.3.0rc1/pyproject.toml
--rw-r--r--   0        0        0     9544 2024-03-18 13:20:32.000000 jupyterlite-0.3.0rc1/PKG-INFO
+-rw-r--r--   0        0        0       56 2024-05-21 06:19:07.000000 jupyterlite-0.4.0a0/jupyterlite/__init__.py
+-rw-r--r--   0        0        0       81 2024-05-21 06:19:07.000000 jupyterlite-0.4.0a0/jupyterlite/__main__.py
+-rw-r--r--   0        0        0      354 2024-05-21 06:19:07.000000 jupyterlite-0.4.0a0/jupyterlite/constants.py
+-rw-r--r--   0        0        0      331 2024-05-21 06:19:07.000000 jupyterlite-0.4.0a0/jupyterlite/addons/base.py
+-rw-r--r--   0        0        0     2189 2024-05-21 06:19:07.000000 jupyterlite-0.4.0a0/.gitignore
+-rw-r--r--   0        0        0     1524 2024-05-21 06:19:07.000000 jupyterlite-0.4.0a0/LICENSE
+-rw-r--r--   0        0        0     5688 2024-05-21 06:19:07.000000 jupyterlite-0.4.0a0/README.md
+-rw-r--r--   0        0        0     1995 2024-05-21 06:19:07.000000 jupyterlite-0.4.0a0/pyproject.toml
+-rw-r--r--   0        0        0     9542 2024-05-21 06:19:07.000000 jupyterlite-0.4.0a0/PKG-INFO
```

### Comparing `jupyterlite-0.3.0rc1/.gitignore` & `jupyterlite-0.4.0a0/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlite-0.3.0rc1/LICENSE` & `jupyterlite-0.4.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlite-0.3.0rc1/README.md` & `jupyterlite-0.4.0a0/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlite-0.3.0rc1/pyproject.toml` & `jupyterlite-0.4.0a0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "jupyterlite"
 authors = [
     {name = "JupyterLite Contributors"},
 ]
 dependencies = [
-    "jupyterlite-core >=0.3.0rc1",
+    "jupyterlite-core >=0.4.0a0",
 ]
 keywords = [
     "browser",
     "js",
     "jupyter",
     "jupyterlab",
     "notebook",
@@ -47,15 +47,15 @@
 
 [project.optional-dependencies]
 libarchive = [
     "libarchive-c >=4.0",
 ]
 lab = [
     "jupyterlab >=4.1.0,<4.2",
-    "notebook >=7.1.0,<7.2",
+    "notebook >=7.2.0,<7.3",
 ]
 contents = [
     "jupyter_server",
 ]
 translation = [
     "jupyterlab_server >=2.8.1,<3",
 ]
@@ -64,18 +64,18 @@
 ]
 check = [
     "jsonschema[format_nongpl] >=3",
 ]
 all = [
     "jsonschema >=3",
     "jupyter_server",
-    "jupyterlab >=4.1.1,<4.2",
+    "jupyterlab >=4.2.0,<4.3",
     "jupyterlab_server >=2.8.1,<3",
     "libarchive-c >=4.0",
-    "notebook >=7.1.0,<7.2",
+    "notebook >=7.2.0,<7.3",
     "pkginfo",
     "tornado >=6.1",
 ]
 
 [tool.hatch.version]
 path = "jupyterlite/__init__.py"
```

### Comparing `jupyterlite-0.3.0rc1/PKG-INFO` & `jupyterlite-0.4.0a0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: jupyterlite
-Version: 0.3.0rc1
+Version: 0.4.0a0
 Dynamic: Summary
 Project-URL: Source, https://github.com/jupyterlite/jupyterlite
 Author: JupyterLite Contributors
 License: BSD 3-Clause License
         
         Copyright (c) 2022, JupyterLite Contributors
         All rights reserved.
@@ -48,31 +48,31 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Software Development :: Pre-processors
 Classifier: Topic :: Text Processing :: Markup :: HTML
 Requires-Python: >=3.8
-Requires-Dist: jupyterlite-core>=0.3.0rc1
+Requires-Dist: jupyterlite-core>=0.4.0a0
 Provides-Extra: all
 Requires-Dist: jsonschema>=3; extra == 'all'
 Requires-Dist: jupyter-server; extra == 'all'
 Requires-Dist: jupyterlab-server<3,>=2.8.1; extra == 'all'
-Requires-Dist: jupyterlab<4.2,>=4.1.1; extra == 'all'
+Requires-Dist: jupyterlab<4.3,>=4.2.0; extra == 'all'
 Requires-Dist: libarchive-c>=4.0; extra == 'all'
-Requires-Dist: notebook<7.2,>=7.1.0; extra == 'all'
+Requires-Dist: notebook<7.3,>=7.2.0; extra == 'all'
 Requires-Dist: pkginfo; extra == 'all'
 Requires-Dist: tornado>=6.1; extra == 'all'
 Provides-Extra: check
 Requires-Dist: jsonschema[format-nongpl]>=3; extra == 'check'
 Provides-Extra: contents
 Requires-Dist: jupyter-server; extra == 'contents'
 Provides-Extra: lab
 Requires-Dist: jupyterlab<4.2,>=4.1.0; extra == 'lab'
-Requires-Dist: notebook<7.2,>=7.1.0; extra == 'lab'
+Requires-Dist: notebook<7.3,>=7.2.0; extra == 'lab'
 Provides-Extra: libarchive
 Requires-Dist: libarchive-c>=4.0; extra == 'libarchive'
 Provides-Extra: serve
 Requires-Dist: tornado>=6.1; extra == 'serve'
 Provides-Extra: translation
 Requires-Dist: jupyterlab-server<3,>=2.8.1; extra == 'translation'
 Description-Content-Type: text/markdown
```

