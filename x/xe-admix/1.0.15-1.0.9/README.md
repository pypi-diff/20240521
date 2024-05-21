# Comparing `tmp/xe-admix-1.0.15.tar.gz` & `tmp/xe-admix-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xe-admix-1.0.15.tar", last modified: Tue May 21 14:53:58 2024, max compression
+gzip compressed data, was "xe-admix-1.0.9.tar", last modified: Sun May 21 18:04:49 2023, max compression
```

## Comparing `xe-admix-1.0.15.tar` & `xe-admix-1.0.9.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:53:58.312238 xe-admix-1.0.15/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-21 14:53:54.000000 xe-admix-1.0.15/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-05-21 14:53:54.000000 xe-admix-1.0.15/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-21 14:53:54.000000 xe-admix-1.0.15/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-21 14:53:54.000000 xe-admix-1.0.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-21 14:53:54.000000 xe-admix-1.0.15/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-05-21 14:53:58.312238 xe-admix-1.0.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-21 14:53:54.000000 xe-admix-1.0.15/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:53:58.304238 xe-admix-1.0.15/admix/
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-21 14:53:54.000000 xe-admix-1.0.15/admix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-05-21 14:53:54.000000 xe-admix-1.0.15/admix/admix.py
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-21 14:53:54.000000 xe-admix-1.0.15/admix/clients.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:53:58.308238 xe-admix-1.0.15/admix/daemons/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 14:53:54.000000 xe-admix-1.0.15/admix/daemons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-21 14:53:54.000000 xe-admix-1.0.15/admix/daemons/daemon.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-21 14:53:54.000000 xe-admix-1.0.15/admix/daemons/sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-05-21 14:53:54.000000 xe-admix-1.0.15/admix/daemons/upload.py
--rw-r--r--   0 runner    (1001) docker     (127)     7450 2024-05-21 14:53:54.000000 xe-admix-1.0.15/admix/downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)    15707 2024-05-21 14:53:54.000000 xe-admix-1.0.15/admix/fix.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:53:58.308238 xe-admix-1.0.15/admix/helper/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 14:53:54.000000 xe-admix-1.0.15/admix/helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-21 14:53:54.000000 xe-admix-1.0.15/admix/helper/decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)    10103 2024-05-21 14:53:54.000000 xe-admix-1.0.15/admix/helper/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:53:58.308238 xe-admix-1.0.15/admix/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 14:53:54.000000 xe-admix-1.0.15/admix/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22176 2024-05-21 14:53:54.000000 xe-admix-1.0.15/admix/interfaces/rucio_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    36718 2024-05-21 14:53:54.000000 xe-admix-1.0.15/admix/interfaces/rucio_summoner.py
--rw-r--r--   0 runner    (1001) docker     (127)    20523 2024-05-21 14:53:54.000000 xe-admix-1.0.15/admix/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-05-21 14:53:54.000000 xe-admix-1.0.15/admix/monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)    11892 2024-05-21 14:53:54.000000 xe-admix-1.0.15/admix/rucio.py
--rw-r--r--   0 runner    (1001) docker     (127)    12886 2024-05-21 14:53:54.000000 xe-admix-1.0.15/admix/showrun.py
--rw-r--r--   0 runner    (1001) docker     (127)     5493 2024-05-21 14:53:54.000000 xe-admix-1.0.15/admix/uploader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-21 14:53:54.000000 xe-admix-1.0.15/admix/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-05-21 14:53:54.000000 xe-admix-1.0.15/admix/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:53:58.308238 xe-admix-1.0.15/bin/
--rw-r--r--   0 runner    (1001) docker     (127)     3739 2024-05-21 14:53:54.000000 xe-admix-1.0.15/bin/admix-download
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:53:58.308238 xe-admix-1.0.15/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     6758 2024-05-21 14:53:54.000000 xe-admix-1.0.15/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-21 14:53:54.000000 xe-admix-1.0.15/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)     8661 2024-05-21 14:53:54.000000 xe-admix-1.0.15/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-21 14:53:54.000000 xe-admix-1.0.15/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-21 14:53:54.000000 xe-admix-1.0.15/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-21 14:53:54.000000 xe-admix-1.0.15/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-21 14:53:54.000000 xe-admix-1.0.15/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-05-21 14:53:54.000000 xe-admix-1.0.15/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6457 2024-05-21 14:53:54.000000 xe-admix-1.0.15/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-21 14:53:54.000000 xe-admix-1.0.15/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)    28723 2024-05-21 14:53:54.000000 xe-admix-1.0.15/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-21 14:53:54.000000 xe-admix-1.0.15/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 14:53:58.312238 xe-admix-1.0.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-21 14:53:54.000000 xe-admix-1.0.15/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:53:58.308238 xe-admix-1.0.15/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-21 14:53:54.000000 xe-admix-1.0.15/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-21 14:53:54.000000 xe-admix-1.0.15/tests/test_admix.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:53:58.312238 xe-admix-1.0.15/xe_admix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-05-21 14:53:58.000000 xe-admix-1.0.15/xe_admix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-21 14:53:58.000000 xe-admix-1.0.15/xe_admix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 14:53:58.000000 xe-admix-1.0.15/xe_admix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 14:53:58.000000 xe-admix-1.0.15/xe_admix.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-21 14:53:58.000000 xe-admix-1.0.15/xe_admix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-21 14:53:58.000000 xe-admix-1.0.15/xe_admix.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:04:49.279588 xe-admix-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-21 18:04:44.000000 xe-admix-1.0.9/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-05-21 18:04:44.000000 xe-admix-1.0.9/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-21 18:04:44.000000 xe-admix-1.0.9/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-05-21 18:04:44.000000 xe-admix-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-21 18:04:44.000000 xe-admix-1.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-05-21 18:04:49.279588 xe-admix-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-21 18:04:44.000000 xe-admix-1.0.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:04:49.275588 xe-admix-1.0.9/admix/
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-21 18:04:44.000000 xe-admix-1.0.9/admix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-21 18:04:44.000000 xe-admix-1.0.9/admix/admix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-21 18:04:44.000000 xe-admix-1.0.9/admix/clients.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:04:49.275588 xe-admix-1.0.9/admix/daemons/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 18:04:44.000000 xe-admix-1.0.9/admix/daemons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-05-21 18:04:44.000000 xe-admix-1.0.9/admix/daemons/daemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-21 18:04:44.000000 xe-admix-1.0.9/admix/daemons/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-05-21 18:04:44.000000 xe-admix-1.0.9/admix/daemons/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7036 2023-05-21 18:04:44.000000 xe-admix-1.0.9/admix/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15707 2023-05-21 18:04:44.000000 xe-admix-1.0.9/admix/fix.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:04:49.275588 xe-admix-1.0.9/admix/helper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 18:04:44.000000 xe-admix-1.0.9/admix/helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-21 18:04:44.000000 xe-admix-1.0.9/admix/helper/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10103 2023-05-21 18:04:44.000000 xe-admix-1.0.9/admix/helper/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:04:49.275588 xe-admix-1.0.9/admix/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 18:04:44.000000 xe-admix-1.0.9/admix/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22176 2023-05-21 18:04:44.000000 xe-admix-1.0.9/admix/interfaces/rucio_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36718 2023-05-21 18:04:44.000000 xe-admix-1.0.9/admix/interfaces/rucio_summoner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15506 2023-05-21 18:04:44.000000 xe-admix-1.0.9/admix/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-05-21 18:04:44.000000 xe-admix-1.0.9/admix/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11892 2023-05-21 18:04:44.000000 xe-admix-1.0.9/admix/rucio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12886 2023-05-21 18:04:44.000000 xe-admix-1.0.9/admix/showrun.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-05-21 18:04:44.000000 xe-admix-1.0.9/admix/uploader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-05-21 18:04:44.000000 xe-admix-1.0.9/admix/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-05-21 18:04:44.000000 xe-admix-1.0.9/admix/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:04:49.275588 xe-admix-1.0.9/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-05-21 18:04:44.000000 xe-admix-1.0.9/bin/admix-download
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:04:49.279588 xe-admix-1.0.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6758 2023-05-21 18:04:44.000000 xe-admix-1.0.9/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-21 18:04:44.000000 xe-admix-1.0.9/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8661 2023-05-21 18:04:44.000000 xe-admix-1.0.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-21 18:04:44.000000 xe-admix-1.0.9/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-21 18:04:44.000000 xe-admix-1.0.9/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-21 18:04:44.000000 xe-admix-1.0.9/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-21 18:04:44.000000 xe-admix-1.0.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-05-21 18:04:44.000000 xe-admix-1.0.9/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6457 2023-05-21 18:04:44.000000 xe-admix-1.0.9/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-21 18:04:44.000000 xe-admix-1.0.9/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    28723 2023-05-21 18:04:44.000000 xe-admix-1.0.9/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-21 18:04:44.000000 xe-admix-1.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 18:04:49.279588 xe-admix-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-21 18:04:44.000000 xe-admix-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:04:49.279588 xe-admix-1.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-21 18:04:44.000000 xe-admix-1.0.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-21 18:04:44.000000 xe-admix-1.0.9/tests/test_admix.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:04:49.279588 xe-admix-1.0.9/xe_admix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-05-21 18:04:49.000000 xe-admix-1.0.9/xe_admix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-21 18:04:49.000000 xe-admix-1.0.9/xe_admix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 18:04:49.000000 xe-admix-1.0.9/xe_admix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 18:04:49.000000 xe-admix-1.0.9/xe_admix.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-21 18:04:49.000000 xe-admix-1.0.9/xe_admix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-21 18:04:49.000000 xe-admix-1.0.9/xe_admix.egg-info/top_level.txt
```

### Comparing `xe-admix-1.0.15/CONTRIBUTING.rst` & `xe-admix-1.0.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `xe-admix-1.0.15/LICENSE` & `xe-admix-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `xe-admix-1.0.15/PKG-INFO` & `xe-admix-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: xe-admix
-Version: 1.0.15
+Version: 1.0.9
 Summary: advanced Data Management In Xenon (aDMIX)
 Home-page: https://github.com/XENON1T/admix
 Author: UNKNOWN
 Author-email: UNKNOWN
 License: BSD license
 Description: =====
         aDMIX
