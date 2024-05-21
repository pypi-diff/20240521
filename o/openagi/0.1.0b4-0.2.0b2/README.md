# Comparing `tmp/openagi-0.1.0b4.tar.gz` & `tmp/openagi-0.2.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openagi-0.1.0b4.tar", max compression
+gzip compressed data, was "openagi-0.2.0b2.tar", max compression
```

## Comparing `openagi-0.1.0b4.tar` & `openagi-0.2.0b2.tar`

### file list

```diff
@@ -1,46 +1,78 @@
--rw-r--r--   0        0        0     6486 2024-04-23 06:32:39.825436 openagi-0.1.0b4/README.md
--rw-r--r--   0        0        0     1159 2024-04-23 06:34:12.487295 openagi-0.1.0b4/pyproject.toml
--rw-r--r--   0        0        0     1499 2024-04-19 10:30:02.396089 openagi-0.1.0b4/src/Readme.md
--rw-r--r--   0        0        0      667 2024-04-19 10:30:02.396089 openagi-0.1.0b4/src/openagi/__init__.py
--rw-r--r--   0        0        0    14362 2024-04-19 11:33:11.880047 openagi-0.1.0b4/src/openagi/agent.py
--rw-r--r--   0        0        0     3398 2024-04-19 10:30:02.397089 openagi-0.1.0b4/src/openagi/init_agent.py
--rw-r--r--   0        0        0      196 2024-04-19 10:30:02.397089 openagi-0.1.0b4/src/openagi/llms/__init__.py
--rw-r--r--   0        0        0     2722 2024-04-23 06:32:39.889436 openagi-0.1.0b4/src/openagi/llms/azure.py
--rw-r--r--   0        0        0     1352 2024-04-23 06:32:39.890436 openagi-0.1.0b4/src/openagi/llms/base.py
--rw-r--r--   0        0        0     1615 2024-04-23 06:32:39.891436 openagi-0.1.0b4/src/openagi/llms/hf.py
--rw-r--r--   0        0        0      715 2024-04-23 06:32:39.893436 openagi-0.1.0b4/src/openagi/llms/openagi_main.py
--rw-r--r--   0        0        0     1620 2024-04-23 06:32:39.894436 openagi-0.1.0b4/src/openagi/llms/openai.py
--rw-r--r--   0        0        0     3782 2024-04-19 10:30:02.397089 openagi-0.1.0b4/src/openagi/queue/message_broker.py
--rw-r--r--   0        0        0     2750 2024-04-23 06:32:39.895436 openagi-0.1.0b4/src/openagi/queue/pq.py
--rw-r--r--   0        0        0     6433 2024-04-19 10:30:02.397089 openagi-0.1.0b4/src/openagi/queue/timer_pool.py
--rw-r--r--   0        0        0       28 2024-04-19 10:30:02.398089 openagi-0.1.0b4/src/openagi/tools/__init__.py
--rw-r--r--   0        0        0     2078 2024-04-23 06:32:39.897436 openagi-0.1.0b4/src/openagi/tools/base.py
--rw-r--r--   0        0        0      762 2024-04-19 10:30:02.398089 openagi-0.1.0b4/src/openagi/tools/custom_tools/ProxyTool.py
--rw-r--r--   0        0        0      212 2024-04-19 10:30:02.398089 openagi-0.1.0b4/src/openagi/tools/custom_tools/custom_tool_db.py
--rw-r--r--   0        0        0     1292 2024-04-19 10:30:02.398089 openagi-0.1.0b4/src/openagi/tools/integrations/__init__.py
--rw-r--r--   0        0        0      581 2024-04-19 10:30:02.398089 openagi-0.1.0b4/src/openagi/tools/integrations/dalle_image_generator.py
--rw-r--r--   0        0        0     2824 2024-04-23 06:32:39.898436 openagi-0.1.0b4/src/openagi/tools/integrations/document_compare.py
--rw-r--r--   0        0        0     1045 2024-04-23 06:32:39.899436 openagi-0.1.0b4/src/openagi/tools/integrations/duckducksearch.py
--rw-r--r--   0        0        0     1527 2024-04-19 10:30:02.399089 openagi-0.1.0b4/src/openagi/tools/integrations/exa_search_tool.py
--rw-r--r--   0        0        0     1745 2024-04-19 10:30:02.399089 openagi-0.1.0b4/src/openagi/tools/integrations/github.py
--rw-r--r--   0        0        0     1595 2024-04-19 10:30:02.399089 openagi-0.1.0b4/src/openagi/tools/integrations/gmail.py
--rw-r--r--   0        0        0      270 2024-04-19 10:30:02.399089 openagi-0.1.0b4/src/openagi/tools/integrations/google.py
--rw-r--r--   0        0        0     1433 2024-04-19 10:30:02.399089 openagi-0.1.0b4/src/openagi/tools/integrations/google_finance_search.py
--rw-r--r--   0        0        0     1357 2024-04-19 10:30:02.399089 openagi-0.1.0b4/src/openagi/tools/integrations/google_serper_specific.py
--rw-r--r--   0        0        0     1160 2024-04-19 10:30:02.399089 openagi-0.1.0b4/src/openagi/tools/integrations/googlejobsearch.py
--rw-r--r--   0        0        0      841 2024-04-19 10:30:02.399089 openagi-0.1.0b4/src/openagi/tools/integrations/googleserpersearch.py
--rw-r--r--   0        0        0     1350 2024-04-19 10:30:02.399089 openagi-0.1.0b4/src/openagi/tools/integrations/nasa.py
--rw-r--r--   0        0        0      844 2024-04-19 10:30:02.399089 openagi-0.1.0b4/src/openagi/tools/integrations/open_weathermap.py
--rw-r--r--   0        0        0     1743 2024-04-19 10:30:02.399089 openagi-0.1.0b4/src/openagi/tools/integrations/polygon.py
--rw-r--r--   0        0        0     1444 2024-04-19 10:30:02.400089 openagi-0.1.0b4/src/openagi/tools/integrations/serper_intermediate.py
--rw-r--r--   0        0        0     1357 2024-04-19 10:30:02.400089 openagi-0.1.0b4/src/openagi/tools/integrations/sql.py
--rw-r--r--   0        0        0     1141 2024-04-19 10:30:02.400089 openagi-0.1.0b4/src/openagi/tools/integrations/wikipedia_tool.py
--rw-r--r--   0        0        0     1248 2024-04-19 10:30:02.400089 openagi-0.1.0b4/src/openagi/tools/integrations/xorbits.py
--rw-r--r--   0        0        0     1315 2024-04-19 10:30:02.400089 openagi-0.1.0b4/src/openagi/tools/integrations/yahoofinancenews.py
--rw-r--r--   0        0        0      945 2024-04-19 10:30:02.400089 openagi-0.1.0b4/src/openagi/tools/integrations/youtubesearch.py
--rw-r--r--   0        0        0     3198 2024-04-19 10:30:02.400089 openagi-0.1.0b4/src/openagi/tools/tools_db.py
--rw-r--r--   0        0        0     3255 2024-04-19 10:30:02.400089 openagi-0.1.0b4/src/openagi/tools/utils.py
--rw-r--r--   0        0        0      593 2024-04-19 10:30:02.400089 openagi-0.1.0b4/src/openagi/utils/extraction.py
--rw-r--r--   0        0        0    13792 2024-04-19 10:30:02.400089 openagi-0.1.0b4/src/openagi/utils/llmTasks.py
--rw-r--r--   0        0        0      730 2024-04-19 10:30:02.401089 openagi-0.1.0b4/src/openagi/utils/yamlParse.py
--rw-r--r--   0        0        0     8183 1970-01-01 00:00:00.000000 openagi-0.1.0b4/PKG-INFO
+-rw-r--r--   0        0        0     8953 2024-05-21 17:32:13.916710 openagi-0.2.0b2/README.md
+-rw-r--r--   0        0        0     1197 2024-05-21 17:37:51.570525 openagi-0.2.0b2/pyproject.toml
+-rw-r--r--   0        0        0     1499 2024-04-19 10:30:02.396089 openagi-0.2.0b2/src/Readme.md
+-rw-r--r--   0        0        0      558 2024-05-21 17:32:13.930709 openagi-0.2.0b2/src/openagi/__init__.py
+-rw-r--r--   0        0        0      183 2024-05-21 17:32:13.930709 openagi-0.2.0b2/src/openagi/actions/__init__.py
+-rw-r--r--   0        0        0     1667 2024-05-21 17:32:13.931710 openagi-0.2.0b2/src/openagi/actions/base.py
+-rw-r--r--   0        0        0      511 2024-05-21 17:32:13.931710 openagi-0.2.0b2/src/openagi/actions/compressor.py
+-rw-r--r--   0        0        0      381 2024-05-21 17:32:13.931710 openagi-0.2.0b2/src/openagi/actions/console.py
+-rw-r--r--   0        0        0     1990 2024-05-21 17:32:13.933709 openagi-0.2.0b2/src/openagi/actions/files.py
+-rw-r--r--   0        0        0      724 2024-05-21 17:32:13.933709 openagi-0.2.0b2/src/openagi/actions/formatter.py
+-rw-r--r--   0        0        0      404 2024-05-21 17:32:13.934710 openagi-0.2.0b2/src/openagi/actions/human_input.py
+-rw-r--r--   0        0        0     1114 2024-05-21 17:32:13.934710 openagi-0.2.0b2/src/openagi/actions/obs_rag.py
+-rw-r--r--   0        0        0       80 2024-05-21 17:32:13.934710 openagi-0.2.0b2/src/openagi/actions/tools/__init__.py
+-rw-r--r--   0        0        0     1052 2024-05-21 17:32:13.935710 openagi-0.2.0b2/src/openagi/actions/tools/ddg_search.py
+-rw-r--r--   0        0        0     1925 2024-05-21 17:32:13.935710 openagi-0.2.0b2/src/openagi/actions/tools/serp_search.py
+-rw-r--r--   0        0        0      948 2024-05-21 17:32:13.936710 openagi-0.2.0b2/src/openagi/actions/tools/serper_search.py
+-rw-r--r--   0        0        0        0 2024-05-21 17:32:13.936710 openagi-0.2.0b2/src/openagi/actions/utils.py
+-rw-r--r--   0        0        0     7702 2024-05-21 17:32:13.939710 openagi-0.2.0b2/src/openagi/agent.py
+-rw-r--r--   0        0        0      117 2024-05-21 17:32:13.942710 openagi-0.2.0b2/src/openagi/exception.py
+-rw-r--r--   0        0        0     3398 2024-04-19 10:30:02.397089 openagi-0.2.0b2/src/openagi/init_agent.py
+-rw-r--r--   0        0        0      196 2024-04-19 10:30:02.397089 openagi-0.2.0b2/src/openagi/llms/__init__.py
+-rw-r--r--   0        0        0     2356 2024-05-21 17:32:13.943709 openagi-0.2.0b2/src/openagi/llms/azure.py
+-rw-r--r--   0        0        0     1272 2024-05-21 17:32:13.943709 openagi-0.2.0b2/src/openagi/llms/base.py
+-rw-r--r--   0        0        0     1609 2024-05-21 17:32:13.943709 openagi-0.2.0b2/src/openagi/llms/hf.py
+-rw-r--r--   0        0        0      713 2024-05-21 17:32:13.944709 openagi-0.2.0b2/src/openagi/llms/openagi_main.py
+-rw-r--r--   0        0        0     1754 2024-05-21 17:32:13.944709 openagi-0.2.0b2/src/openagi/llms/openai.py
+-rw-r--r--   0        0        0       27 2024-05-21 17:32:13.944709 openagi-0.2.0b2/src/openagi/memory/__init__.py
+-rw-r--r--   0        0        0     2132 2024-05-21 17:32:13.944709 openagi-0.2.0b2/src/openagi/memory/base.py
+-rw-r--r--   0        0        0       80 2024-05-21 17:32:13.944709 openagi-0.2.0b2/src/openagi/memory/memory.py
+-rw-r--r--   0        0        0        0 2024-05-21 17:32:13.944709 openagi-0.2.0b2/src/openagi/planner/LATS.py
+-rw-r--r--   0        0        0       45 2024-05-01 10:04:19.838349 openagi-0.2.0b2/src/openagi/planner/__init__.py
+-rw-r--r--   0        0        0      914 2024-05-21 17:32:13.945710 openagi-0.2.0b2/src/openagi/planner/base.py
+-rw-r--r--   0        0        0        0 2024-05-21 17:32:13.945710 openagi-0.2.0b2/src/openagi/planner/reflexion.py
+-rw-r--r--   0        0        0     2165 2024-05-21 17:32:13.945710 openagi-0.2.0b2/src/openagi/planner/task_decomposer.py
+-rw-r--r--   0        0        0        0 2024-05-01 09:44:08.540909 openagi-0.2.0b2/src/openagi/prompts/__init__.py
+-rw-r--r--   0        0        0     1005 2024-05-21 17:32:13.945710 openagi-0.2.0b2/src/openagi/prompts/base.py
+-rw-r--r--   0        0        0      145 2024-05-21 17:32:13.946709 openagi-0.2.0b2/src/openagi/prompts/constants.py
+-rw-r--r--   0        0        0     2940 2024-05-21 17:32:13.946709 openagi-0.2.0b2/src/openagi/prompts/execution.py
+-rw-r--r--   0        0        0     3034 2024-05-21 17:32:13.946709 openagi-0.2.0b2/src/openagi/prompts/task_creator.py
+-rw-r--r--   0        0        0        0 2024-05-21 17:32:13.946709 openagi-0.2.0b2/src/openagi/storage/__init__.py
+-rw-r--r--   0        0        0      943 2024-05-21 17:32:13.946709 openagi-0.2.0b2/src/openagi/storage/base.py
+-rw-r--r--   0        0        0     2339 2024-05-21 17:32:13.947709 openagi-0.2.0b2/src/openagi/storage/chroma.py
+-rw-r--r--   0        0        0       78 2024-05-02 13:26:09.326553 openagi-0.2.0b2/src/openagi/tasks/__init__.py
+-rw-r--r--   0        0        0     1236 2024-05-21 17:32:13.947709 openagi-0.2.0b2/src/openagi/tasks/lists.py
+-rw-r--r--   0        0        0      787 2024-05-21 17:32:13.947709 openagi-0.2.0b2/src/openagi/tasks/task.py
+-rw-r--r--   0        0        0       28 2024-04-19 10:30:02.398089 openagi-0.2.0b2/src/openagi/tools/__init__.py
+-rw-r--r--   0        0        0     2078 2024-04-23 06:32:39.897436 openagi-0.2.0b2/src/openagi/tools/base.py
+-rw-r--r--   0        0        0      762 2024-04-19 10:30:02.398089 openagi-0.2.0b2/src/openagi/tools/custom_tools/ProxyTool.py
+-rw-r--r--   0        0        0      212 2024-04-19 10:30:02.398089 openagi-0.2.0b2/src/openagi/tools/custom_tools/custom_tool_db.py
+-rw-r--r--   0        0        0     1292 2024-04-19 10:30:02.398089 openagi-0.2.0b2/src/openagi/tools/integrations/__init__.py
+-rw-r--r--   0        0        0      581 2024-04-19 10:30:02.398089 openagi-0.2.0b2/src/openagi/tools/integrations/dalle_image_generator.py
+-rw-r--r--   0        0        0     2806 2024-05-21 17:32:13.947709 openagi-0.2.0b2/src/openagi/tools/integrations/document_compare.py
+-rw-r--r--   0        0        0     1045 2024-04-23 06:32:39.899436 openagi-0.2.0b2/src/openagi/tools/integrations/duckducksearch.py
+-rw-r--r--   0        0        0     1527 2024-04-19 10:30:02.399089 openagi-0.2.0b2/src/openagi/tools/integrations/exa_search_tool.py
+-rw-r--r--   0        0        0     1733 2024-05-21 17:32:13.948710 openagi-0.2.0b2/src/openagi/tools/integrations/github.py
+-rw-r--r--   0        0        0     1589 2024-05-21 17:32:13.948710 openagi-0.2.0b2/src/openagi/tools/integrations/gmail.py
+-rw-r--r--   0        0        0      277 2024-05-21 17:32:13.948710 openagi-0.2.0b2/src/openagi/tools/integrations/google.py
+-rw-r--r--   0        0        0     1424 2024-05-21 17:32:13.948710 openagi-0.2.0b2/src/openagi/tools/integrations/google_finance_search.py
+-rw-r--r--   0        0        0     1351 2024-05-21 17:32:13.949710 openagi-0.2.0b2/src/openagi/tools/integrations/google_serper_specific.py
+-rw-r--r--   0        0        0     1160 2024-04-19 10:30:02.399089 openagi-0.2.0b2/src/openagi/tools/integrations/googlejobsearch.py
+-rw-r--r--   0        0        0      841 2024-04-19 10:30:02.399089 openagi-0.2.0b2/src/openagi/tools/integrations/googleserpersearch.py
+-rw-r--r--   0        0        0     1350 2024-04-19 10:30:02.399089 openagi-0.2.0b2/src/openagi/tools/integrations/nasa.py
+-rw-r--r--   0        0        0      844 2024-04-19 10:30:02.399089 openagi-0.2.0b2/src/openagi/tools/integrations/open_weathermap.py
+-rw-r--r--   0        0        0     1743 2024-04-19 10:30:02.399089 openagi-0.2.0b2/src/openagi/tools/integrations/polygon.py
+-rw-r--r--   0        0        0     1444 2024-04-19 10:30:02.400089 openagi-0.2.0b2/src/openagi/tools/integrations/serper_intermediate.py
+-rw-r--r--   0        0        0     1351 2024-05-21 17:32:13.950709 openagi-0.2.0b2/src/openagi/tools/integrations/sql.py
+-rw-r--r--   0        0        0     1141 2024-04-19 10:30:02.400089 openagi-0.2.0b2/src/openagi/tools/integrations/wikipedia_tool.py
+-rw-r--r--   0        0        0     1242 2024-05-21 17:32:13.950709 openagi-0.2.0b2/src/openagi/tools/integrations/xorbits.py
+-rw-r--r--   0        0        0     1315 2024-04-19 10:30:02.400089 openagi-0.2.0b2/src/openagi/tools/integrations/yahoofinancenews.py
+-rw-r--r--   0        0        0      945 2024-04-19 10:30:02.400089 openagi-0.2.0b2/src/openagi/tools/integrations/youtubesearch.py
+-rw-r--r--   0        0        0     3198 2024-04-19 10:30:02.400089 openagi-0.2.0b2/src/openagi/tools/tools_db.py
+-rw-r--r--   0        0        0     3246 2024-05-21 17:32:13.950709 openagi-0.2.0b2/src/openagi/tools/utils.py
+-rw-r--r--   0        0        0     3017 2024-05-21 17:32:13.951709 openagi-0.2.0b2/src/openagi/utils/extraction.py
+-rw-r--r--   0        0        0    13792 2024-04-30 05:51:06.030343 openagi-0.2.0b2/src/openagi/utils/llmTasks.py
+-rw-r--r--   0        0        0      260 2024-05-21 17:32:13.951709 openagi-0.2.0b2/src/openagi/utils/yamlParse.py
+-rw-r--r--   0        0        0        0 2024-05-21 17:32:13.951709 openagi-0.2.0b2/src/openagi/worker/__init__.py
+-rw-r--r--   0        0        0      589 2024-05-21 17:32:13.951709 openagi-0.2.0b2/src/openagi/worker/worker.py
+-rw-r--r--   0        0        0    10730 1970-01-01 00:00:00.000000 openagi-0.2.0b2/PKG-INFO
```

### Comparing `openagi-0.1.0b4/pyproject.toml` & `openagi-0.2.0b2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "openagi"
-version = "0.1.0-b4"
+version = "0.2.0-b2"
 description = ""
 authors = ["AI Planet <tech@aiplanet.com>"]
 readme = "README.md"
 include = ["src/*"]
 
 [tool.poetry.dependencies]
 python = "^3.9, <3.12"
 langchain = "0.1.8"
 langchain-community = "0.0.21"
 langchain-openai = "0.0.6"
