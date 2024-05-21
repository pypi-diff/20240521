# Comparing `tmp/llmsmith-0.6.0.tar.gz` & `tmp/llmsmith-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmsmith-0.6.0.tar", max compression
+gzip compressed data, was "llmsmith-0.7.0.tar", max compression
```

## Comparing `llmsmith-0.6.0.tar` & `llmsmith-0.7.0.tar`

### file list

```diff
@@ -1,49 +1,53 @@
--rw-r--r--   0        0        0     1101 2024-04-03 09:01:34.959168 llmsmith-0.6.0/LICENSE
--rw-r--r--   0        0        0     1530 2024-05-19 16:22:27.175607 llmsmith-0.6.0/README.md
--rw-r--r--   0        0        0       78 2024-03-15 04:21:07.861053 llmsmith-0.6.0/llmsmith/__init__.py
--rw-r--r--   0        0        0        0 2024-04-15 12:18:59.343170 llmsmith-0.6.0/llmsmith/agent/__init__.py
--rw-r--r--   0        0        0      209 2024-04-18 09:12:45.143269 llmsmith-0.6.0/llmsmith/agent/errors.py
--rw-r--r--   0        0        0        0 2024-04-15 12:19:30.041692 llmsmith-0.6.0/llmsmith/agent/function/__init__.py
--rw-r--r--   0        0        0     5618 2024-05-07 11:09:56.773034 llmsmith-0.6.0/llmsmith/agent/function/cohere.py
--rw-r--r--   0        0        0     5926 2024-05-07 11:14:41.988980 llmsmith-0.6.0/llmsmith/agent/function/gemini.py
--rw-r--r--   0        0        0     8889 2024-05-07 11:14:54.558351 llmsmith-0.6.0/llmsmith/agent/function/openai.py
--rw-r--r--   0        0        0        0 2024-04-23 05:43:58.075908 llmsmith-0.6.0/llmsmith/agent/function/options/__init__.py
--rw-r--r--   0        0        0     1985 2024-05-07 12:01:42.276643 llmsmith-0.6.0/llmsmith/agent/function/options/openai.py
--rw-r--r--   0        0        0        0 2024-04-18 05:26:07.193675 llmsmith-0.6.0/llmsmith/agent/tool/__init__.py
--rw-r--r--   0        0        0      898 2024-05-06 11:04:31.823036 llmsmith-0.6.0/llmsmith/agent/tool/cohere.py
--rw-r--r--   0        0        0     1014 2024-05-07 11:15:14.677758 llmsmith-0.6.0/llmsmith/agent/tool/gemini.py
--rw-r--r--   0        0        0     2002 2024-05-07 11:15:20.017868 llmsmith-0.6.0/llmsmith/agent/tool/openai.py
--rw-r--r--   0        0        0        0 2024-03-14 11:47:53.187559 llmsmith-0.6.0/llmsmith/job/__init__.py
--rw-r--r--   0        0        0     7428 2024-04-02 12:37:57.531013 llmsmith-0.6.0/llmsmith/job/base.py
--rw-r--r--   0        0        0     8550 2024-04-03 05:58:40.426172 llmsmith-0.6.0/llmsmith/job/job.py
--rw-r--r--   0        0        0        0 2024-04-30 12:02:50.437340 llmsmith-0.6.0/llmsmith/reranker/__init__.py
--rw-r--r--   0        0        0      575 2024-05-02 04:19:45.995736 llmsmith-0.6.0/llmsmith/reranker/base.py
--rw-r--r--   0        0        0     2849 2024-05-07 11:15:37.535755 llmsmith-0.6.0/llmsmith/reranker/cohere.py
--rw-r--r--   0        0        0        0 2024-05-02 03:46:41.851482 llmsmith-0.6.0/llmsmith/reranker/options/__init__.py
--rw-r--r--   0        0        0     1082 2024-05-07 11:15:49.065554 llmsmith-0.6.0/llmsmith/reranker/options/cohere.py
--rw-r--r--   0        0        0        0 2024-03-14 11:03:16.994184 llmsmith-0.6.0/llmsmith/task/__init__.py
--rw-r--r--   0        0        0     1329 2024-04-02 12:23:38.410395 llmsmith-0.6.0/llmsmith/task/base.py
--rw-r--r--   0        0        0      437 2024-04-22 10:15:31.395712 llmsmith-0.6.0/llmsmith/task/models.py
--rw-r--r--   0        0        0        0 2024-03-15 07:53:27.486482 llmsmith-0.6.0/llmsmith/task/retrieval/__init__.py
--rw-r--r--   0        0        0        0 2024-04-03 07:44:57.026421 llmsmith-0.6.0/llmsmith/task/retrieval/vector/__init__.py
--rw-r--r--   0        0        0      437 2024-05-01 10:16:21.291906 llmsmith-0.6.0/llmsmith/task/retrieval/vector/base.py
--rw-r--r--   0        0        0     3715 2024-05-07 11:16:01.033751 llmsmith-0.6.0/llmsmith/task/retrieval/vector/chromadb.py
--rw-r--r--   0        0        0        0 2024-04-09 12:03:40.797998 llmsmith-0.6.0/llmsmith/task/retrieval/vector/options/__init__.py
--rw-r--r--   0        0        0      897 2024-05-07 11:16:13.459211 llmsmith-0.6.0/llmsmith/task/retrieval/vector/options/chromadb.py
--rw-r--r--   0        0        0     1157 2024-05-19 16:22:27.178379 llmsmith-0.6.0/llmsmith/task/retrieval/vector/options/pinecone.py
--rw-r--r--   0        0        0     1316 2024-05-07 11:16:18.001301 llmsmith-0.6.0/llmsmith/task/retrieval/vector/options/qdrant.py
--rw-r--r--   0        0        0     3858 2024-05-19 16:22:27.179017 llmsmith-0.6.0/llmsmith/task/retrieval/vector/pinecone.py
--rw-r--r--   0        0        0     4295 2024-05-07 11:16:06.806987 llmsmith-0.6.0/llmsmith/task/retrieval/vector/qdrant.py
--rw-r--r--   0        0        0        0 2024-03-15 11:22:26.459597 llmsmith-0.6.0/llmsmith/task/textgen/__init__.py
--rw-r--r--   0        0        0     3036 2024-05-07 11:16:24.273688 llmsmith-0.6.0/llmsmith/task/textgen/claude.py
--rw-r--r--   0        0        0     6108 2024-05-07 04:06:44.987359 llmsmith-0.6.0/llmsmith/task/textgen/cohere.py
--rw-r--r--   0        0        0      681 2024-04-18 12:18:54.653626 llmsmith-0.6.0/llmsmith/task/textgen/errors.py
--rw-r--r--   0        0        0     7102 2024-05-07 11:16:33.346249 llmsmith-0.6.0/llmsmith/task/textgen/gemini.py
--rw-r--r--   0        0        0     6441 2024-05-07 11:16:37.844109 llmsmith-0.6.0/llmsmith/task/textgen/openai.py
--rw-r--r--   0        0        0        0 2024-03-19 08:37:09.919088 llmsmith-0.6.0/llmsmith/task/textgen/options/__init__.py
--rw-r--r--   0        0        0     1489 2024-05-07 11:16:43.800922 llmsmith-0.6.0/llmsmith/task/textgen/options/claude.py
--rw-r--r--   0        0        0     2317 2024-05-07 12:16:46.722433 llmsmith-0.6.0/llmsmith/task/textgen/options/cohere.py
--rw-r--r--   0        0        0     1337 2024-05-07 11:16:51.095809 llmsmith-0.6.0/llmsmith/task/textgen/options/gemini.py
--rw-r--r--   0        0        0     1881 2024-05-07 11:16:55.681932 llmsmith-0.6.0/llmsmith/task/textgen/options/openai.py
--rw-r--r--   0        0        0     2028 2024-05-19 16:22:35.929832 llmsmith-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     3442 1970-01-01 00:00:00.000000 llmsmith-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1101 2024-04-03 09:01:34.959168 llmsmith-0.7.0/LICENSE
+-rw-r--r--   0        0        0     1539 2024-05-21 10:38:22.997573 llmsmith-0.7.0/README.md
+-rw-r--r--   0        0        0       78 2024-03-15 04:21:07.861053 llmsmith-0.7.0/llmsmith/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-15 12:18:59.343170 llmsmith-0.7.0/llmsmith/agent/__init__.py
+-rw-r--r--   0        0        0      209 2024-04-18 09:12:45.143269 llmsmith-0.7.0/llmsmith/agent/errors.py
+-rw-r--r--   0        0        0        0 2024-04-15 12:19:30.041692 llmsmith-0.7.0/llmsmith/agent/function/__init__.py
+-rw-r--r--   0        0        0     5609 2024-05-21 10:38:23.003499 llmsmith-0.7.0/llmsmith/agent/function/cohere.py
+-rw-r--r--   0        0        0     5917 2024-05-21 10:38:23.004387 llmsmith-0.7.0/llmsmith/agent/function/gemini.py
+-rw-r--r--   0        0        0     5539 2024-05-21 10:38:23.005130 llmsmith-0.7.0/llmsmith/agent/function/groq.py
+-rw-r--r--   0        0        0     8889 2024-05-07 11:14:54.558351 llmsmith-0.7.0/llmsmith/agent/function/openai.py
+-rw-r--r--   0        0        0        0 2024-04-23 05:43:58.075908 llmsmith-0.7.0/llmsmith/agent/function/options/__init__.py
+-rw-r--r--   0        0        0     1985 2024-05-07 12:01:42.276643 llmsmith-0.7.0/llmsmith/agent/function/options/openai.py
+-rw-r--r--   0        0        0        0 2024-04-18 05:26:07.193675 llmsmith-0.7.0/llmsmith/agent/tool/__init__.py
+-rw-r--r--   0        0        0      898 2024-05-06 11:04:31.823036 llmsmith-0.7.0/llmsmith/agent/tool/cohere.py
+-rw-r--r--   0        0        0     1014 2024-05-07 11:15:14.677758 llmsmith-0.7.0/llmsmith/agent/tool/gemini.py
+-rw-r--r--   0        0        0      941 2024-05-21 10:38:23.005648 llmsmith-0.7.0/llmsmith/agent/tool/groq.py
+-rw-r--r--   0        0        0     2002 2024-05-07 11:15:20.017868 llmsmith-0.7.0/llmsmith/agent/tool/openai.py
+-rw-r--r--   0        0        0        0 2024-03-14 11:47:53.187559 llmsmith-0.7.0/llmsmith/job/__init__.py
+-rw-r--r--   0        0        0     7428 2024-04-02 12:37:57.531013 llmsmith-0.7.0/llmsmith/job/base.py
+-rw-r--r--   0        0        0     8550 2024-04-03 05:58:40.426172 llmsmith-0.7.0/llmsmith/job/job.py
+-rw-r--r--   0        0        0        0 2024-04-30 12:02:50.437340 llmsmith-0.7.0/llmsmith/reranker/__init__.py
+-rw-r--r--   0        0        0      575 2024-05-02 04:19:45.995736 llmsmith-0.7.0/llmsmith/reranker/base.py
+-rw-r--r--   0        0        0     2849 2024-05-07 11:15:37.535755 llmsmith-0.7.0/llmsmith/reranker/cohere.py
+-rw-r--r--   0        0        0        0 2024-05-02 03:46:41.851482 llmsmith-0.7.0/llmsmith/reranker/options/__init__.py
+-rw-r--r--   0        0        0     1082 2024-05-07 11:15:49.065554 llmsmith-0.7.0/llmsmith/reranker/options/cohere.py
+-rw-r--r--   0        0        0        0 2024-03-14 11:03:16.994184 llmsmith-0.7.0/llmsmith/task/__init__.py
+-rw-r--r--   0        0        0     1329 2024-04-02 12:23:38.410395 llmsmith-0.7.0/llmsmith/task/base.py
+-rw-r--r--   0        0        0      431 2024-05-21 10:38:23.006615 llmsmith-0.7.0/llmsmith/task/models.py
+-rw-r--r--   0        0        0        0 2024-03-15 07:53:27.486482 llmsmith-0.7.0/llmsmith/task/retrieval/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-03 07:44:57.026421 llmsmith-0.7.0/llmsmith/task/retrieval/vector/__init__.py
+-rw-r--r--   0        0        0      437 2024-05-01 10:16:21.291906 llmsmith-0.7.0/llmsmith/task/retrieval/vector/base.py
+-rw-r--r--   0        0        0     3715 2024-05-07 11:16:01.033751 llmsmith-0.7.0/llmsmith/task/retrieval/vector/chromadb.py
+-rw-r--r--   0        0        0        0 2024-04-09 12:03:40.797998 llmsmith-0.7.0/llmsmith/task/retrieval/vector/options/__init__.py
+-rw-r--r--   0        0        0      897 2024-05-07 11:16:13.459211 llmsmith-0.7.0/llmsmith/task/retrieval/vector/options/chromadb.py
+-rw-r--r--   0        0        0     1157 2024-05-19 16:22:27.178379 llmsmith-0.7.0/llmsmith/task/retrieval/vector/options/pinecone.py
+-rw-r--r--   0        0        0     1316 2024-05-07 11:16:18.001301 llmsmith-0.7.0/llmsmith/task/retrieval/vector/options/qdrant.py
+-rw-r--r--   0        0        0     3856 2024-05-21 10:38:23.007671 llmsmith-0.7.0/llmsmith/task/retrieval/vector/pinecone.py
+-rw-r--r--   0        0        0     4295 2024-05-07 11:16:06.806987 llmsmith-0.7.0/llmsmith/task/retrieval/vector/qdrant.py
+-rw-r--r--   0        0        0        0 2024-03-15 11:22:26.459597 llmsmith-0.7.0/llmsmith/task/textgen/__init__.py
+-rw-r--r--   0        0        0     3036 2024-05-07 11:16:24.273688 llmsmith-0.7.0/llmsmith/task/textgen/claude.py
+-rw-r--r--   0        0        0     6170 2024-05-21 10:38:23.008580 llmsmith-0.7.0/llmsmith/task/textgen/cohere.py
+-rw-r--r--   0        0        0      681 2024-04-18 12:18:54.653626 llmsmith-0.7.0/llmsmith/task/textgen/errors.py
+-rw-r--r--   0        0        0     7201 2024-05-21 10:38:23.009587 llmsmith-0.7.0/llmsmith/task/textgen/gemini.py
+-rw-r--r--   0        0        0     6242 2024-05-21 10:38:23.010499 llmsmith-0.7.0/llmsmith/task/textgen/groq.py
+-rw-r--r--   0        0        0     6441 2024-05-21 10:38:23.011350 llmsmith-0.7.0/llmsmith/task/textgen/openai.py
+-rw-r--r--   0        0        0        0 2024-03-19 08:37:09.919088 llmsmith-0.7.0/llmsmith/task/textgen/options/__init__.py
+-rw-r--r--   0        0        0     1489 2024-05-07 11:16:43.800922 llmsmith-0.7.0/llmsmith/task/textgen/options/claude.py
+-rw-r--r--   0        0        0     2317 2024-05-07 12:16:46.722433 llmsmith-0.7.0/llmsmith/task/textgen/options/cohere.py
+-rw-r--r--   0        0        0     1337 2024-05-07 11:16:51.095809 llmsmith-0.7.0/llmsmith/task/textgen/options/gemini.py
+-rw-r--r--   0        0        0     1771 2024-05-21 10:38:23.012005 llmsmith-0.7.0/llmsmith/task/textgen/options/groq.py
+-rw-r--r--   0        0        0     1881 2024-05-07 11:16:55.681932 llmsmith-0.7.0/llmsmith/task/textgen/options/openai.py
+-rw-r--r--   0        0        0     2097 2024-05-21 10:42:10.953454 llmsmith-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     3545 1970-01-01 00:00:00.000000 llmsmith-0.7.0/PKG-INFO
```

### Comparing `llmsmith-0.6.0/LICENSE` & `llmsmith-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `llmsmith-0.6.0/README.md` & `llmsmith-0.7.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 - `openai`
 - `claude`
 - `gemini`
 - `chromadb`
 - `qdrant`
 - `cohere`
 - `pinecone`
+- `groq`
 - `all` (downloads all extra dependencies)
 
 ## Example
 
 Refer [this](https://llmsmith.readthedocs.io/en/latest/examples.html) page from the documentation to see examples on how LLMSmith can be used to build LLM powered functionalities.
 
 ## Documentation
```

