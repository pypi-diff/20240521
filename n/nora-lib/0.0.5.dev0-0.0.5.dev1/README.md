# Comparing `tmp/nora_lib-0.0.5.dev0.tar.gz` & `tmp/nora_lib-0.0.5.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nora_lib-0.0.5.dev0.tar", last modified: Mon May 20 21:13:04 2024, max compression
+gzip compressed data, was "nora_lib-0.0.5.dev1.tar", last modified: Mon May 20 22:28:55 2024, max compression
```

## Comparing `nora_lib-0.0.5.dev0.tar` & `nora_lib-0.0.5.dev1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-20 21:13:04.261158 nora_lib-0.0.5.dev0/
--rw-r--r--   0 stefanc    (502) staff       (20)      412 2024-05-20 21:13:04.260002 nora_lib-0.0.5.dev0/PKG-INFO
--rw-r--r--   0 stefanc    (502) staff       (20)      887 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev0/README.md
-drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-20 21:13:04.243296 nora_lib-0.0.5.dev0/nora_lib/
--rw-r--r--   0 stefanc    (502) staff       (20)        0 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev0/nora_lib/__init__.py
-drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-20 21:13:04.248623 nora_lib-0.0.5.dev0/nora_lib/context/
--rw-r--r--   0 stefanc    (502) staff       (20)        0 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev0/nora_lib/context/__init__.py
--rw-r--r--   0 stefanc    (502) staff       (20)     1338 2024-05-17 21:59:16.000000 nora_lib-0.0.5.dev0/nora_lib/context/context_service.py
--rw-r--r--   0 stefanc    (502) staff       (20)      356 2024-05-17 21:59:16.000000 nora_lib-0.0.5.dev0/nora_lib/context/models.py
-drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-20 21:13:04.251074 nora_lib-0.0.5.dev0/nora_lib/interactions/
--rw-r--r--   0 stefanc    (502) staff       (20)        0 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev0/nora_lib/interactions/__init__.py
--rw-r--r--   0 stefanc    (502) staff       (20)     5133 2024-05-20 21:12:03.000000 nora_lib-0.0.5.dev0/nora_lib/interactions/interactions_service.py
--rw-r--r--   0 stefanc    (502) staff       (20)     4196 2024-05-20 21:09:30.000000 nora_lib-0.0.5.dev0/nora_lib/interactions/models.py
--rw-r--r--   0 stefanc    (502) staff       (20)        0 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev0/nora_lib/py.typed
-drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-20 21:13:04.253691 nora_lib-0.0.5.dev0/nora_lib/tasks/
--rw-r--r--   0 stefanc    (502) staff       (20)        0 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev0/nora_lib/tasks/__init__.py
--rw-r--r--   0 stefanc    (502) staff       (20)      925 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev0/nora_lib/tasks/models.py
--rw-r--r--   0 stefanc    (502) staff       (20)     1793 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev0/nora_lib/tasks/state.py
-drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-20 21:13:04.257581 nora_lib-0.0.5.dev0/nora_lib.egg-info/
--rw-r--r--   0 stefanc    (502) staff       (20)      412 2024-05-20 21:13:04.000000 nora_lib-0.0.5.dev0/nora_lib.egg-info/PKG-INFO
--rw-r--r--   0 stefanc    (502) staff       (20)      587 2024-05-20 21:13:04.000000 nora_lib-0.0.5.dev0/nora_lib.egg-info/SOURCES.txt
--rw-r--r--   0 stefanc    (502) staff       (20)        1 2024-05-20 21:13:04.000000 nora_lib-0.0.5.dev0/nora_lib.egg-info/dependency_links.txt
--rw-r--r--   0 stefanc    (502) staff       (20)       64 2024-05-20 21:13:04.000000 nora_lib-0.0.5.dev0/nora_lib.egg-info/requires.txt
--rw-r--r--   0 stefanc    (502) staff       (20)       15 2024-05-20 21:13:04.000000 nora_lib-0.0.5.dev0/nora_lib.egg-info/top_level.txt
--rw-r--r--   0 stefanc    (502) staff       (20)       90 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev0/pyproject.toml
--rw-r--r--   0 stefanc    (502) staff       (20)       38 2024-05-20 21:13:04.261384 nora_lib-0.0.5.dev0/setup.cfg
--rw-r--r--   0 stefanc    (502) staff       (20)      605 2024-05-20 21:09:30.000000 nora_lib-0.0.5.dev0/setup.py
-drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-20 21:13:04.254789 nora_lib-0.0.5.dev0/tests/
-drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-20 21:13:04.256176 nora_lib-0.0.5.dev0/tests/tasks/
--rw-r--r--   0 stefanc    (502) staff       (20)        0 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev0/tests/tasks/__init__.py
--rw-r--r--   0 stefanc    (502) staff       (20)     2670 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev0/tests/tasks/test_state.py
--rw-r--r--   0 stefanc    (502) staff       (20)      123 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev0/tests/test_placeholder.py
+drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-20 22:28:55.571784 nora_lib-0.0.5.dev1/
+-rw-r--r--   0 stefanc    (502) staff       (20)      412 2024-05-20 22:28:55.571366 nora_lib-0.0.5.dev1/PKG-INFO
+-rw-r--r--   0 stefanc    (502) staff       (20)      887 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev1/README.md
+drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-20 22:28:55.559666 nora_lib-0.0.5.dev1/nora_lib/
+-rw-r--r--   0 stefanc    (502) staff       (20)        0 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev1/nora_lib/__init__.py
+drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-20 22:28:55.564235 nora_lib-0.0.5.dev1/nora_lib/context/
+-rw-r--r--   0 stefanc    (502) staff       (20)        0 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev1/nora_lib/context/__init__.py
+-rw-r--r--   0 stefanc    (502) staff       (20)     1338 2024-05-17 21:59:16.000000 nora_lib-0.0.5.dev1/nora_lib/context/context_service.py
+-rw-r--r--   0 stefanc    (502) staff       (20)      356 2024-05-17 21:59:16.000000 nora_lib-0.0.5.dev1/nora_lib/context/models.py
+drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-20 22:28:55.566083 nora_lib-0.0.5.dev1/nora_lib/interactions/
+-rw-r--r--   0 stefanc    (502) staff       (20)        0 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev1/nora_lib/interactions/__init__.py
+-rw-r--r--   0 stefanc    (502) staff       (20)     8240 2024-05-20 22:22:24.000000 nora_lib-0.0.5.dev1/nora_lib/interactions/interactions_service.py
+-rw-r--r--   0 stefanc    (502) staff       (20)     4362 2024-05-20 22:27:32.000000 nora_lib-0.0.5.dev1/nora_lib/interactions/models.py
+-rw-r--r--   0 stefanc    (502) staff       (20)        0 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev1/nora_lib/py.typed
+drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-20 22:28:55.567734 nora_lib-0.0.5.dev1/nora_lib/tasks/
+-rw-r--r--   0 stefanc    (502) staff       (20)        0 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev1/nora_lib/tasks/__init__.py
+-rw-r--r--   0 stefanc    (502) staff       (20)      925 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev1/nora_lib/tasks/models.py
+-rw-r--r--   0 stefanc    (502) staff       (20)     1793 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev1/nora_lib/tasks/state.py
+drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-20 22:28:55.570340 nora_lib-0.0.5.dev1/nora_lib.egg-info/
+-rw-r--r--   0 stefanc    (502) staff       (20)      412 2024-05-20 22:28:55.000000 nora_lib-0.0.5.dev1/nora_lib.egg-info/PKG-INFO
+-rw-r--r--   0 stefanc    (502) staff       (20)      587 2024-05-20 22:28:55.000000 nora_lib-0.0.5.dev1/nora_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 stefanc    (502) staff       (20)        1 2024-05-20 22:28:55.000000 nora_lib-0.0.5.dev1/nora_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 stefanc    (502) staff       (20)       64 2024-05-20 22:28:55.000000 nora_lib-0.0.5.dev1/nora_lib.egg-info/requires.txt
+-rw-r--r--   0 stefanc    (502) staff       (20)       15 2024-05-20 22:28:55.000000 nora_lib-0.0.5.dev1/nora_lib.egg-info/top_level.txt
+-rw-r--r--   0 stefanc    (502) staff       (20)       90 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev1/pyproject.toml
+-rw-r--r--   0 stefanc    (502) staff       (20)       38 2024-05-20 22:28:55.571870 nora_lib-0.0.5.dev1/setup.cfg
+-rw-r--r--   0 stefanc    (502) staff       (20)      605 2024-05-20 22:07:18.000000 nora_lib-0.0.5.dev1/setup.py
+drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-20 22:28:55.568556 nora_lib-0.0.5.dev1/tests/
+drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-20 22:28:55.569524 nora_lib-0.0.5.dev1/tests/tasks/
+-rw-r--r--   0 stefanc    (502) staff       (20)        0 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev1/tests/tasks/__init__.py
+-rw-r--r--   0 stefanc    (502) staff       (20)     2670 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev1/tests/tasks/test_state.py
+-rw-r--r--   0 stefanc    (502) staff       (20)      123 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev1/tests/test_placeholder.py
```

### Comparing `nora_lib-0.0.5.dev0/README.md` & `nora_lib-0.0.5.dev1/README.md`

 * *Files identical despite different names*

### Comparing `nora_lib-0.0.5.dev0/nora_lib/context/context_service.py` & `nora_lib-0.0.5.dev1/nora_lib/context/context_service.py`

 * *Files identical despite different names*

### Comparing `nora_lib-0.0.5.dev0/nora_lib/interactions/models.py` & `nora_lib-0.0.5.dev1/nora_lib/interactions/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
     type: str
     actor_id: UUID = Field(
         description="identifies actor writing the event to the interaction service"
     )
     timestamp: datetime
     text: Optional[str] = None
