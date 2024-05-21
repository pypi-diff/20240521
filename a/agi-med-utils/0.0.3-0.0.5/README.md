# Comparing `tmp/agi_med_utils-0.0.3.tar.gz` & `tmp/agi_med_utils-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agi_med_utils-0.0.3.tar", last modified: Mon May 20 11:04:34 2024, max compression
+gzip compressed data, was "agi_med_utils-0.0.5.tar", last modified: Tue May 21 08:50:14 2024, max compression
```

## Comparing `agi_med_utils-0.0.3.tar` & `agi_med_utils-0.0.5.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-20 11:04:34.697660 agi_med_utils-0.0.3/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       25 2024-05-13 08:33:25.000000 agi_med_utils-0.0.3/MANIFEST.in
--rw-r--r--   0 ivan      (1000) ivan      (1000)      348 2024-05-20 11:04:34.697660 agi_med_utils-0.0.3/PKG-INFO
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      110 2024-05-13 08:25:13.000000 agi_med_utils-0.0.3/README.md
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-20 11:04:34.697660 agi_med_utils-0.0.3/agi_med_utils/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       22 2024-05-20 10:58:10.000000 agi_med_utils-0.0.3/agi_med_utils/__init__.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      382 2024-05-13 10:18:02.000000 agi_med_utils-0.0.3/agi_med_utils/abstract_client.py
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-20 11:04:34.697660 agi_med_utils-0.0.3/agi_med_utils/config/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)        0 2024-05-13 08:25:13.000000 agi_med_utils-0.0.3/agi_med_utils/config/__init__.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      523 2024-05-13 09:00:12.000000 agi_med_utils-0.0.3/agi_med_utils/config/config.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      232 2024-05-13 09:00:59.000000 agi_med_utils-0.0.3/agi_med_utils/config/singleton.py
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-20 11:04:34.697660 agi_med_utils-0.0.3/agi_med_utils/llm/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)        0 2024-05-13 08:25:13.000000 agi_med_utils-0.0.3/agi_med_utils/llm/__init__.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     1494 2024-05-20 10:22:34.000000 agi_med_utils-0.0.3/agi_med_utils/llm/giga_access.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     2142 2024-05-20 10:22:34.000000 agi_med_utils-0.0.3/agi_med_utils/llm/yandex_access.py
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-20 11:04:34.697660 agi_med_utils-0.0.3/agi_med_utils.egg-info/
--rw-r--r--   0 ivan      (1000) ivan      (1000)      348 2024-05-20 11:04:34.000000 agi_med_utils-0.0.3/agi_med_utils.egg-info/PKG-INFO
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      516 2024-05-20 11:04:34.000000 agi_med_utils-0.0.3/agi_med_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)        1 2024-05-20 11:04:34.000000 agi_med_utils-0.0.3/agi_med_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       67 2024-05-20 11:04:34.000000 agi_med_utils-0.0.3/agi_med_utils.egg-info/requires.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       19 2024-05-20 11:04:34.000000 agi_med_utils-0.0.3/agi_med_utils.egg-info/top_level.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       70 2024-05-14 09:41:09.000000 agi_med_utils-0.0.3/requirements.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       38 2024-05-20 11:04:34.697660 agi_med_utils-0.0.3/setup.cfg
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      778 2024-05-13 08:36:40.000000 agi_med_utils-0.0.3/setup.py
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-20 11:04:34.697660 agi_med_utils-0.0.3/test/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)        0 2024-05-20 10:22:34.000000 agi_med_utils-0.0.3/test/__init__.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       81 2024-05-20 10:22:34.000000 agi_med_utils-0.0.3/test/base.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-21 08:50:14.757810 agi_med_utils-0.0.5/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       25 2024-05-13 08:33:25.000000 agi_med_utils-0.0.5/MANIFEST.in
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      721 2024-05-21 08:50:14.757810 agi_med_utils-0.0.5/PKG-INFO
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      422 2024-05-21 08:24:29.000000 agi_med_utils-0.0.5/README.md
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-21 08:50:14.753810 agi_med_utils-0.0.5/agi_med_utils/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       22 2024-05-21 08:49:45.000000 agi_med_utils-0.0.5/agi_med_utils/__init__.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      382 2024-05-13 10:18:02.000000 agi_med_utils-0.0.5/agi_med_utils/abstract_client.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-21 08:50:14.757810 agi_med_utils-0.0.5/agi_med_utils/config/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)        0 2024-05-13 08:25:13.000000 agi_med_utils-0.0.5/agi_med_utils/config/__init__.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      523 2024-05-13 09:00:12.000000 agi_med_utils-0.0.5/agi_med_utils/config/config.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      232 2024-05-13 09:00:59.000000 agi_med_utils-0.0.5/agi_med_utils/config/singleton.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-21 08:50:14.757810 agi_med_utils-0.0.5/agi_med_utils/llm/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)        0 2024-05-13 08:25:13.000000 agi_med_utils-0.0.5/agi_med_utils/llm/__init__.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     2004 2024-05-21 08:24:29.000000 agi_med_utils-0.0.5/agi_med_utils/llm/giga_access.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     2538 2024-05-21 08:24:29.000000 agi_med_utils-0.0.5/agi_med_utils/llm/yandex_access.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-21 08:50:14.757810 agi_med_utils-0.0.5/agi_med_utils.egg-info/
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      721 2024-05-21 08:50:14.000000 agi_med_utils-0.0.5/agi_med_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      538 2024-05-21 08:50:14.000000 agi_med_utils-0.0.5/agi_med_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)        1 2024-05-21 08:50:14.000000 agi_med_utils-0.0.5/agi_med_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       98 2024-05-21 08:50:14.000000 agi_med_utils-0.0.5/agi_med_utils.egg-info/requires.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       19 2024-05-21 08:50:14.000000 agi_med_utils-0.0.5/agi_med_utils.egg-info/top_level.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       98 2024-05-21 08:24:29.000000 agi_med_utils-0.0.5/requirements.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       38 2024-05-21 08:50:14.757810 agi_med_utils-0.0.5/setup.cfg
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      778 2024-05-13 08:36:40.000000 agi_med_utils-0.0.5/setup.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-21 08:50:14.757810 agi_med_utils-0.0.5/test/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)        0 2024-05-20 10:22:34.000000 agi_med_utils-0.0.5/test/__init__.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       61 2024-05-21 08:24:29.000000 agi_med_utils-0.0.5/test/test_base.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      843 2024-05-21 08:24:29.000000 agi_med_utils-0.0.5/test/test_llm.py
```

### Comparing `agi_med_utils-0.0.3/agi_med_utils/config/config.py` & `agi_med_utils-0.0.5/agi_med_utils/config/config.py`

 * *Files identical despite different names*

### Comparing `agi_med_utils-0.0.3/agi_med_utils/llm/giga_access.py` & `agi_med_utils-0.0.5/agi_med_utils/llm/giga_access.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 from base64 import b64encode
 from gigachat import GigaChat
 
 
 class GigaChatEntryPoint:
