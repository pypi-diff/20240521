# Comparing `tmp/mpbridge-1.4.0.tar.gz` & `tmp/mpbridge-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpbridge-1.4.0.tar", last modified: Sun Oct 29 13:14:12 2023, max compression
+gzip compressed data, was "mpbridge-1.4.1.tar", last modified: Tue May 21 16:31:47 2024, max compression
```

## Comparing `mpbridge-1.4.0.tar` & `mpbridge-1.4.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-29 13:14:12.726818 mpbridge-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2023-10-29 13:13:59.000000 mpbridge-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6030 2023-10-29 13:14:12.726818 mpbridge-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4208 2023-10-29 13:13:59.000000 mpbridge-1.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-29 13:14:12.726818 mpbridge-1.4.0/mpbridge/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-10-29 13:13:59.000000 mpbridge-1.4.0/mpbridge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4403 2023-10-29 13:13:59.000000 mpbridge-1.4.0/mpbridge/bridge.py
--rw-r--r--   0 runner    (1001) docker     (127)     2325 2023-10-29 13:13:59.000000 mpbridge-1.4.0/mpbridge/handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1696 2023-10-29 13:13:59.000000 mpbridge-1.4.0/mpbridge/ignore.py
--rw-r--r--   0 runner    (1001) docker     (127)     7399 2023-10-29 13:13:59.000000 mpbridge-1.4.0/mpbridge/serial_transport.py
--rw-r--r--   0 runner    (1001) docker     (127)     4783 2023-10-29 13:13:59.000000 mpbridge-1.4.0/mpbridge/shell.py
--rw-r--r--   0 runner    (1001) docker     (127)     2627 2023-10-29 13:13:59.000000 mpbridge-1.4.0/mpbridge/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-29 13:14:12.726818 mpbridge-1.4.0/mpbridge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6030 2023-10-29 13:14:12.000000 mpbridge-1.4.0/mpbridge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      370 2023-10-29 13:14:12.000000 mpbridge-1.4.0/mpbridge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-29 13:14:12.000000 mpbridge-1.4.0/mpbridge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2023-10-29 13:14:12.000000 mpbridge-1.4.0/mpbridge.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2023-10-29 13:14:12.000000 mpbridge-1.4.0/mpbridge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-10-29 13:14:12.000000 mpbridge-1.4.0/mpbridge.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      815 2023-10-29 13:13:59.000000 mpbridge-1.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-29 13:14:12.726818 mpbridge-1.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 16:31:47.634262 mpbridge-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-21 16:31:43.000000 mpbridge-1.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6030 2024-05-21 16:31:47.634262 mpbridge-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4208 2024-05-21 16:31:43.000000 mpbridge-1.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 16:31:47.630262 mpbridge-1.4.1/mpbridge/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-21 16:31:43.000000 mpbridge-1.4.1/mpbridge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4403 2024-05-21 16:31:43.000000 mpbridge-1.4.1/mpbridge/bridge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-05-21 16:31:43.000000 mpbridge-1.4.1/mpbridge/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-05-21 16:31:43.000000 mpbridge-1.4.1/mpbridge/ignore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7399 2024-05-21 16:31:43.000000 mpbridge-1.4.1/mpbridge/serial_transport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4783 2024-05-21 16:31:43.000000 mpbridge-1.4.1/mpbridge/shell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-05-21 16:31:43.000000 mpbridge-1.4.1/mpbridge/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 16:31:47.634262 mpbridge-1.4.1/mpbridge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6030 2024-05-21 16:31:47.000000 mpbridge-1.4.1/mpbridge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-21 16:31:47.000000 mpbridge-1.4.1/mpbridge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 16:31:47.000000 mpbridge-1.4.1/mpbridge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-21 16:31:47.000000 mpbridge-1.4.1/mpbridge.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-21 16:31:47.000000 mpbridge-1.4.1/mpbridge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-21 16:31:47.000000 mpbridge-1.4.1/mpbridge.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-21 16:31:43.000000 mpbridge-1.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 16:31:47.634262 mpbridge-1.4.1/setup.cfg
```

### Comparing `mpbridge-1.4.0/LICENSE` & `mpbridge-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mpbridge-1.4.0/PKG-INFO` & `mpbridge-1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpbridge
-Version: 1.4.0
+Version: 1.4.1
 Summary: File System Bridge to facilitate working with files on Micropython devices
 License: MIT License
         
         Copyright (c) 2022 Amirreza Hamzavi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -24,20 +24,20 @@
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: homepage, https://github.com/AmirHmZz/mpbridge
 Keywords: micropython,filemanager,file-manager,filesystem,sync,synchronize
 Classifier: Programming Language :: Python
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: watchdog>=2.2.0
 Requires-Dist: colorama>=0.4.0
