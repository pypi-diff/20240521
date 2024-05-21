# Comparing `tmp/modelmerge-0.5.4.tar.gz` & `tmp/modelmerge-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelmerge-0.5.4.tar", last modified: Mon May 20 05:24:30 2024, max compression
+gzip compressed data, was "modelmerge-0.5.5.tar", last modified: Tue May 21 07:05:39 2024, max compression
```

## Comparing `modelmerge-0.5.4.tar` & `modelmerge-0.5.5.tar`

### file list

```diff
@@ -1,57 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:24:30.865737 modelmerge-0.5.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-20 05:24:21.000000 modelmerge-0.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-20 05:24:30.865737 modelmerge-0.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-05-20 05:24:21.000000 modelmerge-0.5.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 05:24:30.865737 modelmerge-0.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-20 05:24:21.000000 modelmerge-0.5.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:24:30.857737 modelmerge-0.5.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:24:30.857737 modelmerge-0.5.4/src/ModelMerge/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 05:24:21.000000 modelmerge-0.5.4/src/ModelMerge/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:24:30.861737 modelmerge-0.5.4/src/ModelMerge/models/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-20 05:24:21.000000 modelmerge-0.5.4/src/ModelMerge/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31091 2024-05-20 05:24:21.000000 modelmerge-0.5.4/src/ModelMerge/models/chatgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)    20892 2024-05-20 05:24:21.000000 modelmerge-0.5.4/src/ModelMerge/models/claude.py
--rw-r--r--   0 runner    (1001) docker     (127)     8808 2024-05-20 05:24:21.000000 modelmerge-0.5.4/src/ModelMerge/models/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5987 2024-05-20 05:24:21.000000 modelmerge-0.5.4/src/ModelMerge/models/genimi.py
--rw-r--r--   0 runner    (1001) docker     (127)     5989 2024-05-20 05:24:21.000000 modelmerge-0.5.4/src/ModelMerge/models/groq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:24:30.861737 modelmerge-0.5.4/src/ModelMerge/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-20 05:24:21.000000 modelmerge-0.5.4/src/ModelMerge/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-05-20 05:24:21.000000 modelmerge-0.5.4/src/ModelMerge/plugins/image.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-20 05:24:21.000000 modelmerge-0.5.4/src/ModelMerge/plugins/run_python.py
--rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-05-20 05:24:21.000000 modelmerge-0.5.4/src/ModelMerge/plugins/tarvel.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-20 05:24:21.000000 modelmerge-0.5.4/src/ModelMerge/plugins/today.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-20 05:24:21.000000 modelmerge-0.5.4/src/ModelMerge/plugins/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    11903 2024-05-20 05:24:21.000000 modelmerge-0.5.4/src/ModelMerge/plugins/websearch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:24:30.861737 modelmerge-0.5.4/src/ModelMerge/tools/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-20 05:24:21.000000 modelmerge-0.5.4/src/ModelMerge/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3576 2024-05-20 05:24:21.000000 modelmerge-0.5.4/src/ModelMerge/tools/chatgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-20 05:24:21.000000 modelmerge-0.5.4/src/ModelMerge/tools/claude.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:24:30.861737 modelmerge-0.5.4/src/ModelMerge/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 05:24:21.000000 modelmerge-0.5.4/src/ModelMerge/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8453 2024-05-20 05:24:21.000000 modelmerge-0.5.4/src/ModelMerge/utils/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-05-20 05:24:21.000000 modelmerge-0.5.4/src/ModelMerge/utils/scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:24:30.865737 modelmerge-0.5.4/src/modelmerge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-20 05:24:30.000000 modelmerge-0.5.4/src/modelmerge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-20 05:24:30.000000 modelmerge-0.5.4/src/modelmerge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 05:24:30.000000 modelmerge-0.5.4/src/modelmerge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-20 05:24:30.000000 modelmerge-0.5.4/src/modelmerge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-20 05:24:30.000000 modelmerge-0.5.4/src/modelmerge.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:24:30.865737 modelmerge-0.5.4/test/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-20 05:24:21.000000 modelmerge-0.5.4/test/test.py
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-20 05:24:21.000000 modelmerge-0.5.4/test/test_API.py
--rw-r--r--   0 runner    (1001) docker     (127)     9792 2024-05-20 05:24:21.000000 modelmerge-0.5.4/test/test_Web_crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-20 05:24:21.000000 modelmerge-0.5.4/test/test_claude_zh_char.py
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-20 05:24:21.000000 modelmerge-0.5.4/test/test_ddg_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-20 05:24:21.000000 modelmerge-0.5.4/test/test_download_pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-20 05:24:21.000000 modelmerge-0.5.4/test/test_get_token_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-20 05:24:21.000000 modelmerge-0.5.4/test/test_google_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-20 05:24:21.000000 modelmerge-0.5.4/test/test_jieba.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-20 05:24:21.000000 modelmerge-0.5.4/test/test_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     9066 2024-05-20 05:24:21.000000 modelmerge-0.5.4/test/test_langchain_search_old.py
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-20 05:24:21.000000 modelmerge-0.5.4/test/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-05-20 05:24:21.000000 modelmerge-0.5.4/test/test_ollama.py
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-20 05:24:21.000000 modelmerge-0.5.4/test/test_py_run.py
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-20 05:24:21.000000 modelmerge-0.5.4/test/test_tikitoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-05-20 05:24:21.000000 modelmerge-0.5.4/test/test_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-20 05:24:21.000000 modelmerge-0.5.4/test/test_url.py
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-20 05:24:21.000000 modelmerge-0.5.4/test/test_whisper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:05:39.339171 modelmerge-0.5.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-21 07:05:30.000000 modelmerge-0.5.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-21 07:05:39.339171 modelmerge-0.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-05-21 07:05:30.000000 modelmerge-0.5.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 07:05:39.339171 modelmerge-0.5.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-21 07:05:30.000000 modelmerge-0.5.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:05:39.331171 modelmerge-0.5.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:05:39.331171 modelmerge-0.5.5/src/ModelMerge/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 07:05:30.000000 modelmerge-0.5.5/src/ModelMerge/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:05:39.331171 modelmerge-0.5.5/src/ModelMerge/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-21 07:05:30.000000 modelmerge-0.5.5/src/ModelMerge/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26007 2024-05-21 07:05:30.000000 modelmerge-0.5.5/src/ModelMerge/models/chatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16005 2024-05-21 07:05:30.000000 modelmerge-0.5.5/src/ModelMerge/models/claude.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9130 2024-05-21 07:05:30.000000 modelmerge-0.5.5/src/ModelMerge/models/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5987 2024-05-21 07:05:30.000000 modelmerge-0.5.5/src/ModelMerge/models/genimi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5989 2024-05-21 07:05:30.000000 modelmerge-0.5.5/src/ModelMerge/models/groq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:05:39.331171 modelmerge-0.5.5/src/ModelMerge/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-21 07:05:30.000000 modelmerge-0.5.5/src/ModelMerge/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-05-21 07:05:30.000000 modelmerge-0.5.5/src/ModelMerge/plugins/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-21 07:05:30.000000 modelmerge-0.5.5/src/ModelMerge/plugins/run_python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-05-21 07:05:30.000000 modelmerge-0.5.5/src/ModelMerge/plugins/tarvel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-21 07:05:30.000000 modelmerge-0.5.5/src/ModelMerge/plugins/today.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-21 07:05:30.000000 modelmerge-0.5.5/src/ModelMerge/plugins/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11903 2024-05-21 07:05:30.000000 modelmerge-0.5.5/src/ModelMerge/plugins/websearch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:05:39.335171 modelmerge-0.5.5/src/ModelMerge/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-21 07:05:30.000000 modelmerge-0.5.5/src/ModelMerge/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3576 2024-05-21 07:05:30.000000 modelmerge-0.5.5/src/ModelMerge/tools/chatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-21 07:05:30.000000 modelmerge-0.5.5/src/ModelMerge/tools/claude.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-05-21 07:05:30.000000 modelmerge-0.5.5/src/ModelMerge/tools/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:05:39.335171 modelmerge-0.5.5/src/ModelMerge/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 07:05:30.000000 modelmerge-0.5.5/src/ModelMerge/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8453 2024-05-21 07:05:30.000000 modelmerge-0.5.5/src/ModelMerge/utils/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-05-21 07:05:30.000000 modelmerge-0.5.5/src/ModelMerge/utils/scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:05:39.339171 modelmerge-0.5.5/src/modelmerge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-21 07:05:39.000000 modelmerge-0.5.5/src/modelmerge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-21 07:05:39.000000 modelmerge-0.5.5/src/modelmerge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 07:05:39.000000 modelmerge-0.5.5/src/modelmerge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-21 07:05:39.000000 modelmerge-0.5.5/src/modelmerge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-21 07:05:39.000000 modelmerge-0.5.5/src/modelmerge.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:05:39.339171 modelmerge-0.5.5/test/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-21 07:05:30.000000 modelmerge-0.5.5/test/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-21 07:05:30.000000 modelmerge-0.5.5/test/test_API.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9792 2024-05-21 07:05:30.000000 modelmerge-0.5.5/test/test_Web_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-21 07:05:30.000000 modelmerge-0.5.5/test/test_claude_zh_char.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-21 07:05:30.000000 modelmerge-0.5.5/test/test_ddg_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-21 07:05:30.000000 modelmerge-0.5.5/test/test_download_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-21 07:05:30.000000 modelmerge-0.5.5/test/test_get_token_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-21 07:05:30.000000 modelmerge-0.5.5/test/test_google_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-21 07:05:30.000000 modelmerge-0.5.5/test/test_jieba.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-21 07:05:30.000000 modelmerge-0.5.5/test/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9066 2024-05-21 07:05:30.000000 modelmerge-0.5.5/test/test_langchain_search_old.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-21 07:05:30.000000 modelmerge-0.5.5/test/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-05-21 07:05:30.000000 modelmerge-0.5.5/test/test_ollama.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-21 07:05:30.000000 modelmerge-0.5.5/test/test_py_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-21 07:05:30.000000 modelmerge-0.5.5/test/test_tikitoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-05-21 07:05:30.000000 modelmerge-0.5.5/test/test_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-21 07:05:30.000000 modelmerge-0.5.5/test/test_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-21 07:05:30.000000 modelmerge-0.5.5/test/test_whisper.py
```

### Comparing `modelmerge-0.5.4/LICENSE` & `modelmerge-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.4/PKG-INFO` & `modelmerge-0.5.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelmerge
-Version: 0.5.4
+Version: 0.5.5
 Summary: modelmerge is a multi-large language model API aggregator.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: lxml
 Requires-Dist: PyExecJS
 Requires-Dist: requests
 Requires-Dist: pdfminer.six
