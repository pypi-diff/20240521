# Comparing `tmp/pytigon-batteries-0.240505.tar.gz` & `tmp/pytigon-batteries-0.240521.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytigon-batteries-0.240505.tar", last modified: Sun May  5 11:47:48 2024, max compression
+gzip compressed data, was "pytigon-batteries-0.240521.tar", last modified: Tue May 21 21:07:42 2024, max compression
```

## Comparing `pytigon-batteries-0.240505.tar` & `pytigon-batteries-0.240521.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2024-05-05 11:47:48.714277 pytigon-batteries-0.240505/
--rw-rw-r--   0 sch       (1000) sch       (1000)     7652 2024-05-05 11:44:41.000000 pytigon-batteries-0.240505/LICENSE
--rw-r--r--   0 sch       (1000) sch       (1000)     5530 2024-05-05 11:47:48.714277 pytigon-batteries-0.240505/PKG-INFO
--rw-rw-r--   0 sch       (1000) sch       (1000)       53 2024-05-05 11:44:41.000000 pytigon-batteries-0.240505/README.md
-drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2024-05-05 11:47:48.706277 pytigon-batteries-0.240505/pytigon_batteries.egg-info/
--rw-r--r--   0 sch       (1000) sch       (1000)     5530 2024-05-05 11:47:48.000000 pytigon-batteries-0.240505/pytigon_batteries.egg-info/PKG-INFO
--rw-rw-r--   0 sch       (1000) sch       (1000)      230 2024-05-05 11:47:48.000000 pytigon-batteries-0.240505/pytigon_batteries.egg-info/SOURCES.txt
--rw-rw-r--   0 sch       (1000) sch       (1000)        1 2024-05-05 11:47:48.000000 pytigon-batteries-0.240505/pytigon_batteries.egg-info/dependency_links.txt
--rw-rw-r--   0 sch       (1000) sch       (1000)     1180 2024-05-05 11:47:48.000000 pytigon-batteries-0.240505/pytigon_batteries.egg-info/requires.txt
--rw-rw-r--   0 sch       (1000) sch       (1000)        1 2024-05-05 11:47:48.000000 pytigon-batteries-0.240505/pytigon_batteries.egg-info/top_level.txt
--rw-rw-r--   0 sch       (1000) sch       (1000)       38 2024-05-05 11:47:48.714277 pytigon-batteries-0.240505/setup.cfg
--rw-rw-r--   0 sch       (1000) sch       (1000)     2556 2024-05-05 11:44:41.000000 pytigon-batteries-0.240505/setup.py
+drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2024-05-21 21:07:42.813528 pytigon-batteries-0.240521/
+-rw-rw-r--   0 sch       (1000) sch       (1000)     7652 2024-05-21 21:04:48.000000 pytigon-batteries-0.240521/LICENSE
+-rw-r--r--   0 sch       (1000) sch       (1000)     5530 2024-05-21 21:07:42.813528 pytigon-batteries-0.240521/PKG-INFO
+-rw-rw-r--   0 sch       (1000) sch       (1000)       53 2024-05-21 21:04:48.000000 pytigon-batteries-0.240521/README.md
+drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2024-05-21 21:07:42.805528 pytigon-batteries-0.240521/pytigon_batteries.egg-info/
+-rw-r--r--   0 sch       (1000) sch       (1000)     5530 2024-05-21 21:07:42.000000 pytigon-batteries-0.240521/pytigon_batteries.egg-info/PKG-INFO
+-rw-rw-r--   0 sch       (1000) sch       (1000)      230 2024-05-21 21:07:42.000000 pytigon-batteries-0.240521/pytigon_batteries.egg-info/SOURCES.txt
+-rw-rw-r--   0 sch       (1000) sch       (1000)        1 2024-05-21 21:07:42.000000 pytigon-batteries-0.240521/pytigon_batteries.egg-info/dependency_links.txt
+-rw-rw-r--   0 sch       (1000) sch       (1000)     1180 2024-05-21 21:07:42.000000 pytigon-batteries-0.240521/pytigon_batteries.egg-info/requires.txt
+-rw-rw-r--   0 sch       (1000) sch       (1000)        1 2024-05-21 21:07:42.000000 pytigon-batteries-0.240521/pytigon_batteries.egg-info/top_level.txt
+-rw-rw-r--   0 sch       (1000) sch       (1000)       38 2024-05-21 21:07:42.813528 pytigon-batteries-0.240521/setup.cfg
+-rw-rw-r--   0 sch       (1000) sch       (1000)     2556 2024-05-21 21:04:48.000000 pytigon-batteries-0.240521/setup.py
```

### Comparing `pytigon-batteries-0.240505/LICENSE` & `pytigon-batteries-0.240521/LICENSE`

 * *Files identical despite different names*

### Comparing `pytigon-batteries-0.240505/PKG-INFO` & `pytigon-batteries-0.240521/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytigon-batteries
-Version: 0.240505
+Version: 0.240521
 Summary: Pytigon library
 Author: Sławomir Chołaj
 Author-email: slawomir.cholaj@gmail.com
 License: LGPLv3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `pytigon-batteries-0.240505/pytigon_batteries.egg-info/PKG-INFO` & `pytigon-batteries-0.240521/pytigon_batteries.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytigon-batteries
-Version: 0.240505
+Version: 0.240521
 Summary: Pytigon library
 Author: Sławomir Chołaj
 Author-email: slawomir.cholaj@gmail.com
 License: LGPLv3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `pytigon-batteries-0.240505/pytigon_batteries.egg-info/requires.txt` & `pytigon-batteries-0.240521/pytigon_batteries.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pytigon-batteries-0.240505/setup.py` & `pytigon-batteries-0.240521/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 extras_require["all"] = (
     extras_require["server"] + extras_require["data"] + extras_require["interface"]
 )
 
 setup(
     name="pytigon-batteries",
-    version="0.240505",
+    version="0.240521",
     description="Pytigon library",
     author="Sławomir Chołaj",
     author_email="slawomir.cholaj@gmail.com",
     license="LGPLv3",
     packages=find_packages(),
     package_data={"": extra_files},
     install_requires=install_requires,
```

