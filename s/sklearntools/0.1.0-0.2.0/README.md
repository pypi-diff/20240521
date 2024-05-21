# Comparing `tmp/sklearntools-0.1.0.tar.gz` & `tmp/sklearntools-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sklearntools-0.1.0.tar", last modified: Tue May 21 10:29:05 2024, max compression
+gzip compressed data, was "sklearntools-0.2.0.tar", last modified: Tue May 21 10:29:57 2024, max compression
```

## Comparing `sklearntools-0.1.0.tar` & `sklearntools-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-21 10:29:05.189301 sklearntools-0.1.0/
--rw-r--r--   0 summy      (501) staff       (20)     1061 2024-05-21 10:29:05.188516 sklearntools-0.1.0/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      761 2024-05-21 10:29:01.000000 sklearntools-0.1.0/README.rst
--rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-21 10:29:05.189578 sklearntools-0.1.0/setup.cfg
--rw-r--r--   0 summy      (501) staff       (20)      882 2024-05-21 10:29:01.000000 sklearntools-0.1.0/setup.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-21 10:29:05.182940 sklearntools-0.1.0/sklearntools/
--rw-r--r--   0 summy      (501) staff       (20)     4883 2024-05-21 10:27:59.000000 sklearntools-0.1.0/sklearntools/__init__.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-21 10:29:05.187590 sklearntools-0.1.0/sklearntools.egg-info/
--rw-r--r--   0 summy      (501) staff       (20)     1061 2024-05-21 10:29:05.000000 sklearntools-0.1.0/sklearntools.egg-info/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      258 2024-05-21 10:29:05.000000 sklearntools-0.1.0/sklearntools.egg-info/SOURCES.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-21 10:29:05.000000 sklearntools-0.1.0/sklearntools.egg-info/dependency_links.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-21 10:29:05.000000 sklearntools-0.1.0/sklearntools.egg-info/not-zip-safe
--rw-r--r--   0 summy      (501) staff       (20)       32 2024-05-21 10:29:05.000000 sklearntools-0.1.0/sklearntools.egg-info/requires.txt
--rw-r--r--   0 summy      (501) staff       (20)       13 2024-05-21 10:29:05.000000 sklearntools-0.1.0/sklearntools.egg-info/top_level.txt
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-21 10:29:57.751247 sklearntools-0.2.0/
+-rw-r--r--   0 summy      (501) staff       (20)     1061 2024-05-21 10:29:57.750534 sklearntools-0.2.0/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      761 2024-05-21 10:29:01.000000 sklearntools-0.2.0/README.rst
+-rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-21 10:29:57.751534 sklearntools-0.2.0/setup.cfg
+-rw-r--r--   0 summy      (501) staff       (20)      882 2024-05-21 10:29:53.000000 sklearntools-0.2.0/setup.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-21 10:29:57.744905 sklearntools-0.2.0/sklearntools/
+-rw-r--r--   0 summy      (501) staff       (20)     4883 2024-05-21 10:27:59.000000 sklearntools-0.2.0/sklearntools/__init__.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-21 10:29:57.749514 sklearntools-0.2.0/sklearntools.egg-info/
+-rw-r--r--   0 summy      (501) staff       (20)     1061 2024-05-21 10:29:57.000000 sklearntools-0.2.0/sklearntools.egg-info/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      258 2024-05-21 10:29:57.000000 sklearntools-0.2.0/sklearntools.egg-info/SOURCES.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-21 10:29:57.000000 sklearntools-0.2.0/sklearntools.egg-info/dependency_links.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-21 10:29:05.000000 sklearntools-0.2.0/sklearntools.egg-info/not-zip-safe
+-rw-r--r--   0 summy      (501) staff       (20)       32 2024-05-21 10:29:57.000000 sklearntools-0.2.0/sklearntools.egg-info/requires.txt
+-rw-r--r--   0 summy      (501) staff       (20)       13 2024-05-21 10:29:57.000000 sklearntools-0.2.0/sklearntools.egg-info/top_level.txt
```

### Comparing `sklearntools-0.1.0/PKG-INFO` & `sklearntools-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: sklearntools
-Version: 0.1.0
-Summary: Utils of sklearn.
+Version: 0.2.0
+Summary: Tools of sklearn.
 Home-page: https://gitee.com/summry/sklearntools
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sklearn
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `sklearntools-0.1.0/README.rst` & `sklearntools-0.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `sklearntools-0.1.0/setup.py` & `sklearntools-0.2.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 
 
 long_description = read("README.rst")
 
 setup(
     name='sklearntools',
     packages=['sklearntools'],
-    description="Utils of sklearn.",
+    description="Tools of sklearn.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='0.1.0',
+    version='0.2.0',
     install_requires=[
         'joblib>=1.1.0',
         'scikit-learn>=1.0',
     ],
     url='https://gitee.com/summry/sklearntools',
     author='summy',
     author_email='xiazhongbiao@126.com',
```

### Comparing `sklearntools-0.1.0/sklearntools/__init__.py` & `sklearntools-0.2.0/sklearntools/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearntools-0.1.0/sklearntools.egg-info/PKG-INFO` & `sklearntools-0.2.0/sklearntools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: sklearntools
-Version: 0.1.0
-Summary: Utils of sklearn.
+Version: 0.2.0
+Summary: Tools of sklearn.
 Home-page: https://gitee.com/summry/sklearntools
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sklearn
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