```

### Comparing `modelmerge-0.5.4/README.md` & `modelmerge-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.4/src/ModelMerge/models/chatgpt.py` & `modelmerge-0.5.5/src/ModelMerge/models/chatgpt.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 import os
 import re
 import json
 import copy
 from pathlib import Path
 from typing import AsyncGenerator, Set
-from .config import BaseLLM, PLUGINS, LANGUAGE
 
 import httpx
 import requests
 import tiktoken
 
-# import config
-from ..utils.scripts import check_json, cut_message
-from ..utils.prompt import search_key_word_prompt
-from ..tools.chatgpt import function_call_list
-from ..plugins import *
+from .config import BaseLLM, PLUGINS
+from ..utils.scripts import check_json
+from ..tools import get_tools_result, function_call_list
 
 def get_filtered_keys_from_object(obj: object, *keys: str) -> Set[str]:
     """
     Get filtered list of object variable names.
     :param keys: List of keys to include. If the first key is "not", the remaining keys will be removed from the class keys.
     :return: List of class keys.
     """
@@ -53,19 +50,20 @@
         max_tokens: int = None,
         temperature: float = 0.5,
         top_p: float = 1.0,
         presence_penalty: float = 0.0,
         frequency_penalty: float = 0.0,
         reply_count: int = 1,
         truncate_limit: int = None,
