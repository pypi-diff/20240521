# Comparing `tmp/llama_index_embeddings_openai-0.1.8.tar.gz` & `tmp/llama_index_embeddings_openai-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_embeddings_openai-0.1.8.tar", max compression
+gzip compressed data, was "llama_index_embeddings_openai-0.1.9.tar", max compression
```

## Comparing `llama_index_embeddings_openai-0.1.8.tar` & `llama_index_embeddings_openai-0.1.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       44 2024-04-19 17:50:27.424508 llama_index_embeddings_openai-0.1.8/README.md
--rw-r--r--   0        0        0      286 2024-04-19 17:50:27.424508 llama_index_embeddings_openai-0.1.8/llama_index/embeddings/openai/__init__.py
--rw-r--r--   0        0        0    14911 2024-04-19 17:50:27.424508 llama_index_embeddings_openai-0.1.8/llama_index/embeddings/openai/base.py
--rw-r--r--   0        0        0     3272 2024-04-19 17:50:27.424508 llama_index_embeddings_openai-0.1.8/llama_index/embeddings/openai/utils.py
--rw-r--r--   0        0        0     1448 2024-04-19 17:50:27.424508 llama_index_embeddings_openai-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      603 1970-01-01 00:00:00.000000 llama_index_embeddings_openai-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0       44 2024-04-26 03:45:06.072109 llama_index_embeddings_openai-0.1.9/README.md
+-rw-r--r--   0        0        0      286 2024-04-26 03:45:06.072109 llama_index_embeddings_openai-0.1.9/llama_index/embeddings/openai/__init__.py
+-rw-r--r--   0        0        0    14991 2024-04-26 03:45:06.072109 llama_index_embeddings_openai-0.1.9/llama_index/embeddings/openai/base.py
+-rw-r--r--   0        0        0     3272 2024-04-26 03:45:06.072109 llama_index_embeddings_openai-0.1.9/llama_index/embeddings/openai/utils.py
+-rw-r--r--   0        0        0     1448 2024-04-26 03:45:06.072109 llama_index_embeddings_openai-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      603 1970-01-01 00:00:00.000000 llama_index_embeddings_openai-0.1.9/PKG-INFO
```

### Comparing `llama_index_embeddings_openai-0.1.8/llama_index/embeddings/openai/base.py` & `llama_index_embeddings_openai-0.1.9/llama_index/embeddings/openai/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -293,14 +293,15 @@
         api_version: Optional[str] = None,
         max_retries: int = 10,
         timeout: float = 60.0,
         reuse_client: bool = True,
         callback_manager: Optional[CallbackManager] = None,
         default_headers: Optional[Dict[str, str]] = None,
         http_client: Optional[httpx.Client] = None,
+        num_workers: Optional[int] = None,
         **kwargs: Any,
     ) -> None:
         additional_kwargs = additional_kwargs or {}
         if dimensions is not None:
             additional_kwargs["dimensions"] = dimensions
 
         api_key, api_base, api_version = self._resolve_credentials(
@@ -327,14 +328,15 @@
             api_key=api_key,
             api_base=api_base,
             api_version=api_version,
             max_retries=max_retries,
             reuse_client=reuse_client,
             timeout=timeout,
             default_headers=default_headers,
+            num_workers=num_workers,
             **kwargs,
         )
 
         self._client = None
         self._aclient = None
         self._http_client = http_client
```

### Comparing `llama_index_embeddings_openai-0.1.8/llama_index/embeddings/openai/utils.py` & `llama_index_embeddings_openai-0.1.9/llama_index/embeddings/openai/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_embeddings_openai-0.1.8/pyproject.toml` & `llama_index_embeddings_openai-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index embeddings openai integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-embeddings-openai"
 readme = "README.md"
-version = "0.1.8"
+version = "0.1.9"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "8.10.0"
```

### Comparing `llama_index_embeddings_openai-0.1.8/PKG-INFO` & `llama_index_embeddings_openai-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-embeddings-openai
-Version: 0.1.8
+Version: 0.1.9
 Summary: llama-index embeddings openai integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