### Comparing `llmsmith-0.6.0/llmsmith/agent/function/cohere.py` & `llmsmith-0.7.0/llmsmith/agent/function/cohere.py`

 * *Files 6% similar despite different names*

```diff
@@ -108,27 +108,27 @@
             raw_output: NonStreamedChatResponse = chat_response.raw_output
             chat_hist = raw_output.chat_history
             func_calls = chat_response.function_calls or {}
 
             # Exit condition: If no function calls are required.
             if not func_calls:
                 log.debug(
-                    f"CohereFunctionAgent turn-{turn+1} | Exiting agent loop with text output: f{chat_response.text}"
+                    f"CohereFunctionAgent turn-{turn+1} | Exiting agent loop with text output: {chat_response.text}"
                 )
                 return TaskOutput(
                     content=chat_response.text,
                     raw_output=chat_response.raw_output,
                 )
 
             log.debug(
                 f"CohereFunctionAgent turn-{turn+1} | Function call required: {func_calls}"
             )
 
             # Execute functions (tools)
-            for func_name, func in func_calls.items():
-                func_output = self._tool_callables[func_name](**func.args)
-                tool_call = ToolCall(name=func_name, parameters=func.args)
+            for _, func in func_calls.items():
+                func_output = self._tool_callables[func.name](**func.args)
+                tool_call = ToolCall(name=func.name, parameters=func.args)
                 func_results.append(
                     {"call": tool_call, "outputs": [{"answer": func_output}]}
                 )
 
         raise MaxTurnsReachedException()
```

