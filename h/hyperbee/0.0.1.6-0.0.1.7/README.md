# Comparing `tmp/hyperbee-0.0.1.6.tar.gz` & `tmp/hyperbee-0.0.1.7.tar.gz`

## Comparing `hyperbee-0.0.1.6.tar` & `hyperbee-0.0.1.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     6631 2020-02-02 00:00:00.000000 hyperbee-0.0.1.6/src/hyperbee/__init__.py
--rw-r--r--   0        0        0    16885 2020-02-02 00:00:00.000000 hyperbee-0.0.1.6/src/hyperbee/_client.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 hyperbee-0.0.1.6/src/hyperbee/_version.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 hyperbee-0.0.1.6/src/hyperbee/version.py
--rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 hyperbee-0.0.1.6/src/hyperbee/resources/__init__.py
--rw-r--r--   0        0        0    30808 2020-02-02 00:00:00.000000 hyperbee-0.0.1.6/src/hyperbee/resources/completions.py
--rw-r--r--   0        0        0    10189 2020-02-02 00:00:00.000000 hyperbee-0.0.1.6/src/hyperbee/resources/models.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 hyperbee-0.0.1.6/src/hyperbee/resources/batch_request/__init__.py
--rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 hyperbee-0.0.1.6/src/hyperbee/resources/batch_request/batch_request.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 hyperbee-0.0.1.6/src/hyperbee/resources/chat/__init__.py
--rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 hyperbee-0.0.1.6/src/hyperbee/resources/chat/chat.py
--rw-r--r--   0        0        0    36597 2020-02-02 00:00:00.000000 hyperbee-0.0.1.6/src/hyperbee/resources/chat/completions.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 hyperbee-0.0.1.6/src/hyperbee/resources/pipeline/__init__.py
--rw-r--r--   0        0        0     6690 2020-02-02 00:00:00.000000 hyperbee-0.0.1.6/src/hyperbee/resources/pipeline/pipeline.py
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 hyperbee-0.0.1.6/.gitignore
--rw-r--r--   0        0        0    11307 2020-02-02 00:00:00.000000 hyperbee-0.0.1.6/README.md
--rw-r--r--   0        0        0     3894 2020-02-02 00:00:00.000000 hyperbee-0.0.1.6/pyproject.toml
--rw-r--r--   0        0        0    12901 2020-02-02 00:00:00.000000 hyperbee-0.0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     6631 2020-02-02 00:00:00.000000 hyperbee-0.0.1.7/src/hyperbee/__init__.py
+-rw-r--r--   0        0        0    16885 2020-02-02 00:00:00.000000 hyperbee-0.0.1.7/src/hyperbee/_client.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 hyperbee-0.0.1.7/src/hyperbee/_version.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 hyperbee-0.0.1.7/src/hyperbee/version.py
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 hyperbee-0.0.1.7/src/hyperbee/resources/__init__.py
+-rw-r--r--   0        0        0    30808 2020-02-02 00:00:00.000000 hyperbee-0.0.1.7/src/hyperbee/resources/completions.py
+-rw-r--r--   0        0        0    10189 2020-02-02 00:00:00.000000 hyperbee-0.0.1.7/src/hyperbee/resources/models.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 hyperbee-0.0.1.7/src/hyperbee/resources/batch_request/__init__.py
+-rw-r--r--   0        0        0     2988 2020-02-02 00:00:00.000000 hyperbee-0.0.1.7/src/hyperbee/resources/batch_request/batch_request.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 hyperbee-0.0.1.7/src/hyperbee/resources/chat/__init__.py
+-rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 hyperbee-0.0.1.7/src/hyperbee/resources/chat/chat.py
+-rw-r--r--   0        0        0    36597 2020-02-02 00:00:00.000000 hyperbee-0.0.1.7/src/hyperbee/resources/chat/completions.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 hyperbee-0.0.1.7/src/hyperbee/resources/pipeline/__init__.py
+-rw-r--r--   0        0        0     6690 2020-02-02 00:00:00.000000 hyperbee-0.0.1.7/src/hyperbee/resources/pipeline/pipeline.py
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 hyperbee-0.0.1.7/.gitignore
+-rw-r--r--   0        0        0    11307 2020-02-02 00:00:00.000000 hyperbee-0.0.1.7/README.md
+-rw-r--r--   0        0        0     3894 2020-02-02 00:00:00.000000 hyperbee-0.0.1.7/pyproject.toml
+-rw-r--r--   0        0        0    12901 2020-02-02 00:00:00.000000 hyperbee-0.0.1.7/PKG-INFO
```

### Comparing `hyperbee-0.0.1.6/src/hyperbee/__init__.py` & `hyperbee-0.0.1.7/src/hyperbee/__init__.py`

 * *Files identical despite different names*

### Comparing `hyperbee-0.0.1.6/src/hyperbee/_client.py` & `hyperbee-0.0.1.7/src/hyperbee/_client.py`

 * *Files identical despite different names*

### Comparing `hyperbee-0.0.1.6/src/hyperbee/resources/__init__.py` & `hyperbee-0.0.1.7/src/hyperbee/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `hyperbee-0.0.1.6/src/hyperbee/resources/completions.py` & `hyperbee-0.0.1.7/src/hyperbee/resources/completions.py`

 * *Files identical despite different names*

### Comparing `hyperbee-0.0.1.6/src/hyperbee/resources/models.py` & `hyperbee-0.0.1.7/src/hyperbee/resources/models.py`

 * *Files identical despite different names*

