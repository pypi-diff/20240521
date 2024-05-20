# Comparing `tmp/blueness-3.2.1.tar.gz` & `tmp/blueness-3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blueness-3.2.1.tar", last modified: Mon May 20 22:35:48 2024, max compression
+gzip compressed data, was "blueness-3.3.1.tar", last modified: Mon May 20 22:37:55 2024, max compression
```

## Comparing `blueness-3.2.1.tar` & `blueness-3.3.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-20 22:35:48.729709 blueness-3.2.1/
--rw-r--r--   0 kamangir   (502) staff       (20)     7048 2024-05-20 22:22:24.000000 blueness-3.2.1/LICENSE
--rw-r--r--   0 kamangir   (502) staff       (20)       24 2024-05-20 22:22:24.000000 blueness-3.2.1/MANIFEST.in
--rw-r--r--   0 kamangir   (502) staff       (20)      790 2024-05-20 22:35:48.729115 blueness-3.2.1/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)       11 2024-05-20 22:22:27.000000 blueness-3.2.1/README.md
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-20 22:35:48.724711 blueness-3.2.1/blueness/
--rw-r--r--   0 kamangir   (502) staff       (20)       97 2024-05-20 22:35:44.000000 blueness-3.2.1/blueness/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      191 2024-05-20 22:32:11.000000 blueness-3.2.1/blueness/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)        0 2024-05-20 22:22:24.000000 blueness-3.2.1/blueness/functions.py
--rw-r--r--   0 kamangir   (502) staff       (20)       17 2024-05-20 22:22:24.000000 blueness-3.2.1/blueness/urls.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-20 22:35:48.728231 blueness-3.2.1/blueness.egg-info/
--rw-r--r--   0 kamangir   (502) staff       (20)      790 2024-05-20 22:35:48.000000 blueness-3.2.1/blueness.egg-info/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)      295 2024-05-20 22:35:48.000000 blueness-3.2.1/blueness.egg-info/SOURCES.txt
--rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-20 22:35:48.000000 blueness-3.2.1/blueness.egg-info/dependency_links.txt
--rw-r--r--   0 kamangir   (502) staff       (20)      122 2024-05-20 22:35:48.000000 blueness-3.2.1/blueness.egg-info/requires.txt
--rw-r--r--   0 kamangir   (502) staff       (20)        9 2024-05-20 22:35:48.000000 blueness-3.2.1/blueness.egg-info/top_level.txt
--rw-r--r--   0 kamangir   (502) staff       (20)      122 2024-05-20 22:22:24.000000 blueness-3.2.1/requirements.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-20 22:35:48.729846 blueness-3.2.1/setup.cfg
--rw-r--r--   0 kamangir   (502) staff       (20)     1037 2024-05-20 22:22:27.000000 blueness-3.2.1/setup.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-20 22:37:55.046262 blueness-3.3.1/
+-rw-r--r--   0 kamangir   (502) staff       (20)     7048 2024-05-20 22:22:24.000000 blueness-3.3.1/LICENSE
+-rw-r--r--   0 kamangir   (502) staff       (20)       24 2024-05-20 22:22:24.000000 blueness-3.3.1/MANIFEST.in
+-rw-r--r--   0 kamangir   (502) staff       (20)      790 2024-05-20 22:37:55.045717 blueness-3.3.1/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)       11 2024-05-20 22:22:27.000000 blueness-3.3.1/README.md
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-20 22:37:55.043145 blueness-3.3.1/blueness/
+-rw-r--r--   0 kamangir   (502) staff       (20)       97 2024-05-20 22:37:50.000000 blueness-3.3.1/blueness/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      191 2024-05-20 22:32:11.000000 blueness-3.3.1/blueness/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)        0 2024-05-20 22:22:24.000000 blueness-3.3.1/blueness/functions.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       17 2024-05-20 22:22:24.000000 blueness-3.3.1/blueness/urls.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-20 22:37:55.045267 blueness-3.3.1/blueness.egg-info/
+-rw-r--r--   0 kamangir   (502) staff       (20)      790 2024-05-20 22:37:55.000000 blueness-3.3.1/blueness.egg-info/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)      295 2024-05-20 22:37:55.000000 blueness-3.3.1/blueness.egg-info/SOURCES.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-20 22:37:55.000000 blueness-3.3.1/blueness.egg-info/dependency_links.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)      122 2024-05-20 22:37:55.000000 blueness-3.3.1/blueness.egg-info/requires.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)        9 2024-05-20 22:37:55.000000 blueness-3.3.1/blueness.egg-info/top_level.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)      122 2024-05-20 22:22:24.000000 blueness-3.3.1/requirements.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-20 22:37:55.046372 blueness-3.3.1/setup.cfg
+-rw-r--r--   0 kamangir   (502) staff       (20)     1037 2024-05-20 22:22:27.000000 blueness-3.3.1/setup.py
```

### Comparing `blueness-3.2.1/LICENSE` & `blueness-3.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `blueness-3.2.1/PKG-INFO` & `blueness-3.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blueness
-Version: 3.2.1
+Version: 3.3.1
 Summary: 🌀 the blueness of ai.
 Home-page: https://github.com/kamangir/blue-plugin
 Author: arash@kamangir.net
 Author-email: arash@kamangir.net
 License: Public Domain
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Unix Shell
```

### Comparing `blueness-3.2.1/blueness.egg-info/PKG-INFO` & `blueness-3.3.1/blueness.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blueness
-Version: 3.2.1
+Version: 3.3.1
 Summary: 🌀 the blueness of ai.
 Home-page: https://github.com/kamangir/blue-plugin
 Author: arash@kamangir.net
 Author-email: arash@kamangir.net
 License: Public Domain
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Unix Shell
```

### Comparing `blueness-3.2.1/setup.py` & `blueness-3.3.1/setup.py`

 * *Files identical despite different names*

