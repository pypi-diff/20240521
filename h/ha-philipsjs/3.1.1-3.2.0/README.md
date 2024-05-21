# Comparing `tmp/ha-philipsjs-3.1.1.tar.gz` & `tmp/ha-philipsjs-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ha-philipsjs-3.1.1.tar", last modified: Sat Oct  7 08:17:35 2023, max compression
+gzip compressed data, was "ha-philipsjs-3.2.0.tar", last modified: Tue May 21 20:59:27 2024, max compression
```

## Comparing `ha-philipsjs-3.1.1.tar` & `ha-philipsjs-3.2.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 joakim     (501) staff       (20)        0 2023-10-07 08:17:35.103835 ha-philipsjs-3.1.1/
--rw-r--r--   0 joakim     (501) staff       (20)     1069 2018-09-06 12:45:31.000000 ha-philipsjs-3.1.1/LICENSE
--rw-r--r--   0 joakim     (501) staff       (20)     2124 2023-10-07 08:17:35.103917 ha-philipsjs-3.1.1/PKG-INFO
--rw-r--r--   0 joakim     (501) staff       (20)     1479 2021-05-14 12:35:57.000000 ha-philipsjs-3.1.1/README.md
-drwxr-xr-x   0 joakim     (501) staff       (20)        0 2023-10-07 08:17:35.101514 ha-philipsjs-3.1.1/ha_philipsjs.egg-info/
--rw-r--r--   0 joakim     (501) staff       (20)     2124 2023-10-07 08:17:35.000000 ha-philipsjs-3.1.1/ha_philipsjs.egg-info/PKG-INFO
--rw-r--r--   0 joakim     (501) staff       (20)      522 2023-10-07 08:17:35.000000 ha-philipsjs-3.1.1/ha_philipsjs.egg-info/SOURCES.txt
--rw-r--r--   0 joakim     (501) staff       (20)        1 2023-10-07 08:17:35.000000 ha-philipsjs-3.1.1/ha_philipsjs.egg-info/dependency_links.txt
--rw-r--r--   0 joakim     (501) staff       (20)        1 2018-09-06 12:45:43.000000 ha-philipsjs-3.1.1/ha_philipsjs.egg-info/not-zip-safe
--rw-r--r--   0 joakim     (501) staff       (20)      123 2023-10-07 08:17:35.000000 ha-philipsjs-3.1.1/ha_philipsjs.egg-info/requires.txt
--rw-r--r--   0 joakim     (501) staff       (20)       12 2023-10-07 08:17:35.000000 ha-philipsjs-3.1.1/ha_philipsjs.egg-info/top_level.txt
-drwxr-xr-x   0 joakim     (501) staff       (20)        0 2023-10-07 08:17:35.102252 ha-philipsjs-3.1.1/haphilipsjs/
--rw-r--r--   0 joakim     (501) staff       (20)    51665 2023-10-06 23:10:38.000000 ha-philipsjs-3.1.1/haphilipsjs/__init__.py
--rw-r--r--   0 joakim     (501) staff       (20)    11396 2023-10-06 23:11:07.000000 ha-philipsjs-3.1.1/haphilipsjs/__main__.py
--rw-r--r--   0 joakim     (501) staff       (20)     7379 2022-10-15 15:42:29.000000 ha-philipsjs-3.1.1/haphilipsjs/auth.py
-drwxr-xr-x   0 joakim     (501) staff       (20)        0 2023-10-07 08:17:35.102692 ha-philipsjs-3.1.1/haphilipsjs/data/
--rw-r--r--   0 joakim     (501) staff       (20)       20 2021-04-15 20:10:56.000000 ha-philipsjs-3.1.1/haphilipsjs/data/__init__.py
--rw-r--r--   0 joakim     (501) staff       (20)     6598 2022-03-03 14:18:45.000000 ha-philipsjs-3.1.1/haphilipsjs/data/v1.py
--rw-r--r--   0 joakim     (501) staff       (20)   428744 2023-10-06 23:19:21.000000 ha-philipsjs-3.1.1/haphilipsjs/data/v6.py
-drwxr-xr-x   0 joakim     (501) staff       (20)        0 2023-10-07 08:17:35.103278 ha-philipsjs-3.1.1/haphilipsjs/dummy/
--rw-r--r--   0 joakim     (501) staff       (20)       18 2021-04-15 20:10:56.000000 ha-philipsjs-3.1.1/haphilipsjs/dummy/__init__.py
--rw-r--r--   0 joakim     (501) staff       (20)     1588 2021-04-15 20:10:56.000000 ha-philipsjs-3.1.1/haphilipsjs/dummy/v1.py
--rw-r--r--   0 joakim     (501) staff       (20)     9389 2023-02-17 18:44:47.000000 ha-philipsjs-3.1.1/haphilipsjs/typing.py
--rw-r--r--   0 joakim     (501) staff       (20)      132 2023-10-07 08:17:35.104212 ha-philipsjs-3.1.1/setup.cfg
--rw-r--r--   0 joakim     (501) staff       (20)     1550 2023-10-07 08:16:58.000000 ha-philipsjs-3.1.1/setup.py
-drwxr-xr-x   0 joakim     (501) staff       (20)        0 2023-10-07 08:17:35.103693 ha-philipsjs-3.1.1/tests/
--rw-r--r--   0 joakim     (501) staff       (20)      392 2023-10-06 23:10:38.000000 ha-philipsjs-3.1.1/tests/test_auth.py
--rw-r--r--   0 joakim     (501) staff       (20)    10142 2023-01-23 23:01:01.000000 ha-philipsjs-3.1.1/tests/test_v1.py
--rw-r--r--   0 joakim     (501) staff       (20)    21600 2023-10-06 23:19:55.000000 ha-philipsjs-3.1.1/tests/test_v6.py
+drwxr-xr-x   0 joakim     (501) staff       (20)        0 2024-05-21 20:59:27.469964 ha-philipsjs-3.2.0/
+-rw-r--r--   0 joakim     (501) staff       (20)     1069 2018-09-06 12:45:31.000000 ha-philipsjs-3.2.0/LICENSE
+-rw-r--r--   0 joakim     (501) staff       (20)     2124 2024-05-21 20:59:27.470061 ha-philipsjs-3.2.0/PKG-INFO
+-rw-r--r--   0 joakim     (501) staff       (20)     1479 2023-10-24 10:31:13.000000 ha-philipsjs-3.2.0/README.md
+drwxr-xr-x   0 joakim     (501) staff       (20)        0 2024-05-21 20:59:27.468109 ha-philipsjs-3.2.0/ha_philipsjs.egg-info/
+-rw-r--r--   0 joakim     (501) staff       (20)     2124 2024-05-21 20:59:27.000000 ha-philipsjs-3.2.0/ha_philipsjs.egg-info/PKG-INFO
+-rw-r--r--   0 joakim     (501) staff       (20)      522 2024-05-21 20:59:27.000000 ha-philipsjs-3.2.0/ha_philipsjs.egg-info/SOURCES.txt
+-rw-r--r--   0 joakim     (501) staff       (20)        1 2024-05-21 20:59:27.000000 ha-philipsjs-3.2.0/ha_philipsjs.egg-info/dependency_links.txt
+-rw-r--r--   0 joakim     (501) staff       (20)        1 2018-09-06 12:45:43.000000 ha-philipsjs-3.2.0/ha_philipsjs.egg-info/not-zip-safe
+-rw-r--r--   0 joakim     (501) staff       (20)      123 2024-05-21 20:59:27.000000 ha-philipsjs-3.2.0/ha_philipsjs.egg-info/requires.txt
+-rw-r--r--   0 joakim     (501) staff       (20)       12 2024-05-21 20:59:27.000000 ha-philipsjs-3.2.0/ha_philipsjs.egg-info/top_level.txt
+drwxr-xr-x   0 joakim     (501) staff       (20)        0 2024-05-21 20:59:27.468615 ha-philipsjs-3.2.0/haphilipsjs/
+-rw-r--r--   0 joakim     (501) staff       (20)    51848 2024-05-21 20:58:54.000000 ha-philipsjs-3.2.0/haphilipsjs/__init__.py
+-rw-r--r--   0 joakim     (501) staff       (20)    12169 2023-10-25 16:41:37.000000 ha-philipsjs-3.2.0/haphilipsjs/__main__.py
+-rw-r--r--   0 joakim     (501) staff       (20)     7379 2023-10-24 10:31:39.000000 ha-philipsjs-3.2.0/haphilipsjs/auth.py
+drwxr-xr-x   0 joakim     (501) staff       (20)        0 2024-05-21 20:59:27.468984 ha-philipsjs-3.2.0/haphilipsjs/data/
+-rw-r--r--   0 joakim     (501) staff       (20)       20 2023-10-24 10:31:13.000000 ha-philipsjs-3.2.0/haphilipsjs/data/__init__.py
+-rw-r--r--   0 joakim     (501) staff       (20)     6598 2023-10-24 10:31:13.000000 ha-philipsjs-3.2.0/haphilipsjs/data/v1.py
+-rw-r--r--   0 joakim     (501) staff       (20)   428744 2023-10-24 10:31:39.000000 ha-philipsjs-3.2.0/haphilipsjs/data/v6.py
+drwxr-xr-x   0 joakim     (501) staff       (20)        0 2024-05-21 20:59:27.469483 ha-philipsjs-3.2.0/haphilipsjs/dummy/
+-rw-r--r--   0 joakim     (501) staff       (20)       18 2023-10-24 10:31:13.000000 ha-philipsjs-3.2.0/haphilipsjs/dummy/__init__.py
+-rw-r--r--   0 joakim     (501) staff       (20)     1588 2023-10-24 10:31:13.000000 ha-philipsjs-3.2.0/haphilipsjs/dummy/v1.py
+-rw-r--r--   0 joakim     (501) staff       (20)     9389 2023-10-24 10:31:39.000000 ha-philipsjs-3.2.0/haphilipsjs/typing.py
+-rw-r--r--   0 joakim     (501) staff       (20)      132 2024-05-21 20:59:27.470353 ha-philipsjs-3.2.0/setup.cfg
+-rw-r--r--   0 joakim     (501) staff       (20)     1550 2024-05-21 20:58:54.000000 ha-philipsjs-3.2.0/setup.py
+drwxr-xr-x   0 joakim     (501) staff       (20)        0 2024-05-21 20:59:27.469836 ha-philipsjs-3.2.0/tests/
+-rw-r--r--   0 joakim     (501) staff       (20)      392 2023-10-24 10:31:39.000000 ha-philipsjs-3.2.0/tests/test_auth.py
+-rw-r--r--   0 joakim     (501) staff       (20)    10142 2023-10-24 10:31:39.000000 ha-philipsjs-3.2.0/tests/test_v1.py
+-rw-r--r--   0 joakim     (501) staff       (20)    21705 2024-05-21 20:49:24.000000 ha-philipsjs-3.2.0/tests/test_v6.py
```

### Comparing `ha-philipsjs-3.1.1/LICENSE` & `ha-philipsjs-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ha-philipsjs-3.1.1/PKG-INFO` & `ha-philipsjs-3.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: ha-philipsjs
-Version: 3.1.1
+Version: 3.2.0
 Summary: jointSPACE API for Home-Assistant
 Home-page: https://github.com/danielperna84/ha-philipsjs
