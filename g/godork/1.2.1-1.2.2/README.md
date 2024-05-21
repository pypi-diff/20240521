# Comparing `tmp/godork-1.2.1.tar.gz` & `tmp/godork-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "godork-1.2.1.tar", last modified: Mon May 20 15:30:12 2024, max compression
+gzip compressed data, was "godork-1.2.2.tar", last modified: Mon May 20 15:43:40 2024, max compression
```

## Comparing `godork-1.2.1.tar` & `godork-1.2.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 thd3r     (1000) thd3r     (1000)        0 2024-05-20 15:30:12.946059 godork-1.2.1/
--rw-rw-r--   0 thd3r     (1000) thd3r     (1000)     1069 2024-05-20 15:25:46.000000 godork-1.2.1/LICENSE
--rw-r--r--   0 thd3r     (1000) thd3r     (1000)     3230 2024-05-20 15:30:12.946059 godork-1.2.1/PKG-INFO
--rw-rw-r--   0 thd3r     (1000) thd3r     (1000)     2822 2024-05-20 15:26:41.000000 godork-1.2.1/README.md
-drwxrwxr-x   0 thd3r     (1000) thd3r     (1000)        0 2024-05-20 15:30:12.946059 godork-1.2.1/godork.egg-info/
--rw-r--r--   0 thd3r     (1000) thd3r     (1000)     3230 2024-05-20 15:30:12.000000 godork-1.2.1/godork.egg-info/PKG-INFO
--rw-rw-r--   0 thd3r     (1000) thd3r     (1000)      238 2024-05-20 15:30:12.000000 godork-1.2.1/godork.egg-info/SOURCES.txt
--rw-rw-r--   0 thd3r     (1000) thd3r     (1000)        1 2024-05-20 15:30:12.000000 godork-1.2.1/godork.egg-info/dependency_links.txt
--rw-rw-r--   0 thd3r     (1000) thd3r     (1000)       43 2024-05-20 15:30:12.000000 godork-1.2.1/godork.egg-info/entry_points.txt
--rw-rw-r--   0 thd3r     (1000) thd3r     (1000)       29 2024-05-20 15:30:12.000000 godork-1.2.1/godork.egg-info/requires.txt
--rw-rw-r--   0 thd3r     (1000) thd3r     (1000)        4 2024-05-20 15:30:12.000000 godork-1.2.1/godork.egg-info/top_level.txt
--rw-rw-r--   0 thd3r     (1000) thd3r     (1000)       38 2024-05-20 15:30:12.946059 godork-1.2.1/setup.cfg
--rw-rw-r--   0 thd3r     (1000) thd3r     (1000)      717 2024-05-20 15:25:46.000000 godork-1.2.1/setup.py
-drwxrwxr-x   0 thd3r     (1000) thd3r     (1000)        0 2024-05-20 15:30:12.946059 godork-1.2.1/src/
--rw-rw-r--   0 thd3r     (1000) thd3r     (1000)       27 2024-05-20 15:25:46.000000 godork-1.2.1/src/__init__.py
--rw-rw-r--   0 thd3r     (1000) thd3r     (1000)     6710 2024-05-20 15:26:17.000000 godork-1.2.1/src/godork.py
+drwxrwxr-x   0 thd3r     (1000) thd3r     (1000)        0 2024-05-20 15:43:40.740974 godork-1.2.2/
+-rw-rw-r--   0 thd3r     (1000) thd3r     (1000)     1069 2024-05-20 15:42:13.000000 godork-1.2.2/LICENSE
+-rw-r--r--   0 thd3r     (1000) thd3r     (1000)     3287 2024-05-20 15:43:40.740974 godork-1.2.2/PKG-INFO
+-rw-rw-r--   0 thd3r     (1000) thd3r     (1000)     2879 2024-05-20 15:42:13.000000 godork-1.2.2/README.md
+drwxrwxr-x   0 thd3r     (1000) thd3r     (1000)        0 2024-05-20 15:43:40.740974 godork-1.2.2/godork.egg-info/
+-rw-r--r--   0 thd3r     (1000) thd3r     (1000)     3287 2024-05-20 15:43:40.000000 godork-1.2.2/godork.egg-info/PKG-INFO
+-rw-rw-r--   0 thd3r     (1000) thd3r     (1000)      238 2024-05-20 15:43:40.000000 godork-1.2.2/godork.egg-info/SOURCES.txt
+-rw-rw-r--   0 thd3r     (1000) thd3r     (1000)        1 2024-05-20 15:43:40.000000 godork-1.2.2/godork.egg-info/dependency_links.txt
+-rw-rw-r--   0 thd3r     (1000) thd3r     (1000)       43 2024-05-20 15:43:40.000000 godork-1.2.2/godork.egg-info/entry_points.txt
+-rw-rw-r--   0 thd3r     (1000) thd3r     (1000)       29 2024-05-20 15:43:40.000000 godork-1.2.2/godork.egg-info/requires.txt
+-rw-rw-r--   0 thd3r     (1000) thd3r     (1000)        4 2024-05-20 15:43:40.000000 godork-1.2.2/godork.egg-info/top_level.txt
+-rw-rw-r--   0 thd3r     (1000) thd3r     (1000)       38 2024-05-20 15:43:40.740974 godork-1.2.2/setup.cfg
+-rw-rw-r--   0 thd3r     (1000) thd3r     (1000)      717 2024-05-20 15:42:13.000000 godork-1.2.2/setup.py
+drwxrwxr-x   0 thd3r     (1000) thd3r     (1000)        0 2024-05-20 15:43:40.740974 godork-1.2.2/src/
+-rw-rw-r--   0 thd3r     (1000) thd3r     (1000)       27 2024-05-20 15:42:13.000000 godork-1.2.2/src/__init__.py
+-rw-rw-r--   0 thd3r     (1000) thd3r     (1000)     6710 2024-05-20 15:42:13.000000 godork-1.2.2/src/godork.py
```

### Comparing `godork-1.2.1/LICENSE` & `godork-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `godork-1.2.1/PKG-INFO` & `godork-1.2.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: godork
-Version: 1.2.1
+Version: 1.2.2
 Summary: Scrape Google search quickly
 Home-page: https://github.com/thd3r/godork
 Author: Thunder (@thd3r)
 Author-email: thd3r@proton.me
 License: MIT
 Keywords: godork,google dorks,google dork,google dorking
 Description-Content-Type: text/markdown
@@ -15,24 +15,24 @@
 Requires-Dist: bs4
 
 <h1 align="center">
   Godork - Scrape Google search quickly
 </h1>
 
 <div align="center">
-  <img src="assets/images/godork-logo.png" alt="godork" width="300px">
+  <img src="https://raw.githubusercontent.com/thd3r/godork/master/assets/images/godork-logo.png" alt="godork" width="300px">
 </div>
 
 <div align="center">
   <a href="https://python.org"><img src="https://img.shields.io/badge/Built%20with-Python-Blue"></a>
   <a href="https://opensource.org/licenses/MIT"><img src="https://img.shields.io/badge/license-MIT-_red.svg"></a>
   <a href="https://github.com/thd3r/godork/releases"><img src="https://img.shields.io/github/release/thd3r/godork.svg"></a>
   <a href="https://pypi.python.org/pypi/godork/"><img src="https://img.shields.io/pypi/v/godork.svg"></a>
   <a href="https://github.com/thd3r/godork/issues?q=is%3Aissue+is%3Aclosed"><img src="https://img.shields.io/github/issues-closed-raw/thd3r/godork?color=dark-green&label=issues%20fixed"></a>
-  <a href="https://github.com/thd3r/godork/tree/dev?tab=readme-ov-file#contributing"><img src="https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat"></a>
+  <a href="https://github.com/thd3r/godork/tree/master?tab=readme-ov-file#contributing"><img src="https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat"></a>
 </div>
 
 # About
 
 **godork** can scrape results from google searches quickly by using the [asyncio](https://docs.python.org/3/library/asyncio.html) library which uses **cooperative multitasking** in combination with [aiohttp](https://docs.aiohttp.org) and with this tool you can extract links including their titles. This tool is also able to bypass prohibitions made by providers
 
 # Installation
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: godork Version: 1.2.1 Summary: Scrape Google search
+Metadata-Version: 2.1 Name: godork Version: 1.2.2 Summary: Scrape Google search
 quickly Home-page: https://github.com/thd3r/godork Author: Thunder (@thd3r)
 Author-email: thd3r@proton.me License: MIT Keywords: godork,google dorks,google
 dork,google dorking Description-Content-Type: text/markdown License-File:
 LICENSE Requires-Dist: aiohttp Requires-Dist: asyncio Requires-Dist: requests
 Requires-Dist: bs4
               ************ GGooddoorrkk -- SSccrraappee GGooooggllee sseeaarrcchh qquuiicckkllyy ************
                                    [godork]
```

