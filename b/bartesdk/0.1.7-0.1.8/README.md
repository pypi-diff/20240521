# Comparing `tmp/BarteSDK-0.1.7.tar.gz` & `tmp/bartesdk-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BarteSDK-0.1.7.tar", last modified: Mon May 20 22:23:35 2024, max compression
+gzip compressed data, was "bartesdk-0.1.8.tar", last modified: Tue May 21 10:25:46 2024, max compression
```

## Comparing `BarteSDK-0.1.7.tar` & `bartesdk-0.1.8.tar`

### file list

```diff
@@ -1,18 +1,12 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 22:23:35.689404 BarteSDK-0.1.7/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 22:23:35.689404 BarteSDK-0.1.7/BarteSDK.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4076 2024-05-20 22:23:35.000000 BarteSDK-0.1.7/BarteSDK.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      269 2024-05-20 22:23:35.000000 BarteSDK-0.1.7/BarteSDK.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-20 22:23:35.000000 BarteSDK-0.1.7/BarteSDK.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-05-20 22:23:35.000000 BarteSDK-0.1.7/BarteSDK.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-20 22:23:35.000000 BarteSDK-0.1.7/BarteSDK.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)        0 2024-05-20 21:33:08.000000 BarteSDK-0.1.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4076 2024-05-20 22:23:35.689404 BarteSDK-0.1.7/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     3800 2024-05-20 21:33:08.000000 BarteSDK-0.1.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 22:23:35.689404 BarteSDK-0.1.7/charges/
--rw-rw-r--   0 root         (0) root         (0)       56 2024-05-20 22:23:18.000000 BarteSDK-0.1.7/charges/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      667 2024-05-20 22:23:18.000000 BarteSDK-0.1.7/charges/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 22:23:35.689404 BarteSDK-0.1.7/reportsellers/
--rw-rw-r--   0 root         (0) root         (0)       32 2024-05-20 21:33:08.000000 BarteSDK-0.1.7/reportsellers/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      719 2024-05-20 21:33:08.000000 BarteSDK-0.1.7/reportsellers/main.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-20 22:23:35.689404 BarteSDK-0.1.7/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)      562 2024-05-20 22:23:20.000000 BarteSDK-0.1.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 10:25:46.629469 bartesdk-0.1.8/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-05-21 10:23:50.000000 bartesdk-0.1.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4076 2024-05-21 10:25:46.629469 bartesdk-0.1.8/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     3800 2024-05-21 10:23:50.000000 bartesdk-0.1.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 10:25:46.629469 bartesdk-0.1.8/bartesdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4076 2024-05-21 10:25:46.000000 bartesdk-0.1.8/bartesdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      185 2024-05-21 10:25:46.000000 bartesdk-0.1.8/bartesdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 10:25:46.000000 bartesdk-0.1.8/bartesdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-21 10:25:46.000000 bartesdk-0.1.8/bartesdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 10:25:46.000000 bartesdk-0.1.8/bartesdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-21 10:25:46.629469 bartesdk-0.1.8/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)      562 2024-05-21 10:25:27.000000 bartesdk-0.1.8/setup.py
```

### Comparing `BarteSDK-0.1.7/BarteSDK.egg-info/PKG-INFO` & `bartesdk-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: BarteSDK
-Version: 0.1.7
+Name: bartesdk
+Version: 0.1.8
 Summary: SDK para interação com a API da Barte.
 Author: Engenharia de Plataforma da Barte
 Author-email: devops@barte.com
 License: MIT
 Keywords: barte pay sdk
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `BarteSDK-0.1.7/PKG-INFO` & `bartesdk-0.1.8/bartesdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: BarteSDK
-Version: 0.1.7
+Name: bartesdk
+Version: 0.1.8
 Summary: SDK para interação com a API da Barte.
 Author: Engenharia de Plataforma da Barte
 Author-email: devops@barte.com
 License: MIT
 Keywords: barte pay sdk
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `BarteSDK-0.1.7/README.md` & `bartesdk-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `BarteSDK-0.1.7/setup.py` & `bartesdk-0.1.8/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # setup.py
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
-    name='BarteSDK',
-    version='0.1.7',
+    name='bartesdk',
+    version='0.1.8',
     packages=find_packages(),
     install_requires=[
         'requests',
     ],
     author='Engenharia de Plataforma da Barte',
     author_email='devops@barte.com',
     description='SDK para interação com a API da Barte.',
```