```

### Comparing `xe-admix-1.0.15/README.rst` & `xe-admix-1.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `xe-admix-1.0.15/admix/__init__.py` & `xe-admix-1.0.9/admix/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 """Top-level package for aDMIX."""
-__version__ = '1.0.15'
+__version__ = '1.0.9'
 
 import os
 import logging
 from utilix import uconfig
 
 def get_logger():
     logger = logging.getLogger("admix")
@@ -22,11 +22,10 @@
 PKGDIR = os.path.dirname(__file__)
 
 DEFAULT_CONFIG = os.path.join(PKGDIR, 'config', 'default.config')
 
 from . import utils
 from .downloader import download
 from .uploader import upload
-from .uploader import preupload
 from . import manager
 from . import monitor
 from . import validator
```

### Comparing `xe-admix-1.0.15/admix/admix.py` & `xe-admix-1.0.9/admix/admix.py`

 * *Files identical despite different names*

### Comparing `xe-admix-1.0.15/admix/clients.py` & `xe-admix-1.0.9/admix/clients.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,46 +1,40 @@
 from rucio.client.client import Client
 from rucio.client.replicaclient import ReplicaClient
 from rucio.client.accountclient import AccountClient
 from rucio.client.rseclient import RSEClient
 from rucio.client.downloadclient import DownloadClient
 from rucio.client.uploadclient import UploadClient
