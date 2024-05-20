# Comparing `tmp/annobee-0.5.8.tar.gz` & `tmp/annobee-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "annobee-0.5.8.tar", last modified: Wed May 15 14:40:26 2024, max compression
+gzip compressed data, was "annobee-0.5.9.tar", last modified: Mon May 20 21:58:18 2024, max compression
```

## Comparing `annobee-0.5.8.tar` & `annobee-0.5.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 kadir     (1001) kadir     (1001)        0 2024-05-15 14:40:26.465857 annobee-0.5.8/
--rw-rw-r--   0 kadir     (1001) kadir     (1001)     1074 2024-05-13 19:30:06.000000 annobee-0.5.8/LICENSE
--rw-rw-r--   0 kadir     (1001) kadir     (1001)     7350 2024-05-15 14:40:26.465857 annobee-0.5.8/PKG-INFO
--rw-rw-r--   0 kadir     (1001) kadir     (1001)     6953 2024-05-15 12:36:35.000000 annobee-0.5.8/README.md
-drwxrwxr-x   0 kadir     (1001) kadir     (1001)        0 2024-05-15 14:40:26.465857 annobee-0.5.8/annobee/
--rw-rw-r--   0 kadir     (1001) kadir     (1001)       30 2024-05-15 11:15:27.000000 annobee-0.5.8/annobee/__init__.py
--rw-rw-r--   0 kadir     (1001) kadir     (1001)     6243 2024-05-15 11:16:29.000000 annobee-0.5.8/annobee/cli.py
-drwxrwxr-x   0 kadir     (1001) kadir     (1001)        0 2024-05-15 14:40:26.465857 annobee-0.5.8/annobee.egg-info/
--rw-rw-r--   0 kadir     (1001) kadir     (1001)     7350 2024-05-15 14:40:26.000000 annobee-0.5.8/annobee.egg-info/PKG-INFO
--rw-rw-r--   0 kadir     (1001) kadir     (1001)      249 2024-05-15 14:40:26.000000 annobee-0.5.8/annobee.egg-info/SOURCES.txt
--rw-rw-r--   0 kadir     (1001) kadir     (1001)        1 2024-05-15 14:40:26.000000 annobee-0.5.8/annobee.egg-info/dependency_links.txt
--rw-rw-r--   0 kadir     (1001) kadir     (1001)       46 2024-05-15 14:40:26.000000 annobee-0.5.8/annobee.egg-info/entry_points.txt
--rw-rw-r--   0 kadir     (1001) kadir     (1001)       82 2024-05-15 14:40:26.000000 annobee-0.5.8/annobee.egg-info/requires.txt
--rw-rw-r--   0 kadir     (1001) kadir     (1001)        8 2024-05-15 14:40:26.000000 annobee-0.5.8/annobee.egg-info/top_level.txt
--rw-rw-r--   0 kadir     (1001) kadir     (1001)       38 2024-05-15 14:40:26.465857 annobee-0.5.8/setup.cfg
--rw-rw-r--   0 kadir     (1001) kadir     (1001)      937 2024-05-15 14:40:01.000000 annobee-0.5.8/setup.py
+drwxrwxr-x   0 kadir     (1001) kadir     (1001)        0 2024-05-20 21:58:18.771803 annobee-0.5.9/
+-rw-rw-r--   0 kadir     (1001) kadir     (1001)     1074 2024-05-13 19:30:06.000000 annobee-0.5.9/LICENSE
+-rw-rw-r--   0 kadir     (1001) kadir     (1001)     7350 2024-05-20 21:58:18.771803 annobee-0.5.9/PKG-INFO
+-rw-rw-r--   0 kadir     (1001) kadir     (1001)     6953 2024-05-15 12:36:35.000000 annobee-0.5.9/README.md
+drwxrwxr-x   0 kadir     (1001) kadir     (1001)        0 2024-05-20 21:58:18.767803 annobee-0.5.9/annobee/
+-rw-rw-r--   0 kadir     (1001) kadir     (1001)       30 2024-05-15 11:15:27.000000 annobee-0.5.9/annobee/__init__.py
+-rw-rw-r--   0 kadir     (1001) kadir     (1001)     2984 2024-05-20 21:54:46.000000 annobee-0.5.9/annobee/cli.py
+drwxrwxr-x   0 kadir     (1001) kadir     (1001)        0 2024-05-20 21:58:18.767803 annobee-0.5.9/annobee.egg-info/
+-rw-rw-r--   0 kadir     (1001) kadir     (1001)     7350 2024-05-20 21:58:18.000000 annobee-0.5.9/annobee.egg-info/PKG-INFO
+-rw-rw-r--   0 kadir     (1001) kadir     (1001)      249 2024-05-20 21:58:18.000000 annobee-0.5.9/annobee.egg-info/SOURCES.txt
+-rw-rw-r--   0 kadir     (1001) kadir     (1001)        1 2024-05-20 21:58:18.000000 annobee-0.5.9/annobee.egg-info/dependency_links.txt
+-rw-rw-r--   0 kadir     (1001) kadir     (1001)       46 2024-05-20 21:58:18.000000 annobee-0.5.9/annobee.egg-info/entry_points.txt
+-rw-rw-r--   0 kadir     (1001) kadir     (1001)       82 2024-05-20 21:58:18.000000 annobee-0.5.9/annobee.egg-info/requires.txt
+-rw-rw-r--   0 kadir     (1001) kadir     (1001)        8 2024-05-20 21:58:18.000000 annobee-0.5.9/annobee.egg-info/top_level.txt
+-rw-rw-r--   0 kadir     (1001) kadir     (1001)       38 2024-05-20 21:58:18.771803 annobee-0.5.9/setup.cfg
+-rw-rw-r--   0 kadir     (1001) kadir     (1001)      937 2024-05-20 21:57:22.000000 annobee-0.5.9/setup.py
```

### Comparing `annobee-0.5.8/LICENSE` & `annobee-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `annobee-0.5.8/PKG-INFO` & `annobee-0.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: annobee
-Version: 0.5.8
+Version: 0.5.9
 Summary: UNKNOWN
 Home-page: https://github.com/variantAnnotation/annobee-sdk
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `annobee-0.5.8/README.md` & `annobee-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `annobee-0.5.8/annobee.egg-info/PKG-INFO` & `annobee-0.5.9/annobee.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: annobee
-Version: 0.5.8
+Version: 0.5.9
 Summary: UNKNOWN
 Home-page: https://github.com/variantAnnotation/annobee-sdk
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `annobee-0.5.8/setup.py` & `annobee-0.5.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     description = fh.read()
 
 
 setup(
     name='annobee',
-    version='0.5.8',
+    version='0.5.9',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             'annobee=annobee.cli:main',
         ],
     },
     install_requires=[
```

