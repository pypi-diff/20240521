# Comparing `tmp/webchecks-0.1.1.tar.gz` & `tmp/webchecks-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webchecks-0.1.1.tar", last modified: Thu May  9 16:36:49 2024, max compression
+gzip compressed data, was "webchecks-0.1.2.tar", last modified: Tue May 21 08:43:18 2024, max compression
```

## Comparing `webchecks-0.1.1.tar` & `webchecks-0.1.2.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:36:49.127711 webchecks-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-09 16:36:37.000000 webchecks-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-09 16:36:37.000000 webchecks-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8855 2024-05-09 16:36:49.127711 webchecks-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6274 2024-05-09 16:36:37.000000 webchecks-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     8172 2024-05-09 16:36:37.000000 webchecks-0.1.1/TUTORIAL.md
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-09 16:36:37.000000 webchecks-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 16:36:49.127711 webchecks-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-09 16:36:37.000000 webchecks-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:36:49.123711 webchecks-0.1.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 16:36:37.000000 webchecks-0.1.1/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-05-09 16:36:37.000000 webchecks-0.1.1/test/test_access.py
--rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-05-09 16:36:37.000000 webchecks-0.1.1/test/test_baseprofile.py
--rw-r--r--   0 runner    (1001) docker     (127)     4244 2024-05-09 16:36:37.000000 webchecks-0.1.1/test/test_dryrun_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     4558 2024-05-09 16:36:37.000000 webchecks-0.1.1/test/test_file_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-09 16:36:37.000000 webchecks-0.1.1/test/test_globalcache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-05-09 16:36:37.000000 webchecks-0.1.1/test/test_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)    12720 2024-05-09 16:36:37.000000 webchecks-0.1.1/test/test_security.py
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-09 16:36:37.000000 webchecks-0.1.1/test/test_singleton.py
--rw-r--r--   0 runner    (1001) docker     (127)    10296 2024-05-09 16:36:37.000000 webchecks-0.1.1/test/test_url.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:36:49.123711 webchecks-0.1.1/webchecks/
--rw-r--r--   0 runner    (1001) docker     (127)    15056 2024-05-09 16:36:37.000000 webchecks-0.1.1/webchecks/Project.py
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-05-09 16:36:37.000000 webchecks-0.1.1/webchecks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:36:49.123711 webchecks-0.1.1/webchecks/access/
--rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-05-09 16:36:37.000000 webchecks-0.1.1/webchecks/access/AccessHead.py
--rw-r--r--   0 runner    (1001) docker     (127)     6601 2024-05-09 16:36:37.000000 webchecks-0.1.1/webchecks/access/Gateway.py
--rw-r--r--   0 runner    (1001) docker     (127)     9837 2024-05-09 16:36:37.000000 webchecks-0.1.1/webchecks/access/RequestJS.py
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-05-09 16:36:37.000000 webchecks-0.1.1/webchecks/access/RequestNoJS.py
--rw-r--r--   0 runner    (1001) docker     (127)     6033 2024-05-09 16:36:37.000000 webchecks-0.1.1/webchecks/access/RobotsFile.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 16:36:37.000000 webchecks-0.1.1/webchecks/access/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-05-09 16:36:37.000000 webchecks-0.1.1/webchecks/access/security.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:36:49.127711 webchecks-0.1.1/webchecks/archive/
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-05-09 16:36:37.000000 webchecks-0.1.1/webchecks/archive/AccessNode.py
--rw-r--r--   0 runner    (1001) docker     (127)     9352 2024-05-09 16:36:37.000000 webchecks-0.1.1/webchecks/archive/FileArchive.py
--rw-r--r--   0 runner    (1001) docker     (127)     5980 2024-05-09 16:36:37.000000 webchecks-0.1.1/webchecks/archive/GlobalCache.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 16:36:37.000000 webchecks-0.1.1/webchecks/archive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-09 16:36:37.000000 webchecks-0.1.1/webchecks/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:36:49.127711 webchecks-0.1.1/webchecks/monitor/
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-09 16:36:37.000000 webchecks-0.1.1/webchecks/monitor/KeywordFinder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4133 2024-05-09 16:36:37.000000 webchecks-0.1.1/webchecks/monitor/Report.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 16:36:37.000000 webchecks-0.1.1/webchecks/monitor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:36:49.127711 webchecks-0.1.1/webchecks/profiles/
--rw-r--r--   0 runner    (1001) docker     (127)    11257 2024-05-09 16:36:37.000000 webchecks-0.1.1/webchecks/profiles/BaseProfile.py
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-09 16:36:37.000000 webchecks-0.1.1/webchecks/profiles/ProfileConstants.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 16:36:37.000000 webchecks-0.1.1/webchecks/profiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-09 16:36:37.000000 webchecks-0.1.1/webchecks/profiles/profileDB.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:36:49.127711 webchecks-0.1.1/webchecks/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-09 16:36:37.000000 webchecks-0.1.1/webchecks/utils/Error.py
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-09 16:36:37.000000 webchecks-0.1.1/webchecks/utils/OptionsError.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 16:36:37.000000 webchecks-0.1.1/webchecks/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-09 16:36:37.000000 webchecks-0.1.1/webchecks/utils/check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-05-09 16:36:37.000000 webchecks-0.1.1/webchecks/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-05-09 16:36:37.000000 webchecks-0.1.1/webchecks/utils/file_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-05-09 16:36:37.000000 webchecks-0.1.1/webchecks/utils/messaging.py
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-09 16:36:37.000000 webchecks-0.1.1/webchecks/utils/singleton.py
--rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-05-09 16:36:37.000000 webchecks-0.1.1/webchecks/utils/timedqueue.py
--rw-r--r--   0 runner    (1001) docker     (127)     7090 2024-05-09 16:36:37.000000 webchecks-0.1.1/webchecks/utils/url.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:36:49.127711 webchecks-0.1.1/webchecks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8855 2024-05-09 16:36:49.000000 webchecks-0.1.1/webchecks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-05-09 16:36:49.000000 webchecks-0.1.1/webchecks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 16:36:49.000000 webchecks-0.1.1/webchecks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-09 16:36:49.000000 webchecks-0.1.1/webchecks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-09 16:36:49.000000 webchecks-0.1.1/webchecks.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:43:18.650862 webchecks-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-21 08:43:12.000000 webchecks-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-21 08:43:12.000000 webchecks-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8990 2024-05-21 08:43:18.646862 webchecks-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6409 2024-05-21 08:43:12.000000 webchecks-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8172 2024-05-21 08:43:12.000000 webchecks-0.1.2/TUTORIAL.md
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-21 08:43:12.000000 webchecks-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 08:43:18.650862 webchecks-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-21 08:43:12.000000 webchecks-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:43:18.642862 webchecks-0.1.2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:43:12.000000 webchecks-0.1.2/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-05-21 08:43:12.000000 webchecks-0.1.2/test/test_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-05-21 08:43:12.000000 webchecks-0.1.2/test/test_baseprofile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4244 2024-05-21 08:43:12.000000 webchecks-0.1.2/test/test_dryrun_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4558 2024-05-21 08:43:12.000000 webchecks-0.1.2/test/test_file_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-21 08:43:12.000000 webchecks-0.1.2/test/test_globalcache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-05-21 08:43:12.000000 webchecks-0.1.2/test/test_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12720 2024-05-21 08:43:12.000000 webchecks-0.1.2/test/test_security.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-21 08:43:12.000000 webchecks-0.1.2/test/test_singleton.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10296 2024-05-21 08:43:12.000000 webchecks-0.1.2/test/test_url.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:43:18.642862 webchecks-0.1.2/webchecks/
+-rw-r--r--   0 runner    (1001) docker     (127)    15257 2024-05-21 08:43:12.000000 webchecks-0.1.2/webchecks/Project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-05-21 08:43:12.000000 webchecks-0.1.2/webchecks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:43:18.642862 webchecks-0.1.2/webchecks/access/
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-05-21 08:43:12.000000 webchecks-0.1.2/webchecks/access/AccessHead.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6601 2024-05-21 08:43:12.000000 webchecks-0.1.2/webchecks/access/Gateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9837 2024-05-21 08:43:12.000000 webchecks-0.1.2/webchecks/access/RequestJS.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-05-21 08:43:12.000000 webchecks-0.1.2/webchecks/access/RequestNoJS.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6033 2024-05-21 08:43:12.000000 webchecks-0.1.2/webchecks/access/RobotsFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:43:12.000000 webchecks-0.1.2/webchecks/access/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-05-21 08:43:12.000000 webchecks-0.1.2/webchecks/access/security.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:43:18.646862 webchecks-0.1.2/webchecks/archive/
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-05-21 08:43:12.000000 webchecks-0.1.2/webchecks/archive/AccessNode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9352 2024-05-21 08:43:12.000000 webchecks-0.1.2/webchecks/archive/FileArchive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5980 2024-05-21 08:43:12.000000 webchecks-0.1.2/webchecks/archive/GlobalCache.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:43:12.000000 webchecks-0.1.2/webchecks/archive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-21 08:43:12.000000 webchecks-0.1.2/webchecks/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:43:18.646862 webchecks-0.1.2/webchecks/monitor/
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-21 08:43:12.000000 webchecks-0.1.2/webchecks/monitor/KeywordFinder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4133 2024-05-21 08:43:12.000000 webchecks-0.1.2/webchecks/monitor/Report.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:43:12.000000 webchecks-0.1.2/webchecks/monitor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:43:18.646862 webchecks-0.1.2/webchecks/profiles/
+-rw-r--r--   0 runner    (1001) docker     (127)    11257 2024-05-21 08:43:12.000000 webchecks-0.1.2/webchecks/profiles/BaseProfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-21 08:43:12.000000 webchecks-0.1.2/webchecks/profiles/ProfileConstants.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:43:12.000000 webchecks-0.1.2/webchecks/profiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-21 08:43:12.000000 webchecks-0.1.2/webchecks/profiles/profileDB.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:43:18.646862 webchecks-0.1.2/webchecks/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-21 08:43:12.000000 webchecks-0.1.2/webchecks/utils/Error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-21 08:43:12.000000 webchecks-0.1.2/webchecks/utils/OptionsError.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:43:12.000000 webchecks-0.1.2/webchecks/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-21 08:43:12.000000 webchecks-0.1.2/webchecks/utils/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-05-21 08:43:12.000000 webchecks-0.1.2/webchecks/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-05-21 08:43:12.000000 webchecks-0.1.2/webchecks/utils/file_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-05-21 08:43:12.000000 webchecks-0.1.2/webchecks/utils/messaging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-21 08:43:12.000000 webchecks-0.1.2/webchecks/utils/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-05-21 08:43:12.000000 webchecks-0.1.2/webchecks/utils/timedqueue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7090 2024-05-21 08:43:12.000000 webchecks-0.1.2/webchecks/utils/url.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:43:18.646862 webchecks-0.1.2/webchecks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8990 2024-05-21 08:43:18.000000 webchecks-0.1.2/webchecks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-05-21 08:43:18.000000 webchecks-0.1.2/webchecks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 08:43:18.000000 webchecks-0.1.2/webchecks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-21 08:43:18.000000 webchecks-0.1.2/webchecks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-21 08:43:18.000000 webchecks-0.1.2/webchecks.egg-info/top_level.txt
```

### Comparing `webchecks-0.1.1/LICENSE` & `webchecks-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `webchecks-0.1.1/PKG-INFO` & `webchecks-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webchecks
-Version: 0.1.1
+Version: 0.1.2
 Summary:  WebChecks is a BSD-licensed web search and research tool in Python traversing a given set of domains. 
 Author: CopperEagle
 License: Copyright (c) WebChecks developers.
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification,
         are permitted provided that the following conditions are met:
@@ -38,25 +38,25 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: beautifulsoup4==4.12.2
 Requires-Dist: bs4==0.0.1
 Requires-Dist: python-dotenv==1.0.0
-Requires-Dist: requests==2.31.0
+Requires-Dist: requests==2.32.0
 Requires-Dist: selenium==4.12.0
 Requires-Dist: selenium-wire==5.1.0
 Requires-Dist: typing_extensions==4.7.1
 Requires-Dist: urllib3==2.0.7
 Requires-Dist: webdriver-manager==4.0.0
 
 # WebChecks
 
 [![Python](https://img.shields.io/badge/Python-3.10-3776AB.svg?style=flat&logo=python&logoColor=white)](https://www.python.org)
-![Version](https://img.shields.io/badge/Webchecks_version-0.1-darkgreen)
+![Version](https://img.shields.io/badge/Webchecks_version-0.1.2-darkgreen)
 [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
 [![Linting: Pylint](https://img.shields.io/badge/linting-pylint-green)](https://github.com/pylint-dev/pylint)
 
 ![Linting Score](https://img.shields.io/badge/Linting_score-9.52/10.0-green)
 ![Test Coverage](https://img.shields.io/badge/Test_coverage-87%25-green)
 
 ## The project - goals
@@ -119,14 +119,16 @@
 pip3 install .
 ```
 
 Note: If you require Javascript then make sure you have Firefox because this is what is being used currently by this project.
 
 ## How to use it
 
