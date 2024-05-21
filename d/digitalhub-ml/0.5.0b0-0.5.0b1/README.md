# Comparing `tmp/digitalhub_ml-0.5.0b0.tar.gz` & `tmp/digitalhub_ml-0.5.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digitalhub_ml-0.5.0b0.tar", last modified: Mon May 20 12:49:20 2024, max compression
+gzip compressed data, was "digitalhub_ml-0.5.0b1.tar", last modified: Tue May 21 15:54:41 2024, max compression
```

## Comparing `digitalhub_ml-0.5.0b0.tar` & `digitalhub_ml-0.5.0b1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-20 12:49:20.762657 digitalhub_ml-0.5.0b0/
--rw-r--r--   0 mmartini  (1000) mmartini  (1000)      938 2024-05-20 12:49:20.762657 digitalhub_ml-0.5.0b0/PKG-INFO
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      462 2024-04-23 09:36:04.000000 digitalhub_ml-0.5.0b0/README.md
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-20 12:49:20.758657 digitalhub_ml-0.5.0b0/digitalhub_ml/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      304 2024-05-20 09:51:09.000000 digitalhub_ml-0.5.0b0/digitalhub_ml/__init__.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-20 12:49:20.758657 digitalhub_ml-0.5.0b0/digitalhub_ml/entities/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-02-01 11:38:37.000000 digitalhub_ml-0.5.0b0/digitalhub_ml/entities/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      436 2024-05-06 11:22:14.000000 digitalhub_ml-0.5.0b0/digitalhub_ml/entities/entity_types.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-20 12:49:20.758657 digitalhub_ml-0.5.0b0/digitalhub_ml/entities/models/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-02-01 11:40:22.000000 digitalhub_ml-0.5.0b0/digitalhub_ml/entities/models/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6328 2024-05-20 09:51:09.000000 digitalhub_ml-0.5.0b0/digitalhub_ml/entities/models/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    12517 2024-05-20 09:55:25.000000 digitalhub_ml-0.5.0b0/digitalhub_ml/entities/models/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      318 2024-04-23 09:36:04.000000 digitalhub_ml-0.5.0b0/digitalhub_ml/entities/models/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      996 2024-05-20 07:16:51.000000 digitalhub_ml-0.5.0b0/digitalhub_ml/entities/models/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      209 2024-02-15 10:15:41.000000 digitalhub_ml-0.5.0b0/digitalhub_ml/entities/models/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-20 12:49:20.762657 digitalhub_ml-0.5.0b0/digitalhub_ml/entities/projects/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-02-01 11:33:48.000000 digitalhub_ml-0.5.0b0/digitalhub_ml/entities/projects/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6049 2024-05-20 09:51:09.000000 digitalhub_ml-0.5.0b0/digitalhub_ml/entities/projects/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     5869 2024-05-20 09:51:09.000000 digitalhub_ml-0.5.0b0/digitalhub_ml/entities/projects/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      988 2024-05-20 09:51:09.000000 digitalhub_ml-0.5.0b0/digitalhub_ml/entities/projects/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      730 2024-05-06 11:19:46.000000 digitalhub_ml-0.5.0b0/digitalhub_ml/entities/registries.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-20 12:49:20.762657 digitalhub_ml-0.5.0b0/digitalhub_ml/entities/runs/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-23 14:34:03.000000 digitalhub_ml-0.5.0b0/digitalhub_ml/entities/runs/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      300 2024-03-07 13:39:55.000000 digitalhub_ml-0.5.0b0/digitalhub_ml/entities/runs/models.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      405 2024-05-20 09:51:09.000000 digitalhub_ml-0.5.0b0/digitalhub_ml/entities/runs/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      313 2024-03-14 13:46:16.000000 digitalhub_ml-0.5.0b0/digitalhub_ml/entities/runs/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-20 12:49:20.762657 digitalhub_ml-0.5.0b0/digitalhub_ml.egg-info/
--rw-r--r--   0 mmartini  (1000) mmartini  (1000)      938 2024-05-20 12:49:20.000000 digitalhub_ml-0.5.0b0/digitalhub_ml.egg-info/PKG-INFO
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      903 2024-05-20 12:49:20.000000 digitalhub_ml-0.5.0b0/digitalhub_ml.egg-info/SOURCES.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        1 2024-05-20 12:49:20.000000 digitalhub_ml-0.5.0b0/digitalhub_ml.egg-info/dependency_links.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       21 2024-05-20 12:49:20.000000 digitalhub_ml-0.5.0b0/digitalhub_ml.egg-info/requires.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       19 2024-05-20 12:49:20.000000 digitalhub_ml-0.5.0b0/digitalhub_ml.egg-info/top_level.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1054 2024-05-20 07:16:51.000000 digitalhub_ml-0.5.0b0/pyproject.toml
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       38 2024-05-20 12:49:20.762657 digitalhub_ml-0.5.0b0/setup.cfg
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 15:54:41.207126 digitalhub_ml-0.5.0b1/
+-rw-r--r--   0 mmartini  (1000) mmartini  (1000)      942 2024-05-21 15:54:41.207126 digitalhub_ml-0.5.0b1/PKG-INFO
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      462 2024-04-23 09:36:04.000000 digitalhub_ml-0.5.0b1/README.md
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 15:54:41.195126 digitalhub_ml-0.5.0b1/digitalhub_ml/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      304 2024-05-21 13:14:46.000000 digitalhub_ml-0.5.0b1/digitalhub_ml/__init__.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 15:54:41.199126 digitalhub_ml-0.5.0b1/digitalhub_ml/entities/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-02-01 11:38:37.000000 digitalhub_ml-0.5.0b1/digitalhub_ml/entities/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      436 2024-05-06 11:22:14.000000 digitalhub_ml-0.5.0b1/digitalhub_ml/entities/entity_types.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 15:54:41.199126 digitalhub_ml-0.5.0b1/digitalhub_ml/entities/models/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-02-01 11:40:22.000000 digitalhub_ml-0.5.0b1/digitalhub_ml/entities/models/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6328 2024-05-21 13:14:46.000000 digitalhub_ml-0.5.0b1/digitalhub_ml/entities/models/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    12455 2024-05-21 13:14:46.000000 digitalhub_ml-0.5.0b1/digitalhub_ml/entities/models/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      318 2024-04-23 09:36:04.000000 digitalhub_ml-0.5.0b1/digitalhub_ml/entities/models/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1029 2024-05-21 12:34:21.000000 digitalhub_ml-0.5.0b1/digitalhub_ml/entities/models/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      209 2024-02-15 10:15:41.000000 digitalhub_ml-0.5.0b1/digitalhub_ml/entities/models/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 15:54:41.203126 digitalhub_ml-0.5.0b1/digitalhub_ml/entities/projects/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-02-01 11:33:48.000000 digitalhub_ml-0.5.0b1/digitalhub_ml/entities/projects/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6049 2024-05-21 13:14:46.000000 digitalhub_ml-0.5.0b1/digitalhub_ml/entities/projects/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     5869 2024-05-21 13:14:46.000000 digitalhub_ml-0.5.0b1/digitalhub_ml/entities/projects/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      988 2024-05-21 13:14:46.000000 digitalhub_ml-0.5.0b1/digitalhub_ml/entities/projects/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      730 2024-05-06 11:19:46.000000 digitalhub_ml-0.5.0b1/digitalhub_ml/entities/registries.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 15:54:41.203126 digitalhub_ml-0.5.0b1/digitalhub_ml/entities/runs/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-23 14:34:03.000000 digitalhub_ml-0.5.0b1/digitalhub_ml/entities/runs/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      300 2024-03-07 13:39:55.000000 digitalhub_ml-0.5.0b1/digitalhub_ml/entities/runs/models.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      405 2024-05-21 13:14:46.000000 digitalhub_ml-0.5.0b1/digitalhub_ml/entities/runs/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      313 2024-03-14 13:46:16.000000 digitalhub_ml-0.5.0b1/digitalhub_ml/entities/runs/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 15:54:41.203126 digitalhub_ml-0.5.0b1/digitalhub_ml.egg-info/
+-rw-r--r--   0 mmartini  (1000) mmartini  (1000)      942 2024-05-21 15:54:41.000000 digitalhub_ml-0.5.0b1/digitalhub_ml.egg-info/PKG-INFO
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      903 2024-05-21 15:54:41.000000 digitalhub_ml-0.5.0b1/digitalhub_ml.egg-info/SOURCES.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        1 2024-05-21 15:54:41.000000 digitalhub_ml-0.5.0b1/digitalhub_ml.egg-info/dependency_links.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       25 2024-05-21 15:54:41.000000 digitalhub_ml-0.5.0b1/digitalhub_ml.egg-info/requires.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       19 2024-05-21 15:54:41.000000 digitalhub_ml-0.5.0b1/digitalhub_ml.egg-info/top_level.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1058 2024-05-21 15:33:27.000000 digitalhub_ml-0.5.0b1/pyproject.toml
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       38 2024-05-21 15:54:41.207126 digitalhub_ml-0.5.0b1/setup.cfg
```

### Comparing `digitalhub_ml-0.5.0b0/PKG-INFO` & `digitalhub_ml-0.5.0b1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: digitalhub-ml
-Version: 0.5.0b0
+Version: 0.5.0b1
 Summary: Python SDK for DHCore
 Author-email: Fondazione Bruno Kessler <dslab@fbk.eu>, Matteo Martini <mmartini@fbk.eu>
 Keywords: data,dataops,kubernetes
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: digitalhub-data~=0.5
+Requires-Dist: digitalhub-data==0.5.0b1
 
 # Digitalhub-ml Library
 
 The Digitalhub-ml SDK library is used to manage entities and executions in Digitalhub from Python.
 The Digitalhub-ml layer is the third layer of the Digitalhub ml platform, focused on machine learning functions.
 It contains the ml entities and objects (Models) and the methods to manage them.
