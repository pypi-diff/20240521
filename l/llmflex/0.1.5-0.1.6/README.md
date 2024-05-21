# Comparing `tmp/llmflex-0.1.5.tar.gz` & `tmp/llmflex-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmflex-0.1.5.tar", last modified: Sun Apr 21 17:43:26 2024, max compression
+gzip compressed data, was "llmflex-0.1.6.tar", last modified: Tue May 21 17:59:46 2024, max compression
```

## Comparing `llmflex-0.1.5.tar` & `llmflex-0.1.6.tar`

### file list

```diff
@@ -1,76 +1,79 @@
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-21 17:43:26.245627 llmflex-0.1.5/
--rw-r--r--   0 nathan95   (501) staff       (20)     1067 2024-01-22 01:35:14.000000 llmflex-0.1.5/LICENSE.md
--rw-r--r--   0 nathan95   (501) staff       (20)     9764 2024-04-21 17:43:26.245377 llmflex-0.1.5/PKG-INFO
--rw-r--r--   0 nathan95   (501) staff       (20)     8569 2024-04-09 19:26:07.000000 llmflex-0.1.5/README.md
--rw-r--r--   0 nathan95   (501) staff       (20)     1210 2024-04-21 17:42:51.000000 llmflex-0.1.5/pyproject.toml
--rw-r--r--   0 nathan95   (501) staff       (20)       38 2024-04-21 17:43:26.245668 llmflex-0.1.5/setup.cfg
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-21 17:43:26.235267 llmflex-0.1.5/src/
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-21 17:43:26.237067 llmflex-0.1.5/src/llmflex/
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-21 17:43:26.238376 llmflex-0.1.5/src/llmflex/Data/
--rw-r--r--   0 nathan95   (501) staff       (20)       43 2024-03-11 17:44:28.000000 llmflex-0.1.5/src/llmflex/Data/__init__.py
--rw-r--r--   0 nathan95   (501) staff       (20)     4919 2024-02-24 22:31:02.000000 llmflex-0.1.5/src/llmflex/Data/sqlite_database.py
--rw-r--r--   0 nathan95   (501) staff       (20)    20029 2024-03-11 17:44:28.000000 llmflex-0.1.5/src/llmflex/Data/vector_database.py
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-21 17:43:26.239098 llmflex-0.1.5/src/llmflex/Embeddings/
--rw-r--r--   0 nathan95   (501) staff       (20)      226 2024-02-24 22:31:02.000000 llmflex-0.1.5/src/llmflex/Embeddings/__init__.py
--rw-r--r--   0 nathan95   (501) staff       (20)     4555 2024-04-21 17:42:51.000000 llmflex-0.1.5/src/llmflex/Embeddings/api_embeddings.py
--rw-r--r--   0 nathan95   (501) staff       (20)     4608 2024-04-21 17:42:51.000000 llmflex-0.1.5/src/llmflex/Embeddings/base_embeddings.py
--rw-r--r--   0 nathan95   (501) staff       (20)     2275 2024-03-15 22:38:26.000000 llmflex-0.1.5/src/llmflex/Embeddings/hf_embeddings_server.py
--rw-r--r--   0 nathan95   (501) staff       (20)     4147 2024-04-21 17:42:51.000000 llmflex-0.1.5/src/llmflex/Embeddings/huggingface_embeddings.py
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-21 17:43:26.239535 llmflex-0.1.5/src/llmflex/Frontend/
--rw-r--r--   0 nathan95   (501) staff       (20)      102 2024-02-24 22:31:02.000000 llmflex-0.1.5/src/llmflex/Frontend/__init__.py
--rw-r--r--   0 nathan95   (501) staff       (20)    29992 2024-02-24 22:31:02.000000 llmflex-0.1.5/src/llmflex/Frontend/gradio_interface.py
--rw-r--r--   0 nathan95   (501) staff       (20)    37412 2024-04-14 12:29:06.000000 llmflex-0.1.5/src/llmflex/Frontend/streamlit_interface.py
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-21 17:43:26.240049 llmflex-0.1.5/src/llmflex/Memory/
--rw-r--r--   0 nathan95   (501) staff       (20)      287 2024-02-24 22:31:02.000000 llmflex-0.1.5/src/llmflex/Memory/__init__.py
--rw-r--r--   0 nathan95   (501) staff       (20)     8298 2024-03-11 17:44:28.000000 llmflex-0.1.5/src/llmflex/Memory/assistant_long_term_memory.py
--rw-r--r--   0 nathan95   (501) staff       (20)     8703 2024-03-11 17:44:28.000000 llmflex-0.1.5/src/llmflex/Memory/base_memory.py
--rw-r--r--   0 nathan95   (501) staff       (20)     7727 2024-03-11 17:44:28.000000 llmflex-0.1.5/src/llmflex/Memory/long_short_memory.py
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-21 17:43:26.240161 llmflex-0.1.5/src/llmflex/Models/
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-21 17:43:26.241073 llmflex-0.1.5/src/llmflex/Models/Cores/
--rw-r--r--   0 nathan95   (501) staff       (20)        0 2024-02-24 22:31:02.000000 llmflex-0.1.5/src/llmflex/Models/Cores/__init__.py
--rw-r--r--   0 nathan95   (501) staff       (20)    14710 2024-04-14 12:29:06.000000 llmflex-0.1.5/src/llmflex/Models/Cores/base_core.py
--rw-r--r--   0 nathan95   (501) staff       (20)     7915 2024-02-25 22:17:53.000000 llmflex-0.1.5/src/llmflex/Models/Cores/exllamav2_core.py
--rw-r--r--   0 nathan95   (501) staff       (20)     9508 2024-03-11 17:44:28.000000 llmflex-0.1.5/src/llmflex/Models/Cores/huggingface_core.py
--rw-r--r--   0 nathan95   (501) staff       (20)     8610 2024-02-25 22:17:53.000000 llmflex-0.1.5/src/llmflex/Models/Cores/llamacpp_core.py
--rw-r--r--   0 nathan95   (501) staff       (20)     9425 2024-04-14 12:29:06.000000 llmflex-0.1.5/src/llmflex/Models/Cores/openai_core.py
--rw-r--r--   0 nathan95   (501) staff       (20)     7398 2024-04-21 17:42:51.000000 llmflex-0.1.5/src/llmflex/Models/Cores/utils.py
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-21 17:43:26.241305 llmflex-0.1.5/src/llmflex/Models/Factory/
--rw-r--r--   0 nathan95   (501) staff       (20)        0 2024-02-24 22:31:02.000000 llmflex-0.1.5/src/llmflex/Models/Factory/__init__.py
--rw-r--r--   0 nathan95   (501) staff       (20)    10723 2024-04-14 12:29:06.000000 llmflex-0.1.5/src/llmflex/Models/Factory/llm_factory.py
--rw-r--r--   0 nathan95   (501) staff       (20)       43 2024-02-24 22:31:02.000000 llmflex-0.1.5/src/llmflex/Models/__init__.py
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-21 17:43:26.241722 llmflex-0.1.5/src/llmflex/Prompts/
--rw-r--r--   0 nathan95   (501) staff       (20)       52 2024-02-24 22:31:02.000000 llmflex-0.1.5/src/llmflex/Prompts/__init__.py
--rw-r--r--   0 nathan95   (501) staff       (20)    15747 2024-04-21 17:42:51.000000 llmflex-0.1.5/src/llmflex/Prompts/prompt_template.py
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-21 17:43:26.242257 llmflex-0.1.5/src/llmflex/Rankers/
--rw-r--r--   0 nathan95   (501) staff       (20)       81 2024-04-21 17:42:51.000000 llmflex-0.1.5/src/llmflex/Rankers/__init__.py
--rw-r--r--   0 nathan95   (501) staff       (20)     1471 2024-04-21 17:42:51.000000 llmflex-0.1.5/src/llmflex/Rankers/base_ranker.py
--rw-r--r--   0 nathan95   (501) staff       (20)     2309 2024-04-21 17:42:51.000000 llmflex-0.1.5/src/llmflex/Rankers/flashrank_ranker.py
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-21 17:43:26.242705 llmflex-0.1.5/src/llmflex/Schemas/
--rw-r--r--   0 nathan95   (501) staff       (20)       64 2024-04-21 17:42:51.000000 llmflex-0.1.5/src/llmflex/Schemas/__init__.py
--rw-r--r--   0 nathan95   (501) staff       (20)     1414 2024-04-21 17:42:51.000000 llmflex-0.1.5/src/llmflex/Schemas/documents.py
--rw-r--r--   0 nathan95   (501) staff       (20)     2429 2024-04-21 17:42:51.000000 llmflex-0.1.5/src/llmflex/Schemas/tokenizer.py
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-21 17:43:26.243285 llmflex-0.1.5/src/llmflex/TextSplitters/
--rw-r--r--   0 nathan95   (501) staff       (20)      123 2024-03-11 17:44:28.000000 llmflex-0.1.5/src/llmflex/TextSplitters/__init__.py
--rw-r--r--   0 nathan95   (501) staff       (20)     1526 2024-03-11 17:44:28.000000 llmflex-0.1.5/src/llmflex/TextSplitters/base_text_splitter.py
--rw-r--r--   0 nathan95   (501) staff       (20)     2709 2024-03-11 17:44:28.000000 llmflex-0.1.5/src/llmflex/TextSplitters/sentence_token_text_splitter.py
--rw-r--r--   0 nathan95   (501) staff       (20)     1423 2024-04-21 17:42:51.000000 llmflex-0.1.5/src/llmflex/TextSplitters/token_text_splitter.py
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-21 17:43:26.244035 llmflex-0.1.5/src/llmflex/Tools/
--rw-r--r--   0 nathan95   (501) staff       (20)      115 2024-02-24 22:31:02.000000 llmflex-0.1.5/src/llmflex/Tools/__init__.py
--rw-r--r--   0 nathan95   (501) staff       (20)    11795 2024-02-24 22:31:02.000000 llmflex-0.1.5/src/llmflex/Tools/base_tool.py
--rw-r--r--   0 nathan95   (501) staff       (20)     6603 2024-03-11 17:44:28.000000 llmflex-0.1.5/src/llmflex/Tools/tool_selection.py
--rw-r--r--   0 nathan95   (501) staff       (20)    11421 2024-04-21 17:42:51.000000 llmflex-0.1.5/src/llmflex/Tools/web_search_tool.py
--rw-r--r--   0 nathan95   (501) staff       (20)    14485 2024-04-21 17:42:51.000000 llmflex-0.1.5/src/llmflex/Tools/web_search_utils.py
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-21 17:43:26.244560 llmflex-0.1.5/src/llmflex/VectorDBs/
--rw-r--r--   0 nathan95   (501) staff       (20)       93 2024-03-11 17:44:28.000000 llmflex-0.1.5/src/llmflex/VectorDBs/__init__.py
--rw-r--r--   0 nathan95   (501) staff       (20)    24481 2024-04-21 17:42:51.000000 llmflex-0.1.5/src/llmflex/VectorDBs/base_vectordb.py
--rw-r--r--   0 nathan95   (501) staff       (20)     5362 2024-04-21 17:42:51.000000 llmflex-0.1.5/src/llmflex/VectorDBs/faiss_vectordb.py
--rw-r--r--   0 nathan95   (501) staff       (20)      275 2024-04-21 17:42:51.000000 llmflex-0.1.5/src/llmflex/__init__.py
--rw-r--r--   0 nathan95   (501) staff       (20)     4381 2024-02-24 22:31:02.000000 llmflex-0.1.5/src/llmflex/cli.py
--rw-r--r--   0 nathan95   (501) staff       (20)     6178 2024-03-11 17:44:28.000000 llmflex-0.1.5/src/llmflex/utils.py
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-21 17:43:26.244774 llmflex-0.1.5/src/llmflex.egg-info/
--rw-r--r--   0 nathan95   (501) staff       (20)     9764 2024-04-21 17:43:26.000000 llmflex-0.1.5/src/llmflex.egg-info/PKG-INFO
--rw-r--r--   0 nathan95   (501) staff       (20)     2043 2024-04-21 17:43:26.000000 llmflex-0.1.5/src/llmflex.egg-info/SOURCES.txt
--rw-r--r--   0 nathan95   (501) staff       (20)        1 2024-04-21 17:43:26.000000 llmflex-0.1.5/src/llmflex.egg-info/dependency_links.txt
--rw-r--r--   0 nathan95   (501) staff       (20)       44 2024-04-21 17:43:26.000000 llmflex-0.1.5/src/llmflex.egg-info/entry_points.txt
--rw-r--r--   0 nathan95   (501) staff       (20)      337 2024-04-21 17:43:26.000000 llmflex-0.1.5/src/llmflex.egg-info/requires.txt
--rw-r--r--   0 nathan95   (501) staff       (20)        8 2024-04-21 17:43:26.000000 llmflex-0.1.5/src/llmflex.egg-info/top_level.txt
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-05-21 17:59:46.289543 llmflex-0.1.6/
+-rw-r--r--   0 nathan95   (501) staff       (20)     1067 2024-01-22 01:35:14.000000 llmflex-0.1.6/LICENSE.md
+-rw-r--r--   0 nathan95   (501) staff       (20)    10171 2024-05-21 17:59:46.289237 llmflex-0.1.6/PKG-INFO
+-rw-r--r--   0 nathan95   (501) staff       (20)     8926 2024-05-21 17:59:14.000000 llmflex-0.1.6/README.md
+-rw-r--r--   0 nathan95   (501) staff       (20)     1244 2024-05-21 17:59:14.000000 llmflex-0.1.6/pyproject.toml
+-rw-r--r--   0 nathan95   (501) staff       (20)       38 2024-05-21 17:59:46.289610 llmflex-0.1.6/setup.cfg
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-05-21 17:59:46.278376 llmflex-0.1.6/src/
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-05-21 17:59:46.280372 llmflex-0.1.6/src/llmflex/
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-05-21 17:59:46.282001 llmflex-0.1.6/src/llmflex/Embeddings/
+-rw-r--r--   0 nathan95   (501) staff       (20)      226 2024-02-24 22:31:02.000000 llmflex-0.1.6/src/llmflex/Embeddings/__init__.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     4555 2024-04-21 17:42:51.000000 llmflex-0.1.6/src/llmflex/Embeddings/api_embeddings.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     4608 2024-04-21 17:42:51.000000 llmflex-0.1.6/src/llmflex/Embeddings/base_embeddings.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     2275 2024-03-15 22:38:26.000000 llmflex-0.1.6/src/llmflex/Embeddings/hf_embeddings_server.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     4147 2024-04-21 17:42:51.000000 llmflex-0.1.6/src/llmflex/Embeddings/huggingface_embeddings.py
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-05-21 17:59:46.282454 llmflex-0.1.6/src/llmflex/Frontend/
+-rw-r--r--   0 nathan95   (501) staff       (20)      102 2024-02-24 22:31:02.000000 llmflex-0.1.6/src/llmflex/Frontend/__init__.py
+-rw-r--r--   0 nathan95   (501) staff       (20)    29992 2024-02-24 22:31:02.000000 llmflex-0.1.6/src/llmflex/Frontend/gradio_interface.py
+-rw-r--r--   0 nathan95   (501) staff       (20)    37304 2024-05-21 17:59:14.000000 llmflex-0.1.6/src/llmflex/Frontend/streamlit_interface.py
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-05-21 17:59:46.282741 llmflex-0.1.6/src/llmflex/KnowledgeBase/
+-rw-r--r--   0 nathan95   (501) staff       (20)      108 2024-05-21 17:59:14.000000 llmflex-0.1.6/src/llmflex/KnowledgeBase/__init__.py
+-rw-r--r--   0 nathan95   (501) staff       (20)    13135 2024-05-21 17:59:14.000000 llmflex-0.1.6/src/llmflex/KnowledgeBase/knowledge_base.py
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-05-21 17:59:46.283611 llmflex-0.1.6/src/llmflex/Memory/
+-rw-r--r--   0 nathan95   (501) staff       (20)      287 2024-02-24 22:31:02.000000 llmflex-0.1.6/src/llmflex/Memory/__init__.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     8298 2024-03-11 17:44:28.000000 llmflex-0.1.6/src/llmflex/Memory/assistant_long_term_memory.py
+-rw-r--r--   0 nathan95   (501) staff       (20)    13190 2024-05-21 17:59:14.000000 llmflex-0.1.6/src/llmflex/Memory/base_memory.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     7727 2024-03-11 17:44:28.000000 llmflex-0.1.6/src/llmflex/Memory/long_short_memory.py
+-rw-r--r--   0 nathan95   (501) staff       (20)    13523 2024-05-21 17:59:14.000000 llmflex-0.1.6/src/llmflex/Memory/longshort_memory.py
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-05-21 17:59:46.283819 llmflex-0.1.6/src/llmflex/Models/
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-05-21 17:59:46.284764 llmflex-0.1.6/src/llmflex/Models/Cores/
+-rw-r--r--   0 nathan95   (501) staff       (20)        0 2024-02-24 22:31:02.000000 llmflex-0.1.6/src/llmflex/Models/Cores/__init__.py
+-rw-r--r--   0 nathan95   (501) staff       (20)    15426 2024-05-21 17:59:14.000000 llmflex-0.1.6/src/llmflex/Models/Cores/base_core.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     7915 2024-02-25 22:17:53.000000 llmflex-0.1.6/src/llmflex/Models/Cores/exllamav2_core.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     9365 2024-05-21 17:59:14.000000 llmflex-0.1.6/src/llmflex/Models/Cores/huggingface_core.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     8223 2024-05-21 17:59:14.000000 llmflex-0.1.6/src/llmflex/Models/Cores/llamacpp_core.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     9273 2024-05-21 17:59:14.000000 llmflex-0.1.6/src/llmflex/Models/Cores/openai_core.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     7481 2024-05-21 17:59:14.000000 llmflex-0.1.6/src/llmflex/Models/Cores/utils.py
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-05-21 17:59:46.284987 llmflex-0.1.6/src/llmflex/Models/Factory/
+-rw-r--r--   0 nathan95   (501) staff       (20)        0 2024-02-24 22:31:02.000000 llmflex-0.1.6/src/llmflex/Models/Factory/__init__.py
+-rw-r--r--   0 nathan95   (501) staff       (20)    10723 2024-04-14 12:29:06.000000 llmflex-0.1.6/src/llmflex/Models/Factory/llm_factory.py
+-rw-r--r--   0 nathan95   (501) staff       (20)       43 2024-02-24 22:31:02.000000 llmflex-0.1.6/src/llmflex/Models/__init__.py
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-05-21 17:59:46.285267 llmflex-0.1.6/src/llmflex/Prompts/
+-rw-r--r--   0 nathan95   (501) staff       (20)       52 2024-02-24 22:31:02.000000 llmflex-0.1.6/src/llmflex/Prompts/__init__.py
+-rw-r--r--   0 nathan95   (501) staff       (20)    21647 2024-05-21 17:59:14.000000 llmflex-0.1.6/src/llmflex/Prompts/prompt_template.py
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-05-21 17:59:46.285684 llmflex-0.1.6/src/llmflex/Rankers/
+-rw-r--r--   0 nathan95   (501) staff       (20)       81 2024-04-21 17:42:51.000000 llmflex-0.1.6/src/llmflex/Rankers/__init__.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     1471 2024-04-21 17:42:51.000000 llmflex-0.1.6/src/llmflex/Rankers/base_ranker.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     2309 2024-04-21 17:42:51.000000 llmflex-0.1.6/src/llmflex/Rankers/flashrank_ranker.py
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-05-21 17:59:46.286115 llmflex-0.1.6/src/llmflex/Schemas/
+-rw-r--r--   0 nathan95   (501) staff       (20)       64 2024-04-21 17:42:51.000000 llmflex-0.1.6/src/llmflex/Schemas/__init__.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     1414 2024-04-21 17:42:51.000000 llmflex-0.1.6/src/llmflex/Schemas/documents.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     2429 2024-04-21 17:42:51.000000 llmflex-0.1.6/src/llmflex/Schemas/tokenizer.py
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-05-21 17:59:46.286753 llmflex-0.1.6/src/llmflex/TextSplitters/
+-rw-r--r--   0 nathan95   (501) staff       (20)      123 2024-03-11 17:44:28.000000 llmflex-0.1.6/src/llmflex/TextSplitters/__init__.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     1526 2024-03-11 17:44:28.000000 llmflex-0.1.6/src/llmflex/TextSplitters/base_text_splitter.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     2860 2024-05-21 17:59:14.000000 llmflex-0.1.6/src/llmflex/TextSplitters/sentence_token_text_splitter.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     1423 2024-04-21 17:42:51.000000 llmflex-0.1.6/src/llmflex/TextSplitters/token_text_splitter.py
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-05-21 17:59:46.287865 llmflex-0.1.6/src/llmflex/Tools/
+-rw-r--r--   0 nathan95   (501) staff       (20)      115 2024-02-24 22:31:02.000000 llmflex-0.1.6/src/llmflex/Tools/__init__.py
+-rw-r--r--   0 nathan95   (501) staff       (20)    11795 2024-02-24 22:31:02.000000 llmflex-0.1.6/src/llmflex/Tools/base_tool.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     2983 2024-05-21 17:59:14.000000 llmflex-0.1.6/src/llmflex/Tools/browser_tool.py
+-rw-r--r--   0 nathan95   (501) staff       (20)       45 2024-05-21 17:59:14.000000 llmflex-0.1.6/src/llmflex/Tools/tool_prompting.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     6603 2024-03-11 17:44:28.000000 llmflex-0.1.6/src/llmflex/Tools/tool_selection.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     9639 2024-05-21 17:59:14.000000 llmflex-0.1.6/src/llmflex/Tools/tool_utils.py
+-rw-r--r--   0 nathan95   (501) staff       (20)    11421 2024-04-21 17:42:51.000000 llmflex-0.1.6/src/llmflex/Tools/web_search_tool.py
+-rw-r--r--   0 nathan95   (501) staff       (20)    15193 2024-05-21 17:59:14.000000 llmflex-0.1.6/src/llmflex/Tools/web_search_utils.py
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-05-21 17:59:46.288360 llmflex-0.1.6/src/llmflex/VectorDBs/
+-rw-r--r--   0 nathan95   (501) staff       (20)       93 2024-03-11 17:44:28.000000 llmflex-0.1.6/src/llmflex/VectorDBs/__init__.py
+-rw-r--r--   0 nathan95   (501) staff       (20)    24488 2024-05-21 17:59:14.000000 llmflex-0.1.6/src/llmflex/VectorDBs/base_vectordb.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     5362 2024-04-21 17:42:51.000000 llmflex-0.1.6/src/llmflex/VectorDBs/faiss_vectordb.py
+-rw-r--r--   0 nathan95   (501) staff       (20)      275 2024-05-21 17:59:14.000000 llmflex-0.1.6/src/llmflex/__init__.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     4381 2024-02-24 22:31:02.000000 llmflex-0.1.6/src/llmflex/cli.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     6178 2024-03-11 17:44:28.000000 llmflex-0.1.6/src/llmflex/utils.py
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-05-21 17:59:46.288542 llmflex-0.1.6/src/llmflex.egg-info/
+-rw-r--r--   0 nathan95   (501) staff       (20)    10171 2024-05-21 17:59:46.000000 llmflex-0.1.6/src/llmflex.egg-info/PKG-INFO
+-rw-r--r--   0 nathan95   (501) staff       (20)     2165 2024-05-21 17:59:46.000000 llmflex-0.1.6/src/llmflex.egg-info/SOURCES.txt
+-rw-r--r--   0 nathan95   (501) staff       (20)        1 2024-05-21 17:59:46.000000 llmflex-0.1.6/src/llmflex.egg-info/dependency_links.txt
+-rw-r--r--   0 nathan95   (501) staff       (20)       44 2024-05-21 17:59:46.000000 llmflex-0.1.6/src/llmflex.egg-info/entry_points.txt
+-rw-r--r--   0 nathan95   (501) staff       (20)      357 2024-05-21 17:59:46.000000 llmflex-0.1.6/src/llmflex.egg-info/requires.txt
+-rw-r--r--   0 nathan95   (501) staff       (20)        8 2024-05-21 17:59:46.000000 llmflex-0.1.6/src/llmflex.egg-info/top_level.txt
```

### Comparing `llmflex-0.1.5/LICENSE.md` & `llmflex-0.1.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.5/PKG-INFO` & `llmflex-0.1.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmflex
-Version: 0.1.5
+Version: 0.1.6
 Summary: A python package for developing AI applications with local LLMs.
 Author-email: Nathan Tam <nathan1295@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/nath1295/LLMFlex
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
@@ -24,25 +24,31 @@
 Requires-Dist: tiktoken
 Requires-Dist: protobuf
 Requires-Dist: beautifulsoup4
 Requires-Dist: streamlit
 Requires-Dist: watchdog
 Requires-Dist: spacy>=3.7.0
 Requires-Dist: flask
