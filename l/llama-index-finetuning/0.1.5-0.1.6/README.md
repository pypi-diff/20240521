# Comparing `tmp/llama_index_finetuning-0.1.5.tar.gz` & `tmp/llama_index_finetuning-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_finetuning-0.1.5.tar", max compression
+gzip compressed data, was "llama_index_finetuning-0.1.6.tar", max compression
```

## Comparing `llama_index_finetuning-0.1.5.tar` & `llama_index_finetuning-0.1.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      156 2024-04-04 22:08:09.061314 llama_index_finetuning-0.1.5/README.md
--rw-r--r--   0        0        0     1012 2024-04-04 22:08:09.065314 llama_index_finetuning-0.1.5/llama_index/finetuning/__init__.py
--rw-r--r--   0        0        0      188 2024-04-04 22:08:09.065314 llama_index_finetuning-0.1.5/llama_index/finetuning/callbacks/__init__.py
--rw-r--r--   0        0        0     7574 2024-04-04 22:08:09.065314 llama_index_finetuning-0.1.5/llama_index/finetuning/callbacks/finetuning_handler.py
--rw-r--r--   0        0        0      161 2024-04-04 22:08:09.065314 llama_index_finetuning-0.1.5/llama_index/finetuning/cross_encoders/__init__.py
--rw-r--r--   0        0        0     4797 2024-04-04 22:08:09.065314 llama_index_finetuning-0.1.5/llama_index/finetuning/cross_encoders/cross_encoder.py
--rw-r--r--   0        0        0     9431 2024-04-04 22:08:09.065314 llama_index_finetuning-0.1.5/llama_index/finetuning/cross_encoders/dataset_gen.py
--rw-r--r--   0        0        0      299 2024-04-04 22:08:09.065314 llama_index_finetuning-0.1.5/llama_index/finetuning/embeddings/__init__.py
--rw-r--r--   0        0        0     6400 2024-04-04 22:08:09.065314 llama_index_finetuning-0.1.5/llama_index/finetuning/embeddings/adapter.py
--rw-r--r--   0        0        0     5008 2024-04-04 22:08:09.065314 llama_index_finetuning-0.1.5/llama_index/finetuning/embeddings/adapter_utils.py
--rw-r--r--   0        0        0     3126 2024-04-04 22:08:09.065314 llama_index_finetuning-0.1.5/llama_index/finetuning/embeddings/common.py
--rw-r--r--   0        0        0     3353 2024-04-04 22:08:09.065314 llama_index_finetuning-0.1.5/llama_index/finetuning/embeddings/sentence_transformer.py
--rw-r--r--   0        0        0      110 2024-04-04 22:08:09.065314 llama_index_finetuning-0.1.5/llama_index/finetuning/gradient/__init__.py
--rw-r--r--   0        0        0     4946 2024-04-04 22:08:09.065314 llama_index_finetuning-0.1.5/llama_index/finetuning/gradient/base.py
--rw-r--r--   0        0        0      123 2024-04-04 22:08:09.065314 llama_index_finetuning-0.1.5/llama_index/finetuning/openai/__init__.py
--rw-r--r--   0        0        0     3880 2024-04-04 22:08:09.065314 llama_index_finetuning-0.1.5/llama_index/finetuning/openai/base.py
--rw-r--r--   0        0        0     6562 2024-04-04 22:08:09.065314 llama_index_finetuning-0.1.5/llama_index/finetuning/openai/validate_json.py
--rw-r--r--   0        0        0      282 2024-04-04 22:08:09.065314 llama_index_finetuning-0.1.5/llama_index/finetuning/rerankers/__init__.py
--rw-r--r--   0        0        0     2753 2024-04-04 22:08:09.065314 llama_index_finetuning-0.1.5/llama_index/finetuning/rerankers/cohere_reranker.py
--rw-r--r--   0        0        0     4700 2024-04-04 22:08:09.065314 llama_index_finetuning-0.1.5/llama_index/finetuning/rerankers/dataset_gen.py
--rw-r--r--   0        0        0     1618 2024-04-04 22:08:09.065314 llama_index_finetuning-0.1.5/llama_index/finetuning/types.py
--rw-r--r--   0        0        0     1830 2024-04-04 22:08:09.065314 llama_index_finetuning-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      999 1970-01-01 00:00:00.000000 llama_index_finetuning-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      156 2024-05-20 20:05:27.871841 llama_index_finetuning-0.1.6/README.md
+-rw-r--r--   0        0        0     1012 2024-05-20 20:05:27.871841 llama_index_finetuning-0.1.6/llama_index/finetuning/__init__.py
+-rw-r--r--   0        0        0      188 2024-05-20 20:05:27.871841 llama_index_finetuning-0.1.6/llama_index/finetuning/callbacks/__init__.py
+-rw-r--r--   0        0        0     7574 2024-05-20 20:05:27.871841 llama_index_finetuning-0.1.6/llama_index/finetuning/callbacks/finetuning_handler.py
+-rw-r--r--   0        0        0      161 2024-05-20 20:05:27.871841 llama_index_finetuning-0.1.6/llama_index/finetuning/cross_encoders/__init__.py
+-rw-r--r--   0        0        0     4797 2024-05-20 20:05:27.871841 llama_index_finetuning-0.1.6/llama_index/finetuning/cross_encoders/cross_encoder.py
+-rw-r--r--   0        0        0     9821 2024-05-20 20:05:27.871841 llama_index_finetuning-0.1.6/llama_index/finetuning/cross_encoders/dataset_gen.py
+-rw-r--r--   0        0        0      299 2024-05-20 20:05:27.871841 llama_index_finetuning-0.1.6/llama_index/finetuning/embeddings/__init__.py
+-rw-r--r--   0        0        0     6400 2024-05-20 20:05:27.871841 llama_index_finetuning-0.1.6/llama_index/finetuning/embeddings/adapter.py
+-rw-r--r--   0        0        0     5008 2024-05-20 20:05:27.871841 llama_index_finetuning-0.1.6/llama_index/finetuning/embeddings/adapter_utils.py
+-rw-r--r--   0        0        0     3480 2024-05-20 20:05:27.871841 llama_index_finetuning-0.1.6/llama_index/finetuning/embeddings/common.py
+-rw-r--r--   0        0        0     3353 2024-05-20 20:05:27.875841 llama_index_finetuning-0.1.6/llama_index/finetuning/embeddings/sentence_transformer.py
+-rw-r--r--   0        0        0      110 2024-05-20 20:05:27.875841 llama_index_finetuning-0.1.6/llama_index/finetuning/gradient/__init__.py
+-rw-r--r--   0        0        0     4946 2024-05-20 20:05:27.875841 llama_index_finetuning-0.1.6/llama_index/finetuning/gradient/base.py
+-rw-r--r--   0        0        0      123 2024-05-20 20:05:27.875841 llama_index_finetuning-0.1.6/llama_index/finetuning/openai/__init__.py
+-rw-r--r--   0        0        0     3880 2024-05-20 20:05:27.875841 llama_index_finetuning-0.1.6/llama_index/finetuning/openai/base.py
+-rw-r--r--   0        0        0     6562 2024-05-20 20:05:27.875841 llama_index_finetuning-0.1.6/llama_index/finetuning/openai/validate_json.py
+-rw-r--r--   0        0        0      282 2024-05-20 20:05:27.875841 llama_index_finetuning-0.1.6/llama_index/finetuning/rerankers/__init__.py
+-rw-r--r--   0        0        0     2753 2024-05-20 20:05:27.875841 llama_index_finetuning-0.1.6/llama_index/finetuning/rerankers/cohere_reranker.py
+-rw-r--r--   0        0        0     4700 2024-05-20 20:05:27.875841 llama_index_finetuning-0.1.6/llama_index/finetuning/rerankers/dataset_gen.py
+-rw-r--r--   0        0        0     1618 2024-05-20 20:05:27.875841 llama_index_finetuning-0.1.6/llama_index/finetuning/types.py
+-rw-r--r--   0        0        0     1830 2024-05-20 20:05:27.875841 llama_index_finetuning-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      999 1970-01-01 00:00:00.000000 llama_index_finetuning-0.1.6/PKG-INFO
```

### Comparing `llama_index_finetuning-0.1.5/llama_index/finetuning/__init__.py` & `llama_index_finetuning-0.1.6/llama_index/finetuning/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index_finetuning-0.1.5/llama_index/finetuning/callbacks/finetuning_handler.py` & `llama_index_finetuning-0.1.6/llama_index/finetuning/callbacks/finetuning_handler.py`

 * *Files identical despite different names*

### Comparing `llama_index_finetuning-0.1.5/llama_index/finetuning/cross_encoders/cross_encoder.py` & `llama_index_finetuning-0.1.6/llama_index/finetuning/cross_encoders/cross_encoder.py`

 * *Files identical despite different names*

### Comparing `llama_index_finetuning-0.1.5/llama_index/finetuning/cross_encoders/dataset_gen.py` & `llama_index_finetuning-0.1.6/llama_index/finetuning/cross_encoders/dataset_gen.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Dataset Generator for Cross Encoder Finetuning."""
 import re
+import warnings
 from dataclasses import dataclass
 from typing import List, Optional
 
 from llama_index.core import VectorStoreIndex, get_tokenizer
 from llama_index.core.llms import ChatMessage
 from llama_index.core.llms.llm import LLM
 from llama_index.core.node_parser import TokenTextSplitter
@@ -68,14 +69,23 @@
             ChatMessage(role="user", content=user_msg),
         ]
         response = llm.chat(messages)
         response_content: str = (
             response.message.content if response.message.content is not None else ""
         )
         response_questions = re.split(";|\n", response_content)
+        response_questions = response_questions[:num_questions_per_chunk]
+
+        num_questions_generated = len(response_questions)
+        if num_questions_generated < num_questions_per_chunk:
+            warnings.warn(
+                f"Fewer questions generated ({num_questions_generated}) "
+                f"than requested ({num_questions_per_chunk})."
+            )
+
         questions.extend(response_questions)
 
     return questions
 
 
 # Query-Doc relevance prompt taken from OpenAI cookbook:-
 # https://github.com/openai/openai-cookbook/blob/main/examples/Search_reranking_with_cross-encoders.ipynb
```

### Comparing `llama_index_finetuning-0.1.5/llama_index/finetuning/embeddings/adapter.py` & `llama_index_finetuning-0.1.6/llama_index/finetuning/embeddings/adapter.py`

 * *Files identical despite different names*

### Comparing `llama_index_finetuning-0.1.5/llama_index/finetuning/embeddings/adapter_utils.py` & `llama_index_finetuning-0.1.6/llama_index/finetuning/embeddings/adapter_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_finetuning-0.1.5/llama_index/finetuning/embeddings/common.py` & `llama_index_finetuning-0.1.6/llama_index/finetuning/embeddings/common.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Common utils for embeddings."""
 import json
 import re
 import uuid
