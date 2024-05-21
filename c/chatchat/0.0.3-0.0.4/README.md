# Comparing `tmp/chatchat-0.0.3.tar.gz` & `tmp/chatchat-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatchat-0.0.3.tar", last modified: Sat Sep 16 02:41:08 2023, max compression
+gzip compressed data, was "chatchat-0.0.4.tar", last modified: Tue May 21 10:40:48 2024, max compression
```

## Comparing `chatchat-0.0.3.tar` & `chatchat-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-16 02:41:08.369482 chatchat-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)    18092 2023-09-16 02:40:59.000000 chatchat-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      518 2023-09-16 02:41:08.369482 chatchat-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-16 02:40:59.000000 chatchat-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-16 02:41:08.369482 chatchat-0.0.3/chatchat/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-09-16 02:40:59.000000 chatchat-0.0.3/chatchat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2023-09-16 02:40:59.000000 chatchat-0.0.3/chatchat/baidu.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-16 02:40:59.000000 chatchat-0.0.3/chatchat/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      211 2023-09-16 02:40:59.000000 chatchat-0.0.3/chatchat/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3995 2023-09-16 02:40:59.000000 chatchat-0.0.3/chatchat/xunfei.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-16 02:41:08.369482 chatchat-0.0.3/chatchat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      518 2023-09-16 02:41:08.000000 chatchat-0.0.3/chatchat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      278 2023-09-16 02:41:08.000000 chatchat-0.0.3/chatchat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-16 02:41:08.000000 chatchat-0.0.3/chatchat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-09-16 02:41:08.000000 chatchat-0.0.3/chatchat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-09-16 02:41:08.000000 chatchat-0.0.3/chatchat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-16 02:41:08.369482 chatchat-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      799 2023-09-16 02:40:59.000000 chatchat-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:40:48.687533 chatchat-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-05-21 10:40:42.000000 chatchat-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-21 10:40:48.687533 chatchat-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 10:40:42.000000 chatchat-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:40:48.683533 chatchat-0.0.4/chatchat/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-21 10:40:42.000000 chatchat-0.0.4/chatchat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-05-21 10:40:42.000000 chatchat-0.0.4/chatchat/baidu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-21 10:40:42.000000 chatchat-0.0.4/chatchat/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3971 2024-05-21 10:40:42.000000 chatchat-0.0.4/chatchat/xunfei.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:40:48.687533 chatchat-0.0.4/chatchat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-21 10:40:48.000000 chatchat-0.0.4/chatchat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-21 10:40:48.000000 chatchat-0.0.4/chatchat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 10:40:48.000000 chatchat-0.0.4/chatchat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-21 10:40:48.000000 chatchat-0.0.4/chatchat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-21 10:40:48.000000 chatchat-0.0.4/chatchat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 10:40:48.687533 chatchat-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-21 10:40:42.000000 chatchat-0.0.4/setup.py
```

### Comparing `chatchat-0.0.3/LICENSE` & `chatchat-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `chatchat-0.0.3/PKG-INFO` & `chatchat-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatchat
-Version: 0.0.3
+Version: 0.0.4
 Summary: large language model api
 Home-page: https://github.com/JiauZhang/chatchat
 Author: JiauZhang
 Author-email: jiauzhang@163.com
 License: GPL-2.0
 Keywords: llm,chatapi,chatbot
 Classifier: Intended Audience :: Developers
```

### Comparing `chatchat-0.0.3/chatchat/baidu.py` & `chatchat-0.0.4/chatchat/baidu.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,37 @@
-import chatchat.utils as utils
+from chatchat.base import Base
 import httpx, json, time
 
-class Completion():
-    def __init__(self, jfile):
+class Completion(Base):
+    def __init__(self, jfile, name='ERNIE-Speed-8K'):
+        # https://console.bce.baidu.com/qianfan/ais/console/onlineService
+        self.api_list = {
+            'ERNIE-Speed-8K': 'ernie_speed',
+            'ERNIE-Speed-128K': 'ernie-speed-128k',
+            'ERNIE Speed-AppBuilder': 'ai_apaas',
+            'ERNIE-Lite-8K': 'ernie-lite-8k',
+            'ERNIE-Tiny-8K': 'ernie-tiny-8k',
+            'Yi-34B-Chat': 'yi_34b_chat',
+        }
+
+        if name not in self.api_list:
+            raise RuntimeError(f'supported chat type: {self.api_list.keys()}')
+        self.api = 'https://aip.baidubce.com/rpc/2.0/ai_custom/v1/wenxinworkshop/chat/' + self.api_list[name]
+
         # jfile: https://console.bce.baidu.com/qianfan/ais/console/applicationConsole/application
         #     {
         #         "baidu": {
         #             "api_key": "x",
         #             "secret_key": "y",
         #             "expires_in": "z",
         #             "access_token": "k"
         #         }
         #     }
         self.jfile = jfile
