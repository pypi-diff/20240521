# Comparing `tmp/blue_plugin-2.185.1.tar.gz` & `tmp/blue_plugin-2.187.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blue_plugin-2.185.1.tar", last modified: Tue May 21 00:53:59 2024, max compression
+gzip compressed data, was "blue_plugin-2.187.1.tar", last modified: Tue May 21 00:54:27 2024, max compression
```

## Comparing `blue_plugin-2.185.1.tar` & `blue_plugin-2.187.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-21 00:53:59.642583 blue_plugin-2.185.1/
--rw-r--r--   0 kamangir   (502) staff       (20)     7048 2022-09-09 01:44:55.000000 blue_plugin-2.185.1/LICENSE
--rw-r--r--   0 kamangir   (502) staff       (20)       24 2024-05-20 04:48:46.000000 blue_plugin-2.185.1/MANIFEST.in
--rw-r--r--   0 kamangir   (502) staff       (20)     1248 2024-05-21 00:53:59.642079 blue_plugin-2.185.1/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)      754 2024-05-19 22:49:48.000000 blue_plugin-2.185.1/README.md
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-21 00:53:59.639023 blue_plugin-2.185.1/blue_plugin/
--rw-r--r--   0 kamangir   (502) staff       (20)      129 2024-05-21 00:53:56.000000 blue_plugin-2.185.1/blue_plugin/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      239 2024-05-21 00:08:25.000000 blue_plugin-2.185.1/blue_plugin/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)       25 2024-04-19 01:49:55.000000 blue_plugin-2.185.1/blue_plugin/config.env
--rw-r--r--   0 kamangir   (502) staff       (20)      235 2024-04-27 21:22:01.000000 blue_plugin-2.185.1/blue_plugin/env.py
--rw-r--r--   0 kamangir   (502) staff       (20)        0 2024-02-25 23:41:15.000000 blue_plugin-2.185.1/blue_plugin/functions.py
--rw-r--r--   0 kamangir   (502) staff       (20)       92 2024-03-24 00:16:06.000000 blue_plugin-2.185.1/blue_plugin/logger.py
--rw-r--r--   0 kamangir   (502) staff       (20)       17 2022-08-20 02:33:38.000000 blue_plugin-2.185.1/blue_plugin/urls.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-21 00:53:59.641460 blue_plugin-2.185.1/blue_plugin.egg-info/
--rw-r--r--   0 kamangir   (502) staff       (20)     1248 2024-05-21 00:53:59.000000 blue_plugin-2.185.1/blue_plugin.egg-info/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)      390 2024-05-21 00:53:59.000000 blue_plugin-2.185.1/blue_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-21 00:53:59.000000 blue_plugin-2.185.1/blue_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       49 2024-05-21 00:53:59.000000 blue_plugin-2.185.1/blue_plugin.egg-info/entry_points.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       12 2024-05-21 00:53:59.000000 blue_plugin-2.185.1/blue_plugin.egg-info/top_level.txt
--rw-r--r--   0 kamangir   (502) staff       (20)      131 2024-05-20 22:39:24.000000 blue_plugin-2.185.1/requirements.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-21 00:53:59.642747 blue_plugin-2.185.1/setup.cfg
--rw-r--r--   0 kamangir   (502) staff       (20)     1172 2024-05-21 00:53:53.000000 blue_plugin-2.185.1/setup.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-21 00:54:27.666911 blue_plugin-2.187.1/
+-rw-r--r--   0 kamangir   (502) staff       (20)     7048 2022-09-09 01:44:55.000000 blue_plugin-2.187.1/LICENSE
+-rw-r--r--   0 kamangir   (502) staff       (20)       24 2024-05-20 04:48:46.000000 blue_plugin-2.187.1/MANIFEST.in
+-rw-r--r--   0 kamangir   (502) staff       (20)     1248 2024-05-21 00:54:27.666442 blue_plugin-2.187.1/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)      754 2024-05-19 22:49:48.000000 blue_plugin-2.187.1/README.md
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-21 00:54:27.663375 blue_plugin-2.187.1/blue_plugin/
+-rw-r--r--   0 kamangir   (502) staff       (20)      129 2024-05-21 00:54:23.000000 blue_plugin-2.187.1/blue_plugin/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      239 2024-05-21 00:08:25.000000 blue_plugin-2.187.1/blue_plugin/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       25 2024-04-19 01:49:55.000000 blue_plugin-2.187.1/blue_plugin/config.env
+-rw-r--r--   0 kamangir   (502) staff       (20)      235 2024-04-27 21:22:01.000000 blue_plugin-2.187.1/blue_plugin/env.py
+-rw-r--r--   0 kamangir   (502) staff       (20)        0 2024-02-25 23:41:15.000000 blue_plugin-2.187.1/blue_plugin/functions.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       92 2024-03-24 00:16:06.000000 blue_plugin-2.187.1/blue_plugin/logger.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       17 2022-08-20 02:33:38.000000 blue_plugin-2.187.1/blue_plugin/urls.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-21 00:54:27.665982 blue_plugin-2.187.1/blue_plugin.egg-info/
+-rw-r--r--   0 kamangir   (502) staff       (20)     1248 2024-05-21 00:54:27.000000 blue_plugin-2.187.1/blue_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)      390 2024-05-21 00:54:27.000000 blue_plugin-2.187.1/blue_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-21 00:54:27.000000 blue_plugin-2.187.1/blue_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       49 2024-05-21 00:54:27.000000 blue_plugin-2.187.1/blue_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       12 2024-05-21 00:54:27.000000 blue_plugin-2.187.1/blue_plugin.egg-info/top_level.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)      131 2024-05-20 22:39:24.000000 blue_plugin-2.187.1/requirements.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-21 00:54:27.666994 blue_plugin-2.187.1/setup.cfg
+-rw-r--r--   0 kamangir   (502) staff       (20)     1172 2024-05-21 00:53:53.000000 blue_plugin-2.187.1/setup.py
```

### Comparing `blue_plugin-2.185.1/LICENSE` & `blue_plugin-2.187.1/LICENSE`

 * *Files identical despite different names*

### Comparing `blue_plugin-2.185.1/PKG-INFO` & `blue_plugin-2.187.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blue_plugin
-Version: 2.185.1
+Version: 2.187.1
 Summary: 🌀 a git template for an awesome-bash-cli plugin.
 Home-page: https://github.com/kamangir/blue-plugin
 Author: arash@kamangir.net
 Author-email: arash@kamangir.net
 License: Public Domain
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Unix Shell
```

### Comparing `blue_plugin-2.185.1/README.md` & `blue_plugin-2.187.1/README.md`

 * *Files identical despite different names*

### Comparing `blue_plugin-2.185.1/blue_plugin.egg-info/PKG-INFO` & `blue_plugin-2.187.1/blue_plugin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blue_plugin
-Version: 2.185.1
+Version: 2.187.1
 Summary: 🌀 a git template for an awesome-bash-cli plugin.
 Home-page: https://github.com/kamangir/blue-plugin
 Author: arash@kamangir.net
 Author-email: arash@kamangir.net
 License: Public Domain
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Unix Shell
```

### Comparing `blue_plugin-2.185.1/setup.py` & `blue_plugin-2.187.1/setup.py`

 * *Files identical despite different names*

