# Comparing `tmp/openai_responses-0.3.2.tar.gz` & `tmp/openai_responses-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_responses-0.3.2.tar", max compression
+gzip compressed data, was "openai_responses-0.3.3.tar", max compression
```

## Comparing `openai_responses-0.3.2.tar` & `openai_responses-0.3.3.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0     1059 2024-05-16 18:41:10.309100 openai_responses-0.3.2/LICENSE
--rw-r--r--   0        0        0     3016 2024-05-14 18:14:24.699878 openai_responses-0.3.2/README.md
--rw-r--r--   0        0        0     1234 2024-05-20 16:24:51.334193 openai_responses-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      310 2024-05-03 15:30:48.556901 openai_responses-0.3.2/src/openai_responses/__init__.py
--rw-r--r--   0        0        0      606 2024-05-10 15:24:55.095526 openai_responses-0.3.2/src/openai_responses/_api.py
--rw-r--r--   0        0        0     1922 2024-05-20 16:30:34.412727 openai_responses-0.3.2/src/openai_responses/_mock.py
--rw-r--r--   0        0        0     3864 2024-05-13 15:32:42.633551 openai_responses-0.3.2/src/openai_responses/_routes/__init__.py
--rw-r--r--   0        0        0     5161 2024-05-14 17:51:42.173434 openai_responses-0.3.2/src/openai_responses/_routes/_base.py
--rw-r--r--   0        0        0     6208 2024-05-16 18:36:55.630698 openai_responses-0.3.2/src/openai_responses/_routes/assistants.py
--rw-r--r--   0        0        0     1123 2024-05-16 18:36:55.631029 openai_responses-0.3.2/src/openai_responses/_routes/chat.py
--rw-r--r--   0        0        0     1385 2024-05-16 18:36:55.631618 openai_responses-0.3.2/src/openai_responses/_routes/embeddings.py
--rw-r--r--   0        0        0     4978 2024-05-03 18:04:28.339502 openai_responses-0.3.2/src/openai_responses/_routes/files.py
--rw-r--r--   0        0        0     8041 2024-05-16 18:36:55.631992 openai_responses-0.3.2/src/openai_responses/_routes/messages.py
--rw-r--r--   0        0        0     3767 2024-05-13 15:31:22.122002 openai_responses-0.3.2/src/openai_responses/_routes/run_steps.py
--rw-r--r--   0        0        0    11511 2024-05-16 18:36:55.632301 openai_responses-0.3.2/src/openai_responses/_routes/runs.py
--rw-r--r--   0        0        0     5291 2024-05-16 18:36:55.632549 openai_responses-0.3.2/src/openai_responses/_routes/threads.py
--rw-r--r--   0        0        0       62 2024-05-02 16:25:57.355893 openai_responses-0.3.2/src/openai_responses/_stores/__init__.py
--rw-r--r--   0        0        0     6151 2024-05-16 18:37:01.157176 openai_responses-0.3.2/src/openai_responses/_stores/state_store.py
--rw-r--r--   0        0        0      233 2024-05-01 20:36:53.215071 openai_responses-0.3.2/src/openai_responses/_types/generics.py
--rw-r--r--   0        0        0     2354 2024-05-03 17:59:52.024893 openai_responses-0.3.2/src/openai_responses/_types/partials/assistants.py
--rw-r--r--   0        0        0     1590 2024-05-01 19:44:50.385563 openai_responses-0.3.2/src/openai_responses/_types/partials/chat.py
--rw-r--r--   0        0        0      525 2024-05-01 21:48:18.770982 openai_responses-0.3.2/src/openai_responses/_types/partials/embeddings.py
--rw-r--r--   0        0        0      837 2024-05-03 18:00:04.674371 openai_responses-0.3.2/src/openai_responses/_types/partials/files.py
--rw-r--r--   0        0        0     2628 2024-05-10 14:25:16.712414 openai_responses-0.3.2/src/openai_responses/_types/partials/messages.py
--rw-r--r--   0        0        0     2945 2024-05-13 15:43:24.432019 openai_responses-0.3.2/src/openai_responses/_types/partials/run_steps.py
--rw-r--r--   0        0        0     3805 2024-05-10 18:42:46.808227 openai_responses-0.3.2/src/openai_responses/_types/partials/runs.py
--rw-r--r--   0        0        0      832 2024-05-03 18:46:19.770456 openai_responses-0.3.2/src/openai_responses/_types/partials/threads.py
--rw-r--r--   0        0        0      186 2024-05-10 19:13:20.627809 openai_responses-0.3.2/src/openai_responses/_utils/copy.py
--rw-r--r--   0        0        0      199 2024-05-01 18:05:53.366742 openai_responses-0.3.2/src/openai_responses/_utils/faker.py
--rw-r--r--   0        0        0      627 2024-05-16 18:36:55.633057 openai_responses-0.3.2/src/openai_responses/_utils/serde.py
--rw-r--r--   0        0        0      108 2024-05-01 18:02:02.875630 openai_responses-0.3.2/src/openai_responses/_utils/time.py
--rw-r--r--   0        0        0      331 2024-05-10 15:48:24.334885 openai_responses-0.3.2/src/openai_responses/helpers/builders/_base.py
--rw-r--r--   0        0        0      489 2024-05-10 15:51:53.484991 openai_responses-0.3.2/src/openai_responses/helpers/builders/assistants.py
--rw-r--r--   0        0        0      527 2024-05-10 15:49:32.318317 openai_responses-0.3.2/src/openai_responses/helpers/builders/chat.py
--rw-r--r--   0        0        0      590 2024-05-10 15:50:34.652155 openai_responses-0.3.2/src/openai_responses/helpers/builders/embeddings.py
--rw-r--r--   0        0        0     1011 2024-05-13 15:26:15.980608 openai_responses-0.3.2/src/openai_responses/helpers/builders/messages.py
--rw-r--r--   0        0        0      563 2024-05-13 15:19:21.740278 openai_responses-0.3.2/src/openai_responses/helpers/builders/run_steps.py
--rw-r--r--   0        0        0      543 2024-05-13 14:41:41.519321 openai_responses-0.3.2/src/openai_responses/helpers/builders/runs.py
--rw-r--r--   0        0        0      456 2024-05-10 15:56:07.151021 openai_responses-0.3.2/src/openai_responses/helpers/builders/threads.py
--rw-r--r--   0        0        0      317 2024-05-20 16:30:34.412882 openai_responses-0.3.2/src/openai_responses/helpers/mergers/_base.py
--rw-r--r--   0        0        0      290 2024-05-20 16:30:34.413017 openai_responses-0.3.2/src/openai_responses/helpers/mergers/runs.py
--rw-r--r--   0        0        0     1271 2024-05-16 18:04:24.511337 openai_responses-0.3.2/src/openai_responses/helpers/state_store.py
--rw-r--r--   0        0        0      267 2024-05-03 18:11:52.021670 openai_responses-0.3.2/src/openai_responses/plugin.py
--rw-r--r--   0        0        0        0 2024-03-18 16:34:03.471292 openai_responses-0.3.2/src/openai_responses/py.typed
--rw-r--r--   0        0        0     3920 1970-01-01 00:00:00.000000 openai_responses-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1059 2024-05-16 18:41:10.309100 openai_responses-0.3.3/LICENSE
+-rw-r--r--   0        0        0     3016 2024-05-14 18:14:24.699878 openai_responses-0.3.3/README.md
+-rw-r--r--   0        0        0     1406 2024-05-20 20:54:09.217968 openai_responses-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0      310 2024-05-03 15:30:48.556901 openai_responses-0.3.3/src/openai_responses/__init__.py
+-rw-r--r--   0        0        0      606 2024-05-10 15:24:55.095526 openai_responses-0.3.3/src/openai_responses/_api.py
+-rw-r--r--   0        0        0     1922 2024-05-20 16:30:34.412727 openai_responses-0.3.3/src/openai_responses/_mock.py
+-rw-r--r--   0        0        0     3864 2024-05-13 15:32:42.633551 openai_responses-0.3.3/src/openai_responses/_routes/__init__.py
+-rw-r--r--   0        0        0     5161 2024-05-14 17:51:42.173434 openai_responses-0.3.3/src/openai_responses/_routes/_base.py
+-rw-r--r--   0        0        0     6208 2024-05-16 18:36:55.630698 openai_responses-0.3.3/src/openai_responses/_routes/assistants.py
+-rw-r--r--   0        0        0     1123 2024-05-16 18:36:55.631029 openai_responses-0.3.3/src/openai_responses/_routes/chat.py
+-rw-r--r--   0        0        0     1385 2024-05-16 18:36:55.631618 openai_responses-0.3.3/src/openai_responses/_routes/embeddings.py
+-rw-r--r--   0        0        0     4978 2024-05-03 18:04:28.339502 openai_responses-0.3.3/src/openai_responses/_routes/files.py
+-rw-r--r--   0        0        0     8041 2024-05-16 18:36:55.631992 openai_responses-0.3.3/src/openai_responses/_routes/messages.py
+-rw-r--r--   0        0        0     3767 2024-05-13 15:31:22.122002 openai_responses-0.3.3/src/openai_responses/_routes/run_steps.py
+-rw-r--r--   0        0        0    11511 2024-05-16 18:36:55.632301 openai_responses-0.3.3/src/openai_responses/_routes/runs.py
+-rw-r--r--   0        0        0     5291 2024-05-16 18:36:55.632549 openai_responses-0.3.3/src/openai_responses/_routes/threads.py
+-rw-r--r--   0        0        0       62 2024-05-02 16:25:57.355893 openai_responses-0.3.3/src/openai_responses/_stores/__init__.py
+-rw-r--r--   0        0        0     6151 2024-05-16 18:37:01.157176 openai_responses-0.3.3/src/openai_responses/_stores/state_store.py
+-rw-r--r--   0        0        0      233 2024-05-01 20:36:53.215071 openai_responses-0.3.3/src/openai_responses/_types/generics.py
+-rw-r--r--   0        0        0     2354 2024-05-03 17:59:52.024893 openai_responses-0.3.3/src/openai_responses/_types/partials/assistants.py
+-rw-r--r--   0        0        0     1590 2024-05-01 19:44:50.385563 openai_responses-0.3.3/src/openai_responses/_types/partials/chat.py
+-rw-r--r--   0        0        0      525 2024-05-01 21:48:18.770982 openai_responses-0.3.3/src/openai_responses/_types/partials/embeddings.py
+-rw-r--r--   0        0        0      837 2024-05-03 18:00:04.674371 openai_responses-0.3.3/src/openai_responses/_types/partials/files.py
+-rw-r--r--   0        0        0     2628 2024-05-10 14:25:16.712414 openai_responses-0.3.3/src/openai_responses/_types/partials/messages.py
+-rw-r--r--   0        0        0     2993 2024-05-20 20:53:53.219560 openai_responses-0.3.3/src/openai_responses/_types/partials/run_steps.py
+-rw-r--r--   0        0        0     3805 2024-05-10 18:42:46.808227 openai_responses-0.3.3/src/openai_responses/_types/partials/runs.py
+-rw-r--r--   0        0        0      832 2024-05-03 18:46:19.770456 openai_responses-0.3.3/src/openai_responses/_types/partials/threads.py
+-rw-r--r--   0        0        0      186 2024-05-10 19:13:20.627809 openai_responses-0.3.3/src/openai_responses/_utils/copy.py
+-rw-r--r--   0        0        0      199 2024-05-01 18:05:53.366742 openai_responses-0.3.3/src/openai_responses/_utils/faker.py
+-rw-r--r--   0        0        0      627 2024-05-16 18:36:55.633057 openai_responses-0.3.3/src/openai_responses/_utils/serde.py
+-rw-r--r--   0        0        0      108 2024-05-01 18:02:02.875630 openai_responses-0.3.3/src/openai_responses/_utils/time.py
+-rw-r--r--   0        0        0      331 2024-05-10 15:48:24.334885 openai_responses-0.3.3/src/openai_responses/helpers/builders/_base.py
+-rw-r--r--   0        0        0      489 2024-05-10 15:51:53.484991 openai_responses-0.3.3/src/openai_responses/helpers/builders/assistants.py
+-rw-r--r--   0        0        0      527 2024-05-10 15:49:32.318317 openai_responses-0.3.3/src/openai_responses/helpers/builders/chat.py
+-rw-r--r--   0        0        0      590 2024-05-10 15:50:34.652155 openai_responses-0.3.3/src/openai_responses/helpers/builders/embeddings.py
+-rw-r--r--   0        0        0     1011 2024-05-13 15:26:15.980608 openai_responses-0.3.3/src/openai_responses/helpers/builders/messages.py
+-rw-r--r--   0        0        0      563 2024-05-13 15:19:21.740278 openai_responses-0.3.3/src/openai_responses/helpers/builders/run_steps.py
+-rw-r--r--   0        0        0      543 2024-05-13 14:41:41.519321 openai_responses-0.3.3/src/openai_responses/helpers/builders/runs.py
+-rw-r--r--   0        0        0      456 2024-05-10 15:56:07.151021 openai_responses-0.3.3/src/openai_responses/helpers/builders/threads.py
+-rw-r--r--   0        0        0      317 2024-05-20 16:30:34.412882 openai_responses-0.3.3/src/openai_responses/helpers/mergers/_base.py
+-rw-r--r--   0        0        0      290 2024-05-20 16:30:34.413017 openai_responses-0.3.3/src/openai_responses/helpers/mergers/runs.py
+-rw-r--r--   0        0        0     1271 2024-05-16 18:04:24.511337 openai_responses-0.3.3/src/openai_responses/helpers/state_store.py
+-rw-r--r--   0        0        0      267 2024-05-03 18:11:52.021670 openai_responses-0.3.3/src/openai_responses/plugin.py
+-rw-r--r--   0        0        0        0 2024-03-18 16:34:03.471292 openai_responses-0.3.3/src/openai_responses/py.typed
+-rw-r--r--   0        0        0     4077 1970-01-01 00:00:00.000000 openai_responses-0.3.3/PKG-INFO
```

### Comparing `openai_responses-0.3.2/LICENSE` & `openai_responses-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.2/README.md` & `openai_responses-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.2/pyproject.toml` & `openai_responses-0.3.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 [tool.poetry]
 name = "openai-responses"