-from rucio.client.ruleclient import RuleClient
-from rucio.client.didclient import DIDClient
 
 from . import logger
 
 
 rucio_client = None
 replica_client = None
 account_client = None
 rse_client = None
 download_client = None
 upload_client = None
-rule_client = None
-did_client = None
+
 
 def _init_clients():
     global rucio_client
     global replica_client
     global account_client
     global rse_client
     global download_client
     global upload_client
-    global rule_client
-    global did_client
 
     rucio_client = Client()
     replica_client = ReplicaClient()
     account_client = AccountClient()
     rse_client = RSEClient()
     download_client = DownloadClient(logger=logger)
     upload_client = UploadClient()
-    rule_client = RuleClient()
-    did_client = DIDClient()
+
 
 def needs_client(func):
     def wrapped(*args, **kwargs):
         if rucio_client is None:
             _init_clients()
         return func(*args, **kwargs)
     return wrapped
```

### Comparing `xe-admix-1.0.15/admix/daemons/daemon.py` & `xe-admix-1.0.9/admix/daemons/daemon.py`

 * *Files identical despite different names*

### Comparing `xe-admix-1.0.15/admix/daemons/upload.py` & `xe-admix-1.0.9/admix/daemons/upload.py`

 * *Files identical despite different names*

### Comparing `xe-admix-1.0.15/admix/downloader.py` & `xe-admix-1.0.9/admix/downloader.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from argparse import ArgumentParser
 
 import socket
 
 import admix.rucio
 from .utils import xe1t_runs_collection
 from .rucio import list_rules, get_did_type, get_rses
