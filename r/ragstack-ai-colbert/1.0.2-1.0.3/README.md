# Comparing `tmp/ragstack_ai_colbert-1.0.2.tar.gz` & `tmp/ragstack_ai_colbert-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ragstack_ai_colbert-1.0.2.tar", max compression
+gzip compressed data, was "ragstack_ai_colbert-1.0.3.tar", max compression
```

## Comparing `ragstack_ai_colbert-1.0.2.tar` & `ragstack_ai_colbert-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      374 2024-05-13 16:14:59.192325 ragstack_ai_colbert-1.0.2/README.md
--rw-r--r--   0        0        0      596 2024-05-13 16:14:59.192325 ragstack_ai_colbert-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     1542 2024-05-13 16:14:59.192325 ragstack_ai_colbert-1.0.2/ragstack_colbert/__init__.py
--rw-r--r--   0        0        0     2470 2024-05-13 16:14:59.192325 ragstack_ai_colbert-1.0.2/ragstack_colbert/base_database.py
--rw-r--r--   0        0        0     1848 2024-05-13 16:14:59.192325 ragstack_ai_colbert-1.0.2/ragstack_colbert/base_embedding_model.py
--rw-r--r--   0        0        0     5645 2024-05-13 16:14:59.192325 ragstack_ai_colbert-1.0.2/ragstack_colbert/base_retriever.py
--rw-r--r--   0        0        0     3275 2024-05-13 16:14:59.192325 ragstack_ai_colbert-1.0.2/ragstack_colbert/base_vector_store.py
--rw-r--r--   0        0        0     8525 2024-05-13 16:14:59.192325 ragstack_ai_colbert-1.0.2/ragstack_colbert/cassandra_database.py
--rw-r--r--   0        0        0     5403 2024-05-13 16:14:59.192325 ragstack_ai_colbert-1.0.2/ragstack_colbert/colbert_embedding_model.py
--rw-r--r--   0        0        0    15736 2024-05-13 16:14:59.192325 ragstack_ai_colbert-1.0.2/ragstack_colbert/colbert_retriever.py
--rw-r--r--   0        0        0     4385 2024-05-13 16:14:59.192325 ragstack_ai_colbert-1.0.2/ragstack_colbert/colbert_vector_store.py
--rw-r--r--   0        0        0      664 2024-05-13 16:14:59.192325 ragstack_ai_colbert-1.0.2/ragstack_colbert/constant.py
--rw-r--r--   0        0        0     2178 2024-05-13 16:14:59.192325 ragstack_ai_colbert-1.0.2/ragstack_colbert/objects.py
--rw-r--r--   0        0        0     4580 2024-05-13 16:14:59.192325 ragstack_ai_colbert-1.0.2/ragstack_colbert/text_encoder.py
--rw-r--r--   0        0        0     1206 1970-01-01 00:00:00.000000 ragstack_ai_colbert-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0      374 2024-05-21 18:44:38.654207 ragstack_ai_colbert-1.0.3/README.md
+-rw-r--r--   0        0        0      662 2024-05-21 18:44:38.654207 ragstack_ai_colbert-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1542 2024-05-21 18:44:38.654207 ragstack_ai_colbert-1.0.3/ragstack_colbert/__init__.py
+-rw-r--r--   0        0        0     3531 2024-05-21 18:44:38.654207 ragstack_ai_colbert-1.0.3/ragstack_colbert/base_database.py
+-rw-r--r--   0        0        0     1848 2024-05-21 18:44:38.654207 ragstack_ai_colbert-1.0.3/ragstack_colbert/base_embedding_model.py
+-rw-r--r--   0        0        0     5645 2024-05-21 18:44:38.654207 ragstack_ai_colbert-1.0.3/ragstack_colbert/base_retriever.py
+-rw-r--r--   0        0        0     5436 2024-05-21 18:44:38.654207 ragstack_ai_colbert-1.0.3/ragstack_colbert/base_vector_store.py
+-rw-r--r--   0        0        0    14323 2024-05-21 18:44:38.654207 ragstack_ai_colbert-1.0.3/ragstack_colbert/cassandra_database.py
+-rw-r--r--   0        0        0     5403 2024-05-21 18:44:38.654207 ragstack_ai_colbert-1.0.3/ragstack_colbert/colbert_embedding_model.py
+-rw-r--r--   0        0        0    15736 2024-05-21 18:44:38.654207 ragstack_ai_colbert-1.0.3/ragstack_colbert/colbert_retriever.py
+-rw-r--r--   0        0        0     7252 2024-05-21 18:44:38.654207 ragstack_ai_colbert-1.0.3/ragstack_colbert/colbert_vector_store.py
+-rw-r--r--   0        0        0      664 2024-05-21 18:44:38.654207 ragstack_ai_colbert-1.0.3/ragstack_colbert/constant.py
+-rw-r--r--   0        0        0     2178 2024-05-21 18:44:38.654207 ragstack_ai_colbert-1.0.3/ragstack_colbert/objects.py
+-rw-r--r--   0        0        0     4579 2024-05-21 18:44:38.654207 ragstack_ai_colbert-1.0.3/ragstack_colbert/text_encoder.py
+-rw-r--r--   0        0        0     1206 1970-01-01 00:00:00.000000 ragstack_ai_colbert-1.0.3/PKG-INFO
```

### Comparing `ragstack_ai_colbert-1.0.2/pyproject.toml` & `ragstack_ai_colbert-1.0.3/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ragstack-ai-colbert"
-version = "1.0.2"
+version = "1.0.3"
 description = "DataStax RAGStack Colbert implementation"
 license = "BUSL-1.1"
 authors = ["DataStax"]
 readme = "README.md"
 repository = "https://github.com/datastax/ragstack-ai"
 documentation = "https://docs.datastax.com/en/ragstack"
 packages = [{ include = "ragstack_colbert" }]