+        use_plugins: bool = True,
     ) -> None:
         """
         Initialize Chatbot with API key (from https://platform.openai.com/account/api-keys)
         """
-        super().__init__(api_key, engine, api_url, system_prompt, proxy, timeout, max_tokens, temperature, top_p, presence_penalty, frequency_penalty, reply_count, truncate_limit)
+        super().__init__(api_key, engine, api_url, system_prompt, proxy, timeout, max_tokens, temperature, top_p, presence_penalty, frequency_penalty, reply_count, truncate_limit, use_plugins=use_plugins)
         self.max_tokens: int = max_tokens or (
             4096
             if "gpt-4-1106-preview" in engine or "gpt-4-0125-preview" in engine or "gpt-4-turbo" in engine or "gpt-3.5-turbo-1106" in engine or "claude" in engine or "gpt-4o" in engine
             else 31000
             if "gpt-4-32k" in engine
             else 7000
             if "gpt-4" in engine
@@ -206,14 +204,15 @@
             num_tokens += 5
             for key, value in message.items():
                 values = list(self.extract_values(value))
                 if "image_url" in values:
                     continue
                 if values:
                     for value in values:
+                        # print("value", value)
                         num_tokens += len(encoding.encode(value))
                 if key == "name":  # if there's a name, the role is omitted
                     num_tokens += 5  # role is always required and always 1 token
         num_tokens += 5  # every reply is primed with <im_start>assistant
         return num_tokens
 
     def get_message_token(self, url, json_post):
@@ -284,15 +283,15 @@
                 "frequency_penalty",
                 self.frequency_penalty,
             ),
             "n": kwargs.get("n", self.reply_count),
             "user": role,
         }
         json_post_body.update(copy.deepcopy(body))
