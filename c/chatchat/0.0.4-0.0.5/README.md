# Comparing `tmp/chatchat-0.0.4.tar.gz` & `tmp/chatchat-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatchat-0.0.4.tar", last modified: Tue May 21 10:40:48 2024, max compression
+gzip compressed data, was "chatchat-0.0.5.tar", last modified: Tue May 21 11:12:30 2024, max compression
```

## Comparing `chatchat-0.0.4.tar` & `chatchat-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:40:48.687533 chatchat-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-05-21 10:40:42.000000 chatchat-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-21 10:40:48.687533 chatchat-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 10:40:42.000000 chatchat-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:40:48.683533 chatchat-0.0.4/chatchat/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-21 10:40:42.000000 chatchat-0.0.4/chatchat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-05-21 10:40:42.000000 chatchat-0.0.4/chatchat/baidu.py
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-21 10:40:42.000000 chatchat-0.0.4/chatchat/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3971 2024-05-21 10:40:42.000000 chatchat-0.0.4/chatchat/xunfei.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:40:48.687533 chatchat-0.0.4/chatchat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-21 10:40:48.000000 chatchat-0.0.4/chatchat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-21 10:40:48.000000 chatchat-0.0.4/chatchat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 10:40:48.000000 chatchat-0.0.4/chatchat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-21 10:40:48.000000 chatchat-0.0.4/chatchat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-21 10:40:48.000000 chatchat-0.0.4/chatchat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 10:40:48.687533 chatchat-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-21 10:40:42.000000 chatchat-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:12:30.727231 chatchat-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-05-21 11:12:26.000000 chatchat-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-21 11:12:30.727231 chatchat-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:12:26.000000 chatchat-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:12:30.727231 chatchat-0.0.5/chatchat/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-21 11:12:26.000000 chatchat-0.0.5/chatchat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-05-21 11:12:26.000000 chatchat-0.0.5/chatchat/baidu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-21 11:12:26.000000 chatchat-0.0.5/chatchat/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3971 2024-05-21 11:12:26.000000 chatchat-0.0.5/chatchat/xunfei.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:12:30.727231 chatchat-0.0.5/chatchat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-21 11:12:30.000000 chatchat-0.0.5/chatchat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-21 11:12:30.000000 chatchat-0.0.5/chatchat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 11:12:30.000000 chatchat-0.0.5/chatchat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-21 11:12:30.000000 chatchat-0.0.5/chatchat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-21 11:12:30.000000 chatchat-0.0.5/chatchat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 11:12:30.727231 chatchat-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-21 11:12:26.000000 chatchat-0.0.5/setup.py
```

### Comparing `chatchat-0.0.4/LICENSE` & `chatchat-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `chatchat-0.0.4/PKG-INFO` & `chatchat-0.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: chatchat
-Version: 0.0.4
-Summary: large language model api
+Version: 0.0.5
+Summary: Large Language Model API
 Home-page: https://github.com/JiauZhang/chatchat
 Author: JiauZhang
 Author-email: jiauzhang@163.com
 License: GPL-2.0
 Keywords: llm,chatapi,chatbot
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

### Comparing `chatchat-0.0.4/chatchat/baidu.py` & `chatchat-0.0.5/chatchat/baidu.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 from chatchat.base import Base
-import httpx, json, time
+import httpx, time
 
 class Completion(Base):
-    def __init__(self, jfile, name='ERNIE-Speed-8K'):
+    def __init__(self, jfile, model='ERNIE-Speed-8K'):
         # https://console.bce.baidu.com/qianfan/ais/console/onlineService
         self.api_list = {
             'ERNIE-Speed-8K': 'ernie_speed',
             'ERNIE-Speed-128K': 'ernie-speed-128k',
             'ERNIE Speed-AppBuilder': 'ai_apaas',
             'ERNIE-Lite-8K': 'ernie-lite-8k',
+            'ERNIE-Lite-8K-0922': 'eb-instant',
+            'ERNIE-Bot-turbo-0922': 'eb-instant',
             'ERNIE-Tiny-8K': 'ernie-tiny-8k',
             'Yi-34B-Chat': 'yi_34b_chat',
         }
 
-        if name not in self.api_list:
+        if model not in self.api_list:
             raise RuntimeError(f'supported chat type: {self.api_list.keys()}')
-        self.api = 'https://aip.baidubce.com/rpc/2.0/ai_custom/v1/wenxinworkshop/chat/' + self.api_list[name]
+        self.api = 'https://aip.baidubce.com/rpc/2.0/ai_custom/v1/wenxinworkshop/chat/' + self.api_list[model]
+        self.client = httpx.Client()
 
         # jfile: https://console.bce.baidu.com/qianfan/ais/console/applicationConsole/application
         #     {
         #         "baidu": {
         #             "api_key": "x",
         #             "secret_key": "y",
         #             "expires_in": "z",
@@ -53,26 +56,37 @@
             #     "expires_in": b,
             #     "session_key": "c",
             #     "access_token": "d",
             #     "scope": "e",
             #     "session_secret": "f"
             # }
             cur_time = time.time()
-            r = httpx.post(url, headers=self.headers, params=params).json()
+            r = self.client.post(url, headers=self.headers, params=params).json()
             self.jdata['access_token'] = r['access_token']
             self.jdata['expires_in'] = cur_time + float(r['expires_in'])
             jdata = self.load_json(self.jfile)
             jdata.update({'baidu': self.jdata})
             self.write_json(self.jfile, jdata)
 
     def get_access_token(self):
         self.update_access_token()
         return self.jdata['access_token']
 
-    def create(self, json):
+    def create(self, message):
+        jmsg = {
+            "messages": [
+                {
+                    "role": "user",
+                    "content": message,
+                }
+            ]
+        }
         url = f'{self.api}?access_token={self.get_access_token()}'
-        r = httpx.request("POST", url, headers=self.headers, json=json)
+        r = self.client.post(url, headers=self.headers, json=jmsg)
         return r.json()
 
-class Chat():
-    def __init__(self):
+class Chat(Completion):
+    def __init__(self, jfile, model='ERNIE-Speed-8K'):
+        super().__init__(jfile, model=model)
+
+    def chat(self):
         ...
```

### Comparing `chatchat-0.0.4/chatchat/xunfei.py` & `chatchat-0.0.5/chatchat/xunfei.py`

 * *Files identical despite different names*

### Comparing `chatchat-0.0.4/chatchat.egg-info/PKG-INFO` & `chatchat-0.0.5/chatchat.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: chatchat
-Version: 0.0.4
-Summary: large language model api
+Version: 0.0.5
+Summary: Large Language Model API
 Home-page: https://github.com/JiauZhang/chatchat
 Author: JiauZhang
 Author-email: jiauzhang@163.com
 License: GPL-2.0
 Keywords: llm,chatapi,chatbot
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

### Comparing `chatchat-0.0.4/setup.py` & `chatchat-0.0.5/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 setup(
     name = 'chatchat',
     packages = find_packages(exclude=['examples']),
-    version = '0.0.4',
+    version = '0.0.5',
     license = 'GPL-2.0',
-    description = 'large language model api',
+    description = 'Large Language Model API',
     author = 'JiauZhang',
     author_email = 'jiauzhang@163.com',
     url = 'https://github.com/JiauZhang/chatchat',
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type = 'text/markdown',
     keywords = [
         'llm',
```

