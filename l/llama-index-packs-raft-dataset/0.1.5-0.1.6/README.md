# Comparing `tmp/llama_index_packs_raft_dataset-0.1.5.tar.gz` & `tmp/llama_index_packs_raft_dataset-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_packs_raft_dataset-0.1.5.tar", max compression
+gzip compressed data, was "llama_index_packs_raft_dataset-0.1.6.tar", max compression
```

## Comparing `llama_index_packs_raft_dataset-0.1.5.tar` & `llama_index_packs_raft_dataset-0.1.6.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     2896 2024-05-07 16:26:09.151053 llama_index_packs_raft_dataset-0.1.5/README.md
--rw-r--r--   0        0        0       95 2024-05-07 16:26:09.151053 llama_index_packs_raft_dataset-0.1.5/llama_index/packs/raft_dataset/__init__.py
--rw-r--r--   0        0        0     8483 2024-05-07 16:26:09.151053 llama_index_packs_raft_dataset-0.1.5/llama_index/packs/raft_dataset/base.py
--rw-r--r--   0        0        0     1567 2024-05-07 16:26:09.151053 llama_index_packs_raft_dataset-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     3578 1970-01-01 00:00:00.000000 llama_index_packs_raft_dataset-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     2896 2024-05-20 20:05:28.319845 llama_index_packs_raft_dataset-0.1.6/README.md
+-rw-r--r--   0        0        0       95 2024-05-20 20:05:28.319845 llama_index_packs_raft_dataset-0.1.6/llama_index/packs/raft_dataset/__init__.py
+-rw-r--r--   0        0        0     8785 2024-05-20 20:05:28.319845 llama_index_packs_raft_dataset-0.1.6/llama_index/packs/raft_dataset/base.py
+-rw-r--r--   0        0        0     1567 2024-05-20 20:05:28.319845 llama_index_packs_raft_dataset-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     3578 1970-01-01 00:00:00.000000 llama_index_packs_raft_dataset-0.1.6/PKG-INFO
```

### Comparing `llama_index_packs_raft_dataset-0.1.5/README.md` & `llama_index_packs_raft_dataset-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_packs_raft_dataset-0.1.5/llama_index/packs/raft_dataset/base.py` & `llama_index_packs_raft_dataset-0.1.6/llama_index/packs/raft_dataset/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """RAFT Dataset LlamaPack class."""
 
 # Inspired from https://github.com/ShishirPatil/gorilla/tree/main/raft
 
 from typing import Any, List
 import random
 import logging
+import warnings
+
 from datasets import Dataset
 
 # Configure logging to output to the console, with messages of level DEBUG and above
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.INFO)
 
 from llama_index.core.llama_pack.base import BaseLlamaPack
@@ -104,16 +106,25 @@
                 content="You are a synthetic question-answer pair generator. Given a chunk of context about some topic(s), generate %s example questions a user could ask and would be answered using information from the chunk. For example, if the given context was a Wikipedia paragraph about the United States, an example question could be 'How many states are in the United States?'. The questions should be able to be answered in a few words or less."
                 % (x),
             ),
             ChatMessage(role="user", content=str(chunk)),
         ]
 
         queries = str(self.llm.chat(messages)).split("\n")
-        queries = [self.strip_str(q) for q in queries]
-        return [q for q in queries if any(c.isalpha() for c in q)]
+        questions = [self.strip_str(q) for q in queries]
+        questions = [q for q in questions if any(c.isalpha() for c in q)][:x]
+
+        num_questions_generated = len(questions)
+        if num_questions_generated < x:
+            warnings.warn(
+                f"Fewer questions generated ({num_questions_generated}) "
+                f"than requested ({x})."
+            )
+
+        return questions
 
     def get_chunks(self, file_path: str, chunk_size: int) -> List[str]:
         """
         Takes in a `file_path`, retrieves the document, breaks it down into chunks of size
         `chunk_size`, and returns the chunks.
         """
         documents = SimpleDirectoryReader(input_files=[file_path]).load_data()
```

### Comparing `llama_index_packs_raft_dataset-0.1.5/pyproject.toml` & `llama_index_packs_raft_dataset-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 description = "llama-index packs RAFT Dataset paper implementation"
 exclude = ["**/BUILD"]
 keywords = ["finetuning", "raft", "raft_dataset"]
 license = "MIT"
 maintainers = ["ravi-theja"]
 name = "llama-index-packs-raft-dataset"
 readme = "README.md"
-version = "0.1.5"
+version = "0.1.6"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.0"
 datasets = "^2.18.0"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `llama_index_packs_raft_dataset-0.1.5/PKG-INFO` & `llama_index_packs_raft_dataset-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-packs-raft-dataset
-Version: 0.1.5
+Version: 0.1.6
 Summary: llama-index packs RAFT Dataset paper implementation
 License: MIT
 Keywords: finetuning,raft,raft_dataset
 Author: Ravi Theja
 Author-email: ravi03071991@gmail.com
 Maintainer: ravi-theja
 Requires-Python: >=3.8.1,<4.0
```