-from .manager import bring_online
 from . import logger
 from . import clients
 try:
     from straxen import __version__
     straxen_version = __version__
 except ImportError:
     print("Straxen not installed in current env, so must pass straxen_version manually")
@@ -24,22 +23,22 @@
 class RucioDownloadError(Exception):
     pass
 
 
 def determine_rse(rse_list):
     # TODO put this in config or something?
 
-    preferred_host_rses = {'rcc': ['UC_DALI_USERDISK', 'UC_OSG_USERDISK', 'SDSC_USERDISK', 'SDSC_NSDF_USERDISK'],
-                           'sdsc': ['SDSC_USERDISK', 'UC_OSG_USERDISK', 'UC_DALI_USERDISK', 'SDSC_NSDF_USERDISK'],
+    preferred_host_rses = {'rcc': ['UC_DALI_USERDISK', 'UC_OSG_USERDISK', 'SDSC_USERDISK'],
+                           'sdsc': ['SDSC_USERDISK', 'UC_OSG_USERDISK', 'UC_DALI_USERDISK'],
                            'in2p3': ['CCIN2P3_USERDISK', 'NIKHEF2_USERDISK', 'CNAF_USERDISK'],
                            'nikhef': ['NIKHEF2_USERDISK', 'SURFSARA_USERDISK', 'CNAF_USERDISK'],
                            'surf': ['SURFSARA_USERDISK', 'NIKHEF2_USERDISK', 'CNAF_USERDISK'],
                           }
 
-    preferred_glidein_rses = {'US,CA':  ['UC_OSG_USERDISK', 'SDSC_USERDISK', 'UC_DALI_USERDISK', 'SDSC_NSDF_USERDISK'],
+    preferred_glidein_rses = {'US,CA':  ['UC_OSG_USERDISK', 'SDSC_USERDISK', 'UC_DALI_USERDISK'],
                               'EUROPE,NL,IT,FR,IL': ['NIKHEF2_USERDISK', 'CNAF_USERDISK', 'SURFSARA_USERDISK']
                               }
 
     hostname = socket.getfqdn()
 
     # check if we are running on a specific host that's very close to our rses
     for host, pref_rses in preferred_host_rses.items():
@@ -55,15 +54,15 @@
             country_list = country_list.split(',')
             if glidein_country in country_list:
                 for rse in pref_rses:
                     if rse in rse_list:
                         return rse
 
     # as last ditch effort, default to UC_OSG or SDSC
-    for pref_rse in ['UC_OSG_USERDISK', 'SDSC_USERDISK', 'SDSC_NSDF_USERDISK']:
+    for pref_rse in ['UC_OSG_USERDISK', 'SDSC_USERDISK']:
         if pref_rse in rse_list:
             return pref_rse
 
     # if get here, return None and let rucio figure it out
     return
 
 
@@ -75,39 +74,36 @@
                         **kwargs
                         )
         did_list.append(did_dict)
     return clients.download_client.download_dids(did_list, num_threads=num_threads)
 
 
 def download(did, chunks=None, location='.',  tries=3, metadata=True,
-             only_metadata=False, num_threads=5, rse=None, stage=None):
+             num_threads=5, rse=None):
     """Function download()
 
     """
     did_type = get_did_type(did)
 
     if did_type == 'FILE':
         # make sure we didn't pass certain args
         assert chunks is None, f"You passed the chunks argument, but the DID {did} is a FILE"
 
 
-    if only_metadata:
-        dids = [did + '-metadata.json']
+    if chunks:
+        dids = []
+        for c in chunks:
+            cdid = f"{did}-{c:06d}"
+            dids.append(cdid)
+        # also download metadata
+        if metadata:
+            dids.append(did + '-metadata.json')
     else:
-        if chunks:
-            dids = []
-            for c in chunks:
-                cdid = f"{did}-{c:06d}"
-                dids.append(cdid)
-            # also download metadata
-            if metadata:
-                dids.append(did + '-metadata.json')
-        else:
-            scope = did.split(':')[0]
-            dids = [f"{scope}:{f}" for f in admix.rucio.list_files(did)]
+        scope = did.split(':')[0]
+        dids = [f"{scope}:{f}" for f in admix.rucio.list_files(did)]
 
     path = did.replace(':', '-')
     # drop the xnt at the beginning
     path = path.replace('xnt_', '')
     if did_type == 'FILE':
         path = '-'.join(path.split('-')[:-1])
     location = os.path.join(location, path)
