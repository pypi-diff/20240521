# Comparing `tmp/cdk-constructs-1.8.6.tar.gz` & `tmp/cdk-constructs-1.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-constructs-1.8.6.tar", last modified: Tue May 21 13:50:39 2024, max compression
+gzip compressed data, was "cdk-constructs-1.8.7.tar", last modified: Tue May 21 14:05:57 2024, max compression
```

## Comparing `cdk-constructs-1.8.6.tar` & `cdk-constructs-1.8.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:50:39.952053 cdk-constructs-1.8.6/
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-05-21 13:50:29.000000 cdk-constructs-1.8.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-21 13:50:29.000000 cdk-constructs-1.8.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-05-21 13:50:39.952053 cdk-constructs-1.8.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-05-21 13:50:29.000000 cdk-constructs-1.8.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-21 13:50:29.000000 cdk-constructs-1.8.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 13:50:39.952053 cdk-constructs-1.8.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-21 13:50:29.000000 cdk-constructs-1.8.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:50:39.948053 cdk-constructs-1.8.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:50:39.952053 cdk-constructs-1.8.6/src/cdk-constructs/
--rw-r--r--   0 runner    (1001) docker     (127)    55680 2024-05-21 13:50:29.000000 cdk-constructs-1.8.6/src/cdk-constructs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:50:39.952053 cdk-constructs-1.8.6/src/cdk-constructs/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-21 13:50:29.000000 cdk-constructs-1.8.6/src/cdk-constructs/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    42815 2024-05-21 13:50:29.000000 cdk-constructs-1.8.6/src/cdk-constructs/_jsii/cdk-constructs@1.8.6.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 13:50:29.000000 cdk-constructs-1.8.6/src/cdk-constructs/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:50:39.952053 cdk-constructs-1.8.6/src/cdk_constructs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-05-21 13:50:39.000000 cdk-constructs-1.8.6/src/cdk_constructs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-21 13:50:39.000000 cdk-constructs-1.8.6/src/cdk_constructs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 13:50:39.000000 cdk-constructs-1.8.6/src/cdk_constructs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-21 13:50:39.000000 cdk-constructs-1.8.6/src/cdk_constructs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-21 13:50:39.000000 cdk-constructs-1.8.6/src/cdk_constructs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:05:57.276388 cdk-constructs-1.8.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-05-21 14:05:47.000000 cdk-constructs-1.8.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-21 14:05:47.000000 cdk-constructs-1.8.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-05-21 14:05:57.276388 cdk-constructs-1.8.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-05-21 14:05:47.000000 cdk-constructs-1.8.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-21 14:05:47.000000 cdk-constructs-1.8.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 14:05:57.276388 cdk-constructs-1.8.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-21 14:05:47.000000 cdk-constructs-1.8.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:05:57.272388 cdk-constructs-1.8.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:05:57.276388 cdk-constructs-1.8.7/src/cdk-constructs/
+-rw-r--r--   0 runner    (1001) docker     (127)    55680 2024-05-21 14:05:47.000000 cdk-constructs-1.8.7/src/cdk-constructs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:05:57.276388 cdk-constructs-1.8.7/src/cdk-constructs/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-21 14:05:47.000000 cdk-constructs-1.8.7/src/cdk-constructs/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42818 2024-05-21 14:05:47.000000 cdk-constructs-1.8.7/src/cdk-constructs/_jsii/cdk-constructs@1.8.7.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 14:05:47.000000 cdk-constructs-1.8.7/src/cdk-constructs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:05:57.276388 cdk-constructs-1.8.7/src/cdk_constructs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-05-21 14:05:57.000000 cdk-constructs-1.8.7/src/cdk_constructs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-21 14:05:57.000000 cdk-constructs-1.8.7/src/cdk_constructs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 14:05:57.000000 cdk-constructs-1.8.7/src/cdk_constructs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-21 14:05:57.000000 cdk-constructs-1.8.7/src/cdk_constructs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-21 14:05:57.000000 cdk-constructs-1.8.7/src/cdk_constructs.egg-info/top_level.txt
```

### Comparing `cdk-constructs-1.8.6/LICENSE` & `cdk-constructs-1.8.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-constructs-1.8.6/PKG-INFO` & `cdk-constructs-1.8.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-constructs
-Version: 1.8.6
+Version: 1.8.7
 Summary: A CDK construct library
 Home-page: https://github.com/tm-lcarvalho/cdk-constructs.git
 Author: tm-lcarvalho<lucio.carvalho@toumoro.com>
 License: GPL-3.0-or-later
 Project-URL: Source, https://github.com/tm-lcarvalho/cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-constructs-1.8.6/README.md` & `cdk-constructs-1.8.7/README.md`

 * *Files identical despite different names*

### Comparing `cdk-constructs-1.8.6/setup.py` & `cdk-constructs-1.8.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-constructs",
-    "version": "1.8.6",
+    "version": "1.8.7",
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
-            "cdk-constructs@1.8.6.jsii.tgz"
+            "cdk-constructs@1.8.7.jsii.tgz"
         ],
         "cdk-constructs": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `cdk-constructs-1.8.6/src/cdk-constructs/__init__.py` & `cdk-constructs-1.8.7/src/cdk-constructs/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-constructs-1.8.6/src/cdk_constructs.egg-info/PKG-INFO` & `cdk-constructs-1.8.7/src/cdk_constructs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-constructs
-Version: 1.8.6
+Version: 1.8.7
 Summary: A CDK construct library
 Home-page: https://github.com/tm-lcarvalho/cdk-constructs.git
 Author: tm-lcarvalho<lucio.carvalho@toumoro.com>
 License: GPL-3.0-or-later
 Project-URL: Source, https://github.com/tm-lcarvalho/cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

