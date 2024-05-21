# Comparing `tmp/aecdata-0.0.4.tar.gz` & `tmp/aecdata-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aecdata-0.0.4.tar", last modified: Mon May 20 13:35:42 2024, max compression
+gzip compressed data, was "aecdata-0.0.5.tar", last modified: Tue May 21 08:35:24 2024, max compression
```

## Comparing `aecdata-0.0.4.tar` & `aecdata-0.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 nicodemosvarnava   (501) staff       (20)        0 2024-05-20 13:35:42.526330 aecdata-0.0.4/
--rw-r--r--   0 nicodemosvarnava   (501) staff       (20)      554 2024-04-04 08:44:04.000000 aecdata-0.0.4/LICENSE
--rw-r--r--   0 nicodemosvarnava   (501) staff       (20)    17644 2024-05-20 13:35:42.526056 aecdata-0.0.4/PKG-INFO
--rw-r--r--   0 nicodemosvarnava   (501) staff       (20)    17067 2024-05-20 13:30:58.000000 aecdata-0.0.4/README.md
-drwxr-xr-x   0 nicodemosvarnava   (501) staff       (20)        0 2024-05-20 13:35:42.524232 aecdata-0.0.4/aecdata/
--rw-r--r--   0 nicodemosvarnava   (501) staff       (20)      104 2024-04-03 12:58:03.000000 aecdata-0.0.4/aecdata/__init__.py
--rw-r--r--   0 nicodemosvarnava   (501) staff       (20)     2445 2024-04-26 12:04:05.000000 aecdata-0.0.4/aecdata/auth.py
--rw-r--r--   0 nicodemosvarnava   (501) staff       (20)     9197 2024-04-26 12:04:05.000000 aecdata-0.0.4/aecdata/client.py
--rw-r--r--   0 nicodemosvarnava   (501) staff       (20)    39206 2024-05-20 13:00:48.000000 aecdata-0.0.4/aecdata/productdata.py
--rw-r--r--   0 nicodemosvarnava   (501) staff       (20)    20910 2024-04-26 12:04:05.000000 aecdata-0.0.4/aecdata/utils.py
-drwxr-xr-x   0 nicodemosvarnava   (501) staff       (20)        0 2024-05-20 13:35:42.525798 aecdata-0.0.4/aecdata.egg-info/
--rw-r--r--   0 nicodemosvarnava   (501) staff       (20)    17644 2024-05-20 13:35:42.000000 aecdata-0.0.4/aecdata.egg-info/PKG-INFO
--rw-r--r--   0 nicodemosvarnava   (501) staff       (20)      313 2024-05-20 13:35:42.000000 aecdata-0.0.4/aecdata.egg-info/SOURCES.txt
--rw-r--r--   0 nicodemosvarnava   (501) staff       (20)        1 2024-05-20 13:35:42.000000 aecdata-0.0.4/aecdata.egg-info/dependency_links.txt
--rw-r--r--   0 nicodemosvarnava   (501) staff       (20)       30 2024-05-20 13:35:42.000000 aecdata-0.0.4/aecdata.egg-info/requires.txt
--rw-r--r--   0 nicodemosvarnava   (501) staff       (20)       14 2024-05-20 13:35:42.000000 aecdata-0.0.4/aecdata.egg-info/top_level.txt
--rw-r--r--   0 nicodemosvarnava   (501) staff       (20)       38 2024-05-20 13:35:42.526378 aecdata-0.0.4/setup.cfg
--rw-r--r--   0 nicodemosvarnava   (501) staff       (20)      749 2024-05-20 13:34:21.000000 aecdata-0.0.4/setup.py
-drwxr-xr-x   0 nicodemosvarnava   (501) staff       (20)        0 2024-05-20 13:35:42.525642 aecdata-0.0.4/tests/
--rw-r--r--   0 nicodemosvarnava   (501) staff       (20)        0 2024-04-03 12:58:03.000000 aecdata-0.0.4/tests/__init__.py
--rw-r--r--   0 nicodemosvarnava   (501) staff       (20)        0 2024-04-03 12:58:03.000000 aecdata-0.0.4/tests/test_client.py
+drwxr-xr-x   0 nicodemosvarnava   (501) staff       (20)        0 2024-05-21 08:35:24.304315 aecdata-0.0.5/
+-rw-r--r--   0 nicodemosvarnava   (501) staff       (20)      554 2024-04-04 08:44:04.000000 aecdata-0.0.5/LICENSE
+-rw-r--r--   0 nicodemosvarnava   (501) staff       (20)    17644 2024-05-21 08:35:24.303979 aecdata-0.0.5/PKG-INFO
+-rw-r--r--   0 nicodemosvarnava   (501) staff       (20)    17067 2024-05-20 13:30:58.000000 aecdata-0.0.5/README.md
+drwxr-xr-x   0 nicodemosvarnava   (501) staff       (20)        0 2024-05-21 08:35:24.301858 aecdata-0.0.5/aecdata/
+-rw-r--r--   0 nicodemosvarnava   (501) staff       (20)      104 2024-04-03 12:58:03.000000 aecdata-0.0.5/aecdata/__init__.py
+-rw-r--r--   0 nicodemosvarnava   (501) staff       (20)     2445 2024-04-26 12:04:05.000000 aecdata-0.0.5/aecdata/auth.py
+-rw-r--r--   0 nicodemosvarnava   (501) staff       (20)     9197 2024-04-26 12:04:05.000000 aecdata-0.0.5/aecdata/client.py
+-rw-r--r--   0 nicodemosvarnava   (501) staff       (20)    39206 2024-05-20 13:00:48.000000 aecdata-0.0.5/aecdata/productdata.py
+-rw-r--r--   0 nicodemosvarnava   (501) staff       (20)    20910 2024-04-26 12:04:05.000000 aecdata-0.0.5/aecdata/utils.py
+drwxr-xr-x   0 nicodemosvarnava   (501) staff       (20)        0 2024-05-21 08:35:24.303557 aecdata-0.0.5/aecdata.egg-info/
+-rw-r--r--   0 nicodemosvarnava   (501) staff       (20)    17644 2024-05-21 08:35:24.000000 aecdata-0.0.5/aecdata.egg-info/PKG-INFO
+-rw-r--r--   0 nicodemosvarnava   (501) staff       (20)      313 2024-05-21 08:35:24.000000 aecdata-0.0.5/aecdata.egg-info/SOURCES.txt
+-rw-r--r--   0 nicodemosvarnava   (501) staff       (20)        1 2024-05-21 08:35:24.000000 aecdata-0.0.5/aecdata.egg-info/dependency_links.txt
+-rw-r--r--   0 nicodemosvarnava   (501) staff       (20)       30 2024-05-21 08:35:24.000000 aecdata-0.0.5/aecdata.egg-info/requires.txt
+-rw-r--r--   0 nicodemosvarnava   (501) staff       (20)       14 2024-05-21 08:35:24.000000 aecdata-0.0.5/aecdata.egg-info/top_level.txt
+-rw-r--r--   0 nicodemosvarnava   (501) staff       (20)       38 2024-05-21 08:35:24.304389 aecdata-0.0.5/setup.cfg
+-rw-r--r--   0 nicodemosvarnava   (501) staff       (20)      749 2024-05-21 08:34:46.000000 aecdata-0.0.5/setup.py
+drwxr-xr-x   0 nicodemosvarnava   (501) staff       (20)        0 2024-05-21 08:35:24.303384 aecdata-0.0.5/tests/
+-rw-r--r--   0 nicodemosvarnava   (501) staff       (20)        0 2024-04-03 12:58:03.000000 aecdata-0.0.5/tests/__init__.py
+-rw-r--r--   0 nicodemosvarnava   (501) staff       (20)        0 2024-04-03 12:58:03.000000 aecdata-0.0.5/tests/test_client.py
```

### Comparing `aecdata-0.0.4/LICENSE` & `aecdata-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aecdata-0.0.4/PKG-INFO` & `aecdata-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aecdata
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Python library designed to simplify access to the 2050-materials API
 Home-page: https://github.com/2050-Materials/aecdata
 Author: 2050 Materials
 Author-email: nicodemos@2050-materials.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `aecdata-0.0.4/README.md` & `aecdata-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `aecdata-0.0.4/aecdata/auth.py` & `aecdata-0.0.5/aecdata/auth.py`

 * *Files identical despite different names*

### Comparing `aecdata-0.0.4/aecdata/client.py` & `aecdata-0.0.5/aecdata/client.py`

 * *Files identical despite different names*

### Comparing `aecdata-0.0.4/aecdata/productdata.py` & `aecdata-0.0.5/aecdata/productdata.py`

 * *Files identical despite different names*

### Comparing `aecdata-0.0.4/aecdata/utils.py` & `aecdata-0.0.5/aecdata/utils.py`

 * *Files identical despite different names*

### Comparing `aecdata-0.0.4/aecdata.egg-info/PKG-INFO` & `aecdata-0.0.5/aecdata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aecdata
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Python library designed to simplify access to the 2050-materials API
 Home-page: https://github.com/2050-Materials/aecdata
 Author: 2050 Materials
 Author-email: nicodemos@2050-materials.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `aecdata-0.0.4/setup.py` & `aecdata-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="aecdata",
-    version="0.0.4",
+    version="0.0.5",
     author="2050 Materials",
     license="Apache License 2.0",
     author_email="nicodemos@2050-materials.com",
     description="A Python library designed to simplify access to the 2050-materials API",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/2050-Materials/aecdata",
```

