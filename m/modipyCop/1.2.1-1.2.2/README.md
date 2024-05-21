# Comparing `tmp/modipyCop-1.2.1.tar.gz` & `tmp/modipyCop-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modipyCop-1.2.1.tar", last modified: Wed May 15 05:46:21 2024, max compression
+gzip compressed data, was "modipyCop-1.2.2.tar", last modified: Tue May 21 06:24:57 2024, max compression
```

## Comparing `modipyCop-1.2.1.tar` & `modipyCop-1.2.2.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxr-xr-x   0 nicospok   (501) staff       (20)        0 2024-05-15 05:46:21.194083 modipyCop-1.2.1/
--rw-r--r--   0 nicospok   (501) staff       (20)     1066 2024-05-15 05:39:55.000000 modipyCop-1.2.1/LICENSE
--rw-r--r--   0 nicospok   (501) staff       (20)     2923 2024-05-15 05:46:21.193354 modipyCop-1.2.1/PKG-INFO
--rw-r--r--   0 nicospok   (501) staff       (20)     2480 2024-05-15 05:39:55.000000 modipyCop-1.2.1/README.md
-drwxr-xr-x   0 nicospok   (501) staff       (20)        0 2024-05-15 05:46:21.189301 modipyCop-1.2.1/cop/
--rw-r--r--   0 nicospok   (501) staff       (20)        6 2024-05-15 05:39:55.000000 modipyCop-1.2.1/cop/__init__.py
--rw-r--r--   0 nicospok   (501) staff       (20)     2824 2024-05-15 05:39:55.000000 modipyCop-1.2.1/cop/cop.py
-drwxr-xr-x   0 nicospok   (501) staff       (20)        0 2024-05-15 05:46:21.192556 modipyCop-1.2.1/modipyCop.egg-info/
--rw-r--r--   0 nicospok   (501) staff       (20)     2923 2024-05-15 05:46:20.000000 modipyCop-1.2.1/modipyCop.egg-info/PKG-INFO
--rw-r--r--   0 nicospok   (501) staff       (20)      185 2024-05-15 05:46:21.000000 modipyCop-1.2.1/modipyCop.egg-info/SOURCES.txt
--rw-r--r--   0 nicospok   (501) staff       (20)        1 2024-05-15 05:46:20.000000 modipyCop-1.2.1/modipyCop.egg-info/dependency_links.txt
--rw-r--r--   0 nicospok   (501) staff       (20)        4 2024-05-15 05:46:20.000000 modipyCop-1.2.1/modipyCop.egg-info/top_level.txt
--rw-r--r--   0 nicospok   (501) staff       (20)       38 2024-05-15 05:46:21.194275 modipyCop-1.2.1/setup.cfg
--rw-r--r--   0 nicospok   (501) staff       (20)      626 2024-05-15 05:39:55.000000 modipyCop-1.2.1/setup.py
+drwxr-xr-x   0 nicospok   (501) staff       (20)        0 2024-05-21 06:24:57.115984 modipyCop-1.2.2/
+-rw-r--r--   0 nicospok   (501) staff       (20)     1066 2024-05-15 05:39:55.000000 modipyCop-1.2.2/LICENSE
+-rw-r--r--   0 nicospok   (501) staff       (20)     2923 2024-05-21 06:24:57.115086 modipyCop-1.2.2/PKG-INFO
+-rw-r--r--   0 nicospok   (501) staff       (20)     2480 2024-05-15 05:39:55.000000 modipyCop-1.2.2/README.md
+drwxr-xr-x   0 nicospok   (501) staff       (20)        0 2024-05-21 06:24:57.110749 modipyCop-1.2.2/cop/
+-rw-r--r--   0 nicospok   (501) staff       (20)     2824 2024-05-15 05:39:55.000000 modipyCop-1.2.2/cop/cop.py
+drwxr-xr-x   0 nicospok   (501) staff       (20)        0 2024-05-21 06:24:57.114041 modipyCop-1.2.2/modipyCop.egg-info/
+-rw-r--r--   0 nicospok   (501) staff       (20)     2923 2024-05-21 06:24:56.000000 modipyCop-1.2.2/modipyCop.egg-info/PKG-INFO
+-rw-r--r--   0 nicospok   (501) staff       (20)      169 2024-05-21 06:24:57.000000 modipyCop-1.2.2/modipyCop.egg-info/SOURCES.txt
+-rw-r--r--   0 nicospok   (501) staff       (20)        1 2024-05-21 06:24:56.000000 modipyCop-1.2.2/modipyCop.egg-info/dependency_links.txt
+-rw-r--r--   0 nicospok   (501) staff       (20)        1 2024-05-21 06:24:56.000000 modipyCop-1.2.2/modipyCop.egg-info/top_level.txt
+-rw-r--r--   0 nicospok   (501) staff       (20)       38 2024-05-21 06:24:57.116246 modipyCop-1.2.2/setup.cfg
+-rw-r--r--   0 nicospok   (501) staff       (20)      626 2024-05-21 06:21:37.000000 modipyCop-1.2.2/setup.py
```

### Comparing `modipyCop-1.2.1/LICENSE` & `modipyCop-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `modipyCop-1.2.1/PKG-INFO` & `modipyCop-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modipyCop
-Version: 1.2.1
+Version: 1.2.2
 Summary: Track modification made to file/s.
 Home-page: https://github.com/niCodeLine/modipy
 Author: Nico Spok
 Author-email: nicospok@hotmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `modipyCop-1.2.1/README.md` & `modipyCop-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `modipyCop-1.2.1/cop/cop.py` & `modipyCop-1.2.2/cop/cop.py`

 * *Files identical despite different names*

### Comparing `modipyCop-1.2.1/modipyCop.egg-info/PKG-INFO` & `modipyCop-1.2.2/modipyCop.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modipyCop
-Version: 1.2.1
+Version: 1.2.2
 Summary: Track modification made to file/s.
 Home-page: https://github.com/niCodeLine/modipy
 Author: Nico Spok
 Author-email: nicospok@hotmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `modipyCop-1.2.1/setup.py` & `modipyCop-1.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='modipyCop',
-    version='1.2.1',
+    version='1.2.2',
     packages=find_packages(),
     description='Track modification made to file/s.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/niCodeLine/modipy',
     author='Nico Spok',
     author_email='nicospok@hotmail.com',
```