-Download-URL: https://github.com/danielperna84/ha-philipsjs/tarball/3.1.1
+Download-URL: https://github.com/danielperna84/ha-philipsjs/tarball/3.2.0
 Author: Daniel Perna
 Author-email: danielperna84@gmail.com
 License: MIT License
 Keywords: jointSPACE
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ha-philipsjs-3.1.1/README.md` & `ha-philipsjs-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `ha-philipsjs-3.1.1/ha_philipsjs.egg-info/PKG-INFO` & `ha-philipsjs-3.2.0/ha_philipsjs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: ha-philipsjs
-Version: 3.1.1
+Version: 3.2.0
 Summary: jointSPACE API for Home-Assistant
 Home-page: https://github.com/danielperna84/ha-philipsjs
-Download-URL: https://github.com/danielperna84/ha-philipsjs/tarball/3.1.1
+Download-URL: https://github.com/danielperna84/ha-philipsjs/tarball/3.2.0
 Author: Daniel Perna
 Author-email: danielperna84@gmail.com
 License: MIT License
 Keywords: jointSPACE
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ha-philipsjs-3.1.1/ha_philipsjs.egg-info/SOURCES.txt` & `ha-philipsjs-3.2.0/ha_philipsjs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ha-philipsjs-3.1.1/haphilipsjs/__init__.py` & `ha-philipsjs-3.2.0/haphilipsjs/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,19 @@
         data = json.loads(text)
     except json.decoder.JSONDecodeError:
         LOG.debug("Invalid json received, trying adjusted version")
         text = text.replace("{,", "{")
         text = text.replace(",}", "}")
         while (p := text.find(",,")) >= 0:
             text = text[:p] + text[p + 1 :]
-        data = json.loads(text)
+
+        try:
+            data = json.loads(text)
+        except json.decoder.JSONDecodeError as exception:
+            raise NoneJsonData(text) from exception
 
     return data
 
 
 def decode_xtv_response(response: httpx.Response):
     try:
         text = response.text
@@ -206,15 +210,16 @@
         host=None,
         api_version=DEFAULT_API_VERSION,
         secured_transport=None,
         username=None,
         password=None,
         verify=False,
         auth_shared_key=None,
-        system = None
+        system = None,
+        limits = None,
     ):
         self._host = host
         self._connfail = 0
         self.api_version = int(api_version)
         self.on = False
         self.name: Optional[str] = None
         self.system: Optional[SystemType] = system
@@ -253,15 +258,16 @@
 
         if secured_transport or self.secured_transport:
             self.protocol = "https"
         else:
             self.protocol = "http"
 
         timeout = httpx.Timeout(timeout=TIMEOUT, connect=TIMEOUT_CONNECT)
-        limits = httpx.Limits(max_keepalive_connections=0, max_connections=3)
+        if limits is None:
+            limits = httpx.Limits(max_keepalive_connections=3, max_connections=3)
         self.session = httpx.AsyncClient(limits=limits, timeout=timeout, verify=False)
         self.session.headers["Accept"] = "application/json"
 
         if username and password:
             self.session.auth = CachedDigestAuth(username, password)
 
     @property
```

