# Comparing `tmp/mircheck-1.1.1.tar.gz` & `tmp/mircheck-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mircheck-1.1.1.tar", last modified: Tue May 21 20:37:46 2024, max compression
+gzip compressed data, was "mircheck-1.1.2.tar", last modified: Tue May 21 20:39:27 2024, max compression
```

## Comparing `mircheck-1.1.1.tar` & `mircheck-1.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 kimbozy   (1000) kimbozy   (1000)        0 2024-05-21 20:37:46.626503 mircheck-1.1.1/
--rw-rw-r--   0 kimbozy   (1000) kimbozy   (1000)     1071 2024-05-21 19:27:54.000000 mircheck-1.1.1/LICENSE
--rw-rw-r--   0 kimbozy   (1000) kimbozy   (1000)       34 2024-05-21 20:14:57.000000 mircheck-1.1.1/MANIFEST.in
--rw-rw-r--   0 kimbozy   (1000) kimbozy   (1000)     2881 2024-05-21 20:37:46.626503 mircheck-1.1.1/PKG-INFO
--rw-rw-r--   0 kimbozy   (1000) kimbozy   (1000)     2418 2024-05-21 19:50:01.000000 mircheck-1.1.1/README.md
-drwxrwxr-x   0 kimbozy   (1000) kimbozy   (1000)        0 2024-05-21 20:37:46.626503 mircheck-1.1.1/mircheck/
--rw-rw-r--   0 kimbozy   (1000) kimbozy   (1000)        0 2024-05-21 19:27:54.000000 mircheck-1.1.1/mircheck/__init__.py
--rw-rw-r--   0 kimbozy   (1000) kimbozy   (1000)    16297 2024-05-21 19:27:54.000000 mircheck-1.1.1/mircheck/country-list.json
--rwxrwxr-x   0 kimbozy   (1000) kimbozy   (1000)     5499 2024-05-21 20:20:06.000000 mircheck-1.1.1/mircheck/mircheck.py
-drwxrwxr-x   0 kimbozy   (1000) kimbozy   (1000)        0 2024-05-21 20:37:46.626503 mircheck-1.1.1/mircheck.egg-info/
--rw-rw-r--   0 kimbozy   (1000) kimbozy   (1000)     2881 2024-05-21 20:37:46.000000 mircheck-1.1.1/mircheck.egg-info/PKG-INFO
--rw-rw-r--   0 kimbozy   (1000) kimbozy   (1000)      301 2024-05-21 20:37:46.000000 mircheck-1.1.1/mircheck.egg-info/SOURCES.txt
--rw-rw-r--   0 kimbozy   (1000) kimbozy   (1000)        1 2024-05-21 20:37:46.000000 mircheck-1.1.1/mircheck.egg-info/dependency_links.txt
--rw-rw-r--   0 kimbozy   (1000) kimbozy   (1000)       48 2024-05-21 20:37:46.000000 mircheck-1.1.1/mircheck.egg-info/entry_points.txt
--rw-rw-r--   0 kimbozy   (1000) kimbozy   (1000)        9 2024-05-21 20:37:46.000000 mircheck-1.1.1/mircheck.egg-info/requires.txt
--rw-rw-r--   0 kimbozy   (1000) kimbozy   (1000)        9 2024-05-21 20:37:46.000000 mircheck-1.1.1/mircheck.egg-info/top_level.txt
--rw-rw-r--   0 kimbozy   (1000) kimbozy   (1000)       38 2024-05-21 20:37:46.626503 mircheck-1.1.1/setup.cfg
--rw-rw-r--   0 kimbozy   (1000) kimbozy   (1000)      929 2024-05-21 20:37:14.000000 mircheck-1.1.1/setup.py
+drwxrwxr-x   0 kimbozy   (1000) kimbozy   (1000)        0 2024-05-21 20:39:27.455559 mircheck-1.1.2/
+-rw-rw-r--   0 kimbozy   (1000) kimbozy   (1000)     1071 2024-05-21 19:27:54.000000 mircheck-1.1.2/LICENSE
+-rw-rw-r--   0 kimbozy   (1000) kimbozy   (1000)       34 2024-05-21 20:14:57.000000 mircheck-1.1.2/MANIFEST.in
+-rw-rw-r--   0 kimbozy   (1000) kimbozy   (1000)     2881 2024-05-21 20:39:27.455559 mircheck-1.1.2/PKG-INFO
+-rw-rw-r--   0 kimbozy   (1000) kimbozy   (1000)     2418 2024-05-21 19:50:01.000000 mircheck-1.1.2/README.md
+drwxrwxr-x   0 kimbozy   (1000) kimbozy   (1000)        0 2024-05-21 20:39:27.455559 mircheck-1.1.2/mircheck/
+-rw-rw-r--   0 kimbozy   (1000) kimbozy   (1000)        0 2024-05-21 19:27:54.000000 mircheck-1.1.2/mircheck/__init__.py
+-rw-rw-r--   0 kimbozy   (1000) kimbozy   (1000)    16297 2024-05-21 19:27:54.000000 mircheck-1.1.2/mircheck/country-list.json
+-rwxrwxr-x   0 kimbozy   (1000) kimbozy   (1000)     5499 2024-05-21 20:20:06.000000 mircheck-1.1.2/mircheck/mircheck.py
+drwxrwxr-x   0 kimbozy   (1000) kimbozy   (1000)        0 2024-05-21 20:39:27.455559 mircheck-1.1.2/mircheck.egg-info/
+-rw-rw-r--   0 kimbozy   (1000) kimbozy   (1000)     2881 2024-05-21 20:39:27.000000 mircheck-1.1.2/mircheck.egg-info/PKG-INFO
+-rw-rw-r--   0 kimbozy   (1000) kimbozy   (1000)      301 2024-05-21 20:39:27.000000 mircheck-1.1.2/mircheck.egg-info/SOURCES.txt
+-rw-rw-r--   0 kimbozy   (1000) kimbozy   (1000)        1 2024-05-21 20:39:27.000000 mircheck-1.1.2/mircheck.egg-info/dependency_links.txt
+-rw-rw-r--   0 kimbozy   (1000) kimbozy   (1000)       43 2024-05-21 20:39:27.000000 mircheck-1.1.2/mircheck.egg-info/entry_points.txt
+-rw-rw-r--   0 kimbozy   (1000) kimbozy   (1000)        9 2024-05-21 20:39:27.000000 mircheck-1.1.2/mircheck.egg-info/requires.txt
+-rw-rw-r--   0 kimbozy   (1000) kimbozy   (1000)        9 2024-05-21 20:39:27.000000 mircheck-1.1.2/mircheck.egg-info/top_level.txt
+-rw-rw-r--   0 kimbozy   (1000) kimbozy   (1000)       38 2024-05-21 20:39:27.455559 mircheck-1.1.2/setup.cfg
+-rw-rw-r--   0 kimbozy   (1000) kimbozy   (1000)      924 2024-05-21 20:38:50.000000 mircheck-1.1.2/setup.py
```

### Comparing `mircheck-1.1.1/LICENSE` & `mircheck-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mircheck-1.1.1/PKG-INFO` & `mircheck-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mircheck
-Version: 1.1.1
+Version: 1.1.2
 Summary: A tool to find the fastest mirror for Ubuntu and its derivatives
 Home-page: https://github.com/arkrwn/mircheck
 Author: Arie Kurniawan
 Author-email: hubungi.aja@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mircheck-1.1.1/README.md` & `mircheck-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `mircheck-1.1.1/mircheck/country-list.json` & `mircheck-1.1.2/mircheck/country-list.json`

 * *Files identical despite different names*

### Comparing `mircheck-1.1.1/mircheck/mircheck.py` & `mircheck-1.1.2/mircheck/mircheck.py`

 * *Files identical despite different names*

### Comparing `mircheck-1.1.1/mircheck.egg-info/PKG-INFO` & `mircheck-1.1.2/mircheck.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mircheck
-Version: 1.1.1
+Version: 1.1.2
 Summary: A tool to find the fastest mirror for Ubuntu and its derivatives
 Home-page: https://github.com/arkrwn/mircheck
 Author: Arie Kurniawan
 Author-email: hubungi.aja@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mircheck-1.1.1/setup.py` & `mircheck-1.1.2/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="mircheck",
-    version="1.1.1",
+    version="1.1.2",
     author="Arie Kurniawan",
     author_email="hubungi.aja@gmail.com",
     description="A tool to find the fastest mirror for Ubuntu and its derivatives",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/arkrwn/mircheck",
     packages=find_packages(),
@@ -23,11 +23,11 @@
     ],
     python_requires='>=3.6',
     install_requires=[
         "requests",
     ],
     entry_points={
         'console_scripts': [
-            'mircheck=mircheck.main:main',
+            'mircheck=mircheck:main',
         ],
     },
 )
```