+Requires-Dist: PyMuPDF
+Requires-Dist: python-docx
 Provides-Extra: cu121
 Requires-Dist: auto-gptq>=0.6.0; extra == "cu121"
 Requires-Dist: autoawq; extra == "cu121"
 Requires-Dist: exllamav2; extra == "cu121"
 Provides-Extra: cu118
 Requires-Dist: auto-gptq; extra == "cu118"
 Requires-Dist: autoawq; extra == "cu118"
 Requires-Dist: exllamav2; extra == "cu118"
 
 # LLMFlex
+[![PyPI](https://img.shields.io/pypi/v/llmflex)](https://pypi.org/project/llmflex/)
+[![PyPI - License](https://img.shields.io/pypi/l/llmflex)](https://pypi.org/project/llmflex/)
+[![GitHub Repo stars](https://img.shields.io/github/stars/nath1295/llmflex)](https://pypi.org/project/llmflex/)
 
+## A python package for developing AI applications with local LLMs
 LLMFlex is a python package that allows python developers to work with different large language models (LLM) and do prompt engineering with a simple interface. It favours free and local resources instead of using paid APIs to develop truly local and private AI-powered solutions.
 
 It provides classes to load LLM models, embedding models, and vector databases to create LLM powered applications with your own prompt engineering and RAG techniques. With a one-liner command, you can load a chatbot interface to chat with the LLM or serve a model as OpenAI API as well.
 
 ## Installing LLMFlex
 Creating a virtual environment before installing the package is highly recommended. Also make sure you have installed [Pytorch](https://pytorch.org/get-started/locally/) and [llama-cpp-python](https://pypi.org/project/llama-cpp-python/) with the correct installation method according to your hardware configuration before installing LLMFlex. Please visit the links provided for the respective packages for more detailed installation guides.
```

### Comparing `llmflex-0.1.5/README.md` & `llmflex-0.1.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # LLMFlex
+[![PyPI](https://img.shields.io/pypi/v/llmflex)](https://pypi.org/project/llmflex/)
+[![PyPI - License](https://img.shields.io/pypi/l/llmflex)](https://pypi.org/project/llmflex/)
+[![GitHub Repo stars](https://img.shields.io/github/stars/nath1295/llmflex)](https://pypi.org/project/llmflex/)
 
+## A python package for developing AI applications with local LLMs
 LLMFlex is a python package that allows python developers to work with different large language models (LLM) and do prompt engineering with a simple interface. It favours free and local resources instead of using paid APIs to develop truly local and private AI-powered solutions.
 
 It provides classes to load LLM models, embedding models, and vector databases to create LLM powered applications with your own prompt engineering and RAG techniques. With a one-liner command, you can load a chatbot interface to chat with the LLM or serve a model as OpenAI API as well.
 
 ## Installing LLMFlex
 Creating a virtual environment before installing the package is highly recommended. Also make sure you have installed [Pytorch](https://pytorch.org/get-started/locally/) and [llama-cpp-python](https://pypi.org/project/llama-cpp-python/) with the correct installation method according to your hardware configuration before installing LLMFlex. Please visit the links provided for the respective packages for more detailed installation guides.
```

### Comparing `llmflex-0.1.5/pyproject.toml` & `llmflex-0.1.6/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -25,15 +25,17 @@
     "openai>=1.0.0",
     "tiktoken",
     "protobuf",
     "beautifulsoup4",
     "streamlit",
     "watchdog",
     "spacy>=3.7.0",
-    "flask"
+    "flask",
+    "PyMuPDF",
+    "python-docx"
 ]
 
 [project.urls]
 Homepage = "https://github.com/nath1295/LLMFlex"
 
 [project.scripts]
 llmflex = "llmflex.cli:cli"
```

### Comparing `llmflex-0.1.5/src/llmflex/Data/vector_database.py` & `llmflex-0.1.6/src/llmflex/VectorDBs/base_vectordb.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
-import os
 from ..Embeddings.base_embeddings import BaseEmbeddingsToolkit
-from langchain.schema.document import Document
-from langchain.text_splitter import TextSplitter
-import pandas as pd
-from typing import List, Optional, Type, Dict, Any, Union
+from ..TextSplitters.base_text_splitter import BaseTextSplitter
+from ..Schemas.documents import Document
+from abc import abstractmethod, ABC
+from typing import List, Dict, Union, Any, Type, Optional, Sequence, Callable, Tuple
+import os, numpy as np
 
 def default_vectordb_dir() -> str:
     """Default home directory of vector databases.
 
     Returns:
         str: Default home directory of vector databases.
     """
@@ -23,384 +23,499 @@
 
     Args:
         vectordb_dir (Optional[str], optional): Directory where the vector databases live. If None is given, the default_vectordb_dir will be used. Defaults to None.
 
     Returns:
         List[str]: List all the vector databases in the given directory.
     """
-    vectordb_dir = vectordb_dir if ((isinstance(vectordb_dir, str)) & (os.path.exists(vectordb_dir))) else default_vectordb_dir()
+    vectordb_dir = default_vectordb_dir() if vectordb_dir is None else vectordb_dir
+    vectordb_dir = vectordb_dir if os.path.exists(vectordb_dir) else default_vectordb_dir()
     dbs = list(filter(lambda x: os.path.isdir(os.path.join(vectordb_dir, x)), os.listdir(vectordb_dir)))
     dbs = list(filter(lambda x: os.path.exists(os.path.join(vectordb_dir, x, 'info.json')), dbs))
     return dbs
 
 def name_checker(name: str) -> str:
     """Raise error if the given string has space, newline characters, or tab characters.
 
     Args:
         name (str): String to check.
 
     Returns:
         str: Return the given text if it passes all the checkes.
     """
     if ' ' in name:
-        raise ValueError(f'Spaces cannot be in the name')
+        raise ValueError(f'Spaces cannot be in the name.')
     if '\n' in name:
         raise ValueError(f'Newline characters cannot be in the name.')
     if '\r' in name:
         raise ValueError(f'Newline characters cannot be in the name.')
     if '\t' in name:
         raise ValueError(f'Tab characters cannot be in the name.')
     return name
-        
-def texts_to_documents(texts: List[str], 
-        embeddings: Optional[Type[BaseEmbeddingsToolkit]] = None,
-        text_splitter: Optional[Type[TextSplitter]] = None,
-        data: Optional[Union[pd.DataFrame, List[Dict[str, Any]], Dict[str, Any]]] = None,
-        split_text: bool = True) -> List[Document]:
-    """Create splitted documents from the list of text strings.
-
-    Args:
-        texts (List[str]): List of strings to split into documents.
-        embeddings (Optional[Type[BaseEmbeddingsToolkit]], optional): Embedding toolkit used to split the documents. Defaults to None
-        text_splitter (Optional[Type[TextSplitter]], optional): Text splitter used to split the documents. If provided, it will be used instead of the embedding toolkit. Defaults to None.
-        data (Optional[Union[pd.DataFrame, List[Dict[str, Any]], Dict[str, Any]]], optional): Metadata for each text strings. Defaults to None.
-        split_text (bool, optional): Whether to split text if the given text is too long. Defaults to True.
-
-    Returns:
-        List[Document]: List of splitted documents.
-    """
-    if type(data) == pd.DataFrame:
-        data = data.to_dict('records')
-    elif type(data) == dict:
-        data = [data] * len(texts)
-    elif data is None:
-        data = [dict()] * len(texts)
-    
-    docs = list(map(lambda x: Document(page_content=x[0], metadata=x[1]), list(zip(texts, data))))
-    if split_text:
-        if text_splitter is not None:
-            docs = text_splitter.split_documents(docs)
-        elif embeddings is not None:
-            docs = embeddings.text_splitter.split_documents(docs)
-        else:
-            raise RuntimeError('Either embeddings or text_splitter has to be provided if split_text=True.')
-    return docs
 
-class VectorDatabase:
-    """Vector database class, suitable for storing text data as embeddings for similarity searches and other classes that requires numerical respresentations of texts.
+class BaseVectorDatabase(ABC):
+    """Base class for vector databases.
     """
-
-    def __init__(self, embeddings: Type[BaseEmbeddingsToolkit], 
-                 vectordb_dir: Optional[str] = None, name: Optional[str] = None,
-                 save_raw: bool = False) -> None:
-        """Initialising basic information of the vector database.
+    def __init__(self, embeddings: Type[BaseEmbeddingsToolkit], name: Optional[str] = None, vectordb_dir: Optional[str] = None, 
+                 text_splitter: Optional[Type[BaseTextSplitter]] = None, **kwargs) -> None:
+        """Initialise a vector database.
 
         Args:
-            embeddings (Type[BaseEmbeddingsToolkit]): Embeddings toolkits used in the vector database.
-            vectordb_dir (Optional[str], optional): Parent directory of the vector database if it is not In-memory only. If None is given, the default_vectordb_dir will be used. Defaults to None.
-            name (Optional[str], optional): Name of the vector database. If given, the vector database will be stored in storage. Defaults to None.
-            save_raw (bool, optional): Whether to save raw text data and metadata as a separate json file. Defaults to False.
+            embeddings (Type[BaseEmbeddingsToolkit]): Embeddings toolkit to use.
+            name (Optional[str], optional): Name of the vector database. Will be used as the directory base name of the vector database in vectordb_dir. If None is given, the vector database will not be saved. Defaults to None.
+            vectordb_dir (Optional[str], optional): Directory where the vector databases live. If None is given, the default_vectordb_dir will be used. Defaults to None.
+            text_splitter (Optional[Type[BaseTextSplitter]], optional): Default text splitter for the vecetor database. If None is given, the embeddings toolkit text splitter will be used. Defaults to None.
         """
-        print("VectorDatabase class will be deprecated. Please use llmflex.VectorDBs.FaissVectorDatabase instead in the future.")
-        self._name = '_InMemoryVectorDB_' if name is None else name_checker(name)
         self._embeddings = embeddings
-        self._vectordb_dir = default_vectordb_dir() if vectordb_dir is None else os.path.abspath(vectordb_dir)
-        self._save_raw = save_raw
+        self._name = name_checker(name) if name is not None else None
+        vectordb_dir = default_vectordb_dir() if vectordb_dir is None else vectordb_dir
+        self._db_dir = os.path.join(vectordb_dir, self.name) if self.name is not None else None
+        if self.db_dir is not None:
+            os.makedirs(self.db_dir, exist_ok=True)
+        self._index = self._get_empty_index()
+        self._data = dict()
+        self._text_splitter = self.embeddings.text_splitter if text_splitter is None else text_splitter
 
     @property
-    def name(self) -> str:
-        """Name of the vector database.
+    def embeddings(self) -> BaseEmbeddingsToolkit:
+        """Embeddings toolkit used in the vector database.
 
         Returns:
-            str: Name of the vector database.
+            BaseEmbeddingsToolkit: Embeddings toolkit used in the vector database.
         """
-        return self._name
+        return self._embeddings
     
     @property
-    def embeddings(self) -> Type[BaseEmbeddingsToolkit]:
-        """Embeddings toolkit used in the vector database.
+    def text_splitter(self) -> BaseTextSplitter:
+        """Default text splitter for the vector database.
 
         Returns:
-            Type[BaseEmbeddingsToolkit]: Embeddings toolkit used in the vector database.
+            BaseTextSplitter: Default text splitter for the vector database.
         """
-        return self._embeddings
+        return self._text_splitter
     
     @property
-    def vdb_dir(self) -> Union[str, None]:
-        """Directory of the vector database if it is not in-memory only.
+    def index(self) -> Any:
+        """Index of the vector database.
 
         Returns:
-            Union[str, None]: Directory of the vector database if it is not in-memory only.
+            Any: Index of the vector database.
         """
-        if self.name != '_InMemoryVectorDB_':
-            vdb_dir = os.path.join(self._vectordb_dir, self.name)
-            os.makedirs(vdb_dir, exist_ok=True)
-            return vdb_dir
-        else:
-            return None
-
+        return self._index
+    
     @property
-    def save_raw(self) -> bool:
-        """Whether to save the raw data as json or not.
+    def name(self) -> Optional[str]:
+        """Name of the vector database.
 
         Returns:
-            bool: Whether to save the raw data as json or not.
+            Optional[str]: Name of the vector database.
         """
-        return self._save_raw
+        return self._name
     
     @property
     def info(self) -> Dict[str, Any]:
         """Information of the vector database.
 
         Returns:
             Dict[str, Any]: Information of the vector database.
         """
-        if hasattr(self, '_info'):
-            return self._info
-        elif ((self.vdb_dir is not None) & ('info.json' in os.listdir(self.vdb_dir))):
-            from ..utils import read_json
-            self._info = read_json(os.path.join(self.vdb_dir, 'info.json'))
-            return self._info
-        else:
-            from ..utils import save_json, current_time
-            self._info = dict(embeddings=self.embeddings.name, last_update=current_time())
-            if self.save_raw:
-                save_json(self._info, os.path.join(self.vdb_dir, 'info.json'))
-            return self._info
-        
+        if not hasattr(self, '_info'):
+            from ..utils import current_time, read_json
+            if self.db_dir is not None:
+                info_dir = os.path.join(self.db_dir, 'info.json')
+                if os.path.exists(info_dir):
+                    self._info = read_json(info_dir)
+                else:
+                    self._info = dict(embeddings=self.embeddings.name, last_update=current_time())
+            else:
+                self._info = dict(embeddings=self.embeddings.name, last_update=current_time())
+        return self._info
+    
     @property
-    def vectorstore(self) -> "FAISS":
-        """Return the faiss vectorstore
+    def db_dir(self) -> Optional[str]:
+        """Directory of the vector database.
 
         Returns:
-            FAISS: The vector store.
+            Optional[str]: Directory of the vector database.
         """
-        return self._vectorstore
+        return self._db_dir
     
     @property
-    def data(self) -> List[Dict[str, Any]]:
-        """Raw data of the vector database.
+    def data(self) -> Dict[int, Document]:
+        """Dictionary of all the documents in the vector database.
 
         Returns:
-            List[Dict[str, Any]]: Raw data of the vector database.
+            Dict[int, Document]: Dictionary of all the documents in the vector database.
         """
-        data = list(self._vectorstore.docstore._dict.values())
-        data = list(map(lambda x: dict(index=x.page_content, metadata=x.metadata), data))
-        return data
+        return self._data
     
     @property
     def size(self) -> int:
-        """Number of embeddings in the vector database. May be more than the number of texts you have added into the database due to text splitting for longer texts.
+        """Number of documents in the vector database.
 
         Returns:
-            int: Number of embeddings.
+            int: Number of documents in the vector database.
         """
         return len(self.data)
-        
-    def _init_vectordb(self, embeddings: Type[BaseEmbeddingsToolkit], from_exist: bool = True) -> None:
-        """Initialise the langchain vectorstore
+    
+    @abstractmethod
+    def _get_empty_index(self) -> Any:
+        """Return an empty index.
+
+        Returns:
+            Any: An empty index.
+        """
+        pass
+
+    @property
+    @abstractmethod
+    def _index_filename(self) -> str:
+        """Base name of the file for the index in the vector database directory.
+
+        Returns:
+            str: Base name of the file for the index in the vector database directory.
+        """
+        pass
+    
+    @abstractmethod
+    def _save_index(self) -> None:
+        """Save the index of the vector database.
+        """
+        pass
+
+    @abstractmethod
+    def _load_index(self, index_dir: str) -> Any:
+        """Load the index from an existing saved file.
+        """
+        pass
+
+    @abstractmethod
+    def _add(self, vectors: np.ndarray[np.float32], docs: List[Document]) -> None:
+        """Core method to add documents into the vector database.
 
         Args:
-            from_exist (bool, optional): Whether to initialise from an existing vectorstore. Defaults to True.
+            vectors (np.ndarray[np.float32]): Array of vectors created by the indexes of the documents.
+            docs (List[Document]): List of documents to add.
         """
-        from langchain.vectorstores.faiss import FAISS
-        import faiss
-        import warnings
-        warnings.filterwarnings('ignore')
-        if ((from_exist) & (self.name in list_vectordbs(self._vectordb_dir))):
-            if (self.info.get('embeddings', 'NOT_AVAIALBLE') == embeddings.name):
-                self._vectorstore = FAISS.load_local(folder_path=self.vdb_dir, embeddings=embeddings.embedding_model)
-            elif 'data.json' in os.listdir(self.vdb_dir):
-                from ..utils import read_json
-                data = read_json(os.path.join(self.vdb_dir, 'data.json'))
-                docs = texts_to_documents(texts=list(map(lambda x: x['index'], data)), 
-                                          embeddings=embeddings, data=list(map(lambda x: x['metadata'], data)), split_text=False)
-                self._vectorstore = FAISS.from_documents(docs, embedding=embeddings.embedding_model)
-                self.info
-                self._info['embeddings'] = embeddings.name
-                self.save()
-        else:
-            from langchain.docstore import InMemoryDocstore
-            if ((self.name in list_vectordbs(self._vectordb_dir)) & (self.vdb_dir is not None)):
-                import shutil
-                shutil.rmtree(self.vdb_dir)
-            self._vectorstore = FAISS(embedding_function=embeddings.embedding_model, index=faiss.IndexFlatL2(embeddings.embedding_size),
-                                          docstore=InMemoryDocstore({}), index_to_docstore_id={})
-            self.save()
-                
-    def save(self) -> None:
-        """Save the latest vector database.
+        pass
+
+    @abstractmethod
+    def _delete(self, ids: List[int]) -> None:
+        """Core method to remove records by ids.
+
+        Args:
+            ids (List[int]): Ids to remove.
         """
-        if self.vdb_dir is not None:
-            from ..utils import save_json, current_time
-            self._vectorstore.save_local(self.vdb_dir)
-            self.info
-            self._info['last_update'] = current_time()
-            save_json(self.info, os.path.join(self.vdb_dir, 'info.json'))
-            if self.save_raw:
-                save_json(self.data, os.path.join(self.vdb_dir, 'data.json'))
-        
+        pass
+
+    @abstractmethod
+    def _batch_search_with_scores(self, vectors: np.ndarray[np.float32], k: int = 5, ids_scope: Optional[List[int]] = None) -> Tuple[np.ndarray[np.float32], np.ndarray[np.int64]]:
+        """Batch similarity search with multiple vectors.
+
+        Args:
+            vectors (np.ndarray[np.float32]): Array of vectors for the search.
+            k (int, optional): Maximum results for each vector. Defaults to 5.
+            ids_scope (Optional[List[int]], optional): The list of allowed ids to return for the similarity search. Defaults to None.
+
+        Returns:
+            Tuple[np.ndarray[np.float32], np.ndarray[np.int64]]: Tuple of scores and ids. Both matrices must be in the same shape.
+        """
+        pass
+
+    @abstractmethod
+    def _get_vectors_by_ids(self, ids: List[int]) -> np.ndarray[np.float32]:
+        """Get the array of vectors by ids.
+
+        Args:
+            ids (List[int]): Document ids.
+
+        Returns:
+            np.ndarray[np.float32]: Arrray of vectors.
+        """
+        pass
+
     @classmethod
-    def from_exist(cls, name: str, embeddings: Type[BaseEmbeddingsToolkit], vectordb_dir: Optional[str] = None) -> VectorDatabase:
-        """Initialise the vector database from existing files.
+    def from_exist(cls, embeddings: Type[BaseEmbeddingsToolkit], name: str, vectordb_dir: Optional[str] = None,
+                   text_splitter: Optional[Type[BaseTextSplitter]] = None, **kwargs) -> BaseVectorDatabase:
+        """Load the vector database from an existing vector database.
 
         Args:
-            name (str): Name of the existing vector database.
-            embeddings (Type[BaseEmbeddingsToolkit]): Embeddings toolkit used in this vector database.
-            vectordb_dir (Optional[str], optional): Parent directory of the vector database. If None is given, the default_vectordb_dir will be used. Defaults to None.
+            embeddings (Type[BaseEmbeddingsToolkit]): Embeddings toolkit to use.
+            name (str): Name of the existing database.
+            vectordbs_dir (Optional[str], optional): Directory where the vector databases live. If None is given, the default_vectordb_dir will be used. Defaults to None.
+            text_splitter (Optional[Type[BaseTextSplitter]], optional): Text splitter to split the documents. If none given, the embeddings toolkit text splitter will be used. Defaults to None.
+
 
         Returns:
-            VectorDatabase: The intialised vector database.
+            BaseVectorDatabase: The initialised vector database.
         """
-        if name not in list_vectordbs(vectordb_dir=vectordb_dir):
-            raise FileNotFoundError(f'Vector database "{name}" does not exist.')
-        vdb = cls(embeddings=embeddings, name=name, vectordb_dir=vectordb_dir)
-        if vdb.info.get('embeddings', 'NOT_AVAIALBLE') != embeddings.name:
-            if 'data.json' not in os.listdir(vdb.vdb_dir):
-                raise FileNotFoundError(f'The vector database did not use the embeddings "{embeddings.name}" and no raw data was saved. Vector database cannot be loaded with this embeddings.')
+        vectordbs_dir = default_vectordb_dir() if vectordb_dir is None else vectordb_dir
+        name = name_checker(name)
+        existing_dbs = list_vectordbs(vectordb_dir=vectordbs_dir)
+        if name not in existing_dbs:
+            raise ValueError(f'The vector database "{name}" does not exist.')
+        
+        from ..utils import read_json
+        import pickle
+        db_info_dir = os.path.join(vectordbs_dir, name, 'info.json')
+        db_info = read_json(db_info_dir)
+        db_embeddings_name = db_info.get('embeddings', None)
+        vdb = cls(embeddings, name, vectordbs_dir, text_splitter)
+        data_dir =os.path.join(vdb.db_dir, 'data.pkl')
+        if os.path.exists(data_dir):
+            with open(data_dir, 'rb') as f:
+                vdb._data = pickle.load(f)
+        else: # recovering from old format
+            print('Trying to recover from old format...')
+            old_data_dir = os.path.join(vdb.db_dir, 'index.pkl')
+            if os.path.exists(old_data_dir):
+                with open(old_data_dir, 'rb') as f:
+                    data = pickle.load(f)
+                data = list(map(lambda x: Document(index=x.page_content, metadata=x.metadata), data[0]._dict.values()))
+                vdb.add_documents(data, split_text=False)
             else:
-                vdb._save_raw = True
-                vdb._init_vectordb(embeddings=embeddings, from_exist=True)
+                raise FileExistsError(f'No raw data has been saved. Vector database cannot be recovered.')
+        if db_embeddings_name == embeddings.name:
+            vdb._index = vdb._load_index(os.path.join(vdb.db_dir, vdb._index_filename))
         else:
-            vdb._save_raw = 'data.json' in os.listdir(vdb.vdb_dir)
-            vdb._init_vectordb(embeddings=embeddings, from_exist=True)
+            print(f'You are using a different embeddings model. Switching from embedding model {db_embeddings_name} to {embeddings.name}.')
+            vdb.add_documents(list(vdb.data.values()), split_text=False)
+            vdb.info['embeddings'] = embeddings.name
+        vdb.save()
         return vdb
-    
+
     @classmethod
-    def from_empty(cls, embeddings: Type[BaseEmbeddingsToolkit], name: Optional[str] = None, vectordb_dir: Optional[str] = None, save_raw: bool = False) -> VectorDatabase:
-        """Initialise an empty vector database.
+    def from_documents(cls, embeddings: Type[BaseEmbeddingsToolkit], docs: List[Document], 
+                      name: Optional[str] = None, vectordb_dir: Optional[str] = None,
+                      split_text: bool = True, text_splitter: Optional[Type[BaseTextSplitter]] = None, **kwargs) -> BaseVectorDatabase:
+        """Load the vector database from existing documents.
 
         Args:
-            embeddings (Type[BaseEmbeddingsToolkit]): Embeddings toolkits used in the vector database.
-            name (Optional[str], optional): Name of the vector database. If given, the vector database will be stored in storage. Defaults to None.
-            vectordb_dir (Optional[str], optional): Parent directory of the vector database if it is not In-memory only. If None is given, the default_vectordb_dir will be used. Defaults to None.
-            save_raw (bool, optional): Whether to save raw text data and metadata as a separate json file. Defaults to False.
+            embeddings (Type[BaseEmbeddingsToolkit]): Embeddings toolkit to use.
+            docs (List[Document]): List of documents to use.
+            name (Optional[str], optional): Name of the vector database. Will be used as the directory base name of the vector database in vectordb_dir. If None is given, the vector database will not be saved. Defaults to None.
+            vectordb_dir (Optional[str], optional): Directory where the vector databases live. If None is given, the default_vectordb_dir will be used. Defaults to None.
+            split_text (bool, optional): Whether to split the docuements with the embeddings toolkit text splitter. Defaults to True.
+            text_splitter (Optional[Type[BaseTextSplitter]], optional): Text splitter to split the documents. If none given, the embeddings toolkit text splitter will be used. Defaults to None.
 
         Returns:
-            VectorDatabase: The intialised vector database.
-        """
-        vdb = cls(embeddings=embeddings, name=name, vectordb_dir=vectordb_dir, save_raw=save_raw)
-        vdb._init_vectordb(embeddings=embeddings, from_exist=False)
+            BaseVectorDatabase: The initialised vector database.
+        """
+        vdb = cls(embeddings, name, vectordb_dir, text_splitter)
+        vdb.add_documents(docs=docs, split_text=split_text, text_splitter=text_splitter)
+        vdb.save() # In case an empty list of docs is given.
         return vdb
     
     @classmethod
-    def from_data(cls, index: List[str], embeddings: Type[BaseEmbeddingsToolkit],
-                  data: Union[pd.DataFrame, Dict[str, Any], List[Dict[str, Any]]] = dict(), text_splitter: Type[TextSplitter] = None, name: Optional[str] = None, 
-                  vectordb_dir: Optional[str] = None, save_raw: bool = False, split_text: bool = True) -> VectorDatabase:
-        """Initialise the vector database with list of texts.
-
-        Args:
-            index (List[str]): List of texts to initialise the database.
-            embeddings (Type[BaseEmbeddingsToolkit]): Embeddings toolkits used in the vector database.
-            data (Union[pd.DataFrame, Dict[str, Any], List[Dict[str, Any]]], optional): Metadata for the list of texts. Defaults to dict().
-            text_splitter (Optional[Type[TextSplitter]], optional): Text splitter used to split the documents. If provided, it will be used instead of the embedding toolkit. Defaults to None.
-            name (Optional[str], optional): Name of the vector database. If given, the vector database will be stored in storage. Defaults to None.
-            vectordb_dir (Optional[str], optional): Parent directory of the vector database if it is not In-memory only. If None is given, the default_vectordb_dir will be used. Defaults to None.
-            save_raw (bool, optional): Whether to save raw text data and metadata as a separate json file. Defaults to False.
-            split_text (bool, optional): Whether to split the texts if they are too long. Defaults to True.
+    def from_texts(cls, embeddings: Type[BaseEmbeddingsToolkit], texts: List[str], metadata: Optional[Union[Dict[str, Any], List[Dict[str, Any]]]] = None,
+                      name: Optional[str] = None, vectordb_dir: Optional[str] = None,
+                      split_text: bool = True, text_splitter: Optional[Type[BaseTextSplitter]] = None, **kwargs) -> BaseVectorDatabase:
+        """Load the vector database from existing texts.
+
+        Args:
+            embeddings (Type[BaseEmbeddingsToolkit]): Embeddings toolkit to use.
+            texts (List[str]): List of texts to add.
+            metadata (Optional[Union[Dict[str, Any], List[Dict[str, Any]]]], optional): Metadata to add along with the texts. Defaults to None.
+            name (Optional[str], optional): Name of the vector database. Will be used as the directory base name of the vector database in vectordb_dir. If None is given, the vector database will not be saved. Defaults to None.
+            vectordb_dir (Optional[str], optional): Directory where the vector databases live. If None is given, the default_vectordb_dir will be used. Defaults to None.
+            split_text (bool, optional): Whether to split the docuements with the embeddings toolkit text splitter. Defaults to True.
+            text_splitter (Optional[Type[BaseTextSplitter]], optional): Text splitter to split the documents. If none given, the embeddings toolkit text splitter will be used. Defaults to None.
 
         Returns:
-            VectorDatabase: The intialised vector database.
-        """
-        vdb = cls.from_empty(embeddings=embeddings, name=name, vectordb_dir=vectordb_dir, save_raw=save_raw)
-        vdb.add_texts(texts=index, metadata=data, text_splitter=text_splitter, split_text=split_text)
+            BaseVectorDatabase: The initialised vector database.
+        """
+        vdb = cls(embeddings, name, vectordb_dir, text_splitter)
+        vdb.add_texts(texts=texts, metadata=metadata, split_text=split_text, text_splitter=text_splitter)
+        vdb.save() # In case an empty list of texts is given.
         return vdb
-    
-    def add_texts(self, texts: List[str], metadata: Union[pd.DataFrame, Dict[str, Any], List[Dict[str, Any]]] = dict(), 
-                  text_splitter: Optional[Type[TextSplitter]] = None, split_text: bool = True) -> None:
-        """Adding texts to the vector database.
 
-        Args:
-            texts (List[str]): List of texts to add.
-            metadata (Union[pd.DataFrame, Dict[str, Any], List[Dict[str, Any]]], optional): Metadata for the texts. Defaults to dict().
-            text_splitter (Optional[Type[TextSplitter]], optional): Text splitter used to split the documents. If provided, it will be used instead of the embedding toolkit. Defaults to None.
-            split_text (bool, optional): Whether to split the texts if they are too long. Defaults to True.
+    def _save_data(self) -> None:
+        """Save the documents in the vector database.
         """
-        docs = texts_to_documents(texts=texts, embeddings=self.embeddings, text_splitter=text_splitter, data=metadata, split_text=split_text)
-        self.vectorstore.add_documents(docs)
-        self.save()
+        if self.db_dir is not None:
+            import pickle
+            with open(os.path.join(self.db_dir, 'data.pkl'), 'wb') as f:
+                pickle.dump(self.data, f)
+
+    def _save_info(self) -> None:
+        """Save information about the vector database.
+        """
+        from ..utils import save_json, current_time
+        self.info['last_update'] = current_time()
+        if self.db_dir is not None:
+            save_json(self.info, os.path.join(self.db_dir, 'info.json'))
 
-    def add_documents(self, docs: List[Document], text_splitter: Optional[Type[TextSplitter]] = None, split_text: bool = True) -> None:
-        """Adding documents to the vector database.
-
-        Args:
-            docs (List[Document]): List of documents to add.
-            text_splitter (Optional[Type[TextSplitter]], optional): Text splitter used to split the documents. If provided, it will be used instead of the embedding toolkit. Defaults to None.
-            split_text (bool, optional): Whether to split the texts if they are too long. Defaults to True.
+    def save(self) -> None:
+        """Save the vector database.
         """
-        texts = list(map(lambda x: x.page_content, docs))
-        metadata = list(map(lambda x: x.metadata, docs))
-        self.add_texts(texts=texts, metadata=metadata, text_splitter=text_splitter, split_text=split_text)
+        if self.db_dir is not None:
+            self._save_data()
+            self._save_index()
+            self._save_info()
 
-    def _result_dict(self, index: str, score: float, metadata: Dict[str, Any]) -> Dict[str, Any]:
-        """Helper method to construct search results into a dictionary.
+    def add_documents(self, docs: List[Document], split_text: bool = True, text_splitter: Optional[Type[BaseTextSplitter]] = None) -> None:
+        """Add documents into the vector database.
 
         Args:
-            index (str): Index as a text string.
-            score (float): Relevance score.
-            metadata (Dict[str, Any]): Metadata dictionary.
+            docs (List[Document]): List of documents to split.
+            split_text (bool, optional): Whether to split the docuements with the embeddings toolkit text splitter. Defaults to True.
+            text_splitter (Optional[Type[BaseTextSplitter]], optional): Text splitter to split the documents. If none given, the embeddings toolkit text splitter will be used. Defaults to None.
+        """
+        if len(docs) != 0:
+            text_splitter = self.text_splitter if text_splitter is None else text_splitter
+            docs = text_splitter.split_documents(docs) if split_text else docs
+            vectors = list(map(lambda x: x.index, docs))
+            vectors = self.embeddings.batch_embed(vectors)
+            vectors = np.array(vectors, dtype=np.float32)
+            self._add(vectors=vectors, docs=docs)
+            self.save()
 
-        Returns:
-            Dict[str, Any]:Dictionary with all information of the search result.
+    def add_docs_with_vectors(self, vectors: Sequence[Sequence[float]], docs: List[Document]) -> None:
+        """Add documents with pre-embedded vectors into the vector database.
+
+        Args:
+            vectors (Sequence[Sequence[float]]): Pre-embedded vectors.
+            docs (List[Document]): List of documents.
         """
-        return dict(index=index, score=score, metadata=metadata)
+        len_vec = len(vectors)
+        len_doc = len(docs)
+        if len_vec != 0:
+            if len_vec != len_doc:
+                raise ValueError(f'{len_vec} vectors are given but the number of documents given is {len_doc}. Make sure the number of documents match with the number of vectors given.')
+            vectors = np.array(vectors, dtype=np.float32)
+            self._add(vectors, docs)
+            self.save()
 
-    def _dictionary_filter(self, item: List[Union[str, Document]], **kwargs: Dict[str, Any]) -> bool:
-        """Helper method for dictionary filtering.
+    def add_texts(self, texts: List[str], metadata: Optional[Union[Dict[str, Any], List[Dict[str, Any]]]] = None, 
+                  split_text: bool = True, text_splitter: Optional[Type[BaseTextSplitter]] = None) -> None:
+        """Add texts into the vector database.
 
         Args:
-            item (List[Union[str, Document]]): Document item to check.
-
-        Returns:
-            bool: Return True if all metadata of the item satisfy the kwargs values.
-        """
-        for k, v in kwargs.items():
-            if item[1].metadata.get(k, None) != v:
-                return False
-        return True
+            texts (List[str]): List of texts to add.
+            metadata (Optional[Union[Dict[str, Any], List[Dict[str, Any]]]], optional): Metadata to add along with the texts. Defaults to None.
+            split_text (bool, optional): Whether to split the docuements with the embeddings toolkit text splitter. Defaults to True.
+            text_splitter (Optional[Type[BaseTextSplitter]], optional): Text splitter to split the documents. If none given, the embeddings toolkit text splitter will be used. Defaults to None.
+        """
+        if len(texts) != 0:
+            if metadata is None:
+                metadata = [dict()] * len(texts)
+            if isinstance(metadata, list):
+                if len(metadata) != len(texts):
+                    raise ValueError('Number of texts does not match with number of metadata.')
+            else:
+                metadata = [metadata] * len(texts)
+            docs = list(map(lambda x: Document(index=x[0], metadata=x[1]), list(zip(texts, metadata))))
+            self.add_documents(docs=docs, split_text=split_text, text_splitter=text_splitter)
+
+    def batch_search(self, queries: List[str], top_k: int = 5, index_only: bool = True,
+                      batch_size: int = 100, filter_fn: Optional[Callable[[Document], bool]] = None, **kwargs) -> List[List[Union[str, Dict[str, Any]]]]:
+        """Batch simlarity search on multiple queries.
 
-    def search(self, query: str, top_k: int = 5, index_only: bool = True, **kwargs) -> List[Union[str, Dict[str, Any]]]:
-        """Similarity search of text on the vector database. Pass keyword arguments as filters on metadata.
+        Args:
+            queries (List[str]): List of queries.
+            top_k (int, optional): Maximum number of results for each query. Defaults to 5.
+            index_only (bool, optional): Whether to return the list of indexes only. Defaults to True.
+            batch_size (int, optional): Batch size to perform similarity search. Defaults to 100.
+            filter_fn (Optional[Callable[[Document], bool]], optional): The filter function to limit the scope of similarity search. Defaults to None.
+
+        Returns:
+            List[List[Union[str, Dict[str, Any]]]]: List of list of search results.
+        """
+        import gc
+        # Filtering the scope of search
+        scope = None
+        if filter_fn:
+            scope = filter(lambda x: filter_fn(x[1]), self.data.items())
+        if kwargs:
+            scope = self.data.items() if scope is None else scope
+            for k, v in kwargs.items():
+                scope = filter(lambda x: x[1].metadata.get(k) == v, scope)
+        ids_scope = scope if scope is None else list(map(lambda x: x[0], scope))
+        top_k = min(self.size, top_k) if ids_scope is None else min(self.size, top_k, len(ids_scope))
+        if top_k == 0:
+            return [[]] * len(queries)
+
+        q_num = len(queries)
+        batch_num = q_num // batch_size if ((q_num // batch_size) == (q_num / batch_size)) else (q_num // batch_size) + 1
+        batches = list(map(lambda x: (x * batch_size, min(q_num, (x + 1) * batch_size)), range(batch_num)))
+        scores = list()
+        ids = list()
+        for b in batches:
+            qvecs = self.embeddings.batch_embed(queries[b[0]:b[1]])
+            score, id = self._batch_search_with_scores(vectors=qvecs, k=top_k, ids_scope=ids_scope)
+            scores.append(score)
+            ids.append(id)
+            del qvecs
+            gc.collect()
+        scores = np.concatenate(scores, axis=0)
+        ids = np.concatenate(ids, axis=0)
+        get_docs = np.vectorize(lambda x: self.data[x])
+        get_indexes = np.vectorize(lambda x: x.index)
+        get_metadatas = np.vectorize(lambda x: x.metadata)
+        get_results = np.vectorize(lambda index, score, id, metadata: dict(index=index, score=score, id=id, metadata=metadata))
+        docs = get_docs(ids)
+        indexes = get_indexes(docs)
+        metadatas = get_metadatas(docs)
+        results = get_results(indexes, scores, ids, metadatas)
+        if index_only:
+            get_str = np.vectorize(lambda x: x['index'])
+            return get_str(results).tolist()
+        else:
+            return results.tolist()
+        
+    def search(self, query: str, top_k: int = 5, index_only: bool = True, filter_fn: Optional[Callable[[Document], bool]] = None, **kwargs) -> List[Union[str, Dict[str, Any]]]:
+        """Simlarity search on the given query.
 
         Args:
-            query (str): Text search string query.
-            top_k (int, optional): Maximum number of results to return. Defaults to 5.
-            index_only (bool, optional): If set as True, only the index string will be returned. Otherwise, metadata and scores will be returned as well. Defaults to True.
+            query (str): Query for similarity search.
+            top_k (int, optional): Maximum number of results. Defaults to 5.
+            index_only (bool, optional): Whether to return the list of indexes only. Defaults to True.
+            filter_fn (Optional[Callable[[Document], bool]], optional): The filter function to limit the scope of similarity search. Defaults to None.
 
         Returns:
             List[Union[str, Dict[str, Any]]]: List of search results.
         """
-        results = self.vectorstore.similarity_search_with_relevance_scores(query=query, k=top_k, fetch_k=max(top_k*2, 20), filter=kwargs)
+        return self.batch_search(queries=[query], top_k=top_k, index_only=index_only,filter_fn=filter_fn, **kwargs)[0]
+            
+    def search_by_metadata(self, ids_only: bool = False, filter_fn: Optional[Callable[[Document], bool]] = None, **kwargs) -> Union[List[int], Dict[int, Document]]:
+        """Search documents or ids by metadata. Pass the filters on metadata as keyword arguments or pass a filter_fn.
 
-        if index_only:
-            results = list(map(lambda x: x[0].page_content, results))
-        else:
-            index = list(map(lambda x: x[0].page_content, results))
-            metadata = list(map(lambda x: x[0].metadata, results))
-            scores = list(map(lambda x: x[1], results))
-            results = list(zip(index, scores, metadata))
-            results = list(map(lambda x: self._result_dict(x[0], x[1], x[2]), results))
-        return results
-    
-    def search_by_metadata(self, **kwargs: Dict[str, Any]) -> Dict[str, Document]:
-        """Exact match search on metadata. Filters should be provided as key value pair arguments.
+        Args:
+            ids_only (bool, optional): Whether to return a list of ids or a dictionary with the ids as keys and documents as values. Defaults to False.
+            filter_fn (Optional[Callable[[Document], bool]], optional): The filter function. Defaults to None.
 
         Returns:
-            Dict[str, Document]: Dictionary of saerch results, with docstore ids as the keys.
+            Union[List[int], Dict[int, Document]]: List of ids or dictionary with the ids as keys and documents as values.
         """
-        results = dict(filter(lambda x: self._dictionary_filter(x, **kwargs), self.vectorstore.docstore._dict.items()))
-        return results
+        results = self.data.items()
+        if filter_fn:
+            results = filter(lambda x: filter_fn(x[1]), results)
+        if kwargs:
+            for k, v in kwargs.items():
+                results = list(filter(lambda x: x[1].metadata.get(k) == v, results))
 
-    def delete_by_metadata(self, **kwargs: Dict[str, Any]) -> None:
-        """Remove records base on the given key value pairs criteria.
+        if ids_only:
+            return list(map(lambda x: x[0], results))
+        return dict(results)
+    
+    def delete_by_metadata(self, filter_fn: Optional[Callable[[Document], bool]] = None, **kwargs) -> None:
+        """Remove records by metadata. Pass the filters on metadata as keyword arguments or pass a filter_fn.
 
-        Raises:
-            ValueError: If not key value pairs given, this error will be raised. To clear the whole vector database, please use the "clear()" method.
+        Args:
+            filter_fn (Optional[Callable[[Document], bool]], optional): The filter function. Defaults to None.
         """
-        if len(kwargs) == 0:
-            raise ValueError(f'Keyword arguments must be provided to remove data from the vector database.')
-        ids = list(self.search_by_metadata(**kwargs).keys())
-        self.vectorstore.delete(ids)
+        if ((not kwargs) and (not filter_fn)):
+            raise ValueError('No keyword arguments or filter_fn are passed. Use the "clear" method to clear the entire database.')
+        ids = self.search_by_metadata(ids_only=True, filter_fn=filter_fn, **kwargs)
+        self._delete(ids)
         self.save()
 
-    
-
+    def clear(self) -> None:
+        """Clear the entire vector database. Use it with caution.
+        """
+        import gc
+        del self._index
+        del self._data
+        gc.collect()
+        self._index = self._get_empty_index()
+        self._data = dict()
+        self.save()
```

### Comparing `llmflex-0.1.5/src/llmflex/Embeddings/api_embeddings.py` & `llmflex-0.1.6/src/llmflex/Embeddings/api_embeddings.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.5/src/llmflex/Embeddings/base_embeddings.py` & `llmflex-0.1.6/src/llmflex/Embeddings/base_embeddings.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.5/src/llmflex/Embeddings/hf_embeddings_server.py` & `llmflex-0.1.6/src/llmflex/Embeddings/hf_embeddings_server.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.5/src/llmflex/Embeddings/huggingface_embeddings.py` & `llmflex-0.1.6/src/llmflex/Embeddings/huggingface_embeddings.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.5/src/llmflex/Frontend/gradio_interface.py` & `llmflex-0.1.6/src/llmflex/Frontend/gradio_interface.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.5/src/llmflex/Frontend/streamlit_interface.py` & `llmflex-0.1.6/src/llmflex/Frontend/streamlit_interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -672,18 +672,15 @@
                 self.history_dict.append(input_dict)
                 self.create_generation_config('new', self.user_input)
                 self.toggle_generating()
                 st.rerun()
             
     def launch(self) -> None:
         if self.islogin:
-            if not self.mobile:
-                st.set_page_config(layout='wide')
-            else:
-                st.set_page_config(layout='centered')
+            st.set_page_config(layout='wide')
             with st.sidebar:
                 self.sidebar()
             self.chatbot()
         else:
             self.login()
 
 def embeddings_loader(embeddings_kwargs: Dict[str, Any]) -> BaseEmbeddingsToolkit:
```

### Comparing `llmflex-0.1.5/src/llmflex/Memory/assistant_long_term_memory.py` & `llmflex-0.1.6/src/llmflex/Memory/assistant_long_term_memory.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.5/src/llmflex/Memory/long_short_memory.py` & `llmflex-0.1.6/src/llmflex/Memory/long_short_memory.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.5/src/llmflex/Models/Cores/base_core.py` & `llmflex-0.1.6/src/llmflex/Models/Cores/base_core.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,36 @@
 from __future__ import annotations
 from langchain.llms.base import LLM
 from langchain.callbacks.manager import CallbackManagerForLLMRun
 from langchain.schema.runnable import RunnableConfig
 from ...Prompts.prompt_template import PromptTemplate, DEFAULT_SYSTEM_MESSAGE
-from abc import ABC, abstractmethod, abstractclassmethod
+from abc import ABC, abstractmethod
 from typing import Any, List, Dict, Optional, Union, Iterator, Type, Tuple, Literal
 
+_chat_formats_map = {
+    'llama-2': 'Llama2',
+    'vicuna': 'Vicuna',
+    'chatml': 'ChatML',
+    'openchat': 'OpenChat',
+    'zephyr': 'Zephyr'
+}
+
 class BaseCore(ABC):
     """Base class of Core object to store the llm model and tokenizer.
     """
     def __init__(self, **kwargs) -> None:
         """Initialising the core instance.
 
         Args:
             model_id (str, optional): Model id (from Huggingface) to use. Defaults to 'gpt2'.
         """
         self._init_config = kwargs
         self._core_type = 'BaseCore'
 
-    @abstractclassmethod
+    @classmethod
     def from_model_object(cls, model: Any, tokenizer: Any, model_id: str, **kwargs) -> BaseCore:
         """Load a core directly from an already loaded model object and a tokenizer object for the supported formats.
 
         Args:
             model (Any): The model object.
             tokenizer (Any): The tokenizer object.
             model_id (str): The model_id.
@@ -102,16 +110,24 @@
     def prompt_template(self) -> PromptTemplate:
         """Default prompt template for the model.
 
         Returns:
             PromptTemplate: Default prompt template for the model.
         """
         if not hasattr(self, '_prompt_template'):
-            from .utils import detect_prompt_template_by_id
-            self._prompt_template = PromptTemplate.from_preset(detect_prompt_template_by_id(self.model_id))
+            from transformers import PreTrainedTokenizer
+            from .utils import detect_prompt_template_by_id, get_prompt_template_by_jinja
+            if isinstance(self.tokenizer, PreTrainedTokenizer):
+                self._prompt_template = get_prompt_template_by_jinja(self.model_id, tokenizer=self.tokenizer)
+            elif self.core_type == 'LlamaCppCore':
+                preset = detect_prompt_template_by_id(self.model_id)
+                preset = _chat_formats_map.get(self._model.chat_format, 'Default') if preset == 'Default' else preset
+                self._prompt_template = PromptTemplate.from_preset(preset)
+            else:
+                self._prompt_template = PromptTemplate.from_preset(detect_prompt_template_by_id(self.model_id))
         return self._prompt_template
     
     def encode(self, text: str) -> List[int]:
         """Tokenize the given text.
 
         Args:
             text (str): Text to tokenize.
```

### Comparing `llmflex-0.1.5/src/llmflex/Models/Cores/exllamav2_core.py` & `llmflex-0.1.6/src/llmflex/Models/Cores/exllamav2_core.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.5/src/llmflex/Models/Cores/huggingface_core.py` & `llmflex-0.1.6/src/llmflex/Models/Cores/huggingface_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,27 +90,25 @@
                    model_kwargs: Optional[Dict[str, Any]] = None, tokenizer_kwargs: Optional[Dict[str, Any]] = None) -> None:
         """Initialise everything needed in the core.
 
         Args:
             model_id (str): The repo ID.
         """
         from ...utils import get_config
-        from .utils import get_prompt_template_by_jinja
         os.environ['HF_HOME'] = get_config()['hf_home']
         os.environ['TOKENIZERS_PARALLELISM'] = 'true'
         from transformers import AutoModelForCausalLM, AutoTokenizer
         self._model_id = model_id
         self._model_type = model_type
         model_kwargs = dict() if model_kwargs is None else model_kwargs
         tokenizer_kwargs = dict() if tokenizer_kwargs is None else tokenizer_kwargs
         if not hasattr(tokenizer_kwargs, 'pretrained_model_name_or_path'):
             tokenizer_kwargs['pretrained_model_name_or_path'] = model_id
         self._tokenizer = AutoTokenizer.from_pretrained(**tokenizer_kwargs)
         self._tokenizer_type = 'transformers'
-        self._prompt_template = get_prompt_template_by_jinja(model_id, self.tokenizer)
 
         if not hasattr(model_kwargs, 'device_map'):
             model_kwargs['device_map'] = 'auto'
         model_kwargs['pretrained_model_name_or_path'] = model_id
         self._model = AutoModelForCausalLM.from_pretrained(**model_kwargs)
 
     @property
```

### Comparing `llmflex-0.1.5/src/llmflex/Models/Cores/llamacpp_core.py` & `llmflex-0.1.6/src/llmflex/Models/Cores/llamacpp_core.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,13 @@
 from __future__ import annotations
 import os
 from langchain.callbacks.manager import CallbackManagerForLLMRun
 from .base_core import BaseCore, BaseLLM
 from typing import Optional, List, Dict, Any, Union, Iterator
 
-_chat_formats_map = {
-    'llama-2': 'Llama2',
-    'vicuna': 'Vicuna',
-    'chatml': 'ChatML',
-    'openchat': 'OpenChat',
-    'zephyr': 'Zephyr'
-}
-
 def get_model_dir(model_id: str, model_file: Optional[str] = None) -> str:
     """Download the model file from Huggingface and get the local directory.
 
     Args:
         model_id (str): Model's HuggingFace ID.
         model_file (Optional[str], optional): Specific model quant file. If None, will choose the smallest quant automatically. Defaults to None.
 
@@ -113,17 +105,14 @@
             del kwargs['use_gpu']
         except:
             pass
         load_kwargs.update(kwargs)
         self._model = Llama(**load_kwargs)
         self._tokenizer = self._model
         self._tokenizer_type = 'llamacpp'
-        preset = detect_prompt_template_by_id(self.model_id)
-        preset = _chat_formats_map.get(self._model.chat_format, 'Default') if preset == 'Default' else preset
-        self._prompt_template = PromptTemplate.from_preset(preset)
 
     def encode(self, text: str) -> List[int]:
         """Tokenize the given text.
 
         Args:
             text (str): Text to tokenize.
```

### Comparing `llmflex-0.1.5/src/llmflex/Models/Cores/openai_core.py` & `llmflex-0.1.6/src/llmflex/Models/Cores/openai_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,29 +60,27 @@
             base_url (Optional[str], optional): URL for the model api endpoint, if None is given, it will use the default URL for OpenAI api. Defaults to None.
             api_key (Optional[str], optional): If using OpenAI api, API key should be provided. Defaults to None.
             model_id (Optional[str], optional): If using OpenAI api or using an api with multiple models, please provide the model to use. Otherwise 'gpt-3.5-turbo' or the first available model will be used by default. Defaults to None.
             tokenizer_id (Optional[str], optional): If not using OpenAI api, repo_id to get the tokenizer from HuggingFace must be provided. Defaults to None.
             tokenizer_kwargs (Optional[Dict[str, Any]], optional): If not using OpenAI api, kwargs can be passed to load the tokenizer from HuggingFace. Defaults to None.
         """
         from openai import OpenAI
-        from .utils import get_prompt_template_by_jinja
         api_key = os.environ.get('OPENAI_API_KEY', 'NOAPIKEY') if api_key is None else api_key
         self._model = OpenAI(api_key=api_key, base_url=base_url)
         models = list(map(lambda x: x.id, self._model.models.list().data))
         self._model_id = model_id if model_id is not None else ('gpt-3.5-turbo' if 'gpt-3.5-turbo' in models else models[0])
         self._is_openai = 'gpt-3.5-turbo' in models
         if tokenizer_id is not None:
             from ...utils import get_config
             os.environ['HF_HOME'] = get_config()['hf_home']
             os.environ['TOKENIZERS_PARALLELISM'] = 'true'
             from transformers import AutoTokenizer
             tokenizer_kwargs = dict() if tokenizer_kwargs is None else tokenizer_kwargs
             self._tokenizer = AutoTokenizer.from_pretrained(tokenizer_id, **tokenizer_kwargs)
             self._tokenizer_type = 'transformers'
-            self._prompt_template = get_prompt_template_by_jinja(self.model_id, self.tokenizer)
         elif self._is_openai:
             import tiktoken
             self._tokenizer = tiktoken.encoding_for_model(self._model_id)
             self._tokenizer_type = 'openai'
         else:
             raise ValueError(f'Cannot infer tokenizer, please specify the tokenizer_id.')
```

### Comparing `llmflex-0.1.5/src/llmflex/Models/Cores/utils.py` & `llmflex-0.1.6/src/llmflex/Models/Cores/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,15 +153,17 @@
         jinja_template (str): Jinja template to test.
 
     Returns:
         str: Prompt template preset.
     """
     from ...Prompts.prompt_template import presets
     for k, v in presets.items():
-        if v['template'] == jinja_template:
+        if jinja_template in v['template']:
+            return k
+        if all(kw in jinja_template for kw in v['keywords']):
             return k
     return 'Default'
 
 def get_prompt_template_by_jinja(model_id: str, tokenizer: Any) -> PromptTemplate:
     """Getting the appropriate prompt template given the huggingface tokenizer.
 
     Args:
```

### Comparing `llmflex-0.1.5/src/llmflex/Models/Factory/llm_factory.py` & `llmflex-0.1.6/src/llmflex/Models/Factory/llm_factory.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.5/src/llmflex/Prompts/prompt_template.py` & `llmflex-0.1.6/src/llmflex/Prompts/prompt_template.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,84 +2,118 @@
 from jinja2 import Environment
 from typing import List, Dict, Any, Optional, Literal, Union, Tuple
 
 DEFAULT_SYSTEM_MESSAGE = """This is a conversation between a human user and a helpful AI assistant."""
 
 presets = {
     'Default' : {
-        'template': "{% if messages[0]['role'] == 'system' %}{% set loop_messages = messages[1:] %}{{ 'SYSTEM:\n' + messages[0]['content'].strip() + '\n\n' }}{% else %}{% set loop_messages = messages %}{% endif %}{% for message in loop_messages %}{% if message['role'] == 'user' %}{{ 'USER: ' + message['content'].strip() + '\n' }}{% elif message['role'] == 'assistant' %}{{ 'ASSISTANT: ' + message['content'].strip() + '\n' }}{% endif %}{% endfor %}{% if add_generation_prompt %}{{ 'ASSISTANT:' }}{% endif %}",
+        'template': "{% if messages[0]['role'] == 'system' %}{% set loop_messages = messages[1:] %}{{ 'SYSTEM:\n' + messages[0]['content'].strip() + '\n\n' }}{% else %}{% set loop_messages = messages %}{% endif %}{% for message in loop_messages %}{% if message['role'] == 'user' %}{{ 'USER: ' + message['content'].strip() + '\n' }}{% elif message['role'] == 'assistant' %}{{ 'ASSISTANT: ' + message['content'].strip() + '\n' }}{% else %}{{ message['role'].upper() + ': ' + message['content'].strip() + eos_token + '\n' }}{% endif %}{% endfor %}{% if add_generation_prompt %}{{ 'ASSISTANT:' }}{% endif %}",
         'eos_token': '</s>',
         'bos_token': '<s>',
         'stop': ['\nASSISTANT', '\nUSER:', 'ASSISTANT:', 'USER:']
     },
     'Llama2' : {
         'template': "{% if messages[0]['role'] == 'system' %}{% set loop_messages = messages[1:] %}{% set system_message = messages[0]['content'] %}{% elif false == true and not '<<SYS>>' in messages[0]['content'] %}{% set loop_messages = messages %}{% set system_message = 'You are a helpful, respectful and honest assistant. Always answer as helpfully as possible, while being safe. Your answers should not include any harmful, unethical, racist, sexist, toxic, dangerous, or illegal content. Please ensure that your responses are socially unbiased and positive in nature.\\n\\nIf a question does not make any sense, or is not factually coherent, explain why instead of answering something not correct. If you don\\'t know the answer to a question, please don\\'t share false information.' %}{% else %}{% set loop_messages = messages %}{% set system_message = false %}{% endif %}{% for message in loop_messages %}{% if (message['role'] == 'user') != (loop.index0 % 2 == 0) %}{{ raise_exception('Conversation roles must alternate user/assistant/user/assistant/...') }}{% endif %}{% if loop.index0 == 0 and system_message != false %}{% set content = '<<SYS>>\\n' + system_message + '\\n<</SYS>>\\n\\n' + message['content'] %}{% else %}{% set content = message['content'] %}{% endif %}{% if message['role'] == 'user' %}{{ bos_token + '[INST] ' + content.strip() + ' [/INST]' }}{% elif message['role'] == 'system' %}{{ '<<SYS>>\\n' + content.strip() + '\\n<</SYS>>\\n\\n' }}{% elif message['role'] == 'assistant' %}{{ ' '  + content.strip() + ' ' + eos_token }}{% endif %}{% endfor %}",
         'eos_token': '</s>',
         'bos_token': '<s>',
-        'stop': ['</s>', '</s><s>', '[INST]', '<s>[INST]']
+        'stop': ['</s>', '</s><s>', '[INST]', '<s>[INST]'],
+        'keywords': ['[INST]', '[/INST]']
     },
     'Llama3' : {
         'template': "{% if not add_generation_prompt is defined %}{% set add_generation_prompt = false %}{% endif %}{% set loop_messages = messages %}{% for message in loop_messages %}{% set content = '<|start_header_id|>' + message['role'] + '<|end_header_id|>\n\n'+ message['content'] | trim + '<|eot_id|>' %}{% if loop.index0 == 0 %}{% set content = bos_token + content %}{% endif %}{{ content }}{% endfor %}{% if add_generation_prompt %}{{ '<|start_header_id|>assistant<|end_header_id|>\n\n' }}{% else %}{{ eos_token }}{% endif %}",
         'eos_token': '<|end_of_text|>',
         'bos_token': '<|begin_of_text|>',
-        'stop': ['</s>', '<|end_of_text|>', '<|eot_id|>', '<|start_header_id|>']
+        'stop': ['</s>', '<|end_of_text|>', '<|eot_id|>', '<|start_header_id|>'],
+        'keywords': ['<|start_header_id|>', '<|end_header_id|>']
     },
     'Vicuna' : {
         'template': "{% if messages[0]['role'] == 'system' %}{% set loop_messages = messages[1:] %}{{ messages[0]['content'].strip() + '\n\n' }}{% else %}{% set loop_messages = messages %}{% endif %}{% for message in loop_messages %}{% if message['role'] == 'user' %}{{ 'USER: ' + message['content'].strip() + '\n' }}{% elif message['role'] == 'assistant' %}{{ 'ASSISTANT: ' + message['content'].strip() + eos_token + '\n' }}{% endif %}{% endfor %}{% if add_generation_prompt %}{{ 'ASSISTANT:' }}{% endif %}",
         'eos_token': '</s>',
         'bos_token': '<s>',
-        'stop': ['\nASSISTANT', '\nUSER:', 'ASSISTANT:', 'USER:', '</s>']
+        'stop': ['\nASSISTANT', '\nUSER:', 'ASSISTANT:', 'USER:', '</s>'],
+        'keywords': ['USER:', 'ASSISTANT:']
     },
     'ChatML' : {
-        'template': "{% for message in messages %}{{'<|im_start|>' + message['role'] + '\n' + message['content'] + '<|im_end|>' + '\n'}}{% endfor %}{% if add_generation_prompt %}{{ '<|im_start|>assistant\n' }}{% endif %}",
+        'template': "{{bos_token}}{% for message in messages %}{{'<|im_start|>' + message['role'] + '\n' + message['content'] + '<|im_end|>' + '\n'}}{% endfor %}{% if add_generation_prompt %}{{ '<|im_start|>assistant\n' }}{% endif %}",
         'eos_token': '<|im_end|>',
-        'bos_token': '<|endoftext|>',
-        'stop': ['<|im_start|>', '<|im_end|>', '<|im_start|>user\n', '<|im_end|>\n<|im_start|>user\n', '</s>']
+        'bos_token': '<s>',
+        'stop': ['<|im_start|>', '<|im_end|>', '<|im_start|>user\n', '<|im_end|>\n<|im_start|>user\n', '</s>'],
+        'keywords': ['<|im_start|>', '<|im_end|>']
     },
     'Zephyr' : {
         'template': "{% for message in messages %}\n{% if message['role'] == 'user' %}\n{{ '<|user|>\n' + message['content'] + eos_token }}\n{% elif message['role'] == 'system' %}\n{{ '<|system|>\n' + message['content'] + eos_token }}\n{% elif message['role'] == 'assistant' %}\n{{ '<|assistant|>\n'  + message['content'] + eos_token }}\n{% endif %}\n{% if loop.last and add_generation_prompt %}\n{{ '<|assistant|>' }}\n{% endif %}\n{% endfor %}",
         'eos_token': '</s>',
         'bos_token': '<s>',
-        'stop': ['</s>', '</s>\n', '<|user|>\n', '</s>\n<|user|>\n']
+        'stop': ['</s>', '</s>\n', '<|user|>\n', '</s>\n<|user|>\n'],
+        'keywords': ['<|system|>']
     },
     'OpenChat' : {
         'template': "{{ bos_token }}{% for message in messages %}{{ 'GPT4 Correct ' + message['role'].title() + ': ' + message['content'] + '<|end_of_turn|>'}}{% endfor %}{% if add_generation_prompt %}{{ 'GPT4 Correct Assistant:' }}{% endif %}",
         'eos_token': '<|end_of_turn|>',
         'bos_token': '<s>',
-        'stop': ['</s>', '<|end_of_turn|>', '<|end_of_turn|>GPT4 Correct Assistant: ']
+        'stop': ['</s>', '<|end_of_turn|>', '<|end_of_turn|>GPT4 Correct Assistant: '],
+        'keywords': ['GPT4 Correct']
     },
     'Alpaca' : {
         'template': "{% for message in messages %}{% if message['role'] == 'system' %}{% if message['content']%}{{'### Instruction: ' + message['content']+'\n'}}{% endif %}{% elif message['role'] == 'user' %}{{'### Input: ' + message['content']+'\n'}}{% elif message['role'] == 'assistant' %}{{'### Response: '  + message['content'] + '\n'}}{% endif %}{% if loop.last and add_generation_prompt %}{{ '### Response:' }}{% endif %}{% endfor %}",
         'eos_token': '<|end_of_turn|>',
         'bos_token': '<s>',
-        'stop': ['### Input: ', '\n### Input: ', '###']
+        'stop': ['### Input: ', '\n### Input: ', '###'],
+        'keywords': ['### Input:', '### Response:']
+    },
+    'Phi3' : {
+        'template': "{{ bos_token }}{% for message in messages %}{% if (message['role'] == 'user') %}{{'<|user|>' + '\n' + message['content'] + '<|end|>' + '\n' + '<|assistant|>' + '\n'}}{% elif (message['role'] == 'assistant') %}{{message['content'] + '<|end|>' + '\n'}}{% endif %}{% endfor %}",
+        'eos_token': '<|endoftext|>',
+        'bos_token': '<s>',
+        'stop': ['<|end|>', '<|endoftext|>'],
+        'keywords': ['<|end|>']
     },
 }
 
 hidden_presets = {
     'Llama2' : {
         'template': "{% if messages[0]['role'] == 'system' %}{% set loop_messages = messages[1:] %}{% set system_message = messages[0]['content'] %}{% else %}{% set loop_messages = messages %}{% set system_message = false %}{% endif %}{% for message in loop_messages %}{% if loop.index0 == 0 and system_message != false %}{% set content = '<<SYS>>\\n' + system_message + '\\n<</SYS>>\\n\\n' + message['content'] %}{% else %}{% set content = message['content'] %}{% endif %}{% if message['role'] == 'user' %}{% if loop.index0 == 0 %}{{ '[INST] ' + content.strip() + ' [/INST]' }}{% else %}{{ bos_token + '[INST] ' + content.strip() + ' [/INST]' }}{% endif %}{% elif message['role'] == 'system' %}{{ '<<SYS>>\\n' + content.strip() + '\\n<</SYS>>\\n\\n' }}{% elif message['role'] == 'assistant' %}{% if loop.index0 == 0 and system_message != false %}{% set prefix = '[INST]' + '<<SYS>>\\n' + system_message + '\\n<</SYS>>\\n\\n' + '[/INST] ' %}{% set content = message['content'] %}{% elif loop.index0 == 0 %}{% set prefix = '[INST][/INST] ' %}{% set content = message['content'] %}{% else %}{% set prefix = ' ' %}{% endif %}{{ prefix  + content.strip() + ' ' + eos_token }}{% endif %}{% endfor %}",
         'eos_token': '</s>',
         'bos_token': '<s>',
         'stop': ['</s>', '</s><s>', '[INST]', '<s>[INST]']
-    }
+    },
+    'Zephyr' : {
+        'template': "{% for message in messages %}\n{% if message['role'] == 'user' %}\n{{ '<|user|>\n' + message['content'] + eos_token }}\n{% elif message['role'] == 'system' %}\n{{ '<|system|>\n' + message['content'] + eos_token }}\n{% elif message['role'] == 'assistant' %}\n{{ '<|assistant|>\n'  + message['content'] + eos_token }}\n{% else  %}\n{{ '<|' + message['role'] + '|>\n'  + message['content'] + eos_token }}\n{% endif %}\n{% if loop.last and add_generation_prompt %}\n{{ '<|assistant|>' }}\n{% endif %}\n{% endfor %}",
+        'eos_token': '</s>',
+        'bos_token': '<s>',
+        'stop': ['</s>', '</s>\n', '<|user|>\n', '</s>\n<|user|>\n']
+    },
+    'Vicuna' : {
+        'template': "{% if messages[0]['role'] == 'system' %}{% set loop_messages = messages[1:] %}{{ messages[0]['content'].strip() + '\n\n' }}{% else %}{% set loop_messages = messages %}{% endif %}{% for message in loop_messages %}{% if message['role'] == 'user' %}{{ 'USER: ' + message['content'].strip() + '\n' }}{% elif message['role'] == 'assistant' %}{{ 'ASSISTANT: ' + message['content'].strip() + eos_token + '\n' }}{% else %}{{ message['role'].upper() + ': ' + message['content'].strip() + eos_token + '\n' }}{% endif %}{% endfor %}{% if add_generation_prompt %}{{ 'ASSISTANT:' }}{% endif %}",
+        'eos_token': '</s>',
+        'bos_token': '<s>',
+        'stop': ['\nASSISTANT', '\nUSER:', 'ASSISTANT:', 'USER:', '</s>']
+    },
+    'Phi3' : {
+        'template': "{{ bos_token }}{% for message in messages %}{{'<|' + message['role'] + '|>' + '\n' + message['content'] + '<|end|>' + '\n'}}{% endfor %}{% if add_generation_prompt %}{{ '<|assistant|>\n' }}{% endif %}",
+        'eos_token': '<|endoftext|>',
+        'bos_token': '<s>',
+        'stop': ['<|end|>', '<|endoftext|>'],
+        'keywords': ['<|end|>']
+    },
 }
 
-PRESET_FORMATS =  Literal['Default', 'Llama2', 'Llama3', 'Vicuna', 'ChatML', 'Zephyr', 'OpenChat', 'Alpaca']
+PRESET_FORMATS =  Literal['Default', 'Llama2', 'Llama3', 'Vicuna', 'ChatML', 'Zephyr', 'OpenChat', 'Alpaca', 'Phi3']
 
 class PromptTemplate:
     """Class for storing prompt format presets.
     """
     def __init__(
             self,
             template: str,
             eos_token: Optional[str],
             bos_token: Optional[str],
             stop: Optional[List[str]] = None,
-            force_real_template: bool = False
+            force_real_template: bool = False,
+            **kwargs
     ) -> None:
         """Initialising the chat prompt class.
 
         Args:
             template (str): Jinja2 template.
             eos_token (Optional[str]): EOS token string.
             bos_token (Optional[str]): BOS token string.
@@ -87,36 +121,58 @@
             force_real_template (bool, optional): Whether to render the given template. For most templates it has no effects. Only for some restrictive templates like llama2. Defaults to False.
         """
         self._template = template
         self._eos_token = eos_token
         self._bos_token = bos_token
         self._stop = stop
         self._force_real_template = force_real_template
+        self._keywords = kwargs.get('keywords', [])
 
     @property
     def template(self) -> str:
+        """Jinja template string.
+
+        Returns:
+            str: Jinja template string.
+        """
         return self._template
     
     @property
     def _hidden_template(self) -> str:
         """To fix issues with some default templates like llama 2.
 
         Returns:
             str: The actual template to be rendered.
         """
         config = hidden_presets.get(self.template_name)
         return self.template if config is None else config['template']
     
     @property
     def rendered_template(self) -> Environment:
+        """Rendered Jinja template.
+
+        Returns:
+            Environment: Rendered Jinja template.
+        """
         if not hasattr(self, '_rendered_template'):
             from jinja2 import BaseLoader
             template = self.template if self._force_real_template else self._hidden_template
             self._rendered_template = Environment(loader=BaseLoader).from_string(template)
         return self._rendered_template
+    
+    @property
+    def keywords(self) -> List[str]:
+        """List of keywords to search for in Jinja templates for template detection. Used for presets.
+
+        Returns:
+            List[str]: List of keywords to search for in Jinja templates for template detection.
+        """
+        if not hasattr(self, '_keywords'):
+            self._keywords = []
+        return self._keywords
 
     @property
     def eos_token(self) -> Optional[str]:
         return self._eos_token
     
     @property
     def bos_token(self) -> Optional[str]:
@@ -136,14 +192,32 @@
         if not hasattr(self, '_template_name'):
             self._template_name = 'Unititled template'
             for k, v in presets.items():
                 if self.template == v['template']:
                     self._template_name = k
                     break
         return self._template_name
+    
+    @property
+    def allow_custom_role(self) -> bool:
+        """Check if custom role can be used with the prompt template.
+
+        Returns:
+            bool: Whether custom role can be used with the prompt template.
+        """
+        if not hasattr(self, '_allow_custom_role'):
+            test = [dict(role='user', content='random message'), dict(role='customrole', content='exist')]
+            try: 
+                output = self.create_custom_prompt(test)
+                self._allow_custom_role = 'customrole' in output.lower()
+            except:
+                self._allow_custom_role = False
+        return self._allow_custom_role
+
+
 
     def format_history(self, history: Union[List[str], List[Tuple[str, str]]], return_list: bool = False) -> Union[str, List[Dict[str, str]]]:
         """Formatting a list of conversation history into a full string of conversation history or a list of messages for the Jinja template to render.
 
         Args:
             history (Union[List[str], List[Tuple[str, str]]]): List of conversation history. 
             return_list (bool, optional): Whether to return a list of messages for the Jinja template to render. Defaults to False.
@@ -174,15 +248,15 @@
             user (str): Latest user input.
             system (str, optional): System message. Defaults to DEFAULT_SYSTEM_MESSAGE.
             history (Optional[Union[List[str], List[Tuple[str, str]]]], optional): List of conversation history. Defaults to None.
 
         Returns:
             str: The full prompt.
         """
-        head = [dict(role='system', content=system)] if system.strip(' \n\r\t') != '' else []
+        head = [dict(role='system', content=system)] if system.strip() != '' else []
         history = [] if history is None else history
         body = self.format_history(history=history, return_list=True)
         tail = [dict(role='user', content=user)]
         prompt = head + body + tail
         return self.rendered_template.render(messages=prompt, bos_token=self.bos_token, eos_token=self.eos_token, add_generation_prompt=True)
     
     def create_custom_prompt(self, messages: List[Dict[str, str]], add_generation_prompt: bool = True) -> str:
@@ -193,14 +267,43 @@
             add_generation_prompt (bool, optional): Whether to add the assistant tokens at the end of the prompt. Defaults to True.
 
         Returns:
             str: The full prompt given your messages.
         """
         return self.rendered_template.render(messages=messages, bos_token=self.bos_token, eos_token=self.eos_token, add_generation_prompt=add_generation_prompt)
     
+    def create_custom_prompt_with_open_role(self, messages: List[Dict[str, str]], end_role: str = '', begin_text: str = '') -> str:
+        """Creating a custom prompt with your given list of messages. Each message should contain a dictionary with the key "role" and "content". The prompt will end with starting prompt of the end_role instead of assistant.
+
+        Args:
+            messages (List[Dict[str, str]]): List of messages. Each message should contain a dictionary with the key "role" and "content".
+            end_role (str, optional): The role for text generation instead of assistant. If an empty string is given, it means that the role can be anything the llm is going to generate. Defaults to ''.
+            begin_text (str, optional): The beginning text of the last role. Defaults to ''.
+
+        Returns:
+            str: The full prompt with your custom role.
+        """
+        if self.allow_custom_role:
+            role_ph = end_role if end_role.strip() != '' else 'place_holder_role'
+            text_ph = '$$$PLACE_HOLDER_TEXT$$$'
+            prompt = self.create_custom_prompt(messages=messages + [dict(role=role_ph, content=text_ph)], add_generation_prompt=False)
+            prompt = text_ph.join(prompt.split(text_ph)[:-1])
+            real = self.create_custom_prompt(messages=messages + [dict(role=end_role, content=text_ph)], add_generation_prompt=False)
+            real = text_ph.join(real.split(text_ph)[:-1])
+            if real == prompt:
+                return real + begin_text
+            elif begin_text.strip() != '':
+                return real + begin_text
+            else:
+                import os
+                return os.path.commonprefix([real, prompt])
+        else:
+            raise AssertionError(f'This prompt template "{self.template_name}" does not allow custom_roles.')
+
+    
     @classmethod
     def from_dict(cls, format_dict: Dict[str, Any], template_name: Optional[str] = None) -> PromptTemplate:
         """Initialise the prompt template from a dictionary.
 
         Args:
             format_dict (Dict[str, Any]): Dictionary of the prompt format.
             template_name (Optional[str], optional): Name of the template. Defaults to None.
```

### Comparing `llmflex-0.1.5/src/llmflex/Rankers/base_ranker.py` & `llmflex-0.1.6/src/llmflex/Rankers/base_ranker.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.5/src/llmflex/Rankers/flashrank_ranker.py` & `llmflex-0.1.6/src/llmflex/Rankers/flashrank_ranker.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.5/src/llmflex/Schemas/documents.py` & `llmflex-0.1.6/src/llmflex/Schemas/documents.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.5/src/llmflex/Schemas/tokenizer.py` & `llmflex-0.1.6/src/llmflex/Schemas/tokenizer.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.5/src/llmflex/TextSplitters/base_text_splitter.py` & `llmflex-0.1.6/src/llmflex/TextSplitters/base_text_splitter.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.5/src/llmflex/TextSplitters/sentence_token_text_splitter.py` & `llmflex-0.1.6/src/llmflex/TextSplitters/sentence_token_text_splitter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,33 @@
-from typing import Callable, List
 from .base_text_splitter import BaseTextSplitter
+from spacy.language import Language
+from typing import Callable, List, Union
 
 class SentenceTokenTextSplitter(BaseTextSplitter):
     """Text splitter that split text by sentences and group by token counts.
     """
-    def __init__(self, count_token_fn: Callable[[str], int], language_model: str = 'en_core_web_sm', chunk_size: int = 400, chunk_overlap: int = 40) -> None:
+    def __init__(self, count_token_fn: Callable[[str], int], language_model: Union[str, Language] = 'en_core_web_sm', chunk_size: int = 400, chunk_overlap: int = 40) -> None:
         """Initialise the TextSplitter.
 
         Args:
             count_token_fn (Callable[[str], int]): Function to count the number of tokens in a string.
-            language_model (str, optional): Name of the SpaCy model to use. Defaults to 'en_core_web_sm'.
+            language_model (Union[str, Language], optional): Name of the SpaCy model or the SpaCy model to use. Defaults to 'en_core_web_sm'.
             chunk_size (int, optional): Maximum number of tokens per text chunk. Defaults to 400.
             chunk_overlap (int, optional): Numbers of tokens that overlaps for each subsequent chunks. Defaults to 40.
         """
         import spacy
         from spacy.cli import download
         from spacy.util import is_package
         if not is_package(language_model):
             try:
                 download(language_model)
             except:
                 raise RuntimeError(f'Failed to download the SpaCy languange model "{language_model}".')
         super().__init__(chunk_size=chunk_size, chunk_overlap=chunk_overlap)
-        self.nlp = spacy.load(language_model)
+        self.nlp = spacy.load(language_model) if isinstance(language_model, str) else language_model
         self.count_fn = count_token_fn
         self._language_model = language_model
     
     def split_text(self, text: str) -> List[str]:
         """Splitting the given text.
 
         Args:
```

### Comparing `llmflex-0.1.5/src/llmflex/TextSplitters/token_text_splitter.py` & `llmflex-0.1.6/src/llmflex/TextSplitters/token_text_splitter.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.5/src/llmflex/Tools/base_tool.py` & `llmflex-0.1.6/src/llmflex/Tools/base_tool.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.5/src/llmflex/Tools/tool_selection.py` & `llmflex-0.1.6/src/llmflex/Tools/tool_selection.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.5/src/llmflex/Tools/web_search_tool.py` & `llmflex-0.1.6/src/llmflex/Tools/web_search_tool.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.5/src/llmflex/Tools/web_search_utils.py` & `llmflex-0.1.6/src/llmflex/Tools/web_search_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from bs4 import BeautifulSoup, NavigableString, Tag
 from langchain.llms.base import LLM
-from typing import Optional, List, Union, Callable
+from typing import Optional, List, Union, Callable, Dict, Any
 
 def get_soup_from_url(url: str, timeout: int = 8) -> BeautifulSoup:
     """Get the soup object from a URL.
 
     Args:
         url (str): URL of the  website.
         timeout (int, optional): Timeout for the request in seconds. Defaults to 8.
@@ -416,7 +416,25 @@
         as_list (bool, optional): Whether to return the content as a list or as a string. Defaults to False.
 
     Returns:
         Union[str, List[str]]: Content of the URL as a string or a list of string.
     """
     soup = get_soup_from_url(url, timeout=timeout)
     return process_element(soup, as_list=as_list)
+
+def ddg_search(query: str, n: int = 5, urls_only: bool = True, **kwargs) -> List[Union[str, Dict[str, Any]]]:
+    """Search with DuckDuckGo.
+
+    Args:
+        query (str): Search query.
+        n (int, optional): Maximum number of results. Defaults to 5.
+        urls_only (bool, optional): Only return the list of urls or return other information as well. Defaults to True.
+
+    Returns:
+        List[Union[str, Dict[str, Any]]]: List of search results.
+    """
+    from duckduckgo_search import DDGS
+    with DDGS() as ddgs:
+        results = [r for r in ddgs.text(query, max_results=n, **kwargs)]
+    if urls_only:
+        results = list(map(lambda x: x['href'], results))
+    return results
```

### Comparing `llmflex-0.1.5/src/llmflex/VectorDBs/faiss_vectordb.py` & `llmflex-0.1.6/src/llmflex/VectorDBs/faiss_vectordb.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.5/src/llmflex/cli.py` & `llmflex-0.1.6/src/llmflex/cli.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.5/src/llmflex/utils.py` & `llmflex-0.1.6/src/llmflex/utils.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.5/src/llmflex.egg-info/PKG-INFO` & `llmflex-0.1.6/src/llmflex.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmflex
-Version: 0.1.5
+Version: 0.1.6
 Summary: A python package for developing AI applications with local LLMs.
 Author-email: Nathan Tam <nathan1295@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/nath1295/LLMFlex
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
@@ -24,25 +24,31 @@
 Requires-Dist: tiktoken
 Requires-Dist: protobuf
 Requires-Dist: beautifulsoup4
 Requires-Dist: streamlit
 Requires-Dist: watchdog
 Requires-Dist: spacy>=3.7.0
 Requires-Dist: flask
+Requires-Dist: PyMuPDF
+Requires-Dist: python-docx
 Provides-Extra: cu121
 Requires-Dist: auto-gptq>=0.6.0; extra == "cu121"
 Requires-Dist: autoawq; extra == "cu121"
 Requires-Dist: exllamav2; extra == "cu121"
 Provides-Extra: cu118
 Requires-Dist: auto-gptq; extra == "cu118"
 Requires-Dist: autoawq; extra == "cu118"
 Requires-Dist: exllamav2; extra == "cu118"
 
 # LLMFlex
+[![PyPI](https://img.shields.io/pypi/v/llmflex)](https://pypi.org/project/llmflex/)
+[![PyPI - License](https://img.shields.io/pypi/l/llmflex)](https://pypi.org/project/llmflex/)
+[![GitHub Repo stars](https://img.shields.io/github/stars/nath1295/llmflex)](https://pypi.org/project/llmflex/)
 
+## A python package for developing AI applications with local LLMs
 LLMFlex is a python package that allows python developers to work with different large language models (LLM) and do prompt engineering with a simple interface. It favours free and local resources instead of using paid APIs to develop truly local and private AI-powered solutions.
 
 It provides classes to load LLM models, embedding models, and vector databases to create LLM powered applications with your own prompt engineering and RAG techniques. With a one-liner command, you can load a chatbot interface to chat with the LLM or serve a model as OpenAI API as well.
 
 ## Installing LLMFlex
 Creating a virtual environment before installing the package is highly recommended. Also make sure you have installed [Pytorch](https://pytorch.org/get-started/locally/) and [llama-cpp-python](https://pypi.org/project/llama-cpp-python/) with the correct installation method according to your hardware configuration before installing LLMFlex. Please visit the links provided for the respective packages for more detailed installation guides.
```

### Comparing `llmflex-0.1.5/src/llmflex.egg-info/SOURCES.txt` & `llmflex-0.1.6/src/llmflex.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 src/llmflex/utils.py
 src/llmflex.egg-info/PKG-INFO
 src/llmflex.egg-info/SOURCES.txt
 src/llmflex.egg-info/dependency_links.txt
 src/llmflex.egg-info/entry_points.txt
 src/llmflex.egg-info/requires.txt
 src/llmflex.egg-info/top_level.txt
-src/llmflex/Data/__init__.py
-src/llmflex/Data/sqlite_database.py
-src/llmflex/Data/vector_database.py
 src/llmflex/Embeddings/__init__.py
 src/llmflex/Embeddings/api_embeddings.py
 src/llmflex/Embeddings/base_embeddings.py
 src/llmflex/Embeddings/hf_embeddings_server.py
 src/llmflex/Embeddings/huggingface_embeddings.py
 src/llmflex/Frontend/__init__.py
 src/llmflex/Frontend/gradio_interface.py
 src/llmflex/Frontend/streamlit_interface.py
+src/llmflex/KnowledgeBase/__init__.py
+src/llmflex/KnowledgeBase/knowledge_base.py
 src/llmflex/Memory/__init__.py
 src/llmflex/Memory/assistant_long_term_memory.py
 src/llmflex/Memory/base_memory.py
 src/llmflex/Memory/long_short_memory.py
+src/llmflex/Memory/longshort_memory.py
 src/llmflex/Models/__init__.py
 src/llmflex/Models/Cores/__init__.py
 src/llmflex/Models/Cores/base_core.py
 src/llmflex/Models/Cores/exllamav2_core.py
 src/llmflex/Models/Cores/huggingface_core.py
 src/llmflex/Models/Cores/llamacpp_core.py
 src/llmflex/Models/Cores/openai_core.py
@@ -45,13 +45,16 @@
 src/llmflex/Schemas/tokenizer.py
 src/llmflex/TextSplitters/__init__.py
 src/llmflex/TextSplitters/base_text_splitter.py
 src/llmflex/TextSplitters/sentence_token_text_splitter.py
 src/llmflex/TextSplitters/token_text_splitter.py
 src/llmflex/Tools/__init__.py
 src/llmflex/Tools/base_tool.py
+src/llmflex/Tools/browser_tool.py
+src/llmflex/Tools/tool_prompting.py
 src/llmflex/Tools/tool_selection.py
+src/llmflex/Tools/tool_utils.py
 src/llmflex/Tools/web_search_tool.py
 src/llmflex/Tools/web_search_utils.py
 src/llmflex/VectorDBs/__init__.py
 src/llmflex/VectorDBs/base_vectordb.py
 src/llmflex/VectorDBs/faiss_vectordb.py
```