```

### Comparing `digitalhub_ml-0.5.0b0/digitalhub_ml/entities/models/crud.py` & `digitalhub_ml-0.5.0b1/digitalhub_ml/entities/models/crud.py`

 * *Files identical despite different names*

### Comparing `digitalhub_ml-0.5.0b0/digitalhub_ml/entities/models/entity.py` & `digitalhub_ml-0.5.0b1/digitalhub_ml/entities/models/entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from urllib.parse import urlparse
 
 from digitalhub_core.context.builder import get_context
 from digitalhub_core.entities._base.entity import Entity
 from digitalhub_core.entities._builders.metadata import build_metadata
 from digitalhub_core.entities._builders.spec import build_spec
 from digitalhub_core.entities._builders.status import build_status
-from digitalhub_core.entities.entity_types import EntityTypes
 from digitalhub_core.stores.builder import get_store
 from digitalhub_core.utils.api import api_ctx_create, api_ctx_read, api_ctx_update
 from digitalhub_core.utils.exceptions import EntityError
 from digitalhub_core.utils.generic_utils import build_uuid, get_timestamp
 from digitalhub_core.utils.io_utils import write_yaml
 from digitalhub_core.utils.uri_utils import map_uri_scheme
 from digitalhub_ml.entities.entity_types import EntityTypes