@@ -130,20 +126,14 @@
 
     if not rse:
         # determine which rses this did is on
         rses = get_rses(did, state='OK')
         # find closest rse
         rse = determine_rse(rses)
 
-
-    if stage:
-        logger.info(f"Staging {len(dids)} file{'s'*(len(dids)>1)} of {did} from {rse}")        
-        bring_online(did,rse)
-
-
     if chunks:
         logger.info(f"Downloading {len(dids)} file{'s'*(len(dids)>1)} of {did} from {rse}")
     else:
         logger.info(f"Downloading {did} from {rse}")
 
     _try = 1
     success = False
```

### Comparing `xe-admix-1.0.15/admix/fix.py` & `xe-admix-1.0.9/admix/fix.py`

 * *Files identical despite different names*

### Comparing `xe-admix-1.0.15/admix/helper/helper.py` & `xe-admix-1.0.9/admix/helper/helper.py`

 * *Files identical despite different names*

### Comparing `xe-admix-1.0.15/admix/interfaces/rucio_api.py` & `xe-admix-1.0.9/admix/interfaces/rucio_api.py`

 * *Files identical despite different names*

### Comparing `xe-admix-1.0.15/admix/interfaces/rucio_summoner.py` & `xe-admix-1.0.9/admix/interfaces/rucio_summoner.py`

 * *Files identical despite different names*

### Comparing `xe-admix-1.0.15/admix/manager.py` & `xe-admix-1.0.9/admix/manager.py`

 * *Files 27% similar despite different names*

```diff
@@ -6,24 +6,18 @@
 import tempfile
 
 from packaging import version
 from tqdm import tqdm
 from rucio.common.exception import DataIdentifierNotFound
 
 import admix.rucio
-from . import clients
 from . import rucio, logger
 from . import utils
 from .utils import db
 
-import gfal2
-import time
-from datetime import timezone, datetime, timedelta
-
-TAPE_RSES = ['SURFSARA_USERDISK','CNAF_TAPE3_USERDISK','CNAF_TAPE2_USERDISK','CNAF_TAPE_USERDISK','CCIN2P3_USERDISK']
 
 def has_metadata(did):
     scope, dset = did.split(':')
     files = rucio.list_files(did)
     metadata_file = f"{dset}-metadata.json"
     return metadata_file in files
 
@@ -399,87 +393,7 @@
         _, tmpfile = tempfile.mkstemp(suffix='.txt', dir="./")
         with open(tmpfile, 'w') as f:
             for dataset in to_delete:
                 f.write(f"{os.path.join(path, dataset)}\n")
         print(f"Files that we can delete written to {tmpfile}")
 
 