-duckduckgo-search = "^5.3.0"
+duckduckgo-search = "^6.1.0"
 spacy = "3.7.4"
 xorbits = "^0.7.2"
 azure-identity = "^1.15.0"
 langchain-text-splitters = "^0.0.1"
 python-dotenv = "^1.0.1"
 langchain-experimental = "^0.0.53"
 spacytextblob = "^4.0.0"
@@ -33,14 +33,16 @@
 langchainhub = "^0.1.15"
 python-multipart = "^0.0.9"
 pandas = "^2.2.2"
 numpy = "^1.26.4"
 transformers = "^4.40.0"
 pypdf = "^4.2.0"
 faiss-cpu = "^1.8.0"
+pytest = "^8.2.0"
+chromadb = "^0.5.0"
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.1.11"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `openagi-0.1.0b4/src/Readme.md` & `openagi-0.2.0b2/src/Readme.md`

 * *Files identical despite different names*

### Comparing `openagi-0.1.0b4/src/openagi/__init__.py` & `openagi-0.2.0b2/src/openagi/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 import logging
+import os
 from datetime import datetime
 from pathlib import Path
 
 BASE_PATH = "logs"
 pth = Path(BASE_PATH)
 pth.mkdir(parents=True, exist_ok=True)
-filename = (f'{pth.absolute()}/application_{datetime.now().strftime("%Y-%m-%d_%H-%M-%S")}.log')
+filename = f'{pth.absolute()}/application_{datetime.now().strftime("%Y-%m-%d_%H-%M-%S")}.log'
+
+LOG_LEVEL = getattr(
+    logging,
+    os.environ.get("OPENAGI_LOG_LEVEL", "INFO").upper(),
+    logging.INFO,
+)
+
 
 # Setup basic logging configuration
 logging.basicConfig(
-    level=logging.DEBUG,
-    format="%(asctime)s %(levelname)s::%(thread)d::%(pathname)s:%(lineno)d:%(funcName)s:%(message)s",
+    level=LOG_LEVEL,
+    format="%(asctime)s %(pathname)s:%(lineno)d:%(funcName)s: %(message)s",
     datefmt="%Y-%m-%d %H:%M:%S",
-    filename=f'{pth.absolute()}/application_{datetime.now().strftime("%Y-%m-%d_%H-%M-%S")}.log',
-    filemode="w",
 )
