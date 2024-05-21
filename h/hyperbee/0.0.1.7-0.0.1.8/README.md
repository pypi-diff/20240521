# Comparing `tmp/hyperbee-0.0.1.7.tar.gz` & `tmp/hyperbee-0.0.1.8.tar.gz`

## Comparing `hyperbee-0.0.1.7.tar` & `hyperbee-0.0.1.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     6631 2020-02-02 00:00:00.000000 hyperbee-0.0.1.7/src/hyperbee/__init__.py
--rw-r--r--   0        0        0    16885 2020-02-02 00:00:00.000000 hyperbee-0.0.1.7/src/hyperbee/_client.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 hyperbee-0.0.1.7/src/hyperbee/_version.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 hyperbee-0.0.1.7/src/hyperbee/version.py
--rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 hyperbee-0.0.1.7/src/hyperbee/resources/__init__.py
--rw-r--r--   0        0        0    30808 2020-02-02 00:00:00.000000 hyperbee-0.0.1.7/src/hyperbee/resources/completions.py
--rw-r--r--   0        0        0    10189 2020-02-02 00:00:00.000000 hyperbee-0.0.1.7/src/hyperbee/resources/models.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 hyperbee-0.0.1.7/src/hyperbee/resources/batch_request/__init__.py
--rw-r--r--   0        0        0     2988 2020-02-02 00:00:00.000000 hyperbee-0.0.1.7/src/hyperbee/resources/batch_request/batch_request.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 hyperbee-0.0.1.7/src/hyperbee/resources/chat/__init__.py
--rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 hyperbee-0.0.1.7/src/hyperbee/resources/chat/chat.py
--rw-r--r--   0        0        0    36597 2020-02-02 00:00:00.000000 hyperbee-0.0.1.7/src/hyperbee/resources/chat/completions.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 hyperbee-0.0.1.7/src/hyperbee/resources/pipeline/__init__.py
--rw-r--r--   0        0        0     6690 2020-02-02 00:00:00.000000 hyperbee-0.0.1.7/src/hyperbee/resources/pipeline/pipeline.py
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 hyperbee-0.0.1.7/.gitignore
--rw-r--r--   0        0        0    11307 2020-02-02 00:00:00.000000 hyperbee-0.0.1.7/README.md
--rw-r--r--   0        0        0     3894 2020-02-02 00:00:00.000000 hyperbee-0.0.1.7/pyproject.toml
--rw-r--r--   0        0        0    12901 2020-02-02 00:00:00.000000 hyperbee-0.0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     6631 2020-02-02 00:00:00.000000 hyperbee-0.0.1.8/src/hyperbee/__init__.py
+-rw-r--r--   0        0        0    16885 2020-02-02 00:00:00.000000 hyperbee-0.0.1.8/src/hyperbee/_client.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 hyperbee-0.0.1.8/src/hyperbee/_version.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 hyperbee-0.0.1.8/src/hyperbee/version.py
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 hyperbee-0.0.1.8/src/hyperbee/resources/__init__.py
+-rw-r--r--   0        0        0    30808 2020-02-02 00:00:00.000000 hyperbee-0.0.1.8/src/hyperbee/resources/completions.py
+-rw-r--r--   0        0        0    10189 2020-02-02 00:00:00.000000 hyperbee-0.0.1.8/src/hyperbee/resources/models.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 hyperbee-0.0.1.8/src/hyperbee/resources/batch_request/__init__.py
+-rw-r--r--   0        0        0     2894 2020-02-02 00:00:00.000000 hyperbee-0.0.1.8/src/hyperbee/resources/batch_request/batch_request.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 hyperbee-0.0.1.8/src/hyperbee/resources/chat/__init__.py
+-rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 hyperbee-0.0.1.8/src/hyperbee/resources/chat/chat.py
+-rw-r--r--   0        0        0    36597 2020-02-02 00:00:00.000000 hyperbee-0.0.1.8/src/hyperbee/resources/chat/completions.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 hyperbee-0.0.1.8/src/hyperbee/resources/pipeline/__init__.py
+-rw-r--r--   0        0        0     6690 2020-02-02 00:00:00.000000 hyperbee-0.0.1.8/src/hyperbee/resources/pipeline/pipeline.py
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 hyperbee-0.0.1.8/.gitignore
+-rw-r--r--   0        0        0    11307 2020-02-02 00:00:00.000000 hyperbee-0.0.1.8/README.md
+-rw-r--r--   0        0        0     3894 2020-02-02 00:00:00.000000 hyperbee-0.0.1.8/pyproject.toml
+-rw-r--r--   0        0        0    12901 2020-02-02 00:00:00.000000 hyperbee-0.0.1.8/PKG-INFO
```

### Comparing `hyperbee-0.0.1.7/src/hyperbee/__init__.py` & `hyperbee-0.0.1.8/src/hyperbee/__init__.py`

 * *Files identical despite different names*

### Comparing `hyperbee-0.0.1.7/src/hyperbee/_client.py` & `hyperbee-0.0.1.8/src/hyperbee/_client.py`

 * *Files identical despite different names*

### Comparing `hyperbee-0.0.1.7/src/hyperbee/resources/__init__.py` & `hyperbee-0.0.1.8/src/hyperbee/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `hyperbee-0.0.1.7/src/hyperbee/resources/completions.py` & `hyperbee-0.0.1.8/src/hyperbee/resources/completions.py`

 * *Files identical despite different names*