### Comparing `llmsmith-0.6.0/llmsmith/agent/function/gemini.py` & `llmsmith-0.7.0/llmsmith/agent/function/gemini.py`

 * *Files 11% similar despite different names*

```diff
@@ -104,46 +104,46 @@
             )
 
             func_calls = chat_response.function_calls or {}
 
             # Exit condition: If no function calls are required.
             if not func_calls:
                 log.debug(
-                    f"GeminiFunctionAgent turn-{turn+1} | Exiting agent loop with text output: f{chat_response.text}"
+                    f"GeminiFunctionAgent turn-{turn+1} | Exiting agent loop with text output: {chat_response.text}"
                 )
                 return TaskOutput(
                     content=chat_response.text,
                     raw_output=chat_response.raw_output,
                 )
 
             log.debug(
                 f"GeminiFunctionAgent turn-{turn+1} | Function call required: {func_calls}"
             )
 
-            for func_name, func in func_calls.items():
-                func_output = self._tool_callables[func_name](**func.args)
+            for _, func in func_calls.items():
+                func_output = self._tool_callables[func.name](**func.args)
                 messages_payload.append(
                     {
                         "role": "function",
                         "parts": [
                             Part(
                                 function_call=FunctionCall(
-                                    name=func_name, args=func.args
+                                    name=func.name, args=func.args
                                 )
                             )
                         ],
                     }
                 )
                 messages_payload.append(
                     {
                         "role": "function",
                         "parts": [
                             Part(
                                 function_response=FunctionResponse(
-                                    name=func_name, response={"result": func_output}
+                                    name=func.name, response={"result": func_output}
                                 )
                             )
                         ],
                     }
                 )
 
         raise MaxTurnsReachedException()
```

