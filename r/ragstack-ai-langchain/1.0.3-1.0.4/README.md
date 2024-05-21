# Comparing `tmp/ragstack_ai_langchain-1.0.3.tar.gz` & `tmp/ragstack_ai_langchain-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ragstack_ai_langchain-1.0.3.tar", max compression
+gzip compressed data, was "ragstack_ai_langchain-1.0.4.tar", max compression
```

## Comparing `ragstack_ai_langchain-1.0.3.tar` & `ragstack_ai_langchain-1.0.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      371 2024-05-13 16:30:58.004527 ragstack_ai_langchain-1.0.3/README.md
--rw-r--r--   0        0        0     1153 2024-05-13 16:30:58.004527 ragstack_ai_langchain-1.0.3/pyproject.toml
--rw-r--r--   0        0        0      271 2024-05-13 16:30:58.004527 ragstack_ai_langchain-1.0.3/ragstack_langchain/__init__.py
--rw-r--r--   0        0        0      434 2024-05-13 16:30:58.004527 ragstack_ai_langchain-1.0.3/ragstack_langchain/colbert/__init__.py
--rw-r--r--   0        0        0     2727 2024-05-13 16:30:58.004527 ragstack_ai_langchain-1.0.3/ragstack_langchain/colbert/colbert_retriever.py
--rw-r--r--   0        0        0     7346 2024-05-13 16:30:58.004527 ragstack_ai_langchain-1.0.3/ragstack_langchain/colbert/colbert_vector_store.py
--rw-r--r--   0        0        0     1679 1970-01-01 00:00:00.000000 ragstack_ai_langchain-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0      371 2024-05-21 20:07:23.544376 ragstack_ai_langchain-1.0.4/README.md
+-rw-r--r--   0        0        0     1219 2024-05-21 20:07:23.544376 ragstack_ai_langchain-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0      271 2024-05-21 20:07:23.544376 ragstack_ai_langchain-1.0.4/ragstack_langchain/__init__.py
+-rw-r--r--   0        0        0      434 2024-05-21 20:07:23.544376 ragstack_ai_langchain-1.0.4/ragstack_langchain/colbert/__init__.py
+-rw-r--r--   0        0        0     2715 2024-05-21 20:07:23.544376 ragstack_ai_langchain-1.0.4/ragstack_langchain/colbert/colbert_retriever.py
+-rw-r--r--   0        0        0     9303 2024-05-21 20:07:23.544376 ragstack_ai_langchain-1.0.4/ragstack_langchain/colbert/colbert_vector_store.py
+-rw-r--r--   0        0        0     1679 1970-01-01 00:00:00.000000 ragstack_ai_langchain-1.0.4/PKG-INFO
```

### Comparing `ragstack_ai_langchain-1.0.3/pyproject.toml` & `ragstack_ai_langchain-1.0.4/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "ragstack-ai-langchain"
-version = "1.0.3"
+version = "1.0.4"
 description = "DataStax RAGStack Langchain"
 license = "BUSL-1.1"
 authors = ["DataStax"]
 readme = "README.md"
 repository = "https://github.com/datastax/ragstack-ai"
 documentation = "https://docs.datastax.com/en/ragstack"
 packages = [{ include = "ragstack_langchain" }]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
 astrapy = "^1"
 cassio = "~0.1.4"
 unstructured = "0.12.5"
-ragstack-ai-colbert = "1.0.2"
+ragstack-ai-colbert = "1.0.3"
 
 # langchain
 langchain = "0.1.19"
 langchain-core = "0.1.52"
 langchain-community = "0.0.38"
 langchain-astradb = "0.3.0"
 langchain-openai = "0.1.3"
@@ -30,8 +30,11 @@
 colbert = ["ragstack-ai-colbert"]
 
 google = ["langchain-google-genai", "langchain-google-vertexai"]
 nvidia = ["langchain-nvidia-ai-endpoints"]
 
 [tool.poetry.group.test.dependencies]
 ragstack-ai-tests-utils = { path = "../tests-utils", develop = true }