### Comparing `ha-philipsjs-3.1.1/haphilipsjs/__main__.py` & `ha-philipsjs-3.2.0/haphilipsjs/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,64 +1,69 @@
 import curses
 import platform
 import json
 import sys
+import pprint
 
 from . import PhilipsTV
+from haphilipsjs.typing import AmbilightCurrentConfiguration
+
 import asyncio
 from ast import literal_eval
 
+pp = pprint.PrettyPrinter(indent=2)
 
-async def monitor_run(stdscr, tv: PhilipsTV):
+async def monitor_run(stdscr: curses.window, tv: PhilipsTV):
 
     stdscr.clear()
     stdscr.timeout(1000)
 
     await tv.update()
 
     def get_application_name():
 
         if tv.applications:
             for app in tv.applications.values():
                 if app.get("intent") == tv.application:
                     return app.get("label")
 
-        return tv.application.get("component", {}).get("className")
+        if tv.application:
+            return tv.application.get("component", {}).get("className")
 
     while True:
 
         stdscr.clear()
         stdscr.addstr(0, 0, "Source")
         if tv.source_id:
-            stdscr.addstr(1, 0, await tv.getSourceName(tv.source_id))
+            stdscr.addstr(1, 0, await tv.getSourceName(tv.source_id) or "")
 
         stdscr.addstr(3, 15, "Menu Version")
         if tv.channel_id:
             stdscr.addstr(4, 15, str(tv.settings_version))
 
         stdscr.addstr(0, 15, "Channel")
         if tv.channel_id:
