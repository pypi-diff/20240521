# Comparing `tmp/langchain_rag-0.1.52.tar.gz` & `tmp/langchain_rag-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_rag-0.1.52.tar", max compression
+gzip compressed data, was "langchain_rag-0.2.0.tar", max compression
```

## Comparing `langchain_rag-0.1.52.tar` & `langchain_rag-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    11357 2023-10-19 05:47:38.233379 langchain_rag-0.1.52/LICENSE.txt
--rw-r--r--   0        0        0     2155 2024-02-07 08:38:30.870089 langchain_rag-0.1.52/README.md
--rw-r--r--   0        0        0        0 2023-10-23 07:07:51.650962 langchain_rag-0.1.52/langchain_rag/__init__.py
--rw-r--r--   0        0        0      698 2024-04-23 11:15:14.817186 langchain_rag-0.1.52/langchain_rag/document_transformers/__init__.py
--rw-r--r--   0        0        0     1096 2024-01-29 11:57:32.041286 langchain_rag-0.1.52/langchain_rag/document_transformers/copy_transformer.py
--rw-r--r--   0        0        0     2859 2024-04-23 11:15:14.817186 langchain_rag-0.1.52/langchain_rag/document_transformers/document_transform_pipeline.py
--rw-r--r--   0        0        0     6134 2024-04-23 11:15:14.817186 langchain_rag-0.1.52/langchain_rag/document_transformers/document_transformers.py
--rw-r--r--   0        0        0     3978 2024-01-29 11:07:27.844752 langchain_rag-0.1.52/langchain_rag/document_transformers/generate_questions.py
--rw-r--r--   0        0        0     9254 2024-04-23 11:17:36.261006 langchain_rag-0.1.52/langchain_rag/document_transformers/runnable_document_transformer.py
--rw-r--r--   0        0        0     4740 2024-04-23 11:15:14.821186 langchain_rag-0.1.52/langchain_rag/document_transformers/summarize_and_questions_transformer.py
--rw-r--r--   0        0        0     3257 2024-04-23 11:15:14.821186 langchain_rag-0.1.52/langchain_rag/document_transformers/summarize_transformer.py
--rw-r--r--   0        0        0       89 2024-01-24 09:40:10.848052 langchain_rag-0.1.52/langchain_rag/indexes/__init__.py
--rw-r--r--   0        0        0     3637 2024-01-24 07:30:49.261495 langchain_rag-0.1.52/langchain_rag/indexes/memory_recordmanager.py
--rw-r--r--   0        0        0        0 2024-04-23 11:15:14.821186 langchain_rag-0.1.52/langchain_rag/patch_langchain_community/__init__.py
--rw-r--r--   0        0        0        0 2024-04-23 11:15:14.821186 langchain_rag-0.1.52/langchain_rag/patch_langchain_community/indexes/__init__.py
--rw-r--r--   0        0        0    21023 2024-05-07 08:27:10.339308 langchain_rag-0.1.52/langchain_rag/patch_langchain_community/indexes/_sql_record_manager.py
--rw-r--r--   0        0        0       59 2023-11-02 16:16:50.944534 langchain_rag-0.1.52/langchain_rag/storage/__init__.py
--rw-r--r--   0        0        0     8371 2024-05-16 08:17:57.407069 langchain_rag-0.1.52/langchain_rag/storage/sql_docstore.py
--rw-r--r--   0        0        0      247 2024-05-16 08:17:55.931065 langchain_rag-0.1.52/langchain_rag/test_p.py
--rw-r--r--   0        0        0      148 2023-11-02 16:16:50.948534 langchain_rag-0.1.52/langchain_rag/vectorstores/__init__.py
--rw-r--r--   0        0        0    36578 2024-05-16 08:18:29.515150 langchain_rag-0.1.52/langchain_rag/vectorstores/rag_vectorstore.py
--rw-r--r--   0        0        0     6658 2024-01-24 07:30:49.265495 langchain_rag-0.1.52/langchain_rag/vectorstores/wrapper_vectorstore.py
--rw-r--r--   0        0        0     3816 2024-05-15 14:59:30.039235 langchain_rag-0.1.52/pyproject.toml
--rw-r--r--   0        0        0     2948 1970-01-01 00:00:00.000000 langchain_rag-0.1.52/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-10-19 05:47:38.233379 langchain_rag-0.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     2155 2024-02-07 08:38:30.870089 langchain_rag-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-10-23 07:07:51.650962 langchain_rag-0.2.0/langchain_rag/__init__.py
+-rw-r--r--   0        0        0      698 2024-04-23 11:15:14.817186 langchain_rag-0.2.0/langchain_rag/document_transformers/__init__.py
+-rw-r--r--   0        0        0     1096 2024-01-29 11:57:32.041286 langchain_rag-0.2.0/langchain_rag/document_transformers/copy_transformer.py
+-rw-r--r--   0        0        0     2859 2024-04-23 11:15:14.817186 langchain_rag-0.2.0/langchain_rag/document_transformers/document_transform_pipeline.py
+-rw-r--r--   0        0        0     6134 2024-04-23 11:15:14.817186 langchain_rag-0.2.0/langchain_rag/document_transformers/document_transformers.py
+-rw-r--r--   0        0        0     3978 2024-01-29 11:07:27.844752 langchain_rag-0.2.0/langchain_rag/document_transformers/generate_questions.py
+-rw-r--r--   0        0        0     9254 2024-04-23 11:17:36.261006 langchain_rag-0.2.0/langchain_rag/document_transformers/runnable_document_transformer.py
+-rw-r--r--   0        0        0     4740 2024-04-23 11:15:14.821186 langchain_rag-0.2.0/langchain_rag/document_transformers/summarize_and_questions_transformer.py
+-rw-r--r--   0        0        0     3257 2024-04-23 11:15:14.821186 langchain_rag-0.2.0/langchain_rag/document_transformers/summarize_transformer.py
+-rw-r--r--   0        0        0       89 2024-01-24 09:40:10.848052 langchain_rag-0.2.0/langchain_rag/indexes/__init__.py
+-rw-r--r--   0        0        0     3637 2024-01-24 07:30:49.261495 langchain_rag-0.2.0/langchain_rag/indexes/memory_recordmanager.py
+-rw-r--r--   0        0        0        0 2024-04-23 11:15:14.821186 langchain_rag-0.2.0/langchain_rag/patch_langchain_community/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-23 11:15:14.821186 langchain_rag-0.2.0/langchain_rag/patch_langchain_community/indexes/__init__.py
+-rw-r--r--   0        0        0    21023 2024-05-07 08:27:10.339308 langchain_rag-0.2.0/langchain_rag/patch_langchain_community/indexes/_sql_record_manager.py
+-rw-r--r--   0        0        0       59 2023-11-02 16:16:50.944534 langchain_rag-0.2.0/langchain_rag/storage/__init__.py
+-rw-r--r--   0        0        0     8371 2024-05-16 08:17:57.407069 langchain_rag-0.2.0/langchain_rag/storage/sql_docstore.py
+-rw-r--r--   0        0        0      247 2024-05-16 08:17:55.931065 langchain_rag-0.2.0/langchain_rag/test_p.py
+-rw-r--r--   0        0        0      148 2023-11-02 16:16:50.948534 langchain_rag-0.2.0/langchain_rag/vectorstores/__init__.py
+-rw-r--r--   0        0        0    36578 2024-05-16 08:18:29.515150 langchain_rag-0.2.0/langchain_rag/vectorstores/rag_vectorstore.py
+-rw-r--r--   0        0        0     6658 2024-01-24 07:30:49.265495 langchain_rag-0.2.0/langchain_rag/vectorstores/wrapper_vectorstore.py
+-rw-r--r--   0        0        0     3812 2024-05-21 10:15:26.041841 langchain_rag-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2989 1970-01-01 00:00:00.000000 langchain_rag-0.2.0/PKG-INFO
```

### Comparing `langchain_rag-0.1.52/LICENSE.txt` & `langchain_rag-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `langchain_rag-0.1.52/README.md` & `langchain_rag-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `langchain_rag-0.1.52/langchain_rag/document_transformers/__init__.py` & `langchain_rag-0.2.0/langchain_rag/document_transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_rag-0.1.52/langchain_rag/document_transformers/copy_transformer.py` & `langchain_rag-0.2.0/langchain_rag/document_transformers/copy_transformer.py`

 * *Files identical despite different names*

### Comparing `langchain_rag-0.1.52/langchain_rag/document_transformers/document_transform_pipeline.py` & `langchain_rag-0.2.0/langchain_rag/document_transformers/document_transform_pipeline.py`

 * *Files identical despite different names*

### Comparing `langchain_rag-0.1.52/langchain_rag/document_transformers/document_transformers.py` & `langchain_rag-0.2.0/langchain_rag/document_transformers/document_transformers.py`

 * *Files identical despite different names*

### Comparing `langchain_rag-0.1.52/langchain_rag/document_transformers/generate_questions.py` & `langchain_rag-0.2.0/langchain_rag/document_transformers/generate_questions.py`

 * *Files identical despite different names*

### Comparing `langchain_rag-0.1.52/langchain_rag/document_transformers/runnable_document_transformer.py` & `langchain_rag-0.2.0/langchain_rag/document_transformers/runnable_document_transformer.py`

 * *Files identical despite different names*

### Comparing `langchain_rag-0.1.52/langchain_rag/document_transformers/summarize_and_questions_transformer.py` & `langchain_rag-0.2.0/langchain_rag/document_transformers/summarize_and_questions_transformer.py`

 * *Files identical despite different names*

### Comparing `langchain_rag-0.1.52/langchain_rag/document_transformers/summarize_transformer.py` & `langchain_rag-0.2.0/langchain_rag/document_transformers/summarize_transformer.py`

 * *Files identical despite different names*

### Comparing `langchain_rag-0.1.52/langchain_rag/indexes/memory_recordmanager.py` & `langchain_rag-0.2.0/langchain_rag/indexes/memory_recordmanager.py`

 * *Files identical despite different names*

### Comparing `langchain_rag-0.1.52/langchain_rag/patch_langchain_community/indexes/_sql_record_manager.py` & `langchain_rag-0.2.0/langchain_rag/patch_langchain_community/indexes/_sql_record_manager.py`

 * *Files identical despite different names*

### Comparing `langchain_rag-0.1.52/langchain_rag/storage/sql_docstore.py` & `langchain_rag-0.2.0/langchain_rag/storage/sql_docstore.py`

 * *Files identical despite different names*

### Comparing `langchain_rag-0.1.52/langchain_rag/vectorstores/rag_vectorstore.py` & `langchain_rag-0.2.0/langchain_rag/vectorstores/rag_vectorstore.py`

 * *Files identical despite different names*

### Comparing `langchain_rag-0.1.52/langchain_rag/vectorstores/wrapper_vectorstore.py` & `langchain_rag-0.2.0/langchain_rag/vectorstores/wrapper_vectorstore.py`

 * *Files identical despite different names*

### Comparing `langchain_rag-0.1.52/pyproject.toml` & `langchain_rag-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 packages = [
   { include = "langchain_rag" },
 ]
 
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
-#langchain-core = ">=0.1.52"
-#langchain-community = ">=0.0.38"
-langchain = "^0.1.20"
+langchain-core = ">=0.2.0"
+langchain-community = ">=0.2.0"
+#langchain = "^0.2.0"
 
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 playwright = "^1.28.0"
@@ -45,15 +45,15 @@
 pytest-socket = "^0.6.0"
 syrupy = "^4.0.2"
 wikipedia = '*'
 chromadb = "^0.4.10"
 aiosqlite = "*"
 pgvector = "*"
 psycopg2-binary = "*"
-langchain_openai = "^0.0.5"
+langchain_openai = "^0.1.7"
 #langchain-qa_with_references = { path = "../langchain-qa_with_references", develop = true }
 #langchain-qa_with_references = "^0.0.330"
 faiss-cpu = {version = "^1"}
 lark = "^1.1"
 
 [tool.poetry.group.lint]
 optional = true
```

### Comparing `langchain_rag-0.1.52/PKG-INFO` & `langchain_rag-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: langchain-rag
-Version: 0.1.52
+Version: 0.2.0
 Summary: This is a temporary project while I wait for my langchain [pull-request](https://github.com/langchain-ai/langchain/pull/7278) to be validated.
 Home-page: https://www.github.com/pprados/langchain-rag
 License: Apache 2.0
 Author: Philippe PRADOS
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: langchain (>=0.1.20,<0.2.0)
+Requires-Dist: langchain-community (>=0.2.0)
+Requires-Dist: langchain-core (>=0.2.0)
 Project-URL: Repository, https://www.github.com/pprados/langchain-rag
 Description-Content-Type: text/markdown
 
 Langchain-RAG
 =============
 
 [![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://codespaces.new/pprados/langchain-rag?quickstart=1)
```

