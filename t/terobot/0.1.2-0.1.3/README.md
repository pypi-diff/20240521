# Comparing `tmp/terobot-0.1.2.tar.gz` & `tmp/terobot-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terobot-0.1.2.tar", last modified: Tue May 21 10:53:36 2024, max compression
+gzip compressed data, was "terobot-0.1.3.tar", last modified: Tue May 21 10:57:01 2024, max compression
```

## Comparing `terobot-0.1.2.tar` & `terobot-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 tvarnier   (501) staff       (20)        0 2024-05-21 10:53:36.104509 terobot-0.1.2/
--rw-r--r--   0 tvarnier   (501) staff       (20)      275 2024-05-21 10:53:36.104200 terobot-0.1.2/PKG-INFO
--rw-r--r--   0 tvarnier   (501) staff       (20)       34 2024-05-21 09:02:31.000000 terobot-0.1.2/README.md
--rw-r--r--   0 tvarnier   (501) staff       (20)      381 2024-05-21 10:53:29.000000 terobot-0.1.2/pyproject.toml
--rw-r--r--   0 tvarnier   (501) staff       (20)       38 2024-05-21 10:53:36.104584 terobot-0.1.2/setup.cfg
-drwxr-xr-x   0 tvarnier   (501) staff       (20)        0 2024-05-21 10:53:36.094658 terobot-0.1.2/terobot/
--rw-r--r--   0 tvarnier   (501) staff       (20)       27 2024-05-21 10:43:05.000000 terobot-0.1.2/terobot/__init__.py
--rw-r--r--   0 tvarnier   (501) staff       (20)     4642 2024-05-21 10:53:17.000000 terobot-0.1.2/terobot/client.py
-drwxr-xr-x   0 tvarnier   (501) staff       (20)        0 2024-05-21 10:53:36.103781 terobot-0.1.2/terobot.egg-info/
--rw-r--r--   0 tvarnier   (501) staff       (20)      275 2024-05-21 10:53:36.000000 terobot-0.1.2/terobot.egg-info/PKG-INFO
--rw-r--r--   0 tvarnier   (501) staff       (20)      216 2024-05-21 10:53:36.000000 terobot-0.1.2/terobot.egg-info/SOURCES.txt
--rw-r--r--   0 tvarnier   (501) staff       (20)        1 2024-05-21 10:53:36.000000 terobot-0.1.2/terobot.egg-info/dependency_links.txt
--rw-r--r--   0 tvarnier   (501) staff       (20)       17 2024-05-21 10:53:36.000000 terobot-0.1.2/terobot.egg-info/requires.txt
--rw-r--r--   0 tvarnier   (501) staff       (20)        8 2024-05-21 10:53:36.000000 terobot-0.1.2/terobot.egg-info/top_level.txt
+drwxr-xr-x   0 tvarnier   (501) staff       (20)        0 2024-05-21 10:57:01.184562 terobot-0.1.3/
+-rw-r--r--   0 tvarnier   (501) staff       (20)      275 2024-05-21 10:57:01.184287 terobot-0.1.3/PKG-INFO
+-rw-r--r--   0 tvarnier   (501) staff       (20)       34 2024-05-21 09:02:31.000000 terobot-0.1.3/README.md
+-rw-r--r--   0 tvarnier   (501) staff       (20)      381 2024-05-21 10:56:54.000000 terobot-0.1.3/pyproject.toml
+-rw-r--r--   0 tvarnier   (501) staff       (20)       38 2024-05-21 10:57:01.184619 terobot-0.1.3/setup.cfg
+drwxr-xr-x   0 tvarnier   (501) staff       (20)        0 2024-05-21 10:57:01.176609 terobot-0.1.3/terobot/
+-rw-r--r--   0 tvarnier   (501) staff       (20)       21 2024-05-21 10:56:34.000000 terobot-0.1.3/terobot/__init__.py
+-rw-r--r--   0 tvarnier   (501) staff       (20)     4636 2024-05-21 10:56:40.000000 terobot-0.1.3/terobot/client.py
+drwxr-xr-x   0 tvarnier   (501) staff       (20)        0 2024-05-21 10:57:01.183897 terobot-0.1.3/terobot.egg-info/
+-rw-r--r--   0 tvarnier   (501) staff       (20)      275 2024-05-21 10:57:01.000000 terobot-0.1.3/terobot.egg-info/PKG-INFO
+-rw-r--r--   0 tvarnier   (501) staff       (20)      216 2024-05-21 10:57:01.000000 terobot-0.1.3/terobot.egg-info/SOURCES.txt
+-rw-r--r--   0 tvarnier   (501) staff       (20)        1 2024-05-21 10:57:01.000000 terobot-0.1.3/terobot.egg-info/dependency_links.txt
+-rw-r--r--   0 tvarnier   (501) staff       (20)       17 2024-05-21 10:57:01.000000 terobot-0.1.3/terobot.egg-info/requires.txt
+-rw-r--r--   0 tvarnier   (501) staff       (20)        8 2024-05-21 10:57:01.000000 terobot-0.1.3/terobot.egg-info/top_level.txt
```

### Comparing `terobot-0.1.2/terobot/client.py` & `terobot-0.1.3/terobot/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import requests
 from datetime import datetime, timezone
-from typing import Optional, Any, Dict
+from typing import Optional, Any
 
 DEFAULT_SERVER = 'https://terobot.lobelia.earth'
 
 # ====================================
 # Declarations
 # ====================================
 class BotOptions:
```

