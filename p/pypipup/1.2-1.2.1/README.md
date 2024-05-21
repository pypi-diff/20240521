# Comparing `tmp/pypipup-1.2.tar.gz` & `tmp/pypipup-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypipup-1.2.tar", last modified: Wed May 15 06:00:57 2024, max compression
+gzip compressed data, was "pypipup-1.2.1.tar", last modified: Tue May 21 06:25:17 2024, max compression
```

## Comparing `pypipup-1.2.tar` & `pypipup-1.2.1.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxr-xr-x   0 nicospok   (501) staff       (20)        0 2024-05-15 06:00:57.246984 pypipup-1.2/
--rw-r--r--   0 nicospok   (501) staff       (20)     1066 2024-05-15 05:40:07.000000 pypipup-1.2/LICENSE
--rw-r--r--   0 nicospok   (501) staff       (20)     1596 2024-05-15 06:00:57.246286 pypipup-1.2/PKG-INFO
--rw-r--r--   0 nicospok   (501) staff       (20)     1132 2024-05-15 05:40:07.000000 pypipup-1.2/README.md
-drwxr-xr-x   0 nicospok   (501) staff       (20)        0 2024-05-15 06:00:57.242252 pypipup-1.2/pypipup/
--rw-r--r--   0 nicospok   (501) staff       (20)        6 2024-05-15 05:40:07.000000 pypipup-1.2/pypipup/__init__.py
--rw-r--r--   0 nicospok   (501) staff       (20)     1452 2024-05-15 05:40:07.000000 pypipup-1.2/pypipup/pypipup.py
-drwxr-xr-x   0 nicospok   (501) staff       (20)        0 2024-05-15 06:00:57.245483 pypipup-1.2/pypipup.egg-info/
--rw-r--r--   0 nicospok   (501) staff       (20)     1596 2024-05-15 06:00:56.000000 pypipup-1.2/pypipup.egg-info/PKG-INFO
--rw-r--r--   0 nicospok   (501) staff       (20)      189 2024-05-15 06:00:57.000000 pypipup-1.2/pypipup.egg-info/SOURCES.txt
--rw-r--r--   0 nicospok   (501) staff       (20)        1 2024-05-15 06:00:56.000000 pypipup-1.2/pypipup.egg-info/dependency_links.txt
--rw-r--r--   0 nicospok   (501) staff       (20)        8 2024-05-15 06:00:56.000000 pypipup-1.2/pypipup.egg-info/top_level.txt
--rw-r--r--   0 nicospok   (501) staff       (20)       38 2024-05-15 06:00:57.247186 pypipup-1.2/setup.cfg
--rw-r--r--   0 nicospok   (501) staff       (20)      647 2024-05-15 05:52:11.000000 pypipup-1.2/setup.py
+drwxr-xr-x   0 nicospok   (501) staff       (20)        0 2024-05-21 06:25:17.017756 pypipup-1.2.1/
+-rw-r--r--   0 nicospok   (501) staff       (20)     1066 2024-05-15 05:40:07.000000 pypipup-1.2.1/LICENSE
+-rw-r--r--   0 nicospok   (501) staff       (20)     1598 2024-05-21 06:25:17.017036 pypipup-1.2.1/PKG-INFO
+-rw-r--r--   0 nicospok   (501) staff       (20)     1132 2024-05-15 05:40:07.000000 pypipup-1.2.1/README.md
+drwxr-xr-x   0 nicospok   (501) staff       (20)        0 2024-05-21 06:25:17.012854 pypipup-1.2.1/pypipup/
+-rw-r--r--   0 nicospok   (501) staff       (20)     1452 2024-05-15 05:40:07.000000 pypipup-1.2.1/pypipup/pypipup.py
+drwxr-xr-x   0 nicospok   (501) staff       (20)        0 2024-05-21 06:25:17.016206 pypipup-1.2.1/pypipup.egg-info/
+-rw-r--r--   0 nicospok   (501) staff       (20)     1598 2024-05-21 06:25:16.000000 pypipup-1.2.1/pypipup.egg-info/PKG-INFO
+-rw-r--r--   0 nicospok   (501) staff       (20)      169 2024-05-21 06:25:16.000000 pypipup-1.2.1/pypipup.egg-info/SOURCES.txt
+-rw-r--r--   0 nicospok   (501) staff       (20)        1 2024-05-21 06:25:16.000000 pypipup-1.2.1/pypipup.egg-info/dependency_links.txt
+-rw-r--r--   0 nicospok   (501) staff       (20)        1 2024-05-21 06:25:16.000000 pypipup-1.2.1/pypipup.egg-info/top_level.txt
+-rw-r--r--   0 nicospok   (501) staff       (20)       38 2024-05-21 06:25:17.017988 pypipup-1.2.1/setup.cfg
+-rw-r--r--   0 nicospok   (501) staff       (20)      649 2024-05-21 06:18:45.000000 pypipup-1.2.1/setup.py
```

### Comparing `pypipup-1.2/LICENSE` & `pypipup-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pypipup-1.2/PKG-INFO` & `pypipup-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypipup
-Version: 1.2
+Version: 1.2.1
 Summary: Package that identifies and updates outdated pip packages.
 Home-page: https://github.com/niCodeLine/pypipup
 Author: Nico Spok
 Author-email: nicospok@hotmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pypipup-1.2/README.md` & `pypipup-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pypipup-1.2/pypipup/pypipup.py` & `pypipup-1.2.1/pypipup/pypipup.py`

 * *Files identical despite different names*

### Comparing `pypipup-1.2/pypipup.egg-info/PKG-INFO` & `pypipup-1.2.1/pypipup.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypipup
-Version: 1.2
+Version: 1.2.1
 Summary: Package that identifies and updates outdated pip packages.
 Home-page: https://github.com/niCodeLine/pypipup
 Author: Nico Spok
 Author-email: nicospok@hotmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pypipup-1.2/setup.py` & `pypipup-1.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pypipup',
-    version='1.2',
+    version='1.2.1',
     packages=find_packages(),
     description='Package that identifies and updates outdated pip packages.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/niCodeLine/pypipup',
     author='Nico Spok',
     author_email='nicospok@hotmail.com',
```