+import warnings
 from typing import Dict, List, Tuple
 
 from llama_index.core.bridge.pydantic import BaseModel
 from llama_index.core.llms.utils import LLM
 from llama_index.core.schema import MetadataMode, TextNode
 from tqdm import tqdm
 
@@ -85,15 +86,24 @@
         )
         response = llm.complete(query)
 
         result = str(response).strip().split("\n")
         questions = [
             re.sub(r"^\d+[\).\s]", "", question).strip() for question in result
         ]
-        questions = [question for question in questions if len(question) > 0]
+        questions = [question for question in questions if len(question) > 0][
+            :num_questions_per_chunk
+        ]
+
+        num_questions_generated = len(questions)
+        if num_questions_generated < num_questions_per_chunk:
+            warnings.warn(
+                f"Fewer questions generated ({num_questions_generated}) "
+                f"than requested ({num_questions_per_chunk})."
+            )
 
         for question in questions:
             question_id = str(uuid.uuid4())
             queries[question_id] = question
             relevant_docs[question_id] = [node_id]
 
     # construct dataset
```

### Comparing `llama_index_finetuning-0.1.5/llama_index/finetuning/embeddings/sentence_transformer.py` & `llama_index_finetuning-0.1.6/llama_index/finetuning/embeddings/sentence_transformer.py`

 * *Files identical despite different names*

### Comparing `llama_index_finetuning-0.1.5/llama_index/finetuning/gradient/base.py` & `llama_index_finetuning-0.1.6/llama_index/finetuning/gradient/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_finetuning-0.1.5/llama_index/finetuning/openai/base.py` & `llama_index_finetuning-0.1.6/llama_index/finetuning/openai/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_finetuning-0.1.5/llama_index/finetuning/openai/validate_json.py` & `llama_index_finetuning-0.1.6/llama_index/finetuning/openai/validate_json.py`

 * *Files identical despite different names*

### Comparing `llama_index_finetuning-0.1.5/llama_index/finetuning/rerankers/cohere_reranker.py` & `llama_index_finetuning-0.1.6/llama_index/finetuning/rerankers/cohere_reranker.py`

 * *Files identical despite different names*

### Comparing `llama_index_finetuning-0.1.5/llama_index/finetuning/rerankers/dataset_gen.py` & `llama_index_finetuning-0.1.6/llama_index/finetuning/rerankers/dataset_gen.py`

 * *Files identical despite different names*

### Comparing `llama_index_finetuning-0.1.5/llama_index/finetuning/types.py` & `llama_index_finetuning-0.1.6/llama_index/finetuning/types.py`

 * *Files identical despite different names*

### Comparing `llama_index_finetuning-0.1.5/pyproject.toml` & `llama_index_finetuning-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index finetuning"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-finetuning"
 readme = "README.md"
-version = "0.1.5"
+version = "0.1.6"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.11.post1"
 llama-index-llms-openai = "^0.1.1"
 llama-index-llms-gradient = "^0.1.1"
 llama-index-postprocessor-cohere-rerank = "^0.1.1"
```

### Comparing `llama_index_finetuning-0.1.5/PKG-INFO` & `llama_index_finetuning-0.1.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-finetuning
-Version: 0.1.5
+Version: 0.1.6
 Summary: llama-index finetuning
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