@@ -16,7 +16,11 @@
 torch = "2.2.1"
 cassio = "~0.1.7"
 pydantic = "^2.7.1"
 
 [tool.poetry.group.test.dependencies]
 ragstack-ai-tests-utils = { path = "../tests-utils", develop = true }
 
+
+[tool.poetry.group.dev.dependencies]
+pytest-asyncio = "^0.23.6"
+
```

### Comparing `ragstack_ai_colbert-1.0.2/ragstack_colbert/__init__.py` & `ragstack_ai_colbert-1.0.3/ragstack_colbert/__init__.py`

 * *Files identical despite different names*

### Comparing `ragstack_ai_colbert-1.0.2/ragstack_colbert/base_database.py` & `ragstack_ai_colbert-1.0.3/ragstack_colbert/base_database.py`

 * *Files 21% similar despite different names*

```diff
@@ -35,15 +35,41 @@
         """
         Deletes chunks from the vector store based on their document id.
 
         Parameters:
             doc_ids (List[str]): A list of document identifiers specifying the chunks to be deleted.
 
         Returns:
-            True if the delete was successful.
+            True if the all the deletes were successful.
+        """
+
+    @abstractmethod
+    async def aadd_chunks(self, chunks: List[Chunk], concurrent_inserts: Optional[int] = 100) -> List[Tuple[str, int]]:
+        """
+        Stores a list of embedded text chunks in the vector store
+
+        Parameters:
+            chunks (List[Chunk]): A list of `Chunk` instances to be stored.
+            concurrent_inserts (Optional[int]): How many concurrent inserts to make to the database. Defaults to 100.
+
+        Returns:
+            a list of tuples: (doc_id, chunk_id)
+        """
+
+    @abstractmethod
+    async def adelete_chunks(self, doc_ids: List[str], concurrent_deletes: Optional[int] = 100) -> bool:
+        """
+        Deletes chunks from the vector store based on their document id.
+
+        Parameters:
+            doc_ids (List[str]): A list of document identifiers specifying the chunks to be deleted.
+            concurrent_deletes (Optional[int]): How many concurrent deletes to make to the database. Defaults to 100.
+
+        Returns:
+            True if the all the deletes were successful.
         """
 
     @abstractmethod
     async def search_relevant_chunks(self, vector: Vector, n: int) -> List[Chunk]:
         """
         Retrieves 'n' ANN results for an embedded token vector.
```

### Comparing `ragstack_ai_colbert-1.0.2/ragstack_colbert/base_embedding_model.py` & `ragstack_ai_colbert-1.0.3/ragstack_colbert/base_embedding_model.py`

 * *Files identical despite different names*

### Comparing `ragstack_ai_colbert-1.0.2/ragstack_colbert/base_retriever.py` & `ragstack_ai_colbert-1.0.3/ragstack_colbert/base_retriever.py`

 * *Files identical despite different names*

### Comparing `ragstack_ai_colbert-1.0.2/ragstack_colbert/base_vector_store.py` & `ragstack_ai_colbert-1.0.3/ragstack_colbert/base_vector_store.py`

 * *Files 26% similar despite different names*

```diff
@@ -72,15 +72,68 @@
         """
         Deletes chunks from the vector store based on their document id.
 
         Parameters:
             doc_ids (List[str]): A list of document identifiers specifying the chunks to be deleted.
 
         Returns:
