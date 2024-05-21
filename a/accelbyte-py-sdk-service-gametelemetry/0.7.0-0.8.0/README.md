# Comparing `tmp/accelbyte_py_sdk_service_gametelemetry-0.7.0.tar.gz` & `tmp/accelbyte_py_sdk_service_gametelemetry-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accelbyte_py_sdk_service_gametelemetry-0.7.0.tar", last modified: Tue May  7 06:27:31 2024, max compression
+gzip compressed data, was "accelbyte_py_sdk_service_gametelemetry-0.8.0.tar", last modified: Tue May 21 03:46:44 2024, max compression
```

## Comparing `accelbyte_py_sdk_service_gametelemetry-0.7.0.tar` & `accelbyte_py_sdk_service_gametelemetry-0.8.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:27:31.026477 accelbyte_py_sdk_service_gametelemetry-0.7.0/
--rw-r--r--   0 root         (0) root         (0)     1103 2024-05-07 06:27:31.026477 accelbyte_py_sdk_service_gametelemetry-0.7.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      862 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gametelemetry-0.7.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:27:31.022477 accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:27:31.022477 accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:27:31.022477 accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/
--rw-rw-r--   0 root         (0) root         (0)     1516 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:27:31.026477 accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/models/
--rw-rw-r--   0 root         (0) root         (0)      947 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/models/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4480 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/models/base_error_response.py
--rw-rw-r--   0 root         (0) root         (0)     9154 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/models/get_namespace_event_response.py
--rw-rw-r--   0 root         (0) root         (0)     4088 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/models/http_validation_error.py
--rw-rw-r--   0 root         (0) root         (0)     3715 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/models/list_base_response_str.py
--rw-rw-r--   0 root         (0) root         (0)     5143 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/models/paged_response_get_namespace_event_response.py
--rw-rw-r--   0 root         (0) root         (0)     4248 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/models/paging.py
--rw-rw-r--   0 root         (0) root         (0)     3825 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/models/play_time_response.py
--rw-rw-r--   0 root         (0) root         (0)     7624 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/models/telemetry_body.py
--rw-rw-r--   0 root         (0) root         (0)     4744 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/models/validation_error.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:27:31.026477 accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/operations/
--rw-rw-r--   0 root         (0) root         (0)      419 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/operations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:27:31.026477 accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/operations/gametelemetry_operations/
--rw-rw-r--   0 root         (0) root         (0)      818 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/operations/gametelemetry_operations/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8434 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/operations/gametelemetry_operations/protected_get_playtime__9a0e17.py
--rw-rw-r--   0 root         (0) root         (0)     9132 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/operations/gametelemetry_operations/protected_save_events_g_832bbb.py
--rw-rw-r--   0 root         (0) root         (0)     9297 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/operations/gametelemetry_operations/protected_update_playti_4b5b85.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:27:31.026477 accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/operations/telemetry/
--rw-rw-r--   0 root         (0) root         (0)      663 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/operations/telemetry/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    14907 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/operations/telemetry/get_events_game_telemet_b2983d.py
--rw-rw-r--   0 root         (0) root         (0)     5261 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/operations/telemetry/get_namespaces_game_tel_1106fd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:27:31.026477 accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/wrappers/
--rw-rw-r--   0 root         (0) root         (0)     1605 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/wrappers/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    13207 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/wrappers/_gametelemetry_operations.py
--rw-rw-r--   0 root         (0) root         (0)     8148 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/wrappers/_telemetry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:27:31.026477 accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk_service_gametelemetry.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1103 2024-05-07 06:27:31.000000 accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk_service_gametelemetry.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1926 2024-05-07 06:27:31.000000 accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk_service_gametelemetry.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-07 06:27:31.000000 accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk_service_gametelemetry.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-07 06:27:31.000000 accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk_service_gametelemetry.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-05-07 06:27:31.000000 accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk_service_gametelemetry.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)      348 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gametelemetry-0.7.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-07 06:27:31.026477 accelbyte_py_sdk_service_gametelemetry-0.7.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:46:44.098979 accelbyte_py_sdk_service_gametelemetry-0.8.0/
+-rw-r--r--   0 root         (0) root         (0)     1103 2024-05-21 03:46:44.098979 accelbyte_py_sdk_service_gametelemetry-0.8.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      862 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gametelemetry-0.8.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:46:44.094979 accelbyte_py_sdk_service_gametelemetry-0.8.0/accelbyte_py_sdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:46:44.094979 accelbyte_py_sdk_service_gametelemetry-0.8.0/accelbyte_py_sdk/api/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:46:44.094979 accelbyte_py_sdk_service_gametelemetry-0.8.0/accelbyte_py_sdk/api/gametelemetry/
+-rw-rw-r--   0 root         (0) root         (0)     1516 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gametelemetry-0.8.0/accelbyte_py_sdk/api/gametelemetry/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:46:44.094979 accelbyte_py_sdk_service_gametelemetry-0.8.0/accelbyte_py_sdk/api/gametelemetry/models/
+-rw-rw-r--   0 root         (0) root         (0)      947 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gametelemetry-0.8.0/accelbyte_py_sdk/api/gametelemetry/models/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4480 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gametelemetry-0.8.0/accelbyte_py_sdk/api/gametelemetry/models/base_error_response.py
+-rw-rw-r--   0 root         (0) root         (0)     9154 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gametelemetry-0.8.0/accelbyte_py_sdk/api/gametelemetry/models/get_namespace_event_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4088 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gametelemetry-0.8.0/accelbyte_py_sdk/api/gametelemetry/models/http_validation_error.py
+-rw-rw-r--   0 root         (0) root         (0)     3715 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gametelemetry-0.8.0/accelbyte_py_sdk/api/gametelemetry/models/list_base_response_str.py
+-rw-rw-r--   0 root         (0) root         (0)     5143 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gametelemetry-0.8.0/accelbyte_py_sdk/api/gametelemetry/models/paged_response_get_namespace_event_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4248 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gametelemetry-0.8.0/accelbyte_py_sdk/api/gametelemetry/models/paging.py
+-rw-rw-r--   0 root         (0) root         (0)     3825 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gametelemetry-0.8.0/accelbyte_py_sdk/api/gametelemetry/models/play_time_response.py
+-rw-rw-r--   0 root         (0) root         (0)     7624 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gametelemetry-0.8.0/accelbyte_py_sdk/api/gametelemetry/models/telemetry_body.py
+-rw-rw-r--   0 root         (0) root         (0)     4744 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gametelemetry-0.8.0/accelbyte_py_sdk/api/gametelemetry/models/validation_error.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:46:44.094979 accelbyte_py_sdk_service_gametelemetry-0.8.0/accelbyte_py_sdk/api/gametelemetry/operations/
+-rw-rw-r--   0 root         (0) root         (0)      419 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gametelemetry-0.8.0/accelbyte_py_sdk/api/gametelemetry/operations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:46:44.098979 accelbyte_py_sdk_service_gametelemetry-0.8.0/accelbyte_py_sdk/api/gametelemetry/operations/gametelemetry_operations/
+-rw-rw-r--   0 root         (0) root         (0)      818 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gametelemetry-0.8.0/accelbyte_py_sdk/api/gametelemetry/operations/gametelemetry_operations/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8434 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gametelemetry-0.8.0/accelbyte_py_sdk/api/gametelemetry/operations/gametelemetry_operations/protected_get_playtime__9a0e17.py
+-rw-rw-r--   0 root         (0) root         (0)     9132 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gametelemetry-0.8.0/accelbyte_py_sdk/api/gametelemetry/operations/gametelemetry_operations/protected_save_events_g_832bbb.py
+-rw-rw-r--   0 root         (0) root         (0)     9297 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gametelemetry-0.8.0/accelbyte_py_sdk/api/gametelemetry/operations/gametelemetry_operations/protected_update_playti_4b5b85.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:46:44.098979 accelbyte_py_sdk_service_gametelemetry-0.8.0/accelbyte_py_sdk/api/gametelemetry/operations/telemetry/
+-rw-rw-r--   0 root         (0) root         (0)      663 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gametelemetry-0.8.0/accelbyte_py_sdk/api/gametelemetry/operations/telemetry/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    14907 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gametelemetry-0.8.0/accelbyte_py_sdk/api/gametelemetry/operations/telemetry/get_events_game_telemet_b2983d.py
+-rw-rw-r--   0 root         (0) root         (0)     5261 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gametelemetry-0.8.0/accelbyte_py_sdk/api/gametelemetry/operations/telemetry/get_namespaces_game_tel_1106fd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:46:44.098979 accelbyte_py_sdk_service_gametelemetry-0.8.0/accelbyte_py_sdk/api/gametelemetry/wrappers/
+-rw-rw-r--   0 root         (0) root         (0)     1605 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gametelemetry-0.8.0/accelbyte_py_sdk/api/gametelemetry/wrappers/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    13207 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gametelemetry-0.8.0/accelbyte_py_sdk/api/gametelemetry/wrappers/_gametelemetry_operations.py
+-rw-rw-r--   0 root         (0) root         (0)     8148 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gametelemetry-0.8.0/accelbyte_py_sdk/api/gametelemetry/wrappers/_telemetry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:46:44.098979 accelbyte_py_sdk_service_gametelemetry-0.8.0/accelbyte_py_sdk_service_gametelemetry.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1103 2024-05-21 03:46:44.000000 accelbyte_py_sdk_service_gametelemetry-0.8.0/accelbyte_py_sdk_service_gametelemetry.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1926 2024-05-21 03:46:44.000000 accelbyte_py_sdk_service_gametelemetry-0.8.0/accelbyte_py_sdk_service_gametelemetry.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 03:46:44.000000 accelbyte_py_sdk_service_gametelemetry-0.8.0/accelbyte_py_sdk_service_gametelemetry.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-21 03:46:44.000000 accelbyte_py_sdk_service_gametelemetry-0.8.0/accelbyte_py_sdk_service_gametelemetry.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-05-21 03:46:44.000000 accelbyte_py_sdk_service_gametelemetry-0.8.0/accelbyte_py_sdk_service_gametelemetry.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)      348 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gametelemetry-0.8.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-21 03:46:44.098979 accelbyte_py_sdk_service_gametelemetry-0.8.0/setup.cfg
```

### Comparing `accelbyte_py_sdk_service_gametelemetry-0.7.0/PKG-INFO` & `accelbyte_py_sdk_service_gametelemetry-0.8.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: accelbyte-py-sdk-service-gametelemetry
-Version: 0.7.0
+Version: 0.8.0
 Summary: AccelByte Python SDK - Analytics Game Telemetry
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: accelbyte-py-sdk-core
 
 [//]: # (Code generated. DO NOT EDIT!)
 
 # AccelByte Modular Python SDK - Service Module
 
 This is a service module for the [AccelByte Modular Python SDK](https://github.com/AccelByte/accelbyte-python-modular-sdk) package.
 
 ```text
 Analytics Game Telemetry
-* Version: 1.24.2
+* Version: 1.25.1
 ```
 
 ## Setup
 
 This SDK requires Python 3.9 to be installed.
 
 ### Install with Pip
```

### Comparing `accelbyte_py_sdk_service_gametelemetry-0.7.0/README.md` & `accelbyte_py_sdk_service_gametelemetry-0.8.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # AccelByte Modular Python SDK - Service Module
 
 This is a service module for the [AccelByte Modular Python SDK](https://github.com/AccelByte/accelbyte-python-modular-sdk) package.
 
 ```text
 Analytics Game Telemetry
-* Version: 1.24.2
+* Version: 1.25.1
 ```
 
 ## Setup
 
 This SDK requires Python 3.9 to be installed.
 
 ### Install with Pip
```

### Comparing `accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/__init__.py` & `accelbyte_py_sdk_service_gametelemetry-0.8.0/accelbyte_py_sdk/api/gametelemetry/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: service-init.j2
 
 """Auto-generated package that contains models used by the Analytics Game Telemetry."""
 
-__version__ = "1.24.2"
+__version__ = "1.25.1"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 # gametelemetry_operations
 from .wrappers import (
```

### Comparing `accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/models/__init__.py` & `accelbyte_py_sdk_service_gametelemetry-0.8.0/accelbyte_py_sdk/api/gametelemetry/models/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: model-init.j2
 
 """Auto-generated package that contains models used by the Analytics Game Telemetry."""
 
-__version__ = "1.24.2"
+__version__ = "1.25.1"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .base_error_response import BaseErrorResponse
 from .get_namespace_event_response import GetNamespaceEventResponse
```

### Comparing `accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/models/base_error_response.py` & `accelbyte_py_sdk_service_gametelemetry-0.8.0/accelbyte_py_sdk/api/gametelemetry/models/base_error_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/models/get_namespace_event_response.py` & `accelbyte_py_sdk_service_gametelemetry-0.8.0/accelbyte_py_sdk/api/gametelemetry/models/get_namespace_event_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/models/http_validation_error.py` & `accelbyte_py_sdk_service_gametelemetry-0.8.0/accelbyte_py_sdk/api/gametelemetry/models/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/models/list_base_response_str.py` & `accelbyte_py_sdk_service_gametelemetry-0.8.0/accelbyte_py_sdk/api/gametelemetry/models/list_base_response_str.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/models/paged_response_get_namespace_event_response.py` & `accelbyte_py_sdk_service_gametelemetry-0.8.0/accelbyte_py_sdk/api/gametelemetry/models/paged_response_get_namespace_event_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/models/paging.py` & `accelbyte_py_sdk_service_gametelemetry-0.8.0/accelbyte_py_sdk/api/gametelemetry/models/paging.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/models/play_time_response.py` & `accelbyte_py_sdk_service_gametelemetry-0.8.0/accelbyte_py_sdk/api/gametelemetry/models/play_time_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/models/telemetry_body.py` & `accelbyte_py_sdk_service_gametelemetry-0.8.0/accelbyte_py_sdk/api/gametelemetry/models/telemetry_body.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/models/validation_error.py` & `accelbyte_py_sdk_service_gametelemetry-0.8.0/accelbyte_py_sdk/api/gametelemetry/models/validation_error.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/operations/gametelemetry_operations/__init__.py` & `accelbyte_py_sdk_service_gametelemetry-0.8.0/accelbyte_py_sdk/api/gametelemetry/operations/gametelemetry_operations/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the Analytics Game Telemetry."""
 
-__version__ = "1.24.2"
+__version__ = "1.25.1"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .protected_get_playtime__9a0e17 import (
     ProtectedGetPlaytimeGameTelemetryV1ProtectedSteamIdsSteamIdPlaytimeGet,
```

### Comparing `accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/operations/gametelemetry_operations/protected_get_playtime__9a0e17.py` & `accelbyte_py_sdk_service_gametelemetry-0.8.0/accelbyte_py_sdk/api/gametelemetry/operations/gametelemetry_operations/protected_get_playtime__9a0e17.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/operations/gametelemetry_operations/protected_save_events_g_832bbb.py` & `accelbyte_py_sdk_service_gametelemetry-0.8.0/accelbyte_py_sdk/api/gametelemetry/operations/gametelemetry_operations/protected_save_events_g_832bbb.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/operations/gametelemetry_operations/protected_update_playti_4b5b85.py` & `accelbyte_py_sdk_service_gametelemetry-0.8.0/accelbyte_py_sdk/api/gametelemetry/operations/gametelemetry_operations/protected_update_playti_4b5b85.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/operations/telemetry/__init__.py` & `accelbyte_py_sdk_service_gametelemetry-0.8.0/accelbyte_py_sdk/api/gametelemetry/operations/telemetry/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the Analytics Game Telemetry."""
 
-__version__ = "1.24.2"
+__version__ = "1.25.1"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .get_events_game_telemet_b2983d import (
     GetEventsGameTelemetryV1AdminNamespacesNamespaceEventsGet,
```

### Comparing `accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/operations/telemetry/get_events_game_telemet_b2983d.py` & `accelbyte_py_sdk_service_gametelemetry-0.8.0/accelbyte_py_sdk/api/gametelemetry/operations/telemetry/get_events_game_telemet_b2983d.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/operations/telemetry/get_namespaces_game_tel_1106fd.py` & `accelbyte_py_sdk_service_gametelemetry-0.8.0/accelbyte_py_sdk/api/gametelemetry/operations/telemetry/get_namespaces_game_tel_1106fd.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/wrappers/__init__.py` & `accelbyte_py_sdk_service_gametelemetry-0.8.0/accelbyte_py_sdk/api/gametelemetry/wrappers/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: wrapper-init.j2
 
 """Auto-generated package that contains models used by the Analytics Game Telemetry."""
 
-__version__ = "1.24.2"
+__version__ = "1.25.1"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from ._gametelemetry_operations import (
     protected_get_playtime_game_telemetry_v1_protected_steam_ids_steam_id_playtime_get,
```

### Comparing `accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/wrappers/_gametelemetry_operations.py` & `accelbyte_py_sdk_service_gametelemetry-0.8.0/accelbyte_py_sdk/api/gametelemetry/wrappers/_gametelemetry_operations.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/wrappers/_telemetry.py` & `accelbyte_py_sdk_service_gametelemetry-0.8.0/accelbyte_py_sdk/api/gametelemetry/wrappers/_telemetry.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk_service_gametelemetry.egg-info/PKG-INFO` & `accelbyte_py_sdk_service_gametelemetry-0.8.0/accelbyte_py_sdk_service_gametelemetry.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: accelbyte-py-sdk-service-gametelemetry
-Version: 0.7.0
+Version: 0.8.0
 Summary: AccelByte Python SDK - Analytics Game Telemetry
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: accelbyte-py-sdk-core
 
 [//]: # (Code generated. DO NOT EDIT!)
 
 # AccelByte Modular Python SDK - Service Module
 
 This is a service module for the [AccelByte Modular Python SDK](https://github.com/AccelByte/accelbyte-python-modular-sdk) package.
 
 ```text
 Analytics Game Telemetry
-* Version: 1.24.2
+* Version: 1.25.1
 ```
 
 ## Setup
 
 This SDK requires Python 3.9 to be installed.
 
 ### Install with Pip
```

### Comparing `accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk_service_gametelemetry.egg-info/SOURCES.txt` & `accelbyte_py_sdk_service_gametelemetry-0.8.0/accelbyte_py_sdk_service_gametelemetry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