-print(f"Logs stored at {filename}")
-logging.info(f"Logs stored at {pth.absolute()}")
```

### Comparing `openagi-0.1.0b4/src/openagi/init_agent.py` & `openagi-0.2.0b2/src/openagi/init_agent.py`

 * *Files identical despite different names*

### Comparing `openagi-0.1.0b4/src/openagi/llms/azure.py` & `openagi-0.2.0b2/src/openagi/llms/azure.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+from typing import Any
 from langchain_core.messages import HumanMessage
 from langchain_openai import AzureChatOpenAI  # Assuming this import is correct
 
 from openagi.llms.base import LLMBaseModel, LLMConfigModel
-from openagi.utils.yamlParse import read_yaml_config
+from openagi.utils.yamlParse import read_from_env
 
 
 class AzureChatConfigModel(LLMConfigModel):
     """Configuration model for Azure Chat OpenAI."""
 
     base_url: str
     deployment_name: str
@@ -17,66 +18,51 @@
 
 class AzureChatOpenAIModel(LLMBaseModel):
     """Azure's OpenAI service implementation of the LLMBaseModel.
 
     This class implements the specific logic required to work with Azure's OpenAI service.
     """
 
-    def __init__(self, config: AzureChatConfigModel):
-        super().__init__(config)
+    config: Any
 
     def load(self):
         """Initializes the AzureChatOpenAI instance with configurations."""
         self.llm = AzureChatOpenAI(
             azure_deployment=self.config.deployment_name,
             model_name=self.config.model_name,
             openai_api_version=self.config.openai_api_version,
             openai_api_key=self.config.api_key,
             azure_endpoint=self.config.base_url,
         )
         return self.llm
 