+For the tutorial, please go to the [wiki](https://github.com/CopperEagle/WebChecks/wiki) or visit the [tutorial page](TUTORIAL.md).
+
 Basic use is fairly straight forward. *ALMOST ALL* calls the user performs is using the Project class.
 For more examples and how to programmatically access the results, enable compression, using profiles, etc. check out [the tutorial](TUTORIAL.md).
 
 ```python
 from webchecks import Project
 
 # Give name and starting address. The latter may be a list of URLs.
```

### Comparing `webchecks-0.1.1/README.md` & `webchecks-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # WebChecks
 
 [![Python](https://img.shields.io/badge/Python-3.10-3776AB.svg?style=flat&logo=python&logoColor=white)](https://www.python.org)
-![Version](https://img.shields.io/badge/Webchecks_version-0.1-darkgreen)
+![Version](https://img.shields.io/badge/Webchecks_version-0.1.2-darkgreen)
 [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
 [![Linting: Pylint](https://img.shields.io/badge/linting-pylint-green)](https://github.com/pylint-dev/pylint)
 
 ![Linting Score](https://img.shields.io/badge/Linting_score-9.52/10.0-green)
 ![Test Coverage](https://img.shields.io/badge/Test_coverage-87%25-green)
 
 ## The project - goals
@@ -68,14 +68,16 @@
 pip3 install .
 ```
 
 Note: If you require Javascript then make sure you have Firefox because this is what is being used currently by this project.
 
 ## How to use it
 
+For the tutorial, please go to the [wiki](https://github.com/CopperEagle/WebChecks/wiki) or visit the [tutorial page](TUTORIAL.md).
+
 Basic use is fairly straight forward. *ALMOST ALL* calls the user performs is using the Project class.
 For more examples and how to programmatically access the results, enable compression, using profiles, etc. check out [the tutorial](TUTORIAL.md).
 
 ```python
 from webchecks import Project
 
 # Give name and starting address. The latter may be a list of URLs.
```

### Comparing `webchecks-0.1.1/TUTORIAL.md` & `webchecks-0.1.2/TUTORIAL.md`

 * *Files identical despite different names*

### Comparing `webchecks-0.1.1/pyproject.toml` & `webchecks-0.1.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "webchecks"
-version = "0.1.1"
+version = "0.1.2"
 description = " WebChecks is a BSD-licensed web search and research tool in Python traversing a given set of domains. "
 readme = "README.md"
 authors = [{ name = "CopperEagle" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["websearch", "analysis", "automation", "web"]
 dependencies = [
     "beautifulsoup4==4.12.2",
 	"bs4==0.0.1",
 	"python-dotenv==1.0.0",
-	"requests==2.31.0",
+	"requests==2.32.0",
 	"selenium==4.12.0",
 	"selenium-wire==5.1.0",
 	"typing_extensions==4.7.1",
 	"urllib3==2.0.7",
 	"webdriver-manager==4.0.0",
 ]
 requires-python = ">=3.9"
```

### Comparing `webchecks-0.1.1/test/test_access.py` & `webchecks-0.1.2/test/test_access.py`

 * *Files identical despite different names*

### Comparing `webchecks-0.1.1/test/test_baseprofile.py` & `webchecks-0.1.2/test/test_baseprofile.py`

 * *Files identical despite different names*

### Comparing `webchecks-0.1.1/test/test_dryrun_project.py` & `webchecks-0.1.2/test/test_dryrun_project.py`

 * *Files identical despite different names*

### Comparing `webchecks-0.1.1/test/test_file_ops.py` & `webchecks-0.1.2/test/test_file_ops.py`

 * *Files identical despite different names*

### Comparing `webchecks-0.1.1/test/test_globalcache.py` & `webchecks-0.1.2/test/test_globalcache.py`

 * *Files identical despite different names*

### Comparing `webchecks-0.1.1/test/test_queue.py` & `webchecks-0.1.2/test/test_queue.py`

 * *Files identical despite different names*

### Comparing `webchecks-0.1.1/test/test_security.py` & `webchecks-0.1.2/test/test_security.py`

 * *Files identical despite different names*

### Comparing `webchecks-0.1.1/test/test_singleton.py` & `webchecks-0.1.2/test/test_singleton.py`

 * *Files identical despite different names*

### Comparing `webchecks-0.1.1/test/test_url.py` & `webchecks-0.1.2/test/test_url.py`

 * *Files identical despite different names*

### Comparing `webchecks-0.1.1/webchecks/Project.py` & `webchecks-0.1.2/webchecks/Project.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,14 +84,15 @@
         return
 
     def access_node(self) -> Type[AccessNode]:
         """Get the interface through which to access all content that was accessed."""
         return self.acc_node
 
     def _setup(self):
+        """Setup method setting up the required folders. Do not use."""
         logging("Initializing project")
         try:
             os.mkdir(self.root)
         except:
             pass
         config[RESULT_STORAGE_LOCATION] = os.path.join(self.root, config[RESULT_STORAGE_LOCATION])
         config[CACHE_STORAGE_LOCATION] = os.path.join(self.root, config[CACHE_STORAGE_LOCATION])
@@ -104,14 +105,16 @@
                 if domain == ".cache":
                     continue
                 add_profile(BaseProfile(domain))
 
         logging("Finished initializing")
 
     def __report(self):
+        """Reporter method that will be registered to be called at shutdown. Will print
+        and write the report to disk."""
         s = self.reporter.print()
         with self.open(os.path.join(self.root, "REPORT.txt"), "w") as f:
             f.write(s)
         print(s)
 
     def run(self, n_seconds : int):
         """Crawl for the specified amount of seconds.
```

### Comparing `webchecks-0.1.1/webchecks/__init__.py` & `webchecks-0.1.2/webchecks/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,8 +32,8 @@
 """
 
 
 from .Project import Project
 from .profiles.BaseProfile import BaseProfile
 
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
```

### Comparing `webchecks-0.1.1/webchecks/access/AccessHead.py` & `webchecks-0.1.2/webchecks/access/AccessHead.py`

 * *Files identical despite different names*

### Comparing `webchecks-0.1.1/webchecks/access/Gateway.py` & `webchecks-0.1.2/webchecks/access/Gateway.py`

 * *Files identical despite different names*

### Comparing `webchecks-0.1.1/webchecks/access/RequestJS.py` & `webchecks-0.1.2/webchecks/access/RequestJS.py`

 * *Files identical despite different names*

### Comparing `webchecks-0.1.1/webchecks/access/RequestNoJS.py` & `webchecks-0.1.2/webchecks/access/RequestNoJS.py`

 * *Files identical despite different names*

### Comparing `webchecks-0.1.1/webchecks/access/RobotsFile.py` & `webchecks-0.1.2/webchecks/access/RobotsFile.py`

 * *Files identical despite different names*

### Comparing `webchecks-0.1.1/webchecks/access/security.py` & `webchecks-0.1.2/webchecks/access/security.py`

 * *Files identical despite different names*

### Comparing `webchecks-0.1.1/webchecks/archive/AccessNode.py` & `webchecks-0.1.2/webchecks/archive/AccessNode.py`

 * *Files identical despite different names*

### Comparing `webchecks-0.1.1/webchecks/archive/FileArchive.py` & `webchecks-0.1.2/webchecks/archive/FileArchive.py`

 * *Files identical despite different names*

### Comparing `webchecks-0.1.1/webchecks/archive/GlobalCache.py` & `webchecks-0.1.2/webchecks/archive/GlobalCache.py`

 * *Files identical despite different names*

### Comparing `webchecks-0.1.1/webchecks/config.py` & `webchecks-0.1.2/webchecks/config.py`

 * *Files identical despite different names*

### Comparing `webchecks-0.1.1/webchecks/monitor/KeywordFinder.py` & `webchecks-0.1.2/webchecks/monitor/KeywordFinder.py`

 * *Files identical despite different names*

### Comparing `webchecks-0.1.1/webchecks/monitor/Report.py` & `webchecks-0.1.2/webchecks/monitor/Report.py`

 * *Files identical despite different names*

### Comparing `webchecks-0.1.1/webchecks/profiles/BaseProfile.py` & `webchecks-0.1.2/webchecks/profiles/BaseProfile.py`

 * *Files identical despite different names*

### Comparing `webchecks-0.1.1/webchecks/profiles/profileDB.py` & `webchecks-0.1.2/webchecks/profiles/profileDB.py`

 * *Files identical despite different names*

### Comparing `webchecks-0.1.1/webchecks/utils/Error.py` & `webchecks-0.1.2/webchecks/utils/Error.py`

 * *Files identical despite different names*

### Comparing `webchecks-0.1.1/webchecks/utils/constants.py` & `webchecks-0.1.2/webchecks/utils/constants.py`

 * *Files identical despite different names*

### Comparing `webchecks-0.1.1/webchecks/utils/file_ops.py` & `webchecks-0.1.2/webchecks/utils/file_ops.py`

 * *Files identical despite different names*

### Comparing `webchecks-0.1.1/webchecks/utils/messaging.py` & `webchecks-0.1.2/webchecks/utils/messaging.py`

 * *Files identical despite different names*

### Comparing `webchecks-0.1.1/webchecks/utils/timedqueue.py` & `webchecks-0.1.2/webchecks/utils/timedqueue.py`

 * *Files identical despite different names*

### Comparing `webchecks-0.1.1/webchecks/utils/url.py` & `webchecks-0.1.2/webchecks/utils/url.py`

 * *Files identical despite different names*

### Comparing `webchecks-0.1.1/webchecks.egg-info/PKG-INFO` & `webchecks-0.1.2/webchecks.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webchecks
-Version: 0.1.1
+Version: 0.1.2
 Summary:  WebChecks is a BSD-licensed web search and research tool in Python traversing a given set of domains. 
 Author: CopperEagle
 License: Copyright (c) WebChecks developers.
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification,
         are permitted provided that the following conditions are met:
@@ -38,25 +38,25 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: beautifulsoup4==4.12.2
 Requires-Dist: bs4==0.0.1
 Requires-Dist: python-dotenv==1.0.0
-Requires-Dist: requests==2.31.0
+Requires-Dist: requests==2.32.0
 Requires-Dist: selenium==4.12.0
 Requires-Dist: selenium-wire==5.1.0
 Requires-Dist: typing_extensions==4.7.1
 Requires-Dist: urllib3==2.0.7
 Requires-Dist: webdriver-manager==4.0.0
 
 # WebChecks
 
 [![Python](https://img.shields.io/badge/Python-3.10-3776AB.svg?style=flat&logo=python&logoColor=white)](https://www.python.org)
-![Version](https://img.shields.io/badge/Webchecks_version-0.1-darkgreen)
+![Version](https://img.shields.io/badge/Webchecks_version-0.1.2-darkgreen)
 [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
 [![Linting: Pylint](https://img.shields.io/badge/linting-pylint-green)](https://github.com/pylint-dev/pylint)
 
 ![Linting Score](https://img.shields.io/badge/Linting_score-9.52/10.0-green)
 ![Test Coverage](https://img.shields.io/badge/Test_coverage-87%25-green)
 
 ## The project - goals
@@ -119,14 +119,16 @@
 pip3 install .
 ```
 
 Note: If you require Javascript then make sure you have Firefox because this is what is being used currently by this project.
 
 ## How to use it
 
+For the tutorial, please go to the [wiki](https://github.com/CopperEagle/WebChecks/wiki) or visit the [tutorial page](TUTORIAL.md).
+
 Basic use is fairly straight forward. *ALMOST ALL* calls the user performs is using the Project class.
 For more examples and how to programmatically access the results, enable compression, using profiles, etc. check out [the tutorial](TUTORIAL.md).
 
 ```python
 from webchecks import Project
 
 # Give name and starting address. The latter may be a list of URLs.
```

### Comparing `webchecks-0.1.1/webchecks.egg-info/SOURCES.txt` & `webchecks-0.1.2/webchecks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

