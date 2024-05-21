# Comparing `tmp/dictoat-1.0.1.tar.gz` & `tmp/dictoat-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dictoat-1.0.1.tar", last modified: Wed May 15 05:49:18 2024, max compression
+gzip compressed data, was "dictoat-1.0.2.tar", last modified: Tue May 21 06:24:27 2024, max compression
```

## Comparing `dictoat-1.0.1.tar` & `dictoat-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxr-xr-x   0 nicospok   (501) staff       (20)        0 2024-05-15 05:49:18.916274 dictoat-1.0.1/
--rw-r--r--   0 nicospok   (501) staff       (20)     1066 2024-05-15 05:40:04.000000 dictoat-1.0.1/LICENSE
--rw-r--r--   0 nicospok   (501) staff       (20)     3639 2024-05-15 05:49:18.915102 dictoat-1.0.1/PKG-INFO
--rw-r--r--   0 nicospok   (501) staff       (20)     3178 2024-05-15 05:40:04.000000 dictoat-1.0.1/README.md
-drwxr-xr-x   0 nicospok   (501) staff       (20)        0 2024-05-15 05:49:18.910170 dictoat-1.0.1/dictoat/
--rw-r--r--   0 nicospok   (501) staff       (20)     6148 2024-05-15 05:40:04.000000 dictoat-1.0.1/dictoat/.DS_Store
--rw-r--r--   0 nicospok   (501) staff       (20)        6 2024-05-15 05:40:04.000000 dictoat-1.0.1/dictoat/__init__.py
--rw-r--r--   0 nicospok   (501) staff       (20)      529 2024-05-15 05:40:04.000000 dictoat-1.0.1/dictoat/dictoat.py
-drwxr-xr-x   0 nicospok   (501) staff       (20)        0 2024-05-15 05:49:18.914162 dictoat-1.0.1/dictoat.egg-info/
--rw-r--r--   0 nicospok   (501) staff       (20)     3639 2024-05-15 05:49:17.000000 dictoat-1.0.1/dictoat.egg-info/PKG-INFO
--rw-r--r--   0 nicospok   (501) staff       (20)      207 2024-05-15 05:49:18.000000 dictoat-1.0.1/dictoat.egg-info/SOURCES.txt
--rw-r--r--   0 nicospok   (501) staff       (20)        1 2024-05-15 05:49:17.000000 dictoat-1.0.1/dictoat.egg-info/dependency_links.txt
--rw-r--r--   0 nicospok   (501) staff       (20)        8 2024-05-15 05:49:17.000000 dictoat-1.0.1/dictoat.egg-info/top_level.txt
--rw-r--r--   0 nicospok   (501) staff       (20)       38 2024-05-15 05:49:18.916514 dictoat-1.0.1/setup.cfg
--rw-r--r--   0 nicospok   (501) staff       (20)      650 2024-05-15 05:40:04.000000 dictoat-1.0.1/setup.py
+drwxr-xr-x   0 nicospok   (501) staff       (20)        0 2024-05-21 06:24:27.757303 dictoat-1.0.2/
+-rw-r--r--   0 nicospok   (501) staff       (20)     1066 2024-05-15 05:40:04.000000 dictoat-1.0.2/LICENSE
+-rw-r--r--   0 nicospok   (501) staff       (20)     3639 2024-05-21 06:24:27.756427 dictoat-1.0.2/PKG-INFO
+-rw-r--r--   0 nicospok   (501) staff       (20)     3178 2024-05-15 05:40:04.000000 dictoat-1.0.2/README.md
+drwxr-xr-x   0 nicospok   (501) staff       (20)        0 2024-05-21 06:24:27.751504 dictoat-1.0.2/dictoat/
+-rw-r--r--   0 nicospok   (501) staff       (20)     6148 2024-05-21 06:21:01.000000 dictoat-1.0.2/dictoat/.DS_Store
+-rw-r--r--   0 nicospok   (501) staff       (20)      529 2024-05-15 05:40:04.000000 dictoat-1.0.2/dictoat/dictoat.py
+drwxr-xr-x   0 nicospok   (501) staff       (20)        0 2024-05-21 06:24:27.755335 dictoat-1.0.2/dictoat.egg-info/
+-rw-r--r--   0 nicospok   (501) staff       (20)     3639 2024-05-21 06:24:27.000000 dictoat-1.0.2/dictoat.egg-info/PKG-INFO
+-rw-r--r--   0 nicospok   (501) staff       (20)      187 2024-05-21 06:24:27.000000 dictoat-1.0.2/dictoat.egg-info/SOURCES.txt
+-rw-r--r--   0 nicospok   (501) staff       (20)        1 2024-05-21 06:24:27.000000 dictoat-1.0.2/dictoat.egg-info/dependency_links.txt
+-rw-r--r--   0 nicospok   (501) staff       (20)        1 2024-05-21 06:24:27.000000 dictoat-1.0.2/dictoat.egg-info/top_level.txt
+-rw-r--r--   0 nicospok   (501) staff       (20)       38 2024-05-21 06:24:27.757568 dictoat-1.0.2/setup.cfg
+-rw-r--r--   0 nicospok   (501) staff       (20)      650 2024-05-21 06:21:08.000000 dictoat-1.0.2/setup.py
```

### Comparing `dictoat-1.0.1/LICENSE` & `dictoat-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dictoat-1.0.1/PKG-INFO` & `dictoat-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dictoat
-Version: 1.0.1
+Version: 1.0.2
 Summary: Convert a dict into an object to access items faster.
 Home-page: https://github.com/niCodeLine/dictoat
 Author: Nico Spok
 Author-email: nicospok@hotmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dictoat-1.0.1/README.md` & `dictoat-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `dictoat-1.0.1/dictoat/dictoat.py` & `dictoat-1.0.2/dictoat/dictoat.py`

 * *Files identical despite different names*

### Comparing `dictoat-1.0.1/dictoat.egg-info/PKG-INFO` & `dictoat-1.0.2/dictoat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dictoat
-Version: 1.0.1
+Version: 1.0.2
 Summary: Convert a dict into an object to access items faster.
 Home-page: https://github.com/niCodeLine/dictoat
 Author: Nico Spok
 Author-email: nicospok@hotmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dictoat-1.0.1/setup.py` & `dictoat-1.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='dictoat',
-    version='1.0.1',
+    version='1.0.2',
     packages=find_packages(),
     description='Convert a dict into an object to access items faster.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/niCodeLine/dictoat',
     author='Nico Spok',
     author_email='nicospok@hotmail.com',
```