-    def run(self, input_text: str):
+    def run(self, input_data: str):
         """Runs the Azure Chat OpenAI model with the provided input text.
 
         Args:
-            input_text: The input text to process.
+            input_data: The input text to process.
 
         Returns:
             The response from Azure's OpenAI service.
         """
         if not self.llm:
             self.load()
         if not self.llm:
             raise ValueError("`llm` attribute not set.")
-        message = HumanMessage(content=input_text)
+        message = HumanMessage(content=input_data)
         resp = self.llm([message])
         return resp.content
 
     @staticmethod
-    def load_from_yaml_config() -> AzureChatConfigModel:
+    def load_from_env_config() -> AzureChatConfigModel:
         """Loads the AzureChatOpenAI configurations from a YAML file.
 
         Returns:
             An instance of AzureChatConfigModel with loaded configurations.
         """
         return AzureChatConfigModel(
-            base_url=read_yaml_config("BASE_URL", raise_exception=True),
-            deployment_name=read_yaml_config("DEPLOYMENT_NAME", raise_exception=True),
-            model_name=read_yaml_config("MODEL_NAME", raise_exception=True),
-            openai_api_version=read_yaml_config("OPENAI_API_VERSION", raise_exception=True),
-            api_key=read_yaml_config("AZURE_OPENAI_API_KEY", raise_exception=True),
+            base_url=read_from_env("AZURE_BASE_URL", raise_exception=True),
+            deployment_name=read_from_env("AZURE_DEPLOYMENT_NAME", raise_exception=True),
+            model_name=read_from_env("AZURE_MODEL_NAME", raise_exception=True),
+            openai_api_version=read_from_env("AZURE_OPENAI_API_VERSION", raise_exception=True),
+            api_key=read_from_env("AZURE_OPENAI_API_KEY", raise_exception=True),
         )