### Comparing `hyperbee-0.0.1.6/src/hyperbee/resources/batch_request/batch_request.py` & `hyperbee-0.0.1.7/src/hyperbee/resources/batch_request/batch_request.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,37 +6,37 @@
 import json
 import queue
 import re
 
 class batch_request():
     
     def __init__(self, api_key):
-        self.base_url = "http://34.123.162.171:30002"
-        self.base_url2 = "http://35.202.29.116:30001"
-        self.client = httpx.Client(timeout=180.0)
-        self.client2 = httpx.Client(timeout=180.0)
-        self.thread_cnt = 160
-        self.thread_cnt2 = 60
-        
+        self.base_url = "http://35.239.135.107:30001"
+        self.base_url2 = "http://34.68.121.35:30001"
+        self.client = httpx.Client(timeout=180.0,follow_redirects=True)
+        self.client2 = httpx.Client(timeout=180.0,follow_redirects=True)
+        self.thread_cnt = 120
+        self.thread_cnt2 = 120
+
     def __call__(self, prompt_list: List[str], output_length: int):
-        self.base_url = "http://34.123.162.171:30002"
-        self.base_url2 = "http://35.202.29.116:30001"
-        self.client = httpx.Client(timeout=180.0)
-        self.client2 = httpx.Client(timeout=180.0)
+        self.base_url = "http://35.239.135.107:30001"
+        self.base_url2 = "http://34.68.121.35:30001"
+        self.client = httpx.Client(timeout=180.0,follow_redirects=True)
+        self.client2 = httpx.Client(timeout=180.0,follow_redirects=True)
         output_length = output_length + 1
         threads = []
         result_queue = queue.Queue()
         
         total_thread_cnt = self.thread_cnt + self.thread_cnt2
         prompt_per_thread = (len(prompt_list) // total_thread_cnt) + 1
         try:
             thread_index = 1
             for i in range(0, len(prompt_list), prompt_per_thread):
                 batch = prompt_list[i:i + prompt_per_thread]
-                batch_tuples = [(f"<|user|>\n{prompt}<|end|>\n<|assistant|>", output_length) for prompt in batch]
+                batch_tuples = [(f"{prompt}", output_length) for prompt in batch]
                 if thread_index <= self.thread_cnt:
                     t = threading.Thread(target=send_batch, args=(self.client, self.base_url, batch_tuples, thread_index, result_queue))
                 else:
                     t = threading.Thread(target=send_batch, args=(self.client2, self.base_url2, batch_tuples, thread_index, result_queue))
                 threads.append(t)
                 thread_index += 1
                 t.start()
@@ -53,22 +53,22 @@
                 combined_results.extend(result[1])
                 
             return combined_results
         finally:
             self.client.close()
 
 def extract_required_part(output: str) -> str:
-    return output.split("<|end|>")[0][1:]
+    return output #.split("<|end|>")[0][1:]
 
 def send_batch(client, base_url, requests, thread_id, result_queue):
     results = run_vllm(client, base_url, requests)
     result_queue.put((thread_id, results))
 
 def run_vllm(client, base_url, requests: List[Tuple[str, int]]) -> List[Tuple[str, str]]:
     request_items = [{'prompt': prompt, 'output_len': output_len} for prompt, output_len in requests]
     response = client.post(f"{base_url}/run_batch", json=request_items)
     response.raise_for_status()
     results = response.json()
     batch_results = [item['result'] for item in results]
     processed_list = [extract_required_part(string) for string in batch_results]
     return processed_list
-    
+
```

### Comparing `hyperbee-0.0.1.6/src/hyperbee/resources/chat/__init__.py` & `hyperbee-0.0.1.7/src/hyperbee/resources/chat/__init__.py`

 * *Files identical despite different names*

### Comparing `hyperbee-0.0.1.6/src/hyperbee/resources/chat/chat.py` & `hyperbee-0.0.1.7/src/hyperbee/resources/chat/chat.py`

 * *Files identical despite different names*

### Comparing `hyperbee-0.0.1.6/src/hyperbee/resources/chat/completions.py` & `hyperbee-0.0.1.7/src/hyperbee/resources/chat/completions.py`

 * *Files identical despite different names*

### Comparing `hyperbee-0.0.1.6/src/hyperbee/resources/pipeline/pipeline.py` & `hyperbee-0.0.1.7/src/hyperbee/resources/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `hyperbee-0.0.1.6/README.md` & `hyperbee-0.0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `hyperbee-0.0.1.6/pyproject.toml` & `hyperbee-0.0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "hyperbee"
-version = "0.0.1.6"
+version = "0.0.1.7"
 description = "The official Python library for the hyperbee API"
 readme = "README.md"
 license = "Apache-2.0"
 authors = [
 { name = "Hive", email = "support@hyperbee.ai" },
 ]
 dependencies = [
```

### Comparing `hyperbee-0.0.1.6/PKG-INFO` & `hyperbee-0.0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: hyperbee
-Version: 0.0.1.6
+Version: 0.0.1.7
 Summary: The official Python library for the hyperbee API
 Project-URL: Homepage, https://github.com/HyperbeeAI/hive-python
 Project-URL: Repository, https://github.com/HyperbeeAI/hive-python
 Author-email: Hive <support@hyperbee.ai>
 License-Expression: Apache-2.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```