-ragstack-ai-colbert = { path = "../colbert", develop = true }
+ragstack-ai-colbert = { path = "../colbert", develop = true }
+[tool.poetry.group.dev.dependencies]
+pytest-asyncio = "^0.23.6"
+
```

### Comparing `ragstack_ai_langchain-1.0.3/ragstack_langchain/colbert/colbert_retriever.py` & `ragstack_ai_langchain-1.0.4/ragstack_langchain/colbert/colbert_retriever.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,45 +21,45 @@
 
         llm = AzureChatOpenAI()
         retriever = ColbertLCRetriever(colbert_retriever, k=5)
         qa = RetrievalQA.from_chain_type(llm=llm, chain_type="stuff", retriever=retriever)
         qa.run("what happened on June 4th?")
     """
 
-    _retriever: ColbertBaseRetriever
-    _k: int
-    _query_maxlen: Optional[int]
+    retriever: ColbertBaseRetriever
+    k: int
+    query_maxlen: Optional[int]
 
     def __init__(
         self,
         retriever: ColbertBaseRetriever,
         k: Optional[int] = 5,
         query_maxlen: Optional[int] = None,
         **kwargs: Any,
     ):
         super().__init__(retriever=retriever, k=k, **kwargs)
-        self._retriever = retriever
-        self._k = k
-        self._query_maxlen = query_maxlen
+        self.retriever = retriever
+        self.k = k
+        self.query_maxlen = query_maxlen
 
     def _get_relevant_documents(
         self,
         query: str,
         *,
         run_manager: CallbackManagerForRetrieverRun,  # noqa
     ) -> List[Document]:
         """Get documents relevant to a query.
         Args:
             query: String to find relevant documents for
             run_manager: The callbacks handler to use
         Returns:
             List of relevant documents
         """
-        chunk_scores: List[Tuple[Chunk, float]] = self._retriever.text_search(
-            query_text=query, k=self._k, query_maxlen=self._query_maxlen
+        chunk_scores: List[Tuple[Chunk, float]] = self.retriever.text_search(
+            query_text=query, k=self.k, query_maxlen=self.query_maxlen
         )
 
         return [
             Document(page_content=c.text, metadata=c.metadata)
             for (c, _) in chunk_scores
         ]
 
@@ -72,15 +72,15 @@
         """Asynchronously get documents relevant to a query.
         Args:
             query: String to find relevant documents for
             run_manager: The callbacks handler to use
         Returns:
             List of relevant documents
         """
-        chunk_scores: List[Tuple[Chunk, float]] = await self._retriever.atext_search(
-            query_text=query, k=self._k, query_maxlen=self._query_maxlen
+        chunk_scores: List[Tuple[Chunk, float]] = await self.retriever.atext_search(
+            query_text=query, k=self.k, query_maxlen=self.query_maxlen
         )
 
         return [
             Document(page_content=c.text, metadata=c.metadata)
             for (c, _) in chunk_scores
         ]
```

### Comparing `ragstack_ai_langchain-1.0.3/PKG-INFO` & `ragstack_ai_langchain-1.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ragstack-ai-langchain
-Version: 1.0.3
+Version: 1.0.4
 Summary: DataStax RAGStack Langchain
 Home-page: https://github.com/datastax/ragstack-ai
 License: BUSL-1.1
 Author: DataStax
 Requires-Python: >=3.9,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -20,15 +20,15 @@
 Requires-Dist: langchain-astradb (==0.3.0)
 Requires-Dist: langchain-community (==0.0.38)
 Requires-Dist: langchain-core (==0.1.52)
 Requires-Dist: langchain-google-genai (==0.0.11) ; extra == "google"
 Requires-Dist: langchain-google-vertexai (==1.0.1) ; extra == "google"
 Requires-Dist: langchain-nvidia-ai-endpoints (==0.0.9) ; extra == "nvidia"
 Requires-Dist: langchain-openai (==0.1.3)
-Requires-Dist: ragstack-ai-colbert (==1.0.2) ; extra == "colbert"
+Requires-Dist: ragstack-ai-colbert (==1.0.3) ; extra == "colbert"
 Requires-Dist: unstructured (==0.12.5)
 Project-URL: Documentation, https://docs.datastax.com/en/ragstack
 Project-URL: Repository, https://github.com/datastax/ragstack-ai
 Description-Content-Type: text/markdown
 
 # RAGStack LangChain
```

