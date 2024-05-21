# Comparing `tmp/udirect-0.1.3.dev0.tar.gz` & `tmp/udirect-0.1.4.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "udirect-0.1.3.dev0.tar", last modified: Tue May 21 14:46:29 2024, max compression
+gzip compressed data, was "udirect-0.1.4.dev0.tar", last modified: Tue May 21 14:47:46 2024, max compression
```

## Comparing `udirect-0.1.3.dev0.tar` & `udirect-0.1.4.dev0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 lilienka  (1000) lilienka  (1000)        0 2024-05-21 14:46:29.922529 udirect-0.1.3.dev0/
--rw-rw-r--   0 lilienka  (1000) lilienka  (1000)     1074 2024-05-21 13:48:20.000000 udirect-0.1.3.dev0/LICENSE.txt
--rw-rw-r--   0 lilienka  (1000) lilienka  (1000)      743 2024-05-21 14:46:29.922529 udirect-0.1.3.dev0/PKG-INFO
--rw-rw-r--   0 lilienka  (1000) lilienka  (1000)        9 2024-05-21 12:47:16.000000 udirect-0.1.3.dev0/README.md
--rw-rw-r--   0 lilienka  (1000) lilienka  (1000)       79 2024-05-21 14:46:29.922529 udirect-0.1.3.dev0/setup.cfg
--rw-rw-r--   0 lilienka  (1000) lilienka  (1000)     1769 2024-05-21 14:46:26.000000 udirect-0.1.3.dev0/setup.py
-drwxrwxr-x   0 lilienka  (1000) lilienka  (1000)        0 2024-05-21 14:46:29.922529 udirect-0.1.3.dev0/udirect/
--rw-rw-r--   0 lilienka  (1000) lilienka  (1000)     1564 2024-05-21 12:47:16.000000 udirect-0.1.3.dev0/udirect/predictiveModel.py
-drwxrwxr-x   0 lilienka  (1000) lilienka  (1000)        0 2024-05-21 14:46:29.922529 udirect-0.1.3.dev0/udirect.egg-info/
--rw-rw-r--   0 lilienka  (1000) lilienka  (1000)      743 2024-05-21 14:46:29.000000 udirect-0.1.3.dev0/udirect.egg-info/PKG-INFO
--rw-rw-r--   0 lilienka  (1000) lilienka  (1000)      221 2024-05-21 14:46:29.000000 udirect-0.1.3.dev0/udirect.egg-info/SOURCES.txt
--rw-rw-r--   0 lilienka  (1000) lilienka  (1000)        1 2024-05-21 14:46:29.000000 udirect-0.1.3.dev0/udirect.egg-info/dependency_links.txt
--rw-rw-r--   0 lilienka  (1000) lilienka  (1000)       17 2024-05-21 14:46:29.000000 udirect-0.1.3.dev0/udirect.egg-info/requires.txt
--rw-rw-r--   0 lilienka  (1000) lilienka  (1000)        8 2024-05-21 14:46:29.000000 udirect-0.1.3.dev0/udirect.egg-info/top_level.txt
+drwxrwxr-x   0 lilienka  (1000) lilienka  (1000)        0 2024-05-21 14:47:46.159143 udirect-0.1.4.dev0/
+-rw-rw-r--   0 lilienka  (1000) lilienka  (1000)     1074 2024-05-21 13:48:20.000000 udirect-0.1.4.dev0/LICENSE.txt
+-rw-rw-r--   0 lilienka  (1000) lilienka  (1000)      743 2024-05-21 14:47:46.159143 udirect-0.1.4.dev0/PKG-INFO
+-rw-rw-r--   0 lilienka  (1000) lilienka  (1000)        9 2024-05-21 12:47:16.000000 udirect-0.1.4.dev0/README.md
+-rw-rw-r--   0 lilienka  (1000) lilienka  (1000)       79 2024-05-21 14:47:46.163143 udirect-0.1.4.dev0/setup.cfg
+-rw-rw-r--   0 lilienka  (1000) lilienka  (1000)     1769 2024-05-21 14:47:19.000000 udirect-0.1.4.dev0/setup.py
+drwxrwxr-x   0 lilienka  (1000) lilienka  (1000)        0 2024-05-21 14:47:46.159143 udirect-0.1.4.dev0/udirect/
+-rw-rw-r--   0 lilienka  (1000) lilienka  (1000)     1564 2024-05-21 12:47:16.000000 udirect-0.1.4.dev0/udirect/predictiveModel.py
+drwxrwxr-x   0 lilienka  (1000) lilienka  (1000)        0 2024-05-21 14:47:46.159143 udirect-0.1.4.dev0/udirect.egg-info/
+-rw-rw-r--   0 lilienka  (1000) lilienka  (1000)      743 2024-05-21 14:47:46.000000 udirect-0.1.4.dev0/udirect.egg-info/PKG-INFO
+-rw-rw-r--   0 lilienka  (1000) lilienka  (1000)      221 2024-05-21 14:47:46.000000 udirect-0.1.4.dev0/udirect.egg-info/SOURCES.txt
+-rw-rw-r--   0 lilienka  (1000) lilienka  (1000)        1 2024-05-21 14:47:46.000000 udirect-0.1.4.dev0/udirect.egg-info/dependency_links.txt
+-rw-rw-r--   0 lilienka  (1000) lilienka  (1000)       17 2024-05-21 14:47:46.000000 udirect-0.1.4.dev0/udirect.egg-info/requires.txt
+-rw-rw-r--   0 lilienka  (1000) lilienka  (1000)        8 2024-05-21 14:47:46.000000 udirect-0.1.4.dev0/udirect.egg-info/top_level.txt
```

### Comparing `udirect-0.1.3.dev0/LICENSE.txt` & `udirect-0.1.4.dev0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `udirect-0.1.3.dev0/PKG-INFO` & `udirect-0.1.4.dev0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: udirect
-Version: 0.1.3.dev0
+Version: 0.1.4.dev0
 Summary: Deep learning tools for modeling rupture forward directivity
 Home-page: https://github.com/HenningLilienkamp/udirect
 Download-URL: https://github.com/HenningLilienkamp/udirect/archive/refs/tags/v.0.1.tar.gz
 Author: Henning Lilienkamp
 Author-email: henninglilienkamp@gmx.de
 License: MIT
 Keywords: Deep learning,Rupture forward directivity,Modifier of moments
```