### Comparing `llmsmith-0.6.0/llmsmith/agent/function/openai.py` & `llmsmith-0.7.0/llmsmith/agent/function/openai.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.6.0/llmsmith/agent/function/options/openai.py` & `llmsmith-0.7.0/llmsmith/agent/function/options/openai.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.6.0/llmsmith/agent/tool/cohere.py` & `llmsmith-0.7.0/llmsmith/agent/tool/cohere.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.6.0/llmsmith/agent/tool/gemini.py` & `llmsmith-0.7.0/llmsmith/agent/tool/gemini.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.6.0/llmsmith/agent/tool/openai.py` & `llmsmith-0.7.0/llmsmith/agent/tool/openai.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.6.0/llmsmith/job/base.py` & `llmsmith-0.7.0/llmsmith/job/base.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.6.0/llmsmith/job/job.py` & `llmsmith-0.7.0/llmsmith/job/job.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.6.0/llmsmith/reranker/base.py` & `llmsmith-0.7.0/llmsmith/reranker/base.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.6.0/llmsmith/reranker/cohere.py` & `llmsmith-0.7.0/llmsmith/reranker/cohere.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.6.0/llmsmith/reranker/options/cohere.py` & `llmsmith-0.7.0/llmsmith/reranker/options/cohere.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.6.0/llmsmith/task/base.py` & `llmsmith-0.7.0/llmsmith/task/base.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.6.0/llmsmith/task/retrieval/vector/chromadb.py` & `llmsmith-0.7.0/llmsmith/task/retrieval/vector/chromadb.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.6.0/llmsmith/task/retrieval/vector/options/chromadb.py` & `llmsmith-0.7.0/llmsmith/task/retrieval/vector/options/chromadb.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.6.0/llmsmith/task/retrieval/vector/options/pinecone.py` & `llmsmith-0.7.0/llmsmith/task/retrieval/vector/options/pinecone.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.6.0/llmsmith/task/retrieval/vector/options/qdrant.py` & `llmsmith-0.7.0/llmsmith/task/retrieval/vector/options/qdrant.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.6.0/llmsmith/task/retrieval/vector/pinecone.py` & `llmsmith-0.7.0/llmsmith/task/retrieval/vector/pinecone.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,18 +81,18 @@
         log.debug(
             f"Pinecone query request: input string: {task_input.content}\n OPTIONS: {query_options}"
         )
 
         embeddings = self.embedding_func([task_input.content])
 
         res: QueryResponse = self.index.query(
-            vector=embeddings,
-            include_metadata=True,
-            **query_options
+            vector=embeddings, include_metadata=True, **query_options
         )
 
