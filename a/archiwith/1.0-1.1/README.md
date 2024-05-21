# Comparing `tmp/archiwith-1.0.tar.gz` & `tmp/archiwith-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "archiwith-1.0.tar", last modified: Wed May 15 05:59:00 2024, max compression
+gzip compressed data, was "archiwith-1.1.tar", last modified: Tue May 21 06:23:28 2024, max compression
```

## Comparing `archiwith-1.0.tar` & `archiwith-1.1.tar`

### file list

```diff
@@ -1,15 +1,13 @@
-drwxr-xr-x   0 nicospok   (501) staff       (20)        0 2024-05-15 05:59:00.848397 archiwith-1.0/
--rw-r--r--   0 nicospok   (501) staff       (20)     6148 2024-05-15 05:41:09.000000 archiwith-1.0/.DS_Store
--rw-r--r--   0 nicospok   (501) staff       (20)       44 2024-05-15 05:39:58.000000 archiwith-1.0/.gitignore
--rw-r--r--   0 nicospok   (501) staff       (20)     1066 2024-05-15 05:39:58.000000 archiwith-1.0/LICENSE
--rw-r--r--   0 nicospok   (501) staff       (20)     2212 2024-05-15 05:59:00.847418 archiwith-1.0/PKG-INFO
--rw-r--r--   0 nicospok   (501) staff       (20)     1753 2024-05-15 05:39:58.000000 archiwith-1.0/README.md
-drwxr-xr-x   0 nicospok   (501) staff       (20)        0 2024-05-15 05:59:00.842479 archiwith-1.0/archiwith/
--rw-r--r--   0 nicospok   (501) staff       (20)        6 2024-05-15 05:39:58.000000 archiwith-1.0/archiwith/__init__.py
-drwxr-xr-x   0 nicospok   (501) staff       (20)        0 2024-05-15 05:59:00.846489 archiwith-1.0/archiwith.egg-info/
--rw-r--r--   0 nicospok   (501) staff       (20)     2212 2024-05-15 05:59:00.000000 archiwith-1.0/archiwith.egg-info/PKG-INFO
--rw-r--r--   0 nicospok   (501) staff       (20)      201 2024-05-15 05:59:00.000000 archiwith-1.0/archiwith.egg-info/SOURCES.txt
--rw-r--r--   0 nicospok   (501) staff       (20)        1 2024-05-15 05:59:00.000000 archiwith-1.0/archiwith.egg-info/dependency_links.txt
--rw-r--r--   0 nicospok   (501) staff       (20)       10 2024-05-15 05:59:00.000000 archiwith-1.0/archiwith.egg-info/top_level.txt
--rw-r--r--   0 nicospok   (501) staff       (20)       38 2024-05-15 05:59:00.848602 archiwith-1.0/setup.cfg
--rw-r--r--   0 nicospok   (501) staff       (20)      648 2024-05-15 05:39:58.000000 archiwith-1.0/setup.py
+drwxr-xr-x   0 nicospok   (501) staff       (20)        0 2024-05-21 06:23:28.705295 archiwith-1.1/
+-rw-r--r--   0 nicospok   (501) staff       (20)     8196 2024-05-21 06:19:40.000000 archiwith-1.1/.DS_Store
+-rw-r--r--   0 nicospok   (501) staff       (20)       44 2024-05-15 05:39:58.000000 archiwith-1.1/.gitignore
+-rw-r--r--   0 nicospok   (501) staff       (20)     1066 2024-05-15 05:39:58.000000 archiwith-1.1/LICENSE
+-rw-r--r--   0 nicospok   (501) staff       (20)     2212 2024-05-21 06:23:28.704588 archiwith-1.1/PKG-INFO
+-rw-r--r--   0 nicospok   (501) staff       (20)     1753 2024-05-15 05:39:58.000000 archiwith-1.1/README.md
+drwxr-xr-x   0 nicospok   (501) staff       (20)        0 2024-05-21 06:23:28.703786 archiwith-1.1/archiwith.egg-info/
+-rw-r--r--   0 nicospok   (501) staff       (20)     2212 2024-05-21 06:23:28.000000 archiwith-1.1/archiwith.egg-info/PKG-INFO
+-rw-r--r--   0 nicospok   (501) staff       (20)      179 2024-05-21 06:23:28.000000 archiwith-1.1/archiwith.egg-info/SOURCES.txt
+-rw-r--r--   0 nicospok   (501) staff       (20)        1 2024-05-21 06:23:28.000000 archiwith-1.1/archiwith.egg-info/dependency_links.txt
+-rw-r--r--   0 nicospok   (501) staff       (20)        1 2024-05-21 06:23:28.000000 archiwith-1.1/archiwith.egg-info/top_level.txt
+-rw-r--r--   0 nicospok   (501) staff       (20)       38 2024-05-21 06:23:28.705511 archiwith-1.1/setup.cfg
+-rw-r--r--   0 nicospok   (501) staff       (20)      648 2024-05-21 06:20:33.000000 archiwith-1.1/setup.py
```

### Comparing `archiwith-1.0/LICENSE` & `archiwith-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `archiwith-1.0/PKG-INFO` & `archiwith-1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: archiwith
-Version: 1.0
+Version: 1.1
 Summary: File opener and closener when managed via `with`.
 Home-page: https://github.com/niCodeLine/archiwith
 Author: Nico Spok
 Author-email: nicospok@hotmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `archiwith-1.0/README.md` & `archiwith-1.1/README.md`

 * *Files identical despite different names*

### Comparing `archiwith-1.0/archiwith.egg-info/PKG-INFO` & `archiwith-1.1/archiwith.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: archiwith
-Version: 1.0
+Version: 1.1
 Summary: File opener and closener when managed via `with`.
 Home-page: https://github.com/niCodeLine/archiwith
 Author: Nico Spok
 Author-email: nicospok@hotmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `archiwith-1.0/setup.py` & `archiwith-1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='archiwith',
-    version='1.0',
+    version='1.1',
     packages=find_packages(),
     description='File opener and closener when managed via `with`.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/niCodeLine/archiwith',
     author='Nico Spok',
     author_email='nicospok@hotmail.com',
```