### Comparing `godork-1.2.1/README.md` & `godork-1.2.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 <h1 align="center">
   Godork - Scrape Google search quickly
 </h1>
 
 <div align="center">
-  <img src="assets/images/godork-logo.png" alt="godork" width="300px">
+  <img src="https://raw.githubusercontent.com/thd3r/godork/master/assets/images/godork-logo.png" alt="godork" width="300px">
 </div>
 
 <div align="center">
   <a href="https://python.org"><img src="https://img.shields.io/badge/Built%20with-Python-Blue"></a>
   <a href="https://opensource.org/licenses/MIT"><img src="https://img.shields.io/badge/license-MIT-_red.svg"></a>
   <a href="https://github.com/thd3r/godork/releases"><img src="https://img.shields.io/github/release/thd3r/godork.svg"></a>
   <a href="https://pypi.python.org/pypi/godork/"><img src="https://img.shields.io/pypi/v/godork.svg"></a>
   <a href="https://github.com/thd3r/godork/issues?q=is%3Aissue+is%3Aclosed"><img src="https://img.shields.io/github/issues-closed-raw/thd3r/godork?color=dark-green&label=issues%20fixed"></a>
-  <a href="https://github.com/thd3r/godork/tree/dev?tab=readme-ov-file#contributing"><img src="https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat"></a>
+  <a href="https://github.com/thd3r/godork/tree/master?tab=readme-ov-file#contributing"><img src="https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat"></a>
 </div>
 
 # About
 
 **godork** can scrape results from google searches quickly by using the [asyncio](https://docs.python.org/3/library/asyncio.html) library which uses **cooperative multitasking** in combination with [aiohttp](https://docs.aiohttp.org) and with this tool you can extract links including their titles. This tool is also able to bypass prohibitions made by providers
 
 # Installation
```

### Comparing `godork-1.2.1/godork.egg-info/PKG-INFO` & `godork-1.2.2/godork.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: godork
-Version: 1.2.1
+Version: 1.2.2
 Summary: Scrape Google search quickly
 Home-page: https://github.com/thd3r/godork
 Author: Thunder (@thd3r)
 Author-email: thd3r@proton.me
 License: MIT
 Keywords: godork,google dorks,google dork,google dorking
 Description-Content-Type: text/markdown
@@ -15,24 +15,24 @@
 Requires-Dist: bs4
 
 <h1 align="center">
   Godork - Scrape Google search quickly
 </h1>
 
 <div align="center">
-  <img src="assets/images/godork-logo.png" alt="godork" width="300px">
+  <img src="https://raw.githubusercontent.com/thd3r/godork/master/assets/images/godork-logo.png" alt="godork" width="300px">
 </div>
 
 <div align="center">
   <a href="https://python.org"><img src="https://img.shields.io/badge/Built%20with-Python-Blue"></a>
   <a href="https://opensource.org/licenses/MIT"><img src="https://img.shields.io/badge/license-MIT-_red.svg"></a>
   <a href="https://github.com/thd3r/godork/releases"><img src="https://img.shields.io/github/release/thd3r/godork.svg"></a>
   <a href="https://pypi.python.org/pypi/godork/"><img src="https://img.shields.io/pypi/v/godork.svg"></a>
   <a href="https://github.com/thd3r/godork/issues?q=is%3Aissue+is%3Aclosed"><img src="https://img.shields.io/github/issues-closed-raw/thd3r/godork?color=dark-green&label=issues%20fixed"></a>
-  <a href="https://github.com/thd3r/godork/tree/dev?tab=readme-ov-file#contributing"><img src="https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat"></a>
+  <a href="https://github.com/thd3r/godork/tree/master?tab=readme-ov-file#contributing"><img src="https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat"></a>
 </div>
 
 # About
 
 **godork** can scrape results from google searches quickly by using the [asyncio](https://docs.python.org/3/library/asyncio.html) library which uses **cooperative multitasking** in combination with [aiohttp](https://docs.aiohttp.org) and with this tool you can extract links including their titles. This tool is also able to bypass prohibitions made by providers
 
 # Installation
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: godork Version: 1.2.1 Summary: Scrape Google search
+Metadata-Version: 2.1 Name: godork Version: 1.2.2 Summary: Scrape Google search
 quickly Home-page: https://github.com/thd3r/godork Author: Thunder (@thd3r)
 Author-email: thd3r@proton.me License: MIT Keywords: godork,google dorks,google
 dork,google dorking Description-Content-Type: text/markdown License-File:
 LICENSE Requires-Dist: aiohttp Requires-Dist: asyncio Requires-Dist: requests
 Requires-Dist: bs4
               ************ GGooddoorrkk -- SSccrraappee GGooooggllee sseeaarrcchh qquuiicckkllyy ************
                                    [godork]
```

### Comparing `godork-1.2.1/setup.py` & `godork-1.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `godork-1.2.1/src/godork.py` & `godork-1.2.2/src/godork.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 import asyncio # v3.4.3
 import random
 import time
 import json
 import os
 
-__version__ = "1.2.1"
+__version__ = "1.2.2"
 
 class OptionsArgs(object):
     
     def __init__(self):
         self.parser = ArgumentParser(
             prog="godork",
             add_help=False,
```