-        self.jdata = utils.load_json(jfile)['baidu']
+        self.jdata = self.load_json(jfile)['baidu']
         self.update_interval = 3600
         self.headers = {
             'Content-Type': 'application/json',
             'Accept': 'application/json'
         }
 
         if "api_key" not in self.jdata or "secret_key" not in self.jdata:
@@ -42,24 +56,23 @@
             #     "scope": "e",
             #     "session_secret": "f"
             # }
             cur_time = time.time()
             r = httpx.post(url, headers=self.headers, params=params).json()
             self.jdata['access_token'] = r['access_token']
             self.jdata['expires_in'] = cur_time + float(r['expires_in'])
-            jdata = utils.load_json(self.jfile)
+            jdata = self.load_json(self.jfile)
             jdata.update({'baidu': self.jdata})
-            utils.write_json(self.jfile, jdata)
+            self.write_json(self.jfile, jdata)
 
     def get_access_token(self):
         self.update_access_token()
         return self.jdata['access_token']
 
     def create(self, json):
-        url = "https://aip.baidubce.com/rpc/2.0/ai_custom/v1/wenxinworkshop/chat/eb-instant?access_token=" \
-            + self.get_access_token()
+        url = f'{self.api}?access_token={self.get_access_token()}'
         r = httpx.request("POST", url, headers=self.headers, json=json)
         return r.json()
 
 class Chat():
     def __init__(self):
         ...
```

### Comparing `chatchat-0.0.3/chatchat/xunfei.py` & `chatchat-0.0.4/chatchat/xunfei.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 from wsgiref.handlers import format_date_time
 from urllib.parse import urlencode
-import chatchat.utils as utils
+from chatchat.base import Base
 import base64, hashlib, hmac
 from datetime import datetime
 from time import mktime
 import time, websocket, json, ssl
-import _thread as thread
 
-class Completion():
+class Completion(Base):
     def __init__(self, jfile, version='2.0'):
         # jfile: https://console.xfyun.cn/services/bm2
         # "xunfei": {
         #     "app_id": "x",
         #     "api_secret": "y",
         #     "api_key": "z"
         # }
         self.jfile = jfile
-        self.jdata = utils.load_json(jfile)['xunfei']
+        self.jdata = self.load_json(jfile)['xunfei']
         self.update_interval = 150
         self.headers = {
             'Content-Type': 'application/json',
             'Accept': 'application/json'
         }
 
         if "api_key" not in self.jdata or "api_secret" not in self.jdata:
@@ -63,17 +62,17 @@
     def update_url(self):
         if 'expires_in' not in self.jdata or not self.jdata['expires_in'] \
             or self.jdata['expires_in'] < time.time() + self.update_interval:
             cur_time = time.time()
             url = self.create_url()
             self.jdata['url'] = url
             self.jdata['expires_in'] = cur_time + 300
-            jdata = utils.load_json(self.jfile)
+            jdata = self.load_json(self.jfile)
             jdata.update({'xunfei': self.jdata})
-            utils.write_json(self.jfile, jdata)
+            self.write_json(self.jfile, jdata)
 
     def get_url(self):
         self.update_url()
         return self.jdata['url']
 
     def on_error(self, wsapp, error):
         print(f'Error: {error}')
```

### Comparing `chatchat-0.0.3/chatchat.egg-info/PKG-INFO` & `chatchat-0.0.4/chatchat.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatchat
-Version: 0.0.3
+Version: 0.0.4
 Summary: large language model api
 Home-page: https://github.com/JiauZhang/chatchat
 Author: JiauZhang
 Author-email: jiauzhang@163.com
 License: GPL-2.0
 Keywords: llm,chatapi,chatbot
 Classifier: Intended Audience :: Developers
```

### Comparing `chatchat-0.0.3/setup.py` & `chatchat-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name = 'chatchat',
     packages = find_packages(exclude=['examples']),
-    version = '0.0.3',
+    version = '0.0.4',
     license = 'GPL-2.0',
     description = 'large language model api',
     author = 'JiauZhang',
     author_email = 'jiauzhang@163.com',
     url = 'https://github.com/JiauZhang/chatchat',
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type = 'text/markdown',
```