-    data: Optional[dict] = Field(default_factory=dict)
+    data: dict = Field(default_factory=dict)
     message_id: Optional[str] = None
     thread_id: Optional[str] = None
     channel_id: Optional[str] = None
 
     @field_serializer("actor_id")
     def serialize_actor_id(self, actor_id: UUID):
         return str(actor_id)
@@ -78,15 +78,18 @@
     """Message format returned by interaction service"""
 
     message_id: str
     actor_id: str
     text: str
     ts: str
     annotated_text: Optional[str] = None
-    events: Optional[List[dict]] = None
+    events: List[Event] = Field(default_factory=list)
+    thread_id: Optional[str] = None
+    channel_id: Optional[str] = None
+    annotations: Optional[List[Annotation]] = None
 
 
 class AgentMessageData(BaseModel):
     """capture requests to and responses from tools within Events"""
 
     message_data: dict  # dict of agent/tool request/response format
     data_sender_actor_id: Optional[str] = None  # agent sending the data
@@ -121,18 +124,20 @@
     previous_message_id: str
 
 
 class ThreadRelationsResponse(BaseModel):
     """Thread format returned by interaction service for thread relations in a search response"""
 
     thread_id: str
-    events: Optional[List[Event]] = None  # events associated only with the thread
-    messages: Optional[List[ReturnedMessage]] = (
-        None  # includes events associated with each message
-    )
+    events: List[Event] = Field(
+        default_factory=list
+    )  # events associated only with the thread
+    messages: List[ReturnedMessage] = Field(
+        default_factory=list
+    )  # includes events associated with each message
 
 
 def thread_message_lookup_request(message_id: str, event_type: str) -> dict:
     """retrieve messages and events for the thread associated with a message"""
     return {
         "id": message_id,
         "relations": {
```

### Comparing `nora_lib-0.0.5.dev0/nora_lib/tasks/models.py` & `nora_lib-0.0.5.dev1/nora_lib/tasks/models.py`

 * *Files identical despite different names*

### Comparing `nora_lib-0.0.5.dev0/nora_lib/tasks/state.py` & `nora_lib-0.0.5.dev1/nora_lib/tasks/state.py`

 * *Files identical despite different names*

### Comparing `nora_lib-0.0.5.dev0/nora_lib.egg-info/SOURCES.txt` & `nora_lib-0.0.5.dev1/nora_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nora_lib-0.0.5.dev0/setup.py` & `nora_lib-0.0.5.dev1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 runtime_requirements = ["pydantic>=2,<3", "requests"]
 
 # For running tests, linting, etc
 dev_requirements = ["mypy", "pytest", "black", "types-requests"]
 
 setuptools.setup(
     name="nora_lib",
-    version="0.0.5.dev0",
+    version="0.0.5.dev1",
     description="For making and coordinating agents and tools",
     url="https://github.com/allenai/nora_lib",
     packages=setuptools.find_packages(exclude=(["tests"])),
     install_requires=runtime_requirements,
     package_data={
         "nora_lib": ["py.typed"],
     },
```

### Comparing `nora_lib-0.0.5.dev0/tests/tasks/test_state.py` & `nora_lib-0.0.5.dev1/tests/tasks/test_state.py`

 * *Files identical despite different names*