-    def __init__(self, config):
-        client_id = config['gigachat_creds']['client_id']
-        client_secret = config['gigachat_creds']['client_secret']
+    def __init__(self, client_id, client_secret):
         creds = b64encode(f'{client_id}:{client_secret}'.encode('utf-8')).decode('utf-8')
         self.model = GigaChat(
             credentials=creds,
             scope='GIGACHAT_API_CORP',
             verify_ssl_certs=False,
             model='GigaChat-Pro',
             profanity_check=False,
@@ -20,20 +18,29 @@
             verify_ssl_certs=False,
             model='GigaChat-Plus',
             profanity_check=False,
         )
         self.DIM = 1024
         self.ZEROS = [0 for _ in range(self.DIM)]
         self.ERROR_MESSAGE = 'Простите, я Вас не понял. Повторите, пожалуйста, поподробнее и другими словами'
+        self.warmup()
 
-    def get_response(self, total_input: str) -> str:
+    def get_response(self, total_input: str, input_is_long=False) -> str:
+        this_model = self.long_model if input_is_long else self.model
         try:
-            return self.model.chat(total_input).choices[0].message.content
+            return this_model.chat(total_input).choices[0].message.content
         except:
             return self.ERROR_MESSAGE
 
     def get_embeddings(self, total_input: str, input_is_long=False) -> list:
         this_model = self.long_model if input_is_long else self.model
         try:
             return this_model.embeddings(total_input).data[0].embedding
         except:
             return self.ZEROS
+
+    def warmup(self) -> None:
+        assert self.get_response('Прогрев') != self.ERROR_MESSAGE, 'Нет доступа к ллм!'
+        assert self.get_response('Прогрев', input_is_long=True) != self.ERROR_MESSAGE, 'Нет доступа к ллм!'
+        assert self.get_embeddings('Прогрев') != self.ZEROS, 'Нет доступа к ллм!'
+        assert self.get_embeddings('Прогрев', input_is_long=True) != self.ZEROS, 'Нет доступа к ллм!'
+
```

### Comparing `agi_med_utils-0.0.3/agi_med_utils.egg-info/SOURCES.txt` & `agi_med_utils-0.0.5/agi_med_utils.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -12,8 +12,9 @@
 agi_med_utils/config/__init__.py
 agi_med_utils/config/config.py
 agi_med_utils/config/singleton.py
 agi_med_utils/llm/__init__.py
 agi_med_utils/llm/giga_access.py
 agi_med_utils/llm/yandex_access.py
 test/__init__.py
-test/base.py
+test/test_base.py
+test/test_llm.py
```

### Comparing `agi_med_utils-0.0.3/setup.py` & `agi_med_utils-0.0.5/setup.py`

 * *Files identical despite different names*

