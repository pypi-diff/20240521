# Comparing `tmp/cdk-constructs-1.8.4.tar.gz` & `tmp/cdk-constructs-1.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-constructs-1.8.4.tar", last modified: Fri May 17 19:13:43 2024, max compression
+gzip compressed data, was "cdk-constructs-1.8.5.tar", last modified: Tue May 21 12:21:23 2024, max compression
```

## Comparing `cdk-constructs-1.8.4.tar` & `cdk-constructs-1.8.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:13:43.577456 cdk-constructs-1.8.4/
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-05-17 19:13:33.000000 cdk-constructs-1.8.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-17 19:13:33.000000 cdk-constructs-1.8.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-05-17 19:13:43.577456 cdk-constructs-1.8.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-05-17 19:13:33.000000 cdk-constructs-1.8.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-17 19:13:33.000000 cdk-constructs-1.8.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 19:13:43.577456 cdk-constructs-1.8.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-17 19:13:33.000000 cdk-constructs-1.8.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:13:43.573456 cdk-constructs-1.8.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:13:43.577456 cdk-constructs-1.8.4/src/cdk-constructs/
--rw-r--r--   0 runner    (1001) docker     (127)    55680 2024-05-17 19:13:33.000000 cdk-constructs-1.8.4/src/cdk-constructs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:13:43.577456 cdk-constructs-1.8.4/src/cdk-constructs/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-17 19:13:33.000000 cdk-constructs-1.8.4/src/cdk-constructs/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    42842 2024-05-17 19:13:33.000000 cdk-constructs-1.8.4/src/cdk-constructs/_jsii/cdk-constructs@1.8.4.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 19:13:33.000000 cdk-constructs-1.8.4/src/cdk-constructs/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:13:43.577456 cdk-constructs-1.8.4/src/cdk_constructs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-05-17 19:13:43.000000 cdk-constructs-1.8.4/src/cdk_constructs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-17 19:13:43.000000 cdk-constructs-1.8.4/src/cdk_constructs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 19:13:43.000000 cdk-constructs-1.8.4/src/cdk_constructs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-17 19:13:43.000000 cdk-constructs-1.8.4/src/cdk_constructs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-17 19:13:43.000000 cdk-constructs-1.8.4/src/cdk_constructs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:21:23.970782 cdk-constructs-1.8.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-05-21 12:21:07.000000 cdk-constructs-1.8.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-21 12:21:07.000000 cdk-constructs-1.8.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-05-21 12:21:23.970782 cdk-constructs-1.8.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-05-21 12:21:07.000000 cdk-constructs-1.8.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-21 12:21:07.000000 cdk-constructs-1.8.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 12:21:23.970782 cdk-constructs-1.8.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-21 12:21:07.000000 cdk-constructs-1.8.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:21:23.966782 cdk-constructs-1.8.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:21:23.966782 cdk-constructs-1.8.5/src/cdk-constructs/
+-rw-r--r--   0 runner    (1001) docker     (127)    55680 2024-05-21 12:21:07.000000 cdk-constructs-1.8.5/src/cdk-constructs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:21:23.970782 cdk-constructs-1.8.5/src/cdk-constructs/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-21 12:21:07.000000 cdk-constructs-1.8.5/src/cdk-constructs/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42844 2024-05-21 12:21:07.000000 cdk-constructs-1.8.5/src/cdk-constructs/_jsii/cdk-constructs@1.8.5.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 12:21:07.000000 cdk-constructs-1.8.5/src/cdk-constructs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:21:23.970782 cdk-constructs-1.8.5/src/cdk_constructs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-05-21 12:21:23.000000 cdk-constructs-1.8.5/src/cdk_constructs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-21 12:21:23.000000 cdk-constructs-1.8.5/src/cdk_constructs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 12:21:23.000000 cdk-constructs-1.8.5/src/cdk_constructs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-21 12:21:23.000000 cdk-constructs-1.8.5/src/cdk_constructs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-21 12:21:23.000000 cdk-constructs-1.8.5/src/cdk_constructs.egg-info/top_level.txt
```

### Comparing `cdk-constructs-1.8.4/LICENSE` & `cdk-constructs-1.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-constructs-1.8.4/PKG-INFO` & `cdk-constructs-1.8.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-constructs
-Version: 1.8.4
+Version: 1.8.5
 Summary: A CDK construct library
 Home-page: https://github.com/tm-lcarvalho/cdk-constructs.git
 Author: tm-lcarvalho<lucio.carvalho@toumoro.com>
 License: GPL-3.0-or-later
 Project-URL: Source, https://github.com/tm-lcarvalho/cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-constructs-1.8.4/README.md` & `cdk-constructs-1.8.5/README.md`

 * *Files identical despite different names*

### Comparing `cdk-constructs-1.8.4/setup.py` & `cdk-constructs-1.8.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-constructs",
-    "version": "1.8.4",
+    "version": "1.8.5",
     "description": "A CDK construct library",
     "license": "GPL-3.0-or-later",
     "url": "https://github.com/tm-lcarvalho/cdk-constructs.git",
     "long_description_content_type": "text/markdown",
     "author": "tm-lcarvalho<lucio.carvalho@toumoro.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk-constructs",
         "cdk-constructs._jsii"
     ],
     "package_data": {
         "cdk-constructs._jsii": [
-            "cdk-constructs@1.8.4.jsii.tgz"
+            "cdk-constructs@1.8.5.jsii.tgz"
         ],
         "cdk-constructs": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `cdk-constructs-1.8.4/src/cdk-constructs/__init__.py` & `cdk-constructs-1.8.5/src/cdk-constructs/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-constructs-1.8.4/src/cdk_constructs.egg-info/PKG-INFO` & `cdk-constructs-1.8.5/src/cdk_constructs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-constructs
-Version: 1.8.4
+Version: 1.8.5
 Summary: A CDK construct library
 Home-page: https://github.com/tm-lcarvalho/cdk-constructs.git
 Author: tm-lcarvalho<lucio.carvalho@toumoro.com>
 License: GPL-3.0-or-later
 Project-URL: Source, https://github.com/tm-lcarvalho/cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

