# Comparing `tmp/xbox_python_api-0.1.2.4.tar.gz` & `tmp/xbox_python_api-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xbox_python_api-0.1.2.4.tar", last modified: Fri May 17 21:32:39 2024, max compression
+gzip compressed data, was "xbox_python_api-0.1.3.tar", last modified: Tue May 21 09:09:42 2024, max compression
```

## Comparing `xbox_python_api-0.1.2.4.tar` & `xbox_python_api-0.1.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:32:39.334333 xbox_python_api-0.1.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-17 21:32:35.000000 xbox_python_api-0.1.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-17 21:32:39.334333 xbox_python_api-0.1.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-17 21:32:35.000000 xbox_python_api-0.1.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 21:32:39.334333 xbox_python_api-0.1.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-17 21:32:35.000000 xbox_python_api-0.1.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:32:39.330333 xbox_python_api-0.1.2.4/xbox_python_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-17 21:32:39.000000 xbox_python_api-0.1.2.4/xbox_python_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-17 21:32:39.000000 xbox_python_api-0.1.2.4/xbox_python_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 21:32:39.000000 xbox_python_api-0.1.2.4/xbox_python_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-17 21:32:39.000000 xbox_python_api-0.1.2.4/xbox_python_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-17 21:32:39.000000 xbox_python_api-0.1.2.4/xbox_python_api.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:32:39.330333 xbox_python_api-0.1.2.4/xpa/
--rw-r--r--   0 runner    (1001) docker     (127)     4903 2024-05-17 21:32:35.000000 xbox_python_api-0.1.2.4/xpa/URLs.py
--rw-r--r--   0 runner    (1001) docker     (127)    29965 2024-05-17 21:32:35.000000 xbox_python_api-0.1.2.4/xpa/XPA.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-17 21:32:35.000000 xbox_python_api-0.1.2.4/xpa/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:32:39.330333 xbox_python_api-0.1.2.4/xpa/classes/
--rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-05-17 21:32:35.000000 xbox_python_api-0.1.2.4/xpa/classes/ACCOUNT_INFO_GAMERTAG.py
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-17 21:32:35.000000 xbox_python_api-0.1.2.4/xpa/classes/ACCOUNT_INFO_XUID.py
--rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-05-17 21:32:35.000000 xbox_python_api-0.1.2.4/xpa/classes/CLUB_DETAILS.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-17 21:32:35.000000 xbox_python_api-0.1.2.4/xpa/classes/FRIEND_INFO_GAMERTAG.py
--rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-05-17 21:32:35.000000 xbox_python_api-0.1.2.4/xpa/classes/PLAYER_SUMMARY.py
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-17 21:32:35.000000 xbox_python_api-0.1.2.4/xpa/classes/XUID_PRESENCE.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-17 21:32:35.000000 xbox_python_api-0.1.2.4/xpa/classes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:09:42.206630 xbox_python_api-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-21 09:09:38.000000 xbox_python_api-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-21 09:09:42.206630 xbox_python_api-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-21 09:09:38.000000 xbox_python_api-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 09:09:42.206630 xbox_python_api-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-21 09:09:38.000000 xbox_python_api-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:09:42.206630 xbox_python_api-0.1.3/xbox_python_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-21 09:09:42.000000 xbox_python_api-0.1.3/xbox_python_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-21 09:09:42.000000 xbox_python_api-0.1.3/xbox_python_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 09:09:42.000000 xbox_python_api-0.1.3/xbox_python_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-21 09:09:42.000000 xbox_python_api-0.1.3/xbox_python_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-21 09:09:42.000000 xbox_python_api-0.1.3/xbox_python_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:09:42.206630 xbox_python_api-0.1.3/xpa/
+-rw-r--r--   0 runner    (1001) docker     (127)     4903 2024-05-21 09:09:38.000000 xbox_python_api-0.1.3/xpa/URLs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29965 2024-05-21 09:09:38.000000 xbox_python_api-0.1.3/xpa/XPA.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-21 09:09:38.000000 xbox_python_api-0.1.3/xpa/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:09:42.206630 xbox_python_api-0.1.3/xpa/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-05-21 09:09:38.000000 xbox_python_api-0.1.3/xpa/classes/ACCOUNT_INFO_GAMERTAG.py
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-21 09:09:38.000000 xbox_python_api-0.1.3/xpa/classes/ACCOUNT_INFO_XUID.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-05-21 09:09:38.000000 xbox_python_api-0.1.3/xpa/classes/CLUB_DETAILS.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-21 09:09:38.000000 xbox_python_api-0.1.3/xpa/classes/FRIEND_INFO_GAMERTAG.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-05-21 09:09:38.000000 xbox_python_api-0.1.3/xpa/classes/PLAYER_SUMMARY.py
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-21 09:09:38.000000 xbox_python_api-0.1.3/xpa/classes/XUID_PRESENCE.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-21 09:09:38.000000 xbox_python_api-0.1.3/xpa/classes/__init__.py
```

### Comparing `xbox_python_api-0.1.2.4/LICENSE` & `xbox_python_api-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `xbox_python_api-0.1.2.4/PKG-INFO` & `xbox_python_api-0.1.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: xbox-python-api
-Version: 0.1.2.4
+Version: 0.1.3
 Summary: Xbox API library
 Home-page: https://github.com/Rarmash/Xbox-Python-API
 Author: Rarmash
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: requests==2.31.0
+Requires-Dist: requests==2.32.0
 
 # Xbox Python API
 Xbox Python API wrapper based on https://xbl.io.
 
 ## Installation
 ```bash
 pip install xbox-python-api
```

### Comparing `xbox_python_api-0.1.2.4/README.md` & `xbox_python_api-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `xbox_python_api-0.1.2.4/xbox_python_api.egg-info/PKG-INFO` & `xbox_python_api-0.1.3/xbox_python_api.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: xbox-python-api
-Version: 0.1.2.4
+Version: 0.1.3
 Summary: Xbox API library
 Home-page: https://github.com/Rarmash/Xbox-Python-API
 Author: Rarmash
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: requests==2.31.0
+Requires-Dist: requests==2.32.0
 
 # Xbox Python API
 Xbox Python API wrapper based on https://xbl.io.
 
 ## Installation
 ```bash
 pip install xbox-python-api
```

### Comparing `xbox_python_api-0.1.2.4/xpa/URLs.py` & `xbox_python_api-0.1.3/xpa/URLs.py`

 * *Files identical despite different names*

### Comparing `xbox_python_api-0.1.2.4/xpa/XPA.py` & `xbox_python_api-0.1.3/xpa/XPA.py`

 * *Files identical despite different names*

### Comparing `xbox_python_api-0.1.2.4/xpa/classes/ACCOUNT_INFO_GAMERTAG.py` & `xbox_python_api-0.1.3/xpa/classes/ACCOUNT_INFO_GAMERTAG.py`

 * *Files identical despite different names*

### Comparing `xbox_python_api-0.1.2.4/xpa/classes/CLUB_DETAILS.py` & `xbox_python_api-0.1.3/xpa/classes/CLUB_DETAILS.py`

 * *Files identical despite different names*

### Comparing `xbox_python_api-0.1.2.4/xpa/classes/FRIEND_INFO_GAMERTAG.py` & `xbox_python_api-0.1.3/xpa/classes/FRIEND_INFO_GAMERTAG.py`

 * *Files identical despite different names*

### Comparing `xbox_python_api-0.1.2.4/xpa/classes/PLAYER_SUMMARY.py` & `xbox_python_api-0.1.3/xpa/classes/PLAYER_SUMMARY.py`

 * *Files identical despite different names*