-            True if the delete was successful.
+            True if the all the deletes were successful.
+        """
+
+        # handles LlamaIndex add
+
+    @abstractmethod
+    async def aadd_chunks(self, chunks: List[Chunk], concurrent_inserts: Optional[int] = 100) -> List[Tuple[str, int]]:
+        """
+        Stores a list of embedded text chunks in the vector store
+
+        Parameters:
+            chunks (List[Chunk]): A list of `Chunk` instances to be stored.
+            concurrent_inserts (Optional[int]): How many concurrent inserts to make to the database. Defaults to 100.
+
+        Returns:
+            a list of tuples: (doc_id, chunk_id)
+        """
+
+    # handles LangChain add
+    @abstractmethod
+    async def aadd_texts(
+        self,
+        texts: List[str],
+        metadatas: Optional[List[Metadata]],
+        doc_id: Optional[str] = None,
+        concurrent_inserts: Optional[int] = 100,
+    ) -> List[Tuple[str, int]]:
+        """
+        Embeds and stores a list of text chunks and optional metadata into the vector store
+
+        Parameters:
+            texts (List[str]): The list of text chunks to be embedded
+            metadatas (Optional[List[Metadata]])): An optional list of Metadata to be stored.
+                                                   If provided, these are set 1 to 1 with the texts list.
+            doc_id (Optional[str]): The document id associated with the texts. If not provided,
+                                    it is generated.
+            concurrent_inserts (Optional[int]): How many concurrent inserts to make to the database. Defaults to 100.
+
+        Returns:
+            a list of tuples: (doc_id, chunk_id)
+        """
+
+    # handles LangChain and LlamaIndex delete
+    @abstractmethod
+    async def adelete_chunks(self, doc_ids: List[str], concurrent_deletes: Optional[int] = 100) -> bool:
+        """
+        Deletes chunks from the vector store based on their document id.
+
+        Parameters:
+            doc_ids (List[str]): A list of document identifiers specifying the chunks to be deleted.
+            concurrent_deletes (Optional[int]): How many concurrent deletes to make to the database. Defaults to 100.
+
+        Returns:
+            True if the all the deletes were successful.
         """
 
     # handles LangChain as_retriever
     @abstractmethod
     def as_retriever(self) -> BaseRetriever:
         """
         Gets a retriever using the vector store.