-
-
-"""
-def main():
-    # Demonstrates the use of AzureChatOpenAIModel.
-    config = AzureChatOpenAIModel.load_from_yaml_config()
-    azure_chat_model = AzureChatOpenAIModel(config=config)
-    response = azure_chat_model.run("Hello, how can I help you today?")
-    print(response)
-
-
-if __name__ == "__main__":
-    main()
-"""
```

### Comparing `openagi-0.1.0b4/src/openagi/llms/base.py` & `openagi-0.2.0b2/src/openagi/llms/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,26 +12,24 @@
 
     class Config:
         protected_namespaces = ()
 
     pass  # Common fields could be defined here, if any.
 
 
-class LLMBaseModel(ABC):
+class LLMBaseModel(BaseModel):
     """Abstract base class for language learning models.
 
     Attributes:
         config: An instance of LLMConfigModel containing configuration.
         llm: Placeholder for the actual LLM instance, to be defined in subclasses.
     """
 
-    def __init__(self, config: LLMConfigModel):
-        self.config = config
-        self.llm = None
-        self.load()
+    config: Any
+    llm: Any = None
 
     @abstractmethod
     def load(self):
         """Initializes the LLM instance with configurations."""
         pass
 
     @abstractmethod
@@ -44,10 +42,10 @@
         Returns:
             The result from processing the input data through the LLM.
         """
         pass
 
     @staticmethod
     @abstractmethod
-    def load_from_yaml_config():
+    def load_from_env_config():
         """Loads configuration values from a YAML file."""
         pass
```

### Comparing `openagi-0.1.0b4/src/openagi/llms/hf.py` & `openagi-0.2.0b2/src/openagi/llms/hf.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from transformers import pipeline
 from openagi.llms.base import LLMBaseModel, LLMConfigModel
-from openagi.utils.yamlParse import read_yaml_config
+from openagi.utils.yamlParse import read_from_env
+
 
 class HuggingFaceConfigModel(LLMConfigModel):
     """Configuration model for Hugging Face."""
 
     huggingface_model: str
 
 
@@ -32,19 +33,19 @@
             The response from Hugging Face service.
         """
         if not self.llm:
             self.load()
         if not self.llm:
             raise ValueError("`llm` attribute not set.")
         resp = self.llm(input_text)
-        return resp[0]['generated_text']
+        return resp[0]["generated_text"]
 
     @staticmethod
-    def load_from_yaml_config() -> HuggingFaceConfigModel:
+    def load_from_env_config() -> HuggingFaceConfigModel:
         """Loads the Hugging Face configurations from a YAML file.
 
         Returns:
             An instance of HuggingFaceConfigModel with loaded configurations.
         """
         return HuggingFaceConfigModel(
-            huggingface_model=read_yaml_config("HUGGINGFACE_MODEL", raise_exception=True),
+            huggingface_model=read_from_env("HUGGINGFACE_MODEL", raise_exception=True),
         )
```

### Comparing `openagi-0.1.0b4/src/openagi/llms/openagi_main.py` & `openagi-0.2.0b2/src/openagi/llms/openagi_main.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from openagi.llms.azure import AzureChatOpenAIModel
 from openagi.llms.openai import OpenAIModel
 
 
 def loadLLM(llm="openai"):
     if llm == "openai":