-def bring_online(did,rse,timeout=3600):
-
-    """Stages data belonging to a given did from a given rse. 
-
-    :param did: DID to stage
-    :param rse: from which RSE data have to be stages
-    :param timeout: optionally you can change the maximum time after which the function gives up waiting for full data staging
-    :return: True if successfull or if staging is not needed, False in case of error or timeout
-    """
-
-    print("Bringing online {0} from {1}".format(did,rse))
-    if timeout>600:
-        print("** Warning! ** This function could take some time (within a timeout equal to {0} seconds). Consider running your program in a screen session".format(timeout))
-
-    if rse not in TAPE_RSES:
-        print("{0} is not a tape-based RSE. Staging is not required".format(rse))
-        return(True)
-
-    scope = did.split(':')[0]
-    dataset = did.split(':')[1]
-
-    file_replicas = clients.replica_client.list_replicas([{'scope':scope,'name': dataset}],rse_expression=rse)
-#    file_replicas = rucio.list_file_replicas(did,rse=rse)
-    files = [list(replica['pfns'].keys())[0] for replica in file_replicas]
-#    files = rucio.list_file_replicas(did,rse=rse)
-
-    print("Bringing online {0} files".format(len(files)))
-
-    if rse=="SURFSARA_USERDISK":
-        for i, file in enumerate(files):
-            files[i] = files[i].replace("gsiftp","srm")
-            files[i] = files[i].replace("gridftp","srm")
-            files[i] = files[i].replace("2811","8443")
-    if rse=="CCIN2P3_USERDISK":
-        for i, file in enumerate(files):
-            files[i] = files[i].replace("gsiftp","srm")
-            files[i] = files[i].replace("ccdcacli392.in2p3.fr","ccsrm02.in2p3.fr")
-            files[i] = files[i].replace("2811","8443")
-
-    #print(files)                                                                                                                                                                                                                       
-    ctx = gfal2.creat_context()
-
-    try:
-        # bring_online(surls, pintime, timeout, async)                                                                                                                                                                                  
-        # Parameters:                                                                                                                                                                                                                   
-        #   surls is the given [srmlist] argument                                                                                                                                                                                       
-        #   pintime in seconds (how long should the file stay PINNED), e.g. value 1209600 will pin files for two weeks                                                                                                                  
-        #   timeout of request in seconds, e.g. value 604800 will timeout the requests after a week                                                                                                                                     
-        #   async is asynchronous request (does not block if != 0)                                                                                                                                                                      
-        pintime = 3600*48
-        timeout_request = 3600
-        (status, token) = ctx.bring_online(files, pintime, timeout_request, True)
-        if token:
-            print(("Got token %s" % token))
-        else:
-            print("No token was returned. Are all files online?")
-    except gfal2.GError as e:
-        print("Could not bring the files online:")
-        print(("\t", e.message))
-        print(("\t Code", e.code))
-
-    print("Waiting until they are all online... (this might take time)")
-    start_time = datetime.now().replace(tzinfo=timezone.utc)
-    while True:
-        errors = ctx.bring_online_poll(files, token)
-        ncompleted = 0
-        for surl, error in zip(files, errors):
-            if not error:
-                ncompleted += 1
-        print("So far {0} files have been staged".format(ncompleted))
-        if ncompleted == len(files):
-            print("Staging of {0} files successfully completed".format(ncompleted))
-            return(True)
-        now_time = datetime.now().replace(tzinfo=timezone.utc)
-        delta_time = now_time - start_time
-        if delta_time > timedelta(seconds = timeout):
-            print("Timeout reached. Stopping waiting for full data staging")
-            print("** Warning ** Staging is not yet completed. If you plan to access data now, performances might be degraded")
-            return(False)
-        time.sleep(60)
```

### Comparing `xe-admix-1.0.15/admix/monitor.py` & `xe-admix-1.0.9/admix/monitor.py`

 * *Files identical despite different names*

### Comparing `xe-admix-1.0.15/admix/rucio.py` & `xe-admix-1.0.9/admix/rucio.py`

 * *Files identical despite different names*

### Comparing `xe-admix-1.0.15/admix/showrun.py` & `xe-admix-1.0.9/admix/showrun.py`

 * *Files identical despite different names*

### Comparing `xe-admix-1.0.15/admix/utils.py` & `xe-admix-1.0.9/admix/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,9 +62,7 @@
     return f"{scope}:{container_name}"
 
 
 def parse_dirname(dirname):
     number, dtype, lineage_hash = dirname.split('-')
     number = int(number)
     return number, dtype, lineage_hash
-
-
```

### Comparing `xe-admix-1.0.15/admix/validator.py` & `xe-admix-1.0.9/admix/validator.py`

 * *Files identical despite different names*

### Comparing `xe-admix-1.0.15/bin/admix-download` & `xe-admix-1.0.9/bin/admix-download`

 * *Files 9% similar despite different names*

```diff
@@ -23,68 +23,59 @@
 
 def main():
     parser = ArgumentParser("admix-download")
 
     parser.add_argument("number", type=int, help="Run number to download")
     parser.add_argument("dtype", help="Data type to download")
     parser.add_argument("--chunks", nargs="*", help="Space-separated list of chunks to download.")
-    parser.add_argument("--metadata", help="Whether only download metadata", action="store_true")
     parser.add_argument("--dir", help="Path to put the downloaded data.", default='.')
     parser.add_argument('--tries', type=int, help="Number of tries to download the data.", default=3)
     parser.add_argument('--rse', help='RSE to download from')
     parser.add_argument('--threads', help='Number of threads to use', default=3, type=int)
     parser.add_argument('--context', help='strax context you need -- this determines the hash',
                          default='xenonnt_online')
     parser.add_argument('--straxen_version', help='straxen version', default=None)
     parser.add_argument('--experiment', help="xent or xe1t", choices=['xe1t', 'xent'], default='xent')