-        if all(value == False for value in PLUGINS.values()):
+        if all(value == False for value in PLUGINS.values()) or self.use_plugins == False:
             return json_post_body
         json_post_body.update(copy.deepcopy(function_call_list["base"]))
         for item in PLUGINS.keys():
             try:
                 # print(item, PLUGINS[item])
                 if PLUGINS[item]:
                     json_post_body["functions"].append(function_call_list[item])
@@ -428,65 +427,15 @@
             else:
                 self.function_calls_counter[function_call_name] += 1
             if self.function_calls_counter[function_call_name] <= self.function_call_max_loop:
                 function_call_max_tokens = self.truncate_limit - message_token["total"] - 1000
                 if function_call_max_tokens <= 0:
                     function_call_max_tokens = int(self.truncate_limit / 2)
                 print("\033[32m function_call", function_call_name, "max token:", function_call_max_tokens, "\033[0m")
-                if function_call_name == "get_search_results":
-                    prompt = json.loads(function_full_response)["prompt"]
-                    yield "🌐 正在搜索您的问题，提取关键词..."
-                    llm = BaseLLM(api_key=self.api_key, api_url=self.api_url.source_api_url , engine=self.engine, system_prompt=self.system_prompt)
-                    keywords = llm.ask(search_key_word_prompt.format(source=prompt)).split("\n")
-                    function_response = yield from eval(function_call_name)(prompt, keywords)
-                    function_call_max_tokens = 32000
-                    function_response, text_len = cut_message(function_response, function_call_max_tokens, self.engine)
-                    if function_response:
-                        function_response = (
-                            f"You need to response the following question: {prompt}. Search results is provided inside <Search_results></Search_results> XML tags. Your task is to think about the question step by step and then answer the above question in {LANGUAGE} based on the Search results provided. Please response in {LANGUAGE} and adopt a style that is logical, in-depth, and detailed. Note: In order to make the answer appear highly professional, you should be an expert in textual analysis, aiming to make the answer precise and comprehensive. Directly response markdown format, without using markdown code blocks"
-                            "Here is the Search results, inside <Search_results></Search_results> XML tags:"
-                            "<Search_results>"
-                            "{}"
-                            "</Search_results>"
-                        ).format(function_response)
-                    else:
-                        function_response = "无法找到相关信息，停止使用 tools"
-                    # user_prompt = f"You need to response the following question: {prompt}. Search results is provided inside <Search_results></Search_results> XML tags. Your task is to think about the question step by step and then answer the above question in {config.LANGUAGE} based on the Search results provided. Please response in {config.LANGUAGE} and adopt a style that is logical, in-depth, and detailed. Note: In order to make the answer appear highly professional, you should be an expert in textual analysis, aiming to make the answer precise and comprehensive. Directly response markdown format, without using markdown code blocks"
-                    # self.add_to_conversation(user_prompt, "user", convo_id=convo_id)
-                if function_call_name == "get_url_content":
-                    url = json.loads(function_full_response)["url"]
-                    print("\n\nurl", url)
-                    # function_response = jina_ai_Web_crawler(url)
-                    function_response = Web_crawler(url)
-                    function_response, text_len = cut_message(function_response, function_call_max_tokens, self.engine)
-                if function_call_name == "get_city_tarvel_info":
-                    city = json.loads(function_full_response)["city"]
-                    function_response = eval(function_call_name)(city)
-                    function_response, text_len = cut_message(function_response, function_call_max_tokens, self.engine)
-                    function_response = (
-                        f"You need to response the following question: {city}. Tarvel infomation is provided inside <infomation></infomation> XML tags. Your task is to think about the question step by step and then answer the above question in {LANGUAGE} based on the tarvel infomation provided. Please response in {LANGUAGE} and adopt a style that is logical, in-depth, and detailed. Note: In order to make the answer appear highly professional, you should be an expert in textual analysis, aiming to make the answer precise and comprehensive."
-                        "Here is the tarvel infomation, inside <infomation></infomation> XML tags:"
-                        "<infomation>"
-                        "{}"
-                        "</infomation>"
-                    ).format(function_response)
-                if function_call_name == "generate_image":
-                    prompt = json.loads(function_full_response)["prompt"]
-                    function_response = eval(function_call_name)(prompt)
-                    function_response, text_len = cut_message(function_response, function_call_max_tokens, self.engine)
-                if function_call_name == "run_python_script":
-                    prompt = json.loads(function_full_response)["prompt"]
-                    function_response = eval(function_call_name)(prompt)
-                    function_response, text_len = cut_message(function_response, function_call_max_tokens, self.engine)
-                if function_call_name == "get_date_time_weekday":
-                    function_response = eval(function_call_name)()
-                    function_response, text_len = cut_message(function_response, function_call_max_tokens, self.engine)
-                if function_call_name == "get_version_info":
-                    function_response = eval(function_call_name)()
-                    function_response, text_len = cut_message(function_response, function_call_max_tokens, self.engine)
+                function_response = yield from get_tools_result(function_call_name, function_full_response, function_call_max_tokens, self.engine, chatgpt, self.api_key, self.api_url, use_plugins=False)
             else:
                 function_response = "无法找到相关信息，停止使用 tools"
             response_role = "function"
             # print(self.conversation[convo_id][-1])
             if self.conversation[convo_id][-1]["role"] == "function" and self.conversation[convo_id][-1]["name"] == "get_search_results":
                 mess = self.conversation[convo_id].pop(-1)
                 # print("Truncate message:", mess)
