# Comparing `tmp/mircheck-1.1.0.tar.gz` & `tmp/mircheck-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mircheck-1.1.0.tar", last modified: Tue May 21 20:33:20 2024, max compression
+gzip compressed data, was "mircheck-1.1.1.tar", last modified: Tue May 21 20:37:46 2024, max compression
```

## Comparing `mircheck-1.1.0.tar` & `mircheck-1.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 kimbozy   (1000) kimbozy   (1000)        0 2024-05-21 20:33:20.183712 mircheck-1.1.0/
--rw-rw-r--   0 kimbozy   (1000) kimbozy   (1000)     1071 2024-05-21 19:27:54.000000 mircheck-1.1.0/LICENSE
--rw-rw-r--   0 kimbozy   (1000) kimbozy   (1000)       34 2024-05-21 20:14:57.000000 mircheck-1.1.0/MANIFEST.in
--rw-rw-r--   0 kimbozy   (1000) kimbozy   (1000)     2876 2024-05-21 20:33:20.183712 mircheck-1.1.0/PKG-INFO
--rw-rw-r--   0 kimbozy   (1000) kimbozy   (1000)     2418 2024-05-21 19:50:01.000000 mircheck-1.1.0/README.md
-drwxrwxr-x   0 kimbozy   (1000) kimbozy   (1000)        0 2024-05-21 20:33:20.183712 mircheck-1.1.0/mircheck/
--rw-rw-r--   0 kimbozy   (1000) kimbozy   (1000)        0 2024-05-21 19:27:54.000000 mircheck-1.1.0/mircheck/__init__.py
--rw-rw-r--   0 kimbozy   (1000) kimbozy   (1000)    16297 2024-05-21 19:27:54.000000 mircheck-1.1.0/mircheck/country-list.json
--rwxrwxr-x   0 kimbozy   (1000) kimbozy   (1000)     5499 2024-05-21 20:20:06.000000 mircheck-1.1.0/mircheck/mircheck.py
-drwxrwxr-x   0 kimbozy   (1000) kimbozy   (1000)        0 2024-05-21 20:33:20.183712 mircheck-1.1.0/mircheck.egg-info/
--rw-rw-r--   0 kimbozy   (1000) kimbozy   (1000)     2876 2024-05-21 20:33:20.000000 mircheck-1.1.0/mircheck.egg-info/PKG-INFO
--rw-rw-r--   0 kimbozy   (1000) kimbozy   (1000)      301 2024-05-21 20:33:20.000000 mircheck-1.1.0/mircheck.egg-info/SOURCES.txt
--rw-rw-r--   0 kimbozy   (1000) kimbozy   (1000)        1 2024-05-21 20:33:20.000000 mircheck-1.1.0/mircheck.egg-info/dependency_links.txt
--rw-rw-r--   0 kimbozy   (1000) kimbozy   (1000)       48 2024-05-21 20:33:20.000000 mircheck-1.1.0/mircheck.egg-info/entry_points.txt
--rw-rw-r--   0 kimbozy   (1000) kimbozy   (1000)       14 2024-05-21 20:33:20.000000 mircheck-1.1.0/mircheck.egg-info/requires.txt
--rw-rw-r--   0 kimbozy   (1000) kimbozy   (1000)        9 2024-05-21 20:33:20.000000 mircheck-1.1.0/mircheck.egg-info/top_level.txt
--rw-rw-r--   0 kimbozy   (1000) kimbozy   (1000)       38 2024-05-21 20:33:20.183712 mircheck-1.1.0/setup.cfg
--rw-rw-r--   0 kimbozy   (1000) kimbozy   (1000)      940 2024-05-21 20:33:12.000000 mircheck-1.1.0/setup.py
+drwxrwxr-x   0 kimbozy   (1000) kimbozy   (1000)        0 2024-05-21 20:37:46.626503 mircheck-1.1.1/
+-rw-rw-r--   0 kimbozy   (1000) kimbozy   (1000)     1071 2024-05-21 19:27:54.000000 mircheck-1.1.1/LICENSE
+-rw-rw-r--   0 kimbozy   (1000) kimbozy   (1000)       34 2024-05-21 20:14:57.000000 mircheck-1.1.1/MANIFEST.in
+-rw-rw-r--   0 kimbozy   (1000) kimbozy   (1000)     2881 2024-05-21 20:37:46.626503 mircheck-1.1.1/PKG-INFO
+-rw-rw-r--   0 kimbozy   (1000) kimbozy   (1000)     2418 2024-05-21 19:50:01.000000 mircheck-1.1.1/README.md
+drwxrwxr-x   0 kimbozy   (1000) kimbozy   (1000)        0 2024-05-21 20:37:46.626503 mircheck-1.1.1/mircheck/
+-rw-rw-r--   0 kimbozy   (1000) kimbozy   (1000)        0 2024-05-21 19:27:54.000000 mircheck-1.1.1/mircheck/__init__.py
+-rw-rw-r--   0 kimbozy   (1000) kimbozy   (1000)    16297 2024-05-21 19:27:54.000000 mircheck-1.1.1/mircheck/country-list.json
+-rwxrwxr-x   0 kimbozy   (1000) kimbozy   (1000)     5499 2024-05-21 20:20:06.000000 mircheck-1.1.1/mircheck/mircheck.py
+drwxrwxr-x   0 kimbozy   (1000) kimbozy   (1000)        0 2024-05-21 20:37:46.626503 mircheck-1.1.1/mircheck.egg-info/
+-rw-rw-r--   0 kimbozy   (1000) kimbozy   (1000)     2881 2024-05-21 20:37:46.000000 mircheck-1.1.1/mircheck.egg-info/PKG-INFO
+-rw-rw-r--   0 kimbozy   (1000) kimbozy   (1000)      301 2024-05-21 20:37:46.000000 mircheck-1.1.1/mircheck.egg-info/SOURCES.txt
+-rw-rw-r--   0 kimbozy   (1000) kimbozy   (1000)        1 2024-05-21 20:37:46.000000 mircheck-1.1.1/mircheck.egg-info/dependency_links.txt
+-rw-rw-r--   0 kimbozy   (1000) kimbozy   (1000)       48 2024-05-21 20:37:46.000000 mircheck-1.1.1/mircheck.egg-info/entry_points.txt
+-rw-rw-r--   0 kimbozy   (1000) kimbozy   (1000)        9 2024-05-21 20:37:46.000000 mircheck-1.1.1/mircheck.egg-info/requires.txt
+-rw-rw-r--   0 kimbozy   (1000) kimbozy   (1000)        9 2024-05-21 20:37:46.000000 mircheck-1.1.1/mircheck.egg-info/top_level.txt
+-rw-rw-r--   0 kimbozy   (1000) kimbozy   (1000)       38 2024-05-21 20:37:46.626503 mircheck-1.1.1/setup.cfg
+-rw-rw-r--   0 kimbozy   (1000) kimbozy   (1000)      929 2024-05-21 20:37:14.000000 mircheck-1.1.1/setup.py
```

### Comparing `mircheck-1.1.0/LICENSE` & `mircheck-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mircheck-1.1.0/PKG-INFO` & `mircheck-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: mircheck
-Version: 1.1.0
+Version: 1.1.1
 Summary: A tool to find the fastest mirror for Ubuntu and its derivatives
 Home-page: https://github.com/arkrwn/mircheck
