# Comparing `tmp/rag_assistant-0.1.8.tar.gz` & `tmp/rag_assistant-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rag_assistant-0.1.8.tar", last modified: Fri May 17 04:20:58 2024, max compression
+gzip compressed data, was "rag_assistant-0.1.9.tar", last modified: Fri May 17 20:53:04 2024, max compression
```

## Comparing `rag_assistant-0.1.8.tar` & `rag_assistant-0.1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 04:20:58.001101 rag_assistant-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-17 04:20:58.001101 rag_assistant-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-17 04:20:45.000000 rag_assistant-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 04:20:58.001101 rag_assistant-0.1.8/rag_assistant/
--rw-r--r--   0 runner    (1001) docker     (127)    18841 2024-05-17 04:20:45.000000 rag_assistant-0.1.8/rag_assistant/RagAssistant.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-17 04:20:45.000000 rag_assistant-0.1.8/rag_assistant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 04:20:58.001101 rag_assistant-0.1.8/rag_assistant.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-17 04:20:57.000000 rag_assistant-0.1.8/rag_assistant.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-17 04:20:57.000000 rag_assistant-0.1.8/rag_assistant.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 04:20:57.000000 rag_assistant-0.1.8/rag_assistant.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-17 04:20:57.000000 rag_assistant-0.1.8/rag_assistant.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-17 04:20:57.000000 rag_assistant-0.1.8/rag_assistant.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-17 04:20:57.000000 rag_assistant-0.1.8/rag_assistant.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 04:20:58.001101 rag_assistant-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-17 04:20:45.000000 rag_assistant-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:53:04.779101 rag_assistant-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-17 20:53:04.779101 rag_assistant-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-17 20:52:57.000000 rag_assistant-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:53:04.775101 rag_assistant-0.1.9/rag_assistant/
+-rw-r--r--   0 runner    (1001) docker     (127)    18902 2024-05-17 20:52:57.000000 rag_assistant-0.1.9/rag_assistant/RagAssistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-17 20:52:57.000000 rag_assistant-0.1.9/rag_assistant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:53:04.779101 rag_assistant-0.1.9/rag_assistant.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-17 20:53:04.000000 rag_assistant-0.1.9/rag_assistant.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-17 20:53:04.000000 rag_assistant-0.1.9/rag_assistant.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 20:53:04.000000 rag_assistant-0.1.9/rag_assistant.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-17 20:53:04.000000 rag_assistant-0.1.9/rag_assistant.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-17 20:53:04.000000 rag_assistant-0.1.9/rag_assistant.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-17 20:53:04.000000 rag_assistant-0.1.9/rag_assistant.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 20:53:04.779101 rag_assistant-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-17 20:52:57.000000 rag_assistant-0.1.9/setup.py
```

### Comparing `rag_assistant-0.1.8/PKG-INFO` & `rag_assistant-0.1.9/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rag_assistant
-Version: 0.1.8
+Version: 0.1.9
 Summary: The Swarmauri Rag Assistant is part of the swarmaURI framework.
 Home-page: http://github.com/swarmauri/rag_assistant
 Author: Jacob Stewart
 Author-email: corporate@swarmauri.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
@@ -16,14 +16,14 @@
 # Swarmauri Rag Assistant
 
 ## Overview
 The Swarmauri Rag Assistant
 
 ## Installation
 ```bash
-pip install rag_assistant==0.1.8 --user
+pip install rag_assistant==0.1.9 --user
 ```
 
 ## Execution
 ```bash
 ! rag_assistant --api_key "YOUR API KEY" --db_path "E:\swarmauri_github/prompt_responses.db" --system_context "You are a helpful assistant."
 ```
```

### Comparing `rag_assistant-0.1.8/rag_assistant/RagAssistant.py` & `rag_assistant-0.1.9/rag_assistant/RagAssistant.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,14 +45,15 @@
                             'mistral_mistral-small-latest',
                             'mistral_open-mixtral-8x22b',
                             'mistral_open-mixtral-8x7b',
                             'mistral_open-mistral-7b',
                             'mistral_mistral-large-latest',
                             'openai_gpt-3.5-turbo',
                             'openai_gpt-3.5-turbo-16k',
+                            'openai_gpt-3.5-turbo-16k-0613',
                             'openai_gpt-4-0125-preview',
                             'openai_gpt-4o',
                             'google_gemini-1.5-pro-latest',
                             'anthropic_claude-2.0',
                             'anthropic_claude-instant-1.2',
                             'anthropic_claude-2.1',
                             'anthropic_claude-3-opus-20240229',
```

### Comparing `rag_assistant-0.1.8/rag_assistant.egg-info/PKG-INFO` & `rag_assistant-0.1.9/rag_assistant.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rag_assistant
-Version: 0.1.8
+Version: 0.1.9
 Summary: The Swarmauri Rag Assistant is part of the swarmaURI framework.
 Home-page: http://github.com/swarmauri/rag_assistant
 Author: Jacob Stewart
 Author-email: corporate@swarmauri.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
@@ -16,14 +16,14 @@
 # Swarmauri Rag Assistant
 
 ## Overview
 The Swarmauri Rag Assistant
 
 ## Installation
 ```bash
-pip install rag_assistant==0.1.8 --user
+pip install rag_assistant==0.1.9 --user
 ```
 
 ## Execution
 ```bash
 ! rag_assistant --api_key "YOUR API KEY" --db_path "E:\swarmauri_github/prompt_responses.db" --system_context "You are a helpful assistant."
 ```
```

### Comparing `rag_assistant-0.1.8/setup.py` & `rag_assistant-0.1.9/setup.py`

 * *Files identical despite different names*