```

### Comparing `modelmerge-0.5.4/src/ModelMerge/models/claude.py` & `modelmerge-0.5.5/src/ModelMerge/models/claude.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 import os
 import json
 import copy
 import tiktoken
 import requests
 
-from .config import BaseLLM, PLUGINS, LANGUAGE
-from ..tools.claude import claude_tools_list
-from ..utils.scripts import check_json, cut_message
-from ..utils.prompt import search_key_word_prompt
-from ..plugins import *
-
-
+from .config import BaseLLM, PLUGINS
+from ..utils.scripts import check_json
+from ..tools import get_tools_result, claude_tools_list
 
 class claudeConversation(dict):
     def Conversation(self, index):
         conversation_list = super().__getitem__(index)
         return "\n\n" + "\n\n".join([f"{item['role']}:{item['content']}" for item in conversation_list]) + "\n\nAssistant:"
 
 class claude(BaseLLM):
@@ -23,16 +19,17 @@
         api_key: str,
         engine: str = os.environ.get("GPT_ENGINE") or "claude-2.1",
         api_url: str = "https://api.anthropic.com/v1/complete",
         system_prompt: str = "You are ChatGPT, a large language model trained by OpenAI. Respond conversationally",
         temperature: float = 0.5,
         top_p: float = 0.7,
         timeout: float = 20,
+        use_plugins: bool = True,
     ):
-        super().__init__(api_key, engine, api_url, system_prompt, timeout=timeout, temperature=temperature, top_p=top_p)
+        super().__init__(api_key, engine, api_url, system_prompt, timeout=timeout, temperature=temperature, top_p=top_p, use_plugins=use_plugins)
         # self.api_url = api_url
         self.conversation = claudeConversation()
 
     def add_to_conversation(
         self,
         message: str,
         role: str,
@@ -164,17 +161,17 @@
         api_key: str,
         engine: str = os.environ.get("GPT_ENGINE") or "claude-3-opus-20240229",
         api_url: str = "https://api.anthropic.com/v1/messages",
         system_prompt: str = "You are ChatGPT, a large language model trained by OpenAI. Respond conversationally",
         temperature: float = 0.5,
         timeout: float = 20,
         top_p: float = 0.7,
+        use_plugins: bool = True,
     ):
