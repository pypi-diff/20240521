# Comparing `tmp/backports.shutil_copytree-0.0.0.2.tar.gz` & `tmp/backports.shutil_copytree-0.0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/backports.shutil_copytree-0.0.0.2.tar", last modified: Tue May 24 05:26:25 2022, max compression
+gzip compressed data, was "dist/backports.shutil_copytree-0.0.1.0.tar", last modified: Tue May 21 02:29:57 2024, max compression
```

## Comparing `backports.shutil_copytree-0.0.0.2.tar` & `backports.shutil_copytree-0.0.1.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 mujin     (1000) mujin     (1000)        0 2022-05-24 05:26:25.000000 backports.shutil_copytree-0.0.0.2/
--rw-r--r--   0 mujin     (1000) mujin     (1000)       38 2022-05-24 05:26:25.000000 backports.shutil_copytree-0.0.0.2/setup.cfg
-drwxr-xr-x   0 mujin     (1000) mujin     (1000)        0 2022-05-24 05:26:25.000000 backports.shutil_copytree-0.0.0.2/backports.shutil_copytree.egg-info/
--rw-r--r--   0 mujin     (1000) mujin     (1000)        1 2022-05-24 05:23:40.000000 backports.shutil_copytree-0.0.0.2/backports.shutil_copytree.egg-info/not-zip-safe
--rw-r--r--   0 mujin     (1000) mujin     (1000)        1 2022-05-24 05:26:25.000000 backports.shutil_copytree-0.0.0.2/backports.shutil_copytree.egg-info/dependency_links.txt
--rw-r--r--   0 mujin     (1000) mujin     (1000)       10 2022-05-24 05:26:25.000000 backports.shutil_copytree-0.0.0.2/backports.shutil_copytree.egg-info/top_level.txt
--rw-r--r--   0 mujin     (1000) mujin     (1000)      102 2022-05-24 05:26:25.000000 backports.shutil_copytree-0.0.0.2/backports.shutil_copytree.egg-info/requires.txt
--rw-r--r--   0 mujin     (1000) mujin     (1000)     1755 2022-05-24 05:26:25.000000 backports.shutil_copytree-0.0.0.2/backports.shutil_copytree.egg-info/PKG-INFO
--rw-r--r--   0 mujin     (1000) mujin     (1000)      361 2022-05-24 05:26:25.000000 backports.shutil_copytree-0.0.0.2/backports.shutil_copytree.egg-info/SOURCES.txt
--rw-r--r--   0 mujin     (1000) mujin     (1000)      497 2022-05-24 05:07:36.000000 backports.shutil_copytree-0.0.0.2/README.md
-drwxr-xr-x   0 mujin     (1000) mujin     (1000)        0 2022-05-24 05:26:25.000000 backports.shutil_copytree-0.0.0.2/backports/
--rw-r--r--   0 mujin     (1000) mujin     (1000)     4654 2022-05-24 05:25:54.000000 backports.shutil_copytree-0.0.0.2/backports/shutil_copytree.py
--rw-r--r--   0 mujin     (1000) mujin     (1000)        0 2021-11-26 06:21:01.000000 backports.shutil_copytree-0.0.0.2/backports/__init__.py
--rw-r--r--   0 mujin     (1000) mujin     (1000)     1755 2022-05-24 05:26:25.000000 backports.shutil_copytree-0.0.0.2/PKG-INFO
--rw-r--r--   0 mujin     (1000) mujin     (1000)     1451 2022-05-24 05:26:13.000000 backports.shutil_copytree-0.0.0.2/setup.py
+drwxr-xr-x   0 mujin     (1000) mujin     (1000)        0 2024-05-21 02:29:57.000000 backports.shutil_copytree-0.0.1.0/
+-rw-r--r--   0 mujin     (1000) mujin     (1000)       38 2024-05-21 02:29:57.000000 backports.shutil_copytree-0.0.1.0/setup.cfg
+drwxr-xr-x   0 mujin     (1000) mujin     (1000)        0 2024-05-21 02:29:57.000000 backports.shutil_copytree-0.0.1.0/backports.shutil_copytree.egg-info/
+-rw-r--r--   0 mujin     (1000) mujin     (1000)        1 2024-05-21 02:29:57.000000 backports.shutil_copytree-0.0.1.0/backports.shutil_copytree.egg-info/not-zip-safe
+-rw-r--r--   0 mujin     (1000) mujin     (1000)        1 2024-05-21 02:29:57.000000 backports.shutil_copytree-0.0.1.0/backports.shutil_copytree.egg-info/dependency_links.txt
+-rw-r--r--   0 mujin     (1000) mujin     (1000)       10 2024-05-21 02:29:57.000000 backports.shutil_copytree-0.0.1.0/backports.shutil_copytree.egg-info/top_level.txt
+-rw-r--r--   0 mujin     (1000) mujin     (1000)      102 2024-05-21 02:29:57.000000 backports.shutil_copytree-0.0.1.0/backports.shutil_copytree.egg-info/requires.txt
+-rw-r--r--   0 mujin     (1000) mujin     (1000)     1755 2024-05-21 02:29:57.000000 backports.shutil_copytree-0.0.1.0/backports.shutil_copytree.egg-info/PKG-INFO
+-rw-r--r--   0 mujin     (1000) mujin     (1000)      369 2024-05-21 02:29:57.000000 backports.shutil_copytree-0.0.1.0/backports.shutil_copytree.egg-info/SOURCES.txt
+-rw-r--r--   0 mujin     (1000) mujin     (1000)      497 2024-05-21 02:28:09.000000 backports.shutil_copytree-0.0.1.0/README.md
+drwxr-xr-x   0 mujin     (1000) mujin     (1000)        0 2024-05-21 02:29:57.000000 backports.shutil_copytree-0.0.1.0/backports/
+-rw-r--r--   0 mujin     (1000) mujin     (1000)     4654 2024-05-21 02:28:09.000000 backports.shutil_copytree-0.0.1.0/backports/shutil_copytree.py
+-rw-r--r--   0 mujin     (1000) mujin     (1000)      121 2024-05-21 02:28:31.000000 backports.shutil_copytree-0.0.1.0/backports/__init__.py
+-rw-r--r--   0 mujin     (1000) mujin     (1000)     2478 2024-05-21 02:28:09.000000 backports.shutil_copytree-0.0.1.0/LICENSE
+-rw-r--r--   0 mujin     (1000) mujin     (1000)     1755 2024-05-21 02:29:57.000000 backports.shutil_copytree-0.0.1.0/PKG-INFO
+-rw-r--r--   0 mujin     (1000) mujin     (1000)     1451 2024-05-21 02:29:36.000000 backports.shutil_copytree-0.0.1.0/setup.py
```

### Comparing `backports.shutil_copytree-0.0.0.2/backports.shutil_copytree.egg-info/PKG-INFO` & `backports.shutil_copytree-0.0.1.0/backports.shutil_copytree.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backports.shutil-copytree
-Version: 0.0.0.2
+Version: 0.0.1.0
 Summary: backports shutil copytree (mainly for Python2)
 Home-page: https://github.com/cielavenir/backports.shutil_copytree
 Author: cielavenir
 Author-email: cielartisan@gmail.com
 License: PSF
 Description: ## backports.shutil_copytree
