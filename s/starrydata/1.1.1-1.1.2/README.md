# Comparing `tmp/starrydata-1.1.1.tar.gz` & `tmp/starrydata-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starrydata-1.1.1.tar", last modified: Tue May 21 08:04:24 2024, max compression
+gzip compressed data, was "starrydata-1.1.2.tar", last modified: Tue May 21 08:24:42 2024, max compression
```

## Comparing `starrydata-1.1.1.tar` & `starrydata-1.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 matotomoya   (501) staff       (20)        0 2024-05-21 08:04:24.462881 starrydata-1.1.1/
--rw-r--r--   0 matotomoya   (501) staff       (20)     1073 2023-12-12 10:27:13.000000 starrydata-1.1.1/LICENSE
--rw-r--r--   0 matotomoya   (501) staff       (20)     2790 2024-05-21 08:04:24.462542 starrydata-1.1.1/PKG-INFO
--rw-r--r--   0 matotomoya   (501) staff       (20)     2198 2024-05-21 07:56:14.000000 starrydata-1.1.1/README.md
--rw-r--r--   0 matotomoya   (501) staff       (20)      576 2024-05-21 08:04:22.000000 starrydata-1.1.1/pyproject.toml
--rw-r--r--   0 matotomoya   (501) staff       (20)       38 2024-05-21 08:04:24.462967 starrydata-1.1.1/setup.cfg
-drwxr-xr-x   0 matotomoya   (501) staff       (20)        0 2024-05-21 08:04:24.459452 starrydata-1.1.1/src/
-drwxr-xr-x   0 matotomoya   (501) staff       (20)        0 2024-05-21 08:04:24.460490 starrydata-1.1.1/src/starrydata/
--rw-r--r--   0 matotomoya   (501) staff       (20)      183 2024-05-21 06:08:13.000000 starrydata-1.1.1/src/starrydata/__init__.py
--rw-r--r--   0 matotomoya   (501) staff       (20)     6532 2024-05-21 07:16:15.000000 starrydata-1.1.1/src/starrydata/dataset.py
--rw-r--r--   0 matotomoya   (501) staff       (20)     4914 2024-05-12 10:10:09.000000 starrydata-1.1.1/src/starrydata/test_dataset.py
-drwxr-xr-x   0 matotomoya   (501) staff       (20)        0 2024-05-21 08:04:24.462181 starrydata-1.1.1/src/starrydata.egg-info/
--rw-r--r--   0 matotomoya   (501) staff       (20)     2790 2024-05-21 08:04:24.000000 starrydata-1.1.1/src/starrydata.egg-info/PKG-INFO
--rw-r--r--   0 matotomoya   (501) staff       (20)      305 2024-05-21 08:04:24.000000 starrydata-1.1.1/src/starrydata.egg-info/SOURCES.txt
--rw-r--r--   0 matotomoya   (501) staff       (20)        1 2024-05-21 08:04:24.000000 starrydata-1.1.1/src/starrydata.egg-info/dependency_links.txt
--rw-r--r--   0 matotomoya   (501) staff       (20)       21 2024-05-21 08:04:24.000000 starrydata-1.1.1/src/starrydata.egg-info/requires.txt
--rw-r--r--   0 matotomoya   (501) staff       (20)       11 2024-05-21 08:04:24.000000 starrydata-1.1.1/src/starrydata.egg-info/top_level.txt
+drwxr-xr-x   0 matotomoya   (501) staff       (20)        0 2024-05-21 08:24:42.142511 starrydata-1.1.2/
+-rw-r--r--   0 matotomoya   (501) staff       (20)     1073 2023-12-12 10:27:13.000000 starrydata-1.1.2/LICENSE
+-rw-r--r--   0 matotomoya   (501) staff       (20)     2790 2024-05-21 08:24:42.142119 starrydata-1.1.2/PKG-INFO
+-rw-r--r--   0 matotomoya   (501) staff       (20)     2198 2024-05-21 07:56:14.000000 starrydata-1.1.2/README.md
+-rw-r--r--   0 matotomoya   (501) staff       (20)      576 2024-05-21 08:24:39.000000 starrydata-1.1.2/pyproject.toml
+-rw-r--r--   0 matotomoya   (501) staff       (20)       38 2024-05-21 08:24:42.142613 starrydata-1.1.2/setup.cfg
+drwxr-xr-x   0 matotomoya   (501) staff       (20)        0 2024-05-21 08:24:42.139142 starrydata-1.1.2/src/
+drwxr-xr-x   0 matotomoya   (501) staff       (20)        0 2024-05-21 08:24:42.140136 starrydata-1.1.2/src/starrydata/
+-rw-r--r--   0 matotomoya   (501) staff       (20)      183 2024-05-21 06:08:13.000000 starrydata-1.1.2/src/starrydata/__init__.py
+-rw-r--r--   0 matotomoya   (501) staff       (20)     6532 2024-05-21 07:16:15.000000 starrydata-1.1.2/src/starrydata/dataset.py
+-rw-r--r--   0 matotomoya   (501) staff       (20)     4914 2024-05-12 10:10:09.000000 starrydata-1.1.2/src/starrydata/test_dataset.py
+drwxr-xr-x   0 matotomoya   (501) staff       (20)        0 2024-05-21 08:24:42.141663 starrydata-1.1.2/src/starrydata.egg-info/
+-rw-r--r--   0 matotomoya   (501) staff       (20)     2790 2024-05-21 08:24:42.000000 starrydata-1.1.2/src/starrydata.egg-info/PKG-INFO
+-rw-r--r--   0 matotomoya   (501) staff       (20)      305 2024-05-21 08:24:42.000000 starrydata-1.1.2/src/starrydata.egg-info/SOURCES.txt
+-rw-r--r--   0 matotomoya   (501) staff       (20)        1 2024-05-21 08:24:42.000000 starrydata-1.1.2/src/starrydata.egg-info/dependency_links.txt
+-rw-r--r--   0 matotomoya   (501) staff       (20)       21 2024-05-21 08:24:42.000000 starrydata-1.1.2/src/starrydata.egg-info/requires.txt
+-rw-r--r--   0 matotomoya   (501) staff       (20)       11 2024-05-21 08:24:42.000000 starrydata-1.1.2/src/starrydata.egg-info/top_level.txt
```

### Comparing `starrydata-1.1.1/LICENSE` & `starrydata-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `starrydata-1.1.1/PKG-INFO` & `starrydata-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starrydata
-Version: 1.1.1
+Version: 1.1.2
 Summary: Starrydata Python useful tools 
 Author-email: MATO Tomoya <tomoya.matou@gmail.com>
 Project-URL: Homepage, https://github.com/starrydata/starrydata-python-library
 Project-URL: Issues, https://github.com/starrydata/starrydata-python-library/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `starrydata-1.1.1/README.md` & `starrydata-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `starrydata-1.1.1/pyproject.toml` & `starrydata-1.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "starrydata"
-version = "1.1.1"
+version = "1.1.2"
 authors = [
   { name="MATO Tomoya", email="tomoya.matou@gmail.com" },
 ]
 description = "Starrydata Python useful tools "
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `starrydata-1.1.1/src/starrydata/dataset.py` & `starrydata-1.1.2/src/starrydata/dataset.py`

 * *Files identical despite different names*

### Comparing `starrydata-1.1.1/src/starrydata/test_dataset.py` & `starrydata-1.1.2/src/starrydata/test_dataset.py`

 * *Files identical despite different names*

### Comparing `starrydata-1.1.1/src/starrydata.egg-info/PKG-INFO` & `starrydata-1.1.2/src/starrydata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starrydata
-Version: 1.1.1
+Version: 1.1.2
 Summary: Starrydata Python useful tools 
 Author-email: MATO Tomoya <tomoya.matou@gmail.com>
 Project-URL: Homepage, https://github.com/starrydata/starrydata-python-library
 Project-URL: Issues, https://github.com/starrydata/starrydata-python-library/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