-        super().__init__(api_key, engine, api_url, system_prompt, timeout=timeout, temperature=temperature, top_p=top_p)
-        self.api_url = api_url
+        super().__init__(api_key, engine, api_url, system_prompt, timeout=timeout, temperature=temperature, top_p=top_p, use_plugins=use_plugins)
         self.conversation: dict[str, list[dict]] = {
             "default": [],
         }
 
     def add_to_conversation(
         self,
         message: str,
@@ -275,15 +272,15 @@
         pass_history = True
         if convo_id not in self.conversation or pass_history == False:
             self.reset(convo_id=convo_id)
         self.add_to_conversation(prompt, role, convo_id=convo_id, tools_id=tools_id, total_tokens=total_tokens, function_name=function_name, function_full_response=function_full_response)
         # self.__truncate_conversation(convo_id=convo_id)
         # print(self.conversation[convo_id])
 
-        url = self.api_url
+        url = self.api_url.source_api_url
         headers = {
             "content-type": "application/json",
             "x-api-key": f"{kwargs.get('api_key', self.api_key)}",
             "anthropic-version": "2023-06-01",
             "anthropic-beta": "tools-2024-05-16"
         }
 
@@ -296,15 +293,15 @@
             "temperature": kwargs.get("temperature", self.temperature),
             "top_p": kwargs.get("top_p", self.top_p),
             "max_tokens": model_max_tokens,
             "stream": True,
         }
         if self.system_prompt:
             json_post["system"] = self.system_prompt
-        if all(value == False for value in PLUGINS.values()) == False:
+        if all(value == False for value in PLUGINS.values()) == False and self.use_plugins:
             json_post.update(copy.deepcopy(claude_tools_list["base"]))
             for item in PLUGINS.keys():
                 try:
                     if PLUGINS[item]:
                         json_post["tools"].append(claude_tools_list[item])
                 except:
                     pass
@@ -377,73 +374,18 @@
         # print("function_full_response", function_full_response)
         # print("function_call_name", function_call_name)
         # print("need_function_call", need_function_call)
         if need_function_call:
             function_full_response = check_json(function_full_response)
             print("function_full_response", function_full_response)
             function_response = ""
-            if function_call_name == "get_search_results":
-                prompt = json.loads(function_full_response)["prompt"]
-                yield "🌐 正在搜索您的问题，提取关键词..."
-                llm = claude3(api_key=self.api_key, api_url=self.api_url, engine=self.engine, system_prompt=self.system_prompt)
-                keywords = llm.ask(search_key_word_prompt.format(source=prompt)).split("\n")
-                function_response = yield from eval(function_call_name)(prompt, keywords)
-                function_call_max_tokens = 32000
-                function_response, text_len = cut_message(function_response, function_call_max_tokens, self.engine)
-                if function_response:
-                    function_response = (
-                        f"You need to response the following question: {prompt}. Search results is provided inside <Search_results></Search_results> XML tags. Your task is to think about the question step by step and then answer the above question in {LANGUAGE} based on the Search results provided. Please response in {LANGUAGE} and adopt a style that is logical, in-depth, and detailed. Note: In order to make the answer appear highly professional, you should be an expert in textual analysis, aiming to make the answer precise and comprehensive. Directly response markdown format, without using markdown code blocks"
-                        "Here is the Search results, inside <Search_results></Search_results> XML tags:"
-                        "<Search_results>"
-                        "{}"
-                        "</Search_results>"
-                    ).format(function_response)
-                else:
-                    function_response = "无法找到相关信息，停止使用 tools"
-                # user_prompt = f"You need to response the following question: {prompt}. Search results is provided inside <Search_results></Search_results> XML tags. Your task is to think about the question step by step and then answer the above question in {config.LANGUAGE} based on the Search results provided. Please response in {config.LANGUAGE} and adopt a style that is logical, in-depth, and detailed. Note: In order to make the answer appear highly professional, you should be an expert in textual analysis, aiming to make the answer precise and comprehensive. Directly response markdown format, without using markdown code blocks"
-                # self.add_to_conversation(user_prompt, "user", convo_id=convo_id)
-            if function_call_name == "get_url_content":
-                url = json.loads(function_full_response)["url"]
-                print("\n\nurl", url)
-                # function_response = jina_ai_Web_crawler(url)
-                function_response = Web_crawler(url)
-                function_response, text_len = cut_message(function_response, function_call_max_tokens, self.engine)
-            if function_call_name == "get_city_tarvel_info":
-                city = json.loads(function_full_response)["city"]
-                function_response = eval(function_call_name)(city)
-                function_response, text_len = cut_message(function_response, function_call_max_tokens, self.engine)
-                function_response = (
-                    f"You need to response the following question: {city}. Tarvel infomation is provided inside <infomation></infomation> XML tags. Your task is to think about the question step by step and then answer the above question in {LANGUAGE} based on the tarvel infomation provided. Please response in {LANGUAGE} and adopt a style that is logical, in-depth, and detailed. Note: In order to make the answer appear highly professional, you should be an expert in textual analysis, aiming to make the answer precise and comprehensive."
-                    "Here is the tarvel infomation, inside <infomation></infomation> XML tags:"
-                    "<infomation>"
-                    "{}"
-                    "</infomation>"
-                ).format(function_response)
-            if function_call_name == "generate_image":
-                prompt = json.loads(function_full_response)["prompt"]
-                function_response = eval(function_call_name)(prompt)
-                function_response, text_len = cut_message(function_response, function_call_max_tokens, self.engine)
-            if function_call_name == "run_python_script":
-                prompt = json.loads(function_full_response)["prompt"]
-                function_response = eval(function_call_name)(prompt)
-                function_response, text_len = cut_message(function_response, function_call_max_tokens, self.engine)
-            if function_call_name == "get_date_time_weekday":
-                function_response = eval(function_call_name)()
-                function_response, text_len = cut_message(function_response, function_call_max_tokens, self.engine)
-            if function_call_name == "get_version_info":
-                function_response = eval(function_call_name)()
-                function_response, text_len = cut_message(function_response, function_call_max_tokens, self.engine)
+            function_call_max_tokens = int(self.truncate_limit / 2)
+            function_response = yield from get_tools_result(function_call_name, function_full_response, function_call_max_tokens, self.engine, claude3, self.api_key, self.api_url, use_plugins=False)
             response_role = "assistant"
             if self.conversation[convo_id][-1]["role"] == "function" and self.conversation[convo_id][-1]["name"] == "get_search_results":
                 mess = self.conversation[convo_id].pop(-1)
             yield from self.ask_stream(function_response, response_role, convo_id=convo_id, function_name=function_call_name, total_tokens=total_tokens, tools_id=tools_id, function_full_response=function_full_response)
         else:
             if self.conversation[convo_id][-1]["role"] == "function" and self.conversation[convo_id][-1]["name"] == "get_search_results":
                 mess = self.conversation[convo_id].pop(-1)
             self.add_to_conversation(full_response, response_role, convo_id=convo_id, total_tokens=total_tokens)