-Requires-Dist: mpremote<=1.21.0,>=1.21.0
+Requires-Dist: mpremote<=1.22.0,>=1.21.0
 Requires-Dist: click
 
 # 📂 MPBridge ![Python Version](https://img.shields.io/badge/Python-3.7%20or%20later-blue?style=flat-square) ![PyPI Version](https://img.shields.io/pypi/v/mpbridge?label=PyPI%20Version&style=flat-square) ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/AmirHmZz/mpbridge/python-publish.yml?label=Builds&style=flat-square)
 
 CLI tool to synchronise and manage files on a [MicroPython](https://github.com/micropython/micropython)
 running device.
```

### Comparing `mpbridge-1.4.0/README.md` & `mpbridge-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `mpbridge-1.4.0/mpbridge/bridge.py` & `mpbridge-1.4.1/mpbridge/bridge.py`

 * *Files identical despite different names*

### Comparing `mpbridge-1.4.0/mpbridge/handler.py` & `mpbridge-1.4.1/mpbridge/handler.py`

 * *Files identical despite different names*

### Comparing `mpbridge-1.4.0/mpbridge/ignore.py` & `mpbridge-1.4.1/mpbridge/ignore.py`

 * *Files identical despite different names*

### Comparing `mpbridge-1.4.0/mpbridge/serial_transport.py` & `mpbridge-1.4.1/mpbridge/serial_transport.py`

 * *Files identical despite different names*

### Comparing `mpbridge-1.4.0/mpbridge/shell.py` & `mpbridge-1.4.1/mpbridge/shell.py`

 * *Files identical despite different names*

### Comparing `mpbridge-1.4.0/mpbridge/utils.py` & `mpbridge-1.4.1/mpbridge/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         return string[len(prefix):]
     return string
 
 
 def recursive_list_dir(path: str) -> tuple[dict[str, str], dict[str, str]]:
     out_dirs = {}
     out_files = {}
-    for abs_dir, dirs, files in os.walk(replace_backslashes(path)):
+    for abs_dir, dirs, files in os.walk(replace_backslashes(path), followlinks=True):
         abs_dir = replace_backslashes(abs_dir)
         rel_dir = removeprefix(abs_dir, path)
         for dir_name in dirs:
             out_dirs[f"{rel_dir}/{dir_name}"] = f"{abs_dir}/{dir_name}"
         for file_name in files:
             out_files[f"{rel_dir}/{file_name}"] = f"{abs_dir}/{file_name}"
     return out_dirs, out_files
```

### Comparing `mpbridge-1.4.0/mpbridge.egg-info/PKG-INFO` & `mpbridge-1.4.1/mpbridge.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpbridge
-Version: 1.4.0
+Version: 1.4.1
 Summary: File System Bridge to facilitate working with files on Micropython devices
 License: MIT License
         
         Copyright (c) 2022 Amirreza Hamzavi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -24,20 +24,20 @@
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: homepage, https://github.com/AmirHmZz/mpbridge
 Keywords: micropython,filemanager,file-manager,filesystem,sync,synchronize
 Classifier: Programming Language :: Python
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: watchdog>=2.2.0
 Requires-Dist: colorama>=0.4.0
-Requires-Dist: mpremote<=1.21.0,>=1.21.0
+Requires-Dist: mpremote<=1.22.0,>=1.21.0
 Requires-Dist: click
 
 # 📂 MPBridge ![Python Version](https://img.shields.io/badge/Python-3.7%20or%20later-blue?style=flat-square) ![PyPI Version](https://img.shields.io/pypi/v/mpbridge?label=PyPI%20Version&style=flat-square) ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/AmirHmZz/mpbridge/python-publish.yml?label=Builds&style=flat-square)
 
 CLI tool to synchronise and manage files on a [MicroPython](https://github.com/micropython/micropython)
 running device.
```

### Comparing `mpbridge-1.4.0/pyproject.toml` & `mpbridge-1.4.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -3,30 +3,30 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mpbridge"
-version = "1.4.0"
+version = "1.4.1"
 description = "File System Bridge to facilitate working with files on Micropython devices"
 license = { file = "LICENSE" }
 keywords = [
     "micropython",
     "filemanager",
     "file-manager",
     "filesystem",
     "sync",
     "synchronize",
 ]
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 dependencies = [
     "watchdog>=2.2.0",
     "colorama>=0.4.0",
-    "mpremote>=1.21.0, <=1.21.0",
+    "mpremote>=1.21.0, <=1.22.0",
     "click"
 ]
 classifiers = [
     "Programming Language :: Python",
     "Operating System :: OS Independent"
 ]
```