### Comparing `udirect-0.1.3.dev0/setup.py` & `udirect-0.1.4.dev0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
   name = 'udirect',         # How you named your package folder (MyLib)
   packages = ['udirect'],   # Chose the same as "name"
-  version = '0.1.3-dev.0',      # Start with a small number and increase it with every change you make
+  version = '0.1.4-dev.0',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'Deep learning tools for modeling rupture forward directivity',   # Give a short description about your library
   author = 'Henning Lilienkamp',                   # Type in your name
   author_email = 'henninglilienkamp@gmx.de',      # Type in your E-Mail
   url = 'https://github.com/HenningLilienkamp/udirect',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/HenningLilienkamp/udirect/archive/refs/tags/v.0.1.tar.gz',    # I explain this later on
   keywords = ['Deep learning', 'Rupture forward directivity', 'Modifier of moments'],   # Keywords that define your package best
```

### Comparing `udirect-0.1.3.dev0/udirect/predictiveModel.py` & `udirect-0.1.4.dev0/udirect/predictiveModel.py`

 * *Files identical despite different names*

### Comparing `udirect-0.1.3.dev0/udirect.egg-info/PKG-INFO` & `udirect-0.1.4.dev0/udirect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: udirect
-Version: 0.1.3.dev0
+Version: 0.1.4.dev0
 Summary: Deep learning tools for modeling rupture forward directivity
 Home-page: https://github.com/HenningLilienkamp/udirect
 Download-URL: https://github.com/HenningLilienkamp/udirect/archive/refs/tags/v.0.1.tar.gz
 Author: Henning Lilienkamp
 Author-email: henninglilienkamp@gmx.de
 License: MIT
 Keywords: Deep learning,Rupture forward directivity,Modifier of moments
```