-            self.function_calls_counter = {}
-
-
-
-
-
-        # self.add_to_conversation(full_response, response_role, convo_id=convo_id)
+            self.function_calls_counter = {}
```

### Comparing `modelmerge-0.5.4/src/ModelMerge/models/config.py` & `modelmerge-0.5.5/src/ModelMerge/models/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 import os
 import json
 import httpx
 import requests
 from pathlib import Path
 from collections import defaultdict
 
-
 from ..utils import prompt
 
 PLUGINS = {
-    "SEARCH": (os.environ.get('SEARCH', "True") == "False") == False,
-    "URL": True,
-    "CODE": True,
-    "IMAGE": (os.environ.get('IMAGE', "False") == "False") == False,
-    "DATE": False,
-    "VERSION": False,
-    "TARVEL": (os.environ.get('TARVEL', "False") == "False") == False,
+    "SEARCH" : (os.environ.get('SEARCH', "True") == "False") == False,
+    "URL"    : (os.environ.get('URL', "True") == "False") == False,
+    "CODE"   : (os.environ.get('CODE', "True") == "False") == False,
+    "IMAGE"  : (os.environ.get('IMAGE', "False") == "False") == False,
+    "DATE"   : (os.environ.get('DATE', "False") == "False") == False,
+    "VERSION": (os.environ.get('VERSION', "False") == "False") == False,
+    "TARVEL" : (os.environ.get('TARVEL', "False") == "False") == False,
 }
 
 LANGUAGE = os.environ.get('LANGUAGE', 'Simplified Chinese')
 
 class BaseAPI:
     def __init__(
         self,
@@ -51,14 +50,15 @@
         max_tokens: int = None,
         temperature: float = 0.5,
         top_p: float = 1.0,
         presence_penalty: float = 0.0,
         frequency_penalty: float = 0.0,
         reply_count: int = 1,
         truncate_limit: int = None,
+        use_plugins: bool = True,
     ) -> None:
         self.api_key: str = api_key
         self.engine: str = engine
         self.api_url: str = BaseAPI(api_url or "https://api.openai.com/v1/chat/completions")
         self.system_prompt: str = system_prompt
         self.max_tokens: int = max_tokens
         self.truncate_limit: int = truncate_limit
