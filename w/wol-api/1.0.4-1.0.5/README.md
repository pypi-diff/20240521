# Comparing `tmp/wol_api-1.0.4.tar.gz` & `tmp/wol_api-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wol_api-1.0.4.tar", last modified: Mon May 20 10:33:55 2024, max compression
+gzip compressed data, was "wol_api-1.0.5.tar", last modified: Tue May 21 20:01:36 2024, max compression
```

## Comparing `wol_api-1.0.4.tar` & `wol_api-1.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:33:55.863291 wol_api-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-20 10:33:49.000000 wol_api-1.0.4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-20 10:33:55.863291 wol_api-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-20 10:33:49.000000 wol_api-1.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 10:33:55.863291 wol_api-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-05-20 10:33:49.000000 wol_api-1.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:33:55.859290 wol_api-1.0.4/wol_api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 10:33:49.000000 wol_api-1.0.4/wol_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:33:55.863291 wol_api-1.0.4/wol_api/providers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 10:33:49.000000 wol_api-1.0.4/wol_api/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-20 10:33:49.000000 wol_api-1.0.4/wol_api/providers/shared_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-05-20 10:33:49.000000 wol_api-1.0.4/wol_api/providers/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-05-20 10:33:49.000000 wol_api-1.0.4/wol_api/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:33:55.863291 wol_api-1.0.4/wol_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-20 10:33:55.000000 wol_api-1.0.4/wol_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-20 10:33:55.000000 wol_api-1.0.4/wol_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 10:33:55.000000 wol_api-1.0.4/wol_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-20 10:33:55.000000 wol_api-1.0.4/wol_api.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 10:33:55.000000 wol_api-1.0.4/wol_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-20 10:33:55.000000 wol_api-1.0.4/wol_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-20 10:33:55.000000 wol_api-1.0.4/wol_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:01:36.145172 wol_api-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-21 20:01:28.000000 wol_api-1.0.5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-21 20:01:36.145172 wol_api-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-05-21 20:01:28.000000 wol_api-1.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 20:01:36.145172 wol_api-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-05-21 20:01:28.000000 wol_api-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:01:36.145172 wol_api-1.0.5/wol_api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 20:01:28.000000 wol_api-1.0.5/wol_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:01:36.145172 wol_api-1.0.5/wol_api/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 20:01:28.000000 wol_api-1.0.5/wol_api/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-21 20:01:28.000000 wol_api-1.0.5/wol_api/providers/shared_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-05-21 20:01:28.000000 wol_api-1.0.5/wol_api/providers/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-05-21 20:01:28.000000 wol_api-1.0.5/wol_api/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:01:36.145172 wol_api-1.0.5/wol_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-21 20:01:36.000000 wol_api-1.0.5/wol_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-21 20:01:36.000000 wol_api-1.0.5/wol_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 20:01:36.000000 wol_api-1.0.5/wol_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-21 20:01:36.000000 wol_api-1.0.5/wol_api.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 20:01:36.000000 wol_api-1.0.5/wol_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-21 20:01:36.000000 wol_api-1.0.5/wol_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-21 20:01:36.000000 wol_api-1.0.5/wol_api.egg-info/top_level.txt
```

### Comparing `wol_api-1.0.4/LICENSE.md` & `wol_api-1.0.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `wol_api-1.0.4/PKG-INFO` & `wol_api-1.0.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wol_api
-Version: 1.0.4
+Version: 1.0.5
 Summary: Full template for python web projects with Docker, Github Actions, PyPI, and more.
 Home-page: https://github.com/rix1337/WakeOnLAN-API
 Author: rix1337
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -14,15 +14,23 @@
 License-File: LICENSE.md
 
 #  WakeOnLAN-API
 
 [![PyPI version](https://badge.fury.io/py/wol-api.svg)](https://badge.fury.io/py/wol-api)
 [![Github Sponsorship](https://img.shields.io/badge/support-me-red.svg)](https://github.com/users/rix1337/sponsorship)
 
-A simple http interface to send wake on LAN commands. Just send a `POST` to `/FF:FF:FF:FF:FF:FF` where `FF:FF:FF:FF:FF:FF` is the desired MAC address of the device to be woken up.
+A simple http interface to send wake on LAN commands.
+
+Just send a
+- `GET` to `/FF:FF:FF:FF:FF:FF` 
+- `POST` to `/FF:FF:FF:FF:FF:FF` 
+- `GET` to `/wol/FF:FF:FF:FF:FF:FF` 
+- `POST` to `/wol/FF:FF:FF:FF:FF:FF` 
+
+where `FF:FF:FF:FF:FF:FF` is the desired MAC address of the device to be woken up.
 
 # Setup
 
 `pip install wol_api`
 
 # Run
```