```

### Comparing `ragstack_ai_colbert-1.0.2/ragstack_colbert/colbert_embedding_model.py` & `ragstack_ai_colbert-1.0.3/ragstack_colbert/colbert_embedding_model.py`

 * *Files identical despite different names*

### Comparing `ragstack_ai_colbert-1.0.2/ragstack_colbert/colbert_retriever.py` & `ragstack_ai_colbert-1.0.3/ragstack_colbert/colbert_retriever.py`

 * *Files identical despite different names*

### Comparing `ragstack_ai_colbert-1.0.2/ragstack_colbert/colbert_vector_store.py` & `ragstack_ai_colbert-1.0.3/ragstack_colbert/colbert_vector_store.py`

 * *Files 27% similar despite different names*

```diff
@@ -42,14 +42,44 @@
 
     def _validate_embedding_model(self):
         if self._embedding_model is None:
             raise AttributeError(
                 "To use this method, `embedding_model` must be set on class creation."
             )
 
+    def _build_chunks(
+        self,
+        texts: List[str],
+        metadatas: Optional[List[Metadata]] = None,
+        doc_id: Optional[str] = None,
+    ) -> List[Chunk]:
+
+        self._validate_embedding_model()
+
+        if metadatas is not None and len(texts) != len(metadatas):
+            raise ValueError("Length of texts and metadatas must match.")
+
+        if doc_id is None:
+            doc_id = str(uuid.uuid4())
+
+        embeddings = self._embedding_model.embed_texts(texts=texts)
+
+        chunks: List[Chunk] = []
+        for i, text in enumerate(texts):
+            chunks.append(
+                Chunk(
+                    doc_id=doc_id,
+                    chunk_id=i,
+                    text=text,
+                    metadata={} if metadatas is None else metadatas[i],
+                    embedding=embeddings[i],
+                )
+            )
+        return chunks
+
     # implements the abc method to handle LlamaIndex add
     def add_chunks(self, chunks: List[Chunk]) -> List[Tuple[str, int]]:
         """
         Stores a list of embedded text chunks in the vector store
 
         Parameters:
             chunks (List[Chunk]): A list of `Chunk` instances to be stored.
@@ -76,51 +106,84 @@
                                                    If provided, these are set 1 to 1 with the texts list.
             doc_id (Optional[str]): The document id associated with the texts. If not provided,
                                     it is generated.
 
         Returns:
             a list of tuples: (doc_id, chunk_id)
         """
-        self._validate_embedding_model()
+        chunks = self._build_chunks(texts=texts, metadatas=metadatas, doc_id=doc_id)
+        return self._database.add_chunks(chunks=chunks)
 
-        if metadatas is not None and len(texts) != len(metadatas):
-            raise ValueError("Length of texts and metadatas must match.")
+    # implements the abc method to handle LangChain and LlamaIndex delete
+    def delete_chunks(self, doc_ids: List[str]) -> bool:
+        """
+        Deletes chunks from the vector store based on their document id.
 
-        if doc_id is None:
-            doc_id = str(uuid.uuid4())
+        Parameters:
+            doc_ids (List[str]): A list of document identifiers specifying the chunks to be deleted.
 
-        embeddings = self._embedding_model.embed_texts(texts=texts)
+        Returns:
+            True if the all the deletes were successful.
+        """
 
-        chunks: List[Chunk] = []
-        for i, text in enumerate(texts):
-            chunks.append(
-                Chunk(
-                    doc_id=doc_id,
-                    chunk_id=i,
-                    text=text,
-                    metadata={} if metadatas is None else metadatas[i],
-                    embedding=embeddings[i],
-                )
-            )
+        return self._database.delete_chunks(doc_ids=doc_ids)
 