### Comparing `hyperbee-0.0.1.7/src/hyperbee/resources/models.py` & `hyperbee-0.0.1.8/src/hyperbee/resources/models.py`

 * *Files identical despite different names*

### Comparing `hyperbee-0.0.1.7/src/hyperbee/resources/batch_request/batch_request.py` & `hyperbee-0.0.1.8/src/hyperbee/resources/batch_request/batch_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,20 +8,20 @@
 import re
 
 class batch_request():
     
     def __init__(self, api_key):
         self.base_url = "http://35.239.135.107:30001"
         self.base_url2 = "http://34.68.121.35:30001"
-        self.client = httpx.Client(timeout=180.0,follow_redirects=True)
-        self.client2 = httpx.Client(timeout=180.0,follow_redirects=True)
+        
         self.thread_cnt = 120
         self.thread_cnt2 = 120
 
     def __call__(self, prompt_list: List[str], output_length: int):
+        
         self.base_url = "http://35.239.135.107:30001"
         self.base_url2 = "http://34.68.121.35:30001"
         self.client = httpx.Client(timeout=180.0,follow_redirects=True)
         self.client2 = httpx.Client(timeout=180.0,follow_redirects=True)
         output_length = output_length + 1
         threads = []
         result_queue = queue.Queue()
@@ -51,14 +51,15 @@
             combined_results = []
             for result in results:
                 combined_results.extend(result[1])
                 
             return combined_results
         finally:
             self.client.close()
+            self.client2.close()
 
 def extract_required_part(output: str) -> str:
     return output #.split("<|end|>")[0][1:]
 
 def send_batch(client, base_url, requests, thread_id, result_queue):
     results = run_vllm(client, base_url, requests)
     result_queue.put((thread_id, results))
```

### Comparing `hyperbee-0.0.1.7/src/hyperbee/resources/chat/__init__.py` & `hyperbee-0.0.1.8/src/hyperbee/resources/chat/__init__.py`

 * *Files identical despite different names*

### Comparing `hyperbee-0.0.1.7/src/hyperbee/resources/chat/chat.py` & `hyperbee-0.0.1.8/src/hyperbee/resources/chat/chat.py`

 * *Files identical despite different names*

### Comparing `hyperbee-0.0.1.7/src/hyperbee/resources/chat/completions.py` & `hyperbee-0.0.1.8/src/hyperbee/resources/chat/completions.py`

 * *Files identical despite different names*

### Comparing `hyperbee-0.0.1.7/src/hyperbee/resources/pipeline/pipeline.py` & `hyperbee-0.0.1.8/src/hyperbee/resources/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `hyperbee-0.0.1.7/README.md` & `hyperbee-0.0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `hyperbee-0.0.1.7/pyproject.toml` & `hyperbee-0.0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "hyperbee"
-version = "0.0.1.7"
+version = "0.0.1.8"
 description = "The official Python library for the hyperbee API"
 readme = "README.md"
 license = "Apache-2.0"
 authors = [
 { name = "Hive", email = "support@hyperbee.ai" },
 ]
 dependencies = [
```

### Comparing `hyperbee-0.0.1.7/PKG-INFO` & `hyperbee-0.0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: hyperbee
-Version: 0.0.1.7
+Version: 0.0.1.8
 Summary: The official Python library for the hyperbee API
 Project-URL: Homepage, https://github.com/HyperbeeAI/hive-python
 Project-URL: Repository, https://github.com/HyperbeeAI/hive-python
 Author-email: Hive <support@hyperbee.ai>
 License-Expression: Apache-2.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