-            stdscr.addstr(1, 15, await tv.getChannelName(tv.channel_id))
+            stdscr.addstr(1, 15, await tv.getChannelName(tv.channel_id) or "")
 
 
         stdscr.addstr(0, 30, "Application")
         if tv.application:
-            stdscr.addstr(1, 30, get_application_name())
+            stdscr.addstr(1, 30, get_application_name() or "")
 
         stdscr.addstr(0, 45, "Context")
         if tv.context:
             stdscr.addstr(1, 45, tv.context.get("level1", ""))
             stdscr.addstr(2, 45, tv.context.get("level2", ""))
             stdscr.addstr(3, 45, tv.context.get("level3", ""))
             stdscr.addstr(4, 45, tv.context.get("data", ""))
 
 
         stdscr.addstr(0, 70, "Channels")
         for idx, channel  in enumerate(tv.channels_current):
-            stdscr.addstr(1+idx, 70, channel.get("name", channel.get("ccid")))
+            stdscr.addstr(1+idx, 70, str(channel.get("name", channel.get("ccid", ""))))
 
 
         def print_pixels(side, offset_y, offset_x):
             stdscr.addstr(offset_y, offset_x, "{}".format(side))
             stdscr.addstr(offset_y + 1, offset_x, "-----------")
             if side not in layer:
                 return
