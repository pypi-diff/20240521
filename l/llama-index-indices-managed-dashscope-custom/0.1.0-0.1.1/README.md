# Comparing `tmp/llama_index_indices_managed_dashscope_custom-0.1.0.tar.gz` & `tmp/llama_index_indices_managed_dashscope_custom-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_indices_managed_dashscope_custom-0.1.0.tar", max compression
+gzip compressed data, was "llama_index_indices_managed_dashscope_custom-0.1.1.tar", max compression
```

## Comparing `llama_index_indices_managed_dashscope_custom-0.1.0.tar` & `llama_index_indices_managed_dashscope_custom-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0      962 2024-05-04 10:15:34.641626 llama_index_indices_managed_dashscope_custom-0.1.0/README.md
--rw-r--r--   0        0        0      222 2024-05-04 10:01:07.074363 llama_index_indices_managed_dashscope_custom-0.1.0/llama_index/indices/managed/dashscope/__init__.py
--rw-r--r--   0        0        0     2304 2024-05-04 10:16:50.938220 llama_index_indices_managed_dashscope_custom-0.1.0/llama_index/indices/managed/dashscope/api_utils.py
--rw-r--r--   0        0        0     8547 2024-05-04 10:17:40.841576 llama_index_indices_managed_dashscope_custom-0.1.0/llama_index/indices/managed/dashscope/base.py
--rw-r--r--   0        0        0      451 2024-05-04 10:15:33.319958 llama_index_indices_managed_dashscope_custom-0.1.0/llama_index/indices/managed/dashscope/constants.py
--rw-r--r--   0        0        0     7269 2024-05-04 10:15:43.543900 llama_index_indices_managed_dashscope_custom-0.1.0/llama_index/indices/managed/dashscope/retriever.py
--rw-r--r--   0        0        0     6540 2024-05-04 10:15:33.383777 llama_index_indices_managed_dashscope_custom-0.1.0/llama_index/indices/managed/dashscope/transformations.py
--rw-r--r--   0        0        0      821 2024-05-04 10:18:00.749894 llama_index_indices_managed_dashscope_custom-0.1.0/llama_index/indices/managed/dashscope/utils.py
--rw-r--r--   0        0        0     1779 2024-05-08 05:45:43.557896 llama_index_indices_managed_dashscope_custom-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1802 1970-01-01 00:00:00.000000 llama_index_indices_managed_dashscope_custom-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1043 2024-05-21 09:52:43.927372 llama_index_indices_managed_dashscope_custom-0.1.1/README.md
+-rw-r--r--   0        0        0       17 2024-05-21 10:02:17.074444 llama_index_indices_managed_dashscope_custom-0.1.1/llama_index/indices/managed/dashscope/BUILD
+-rw-r--r--   0        0        0      222 2024-05-04 10:01:07.074363 llama_index_indices_managed_dashscope_custom-0.1.1/llama_index/indices/managed/dashscope/__init__.py
+-rw-r--r--   0        0        0     3810 2024-05-21 09:52:25.342581 llama_index_indices_managed_dashscope_custom-0.1.1/llama_index/indices/managed/dashscope/api_utils.py
+-rw-r--r--   0        0        0     9564 2024-05-21 09:27:42.938984 llama_index_indices_managed_dashscope_custom-0.1.1/llama_index/indices/managed/dashscope/base.py
+-rw-r--r--   0        0        0      594 2024-05-21 09:24:23.662804 llama_index_indices_managed_dashscope_custom-0.1.1/llama_index/indices/managed/dashscope/constants.py
+-rw-r--r--   0        0        0     7269 2024-05-04 10:15:43.543900 llama_index_indices_managed_dashscope_custom-0.1.1/llama_index/indices/managed/dashscope/retriever.py
+-rw-r--r--   0        0        0     3810 2024-05-21 09:24:29.485949 llama_index_indices_managed_dashscope_custom-0.1.1/llama_index/indices/managed/dashscope/transformations.py
+-rw-r--r--   0        0        0     1876 2024-05-21 09:24:29.480657 llama_index_indices_managed_dashscope_custom-0.1.1/llama_index/indices/managed/dashscope/utils.py
+-rw-r--r--   0        0        0     1769 2024-05-21 10:28:34.231790 llama_index_indices_managed_dashscope_custom-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1872 1970-01-01 00:00:00.000000 llama_index_indices_managed_dashscope_custom-0.1.1/PKG-INFO
```

### Comparing `llama_index_indices_managed_dashscope_custom-0.1.0/README.md` & `llama_index_indices_managed_dashscope_custom-0.1.1/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # LlamaIndex Indices Integration: Managed-Dashscope
 
