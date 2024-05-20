# Comparing `tmp/BarteSDK-0.1.5.tar.gz` & `tmp/BarteSDK-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BarteSDK-0.1.5.tar", last modified: Mon May 20 21:33:29 2024, max compression
+gzip compressed data, was "BarteSDK-0.1.6.tar", last modified: Mon May 20 22:11:19 2024, max compression
```

## Comparing `BarteSDK-0.1.5.tar` & `BarteSDK-0.1.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 21:33:29.252346 BarteSDK-0.1.5/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 21:33:29.248345 BarteSDK-0.1.5/BarteChargesAPI/
--rw-rw-r--   0 root         (0) root         (0)       34 2024-05-20 21:33:08.000000 BarteSDK-0.1.5/BarteChargesAPI/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      405 2024-05-20 21:33:08.000000 BarteSDK-0.1.5/BarteChargesAPI/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 21:33:29.248345 BarteSDK-0.1.5/BarteSDK.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4076 2024-05-20 21:33:29.000000 BarteSDK-0.1.5/BarteSDK.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      285 2024-05-20 21:33:29.000000 BarteSDK-0.1.5/BarteSDK.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-20 21:33:29.000000 BarteSDK-0.1.5/BarteSDK.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-05-20 21:33:29.000000 BarteSDK-0.1.5/BarteSDK.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2024-05-20 21:33:29.000000 BarteSDK-0.1.5/BarteSDK.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)        0 2024-05-20 21:33:08.000000 BarteSDK-0.1.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4076 2024-05-20 21:33:29.248345 BarteSDK-0.1.5/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     3800 2024-05-20 21:33:08.000000 BarteSDK-0.1.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 21:33:29.248345 BarteSDK-0.1.5/reportsellers/
--rw-rw-r--   0 root         (0) root         (0)       32 2024-05-20 21:33:08.000000 BarteSDK-0.1.5/reportsellers/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      719 2024-05-20 21:33:08.000000 BarteSDK-0.1.5/reportsellers/main.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-20 21:33:29.252346 BarteSDK-0.1.5/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)      562 2024-05-20 21:33:11.000000 BarteSDK-0.1.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 22:11:19.453184 BarteSDK-0.1.6/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 22:11:19.453184 BarteSDK-0.1.6/BarteSDK.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4076 2024-05-20 22:11:19.000000 BarteSDK-0.1.6/BarteSDK.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      269 2024-05-20 22:11:19.000000 BarteSDK-0.1.6/BarteSDK.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-20 22:11:19.000000 BarteSDK-0.1.6/BarteSDK.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-20 22:11:19.000000 BarteSDK-0.1.6/BarteSDK.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-20 22:11:19.000000 BarteSDK-0.1.6/BarteSDK.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-05-20 21:33:08.000000 BarteSDK-0.1.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4076 2024-05-20 22:11:19.453184 BarteSDK-0.1.6/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     3800 2024-05-20 21:33:08.000000 BarteSDK-0.1.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 22:11:19.453184 BarteSDK-0.1.6/charges/
+-rw-rw-r--   0 root         (0) root         (0)       26 2024-05-20 22:11:00.000000 BarteSDK-0.1.6/charges/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      391 2024-05-20 22:11:00.000000 BarteSDK-0.1.6/charges/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 22:11:19.453184 BarteSDK-0.1.6/reportsellers/
+-rw-rw-r--   0 root         (0) root         (0)       32 2024-05-20 21:33:08.000000 BarteSDK-0.1.6/reportsellers/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      719 2024-05-20 21:33:08.000000 BarteSDK-0.1.6/reportsellers/main.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-20 22:11:19.453184 BarteSDK-0.1.6/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)      562 2024-05-20 22:11:03.000000 BarteSDK-0.1.6/setup.py
```

### Comparing `BarteSDK-0.1.5/BarteSDK.egg-info/PKG-INFO` & `BarteSDK-0.1.6/BarteSDK.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BarteSDK
-Version: 0.1.5
+Version: 0.1.6
 Summary: SDK para interação com a API da Barte.
 Author: Engenharia de Plataforma da Barte
 Author-email: devops@barte.com
 License: MIT
 Keywords: barte pay sdk
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `BarteSDK-0.1.5/PKG-INFO` & `BarteSDK-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BarteSDK
-Version: 0.1.5
+Version: 0.1.6
 Summary: SDK para interação com a API da Barte.
 Author: Engenharia de Plataforma da Barte
 Author-email: devops@barte.com
 License: MIT
 Keywords: barte pay sdk
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `BarteSDK-0.1.5/README.md` & `BarteSDK-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `BarteSDK-0.1.5/reportsellers/main.py` & `BarteSDK-0.1.6/reportsellers/main.py`

 * *Files identical despite different names*

### Comparing `BarteSDK-0.1.5/setup.py` & `BarteSDK-0.1.6/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='BarteSDK',
-    version='0.1.5',
+    version='0.1.6',
     packages=find_packages(),
     install_requires=[
         'requests',
     ],
     author='Engenharia de Plataforma da Barte',
     author_email='devops@barte.com',
     description='SDK para interação com a API da Barte.',
```

