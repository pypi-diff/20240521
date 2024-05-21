# Comparing `tmp/blue_plugin-3.18.1.tar.gz` & `tmp/blue_plugin-3.19.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blue_plugin-3.18.1.tar", last modified: Tue May 21 01:17:47 2024, max compression
+gzip compressed data, was "blue_plugin-3.19.1.tar", last modified: Tue May 21 01:20:15 2024, max compression
```

## Comparing `blue_plugin-3.18.1.tar` & `blue_plugin-3.19.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-21 01:17:47.518281 blue_plugin-3.18.1/
--rw-r--r--   0 kamangir   (502) staff       (20)     7048 2022-09-09 01:44:55.000000 blue_plugin-3.18.1/LICENSE
--rw-r--r--   0 kamangir   (502) staff       (20)       24 2024-05-20 04:48:46.000000 blue_plugin-3.18.1/MANIFEST.in
--rw-r--r--   0 kamangir   (502) staff       (20)     1595 2024-05-21 01:17:47.517906 blue_plugin-3.18.1/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)      754 2024-05-19 22:49:48.000000 blue_plugin-3.18.1/README.md
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-21 01:17:47.515348 blue_plugin-3.18.1/blue_plugin/
--rw-r--r--   0 kamangir   (502) staff       (20)      128 2024-05-21 01:17:44.000000 blue_plugin-3.18.1/blue_plugin/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      239 2024-05-21 00:08:25.000000 blue_plugin-3.18.1/blue_plugin/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)       25 2024-04-19 01:49:55.000000 blue_plugin-3.18.1/blue_plugin/config.env
--rw-r--r--   0 kamangir   (502) staff       (20)      235 2024-04-27 21:22:01.000000 blue_plugin-3.18.1/blue_plugin/env.py
--rw-r--r--   0 kamangir   (502) staff       (20)        0 2024-02-25 23:41:15.000000 blue_plugin-3.18.1/blue_plugin/functions.py
--rw-r--r--   0 kamangir   (502) staff       (20)       92 2024-03-24 00:16:06.000000 blue_plugin-3.18.1/blue_plugin/logger.py
--rw-r--r--   0 kamangir   (502) staff       (20)       17 2022-08-20 02:33:38.000000 blue_plugin-3.18.1/blue_plugin/urls.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-21 01:17:47.517440 blue_plugin-3.18.1/blue_plugin.egg-info/
--rw-r--r--   0 kamangir   (502) staff       (20)     1595 2024-05-21 01:17:47.000000 blue_plugin-3.18.1/blue_plugin.egg-info/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)      386 2024-05-21 01:17:47.000000 blue_plugin-3.18.1/blue_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-21 01:17:47.000000 blue_plugin-3.18.1/blue_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 kamangir   (502) staff       (20)      131 2024-05-21 01:17:47.000000 blue_plugin-3.18.1/blue_plugin.egg-info/requires.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       12 2024-05-21 01:17:47.000000 blue_plugin-3.18.1/blue_plugin.egg-info/top_level.txt
--rw-r--r--   0 kamangir   (502) staff       (20)      131 2024-05-20 22:39:24.000000 blue_plugin-3.18.1/requirements.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-21 01:17:47.518353 blue_plugin-3.18.1/setup.cfg
--rw-r--r--   0 kamangir   (502) staff       (20)      259 2024-05-21 01:00:35.000000 blue_plugin-3.18.1/setup.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-21 01:20:15.140232 blue_plugin-3.19.1/
+-rw-r--r--   0 kamangir   (502) staff       (20)     7048 2022-09-09 01:44:55.000000 blue_plugin-3.19.1/LICENSE
+-rw-r--r--   0 kamangir   (502) staff       (20)       24 2024-05-20 04:48:46.000000 blue_plugin-3.19.1/MANIFEST.in
+-rw-r--r--   0 kamangir   (502) staff       (20)     1595 2024-05-21 01:20:15.139815 blue_plugin-3.19.1/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)      754 2024-05-19 22:49:48.000000 blue_plugin-3.19.1/README.md
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-21 01:20:15.135893 blue_plugin-3.19.1/blue_plugin/
+-rw-r--r--   0 kamangir   (502) staff       (20)      128 2024-05-21 01:20:12.000000 blue_plugin-3.19.1/blue_plugin/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      239 2024-05-21 00:08:25.000000 blue_plugin-3.19.1/blue_plugin/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       25 2024-04-19 01:49:55.000000 blue_plugin-3.19.1/blue_plugin/config.env
+-rw-r--r--   0 kamangir   (502) staff       (20)      235 2024-04-27 21:22:01.000000 blue_plugin-3.19.1/blue_plugin/env.py
+-rw-r--r--   0 kamangir   (502) staff       (20)        0 2024-02-25 23:41:15.000000 blue_plugin-3.19.1/blue_plugin/functions.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       92 2024-03-24 00:16:06.000000 blue_plugin-3.19.1/blue_plugin/logger.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       17 2022-08-20 02:33:38.000000 blue_plugin-3.19.1/blue_plugin/urls.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-21 01:20:15.139272 blue_plugin-3.19.1/blue_plugin.egg-info/
+-rw-r--r--   0 kamangir   (502) staff       (20)     1595 2024-05-21 01:20:15.000000 blue_plugin-3.19.1/blue_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)      386 2024-05-21 01:20:15.000000 blue_plugin-3.19.1/blue_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-21 01:20:15.000000 blue_plugin-3.19.1/blue_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)      131 2024-05-21 01:20:15.000000 blue_plugin-3.19.1/blue_plugin.egg-info/requires.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       12 2024-05-21 01:20:15.000000 blue_plugin-3.19.1/blue_plugin.egg-info/top_level.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)      131 2024-05-20 22:39:24.000000 blue_plugin-3.19.1/requirements.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-21 01:20:15.140316 blue_plugin-3.19.1/setup.cfg
+-rw-r--r--   0 kamangir   (502) staff       (20)      259 2024-05-21 01:00:35.000000 blue_plugin-3.19.1/setup.py
```

### Comparing `blue_plugin-3.18.1/LICENSE` & `blue_plugin-3.19.1/LICENSE`

 * *Files identical despite different names*

### Comparing `blue_plugin-3.18.1/PKG-INFO` & `blue_plugin-3.19.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blue_plugin
-Version: 3.18.1
+Version: 3.19.1
 Summary: 🌀 a git template for an awesome-bash-cli plugin.
 Home-page: https://github.com/kamangir/blue-plugin
 Author: Arash Abadpour (Kamangir)
 Author-email: arash@kamangir.net
 License: Public Domain
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Unix Shell
```

### Comparing `blue_plugin-3.18.1/README.md` & `blue_plugin-3.19.1/README.md`

 * *Files identical despite different names*

### Comparing `blue_plugin-3.18.1/blue_plugin.egg-info/PKG-INFO` & `blue_plugin-3.19.1/blue_plugin.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blue-plugin
-Version: 3.18.1
+Version: 3.19.1
 Summary: 🌀 a git template for an awesome-bash-cli plugin.
 Home-page: https://github.com/kamangir/blue-plugin
 Author: Arash Abadpour (Kamangir)
 Author-email: arash@kamangir.net
 License: Public Domain
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Unix Shell
```