+## Installation
+
+```shell
+pip install llama-index-indices-managed-dashscope
+```
+
 ## Usage
 
 ```python
 import os
 from llama_index.core.schema import QueryBundle
 from llama_index.readers.dashscope.base import DashScopeParse
 from llama_index.readers.dashscope.utils import ResultType
```

### Comparing `llama_index_indices_managed_dashscope_custom-0.1.0/llama_index/indices/managed/dashscope/api_utils.py` & `llama_index_indices_managed_dashscope_custom-0.1.1/llama_index/indices/managed/dashscope/api_utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import json
 from typing import List, Optional
 
 from llama_index.indices.managed.dashscope.transformations import (
-    ConfiguredTransformation,
+    DashScopeConfiguredTransformation,
 )
 from llama_index.core.schema import BaseNode, TransformComponent
 
 
 def default_transformations() -> List[TransformComponent]:
     """Default transformations."""
-    from llama_index.node_parser.relational.dashscope import DashScopeJsonNodeParser
+    from llama_index.node_parser.dashscope import DashScopeJsonNodeParser
     from llama_index.embeddings.dashscope import (
         DashScopeEmbedding,
         DashScopeTextEmbeddingModels,
         DashScopeTextEmbeddingType,
     )
 
     node_parser = DashScopeJsonNodeParser()
@@ -27,20 +27,20 @@
     ]
 
 
 def get_pipeline_create(
     name: str,
     transformations: Optional[List[TransformComponent]] = None,
     documents: Optional[List[BaseNode]] = None,
-) -> str:
-    configured_transformations: List[ConfiguredTransformation] = []
+) -> dict:
+    configured_transformations: List[DashScopeConfiguredTransformation] = []
     for transformation in transformations:
         try:
             configured_transformations.append(
-                ConfiguredTransformation.from_component(transformation)
+                DashScopeConfiguredTransformation.from_component(transformation)
             )
         except ValueError:
             raise ValueError(f"Unsupported transformation: {type(transformation)}")
 
     configured_transformation_items: List[Dict] = []
     for item in configured_transformations:
         configured_transformation_items.append(
@@ -67,7 +67,56 @@
                 "sink_type": "ES",
             }
         ],
         # for debug
         "data_type": "structured",
         "config_model": "recommend",
     }
+
+
+def get_doc_insert(
+    transformations: Optional[List[TransformComponent]] = None,
+    documents: Optional[List[BaseNode]] = None,
+) -> dict:
+    configured_transformations: List[DashScopeConfiguredTransformation] = []
+    for transformation in transformations:
+        try:
+            configured_transformations.append(
+                DashScopeConfiguredTransformation.from_component(transformation)
+            )
+        except ValueError:
+            raise ValueError(f"Unsupported transformation: {type(transformation)}")
+
+    configured_transformation_items: List[Dict] = []
+    for item in configured_transformations:
+        configured_transformation_items.append(
+            {
+                "component": json.loads(item.component.json()),
+                "configurable_transformation_type": item.configurable_transformation_type.name,
+            }
+        )
+    data_sources = [
+        {
+            "source_type": "DATA_CENTER_FILE",
+            "component": {
+                "doc_ids": [doc.node_id for doc in documents],
+            },
+        }
+    ]
+    return {
+        "configured_transformations": configured_transformation_items,
+        "data_sources": data_sources,
+    }
+
+
+def get_doc_delete(ref_doc_ids: List[str]) -> dict:
+    data_sources = [
+        {
+            "source_type": "DATA_CENTER_FILE",
+            "component": {
+                "doc_ids": ref_doc_ids,
+            },
+        }
+    ]
+    return {
+        "data_sources": data_sources,
+    }
```

### Comparing `llama_index_indices_managed_dashscope_custom-0.1.0/llama_index/indices/managed/dashscope/base.py` & `llama_index_indices_managed_dashscope_custom-0.1.1/llama_index/indices/managed/dashscope/base.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,44 @@
 """Managed index.
 
 A managed Index - where the index is accessible via some API that
 interfaces a managed service.
 
 """
 import os
-import time
-from typing import Any, List, Optional, Sequence, Type
+from typing import Any, List, Optional, Type, Union
 from enum import Enum