-        docs = [doc.get("metadata", {}).get(self.text_field_name) for doc in res["matches"]]
+        docs = [
+            doc.get("metadata", {}).get(self.text_field_name) for doc in res["matches"]
+        ]
         if self._reranker:
             docs = await self._reranker.rerank(query=task_input.content, docs=docs)
 
         processed_res: str = self.doc_processing_func(docs)
         return TaskOutput(content=processed_res, raw_output=res)
```

### Comparing `llmsmith-0.6.0/llmsmith/task/retrieval/vector/qdrant.py` & `llmsmith-0.7.0/llmsmith/task/retrieval/vector/qdrant.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.6.0/llmsmith/task/textgen/claude.py` & `llmsmith-0.7.0/llmsmith/task/textgen/claude.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.6.0/llmsmith/task/textgen/cohere.py` & `llmsmith-0.7.0/llmsmith/task/textgen/cohere.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import logging
 from typing import List, Union
+from uuid import uuid4
 
 from llmsmith.task.textgen.errors import TextGenFailedException
 from llmsmith.task.textgen.options.cohere import CohereTextGenOptions
 
 try:
     import cohere
     from cohere.types.non_streamed_chat_response import NonStreamedChatResponse
@@ -88,22 +89,21 @@
 
         if llm_reply.finish_reason != "COMPLETE":
             raise TextGenFailedException(
                 "Failed to generate text",
                 failure_reason=self._block_reason_str(llm_reply),
             )
 