@@ -160,14 +165,20 @@
     )
     ambilight.add_argument(
         "--ambilight_cached",
         dest="ambilight_cached",
         type=ast.literal_eval,
         required=False,
     )
+    ambilight.add_argument(
+        "--style", dest="ambilight_style", type=str, required=False
+    )
+    ambilight.add_argument(
+        "--setting", dest="ambilight_setting", type=str, required=False
+    )
 
     pair = subparsers.add_parser("pair", help="Pair with tv")
 
     get = subparsers.add_parser("get", help="Get data from endpoint")
     get.add_argument("path", help="Sub path to grab from tv")
 
     post = subparsers.add_parser("post", help="Post data to endpoint")
@@ -245,52 +256,62 @@
                             for ccid in list(tv.channels.keys())
                         ]
                     )
                 )
             )
         print("Context: {}".format(tv.context))
 
-        print("Application: {}".format(tv.application))
-        if tv.applications:
-            print(
-                "Applications: {}".format(
-                    ", ".join(
-                        [
-                            application.get("label") or "None"
-                            for application in tv.applications.values()
-                        ]
-                    )
-                )
-            )
+        print("Application:")
+        pp.pprint(tv.application)
+
+        print("Applications:")
+        pp.pprint(list(tv.applications.values()))
+
         print("Power State: {}".format(tv.powerstate))
         print("Screen State: {}".format(tv.screenstate))
 
         await tv.getAmbilightPower()
         print("Ambilight power: {}".format(tv.ambilight_power))
         print("Ambilight mode: {}".format(tv.ambilight_mode))
-        print("Ambilight topology: {}".format(await tv.getAmbilightTopology()))
-        print("Ambilight processed: {}".format(await tv.getAmbilightProcessed()))
-        print("Ambilight measured: {}".format(await tv.getAmbilightMeasured()))
-        print("Ambilight styles: {}".format(list(tv.ambilight_styles.values())))
-        print(
-            "Ambilight currentconfiguration: {}".format(
-                tv.ambilight_current_configuration
-            )
-        )
+        print("Ambilight topology:")
+        pp.pprint(await tv.getAmbilightTopology())
+        print("Ambilight processed:")
+        pp.pprint(await tv.getAmbilightProcessed())
+        print("Ambilight measured:")
+        pp.pprint(await tv.getAmbilightMeasured())
+        print("Ambilight styles:")
+        pp.pprint(list(tv.ambilight_styles.values()))
+        print("Ambilight currentconfiguration:")
+        pp.pprint(tv.ambilight_current_configuration)
         print("Ambilight+Hue State: {}".format(tv.huelamp_power))
 
     elif args.command == "ambilight":
+        await tv.getSystem()
+        await tv.setTransport(tv.secured_transport, tv.api_version_detected)
+
         if args.ambilight_mode:
             if not await tv.setAmbilightMode(args.ambilight_mode):
                 print("Failed to set mode")
 
         if args.ambilight_cached:
             if not await tv.setAmbilightCached(args.ambilight_cached):
                 print("Failed to set ambilight cached")
 