@@ -96,17 +96,19 @@
             "default": [
                 {
                     "role": "system",
                     "content": system_prompt,
                 },
             ],
         }
+        self.truncate_limit: int = 100000
         self.tokens_usage = defaultdict(int)
         self.function_calls_counter = {}
         self.function_call_max_loop = 10
+        self.use_plugins = use_plugins
 
     def add_to_conversation(
         self,
         message: list,
         role: str,
         convo_id: str = "default",
         function_name: str = "",
```

### Comparing `modelmerge-0.5.4/src/ModelMerge/models/genimi.py` & `modelmerge-0.5.5/src/ModelMerge/models/genimi.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.4/src/ModelMerge/models/groq.py` & `modelmerge-0.5.5/src/ModelMerge/models/groq.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.4/src/ModelMerge/plugins/image.py` & `modelmerge-0.5.5/src/ModelMerge/plugins/image.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.4/src/ModelMerge/plugins/tarvel.py` & `modelmerge-0.5.5/src/ModelMerge/plugins/tarvel.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.4/src/ModelMerge/plugins/websearch.py` & `modelmerge-0.5.5/src/ModelMerge/plugins/websearch.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.4/src/ModelMerge/tools/chatgpt.py` & `modelmerge-0.5.5/src/ModelMerge/tools/chatgpt.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.4/src/ModelMerge/tools/claude.py` & `modelmerge-0.5.5/src/ModelMerge/tools/claude.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.4/src/ModelMerge/utils/prompt.py` & `modelmerge-0.5.5/src/ModelMerge/utils/prompt.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.4/src/ModelMerge/utils/scripts.py` & `modelmerge-0.5.5/src/ModelMerge/utils/scripts.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.4/src/modelmerge.egg-info/PKG-INFO` & `modelmerge-0.5.5/src/modelmerge.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelmerge
-Version: 0.5.4
+Version: 0.5.5
 Summary: modelmerge is a multi-large language model API aggregator.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: lxml
 Requires-Dist: PyExecJS
 Requires-Dist: requests
 Requires-Dist: pdfminer.six
```

### Comparing `modelmerge-0.5.4/src/modelmerge.egg-info/SOURCES.txt` & `modelmerge-0.5.5/src/modelmerge.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 src/ModelMerge/plugins/tarvel.py
 src/ModelMerge/plugins/today.py
 src/ModelMerge/plugins/version.py
 src/ModelMerge/plugins/websearch.py
 src/ModelMerge/tools/__init__.py
 src/ModelMerge/tools/chatgpt.py
 src/ModelMerge/tools/claude.py
+src/ModelMerge/tools/run.py
 src/ModelMerge/utils/__init__.py
 src/ModelMerge/utils/prompt.py
 src/ModelMerge/utils/scripts.py
 src/modelmerge.egg-info/PKG-INFO
 src/modelmerge.egg-info/SOURCES.txt
 src/modelmerge.egg-info/dependency_links.txt
 src/modelmerge.egg-info/requires.txt
```

### Comparing `modelmerge-0.5.4/test/test_Web_crawler.py` & `modelmerge-0.5.5/test/test_Web_crawler.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.4/test/test_claude_zh_char.py` & `modelmerge-0.5.5/test/test_claude_zh_char.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.4/test/test_ddg_search.py` & `modelmerge-0.5.5/test/test_ddg_search.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.4/test/test_download_pdf.py` & `modelmerge-0.5.5/test/test_download_pdf.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.4/test/test_get_token_dict.py` & `modelmerge-0.5.5/test/test_get_token_dict.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.4/test/test_google_search.py` & `modelmerge-0.5.5/test/test_google_search.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.4/test/test_jieba.py` & `modelmerge-0.5.5/test/test_jieba.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.4/test/test_json.py` & `modelmerge-0.5.5/test/test_json.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.4/test/test_langchain_search_old.py` & `modelmerge-0.5.5/test/test_langchain_search_old.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.4/test/test_logging.py` & `modelmerge-0.5.5/test/test_logging.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.4/test/test_ollama.py` & `modelmerge-0.5.5/test/test_ollama.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.4/test/test_py_run.py` & `modelmerge-0.5.5/test/test_py_run.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.4/test/test_tikitoken.py` & `modelmerge-0.5.5/test/test_tikitoken.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.4/test/test_token.py` & `modelmerge-0.5.5/test/test_token.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.4/test/test_url.py` & `modelmerge-0.5.5/test/test_url.py`

 * *Files identical despite different names*

