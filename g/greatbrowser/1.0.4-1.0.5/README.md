# Comparing `tmp/greatbrowser-1.0.4.tar.gz` & `tmp/greatbrowser-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "greatbrowser-1.0.4.tar", last modified: Mon May 20 19:00:29 2024, max compression
+gzip compressed data, was "greatbrowser-1.0.5.tar", last modified: Tue May 21 20:06:56 2024, max compression
```

## Comparing `greatbrowser-1.0.4.tar` & `greatbrowser-1.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:00:29.728119 greatbrowser-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-20 19:00:19.000000 greatbrowser-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-05-20 19:00:29.728119 greatbrowser-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-05-20 19:00:19.000000 greatbrowser-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:00:29.728119 greatbrowser-1.0.4/greatbrowser/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-20 19:00:19.000000 greatbrowser-1.0.4/greatbrowser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17115 2024-05-20 19:00:19.000000 greatbrowser-1.0.4/greatbrowser/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    13482 2024-05-20 19:00:19.000000 greatbrowser-1.0.4/greatbrowser/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:00:29.728119 greatbrowser-1.0.4/greatbrowser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-05-20 19:00:29.000000 greatbrowser-1.0.4/greatbrowser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-20 19:00:29.000000 greatbrowser-1.0.4/greatbrowser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 19:00:29.000000 greatbrowser-1.0.4/greatbrowser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-20 19:00:29.000000 greatbrowser-1.0.4/greatbrowser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-20 19:00:29.000000 greatbrowser-1.0.4/greatbrowser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 19:00:29.728119 greatbrowser-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-20 19:00:19.000000 greatbrowser-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:06:56.988410 greatbrowser-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-21 20:06:45.000000 greatbrowser-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-05-21 20:06:56.988410 greatbrowser-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-05-21 20:06:45.000000 greatbrowser-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:06:56.988410 greatbrowser-1.0.5/greatbrowser/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-21 20:06:45.000000 greatbrowser-1.0.5/greatbrowser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17115 2024-05-21 20:06:45.000000 greatbrowser-1.0.5/greatbrowser/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13482 2024-05-21 20:06:45.000000 greatbrowser-1.0.5/greatbrowser/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:06:56.988410 greatbrowser-1.0.5/greatbrowser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-05-21 20:06:56.000000 greatbrowser-1.0.5/greatbrowser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-21 20:06:56.000000 greatbrowser-1.0.5/greatbrowser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 20:06:56.000000 greatbrowser-1.0.5/greatbrowser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-21 20:06:56.000000 greatbrowser-1.0.5/greatbrowser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-21 20:06:56.000000 greatbrowser-1.0.5/greatbrowser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 20:06:56.988410 greatbrowser-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-21 20:06:45.000000 greatbrowser-1.0.5/setup.py
```

### Comparing `greatbrowser-1.0.4/LICENSE` & `greatbrowser-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `greatbrowser-1.0.4/PKG-INFO` & `greatbrowser-1.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: greatbrowser
-Version: 1.0.4
+Version: 1.0.5
 Summary: Automate Stanford's GREAT browser
 Author: Sam Anderson
 Author-email: sanderson01@wesleyan.edu
 Project-URL: Source, https://github.com/SamAndTheSun/greatbrowser
 Project-URL: Bug Reports, https://github.com/SamAndTheSun/greatbrowser/issues
 Keywords: python,genomics,genetics,greatbrowser,great,automated,analysis
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# greatbrowser v1.0.4
+# greatbrowser v1.0.5
 A selenium implementation in python for Stanford's GREAT browser, allowing for quick and easy genomic analysis.
 
 This repository can be installed as a module
 
 ```
 pip install greatbrowser
 ```
```

### Comparing `greatbrowser-1.0.4/README.md` & `greatbrowser-1.0.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# greatbrowser v1.0.4
+# greatbrowser v1.0.5
 A selenium implementation in python for Stanford's GREAT browser, allowing for quick and easy genomic analysis.
 
 This repository can be installed as a module
 
 ```
 pip install greatbrowser
 ```
```

### Comparing `greatbrowser-1.0.4/greatbrowser/functions.py` & `greatbrowser-1.0.5/greatbrowser/functions.py`

 * *Files identical despite different names*

### Comparing `greatbrowser-1.0.4/greatbrowser/main.py` & `greatbrowser-1.0.5/greatbrowser/main.py`

 * *Files identical despite different names*

### Comparing `greatbrowser-1.0.4/greatbrowser.egg-info/PKG-INFO` & `greatbrowser-1.0.5/greatbrowser.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: greatbrowser
-Version: 1.0.4
+Version: 1.0.5
 Summary: Automate Stanford's GREAT browser
 Author: Sam Anderson
 Author-email: sanderson01@wesleyan.edu
 Project-URL: Source, https://github.com/SamAndTheSun/greatbrowser
 Project-URL: Bug Reports, https://github.com/SamAndTheSun/greatbrowser/issues
 Keywords: python,genomics,genetics,greatbrowser,great,automated,analysis
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# greatbrowser v1.0.4
+# greatbrowser v1.0.5
 A selenium implementation in python for Stanford's GREAT browser, allowing for quick and easy genomic analysis.
 
 This repository can be installed as a module
 
 ```
 pip install greatbrowser
 ```
```

### Comparing `greatbrowser-1.0.4/setup.py` & `greatbrowser-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.4'
+VERSION = '1.0.5'
 DESCRIPTION = "Automate Stanford's GREAT browser"
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
```