+        current: AmbilightCurrentConfiguration = {}
+        if args.ambilight_style:
+            current["styleName"] = args.ambilight_style
+        if args.ambilight_setting:
+            current["menuSetting"] = args.ambilight_setting
+        if current:
+            current["isExpert"] = False
+
+            if await tv.setAmbilightCurrentConfiguration(current) is False:
+                print("Failed to set ambilight config")
+
+
     elif args.command == "monitor":
         await monitor(tv)
 
     elif args.command == "pair":
         await tv.getSystem()
         await tv.setTransport(tv.secured_transport, tv.api_version_detected)
         state = await tv.pairRequest(
@@ -325,15 +346,19 @@
             json.dump(res[args.node_id], sys.stdout, indent=2, ensure_ascii=False)
             print()
         elif args.settings_command == "set":
             res = await tv.postMenuItemsSettingsUpdateData({args.node_id: args.data}, force=True)
             json.dump(res, sys.stdout, indent=2, ensure_ascii=False)
             print()
     elif args.command == "markdown":
-        import argmark
+        try:
+            import argmark  # type: ignore
+        except ImportError:
+            print("Unable to find argmmark")
+            return
 
         argmark.md_help(parser)
 
     elif args.command == "notify":
         await tv.update()
         while await tv.notifyChange() is not None:
             pass
```

### Comparing `ha-philipsjs-3.1.1/haphilipsjs/auth.py` & `ha-philipsjs-3.2.0/haphilipsjs/auth.py`

 * *Files identical despite different names*

### Comparing `ha-philipsjs-3.1.1/haphilipsjs/data/v1.py` & `ha-philipsjs-3.2.0/haphilipsjs/data/v1.py`

 * *Files identical despite different names*

### Comparing `ha-philipsjs-3.1.1/haphilipsjs/data/v6.py` & `ha-philipsjs-3.2.0/haphilipsjs/data/v6.py`

 * *Files identical despite different names*

### Comparing `ha-philipsjs-3.1.1/haphilipsjs/dummy/v1.py` & `ha-philipsjs-3.2.0/haphilipsjs/dummy/v1.py`

 * *Files identical despite different names*

### Comparing `ha-philipsjs-3.1.1/haphilipsjs/typing.py` & `ha-philipsjs-3.2.0/haphilipsjs/typing.py`

 * *Files identical despite different names*

### Comparing `ha-philipsjs-3.1.1/setup.py` & `ha-philipsjs-3.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def readme():
     with open('README.md') as f:
         return f.read()
 
 PACKAGE_NAME = 'ha-philipsjs'
 HERE = os.path.abspath(os.path.dirname(__file__))
-VERSION = '3.1.1'
+VERSION = '3.2.0'
 
 PACKAGES = find_packages(exclude=['tests', 'tests.*', 'dist', 'ccu', 'build'])
 
 REQUIRES = [
     "cryptography",
     "httpx>=0.22.0",
 ]
```

### Comparing `ha-philipsjs-3.1.1/tests/test_v1.py` & `ha-philipsjs-3.2.0/tests/test_v1.py`

 * *Files identical despite different names*

### Comparing `ha-philipsjs-3.1.1/tests/test_v6.py` & `ha-philipsjs-3.2.0/tests/test_v6.py`

 * *Files 0% similar despite different names*

```diff
@@ -574,14 +574,16 @@
 
 async def test_buggy_json():
     assert haphilipsjs.decode_xtv_json("") == {}
     assert haphilipsjs.decode_xtv_json("}") == {}
     assert haphilipsjs.decode_xtv_json('{,"a":{}}') == {"a": {}}
     assert haphilipsjs.decode_xtv_json('{"a":{},}') == {"a": {}}
     assert haphilipsjs.decode_xtv_json('{"a":{},,,"b":{}}') == {"a": {}, "b": {}}
+    with pytest.raises(haphilipsjs.NoneJsonData):
+        haphilipsjs.decode_xtv_json("Plain text data")
 
 async def test_get_recordings(client_mock):
     """Verify that we can read back selected recording values"""
     await client_mock.update()
 
     recording_ongoing = False
     recording_new = 0
```

