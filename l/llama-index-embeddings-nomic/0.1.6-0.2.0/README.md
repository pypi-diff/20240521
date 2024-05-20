# Comparing `tmp/llama_index_embeddings_nomic-0.1.6.tar.gz` & `tmp/llama_index_embeddings_nomic-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_embeddings_nomic-0.1.6.tar", max compression
+gzip compressed data, was "llama_index_embeddings_nomic-0.2.0.tar", max compression
```

## Comparing `llama_index_embeddings_nomic-0.1.6.tar` & `llama_index_embeddings_nomic-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       43 2024-02-13 13:53:01.627345 llama_index_embeddings_nomic-0.1.6/README.md
--rw-r--r--   0        0        0       91 2024-02-13 13:53:01.627563 llama_index_embeddings_nomic-0.1.6/llama_index/embeddings/nomic/__init__.py
--rw-r--r--   0        0        0     7986 2024-02-15 22:48:07.062575 llama_index_embeddings_nomic-0.1.6/llama_index/embeddings/nomic/base.py
--rw-r--r--   0        0        0     1533 2024-02-21 16:58:34.818255 llama_index_embeddings_nomic-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      803 1970-01-01 00:00:00.000000 llama_index_embeddings_nomic-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0       43 2024-05-20 22:04:13.052951 llama_index_embeddings_nomic-0.2.0/README.md
+-rw-r--r--   0        0        0       91 2024-05-20 22:04:13.052951 llama_index_embeddings_nomic-0.2.0/llama_index/embeddings/nomic/__init__.py
+-rw-r--r--   0        0        0     7445 2024-05-20 22:04:13.052951 llama_index_embeddings_nomic-0.2.0/llama_index/embeddings/nomic/base.py
+-rw-r--r--   0        0        0     1554 2024-05-20 22:04:13.052951 llama_index_embeddings_nomic-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      719 1970-01-01 00:00:00.000000 llama_index_embeddings_nomic-0.2.0/PKG-INFO
```

### Comparing `llama_index_embeddings_nomic-0.1.6/llama_index/embeddings/nomic/base.py` & `llama_index_embeddings_nomic-0.2.0/llama_index/embeddings/nomic/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,132 +1,121 @@
 from enum import Enum
 from typing import Any, List, Optional, Union
 
+import nomic
+import nomic.embed
+import torch
 from llama_index.core.base.embeddings.base import (
     BaseEmbedding,
     DEFAULT_EMBED_BATCH_SIZE,
 )
 from llama_index.core.bridge.pydantic import Field, PrivateAttr
 from llama_index.core.callbacks import CallbackManager
-
 from llama_index.embeddings.huggingface import HuggingFaceEmbedding
-
-from llama_index.core.bridge.pydantic import Field, PrivateAttr
 from llama_index.embeddings.huggingface.pooling import Pooling
-import torch
-import logging
 
 DEFAULT_HUGGINGFACE_LENGTH = 512
-logger = logging.getLogger(__name__)
 
 
-class NomicAITaskType(str, Enum):
+class NomicTaskType(str, Enum):
     SEARCH_QUERY = "search_query"
     SEARCH_DOCUMENT = "search_document"
     CLUSTERING = "clustering"
     CLASSIFICATION = "classification"
 
 
-TASK_TYPES = [
-    NomicAITaskType.SEARCH_QUERY,
-    NomicAITaskType.SEARCH_DOCUMENT,
-    NomicAITaskType.CLUSTERING,
-    NomicAITaskType.CLASSIFICATION,
-]
+class NomicInferenceMode(str, Enum):
+    REMOTE = "remote"
+    LOCAL = "local"
+    DYNAMIC = "dynamic"
 
 
 class NomicEmbedding(BaseEmbedding):
     """NomicEmbedding uses the Nomic API to generate embeddings."""
 
-    # Instance variables initialized via Pydantic's mechanism
-    query_task_type: Optional[str] = Field(description="Query Embedding prefix")
-    document_task_type: Optional[str] = Field(description="Document Embedding prefix")
-    dimensionality: Optional[int] = Field(description="Dimension of the Embedding")
+    query_task_type: Optional[NomicTaskType] = Field(
+        description="Task type for queries",
+    )
+    document_task_type: Optional[NomicTaskType] = Field(
+        description="Task type for documents",
+    )
+    dimensionality: Optional[int] = Field(
+        description="Embedding dimension, for use with Matryoshka-capable models",
+    )
     model_name: str = Field(description="Embedding model name")
-    _model: Any = PrivateAttr()
+    inference_mode: NomicInferenceMode = Field(
+        description="Whether to generate embeddings locally",
+    )
+    device: Optional[str] = Field(description="Device to use for local embeddings")
 
     def __init__(
         self,
         model_name: str = "nomic-embed-text-v1",
         embed_batch_size: int = 32,
         api_key: Optional[str] = None,
         callback_manager: Optional[CallbackManager] = None,
         query_task_type: Optional[str] = "search_query",
         document_task_type: Optional[str] = "search_document",
         dimensionality: Optional[int] = 768,
-        **kwargs: Any,
-    ) -> None:
-        if query_task_type not in TASK_TYPES or document_task_type not in TASK_TYPES:
-            raise ValueError(
-                f"Invalid task type {query_task_type}, {document_task_type}. Must be one of {TASK_TYPES}"
-            )
-
-        try:
-            import nomic
-            from nomic import embed
-        except ImportError:
-            raise ImportError(
-                "NomicEmbedding requires the 'nomic' package to be installed.\n"
-                "Please install it with `pip install nomic`."
-            )
-
+        inference_mode: str = "remote",
+        device: Optional[str] = None,
+    ):
         if api_key is not None:
-            nomic.cli.login(api_key)
+            nomic.login(api_key)
+
         super().__init__(
             model_name=model_name,
             embed_batch_size=embed_batch_size,
             callback_manager=callback_manager,
-            _model=embed,
             query_task_type=query_task_type,
             document_task_type=document_task_type,
             dimensionality=dimensionality,
-            **kwargs,
+            inference_mode=inference_mode,
+            device=device,
         )
-        self._model = embed
-        self.model_name = model_name
-        self.query_task_type = query_task_type
-        self.document_task_type = document_task_type
-        self.dimensionality = dimensionality
 
     @classmethod
     def class_name(cls) -> str:
         return "NomicEmbedding"
 
     def _embed(
         self, texts: List[str], task_type: Optional[str] = None
     ) -> List[List[float]]:
-        """Embed sentences using NomicAI."""
-        result = self._model.text(
+        result = nomic.embed.text(
             texts,
             model=self.model_name,
             task_type=task_type,
             dimensionality=self.dimensionality,
+            inference_mode=self.inference_mode,
+            device=self.device,
         )
         return result["embeddings"]
 
     def _get_query_embedding(self, query: str) -> List[float]:
-        """Get query embedding."""
         return self._embed([query], task_type=self.query_task_type)[0]
 
     async def _aget_query_embedding(self, query: str) -> List[float]:
-        """Get query embedding async."""
+        self._warn_async()
         return self._get_query_embedding(query)
 
     def _get_text_embedding(self, text: str) -> List[float]:
-        """Get text embedding."""
         return self._embed([text], task_type=self.document_task_type)[0]
 
     async def _aget_text_embedding(self, text: str) -> List[float]:
-        """Get text embedding async."""
+        self._warn_async()
         return self._get_text_embedding(text)
 
     def _get_text_embeddings(self, texts: List[str]) -> List[List[float]]:
-        """Get text embeddings."""
         return self._embed(texts, task_type=self.document_task_type)
 
+    def _warn_async() -> None:
+        warnings.warn(
+            f"{self.class_name()} does not implement async embeddings, falling back to sync method.",
+        )
+
 
 class NomicHFEmbedding(HuggingFaceEmbedding):
     tokenizer_name: str = Field(description="Tokenizer name from HuggingFace.")
     max_length: int = Field(
         default=DEFAULT_HUGGINGFACE_LENGTH, description="Maximum length of input.", gt=0
     )
     pooling: Pooling = Field(default=Pooling.MEAN, description="Pooling strategy.")
```

### Comparing `llama_index_embeddings_nomic-0.1.6/pyproject.toml` & `llama_index_embeddings_nomic-0.2.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -17,28 +17,27 @@
 [tool.mypy]
 disallow_untyped_defs = true
 exclude = ["_static", "build", "examples", "notebooks", "venv"]
 ignore_missing_imports = true
 python_version = "3.8"
 
 [tool.poetry]
-authors = ["Your Name <you@example.com>"]
+authors = ["Jared Van Bortel <jared@nomic.ai>", "Zach Nussbaum <zach@nomic.ai>"]
 description = "llama-index embeddings nomic integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-embeddings-nomic"
 readme = "README.md"
-version = "0.1.6"
+version = "0.2.0"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.11.post1"
 llama-index-embeddings-huggingface = "^0.1.3"
-einops = "^0.7.0"
-nomic = "^3.0.12"
+nomic = "^3.0.29"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "8.10.0"
 jupyter = "^1.0.0"
 mypy = "0.991"
 pre-commit = "3.2.0"
 pylint = "2.15.10"
```

### Comparing `llama_index_embeddings_nomic-0.1.6/PKG-INFO` & `llama_index_embeddings_nomic-0.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 Metadata-Version: 2.1
 Name: llama-index-embeddings-nomic
-Version: 0.1.6
+Version: 0.2.0
 Summary: llama-index embeddings nomic integration
 License: MIT
-Author: Your Name
-Author-email: you@example.com
+Author: Jared Van Bortel
+Author-email: jared@nomic.ai
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: einops (>=0.7.0,<0.8.0)
 Requires-Dist: llama-index-core (>=0.10.11.post1,<0.11.0)
 Requires-Dist: llama-index-embeddings-huggingface (>=0.1.3,<0.2.0)
-Requires-Dist: nomic (>=3.0.12,<4.0.0)
+Requires-Dist: nomic (>=3.0.29,<4.0.0)
 Description-Content-Type: text/markdown
 
 # LlamaIndex Embeddings Integration: Nomic
```