### Comparing `wol_api-1.0.4/setup.py` & `wol_api-1.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `wol_api-1.0.4/wol_api/providers/version.py` & `wol_api-1.0.5/wol_api/providers/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # WakeOnLAN-API
 # Project by https://github.com/rix1337
 
 import re
 
 
 def get_version():
-    return "1.0.4"
+    return "1.0.5"
 
 
 def create_version_file():
     version = get_version()
     version_clean = re.sub(r'[^\d.]', '', version)
     if "a" in version:
         suffix = version.split("a")[1]
```

### Comparing `wol_api-1.0.4/wol_api/run.py` & `wol_api-1.0.5/wol_api/run.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import argparse
 import multiprocessing
 import re
 import sys
 from socketserver import ThreadingMixIn
 from wsgiref.simple_server import make_server, WSGIServer, WSGIRequestHandler
 
-from bottle import Bottle
+from bottle import Bottle, abort, request
 from wakeonlan import send_magic_packet
 
 from wol_api.providers import shared_state, version
 
 
 class ThreadingWSGIServer(ThreadingMixIn, WSGIServer):
     daemon_threads = True
@@ -56,30 +56,31 @@
                 print("[WakeOnLAN-API] Port must be an integer")
                 sys.exit(1)
         else:
             shared_state.update("port", 8080)
 
         app = Bottle()
 
-        @app.post("/<mac>")
-        def status(mac):
-            mac = mac.replace("-", ":").strip()
-            # Validate MAC address
-            if not re.match("^([0-9A-Fa-f]{2}[:-]){5}([0-9A-Fa-f]{2})$", mac):
-                print("Invalid MAC address: " + mac)
-                return "Invalid MAC address", 400
-
-            # Wake up device
+        def wake_device(mac):
             try:
-                print("Waking up: " + mac)
                 send_magic_packet(mac)
-                return "Success", 200
+                message = f"Request type: {request.method}, Path: {request.path} | Woke up: {mac}"
+                print(message)
+                return message
             except Exception as e:
-                print(f"Failed to wake up device: {e}")
-                return "Failed", 500
+                message = f"Request type: {request.method}, Path: {request.path} | Error: {str(e)}"
+                print(message)
+                abort(500, message)
+
+        @app.post("/<mac>")
+        @app.get("/<mac>")
+        @app.post("/wol/<mac>")
+        @app.get("/wol/<mac>")
+        def status(mac):
+            return wake_device(mac)
 
         print(f"[WakeOnLAN-API] Running at http://127.0.0.1:{shared_state.values['port']}")
         try:
             Server(app, listen='0.0.0.0', port=shared_state.values["port"]).serve_forever()
         except KeyboardInterrupt:
             sys.exit(0)
```

### Comparing `wol_api-1.0.4/wol_api.egg-info/PKG-INFO` & `wol_api-1.0.5/wol_api.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wol-api
-Version: 1.0.4
+Version: 1.0.5
 Summary: Full template for python web projects with Docker, Github Actions, PyPI, and more.
 Home-page: https://github.com/rix1337/WakeOnLAN-API
 Author: rix1337
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -14,15 +14,23 @@
 License-File: LICENSE.md
 
 #  WakeOnLAN-API
 
 [![PyPI version](https://badge.fury.io/py/wol-api.svg)](https://badge.fury.io/py/wol-api)
 [![Github Sponsorship](https://img.shields.io/badge/support-me-red.svg)](https://github.com/users/rix1337/sponsorship)
 
-A simple http interface to send wake on LAN commands. Just send a `POST` to `/FF:FF:FF:FF:FF:FF` where `FF:FF:FF:FF:FF:FF` is the desired MAC address of the device to be woken up.
+A simple http interface to send wake on LAN commands.
+
+Just send a
+- `GET` to `/FF:FF:FF:FF:FF:FF` 
+- `POST` to `/FF:FF:FF:FF:FF:FF` 
+- `GET` to `/wol/FF:FF:FF:FF:FF:FF` 
+- `POST` to `/wol/FF:FF:FF:FF:FF:FF` 
+
+where `FF:FF:FF:FF:FF:FF` is the desired MAC address of the device to be woken up.
 
 # Setup
 
 `pip install wol_api`
 
 # Run
```

