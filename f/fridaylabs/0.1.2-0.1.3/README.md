# Comparing `tmp/fridaylabs-0.1.2.tar.gz` & `tmp/fridaylabs-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fridaylabs-0.1.2.tar", last modified: Tue May 21 06:19:38 2024, max compression
+gzip compressed data, was "fridaylabs-0.1.3.tar", last modified: Tue May 21 06:34:59 2024, max compression
```

## Comparing `fridaylabs-0.1.2.tar` & `fridaylabs-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ricky      (501) staff       (20)        0 2024-05-21 06:19:38.193146 fridaylabs-0.1.2/
--rw-r--r--   0 ricky      (501) staff       (20)     1070 2024-05-21 04:23:26.000000 fridaylabs-0.1.2/LICENSE
--rw-r--r--   0 ricky      (501) staff       (20)     1275 2024-05-21 06:19:38.192855 fridaylabs-0.1.2/PKG-INFO
--rw-r--r--   0 ricky      (501) staff       (20)      792 2024-05-21 05:35:31.000000 fridaylabs-0.1.2/README.md
-drwxr-xr-x   0 ricky      (501) staff       (20)        0 2024-05-21 06:19:38.189963 fridaylabs-0.1.2/fridaylabs/
--rw-r--r--   0 ricky      (501) staff       (20)       61 2024-05-21 05:49:44.000000 fridaylabs-0.1.2/fridaylabs/__init__.py
--rw-r--r--   0 ricky      (501) staff       (20)     4742 2024-05-21 06:18:44.000000 fridaylabs-0.1.2/fridaylabs/fridaylabs.py
-drwxr-xr-x   0 ricky      (501) staff       (20)        0 2024-05-21 06:19:38.192449 fridaylabs-0.1.2/fridaylabs.egg-info/
--rw-r--r--   0 ricky      (501) staff       (20)     1275 2024-05-21 06:19:38.000000 fridaylabs-0.1.2/fridaylabs.egg-info/PKG-INFO
--rw-r--r--   0 ricky      (501) staff       (20)      243 2024-05-21 06:19:38.000000 fridaylabs-0.1.2/fridaylabs.egg-info/SOURCES.txt
--rw-r--r--   0 ricky      (501) staff       (20)        1 2024-05-21 06:19:38.000000 fridaylabs-0.1.2/fridaylabs.egg-info/dependency_links.txt
--rw-r--r--   0 ricky      (501) staff       (20)        9 2024-05-21 06:19:38.000000 fridaylabs-0.1.2/fridaylabs.egg-info/requires.txt
--rw-r--r--   0 ricky      (501) staff       (20)       11 2024-05-21 06:19:38.000000 fridaylabs-0.1.2/fridaylabs.egg-info/top_level.txt
--rw-r--r--   0 ricky      (501) staff       (20)       38 2024-05-21 06:19:38.193215 fridaylabs-0.1.2/setup.cfg
--rw-r--r--   0 ricky      (501) staff       (20)      693 2024-05-21 06:19:26.000000 fridaylabs-0.1.2/setup.py
+drwxr-xr-x   0 ricky      (501) staff       (20)        0 2024-05-21 06:34:59.632537 fridaylabs-0.1.3/
+-rw-r--r--   0 ricky      (501) staff       (20)     1070 2024-05-21 04:23:26.000000 fridaylabs-0.1.3/LICENSE
+-rw-r--r--   0 ricky      (501) staff       (20)     1275 2024-05-21 06:34:59.632268 fridaylabs-0.1.3/PKG-INFO
+-rw-r--r--   0 ricky      (501) staff       (20)      792 2024-05-21 05:35:31.000000 fridaylabs-0.1.3/README.md
+drwxr-xr-x   0 ricky      (501) staff       (20)        0 2024-05-21 06:34:59.630769 fridaylabs-0.1.3/fridaylabs/
+-rw-r--r--   0 ricky      (501) staff       (20)       61 2024-05-21 05:49:44.000000 fridaylabs-0.1.3/fridaylabs/__init__.py
+-rw-r--r--   0 ricky      (501) staff       (20)     4714 2024-05-21 06:34:49.000000 fridaylabs-0.1.3/fridaylabs/fridaylabs.py
+drwxr-xr-x   0 ricky      (501) staff       (20)        0 2024-05-21 06:34:59.631994 fridaylabs-0.1.3/fridaylabs.egg-info/
+-rw-r--r--   0 ricky      (501) staff       (20)     1275 2024-05-21 06:34:59.000000 fridaylabs-0.1.3/fridaylabs.egg-info/PKG-INFO
+-rw-r--r--   0 ricky      (501) staff       (20)      243 2024-05-21 06:34:59.000000 fridaylabs-0.1.3/fridaylabs.egg-info/SOURCES.txt
+-rw-r--r--   0 ricky      (501) staff       (20)        1 2024-05-21 06:34:59.000000 fridaylabs-0.1.3/fridaylabs.egg-info/dependency_links.txt
+-rw-r--r--   0 ricky      (501) staff       (20)        9 2024-05-21 06:34:59.000000 fridaylabs-0.1.3/fridaylabs.egg-info/requires.txt
+-rw-r--r--   0 ricky      (501) staff       (20)       11 2024-05-21 06:34:59.000000 fridaylabs-0.1.3/fridaylabs.egg-info/top_level.txt
+-rw-r--r--   0 ricky      (501) staff       (20)       38 2024-05-21 06:34:59.632600 fridaylabs-0.1.3/setup.cfg
+-rw-r--r--   0 ricky      (501) staff       (20)      693 2024-05-21 06:34:53.000000 fridaylabs-0.1.3/setup.py
```

### Comparing `fridaylabs-0.1.2/LICENSE` & `fridaylabs-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fridaylabs-0.1.2/PKG-INFO` & `fridaylabs-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fridaylabs
-Version: 0.1.2
+Version: 0.1.3
 Summary: A package to interact with FridayLabs AI API
 Home-page: https://github.com/ImJustRicky/fridaylabs-package
 Author: FridayLabs
 Author-email: fridaylabs@fridaylabs.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fridaylabs-0.1.2/README.md` & `fridaylabs-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `fridaylabs-0.1.2/fridaylabs/fridaylabs.py` & `fridaylabs-0.1.3/fridaylabs/fridaylabs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# fridaylabs/fridaylabs.py
-
 import requests
 
 class Colors:
     HEADER = "\033[95m"
     OKBLUE = "\033[94m"
     OKGREEN = "\033[92m"
     WARNING = "\033[93m"
```

### Comparing `fridaylabs-0.1.2/fridaylabs.egg-info/PKG-INFO` & `fridaylabs-0.1.3/fridaylabs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fridaylabs
-Version: 0.1.2
+Version: 0.1.3
 Summary: A package to interact with FridayLabs AI API
 Home-page: https://github.com/ImJustRicky/fridaylabs-package
 Author: FridayLabs
 Author-email: fridaylabs@fridaylabs.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fridaylabs-0.1.2/setup.py` & `fridaylabs-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # setup.py
 from setuptools import setup, find_packages
 
 setup(
     name="fridaylabs",
-    version="0.1.2",
+    version="0.1.3",
     packages=find_packages(),
     install_requires=["requests"],  # Add any dependencies here
     author="FridayLabs",
     author_email="fridaylabs@fridaylabs.ai",
     description="A package to interact with FridayLabs AI API",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
```

