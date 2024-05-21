# Comparing `tmp/fridaylabs-0.1.0.tar.gz` & `tmp/fridaylabs-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fridaylabs-0.1.0.tar", last modified: Tue May 21 05:45:17 2024, max compression
+gzip compressed data, was "fridaylabs-0.1.1.tar", last modified: Tue May 21 05:51:14 2024, max compression
```

## Comparing `fridaylabs-0.1.0.tar` & `fridaylabs-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ricky      (501) staff       (20)        0 2024-05-21 05:45:17.506957 fridaylabs-0.1.0/
--rw-r--r--   0 ricky      (501) staff       (20)     1070 2024-05-21 04:23:26.000000 fridaylabs-0.1.0/LICENSE
--rw-r--r--   0 ricky      (501) staff       (20)     1275 2024-05-21 05:45:17.506723 fridaylabs-0.1.0/PKG-INFO
--rw-r--r--   0 ricky      (501) staff       (20)      792 2024-05-21 05:35:31.000000 fridaylabs-0.1.0/README.md
-drwxr-xr-x   0 ricky      (501) staff       (20)        0 2024-05-21 05:45:17.505237 fridaylabs-0.1.0/fridaylabs/
--rw-r--r--   0 ricky      (501) staff       (20)        0 2024-05-21 04:25:44.000000 fridaylabs-0.1.0/fridaylabs/__init__.py
--rw-r--r--   0 ricky      (501) staff       (20)      837 2024-05-21 05:36:01.000000 fridaylabs-0.1.0/fridaylabs/fridaylabs.py
-drwxr-xr-x   0 ricky      (501) staff       (20)        0 2024-05-21 05:45:17.506435 fridaylabs-0.1.0/fridaylabs.egg-info/
--rw-r--r--   0 ricky      (501) staff       (20)     1275 2024-05-21 05:45:17.000000 fridaylabs-0.1.0/fridaylabs.egg-info/PKG-INFO
--rw-r--r--   0 ricky      (501) staff       (20)      243 2024-05-21 05:45:17.000000 fridaylabs-0.1.0/fridaylabs.egg-info/SOURCES.txt
--rw-r--r--   0 ricky      (501) staff       (20)        1 2024-05-21 05:45:17.000000 fridaylabs-0.1.0/fridaylabs.egg-info/dependency_links.txt
--rw-r--r--   0 ricky      (501) staff       (20)        9 2024-05-21 05:45:17.000000 fridaylabs-0.1.0/fridaylabs.egg-info/requires.txt
--rw-r--r--   0 ricky      (501) staff       (20)       11 2024-05-21 05:45:17.000000 fridaylabs-0.1.0/fridaylabs.egg-info/top_level.txt
--rw-r--r--   0 ricky      (501) staff       (20)       38 2024-05-21 05:45:17.507015 fridaylabs-0.1.0/setup.cfg
--rw-r--r--   0 ricky      (501) staff       (20)      693 2024-05-21 05:35:18.000000 fridaylabs-0.1.0/setup.py
+drwxr-xr-x   0 ricky      (501) staff       (20)        0 2024-05-21 05:51:14.228457 fridaylabs-0.1.1/
+-rw-r--r--   0 ricky      (501) staff       (20)     1070 2024-05-21 04:23:26.000000 fridaylabs-0.1.1/LICENSE
+-rw-r--r--   0 ricky      (501) staff       (20)     1275 2024-05-21 05:51:14.228205 fridaylabs-0.1.1/PKG-INFO
+-rw-r--r--   0 ricky      (501) staff       (20)      792 2024-05-21 05:35:31.000000 fridaylabs-0.1.1/README.md
+drwxr-xr-x   0 ricky      (501) staff       (20)        0 2024-05-21 05:51:14.226759 fridaylabs-0.1.1/fridaylabs/
+-rw-r--r--   0 ricky      (501) staff       (20)       61 2024-05-21 05:49:44.000000 fridaylabs-0.1.1/fridaylabs/__init__.py
+-rw-r--r--   0 ricky      (501) staff       (20)      837 2024-05-21 05:49:53.000000 fridaylabs-0.1.1/fridaylabs/fridaylabs.py
+drwxr-xr-x   0 ricky      (501) staff       (20)        0 2024-05-21 05:51:14.227923 fridaylabs-0.1.1/fridaylabs.egg-info/
+-rw-r--r--   0 ricky      (501) staff       (20)     1275 2024-05-21 05:51:14.000000 fridaylabs-0.1.1/fridaylabs.egg-info/PKG-INFO
+-rw-r--r--   0 ricky      (501) staff       (20)      243 2024-05-21 05:51:14.000000 fridaylabs-0.1.1/fridaylabs.egg-info/SOURCES.txt
+-rw-r--r--   0 ricky      (501) staff       (20)        1 2024-05-21 05:51:14.000000 fridaylabs-0.1.1/fridaylabs.egg-info/dependency_links.txt
+-rw-r--r--   0 ricky      (501) staff       (20)        9 2024-05-21 05:51:14.000000 fridaylabs-0.1.1/fridaylabs.egg-info/requires.txt
+-rw-r--r--   0 ricky      (501) staff       (20)       11 2024-05-21 05:51:14.000000 fridaylabs-0.1.1/fridaylabs.egg-info/top_level.txt
+-rw-r--r--   0 ricky      (501) staff       (20)       38 2024-05-21 05:51:14.228520 fridaylabs-0.1.1/setup.cfg
+-rw-r--r--   0 ricky      (501) staff       (20)      693 2024-05-21 05:50:58.000000 fridaylabs-0.1.1/setup.py
```

### Comparing `fridaylabs-0.1.0/LICENSE` & `fridaylabs-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fridaylabs-0.1.0/PKG-INFO` & `fridaylabs-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fridaylabs
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package to interact with FridayLabs AI API
 Home-page: https://github.com/ImJustRicky/fridaylabs-package
 Author: FridayLabs
 Author-email: fridaylabs@fridaylabs.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fridaylabs-0.1.0/README.md` & `fridaylabs-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `fridaylabs-0.1.0/fridaylabs/fridaylabs.py` & `fridaylabs-0.1.1/fridaylabs/fridaylabs.py`

 * *Files identical despite different names*

### Comparing `fridaylabs-0.1.0/fridaylabs.egg-info/PKG-INFO` & `fridaylabs-0.1.1/fridaylabs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fridaylabs
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package to interact with FridayLabs AI API
 Home-page: https://github.com/ImJustRicky/fridaylabs-package
 Author: FridayLabs
 Author-email: fridaylabs@fridaylabs.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fridaylabs-0.1.0/setup.py` & `fridaylabs-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # setup.py
 from setuptools import setup, find_packages
 
 setup(
     name="fridaylabs",
-    version="0.1.0",
+    version="0.1.1",
     packages=find_packages(),
     install_requires=["requests"],  # Add any dependencies here
     author="FridayLabs",
     author_email="fridaylabs@fridaylabs.ai",
     description="A package to interact with FridayLabs AI API",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
```