-        config = OpenAIModel.load_from_yaml_config()
+        config = OpenAIModel.load_from_env_config()
         llm = OpenAIModel(config=config)
         return llm
     else:
-        config = AzureChatOpenAIModel.load_from_yaml_config()
+        config = AzureChatOpenAIModel.load_from_env_config()
         llm = AzureChatOpenAIModel(config=config)
     return llm
 
 
 def getLLM(sys):
     # total arguments
     n = len(sys.argv)
```

### Comparing `openagi-0.1.0b4/src/openagi/llms/openai.py` & `openagi-0.2.0b2/src/openagi/llms/openai.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,54 +1,60 @@
+import logging
+from typing import Any
 from langchain_core.messages import HumanMessage
 from langchain_openai import ChatOpenAI
 
 from openagi.llms.base import LLMBaseModel, LLMConfigModel
-from openagi.utils.yamlParse import read_yaml_config
+from openagi.utils.yamlParse import read_from_env
 
 
 class OpenAIConfigModel(LLMConfigModel):
     """Configuration model for OpenAI."""
 
+    model_name: str = "gpt-4-turbo"
     openai_api_key: str
 
 
 class OpenAIModel(LLMBaseModel):
     """OpenAI service implementation of the LLMBaseModel.
 
     This class implements the specific logic required to work with OpenAI service.
     """
 
-    def __init__(self, config: OpenAIConfigModel):
-        super().__init__(config)
+    config: Any
 
     def load(self):
         """Initializes the OpenAI instance with configurations."""
-        self.llm = ChatOpenAI(openai_api_key=self.config.openai_api_key)
+        self.llm = ChatOpenAI(
+            openai_api_key=self.config.openai_api_key,
+            model_name=self.config.model_name,
+        )
         return self.llm
 
     def run(self, input_text: str):
         """Runs the OpenAI model with the provided input text.
 
         Args:
             input_text: The input text to process.
 
         Returns:
             The response from OpenAI service.
         """
+        logging.info(f"Running LLM - {self.__class__.__name__}")
         if not self.llm:
             self.load()
         if not self.llm:
             raise ValueError("`llm` attribute not set.")
         message = HumanMessage(content=input_text)
         resp = self.llm([message])
         return resp.content
 
     @staticmethod
-    def load_from_yaml_config() -> OpenAIConfigModel:
+    def load_from_env_config() -> OpenAIConfigModel:
         """Loads the OpenAI configurations from a YAML file.
 
         Returns:
             An instance of OpenAIConfigModel with loaded configurations.
         """
         return OpenAIConfigModel(
-            openai_api_key=read_yaml_config("OPENAI_API_KEY", raise_exception=True),
+            openai_api_key=read_from_env("OPENAI_API_KEY", raise_exception=True),
         )
```

### Comparing `openagi-0.1.0b4/src/openagi/tools/base.py` & `openagi-0.2.0b2/src/openagi/tools/base.py`

 * *Files identical despite different names*

### Comparing `openagi-0.1.0b4/src/openagi/tools/custom_tools/ProxyTool.py` & `openagi-0.2.0b2/src/openagi/tools/custom_tools/ProxyTool.py`

 * *Files identical despite different names*

### Comparing `openagi-0.1.0b4/src/openagi/tools/integrations/__init__.py` & `openagi-0.2.0b2/src/openagi/tools/integrations/__init__.py`

 * *Files identical despite different names*

### Comparing `openagi-0.1.0b4/src/openagi/tools/integrations/dalle_image_generator.py` & `openagi-0.2.0b2/src/openagi/tools/integrations/dalle_image_generator.py`

 * *Files identical despite different names*

### Comparing `openagi-0.1.0b4/src/openagi/tools/integrations/document_compare.py` & `openagi-0.2.0b2/src/openagi/tools/integrations/document_compare.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,37 +10,37 @@
 from langchain_community.document_loaders import PyPDFLoader
 from langchain_community.vectorstores import FAISS
 from langchain_openai import AzureOpenAIEmbeddings
 from langchain_text_splitters import CharacterTextSplitter
 from pydantic import BaseModel, Field
 
 from openagi.tools.base import BaseTool, tool
-from openagi.utils.yamlParse import read_yaml_config
+from openagi.utils.yamlParse import read_from_env
 
 
 def DocuCompare(searchString, llm):
-    os.environ["AZURE_OPENAI_ENDPOINT"] = read_yaml_config("BASE_URL")
-    deployment_name = read_yaml_config("EMBEDDING_DEPLOYMENT")
+    os.environ["AZURE_OPENAI_ENDPOINT"] = read_from_env("BASE_URL")
+    deployment_name = read_from_env("EMBEDDING_DEPLOYMENT")
     tools = []
