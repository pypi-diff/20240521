# Comparing `tmp/dzidb-1.0.7.tar.gz` & `tmp/dzidb-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dzidb-1.0.7.tar", last modified: Tue May 21 09:41:32 2024, max compression
+gzip compressed data, was "dzidb-1.1.tar", last modified: Tue May 21 07:45:01 2024, max compression
```

## Comparing `dzidb-1.0.7.tar` & `dzidb-1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 09:41:32.078371 dzidb-1.0.7/
--rw-rw-rw-   0        0        0     1088 2024-05-20 06:49:44.000000 dzidb-1.0.7/LICENSE.txt
--rw-rw-rw-   0        0        0      208 2024-05-21 09:41:32.078371 dzidb-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0       26 2024-05-20 06:49:44.000000 dzidb-1.0.7/README.rst
-drwxrwxrwx   0        0        0        0 2024-05-21 09:41:32.077375 dzidb-1.0.7/dzidb.egg-info/
--rw-rw-rw-   0        0        0      208 2024-05-21 09:41:31.000000 dzidb-1.0.7/dzidb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      198 2024-05-21 09:41:32.000000 dzidb-1.0.7/dzidb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 09:41:31.000000 dzidb-1.0.7/dzidb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2024-05-21 09:41:31.000000 dzidb-1.0.7/dzidb.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        6 2024-05-21 09:41:31.000000 dzidb-1.0.7/dzidb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3750 2024-05-21 09:36:29.000000 dzidb-1.0.7/dzidb.py
--rw-rw-rw-   0        0        0       85 2024-05-21 09:41:32.080391 dzidb-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0      348 2024-05-21 09:41:20.000000 dzidb-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 07:45:01.650020 dzidb-1.1/
+-rw-rw-rw-   0        0        0     1088 2024-05-20 06:49:44.000000 dzidb-1.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      206 2024-05-21 07:45:01.650020 dzidb-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       26 2024-05-20 06:49:44.000000 dzidb-1.1/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-21 07:45:01.648025 dzidb-1.1/dzidb.egg-info/
+-rw-rw-rw-   0        0        0      206 2024-05-21 07:45:01.000000 dzidb-1.1/dzidb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      198 2024-05-21 07:45:01.000000 dzidb-1.1/dzidb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 07:45:01.000000 dzidb-1.1/dzidb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-05-21 07:45:01.000000 dzidb-1.1/dzidb.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        6 2024-05-21 07:45:01.000000 dzidb-1.1/dzidb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3245 2024-05-21 07:23:52.000000 dzidb-1.1/dzidb.py
+-rw-rw-rw-   0        0        0       85 2024-05-21 07:45:01.651016 dzidb-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      346 2024-05-21 07:39:01.000000 dzidb-1.1/setup.py
```

### Comparing `dzidb-1.0.7/LICENSE.txt` & `dzidb-1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dzidb-1.0.7/dzidb.py` & `dzidb-1.1/dzidb.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 import argparse
 import base64
 import json
+
 import wda
 from tabulate import tabulate
+from tidevice import MuxError
+
+from _usbmux import Usbmux
 from _device import Device
 import typing
 from _proto import LOG, MODELS, PROGRAM_NAME, ConnectionType
-from exceptions import MuxError
 
-um: wda.Usbmux = None
+um:Usbmux = None
 
 
 # 定义命令函数
 def cmd_devices(args):
     _json: typing.Final[bool] = args.json
     ds = um.device_list()
     if args.usb:
@@ -40,54 +43,39 @@
         result = []
         for item in tabdata:
             result.append({key: item[idx] for idx, key in enumerate(keys)})
         _print_json(result)
     else:
         print(tabulate(tabdata, headers=headers, tablefmt="plain"))
 
-def cmd_screencap(args):
-    c = wda.USBClient()
-
 def _print_json(value):
     def _bytes_hook(obj):
         if isinstance(obj, bytes):
             return base64.b64encode(obj).decode()
         else:
             return str(obj)
 
     print(json.dumps(value, indent=4, ensure_ascii=False, default=_bytes_hook))
 
-commands = [
+# 定义一个字典来映射命令到函数
+commands = {
     dict(action=cmd_devices,
          command="devices",
          flags=[
              dict(args=['-l'],
                   action='store_true',
                   help='output one entry per line')
          ],
-         help="show connected iOS devices"),
-    dict(action=cmd_screencap,
-         command="screencap",
-         flags=[
-             dict(args=['-u', '--device'],
-                  required=True,
-                  help='device identifier'),
-             dict(args=['-p', '--output'],
-                  required=True,
-                  help='output file path')
-         ],
-         help="take a screenshot from the device"),
-]
+         help="show connected iOS devices")
+}
 
 def main():
     parser = argparse.ArgumentParser(
         description='Custom adb-like tool.',
         formatter_class=argparse.ArgumentDefaultsHelpFormatter)
-    parser.add_argument("--socket", help="usbmuxd listen address, host:port or local-path")
-
     subparsers = parser.add_subparsers(dest='subparser')
     actions = {}
     for c in commands:
         cmd_name = c['command']
         cmd_aliases = c.get('aliases', [])
         for alias in [cmd_name] + cmd_aliases:
             actions[alias] = c['action']
@@ -104,15 +92,14 @@
             kwargs.pop('args', None)
             sp.add_argument(*args, **kwargs)
 
 
     # 解析命令行参数
     args = parser.parse_args()
 
-    um = wda.Usbmux(args.socket)
     # 检查命令是否存在于字典中
     if args.command in commands:
         # 调用相应的函数
         actions[args.command](args)
     else:
         print(f"Unknown command: {args.command}")
```

