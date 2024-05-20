# Comparing `tmp/nora_lib-0.0.5.dev1.tar.gz` & `tmp/nora_lib-0.0.5.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nora_lib-0.0.5.dev1.tar", last modified: Mon May 20 22:28:55 2024, max compression
+gzip compressed data, was "nora_lib-0.0.5.dev2.tar", last modified: Mon May 20 22:44:00 2024, max compression
```

## Comparing `nora_lib-0.0.5.dev1.tar` & `nora_lib-0.0.5.dev2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-20 22:28:55.571784 nora_lib-0.0.5.dev1/
--rw-r--r--   0 stefanc    (502) staff       (20)      412 2024-05-20 22:28:55.571366 nora_lib-0.0.5.dev1/PKG-INFO
--rw-r--r--   0 stefanc    (502) staff       (20)      887 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev1/README.md
-drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-20 22:28:55.559666 nora_lib-0.0.5.dev1/nora_lib/
--rw-r--r--   0 stefanc    (502) staff       (20)        0 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev1/nora_lib/__init__.py
-drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-20 22:28:55.564235 nora_lib-0.0.5.dev1/nora_lib/context/
--rw-r--r--   0 stefanc    (502) staff       (20)        0 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev1/nora_lib/context/__init__.py
--rw-r--r--   0 stefanc    (502) staff       (20)     1338 2024-05-17 21:59:16.000000 nora_lib-0.0.5.dev1/nora_lib/context/context_service.py
--rw-r--r--   0 stefanc    (502) staff       (20)      356 2024-05-17 21:59:16.000000 nora_lib-0.0.5.dev1/nora_lib/context/models.py
-drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-20 22:28:55.566083 nora_lib-0.0.5.dev1/nora_lib/interactions/
--rw-r--r--   0 stefanc    (502) staff       (20)        0 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev1/nora_lib/interactions/__init__.py
--rw-r--r--   0 stefanc    (502) staff       (20)     8240 2024-05-20 22:22:24.000000 nora_lib-0.0.5.dev1/nora_lib/interactions/interactions_service.py
--rw-r--r--   0 stefanc    (502) staff       (20)     4362 2024-05-20 22:27:32.000000 nora_lib-0.0.5.dev1/nora_lib/interactions/models.py
--rw-r--r--   0 stefanc    (502) staff       (20)        0 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev1/nora_lib/py.typed
-drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-20 22:28:55.567734 nora_lib-0.0.5.dev1/nora_lib/tasks/
--rw-r--r--   0 stefanc    (502) staff       (20)        0 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev1/nora_lib/tasks/__init__.py
--rw-r--r--   0 stefanc    (502) staff       (20)      925 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev1/nora_lib/tasks/models.py
--rw-r--r--   0 stefanc    (502) staff       (20)     1793 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev1/nora_lib/tasks/state.py
-drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-20 22:28:55.570340 nora_lib-0.0.5.dev1/nora_lib.egg-info/
--rw-r--r--   0 stefanc    (502) staff       (20)      412 2024-05-20 22:28:55.000000 nora_lib-0.0.5.dev1/nora_lib.egg-info/PKG-INFO
--rw-r--r--   0 stefanc    (502) staff       (20)      587 2024-05-20 22:28:55.000000 nora_lib-0.0.5.dev1/nora_lib.egg-info/SOURCES.txt
--rw-r--r--   0 stefanc    (502) staff       (20)        1 2024-05-20 22:28:55.000000 nora_lib-0.0.5.dev1/nora_lib.egg-info/dependency_links.txt
--rw-r--r--   0 stefanc    (502) staff       (20)       64 2024-05-20 22:28:55.000000 nora_lib-0.0.5.dev1/nora_lib.egg-info/requires.txt
--rw-r--r--   0 stefanc    (502) staff       (20)       15 2024-05-20 22:28:55.000000 nora_lib-0.0.5.dev1/nora_lib.egg-info/top_level.txt
--rw-r--r--   0 stefanc    (502) staff       (20)       90 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev1/pyproject.toml
--rw-r--r--   0 stefanc    (502) staff       (20)       38 2024-05-20 22:28:55.571870 nora_lib-0.0.5.dev1/setup.cfg
--rw-r--r--   0 stefanc    (502) staff       (20)      605 2024-05-20 22:07:18.000000 nora_lib-0.0.5.dev1/setup.py
-drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-20 22:28:55.568556 nora_lib-0.0.5.dev1/tests/
-drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-20 22:28:55.569524 nora_lib-0.0.5.dev1/tests/tasks/
--rw-r--r--   0 stefanc    (502) staff       (20)        0 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev1/tests/tasks/__init__.py
--rw-r--r--   0 stefanc    (502) staff       (20)     2670 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev1/tests/tasks/test_state.py
--rw-r--r--   0 stefanc    (502) staff       (20)      123 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev1/tests/test_placeholder.py
+drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-20 22:44:00.315553 nora_lib-0.0.5.dev2/
+-rw-r--r--   0 stefanc    (502) staff       (20)      412 2024-05-20 22:44:00.314954 nora_lib-0.0.5.dev2/PKG-INFO
+-rw-r--r--   0 stefanc    (502) staff       (20)      887 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev2/README.md
+drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-20 22:44:00.302309 nora_lib-0.0.5.dev2/nora_lib/
+-rw-r--r--   0 stefanc    (502) staff       (20)        0 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev2/nora_lib/__init__.py
+drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-20 22:44:00.306437 nora_lib-0.0.5.dev2/nora_lib/context/
+-rw-r--r--   0 stefanc    (502) staff       (20)        0 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev2/nora_lib/context/__init__.py
+-rw-r--r--   0 stefanc    (502) staff       (20)     1338 2024-05-17 21:59:16.000000 nora_lib-0.0.5.dev2/nora_lib/context/context_service.py
+-rw-r--r--   0 stefanc    (502) staff       (20)      356 2024-05-17 21:59:16.000000 nora_lib-0.0.5.dev2/nora_lib/context/models.py
+drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-20 22:44:00.308104 nora_lib-0.0.5.dev2/nora_lib/interactions/
+-rw-r--r--   0 stefanc    (502) staff       (20)        0 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev2/nora_lib/interactions/__init__.py
+-rw-r--r--   0 stefanc    (502) staff       (20)     8680 2024-05-20 22:42:40.000000 nora_lib-0.0.5.dev2/nora_lib/interactions/interactions_service.py
+-rw-r--r--   0 stefanc    (502) staff       (20)     4585 2024-05-20 22:41:44.000000 nora_lib-0.0.5.dev2/nora_lib/interactions/models.py
+-rw-r--r--   0 stefanc    (502) staff       (20)        0 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev2/nora_lib/py.typed
+drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-20 22:44:00.310050 nora_lib-0.0.5.dev2/nora_lib/tasks/
+-rw-r--r--   0 stefanc    (502) staff       (20)        0 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev2/nora_lib/tasks/__init__.py
+-rw-r--r--   0 stefanc    (502) staff       (20)      925 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev2/nora_lib/tasks/models.py
+-rw-r--r--   0 stefanc    (502) staff       (20)     1793 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev2/nora_lib/tasks/state.py
+drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-20 22:44:00.313071 nora_lib-0.0.5.dev2/nora_lib.egg-info/
+-rw-r--r--   0 stefanc    (502) staff       (20)      412 2024-05-20 22:44:00.000000 nora_lib-0.0.5.dev2/nora_lib.egg-info/PKG-INFO
+-rw-r--r--   0 stefanc    (502) staff       (20)      587 2024-05-20 22:44:00.000000 nora_lib-0.0.5.dev2/nora_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 stefanc    (502) staff       (20)        1 2024-05-20 22:44:00.000000 nora_lib-0.0.5.dev2/nora_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 stefanc    (502) staff       (20)       64 2024-05-20 22:44:00.000000 nora_lib-0.0.5.dev2/nora_lib.egg-info/requires.txt
+-rw-r--r--   0 stefanc    (502) staff       (20)       15 2024-05-20 22:44:00.000000 nora_lib-0.0.5.dev2/nora_lib.egg-info/top_level.txt
+-rw-r--r--   0 stefanc    (502) staff       (20)       90 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev2/pyproject.toml
+-rw-r--r--   0 stefanc    (502) staff       (20)       38 2024-05-20 22:44:00.315782 nora_lib-0.0.5.dev2/setup.cfg
+-rw-r--r--   0 stefanc    (502) staff       (20)      605 2024-05-20 22:31:51.000000 nora_lib-0.0.5.dev2/setup.py
+drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-20 22:44:00.310959 nora_lib-0.0.5.dev2/tests/
+drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-20 22:44:00.311944 nora_lib-0.0.5.dev2/tests/tasks/
+-rw-r--r--   0 stefanc    (502) staff       (20)        0 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev2/tests/tasks/__init__.py
+-rw-r--r--   0 stefanc    (502) staff       (20)     2670 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev2/tests/tasks/test_state.py
+-rw-r--r--   0 stefanc    (502) staff       (20)      123 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev2/tests/test_placeholder.py
```

### Comparing `nora_lib-0.0.5.dev1/README.md` & `nora_lib-0.0.5.dev2/README.md`

 * *Files identical despite different names*

### Comparing `nora_lib-0.0.5.dev1/nora_lib/context/context_service.py` & `nora_lib-0.0.5.dev2/nora_lib/context/context_service.py`

 * *Files identical despite different names*

### Comparing `nora_lib-0.0.5.dev1/nora_lib/interactions/interactions_service.py` & `nora_lib-0.0.5.dev2/nora_lib/interactions/interactions_service.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from datetime import datetime
 import logging
 import requests
 from typing import List, Optional
 
 from nora_lib.interactions.models import (
+    AnnotationBatch,
     Event,
     EventType,
     Message,
     ReturnedMessage,
     ThreadRelationsResponse,
     ThreadForkEventData,
 )