-    directory = read_yaml_config("pdfFile")  # Specify the directory path here
+    directory = read_from_env("pdfFile")  # Specify the directory path here
     files = []
     for filename in os.listdir(directory):
         if filename.endswith(".pdf"):
             file_path = os.path.join(directory, filename)
             file_info = {"name": os.path.splitext(filename)[0], "path": file_path}
             files.append(file_info)
     for file in files:
         loader = PyPDFLoader(file["path"])
         pages = loader.load_and_split()
         text_splitter = CharacterTextSplitter(chunk_size=1000, chunk_overlap=0)
         docs = text_splitter.split_documents(pages)
         embeddings = AzureOpenAIEmbeddings(
-            api_key = read_yaml_config("AZURE_OPENAI_API_KEY"),
+            api_key = read_from_env("AZURE_OPENAI_API_KEY"),
             azure_deployment=deployment_name,
-            openai_api_version=read_yaml_config("OPENAI_API_VERSION"),
+            openai_api_version=read_from_env("OPENAI_API_VERSION"),
         )
         retriever = FAISS.from_documents(docs, embeddings).as_retriever()
         tools.append(
             Tool(
                 name=file["name"],
                 description=f"useful when you want to answer questions about {file['name']}",
                 func=RetrievalQA.from_chain_type(llm=llm, retriever=retriever),
```

### Comparing `openagi-0.1.0b4/src/openagi/tools/integrations/duckducksearch.py` & `openagi-0.2.0b2/src/openagi/tools/integrations/duckducksearch.py`

 * *Files identical despite different names*

### Comparing `openagi-0.1.0b4/src/openagi/tools/integrations/exa_search_tool.py` & `openagi-0.2.0b2/src/openagi/tools/integrations/exa_search_tool.py`

 * *Files identical despite different names*

### Comparing `openagi-0.1.0b4/src/openagi/tools/integrations/github.py` & `openagi-0.2.0b2/src/openagi/tools/integrations/github.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,21 +6,21 @@
     initialize_agent,
 )
 from langchain_community.agent_toolkits.github.toolkit import GitHubToolkit
 from langchain_community.utilities.github import GitHubAPIWrapper
 from pydantic import BaseModel, Field
 
 from openagi.tools.base import BaseTool, tool
-from openagi.utils.yamlParse import read_yaml_config
+from openagi.utils.yamlParse import read_from_env
 
 
 def github_toolkit(searchString, llm):
-    os.environ["GITHUB_APP_ID"] = read_yaml_config("GITHUB_APP_ID")
-    os.environ["GITHUB_APP_PRIVATE_KEY"] = read_yaml_config("GITHUB_APP_PRIVATE_KEY")
-    os.environ["GITHUB_REPOSITORY"] = read_yaml_config("GITHUB_REPOSITORY")
+    os.environ["GITHUB_APP_ID"] = read_from_env("GITHUB_APP_ID")
+    os.environ["GITHUB_APP_PRIVATE_KEY"] = read_from_env("GITHUB_APP_PRIVATE_KEY")
+    os.environ["GITHUB_REPOSITORY"] = read_from_env("GITHUB_REPOSITORY")
     github = GitHubAPIWrapper()
     toolkit = GitHubToolkit.from_github_api_wrapper(github)
     tools = toolkit.get_tools()
     agent = initialize_agent(
         tools=tools,
         llm=llm,
         agent=AgentType.STRUCTURED_CHAT_ZERO_SHOT_REACT_DESCRIPTION,
```

### Comparing `openagi-0.1.0b4/src/openagi/tools/integrations/gmail.py` & `openagi-0.2.0b2/src/openagi/tools/integrations/gmail.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 )
 from langchain_community.agent_toolkits import (
     GmailToolkit,
 )
 from pydantic import BaseModel, Field
 
 from openagi.tools.base import BaseTool, tool
-from openagi.utils.yamlParse import read_yaml_config
+from openagi.utils.yamlParse import read_from_env
 
 
 def gmail_toolkit(searchString, llm):
-    credentials = read_yaml_config("GMAIL_CREDS")
+    credentials = read_from_env("GMAIL_CREDS")
     toolkit = GmailToolkit()
     base_prompt = hub.pull("langchain-ai/openai-functions-template")
     instructions = "Use the Gmail API to search for emails in your inbox and return the results."
     prompt = base_prompt.partial(instructions=instructions)
     agent = create_openai_functions_agent(llm, toolkit.get_tools(), prompt)
     agent_executor = AgentExecutor(
         agent=agent,
```

### Comparing `openagi-0.1.0b4/src/openagi/tools/integrations/google_finance_search.py` & `openagi-0.2.0b2/src/openagi/tools/integrations/google_finance_search.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,20 +4,20 @@
     AgentType,
     initialize_agent,
     load_tools,
 )
 from pydantic import BaseModel, Field
 
 from openagi.tools.base import BaseTool, tool
-from openagi.utils.yamlParse import read_yaml_config
+from openagi.utils.yamlParse import read_from_env
 
 
 def googleFinanceStockSearch(searchString, llm):
-    os.environ["SERPAPI_API_KEY"] = read_yaml_config("SERPER_API_KEY", raise_exception=True)
-    os.environ["SERP_API_KEY"] = read_yaml_config("SERPER_API_KEY", raise_exception=True)
+    os.environ["SERPAPI_API_KEY"] = read_from_env("SERPER_API_KEY", raise_exception=True)
+    os.environ["SERP_API_KEY"] = read_from_env("SERPER_API_KEY", raise_exception=True)
     tools = load_tools(["google-scholar", "google-finance"], llm=llm)
     agent = initialize_agent(
         tools, llm, agent=AgentType.ZERO_SHOT_REACT_DESCRIPTION, verbose=False
     )
     results = agent.run(searchString)
     return results
```

### Comparing `openagi-0.1.0b4/src/openagi/tools/integrations/google_serper_specific.py` & `openagi-0.2.0b2/src/openagi/tools/integrations/google_serper_specific.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import logging
 import os
 
 from langchain_community.utilities import GoogleSerperAPIWrapper
 from pydantic import BaseModel, Field
 
 from openagi.tools.base import BaseTool, tool
-from openagi.utils.yamlParse import read_yaml_config
+from openagi.utils.yamlParse import read_from_env
 
 
 class SerperSpecificInputSchema(BaseModel):
     search_str: str = Field(description="Search string to be passed to the input.")
 
 
 def getSerperScrapeForSpecificTypeAndPeriod(searchString, type="news", tbs="qdr:m"):
-    os.environ["SERPAPI_API_KEY"] = read_yaml_config("SERPER_API_KEY", raise_exception=True)
+    os.environ["SERPAPI_API_KEY"] = read_from_env("SERPER_API_KEY", raise_exception=True)
     search = GoogleSerperAPIWrapper(type=type, tbs=tbs)
     logging.debug(f"searchString: {searchString}, type: {type}, tbs: {tbs}")
     output = search.results(searchString)
     return output
 
 
 class SerperSpecificOutputSchema(BaseModel):
```

### Comparing `openagi-0.1.0b4/src/openagi/tools/integrations/googlejobsearch.py` & `openagi-0.2.0b2/src/openagi/tools/integrations/googlejobsearch.py`

 * *Files identical despite different names*

### Comparing `openagi-0.1.0b4/src/openagi/tools/integrations/googleserpersearch.py` & `openagi-0.2.0b2/src/openagi/tools/integrations/googleserpersearch.py`

 * *Files identical despite different names*

### Comparing `openagi-0.1.0b4/src/openagi/tools/integrations/nasa.py` & `openagi-0.2.0b2/src/openagi/tools/integrations/nasa.py`

 * *Files identical despite different names*

### Comparing `openagi-0.1.0b4/src/openagi/tools/integrations/open_weathermap.py` & `openagi-0.2.0b2/src/openagi/tools/integrations/open_weathermap.py`

 * *Files identical despite different names*

### Comparing `openagi-0.1.0b4/src/openagi/tools/integrations/polygon.py` & `openagi-0.2.0b2/src/openagi/tools/integrations/polygon.py`

 * *Files identical despite different names*

### Comparing `openagi-0.1.0b4/src/openagi/tools/integrations/serper_intermediate.py` & `openagi-0.2.0b2/src/openagi/tools/integrations/serper_intermediate.py`

 * *Files identical despite different names*

### Comparing `openagi-0.1.0b4/src/openagi/tools/integrations/sql.py` & `openagi-0.2.0b2/src/openagi/tools/integrations/sql.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 from langchain_community.agent_toolkits import (
     create_sql_agent,
 )
 from langchain_community.utilities.sql_database import SQLDatabase
 from pydantic import BaseModel, Field
 
 from openagi.tools.base import BaseTool, tool
-from openagi.utils.yamlParse import read_yaml_config
+from openagi.utils.yamlParse import read_from_env
 
 
 def sql_toolkit(searchString, llm):
-    sqlLiteDBName = read_yaml_config("sqlLiteDBName")
+    sqlLiteDBName = read_from_env("sqlLiteDBName")
     db = SQLDatabase.from_uri(sqlLiteDBName)
     agent_executor = create_sql_agent(llm, db=db, agent_type="openai-tools", verbose=True)
     result = agent_executor.invoke(searchString)
     logging.debug(result)
     return result
```

### Comparing `openagi-0.1.0b4/src/openagi/tools/integrations/wikipedia_tool.py` & `openagi-0.2.0b2/src/openagi/tools/integrations/wikipedia_tool.py`

 * *Files identical despite different names*

### Comparing `openagi-0.1.0b4/src/openagi/tools/integrations/xorbits.py` & `openagi-0.2.0b2/src/openagi/tools/integrations/xorbits.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import logging
 
 import pandas as pd
 from langchain_experimental.agents.agent_toolkits import create_xorbits_agent
 from pydantic import BaseModel, Field
 
 from openagi.tools.base import BaseTool, tool
-from openagi.utils.yamlParse import read_yaml_config
+from openagi.utils.yamlParse import read_from_env
 
 
 def xorbits_toolkit(searchString, llm):
-    xorbotsCSVFileName = read_yaml_config("xorbotsCSVFileName")
+    xorbotsCSVFileName = read_from_env("xorbotsCSVFileName")
     data = pd.read_csv(xorbotsCSVFileName)
     agent = create_xorbits_agent(llm, data, verbose=True, handle_parsing_errors=True)
     result = agent.run(searchString)
     logging.debug(result)
     return result
```

### Comparing `openagi-0.1.0b4/src/openagi/tools/integrations/yahoofinancenews.py` & `openagi-0.2.0b2/src/openagi/tools/integrations/yahoofinancenews.py`

 * *Files identical despite different names*

### Comparing `openagi-0.1.0b4/src/openagi/tools/integrations/youtubesearch.py` & `openagi-0.2.0b2/src/openagi/tools/integrations/youtubesearch.py`

 * *Files identical despite different names*

### Comparing `openagi-0.1.0b4/src/openagi/tools/tools_db.py` & `openagi-0.2.0b2/src/openagi/tools/tools_db.py`

 * *Files identical despite different names*

### Comparing `openagi-0.1.0b4/src/openagi/tools/utils.py` & `openagi-0.2.0b2/src/openagi/tools/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from exa_py import Exa
 from langchain.agents import (
     tool,
 )
 import threading
 from openagi.tools.integrations.duckducksearch import getDuckduckgoSearchResults
-from openagi.utils.yamlParse import read_yaml_config
+from openagi.utils.yamlParse import read_from_env
 
 g_num_of_HGI = 0
 lock = threading.Lock()
 
 def getToolExecutionResults(
     agentName, role, goal, backstrory, task, capability, tools_list, llm_api
 ):
@@ -70,26 +70,26 @@
         logging.debug(f"Number of HGI reduced to: {g_num_of_HGI}")
         if g_num_of_HGI == 0:
             return True
         else:
             return False
 
 def ExaAdvToolSetup():
-    exa = Exa(api_key=read_yaml_config("EXA_API_KEY", raise_exception=True))
+    exa = Exa(api_key=read_from_env("EXA_API_KEY", raise_exception=True))
 
     @tool
     def search(query: str, include_domains=None, start_published_date=None):
         """Search for a webpage based on the query.
         Set the optional include_domains (list[str]) parameter to restrict the search to a list of domains.
         Set the optional start_published_date (str) parameter to restrict the search to documents published after the date (YYYY-MM-DD).
         """
         return exa.search_and_contents(
             f"{query}",
             use_autoprompt=True,
-            num_results=read_yaml_config("EXA_NUM_SEARCH_RESULTS", raise_exception=True),
+            num_results=read_from_env("EXA_NUM_SEARCH_RESULTS", raise_exception=True),
             include_domains=include_domains,
             start_published_date=start_published_date,
         )
 
     @tool
     def find_similar(url: str):
         """Search for webpages similar to a given URL.
```

### Comparing `openagi-0.1.0b4/src/openagi/utils/llmTasks.py` & `openagi-0.2.0b2/src/openagi/utils/llmTasks.py`

 * *Files identical despite different names*