-Author: Your Name
+Author: Arie Kurniawan
 Author-email: hubungi.aja@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mircheck-1.1.0/README.md` & `mircheck-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `mircheck-1.1.0/mircheck/country-list.json` & `mircheck-1.1.1/mircheck/country-list.json`

 * *Files identical despite different names*

### Comparing `mircheck-1.1.0/mircheck/mircheck.py` & `mircheck-1.1.1/mircheck/mircheck.py`

 * *Files identical despite different names*

### Comparing `mircheck-1.1.0/mircheck.egg-info/PKG-INFO` & `mircheck-1.1.1/mircheck.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: mircheck
-Version: 1.1.0
+Version: 1.1.1
 Summary: A tool to find the fastest mirror for Ubuntu and its derivatives
 Home-page: https://github.com/arkrwn/mircheck
-Author: Your Name
+Author: Arie Kurniawan
 Author-email: hubungi.aja@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mircheck-1.1.0/setup.py` & `mircheck-1.1.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="mircheck",
-    version="1.1.0",
-    author="Your Name",
+    version="1.1.1",
+    author="Arie Kurniawan",
     author_email="hubungi.aja@gmail.com",
     description="A tool to find the fastest mirror for Ubuntu and its derivatives",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/arkrwn/mircheck",
     packages=find_packages(),
     package_data={
@@ -20,15 +20,14 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
     install_requires=[
         "requests",
-        "json",
     ],
     entry_points={
         'console_scripts': [
             'mircheck=mircheck.main:main',
         ],
     },
 )
```