-import time
 import requests
 import json
 
 from llama_index.core.base.base_query_engine import BaseQueryEngine
 from llama_index.core.base.base_retriever import BaseRetriever
 from llama_index.core.callbacks.base import CallbackManager
 from llama_index.core.indices.managed.base import BaseManagedIndex
 from llama_index.core.schema import BaseNode, Document, TransformComponent
 from llama_index.core.settings import Settings
 
 from llama_index.indices.managed.dashscope.api_utils import (
     get_pipeline_create,
     default_transformations,
+    get_doc_insert,
+    get_doc_delete,
+)
+from llama_index.indices.managed.dashscope.utils import (
+    run_ingestion,
+    get_pipeline_id,
 )
-
 from llama_index.indices.managed.dashscope.constants import (
     DASHSCOPE_DEFAULT_BASE_URL,
     UPSERT_PIPELINE_ENDPOINT,
     START_PIPELINE_ENDPOINT,
     CHECK_INGESTION_ENDPOINT,
+    PIPELINE_SIMPLE_ENDPOINT,
+    INSERT_DOC_ENDPOINT,
+    DELETE_DOC_ENDPOINT,
 )
 
 
 class Status(Enum):
     ERROR = "ERROR"
     SUCCESS = "Success"
     PENDING = "PENDING"
@@ -66,14 +72,21 @@
             raise ValueError(
                 "DashScopeCloudIndex does not support nodes on initialization"
             )
 
         self.workspace_id = workspace_id or os.environ.get("DASHSCOPE_WORKSPACE_ID")
         self._api_key = api_key or os.environ.get("DASHSCOPE_API_KEY")
         self._base_url = os.environ.get("DASHSCOPE_BASE_URL", None) or base_url
+        self._headers = {
+            "Content-Type": "application/json",
+            "Accept-Encoding": "utf-8",
+            "X-DashScope-WorkSpace": self.workspace_id,
+            "Authorization": "Bearer " + self._api_key,
+            "X-DashScope-OpenAPISource": "CloudSDK",
+        }
         self._timeout = timeout
         self._show_progress = show_progress
         self._service_context = None
         self._callback_manager = callback_manager or Settings.callback_manager
 
     @classmethod
     def from_documents(  # type: ignore
@@ -88,39 +101,30 @@
         verbose: bool = True,
         **kwargs: Any,
     ) -> "DashScopeCloudIndex":
         """Build a DashScope index from a sequence of documents."""
         pipeline_create = get_pipeline_create(
             name, transformations or default_transformations(), documents
         )
-        # for debug
-        json.dump(
-            pipeline_create, open("pipeline_create.json", "w"), ensure_ascii=False
-        )
 
         workspace_id = workspace_id or os.environ.get("DASHSCOPE_WORKSPACE_ID")
         api_key = api_key or os.environ.get("DASHSCOPE_API_KEY")
         base_url = (
             base_url
             or os.environ.get("DASHSCOPE_BASE_URL", None)
             or DASHSCOPE_DEFAULT_BASE_URL
         )
         headers = {
             "Content-Type": "application/json",
             "Accept-Encoding": "utf-8",
             "X-DashScope-WorkSpace": workspace_id,
             "Authorization": "Bearer " + api_key,
             "X-DashScope-OpenAPISource": "CloudSDK",
-            # for debug
-            # 'X-DashScope-ApiKeyId': 'test_api_key_id_123456',
-            # 'X-DashScope-Uid': "test_uid_123456",
-            # "X-DashScope-SubUid": "test_sub_uid_123456"
         }
-        print(base_url + UPSERT_PIPELINE_ENDPOINT)
-        print(json.dumps(pipeline_create))
+
         response = requests.put(
             base_url + UPSERT_PIPELINE_ENDPOINT,
             data=json.dumps(pipeline_create),
             headers=headers,
         )
         response_text = response.json()
         pipeline_id = response_text.get("id", None)
@@ -128,16 +132,14 @@
         if response_text.get("code", "") != Status.SUCCESS.value or pipeline_id is None:
             raise ValueError(
                 f"Failed to create index: {response_text.get('message', '')}\n{response_text}"
             )
         if verbose:
             print(f"Starting creating index {name}, pipeline_id: {pipeline_id}")
 
-        print(base_url + START_PIPELINE_ENDPOINT.format(pipeline_id=pipeline_id))
-
         response = requests.post(
             base_url + START_PIPELINE_ENDPOINT.format(pipeline_id=pipeline_id),
             headers=headers,
         )
         response_text = response.json()
         ingestion_id = response_text.get("ingestionId", None)
 