-    parser.add_argument('--hash', help='force to use specific strax hash', default=None)
-    parser.add_argument("--stage", help="Stage data before downloading (useful for tape-based RSEs)", action="store_true")
 
     args = parser.parse_args()
 
     if args.experiment == 'xent':
-        if args.hash is None:
-            # if a particular straxen version is passed, use that
-            if args.straxen_version:
-                utilix_db = utilix.DB()
-                hash = utilix_db.get_hash(args.context, args.dtype, args.straxen_version)
-            # otherwise try to use system
-            else:
-                system_context = None
-                # if we have cutax, try to get context from there
-                err_msg = f"Could not find a useable context called {args.context} in cutax nor straxen"
-                if HAVE_CUTAX:
-                    try:
-                        system_context = getattr(cutax, args.context)()
-                    except:
-                        try:
-                            system_context = getattr(straxen, args.context)()
-                        except:
-                            raise RuntimeError(err_msg)
-                else:
+        # if a particular straxen version is passed, use that
+        if args.straxen_version:
+            utilix_db = utilix.DB()
+            hash = utilix_db.get_hash(args.context, args.dtype, args.straxen_version)
+        # otherwise try to use system
+        else:
+            system_context = None
+            # if we have cutax, try to get context from there
+            err_msg = f"Could not find a useable context called {args.context} in cutax nor straxen"
+            if HAVE_CUTAX:
+                try:
+                    system_context = getattr(cutax, args.context)()
+                except:
                     try:
                         system_context = getattr(straxen, args.context)()
                     except:
                         raise RuntimeError(err_msg)
-                hash = system_context.provided_dtypes()[args.dtype]['hash']
-        else:
-            hash = args.hash
+            else:
+                try:
+                    system_context = getattr(straxen, args.context)()
+                except:
+                    raise RuntimeError(err_msg)
+            hash = system_context.provided_dtypes()[args.dtype]['hash']
 
         if args.chunks:
             chunks = [int(c) for c in args.chunks]
         else:
             chunks = None
 
         did = make_did(args.number, args.dtype, hash)
 
-        downloaded = download(
-            did, chunks=chunks, location=args.dir, tries=args.tries,
-            only_metadata=args.metadata, rse=args.rse, num_threads=args.threads,
-            stage = args.stage,
-        )
+        downloaded = download(did, chunks=chunks, location=args.dir, tries=args.tries,
+                              rse=args.rse, num_threads=args.threads)
 
         print(f"Download of {len(downloaded)} files finished.")
 
     elif args.experiment == 'xe1t':
         download_1t(args.number, args.dtype, location=args.dir, tries=args.tries, rse=args.rse,
                     num_threads=args.threads)
```

### Comparing `xe-admix-1.0.15/docs/Makefile` & `xe-admix-1.0.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `xe-admix-1.0.15/docs/conf.py` & `xe-admix-1.0.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `xe-admix-1.0.15/docs/configuration.rst` & `xe-admix-1.0.9/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `xe-admix-1.0.15/docs/installation.rst` & `xe-admix-1.0.9/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `xe-admix-1.0.15/docs/make.bat` & `xe-admix-1.0.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `xe-admix-1.0.15/docs/usage.rst` & `xe-admix-1.0.9/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `xe-admix-1.0.15/setup.py` & `xe-admix-1.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Get requirements from requirements.txt, stripping the version tags
 with open('requirements.txt') as f:
     requirements = [r.split('/')[-1] if r.startswith('git+') else r for r in f.read().splitlines()]
 
 
 setup(
     name='xe-admix',
-    version='1.0.15',
+    version='1.0.9',
     description="advanced Data Management In Xenon (aDMIX)",
     long_description=readme + '\n\n' + history,
     url='https://github.com/XENON1T/admix',
     install_requires=requirements,
     scripts=['bin/admix-download'],
     packages=find_packages(),
     license="BSD license",
```

### Comparing `xe-admix-1.0.15/xe_admix.egg-info/PKG-INFO` & `xe-admix-1.0.9/xe_admix.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: xe-admix
-Version: 1.0.15
+Version: 1.0.9
 Summary: advanced Data Management In Xenon (aDMIX)
 Home-page: https://github.com/XENON1T/admix
 Author: UNKNOWN
 Author-email: UNKNOWN
 License: BSD license
 Description: =====
         aDMIX
```

### Comparing `xe-admix-1.0.15/xe_admix.egg-info/SOURCES.txt` & `xe-admix-1.0.9/xe_admix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