-version = "0.3.2"
+version = "0.3.3"
 description = "Automatically mock OpenAI requests"
 authors = ["Michael Harris <mharris@definite.app>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/mharrisb1/openai-responses-python"
 homepage = "https://mharrisb1.github.io/openai-responses-python/"
 documentation = "https://mharrisb1.github.io/openai-responses-python/"
 packages = [{ include = "openai_responses", from = "src" }]
+keywords = ["openai", "pytest", "testing"]
+classifiers = [
+  "Topic :: Software Development :: Testing :: Mocking",
+  "Topic :: Software Development :: Testing :: Unit",
+]
 
 [tool.poetry.plugins.pytest11]
 openai_responses = "openai_responses.plugin"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 openai = "^1.25"
```

### Comparing `openai_responses-0.3.2/src/openai_responses/_api.py` & `openai_responses-0.3.3/src/openai_responses/_api.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.2/src/openai_responses/_mock.py` & `openai_responses-0.3.3/src/openai_responses/_mock.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.2/src/openai_responses/_routes/__init__.py` & `openai_responses-0.3.3/src/openai_responses/_routes/__init__.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.2/src/openai_responses/_routes/_base.py` & `openai_responses-0.3.3/src/openai_responses/_routes/_base.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.2/src/openai_responses/_routes/assistants.py` & `openai_responses-0.3.3/src/openai_responses/_routes/assistants.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.2/src/openai_responses/_routes/chat.py` & `openai_responses-0.3.3/src/openai_responses/_routes/chat.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.2/src/openai_responses/_routes/embeddings.py` & `openai_responses-0.3.3/src/openai_responses/_routes/embeddings.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.2/src/openai_responses/_routes/files.py` & `openai_responses-0.3.3/src/openai_responses/_routes/files.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.2/src/openai_responses/_routes/messages.py` & `openai_responses-0.3.3/src/openai_responses/_routes/messages.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.2/src/openai_responses/_routes/run_steps.py` & `openai_responses-0.3.3/src/openai_responses/_routes/run_steps.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.2/src/openai_responses/_routes/runs.py` & `openai_responses-0.3.3/src/openai_responses/_routes/runs.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.2/src/openai_responses/_routes/threads.py` & `openai_responses-0.3.3/src/openai_responses/_routes/threads.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.2/src/openai_responses/_stores/state_store.py` & `openai_responses-0.3.3/src/openai_responses/_stores/state_store.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.2/src/openai_responses/_types/partials/assistants.py` & `openai_responses-0.3.3/src/openai_responses/_types/partials/assistants.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.2/src/openai_responses/_types/partials/chat.py` & `openai_responses-0.3.3/src/openai_responses/_types/partials/chat.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.2/src/openai_responses/_types/partials/embeddings.py` & `openai_responses-0.3.3/src/openai_responses/_types/partials/embeddings.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.2/src/openai_responses/_types/partials/files.py` & `openai_responses-0.3.3/src/openai_responses/_types/partials/files.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.2/src/openai_responses/_types/partials/messages.py` & `openai_responses-0.3.3/src/openai_responses/_types/partials/messages.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.2/src/openai_responses/_types/partials/run_steps.py` & `openai_responses-0.3.3/src/openai_responses/_types/partials/run_steps.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,21 +65,23 @@
 class PartialFunctionToolCall(TypedDict):
     id: str
     function: PartialFunction
     type: Literal["function"]
 
 
 class PartialToolCallsStepDetails(TypedDict):
-    tool_calls: Annotated[
-        Union[
-            PartialCodeInterpreterToolCall,
-            PartialFileSearchToolCall,
-            PartialFunctionToolCall,
-        ],
-        PropertyInfo(discriminator="type"),
+    tool_calls: List[
+        Annotated[
+            Union[
+                PartialCodeInterpreterToolCall,
+                PartialFileSearchToolCall,
+                PartialFunctionToolCall,
+            ],
+            PropertyInfo(discriminator="type"),
+        ]
     ]
     type: Literal["tool_calls"]
 
 
 class PartialUsage(TypedDict):
     completion_tokens: int
     prompt_tokens: int
```

### Comparing `openai_responses-0.3.2/src/openai_responses/_types/partials/runs.py` & `openai_responses-0.3.3/src/openai_responses/_types/partials/runs.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.2/src/openai_responses/_types/partials/threads.py` & `openai_responses-0.3.3/src/openai_responses/_types/partials/threads.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.2/src/openai_responses/_utils/serde.py` & `openai_responses-0.3.3/src/openai_responses/_utils/serde.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.2/src/openai_responses/helpers/builders/chat.py` & `openai_responses-0.3.3/src/openai_responses/helpers/builders/chat.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.2/src/openai_responses/helpers/builders/embeddings.py` & `openai_responses-0.3.3/src/openai_responses/helpers/builders/embeddings.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.2/src/openai_responses/helpers/builders/messages.py` & `openai_responses-0.3.3/src/openai_responses/helpers/builders/messages.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.2/src/openai_responses/helpers/builders/run_steps.py` & `openai_responses-0.3.3/src/openai_responses/helpers/builders/run_steps.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.2/src/openai_responses/helpers/builders/runs.py` & `openai_responses-0.3.3/src/openai_responses/helpers/builders/runs.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.2/src/openai_responses/helpers/state_store.py` & `openai_responses-0.3.3/src/openai_responses/helpers/state_store.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.2/PKG-INFO` & `openai_responses-0.3.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 Metadata-Version: 2.1
 Name: openai-responses
-Version: 0.3.2
+Version: 0.3.3
 Summary: Automatically mock OpenAI requests
 Home-page: https://mharrisb1.github.io/openai-responses-python/
 License: MIT
+Keywords: openai,pytest,testing
 Author: Michael Harris
 Author-email: mharris@definite.app
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Software Development :: Testing :: Mocking
+Classifier: Topic :: Software Development :: Testing :: Unit
 Requires-Dist: faker-openai-api-provider (>=0.1.0,<0.2.0)
 Requires-Dist: openai (>=1.25,<2.0)
 Requires-Dist: respx (>=0.20.2,<0.21.0)
 Project-URL: Documentation, https://mharrisb1.github.io/openai-responses-python/
 Project-URL: Repository, https://github.com/mharrisb1/openai-responses-python
 Description-Content-Type: text/markdown
```