@@ -41,14 +42,25 @@
             event_url,
             json=event.model_dump(),
             headers=self.headers,
             timeout=int(self.timeout),
         )
         response.raise_for_status()
 
+    def save_annotation(self, annotation: AnnotationBatch) -> None:
+        """Save an annotation to the Interactions API"""
+        annotation_url = f"{self.base_url}/interaction/v1/annotation"
+        response = requests.post(
+            annotation_url,
+            json=annotation.model_dump(),
+            headers=self.headers,
+            timeout=int(self.timeout),
+        )
+        response.raise_for_status()
+
     def get_message(self, message_id: str) -> ReturnedMessage:
         """Fetch a message from the Interactions API"""
         message_url = f"{self.base_url}/interaction/v1/search/message"
         request_body = {
             "id": message_id,
             "relations": {"thread": {}, "channel": {}, "events": {}, "annotations": {}},
         }
```

### Comparing `nora_lib-0.0.5.dev1/nora_lib/interactions/models.py` & `nora_lib-0.0.5.dev2/nora_lib/interactions/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,14 +21,24 @@
     model_config = ConfigDict(coerce_numbers_to_str=True)
 
     tag: str
     span: Tuple[int, int]
     attributes: Optional[Dict[str, str]] = None
 
 
+class AnnotationBatch(BaseModel):
+    actor_id: UUID
+    message_id: str
+    annotations: List[Annotation]
+
+    @field_serializer("actor_id")
+    def serialize_actor_id(self, actor_id: UUID):
+        return str(actor_id)
+
+
 class Message(BaseModel):
     message_id: str
     actor_id: UUID
     text: str
     thread_id: Optional[str]
     channel_id: str
     surface: Surface