```

### Comparing `backports.shutil_copytree-0.0.0.2/backports/shutil_copytree.py` & `backports.shutil_copytree-0.0.1.0/backports/shutil_copytree.py`

 * *Files identical despite different names*

### Comparing `backports.shutil_copytree-0.0.0.2/PKG-INFO` & `backports.shutil_copytree-0.0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backports.shutil_copytree
-Version: 0.0.0.2
+Version: 0.0.1.0
 Summary: backports shutil copytree (mainly for Python2)
 Home-page: https://github.com/cielavenir/backports.shutil_copytree
 Author: cielavenir
 Author-email: cielartisan@gmail.com
 License: PSF
 Description: ## backports.shutil_copytree
```

### Comparing `backports.shutil_copytree-0.0.0.2/setup.py` & `backports.shutil_copytree-0.0.1.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 ]
 
 setup(
     name='backports.shutil_copytree',
     description='backports shutil copytree (mainly for Python2)',
     long_description=open("README.md").read(),
     long_description_content_type='text/markdown',
-    version='0.0.0.2',
+    version='0.0.1.0',
     url='https://github.com/cielavenir/backports.shutil_copytree',
     license='PSF',
     author='cielavenir',
     author_email='cielartisan@gmail.com',
     packages=['backports'],
     zip_safe=False,
     include_package_data=True,
```

