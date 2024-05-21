# Comparing `tmp/streamlit-ai-assist-0.0.1.tar.gz` & `tmp/streamlit_ai_assist-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-ai-assist-0.0.1.tar", last modified: Tue May 21 20:50:16 2024, max compression
+gzip compressed data, was "streamlit_ai_assist-0.1.1.tar", last modified: Tue May 21 20:58:33 2024, max compression
```

## Comparing `streamlit-ai-assist-0.0.1.tar` & `streamlit_ai_assist-0.1.1.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 kaitlynhennacy   (501) staff       (20)        0 2024-05-21 20:50:16.085136 streamlit-ai-assist-0.0.1/
--rw-r--r--   0 kaitlynhennacy   (501) staff       (20)     1564 2024-05-21 03:10:31.000000 streamlit-ai-assist-0.0.1/LICENSE
--rw-r--r--   0 kaitlynhennacy   (501) staff       (20)       55 2024-05-21 03:10:31.000000 streamlit-ai-assist-0.0.1/MANIFEST.in
--rw-r--r--   0 kaitlynhennacy   (501) staff       (20)     2817 2024-05-21 20:50:16.084980 streamlit-ai-assist-0.0.1/PKG-INFO
--rw-r--r--   0 kaitlynhennacy   (501) staff       (20)     2514 2024-05-21 20:01:16.000000 streamlit-ai-assist-0.0.1/README.md
--rw-r--r--   0 kaitlynhennacy   (501) staff       (20)       38 2024-05-21 20:50:16.085194 streamlit-ai-assist-0.0.1/setup.cfg
--rw-r--r--   0 kaitlynhennacy   (501) staff       (20)     1276 2024-05-21 20:48:56.000000 streamlit-ai-assist-0.0.1/setup.py
-drwxr-xr-x   0 kaitlynhennacy   (501) staff       (20)        0 2024-05-21 20:50:16.030774 streamlit-ai-assist-0.0.1/streamlit_ai_assist/
--rw-r--r--   0 kaitlynhennacy   (501) staff       (20)     9492 2024-05-21 20:50:02.000000 streamlit-ai-assist-0.0.1/streamlit_ai_assist/__init__.py
-drwxr-xr-x   0 kaitlynhennacy   (501) staff       (20)        0 2024-05-21 20:50:16.031851 streamlit-ai-assist-0.0.1/streamlit_ai_assist/backend/
--rw-r--r--   0 kaitlynhennacy   (501) staff       (20)        0 2024-05-21 03:10:31.000000 streamlit-ai-assist-0.0.1/streamlit_ai_assist/backend/__init__.py
-drwxr-xr-x   0 kaitlynhennacy   (501) staff       (20)        0 2024-05-21 20:50:16.033118 streamlit-ai-assist-0.0.1/streamlit_ai_assist/backend/agents/
--rw-r--r--   0 kaitlynhennacy   (501) staff       (20)        0 2024-05-21 03:10:31.000000 streamlit-ai-assist-0.0.1/streamlit_ai_assist/backend/agents/__init__.py
--rw-r--r--   0 kaitlynhennacy   (501) staff       (20)     5119 2024-05-21 12:35:20.000000 streamlit-ai-assist-0.0.1/streamlit_ai_assist/backend/agents/conversational_agent.py
--rw-r--r--   0 kaitlynhennacy   (501) staff       (20)     5954 2024-05-21 03:10:31.000000 streamlit-ai-assist-0.0.1/streamlit_ai_assist/backend/agents/data_analyst_agent.py
--rw-r--r--   0 kaitlynhennacy   (501) staff       (20)      826 2024-05-21 12:35:20.000000 streamlit-ai-assist-0.0.1/streamlit_ai_assist/backend/agents/function_rewrite_agent.py
--rw-r--r--   0 kaitlynhennacy   (501) staff       (20)      812 2024-05-21 03:10:31.000000 streamlit-ai-assist-0.0.1/streamlit_ai_assist/backend/agents/llm.py
-drwxr-xr-x   0 kaitlynhennacy   (501) staff       (20)        0 2024-05-21 20:50:16.034525 streamlit-ai-assist-0.0.1/streamlit_ai_assist/backend/agents/prompts/
--rw-r--r--   0 kaitlynhennacy   (501) staff       (20)      170 2024-05-21 03:10:31.000000 streamlit-ai-assist-0.0.1/streamlit_ai_assist/backend/agents/prompts/__init__.py
--rw-r--r--   0 kaitlynhennacy   (501) staff       (20)     1627 2024-05-21 19:53:13.000000 streamlit-ai-assist-0.0.1/streamlit_ai_assist/backend/agents/prompts/conversational_prompt.py
--rw-r--r--   0 kaitlynhennacy   (501) staff       (20)     1654 2024-05-21 13:09:26.000000 streamlit-ai-assist-0.0.1/streamlit_ai_assist/backend/agents/prompts/data_analyst_prompt.py
--rw-r--r--   0 kaitlynhennacy   (501) staff       (20)     2882 2024-05-21 03:10:31.000000 streamlit-ai-assist-0.0.1/streamlit_ai_assist/backend/agents/prompts/function_rewrite_prompt.py
-drwxr-xr-x   0 kaitlynhennacy   (501) staff       (20)        0 2024-05-21 20:50:16.034842 streamlit-ai-assist-0.0.1/streamlit_ai_assist/backend/data/
--rw-r--r--   0 kaitlynhennacy   (501) staff       (20)        0 2024-05-21 03:10:31.000000 streamlit-ai-assist-0.0.1/streamlit_ai_assist/backend/data/__init__.py
--rw-r--r--   0 kaitlynhennacy   (501) staff       (20)      683 2024-05-21 03:10:31.000000 streamlit-ai-assist-0.0.1/streamlit_ai_assist/backend/data/database_connection.py
-drwxr-xr-x   0 kaitlynhennacy   (501) staff       (20)        0 2024-05-21 20:50:16.036185 streamlit-ai-assist-0.0.1/streamlit_ai_assist/backend/documents/
--rw-r--r--   0 kaitlynhennacy   (501) staff       (20)      101 2024-05-21 03:10:31.000000 streamlit-ai-assist-0.0.1/streamlit_ai_assist/backend/documents/__init__.py
--rw-r--r--   0 kaitlynhennacy   (501) staff       (20)      610 2024-05-21 03:10:31.000000 streamlit-ai-assist-0.0.1/streamlit_ai_assist/backend/documents/docs_to_function_names.py
--rw-r--r--   0 kaitlynhennacy   (501) staff       (20)      632 2024-05-21 03:10:31.000000 streamlit-ai-assist-0.0.1/streamlit_ai_assist/backend/documents/python_to_docs.py
-drwxr-xr-x   0 kaitlynhennacy   (501) staff       (20)        0 2024-05-21 20:50:16.036487 streamlit-ai-assist-0.0.1/streamlit_ai_assist/backend/github/
--rw-r--r--   0 kaitlynhennacy   (501) staff       (20)        0 2024-05-21 03:10:31.000000 streamlit-ai-assist-0.0.1/streamlit_ai_assist/backend/github/__init__.py
--rw-r--r--   0 kaitlynhennacy   (501) staff       (20)     2545 2024-05-21 03:10:31.000000 streamlit-ai-assist-0.0.1/streamlit_ai_assist/backend/github/repo_actions.py
-drwxr-xr-x   0 kaitlynhennacy   (501) staff       (20)        0 2024-05-21 20:50:16.037056 streamlit-ai-assist-0.0.1/streamlit_ai_assist/backend/interface/
--rw-r--r--   0 kaitlynhennacy   (501) staff       (20)        0 2024-05-21 03:10:31.000000 streamlit-ai-assist-0.0.1/streamlit_ai_assist/backend/interface/__init__.py
--rw-r--r--   0 kaitlynhennacy   (501) staff       (20)     3574 2024-05-21 12:35:20.000000 streamlit-ai-assist-0.0.1/streamlit_ai_assist/backend/interface/main.py
--rw-r--r--   0 kaitlynhennacy   (501) staff       (20)      549 2024-05-21 03:10:31.000000 streamlit-ai-assist-0.0.1/streamlit_ai_assist/backend/interface/renderable.py
-drwxr-xr-x   0 kaitlynhennacy   (501) staff       (20)        0 2024-05-21 20:50:16.037575 streamlit-ai-assist-0.0.1/streamlit_ai_assist/backend/retrieval/
--rw-r--r--   0 kaitlynhennacy   (501) staff       (20)       42 2024-05-21 03:10:31.000000 streamlit-ai-assist-0.0.1/streamlit_ai_assist/backend/retrieval/__init__.py
--rw-r--r--   0 kaitlynhennacy   (501) staff       (20)      725 2024-05-21 03:10:31.000000 streamlit-ai-assist-0.0.1/streamlit_ai_assist/backend/retrieval/retrieve_top_k.py
-drwxr-xr-x   0 kaitlynhennacy   (501) staff       (20)        0 2024-05-21 20:50:16.040770 streamlit-ai-assist-0.0.1/streamlit_ai_assist/backend/tools/
--rw-r--r--   0 kaitlynhennacy   (501) staff       (20)      230 2024-05-21 03:10:31.000000 streamlit-ai-assist-0.0.1/streamlit_ai_assist/backend/tools/__init__.py
--rw-r--r--   0 kaitlynhennacy   (501) staff       (20)      399 2024-05-21 03:10:31.000000 streamlit-ai-assist-0.0.1/streamlit_ai_assist/backend/tools/base.py
--rw-r--r--   0 kaitlynhennacy   (501) staff       (20)     1521 2024-05-21 03:10:31.000000 streamlit-ai-assist-0.0.1/streamlit_ai_assist/backend/tools/graph_tool.py
--rw-r--r--   0 kaitlynhennacy   (501) staff       (20)     2512 2024-05-21 03:10:31.000000 streamlit-ai-assist-0.0.1/streamlit_ai_assist/backend/tools/new_graph_tool.py
--rw-r--r--   0 kaitlynhennacy   (501) staff       (20)     1256 2024-05-21 03:10:31.000000 streamlit-ai-assist-0.0.1/streamlit_ai_assist/backend/tools/schema_tool.py
--rw-r--r--   0 kaitlynhennacy   (501) staff       (20)     1036 2024-05-21 03:10:31.000000 streamlit-ai-assist-0.0.1/streamlit_ai_assist/backend/tools/show_tables_tool.py
--rw-r--r--   0 kaitlynhennacy   (501) staff       (20)     1953 2024-05-21 03:10:31.000000 streamlit-ai-assist-0.0.1/streamlit_ai_assist/backend/tools/show_unique_tool.py
--rw-r--r--   0 kaitlynhennacy   (501) staff       (20)     1736 2024-05-21 03:10:31.000000 streamlit-ai-assist-0.0.1/streamlit_ai_assist/backend/tools/sql_tool.py
--rw-r--r--   0 kaitlynhennacy   (501) staff       (20)      303 2024-05-21 20:44:52.000000 streamlit-ai-assist-0.0.1/streamlit_ai_assist/example.py
-drwxr-xr-x   0 kaitlynhennacy   (501) staff       (20)        0 2024-05-21 20:50:16.029066 streamlit-ai-assist-0.0.1/streamlit_ai_assist/frontend/
-drwxr-xr-x   0 kaitlynhennacy   (501) staff       (20)        0 2024-05-21 20:50:16.044793 streamlit-ai-assist-0.0.1/streamlit_ai_assist/frontend/build/
--rw-r--r--   0 kaitlynhennacy   (501) staff       (20)      374 2024-05-21 19:35:11.000000 streamlit-ai-assist-0.0.1/streamlit_ai_assist/frontend/build/asset-manifest.json
--rw-r--r--   0 kaitlynhennacy   (501) staff       (20)   197459 2024-05-21 19:34:52.000000 streamlit-ai-assist-0.0.1/streamlit_ai_assist/frontend/build/bootstrap.min.css
--rw-r--r--   0 kaitlynhennacy   (501) staff       (20)      595 2024-05-21 19:35:11.000000 streamlit-ai-assist-0.0.1/streamlit_ai_assist/frontend/build/index.html
-drwxr-xr-x   0 kaitlynhennacy   (501) staff       (20)        0 2024-05-21 20:50:16.029290 streamlit-ai-assist-0.0.1/streamlit_ai_assist/frontend/build/static/
-drwxr-xr-x   0 kaitlynhennacy   (501) staff       (20)        0 2024-05-21 20:50:16.045381 streamlit-ai-assist-0.0.1/streamlit_ai_assist/frontend/build/static/css/
--rw-r--r--   0 kaitlynhennacy   (501) staff       (20)       69 2024-05-21 19:35:11.000000 streamlit-ai-assist-0.0.1/streamlit_ai_assist/frontend/build/static/css/main.00e66aec.css
--rw-r--r--   0 kaitlynhennacy   (501) staff       (20)      189 2024-05-21 19:35:11.000000 streamlit-ai-assist-0.0.1/streamlit_ai_assist/frontend/build/static/css/main.00e66aec.css.map
-drwxr-xr-x   0 kaitlynhennacy   (501) staff       (20)        0 2024-05-21 20:50:16.069152 streamlit-ai-assist-0.0.1/streamlit_ai_assist/frontend/build/static/js/
--rw-r--r--   0 kaitlynhennacy   (501) staff       (20)  4034331 2024-05-21 19:35:11.000000 streamlit-ai-assist-0.0.1/streamlit_ai_assist/frontend/build/static/js/main.d19c5144.js
--rw-r--r--   0 kaitlynhennacy   (501) staff       (20)     3305 2024-05-21 19:35:11.000000 streamlit-ai-assist-0.0.1/streamlit_ai_assist/frontend/build/static/js/main.d19c5144.js.LICENSE.txt
--rw-r--r--   0 kaitlynhennacy   (501) staff       (20)  1544991 2024-05-21 19:35:11.000000 streamlit-ai-assist-0.0.1/streamlit_ai_assist/frontend/build/static/js/main.d19c5144.js.map
--rw-r--r--   0 kaitlynhennacy   (501) staff       (20)     1612 2024-05-21 03:20:28.000000 streamlit-ai-assist-0.0.1/streamlit_ai_assist/graphing.py
-drwxr-xr-x   0 kaitlynhennacy   (501) staff       (20)        0 2024-05-21 20:50:16.031707 streamlit-ai-assist-0.0.1/streamlit_ai_assist.egg-info/
--rw-r--r--   0 kaitlynhennacy   (501) staff       (20)     2817 2024-05-21 20:50:15.000000 streamlit-ai-assist-0.0.1/streamlit_ai_assist.egg-info/PKG-INFO
--rw-r--r--   0 kaitlynhennacy   (501) staff       (20)     2414 2024-05-21 20:50:16.000000 streamlit-ai-assist-0.0.1/streamlit_ai_assist.egg-info/SOURCES.txt
--rw-r--r--   0 kaitlynhennacy   (501) staff       (20)        1 2024-05-21 20:50:15.000000 streamlit-ai-assist-0.0.1/streamlit_ai_assist.egg-info/dependency_links.txt
--rw-r--r--   0 kaitlynhennacy   (501) staff       (20)      383 2024-05-21 20:50:15.000000 streamlit-ai-assist-0.0.1/streamlit_ai_assist.egg-info/requires.txt
--rw-r--r--   0 kaitlynhennacy   (501) staff       (20)       20 2024-05-21 20:50:15.000000 streamlit-ai-assist-0.0.1/streamlit_ai_assist.egg-info/top_level.txt
+drwxr-xr-x   0 kaitlynhennacy   (501) staff       (20)        0 2024-05-21 20:58:33.426992 streamlit_ai_assist-0.1.1/
+-rw-r--r--   0 kaitlynhennacy   (501) staff       (20)     1564 2024-05-21 03:10:31.000000 streamlit_ai_assist-0.1.1/LICENSE
+-rw-r--r--   0 kaitlynhennacy   (501) staff       (20)       55 2024-05-21 03:10:31.000000 streamlit_ai_assist-0.1.1/MANIFEST.in
+-rw-r--r--   0 kaitlynhennacy   (501) staff       (20)     3584 2024-05-21 20:58:33.426710 streamlit_ai_assist-0.1.1/PKG-INFO
+-rw-r--r--   0 kaitlynhennacy   (501) staff       (20)     2514 2024-05-21 20:01:16.000000 streamlit_ai_assist-0.1.1/README.md
+-rw-r--r--   0 kaitlynhennacy   (501) staff       (20)       38 2024-05-21 20:58:33.427065 streamlit_ai_assist-0.1.1/setup.cfg
+-rw-r--r--   0 kaitlynhennacy   (501) staff       (20)     1276 2024-05-21 20:55:55.000000 streamlit_ai_assist-0.1.1/setup.py
+drwxr-xr-x   0 kaitlynhennacy   (501) staff       (20)        0 2024-05-21 20:58:33.375201 streamlit_ai_assist-0.1.1/streamlit_ai_assist/
+-rw-r--r--   0 kaitlynhennacy   (501) staff       (20)     9492 2024-05-21 20:50:02.000000 streamlit_ai_assist-0.1.1/streamlit_ai_assist/__init__.py
+drwxr-xr-x   0 kaitlynhennacy   (501) staff       (20)        0 2024-05-21 20:58:33.376340 streamlit_ai_assist-0.1.1/streamlit_ai_assist/backend/
+-rw-r--r--   0 kaitlynhennacy   (501) staff       (20)        0 2024-05-21 03:10:31.000000 streamlit_ai_assist-0.1.1/streamlit_ai_assist/backend/__init__.py
+drwxr-xr-x   0 kaitlynhennacy   (501) staff       (20)        0 2024-05-21 20:58:33.377550 streamlit_ai_assist-0.1.1/streamlit_ai_assist/backend/agents/
+-rw-r--r--   0 kaitlynhennacy   (501) staff       (20)        0 2024-05-21 03:10:31.000000 streamlit_ai_assist-0.1.1/streamlit_ai_assist/backend/agents/__init__.py
+-rw-r--r--   0 kaitlynhennacy   (501) staff       (20)     5119 2024-05-21 12:35:20.000000 streamlit_ai_assist-0.1.1/streamlit_ai_assist/backend/agents/conversational_agent.py
+-rw-r--r--   0 kaitlynhennacy   (501) staff       (20)     5954 2024-05-21 03:10:31.000000 streamlit_ai_assist-0.1.1/streamlit_ai_assist/backend/agents/data_analyst_agent.py
+-rw-r--r--   0 kaitlynhennacy   (501) staff       (20)      826 2024-05-21 12:35:20.000000 streamlit_ai_assist-0.1.1/streamlit_ai_assist/backend/agents/function_rewrite_agent.py
+-rw-r--r--   0 kaitlynhennacy   (501) staff       (20)      812 2024-05-21 03:10:31.000000 streamlit_ai_assist-0.1.1/streamlit_ai_assist/backend/agents/llm.py
+drwxr-xr-x   0 kaitlynhennacy   (501) staff       (20)        0 2024-05-21 20:58:33.379117 streamlit_ai_assist-0.1.1/streamlit_ai_assist/backend/agents/prompts/
+-rw-r--r--   0 kaitlynhennacy   (501) staff       (20)      170 2024-05-21 03:10:31.000000 streamlit_ai_assist-0.1.1/streamlit_ai_assist/backend/agents/prompts/__init__.py
+-rw-r--r--   0 kaitlynhennacy   (501) staff       (20)     1627 2024-05-21 19:53:13.000000 streamlit_ai_assist-0.1.1/streamlit_ai_assist/backend/agents/prompts/conversational_prompt.py
+-rw-r--r--   0 kaitlynhennacy   (501) staff       (20)     1654 2024-05-21 13:09:26.000000 streamlit_ai_assist-0.1.1/streamlit_ai_assist/backend/agents/prompts/data_analyst_prompt.py
+-rw-r--r--   0 kaitlynhennacy   (501) staff       (20)     2882 2024-05-21 03:10:31.000000 streamlit_ai_assist-0.1.1/streamlit_ai_assist/backend/agents/prompts/function_rewrite_prompt.py
+drwxr-xr-x   0 kaitlynhennacy   (501) staff       (20)        0 2024-05-21 20:58:33.379535 streamlit_ai_assist-0.1.1/streamlit_ai_assist/backend/data/
+-rw-r--r--   0 kaitlynhennacy   (501) staff       (20)        0 2024-05-21 03:10:31.000000 streamlit_ai_assist-0.1.1/streamlit_ai_assist/backend/data/__init__.py
+-rw-r--r--   0 kaitlynhennacy   (501) staff       (20)      683 2024-05-21 03:10:31.000000 streamlit_ai_assist-0.1.1/streamlit_ai_assist/backend/data/database_connection.py
+drwxr-xr-x   0 kaitlynhennacy   (501) staff       (20)        0 2024-05-21 20:58:33.380780 streamlit_ai_assist-0.1.1/streamlit_ai_assist/backend/documents/
+-rw-r--r--   0 kaitlynhennacy   (501) staff       (20)      101 2024-05-21 03:10:31.000000 streamlit_ai_assist-0.1.1/streamlit_ai_assist/backend/documents/__init__.py
+-rw-r--r--   0 kaitlynhennacy   (501) staff       (20)      610 2024-05-21 03:10:31.000000 streamlit_ai_assist-0.1.1/streamlit_ai_assist/backend/documents/docs_to_function_names.py
+-rw-r--r--   0 kaitlynhennacy   (501) staff       (20)      632 2024-05-21 03:10:31.000000 streamlit_ai_assist-0.1.1/streamlit_ai_assist/backend/documents/python_to_docs.py
+drwxr-xr-x   0 kaitlynhennacy   (501) staff       (20)        0 2024-05-21 20:58:33.381085 streamlit_ai_assist-0.1.1/streamlit_ai_assist/backend/github/
+-rw-r--r--   0 kaitlynhennacy   (501) staff       (20)        0 2024-05-21 03:10:31.000000 streamlit_ai_assist-0.1.1/streamlit_ai_assist/backend/github/__init__.py
+-rw-r--r--   0 kaitlynhennacy   (501) staff       (20)     2545 2024-05-21 03:10:31.000000 streamlit_ai_assist-0.1.1/streamlit_ai_assist/backend/github/repo_actions.py
+drwxr-xr-x   0 kaitlynhennacy   (501) staff       (20)        0 2024-05-21 20:58:33.381648 streamlit_ai_assist-0.1.1/streamlit_ai_assist/backend/interface/
+-rw-r--r--   0 kaitlynhennacy   (501) staff       (20)        0 2024-05-21 03:10:31.000000 streamlit_ai_assist-0.1.1/streamlit_ai_assist/backend/interface/__init__.py
+-rw-r--r--   0 kaitlynhennacy   (501) staff       (20)     3574 2024-05-21 12:35:20.000000 streamlit_ai_assist-0.1.1/streamlit_ai_assist/backend/interface/main.py
+-rw-r--r--   0 kaitlynhennacy   (501) staff       (20)      549 2024-05-21 03:10:31.000000 streamlit_ai_assist-0.1.1/streamlit_ai_assist/backend/interface/renderable.py
+drwxr-xr-x   0 kaitlynhennacy   (501) staff       (20)        0 2024-05-21 20:58:33.382208 streamlit_ai_assist-0.1.1/streamlit_ai_assist/backend/retrieval/
+-rw-r--r--   0 kaitlynhennacy   (501) staff       (20)       42 2024-05-21 03:10:31.000000 streamlit_ai_assist-0.1.1/streamlit_ai_assist/backend/retrieval/__init__.py
+-rw-r--r--   0 kaitlynhennacy   (501) staff       (20)      725 2024-05-21 03:10:31.000000 streamlit_ai_assist-0.1.1/streamlit_ai_assist/backend/retrieval/retrieve_top_k.py
+drwxr-xr-x   0 kaitlynhennacy   (501) staff       (20)        0 2024-05-21 20:58:33.385497 streamlit_ai_assist-0.1.1/streamlit_ai_assist/backend/tools/
+-rw-r--r--   0 kaitlynhennacy   (501) staff       (20)      230 2024-05-21 03:10:31.000000 streamlit_ai_assist-0.1.1/streamlit_ai_assist/backend/tools/__init__.py
+-rw-r--r--   0 kaitlynhennacy   (501) staff       (20)      399 2024-05-21 03:10:31.000000 streamlit_ai_assist-0.1.1/streamlit_ai_assist/backend/tools/base.py
+-rw-r--r--   0 kaitlynhennacy   (501) staff       (20)     1521 2024-05-21 03:10:31.000000 streamlit_ai_assist-0.1.1/streamlit_ai_assist/backend/tools/graph_tool.py
+-rw-r--r--   0 kaitlynhennacy   (501) staff       (20)     2512 2024-05-21 03:10:31.000000 streamlit_ai_assist-0.1.1/streamlit_ai_assist/backend/tools/new_graph_tool.py
+-rw-r--r--   0 kaitlynhennacy   (501) staff       (20)     1256 2024-05-21 03:10:31.000000 streamlit_ai_assist-0.1.1/streamlit_ai_assist/backend/tools/schema_tool.py
+-rw-r--r--   0 kaitlynhennacy   (501) staff       (20)     1036 2024-05-21 03:10:31.000000 streamlit_ai_assist-0.1.1/streamlit_ai_assist/backend/tools/show_tables_tool.py
+-rw-r--r--   0 kaitlynhennacy   (501) staff       (20)     1953 2024-05-21 03:10:31.000000 streamlit_ai_assist-0.1.1/streamlit_ai_assist/backend/tools/show_unique_tool.py
+-rw-r--r--   0 kaitlynhennacy   (501) staff       (20)     1736 2024-05-21 03:10:31.000000 streamlit_ai_assist-0.1.1/streamlit_ai_assist/backend/tools/sql_tool.py
+-rw-r--r--   0 kaitlynhennacy   (501) staff       (20)      303 2024-05-21 20:44:52.000000 streamlit_ai_assist-0.1.1/streamlit_ai_assist/example.py
+drwxr-xr-x   0 kaitlynhennacy   (501) staff       (20)        0 2024-05-21 20:58:33.373354 streamlit_ai_assist-0.1.1/streamlit_ai_assist/frontend/
+drwxr-xr-x   0 kaitlynhennacy   (501) staff       (20)        0 2024-05-21 20:58:33.387877 streamlit_ai_assist-0.1.1/streamlit_ai_assist/frontend/build/
+-rw-r--r--   0 kaitlynhennacy   (501) staff       (20)      374 2024-05-21 20:57:02.000000 streamlit_ai_assist-0.1.1/streamlit_ai_assist/frontend/build/asset-manifest.json
+-rw-r--r--   0 kaitlynhennacy   (501) staff       (20)   197459 2024-05-21 20:56:43.000000 streamlit_ai_assist-0.1.1/streamlit_ai_assist/frontend/build/bootstrap.min.css
+-rw-r--r--   0 kaitlynhennacy   (501) staff       (20)      595 2024-05-21 20:57:02.000000 streamlit_ai_assist-0.1.1/streamlit_ai_assist/frontend/build/index.html
+drwxr-xr-x   0 kaitlynhennacy   (501) staff       (20)        0 2024-05-21 20:58:33.373609 streamlit_ai_assist-0.1.1/streamlit_ai_assist/frontend/build/static/
+drwxr-xr-x   0 kaitlynhennacy   (501) staff       (20)        0 2024-05-21 20:58:33.388481 streamlit_ai_assist-0.1.1/streamlit_ai_assist/frontend/build/static/css/
+-rw-r--r--   0 kaitlynhennacy   (501) staff       (20)       69 2024-05-21 20:57:02.000000 streamlit_ai_assist-0.1.1/streamlit_ai_assist/frontend/build/static/css/main.00e66aec.css
+-rw-r--r--   0 kaitlynhennacy   (501) staff       (20)      189 2024-05-21 20:57:02.000000 streamlit_ai_assist-0.1.1/streamlit_ai_assist/frontend/build/static/css/main.00e66aec.css.map
+drwxr-xr-x   0 kaitlynhennacy   (501) staff       (20)        0 2024-05-21 20:58:33.409449 streamlit_ai_assist-0.1.1/streamlit_ai_assist/frontend/build/static/js/
+-rw-r--r--   0 kaitlynhennacy   (501) staff       (20)  4034331 2024-05-21 20:57:02.000000 streamlit_ai_assist-0.1.1/streamlit_ai_assist/frontend/build/static/js/main.d19c5144.js
+-rw-r--r--   0 kaitlynhennacy   (501) staff       (20)     3305 2024-05-21 20:57:02.000000 streamlit_ai_assist-0.1.1/streamlit_ai_assist/frontend/build/static/js/main.d19c5144.js.LICENSE.txt
+-rw-r--r--   0 kaitlynhennacy   (501) staff       (20)  1544991 2024-05-21 20:57:02.000000 streamlit_ai_assist-0.1.1/streamlit_ai_assist/frontend/build/static/js/main.d19c5144.js.map
+-rw-r--r--   0 kaitlynhennacy   (501) staff       (20)     1612 2024-05-21 03:20:28.000000 streamlit_ai_assist-0.1.1/streamlit_ai_assist/graphing.py
+drwxr-xr-x   0 kaitlynhennacy   (501) staff       (20)        0 2024-05-21 20:58:33.425889 streamlit_ai_assist-0.1.1/streamlit_ai_assist.egg-info/
+-rw-r--r--   0 kaitlynhennacy   (501) staff       (20)     3584 2024-05-21 20:58:33.000000 streamlit_ai_assist-0.1.1/streamlit_ai_assist.egg-info/PKG-INFO
+-rw-r--r--   0 kaitlynhennacy   (501) staff       (20)     2414 2024-05-21 20:58:33.000000 streamlit_ai_assist-0.1.1/streamlit_ai_assist.egg-info/SOURCES.txt
+-rw-r--r--   0 kaitlynhennacy   (501) staff       (20)        1 2024-05-21 20:58:33.000000 streamlit_ai_assist-0.1.1/streamlit_ai_assist.egg-info/dependency_links.txt
+-rw-r--r--   0 kaitlynhennacy   (501) staff       (20)      383 2024-05-21 20:58:33.000000 streamlit_ai_assist-0.1.1/streamlit_ai_assist.egg-info/requires.txt
+-rw-r--r--   0 kaitlynhennacy   (501) staff       (20)       20 2024-05-21 20:58:33.000000 streamlit_ai_assist-0.1.1/streamlit_ai_assist.egg-info/top_level.txt
```

### Comparing `streamlit-ai-assist-0.0.1/LICENSE` & `streamlit_ai_assist-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-ai-assist-0.0.1/PKG-INFO` & `streamlit_ai_assist-0.1.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: streamlit-ai-assist
-Version: 0.0.1
-Summary: A built in data analyst for your Streamlit app
-Home-page: 
-Author: Kaitlyn Hennacy
-Author-email: kaitlynhennacy@gmail.com
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: devel
-License-File: LICENSE
-
 # streamlit-ai-assist
 
 `streamlit-ai-assist` uses the power of [Snowflake Arctic](https://www.snowflake.com/blog/arctic-open-efficient-foundation-language-models-snowflake/), an open_source LLM, to personalize dashboards and allow all audiences to easily explore new and pre-built data visualizations. It's a built-in data analyst for your Streamlit dashboard.
 
 If you add this component to your dashboard, dashboard viewers will be able to chat with an LLM assistant to get answers to their questions. If there are relevant graphs already in the dashboard, then the assistant will display those. If the question requires a new graph, the LLM is able to write the code to create that. These **new graphs** are highlighted in yellow, and if GitHub connection is configured in the app, then the user will be allowed to easily create a **PR** that integrates the code into the dashboard once reviewed and approved by a team member.
 
 If a user has a particular question, the AI assistant can execute SQL `SELECT` statements that let it access the raw numbers. It can summarize graphs for you and return answers to a quick question you have.
@@ -73,8 +61,8 @@
 
 ### Optional Environment Variables
 ```
 GITHUB_PERSONAL_ACCESS_TOKEN
 REPO_NAME
 REPO_OWNER
 ```
-If these are specified, GitHub PR automation will be enabled.
+If these are specified, GitHub PR automation will be enabled.
```

### Comparing `streamlit-ai-assist-0.0.1/setup.py` & `streamlit_ai_assist-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="streamlit-ai-assist",
-    version="0.0.1",
+    version="0.1.1",
     author="Kaitlyn Hennacy",
     author_email="kaitlynhennacy@gmail.com",
     description="A built in data analyst for your Streamlit app",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

### Comparing `streamlit-ai-assist-0.0.1/streamlit_ai_assist/__init__.py` & `streamlit_ai_assist-0.1.1/streamlit_ai_assist/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-ai-assist-0.0.1/streamlit_ai_assist/backend/agents/conversational_agent.py` & `streamlit_ai_assist-0.1.1/streamlit_ai_assist/backend/agents/conversational_agent.py`

 * *Files identical despite different names*

### Comparing `streamlit-ai-assist-0.0.1/streamlit_ai_assist/backend/agents/data_analyst_agent.py` & `streamlit_ai_assist-0.1.1/streamlit_ai_assist/backend/agents/data_analyst_agent.py`

 * *Files identical despite different names*

### Comparing `streamlit-ai-assist-0.0.1/streamlit_ai_assist/backend/agents/function_rewrite_agent.py` & `streamlit_ai_assist-0.1.1/streamlit_ai_assist/backend/agents/function_rewrite_agent.py`

 * *Files identical despite different names*

### Comparing `streamlit-ai-assist-0.0.1/streamlit_ai_assist/backend/agents/llm.py` & `streamlit_ai_assist-0.1.1/streamlit_ai_assist/backend/agents/llm.py`

 * *Files identical despite different names*

### Comparing `streamlit-ai-assist-0.0.1/streamlit_ai_assist/backend/agents/prompts/conversational_prompt.py` & `streamlit_ai_assist-0.1.1/streamlit_ai_assist/backend/agents/prompts/conversational_prompt.py`

 * *Files identical despite different names*

### Comparing `streamlit-ai-assist-0.0.1/streamlit_ai_assist/backend/agents/prompts/data_analyst_prompt.py` & `streamlit_ai_assist-0.1.1/streamlit_ai_assist/backend/agents/prompts/data_analyst_prompt.py`

 * *Files identical despite different names*

### Comparing `streamlit-ai-assist-0.0.1/streamlit_ai_assist/backend/agents/prompts/function_rewrite_prompt.py` & `streamlit_ai_assist-0.1.1/streamlit_ai_assist/backend/agents/prompts/function_rewrite_prompt.py`

 * *Files identical despite different names*

### Comparing `streamlit-ai-assist-0.0.1/streamlit_ai_assist/backend/data/database_connection.py` & `streamlit_ai_assist-0.1.1/streamlit_ai_assist/backend/data/database_connection.py`

 * *Files identical despite different names*

### Comparing `streamlit-ai-assist-0.0.1/streamlit_ai_assist/backend/documents/docs_to_function_names.py` & `streamlit_ai_assist-0.1.1/streamlit_ai_assist/backend/documents/docs_to_function_names.py`

 * *Files identical despite different names*

### Comparing `streamlit-ai-assist-0.0.1/streamlit_ai_assist/backend/documents/python_to_docs.py` & `streamlit_ai_assist-0.1.1/streamlit_ai_assist/backend/documents/python_to_docs.py`

 * *Files identical despite different names*

### Comparing `streamlit-ai-assist-0.0.1/streamlit_ai_assist/backend/github/repo_actions.py` & `streamlit_ai_assist-0.1.1/streamlit_ai_assist/backend/github/repo_actions.py`

 * *Files identical despite different names*

### Comparing `streamlit-ai-assist-0.0.1/streamlit_ai_assist/backend/interface/main.py` & `streamlit_ai_assist-0.1.1/streamlit_ai_assist/backend/interface/main.py`

 * *Files identical despite different names*

### Comparing `streamlit-ai-assist-0.0.1/streamlit_ai_assist/backend/interface/renderable.py` & `streamlit_ai_assist-0.1.1/streamlit_ai_assist/backend/interface/renderable.py`

 * *Files identical despite different names*

### Comparing `streamlit-ai-assist-0.0.1/streamlit_ai_assist/backend/retrieval/retrieve_top_k.py` & `streamlit_ai_assist-0.1.1/streamlit_ai_assist/backend/retrieval/retrieve_top_k.py`

 * *Files identical despite different names*

### Comparing `streamlit-ai-assist-0.0.1/streamlit_ai_assist/backend/tools/graph_tool.py` & `streamlit_ai_assist-0.1.1/streamlit_ai_assist/backend/tools/graph_tool.py`

 * *Files identical despite different names*

### Comparing `streamlit-ai-assist-0.0.1/streamlit_ai_assist/backend/tools/new_graph_tool.py` & `streamlit_ai_assist-0.1.1/streamlit_ai_assist/backend/tools/new_graph_tool.py`

 * *Files identical despite different names*

### Comparing `streamlit-ai-assist-0.0.1/streamlit_ai_assist/backend/tools/schema_tool.py` & `streamlit_ai_assist-0.1.1/streamlit_ai_assist/backend/tools/schema_tool.py`

 * *Files identical despite different names*

### Comparing `streamlit-ai-assist-0.0.1/streamlit_ai_assist/backend/tools/show_tables_tool.py` & `streamlit_ai_assist-0.1.1/streamlit_ai_assist/backend/tools/show_tables_tool.py`

 * *Files identical despite different names*

### Comparing `streamlit-ai-assist-0.0.1/streamlit_ai_assist/backend/tools/show_unique_tool.py` & `streamlit_ai_assist-0.1.1/streamlit_ai_assist/backend/tools/show_unique_tool.py`

 * *Files identical despite different names*

### Comparing `streamlit-ai-assist-0.0.1/streamlit_ai_assist/backend/tools/sql_tool.py` & `streamlit_ai_assist-0.1.1/streamlit_ai_assist/backend/tools/sql_tool.py`

 * *Files identical despite different names*

### Comparing `streamlit-ai-assist-0.0.1/streamlit_ai_assist/frontend/build/bootstrap.min.css` & `streamlit_ai_assist-0.1.1/streamlit_ai_assist/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `streamlit-ai-assist-0.0.1/streamlit_ai_assist/frontend/build/index.html` & `streamlit_ai_assist-0.1.1/streamlit_ai_assist/frontend/build/index.html`

 * *Files identical despite different names*

### Comparing `streamlit-ai-assist-0.0.1/streamlit_ai_assist/frontend/build/static/js/main.d19c5144.js` & `streamlit_ai_assist-0.1.1/streamlit_ai_assist/frontend/build/static/js/main.d19c5144.js`

 * *Files identical despite different names*

### Comparing `streamlit-ai-assist-0.0.1/streamlit_ai_assist/frontend/build/static/js/main.d19c5144.js.LICENSE.txt` & `streamlit_ai_assist-0.1.1/streamlit_ai_assist/frontend/build/static/js/main.d19c5144.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit-ai-assist-0.0.1/streamlit_ai_assist/frontend/build/static/js/main.d19c5144.js.map` & `streamlit_ai_assist-0.1.1/streamlit_ai_assist/frontend/build/static/js/main.d19c5144.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-ai-assist-0.0.1/streamlit_ai_assist/graphing.py` & `streamlit_ai_assist-0.1.1/streamlit_ai_assist/graphing.py`

 * *Files identical despite different names*

### Comparing `streamlit-ai-assist-0.0.1/streamlit_ai_assist.egg-info/SOURCES.txt` & `streamlit_ai_assist-0.1.1/streamlit_ai_assist.egg-info/SOURCES.txt`

 * *Files identical despite different names*