```

### Comparing `nora_lib-0.0.5.dev1/nora_lib/tasks/models.py` & `nora_lib-0.0.5.dev2/nora_lib/tasks/models.py`

 * *Files identical despite different names*

### Comparing `nora_lib-0.0.5.dev1/nora_lib/tasks/state.py` & `nora_lib-0.0.5.dev2/nora_lib/tasks/state.py`

 * *Files identical despite different names*

### Comparing `nora_lib-0.0.5.dev1/nora_lib.egg-info/SOURCES.txt` & `nora_lib-0.0.5.dev2/nora_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nora_lib-0.0.5.dev1/setup.py` & `nora_lib-0.0.5.dev2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 runtime_requirements = ["pydantic>=2,<3", "requests"]
 
 # For running tests, linting, etc
 dev_requirements = ["mypy", "pytest", "black", "types-requests"]
 
 setuptools.setup(
     name="nora_lib",
-    version="0.0.5.dev1",
+    version="0.0.5.dev2",
     description="For making and coordinating agents and tools",
     url="https://github.com/allenai/nora_lib",
     packages=setuptools.find_packages(exclude=(["tests"])),
     install_requires=runtime_requirements,
     package_data={
         "nora_lib": ["py.typed"],
     },
```

### Comparing `nora_lib-0.0.5.dev1/tests/tasks/test_state.py` & `nora_lib-0.0.5.dev2/tests/tasks/test_state.py`

 * *Files identical despite different names*