-        return self._database.add_chunks(chunks=chunks)
+    # implements the abc method to handle LlamaIndex add
+    async def aadd_chunks(self, chunks: List[Chunk], concurrent_inserts: Optional[int] = 100) -> List[Tuple[str, int]]:
+        """
+        Stores a list of embedded text chunks in the vector store
+
+        Parameters:
+            chunks (List[Chunk]): A list of `Chunk` instances to be stored.
+            concurrent_inserts (Optional[int]): How many concurrent inserts to make to the database. Defaults to 100.
+
+        Returns:
+            a list of tuples: (doc_id, chunk_id)
+        """
+
+        return await self._database.aadd_chunks(chunks=chunks, concurrent_inserts=concurrent_inserts)
+
+    # implements the abc method to handle LangChain add
+    async def aadd_texts(
+        self,
+        texts: List[str],
+        metadatas: Optional[List[Metadata]] = None,
+        doc_id: Optional[str] = None,
+        concurrent_inserts: Optional[int] = 100,
+    ) -> List[Tuple[str, int]]:
+        """
+        Embeds and stores a list of text chunks and optional metadata into the vector store
+
+        Parameters:
+            texts (List[str]): The list of text chunks to be embedded
+            metadatas (Optional[List[Metadata]])): An optional list of Metadata to be stored.
+                                                   If provided, these are set 1 to 1 with the texts list.
+            doc_id (Optional[str]): The document id associated with the texts. If not provided,
+                                    it is generated.
+            concurrent_inserts (Optional[int]): How many concurrent inserts to make to the database. Defaults to 100.
+
+        Returns:
+            a list of tuples: (doc_id, chunk_id)
+        """
+        chunks = self._build_chunks(texts=texts, metadatas=metadatas, doc_id=doc_id)
+        return await self._database.aadd_chunks(chunks=chunks, concurrent_inserts=concurrent_inserts)
 
     # implements the abc method to handle LangChain and LlamaIndex delete
-    def delete_chunks(self, doc_ids: List[str]) -> bool:
+    async def adelete_chunks(self, doc_ids: List[str], concurrent_deletes: Optional[int] = 100) -> bool:
         """
         Deletes chunks from the vector store based on their document id.
 
         Parameters:
             doc_ids (List[str]): A list of document identifiers specifying the chunks to be deleted.
+            concurrent_deletes (Optional[int]): How many concurrent deletes to make to the database. Defaults to 100.
 
         Returns:
-            True if the delete was successful.
+            True if the all the deletes were successful.
         """
-
-        return self._database.delete_chunks(doc_ids=doc_ids)
+        return await self._database.adelete_chunks(doc_ids=doc_ids, concurrent_deletes=concurrent_deletes)
 
     def as_retriever(self) -> BaseRetriever:
         """
         Gets a retriever using the vector store.
         """
 
         self._validate_embedding_model()
```

### Comparing `ragstack_ai_colbert-1.0.2/ragstack_colbert/constant.py` & `ragstack_ai_colbert-1.0.3/ragstack_colbert/constant.py`

 * *Files identical despite different names*

### Comparing `ragstack_ai_colbert-1.0.2/ragstack_colbert/objects.py` & `ragstack_ai_colbert-1.0.3/ragstack_colbert/objects.py`

 * *Files identical despite different names*

### Comparing `ragstack_ai_colbert-1.0.2/ragstack_colbert/text_encoder.py` & `ragstack_ai_colbert-1.0.3/ragstack_colbert/text_encoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 dense embeddings are used to measure the semantic similarity between text chunks.
 """
 
 import logging
 from typing import List, Optional
 
 import torch
-
 from colbert.infra import ColBERTConfig
 from colbert.modeling.checkpoint import Checkpoint
 
 from .objects import Chunk, Embedding
 
 
 def calculate_query_maxlen(tokens: List[List[str]]) -> int:
```

### Comparing `ragstack_ai_colbert-1.0.2/PKG-INFO` & `ragstack_ai_colbert-1.0.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ragstack-ai-colbert
-Version: 1.0.2
+Version: 1.0.3
 Summary: DataStax RAGStack Colbert implementation
 Home-page: https://github.com/datastax/ragstack-ai
 License: BUSL-1.1
 Author: DataStax
 Requires-Python: >=3.9,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