-        function_calls: dict[str, FunctionCall] = (
-            {
-                tool_call.name: FunctionCall(id=None, args=tool_call.parameters or {})
-                for tool_call in llm_reply.tool_calls
-            }
-            if llm_reply.tool_calls
-            else None
-        )
+        llm_tool_calls = llm_reply.tool_calls or []
+        function_calls: dict[str, FunctionCall] = {}
+        for tool_call in llm_tool_calls:
+            tool_id = str(uuid4())
+            function_calls[tool_id] = FunctionCall(
+                id=tool_id, name=tool_call.name, args=tool_call.parameters or {}
+            )
 
         log.debug(f"chat response output value: {llm_reply.text}")
 
         return ChatResponse(
             text=llm_reply.text, raw_output=llm_reply, function_calls=function_calls
         )
```

### Comparing `llmsmith-0.6.0/llmsmith/task/textgen/errors.py` & `llmsmith-0.7.0/llmsmith/task/textgen/errors.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.6.0/llmsmith/task/textgen/gemini.py` & `llmsmith-0.7.0/llmsmith/task/textgen/gemini.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import logging
 from typing import List, Union
+from uuid import uuid4
 
 from llmsmith.task.textgen.errors import PromptBlockedException, TextGenFailedException
 
 try:
     from google.ai.generativelanguage_v1beta.types.content import FunctionCall
     from google.generativeai import GenerativeModel
     from google.generativeai.types import GenerateContentResponse