```

### Comparing `digitalhub_ml-0.5.0b0/digitalhub_ml/entities/models/spec.py` & `digitalhub_ml-0.5.0b1/digitalhub_ml/entities/models/spec.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,15 +27,19 @@
 
 class ModelSpecModel(ModelSpec):
     """
     Model specifications.
     """
 
     def __init__(
-        self, base_model: str | None = None, parameters: dict | None = None, metrics: dict | None = None, **kwargs
+        self,
+        base_model: str | None = None,
+        parameters: dict | None = None,
+        metrics: dict | None = None,
+        **kwargs,
     ) -> None:
         """
         Constructor.
         """
         self.base_model = base_model
         self.parameters = parameters
         self.metrics = metrics
```

### Comparing `digitalhub_ml-0.5.0b0/digitalhub_ml/entities/projects/crud.py` & `digitalhub_ml-0.5.0b1/digitalhub_ml/entities/projects/crud.py`

 * *Files identical despite different names*

### Comparing `digitalhub_ml-0.5.0b0/digitalhub_ml/entities/projects/entity.py` & `digitalhub_ml-0.5.0b1/digitalhub_ml/entities/projects/entity.py`

 * *Files identical despite different names*

### Comparing `digitalhub_ml-0.5.0b0/digitalhub_ml/entities/projects/spec.py` & `digitalhub_ml-0.5.0b1/digitalhub_ml/entities/projects/spec.py`

 * *Files identical despite different names*

### Comparing `digitalhub_ml-0.5.0b0/digitalhub_ml/entities/registries.py` & `digitalhub_ml-0.5.0b1/digitalhub_ml/entities/registries.py`

 * *Files identical despite different names*

### Comparing `digitalhub_ml-0.5.0b0/digitalhub_ml.egg-info/PKG-INFO` & `digitalhub_ml-0.5.0b1/digitalhub_ml.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: digitalhub-ml
-Version: 0.5.0b0
+Version: 0.5.0b1
 Summary: Python SDK for DHCore
 Author-email: Fondazione Bruno Kessler <dslab@fbk.eu>, Matteo Martini <mmartini@fbk.eu>
 Keywords: data,dataops,kubernetes
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: digitalhub-data~=0.5
+Requires-Dist: digitalhub-data==0.5.0b1
 
 # Digitalhub-ml Library
 
 The Digitalhub-ml SDK library is used to manage entities and executions in Digitalhub from Python.
 The Digitalhub-ml layer is the third layer of the Digitalhub ml platform, focused on machine learning functions.
 It contains the ml entities and objects (Models) and the methods to manage them.
```

### Comparing `digitalhub_ml-0.5.0b0/digitalhub_ml.egg-info/SOURCES.txt` & `digitalhub_ml-0.5.0b1/digitalhub_ml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `digitalhub_ml-0.5.0b0/pyproject.toml` & `digitalhub_ml-0.5.0b1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "digitalhub-ml"
-version = "0.5.0b0"
+version = "0.5.0b1"
 description = "Python SDK for DHCore"
 readme = "README.md"
 authors = [
     { name = "Fondazione Bruno Kessler", email = "dslab@fbk.eu" },
     { name = "Matteo Martini", email = "mmartini@fbk.eu" }
 ]
 license = { file = "LICENSE.txt" }
@@ -16,22 +16,22 @@
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10"
 ]
 keywords = ["data", "dataops", "kubernetes"]
 requires-python = ">=3.9"
 dependencies = [
-    "digitalhub-data~=0.5",
+    "digitalhub-data==0.5.0b1",
 ]
 
 [tool.setuptools.packages.find]
 exclude = ["modules*"]
 
 [tool.bumpver]
-current_version = "0.5.0b0"
+current_version = "0.5.0b1"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = false
 tag             = false
 push            = false
 
 [tool.bumpver.file_patterns]
```