@@ -147,49 +149,22 @@
         ):
             raise ValueError(
                 f"Failed to start ingestion: {response_text.get('message', '')}\n{response_text}"
             )
         if verbose:
             print(f"Starting ingestion for index {name}, ingestion_id: {ingestion_id}")
 
-        ingestion_status = ""
-        failed_docs = []
-
-        while True:
-            print(
-                base_url
-                + CHECK_INGESTION_ENDPOINT.format(
-                    pipeline_id=pipeline_id, ingestion_id=ingestion_id
-                )
-            )
-            response = requests.get(
-                base_url
-                + CHECK_INGESTION_ENDPOINT.format(
-                    pipeline_id=pipeline_id, ingestion_id=ingestion_id
-                ),
-                headers=headers,
-            )
-            try:
-                response_text = response.json()
-            except Exception as e:
-                print(f"Failed to get response: \n{response.text}\nretrying...")
-                continue
-
-            if response_text.get("code", "") != Status.SUCCESS.value:
-                print(
-                    f"Failed to get ingestion status: {response_text.get('message', '')}\n{response_text}\nretrying..."
-                )
-                continue
-            ingestion_status = response_text.get("ingestion_status", "")
-            failed_docs = response_text.get("failed_docs", "")
-            if verbose:
-                print(f"Current status: {ingestion_status}")
-            if ingestion_status in ["COMPLETED", "FAILED"]:
-                break
-            time.sleep(5)
+        ingestion_status, failed_docs = run_ingestion(
+            base_url
+            + CHECK_INGESTION_ENDPOINT.format(
+                pipeline_id=pipeline_id, ingestion_id=ingestion_id
+            ),
+            headers,
+            verbose,
+        )
 
         if verbose:
             print(f"ingestion_status {ingestion_status}")
             print(f"failed_docs: {failed_docs}")
 
         if ingestion_status == "FAILED":
             print("Index {name} created failed!")
@@ -223,20 +198,83 @@
         from llama_index.core.query_engine.retriever_query_engine import (
             RetrieverQueryEngine,
         )
 
         kwargs["retriever"] = self.as_retriever(**kwargs)
         return RetrieverQueryEngine.from_args(**kwargs)
 
-    def _insert(self, nodes: Sequence[BaseNode], **insert_kwargs: Any) -> None:
+    def _insert(
+        self,
+        documents: List[Document],
+        transformations: Optional[List[TransformComponent]] = None,
+        verbose: bool = True,
+        **insert_kwargs: Any,
+    ) -> None:
         """Insert a set of documents (each a node)."""
-        raise NotImplementedError("_insert not implemented.")
+        pipeline_id = get_pipeline_id(
+            self._base_url + PIPELINE_SIMPLE_ENDPOINT,
+            self._headers,
+            {"pipeline_name": self.name},
+        )
+        doc_insert = get_doc_insert(
+            transformations or default_transformations(),
+            documents,
+        )
+        response = requests.put(
+            self._base_url + INSERT_DOC_ENDPOINT.format(pipeline_id=pipeline_id),
+            data=json.dumps(doc_insert),
+            headers=self._headers,
+        )
+        response_text = response.json()
+        ingestion_id = response_text.get("ingestionId", None)
+        if (
+            response_text.get("code", "") != Status.SUCCESS.value
+            or ingestion_id is None
+        ):
+            raise ValueError(
+                f"Failed to insert documents: {response_text.get('message', '')}\n{response_text}"
+            )
+
+        ingestion_status, failed_docs = run_ingestion(
+            self._base_url
+            + CHECK_INGESTION_ENDPOINT.format(
+                pipeline_id=pipeline_id, ingestion_id=ingestion_id
+            ),
+            self._headers,
+            verbose,
+        )
+
+        if verbose:
+            print(f"ingestion_status {ingestion_status}")
+            print(f"failed_docs: {failed_docs}")
 
     def delete_ref_doc(
-        self, ref_doc_id: str, delete_from_docstore: bool = False, **delete_kwargs: Any
+        self,
+        ref_doc_ids: Union[str, List[str]],
+        verbose: bool = True,
+        **delete_kwargs: Any,
     ) -> None:
-        """Delete a document and it's nodes by using ref_doc_id."""
-        raise NotImplementedError("delete_ref_doc not implemented.")
+        """Delete documents in index."""
+        if isinstance(ref_doc_ids, str):
+            ref_doc_ids = [ref_doc_ids]
+        pipeline_id = get_pipeline_id(
+            self._base_url + PIPELINE_SIMPLE_ENDPOINT,
+            self._headers,
+            {"pipeline_name": self.name},
+        )
+        doc_delete = get_doc_delete(ref_doc_ids)
+        response = requests.post(
+            self._base_url + DELETE_DOC_ENDPOINT.format(pipeline_id=pipeline_id),
+            json=doc_delete,
+            headers=self._headers,
+        )
+        response_text = response.json()
+        if response_text.get("code", "") != Status.SUCCESS.value:
+            raise ValueError(
+                f"Failed to delete documents: {response_text.get('message', '')}\n{response_text}"
+            )
+        if verbose:
+            print(f"Delete documents {ref_doc_ids} successfully!")
 
     def update_ref_doc(self, document: Document, **update_kwargs: Any) -> None:
         """Update a document and it's corresponding nodes."""
         raise NotImplementedError("update_ref_doc not implemented.")
```

### Comparing `llama_index_indices_managed_dashscope_custom-0.1.0/llama_index/indices/managed/dashscope/retriever.py` & `llama_index_indices_managed_dashscope_custom-0.1.1/llama_index/indices/managed/dashscope/retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index_indices_managed_dashscope_custom-0.1.0/pyproject.toml` & `llama_index_indices_managed_dashscope_custom-0.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 skip = "*.csv,*.html,*.json,*.jsonl,*.pdf,*.txt,*.ipynb"
 
 [tool.llamahub]
 contains_example = false
 import_path = "llama_index.indices.managed.dashscope"
 
 [tool.llamahub.class_authors]
-DashScopeEmbedding = "phantomgrapes"
+DashScopeCloudIndex = "phantomgrapes"
 
 [tool.mypy]
 disallow_untyped_defs = true
 # Remove venv skip when integrated with pre-commit
 exclude = ["_static", "build", "examples", "notebooks", "venv"]
 ignore_missing_imports = true
 python_version = "3.8"
@@ -26,22 +26,22 @@
 [tool.poetry]
 authors = ["Ruixue Ding <ada.drx@alibaba-inc.com>"]
 description = "llama-index indices managed-dashscope integration"
 license = "MIT"
 name = "llama-index-indices-managed-dashscope-custom"
 packages = [{include = "llama_index/"}]
 readme = "README.md"
-version = "0.1.0"
+version = "0.1.1"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.0"
 llama-index-embeddings-dashscope = ">=0.1.3"
-llama-index-readers-dashscope-custom = ">=0.1.0"
-llama-index-node-parser-relational-dashscope-custom = ">=0.1.0"
+llama-index-readers-dashscope-custom = ">=0.1.1"
+llama-index-node-parser-dashscope-custom = ">=0.1.2"
 
 [tool.poetry.group.dev.dependencies]
 black = {extras = ["jupyter"], version = "<=23.9.1,>=23.7.0"}
 codespell = {extras = ["toml"], version = ">=v2.2.6"}
 ipython = "8.10.0"
 jupyter = "^1.0.0"
 mypy = "0.991"
```

### Comparing `llama_index_indices_managed_dashscope_custom-0.1.0/PKG-INFO` & `llama_index_indices_managed_dashscope_custom-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 Metadata-Version: 2.1
 Name: llama-index-indices-managed-dashscope-custom
-Version: 0.1.0
+Version: 0.1.1
 Summary: llama-index indices managed-dashscope integration
 License: MIT
 Author: Ruixue Ding
 Author-email: ada.drx@alibaba-inc.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: llama-index-core (>=0.10.0,<0.11.0)
 Requires-Dist: llama-index-embeddings-dashscope (>=0.1.3)
-Requires-Dist: llama-index-node-parser-relational-dashscope-custom (>=0.1.0)
-Requires-Dist: llama-index-readers-dashscope-custom (>=0.1.0)
+Requires-Dist: llama-index-node-parser-dashscope-custom (>=0.1.2)
+Requires-Dist: llama-index-readers-dashscope-custom (>=0.1.1)
 Description-Content-Type: text/markdown
 
 # LlamaIndex Indices Integration: Managed-Dashscope
 
+## Installation
+
+```shell
+pip install llama-index-indices-managed-dashscope
+```
+
 ## Usage
 
 ```python
 import os
 from llama_index.core.schema import QueryBundle
 from llama_index.readers.dashscope.base import DashScopeParse
 from llama_index.readers.dashscope.utils import ResultType
```