@@ -105,20 +106,22 @@
                 for p in output_candidate.content.parts
                 if p.function_call
             ),
             None,
         )
 
         if function_call:
+            tool_id = str(uuid4())
             return ChatResponse(
                 text=None,
                 raw_output=llm_reply,
                 function_calls={
-                    function_call.name: LLMFunctionCall(
-                        id=None,
+                    tool_id: LLMFunctionCall(
+                        id=tool_id,
+                        name=function_call.name,
                         args={prop: val for prop, val in function_call.args.items()}
                         if function_call.args
                         else {},
                     )
                 },
             )
```

### Comparing `llmsmith-0.6.0/llmsmith/task/textgen/openai.py` & `llmsmith-0.7.0/llmsmith/task/textgen/openai.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,17 +55,17 @@
         messages_payload: List[ChatCompletionMessageParam],
         tools: Union[List[ChatCompletionToolParam], None] = None,
     ) -> ChatResponse:
         """
         Generates text using OpenAI LLM using the given input.
 
         :param messages_payload: The input messages for the chat.
-        :type messages_payload: List[:class:`openai.types.chat.chat_completion_tool_param.ChatCompletionMessageParam`]
+        :type messages_payload: List[:class:`openai.types.chat.chat_completion_message_param.ChatCompletionMessageParam`]
         :param tools: Tools (functions) which can be used by the LLM.
-        :type tools: List[:class:`openai.types.chat.chat_completion_tool_param.ChatCompletionMessageParam`], optional
+        :type tools: List[:class:`openai.types.chat.chat_completion_tool_param.ChatCompletionToolParam`], optional
         :raises TextGenFailedError: If AI fails to generate text based on the prompt.
         :returns: chat response from the LLM.
         :rtype: :class:`llmsmith.task.models.ChatResponse`
         """
         sys_prompt = (self.llm_options.get("system_prompt") or "").strip()
         sys_prompt_in_payload = next(
             (msg for msg in messages_payload if msg.get("role") == "system"), None
```

### Comparing `llmsmith-0.6.0/llmsmith/task/textgen/options/claude.py` & `llmsmith-0.7.0/llmsmith/task/textgen/options/claude.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.6.0/llmsmith/task/textgen/options/cohere.py` & `llmsmith-0.7.0/llmsmith/task/textgen/options/cohere.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.6.0/llmsmith/task/textgen/options/gemini.py` & `llmsmith-0.7.0/llmsmith/task/textgen/options/gemini.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.6.0/llmsmith/task/textgen/options/openai.py` & `llmsmith-0.7.0/llmsmith/task/textgen/options/openai.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.6.0/pyproject.toml` & `llmsmith-0.7.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "LLMSmith"
-version = "0.6.0"
+version = "0.7.0"
 description = "Lightweight Python library designed for developing functionalities powered by Large Language Models (LLMs)"
 authors = ["Dheeraj Gopinath <dheeraj.gopinath@gmail.com>"]
 readme = "README.md"
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
@@ -21,24 +21,26 @@
 onnxruntime = {version = "^1.17.1", optional = true}
 protobuf = {version = "3.20.3", optional = true}
 tokenizers = {version = "^0.15.2", optional = true}
 python-dotenv = "^1.0.1"
 qdrant-client = {version = "^1.8.2", optional = true}
 cohere = {version = "^5.3.2", optional = true}
 pinecone-client = {version = "^4.1.0", optional = true}
+groq = {version = "^0.6.0", optional = true}
 
 [tool.poetry.extras]
 openai = ["openai"]
 claude = ["anthropic"]
 gemini = ["google-generativeai"]
 chromadb = ["chromadb-client", "onnxruntime", "protobuf", "tokenizers"]
 qdrant = ["qdrant-client"]
 cohere = ["cohere"]
 pinecone = ["pinecone-client"]
-all = ["openai", "anthropic", "google-generativeai", "chromadb-client", "onnxruntime", "protobuf", "tokenizers", "qdrant-client", "cohere", "pinecone-client"]
+groq = ["groq"]
+all = ["openai", "anthropic", "google-generativeai", "chromadb-client", "onnxruntime", "protobuf", "tokenizers", "qdrant-client", "cohere", "pinecone-client", "groq"]
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.3.2"
 black = "^24.2.0"
```

### Comparing `llmsmith-0.6.0/PKG-INFO` & `llmsmith-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LLMSmith
-Version: 0.6.0
+Version: 0.7.0
 Summary: Lightweight Python library designed for developing functionalities powered by Large Language Models (LLMs)
 Author: Dheeraj Gopinath
 Author-email: dheeraj.gopinath@gmail.com
 Requires-Python: >=3.9,<3.13
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -16,21 +16,23 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: all
 Provides-Extra: chromadb
 Provides-Extra: claude
 Provides-Extra: cohere
 Provides-Extra: gemini
+Provides-Extra: groq
 Provides-Extra: openai
 Provides-Extra: pinecone
 Provides-Extra: qdrant
 Requires-Dist: anthropic (>=0.19.2,<0.20.0) ; extra == "claude" or extra == "all"
 Requires-Dist: chromadb-client (>=0.4.25.dev0,<0.5.0) ; extra == "chromadb" or extra == "all"
 Requires-Dist: cohere (>=5.3.2,<6.0.0) ; extra == "cohere" or extra == "all"
 Requires-Dist: google-generativeai (>=0.4.0,<0.5.0) ; extra == "gemini" or extra == "all"
+Requires-Dist: groq (>=0.6.0,<0.7.0) ; extra == "groq" or extra == "all"
 Requires-Dist: onnxruntime (>=1.17.1,<2.0.0) ; extra == "chromadb" or extra == "all"
 Requires-Dist: openai (>=1.23.2,<2.0.0) ; extra == "openai" or extra == "all"
 Requires-Dist: pinecone-client (>=4.1.0,<5.0.0) ; extra == "pinecone" or extra == "all"
 Requires-Dist: protobuf (==3.20.3) ; extra == "chromadb" or extra == "all"
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: qdrant-client (>=1.8.2,<2.0.0) ; extra == "qdrant" or extra == "all"
 Requires-Dist: tokenizers (>=0.15.2,<0.16.0) ; extra == "chromadb" or extra == "all"
@@ -58,14 +60,15 @@
 - `openai`
 - `claude`
 - `gemini`
 - `chromadb`
 - `qdrant`
 - `cohere`
 - `pinecone`
+- `groq`
 - `all` (downloads all extra dependencies)
 
 ## Example
 
 Refer [this](https://llmsmith.readthedocs.io/en/latest/examples.html) page from the documentation to see examples on how LLMSmith can be used to build LLM powered functionalities.
 
 ## Documentation
```

