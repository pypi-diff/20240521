# Comparing `tmp/nora_lib-0.0.5.dev2.tar.gz` & `tmp/nora_lib-0.0.5.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nora_lib-0.0.5.dev2.tar", last modified: Mon May 20 22:44:00 2024, max compression
+gzip compressed data, was "nora_lib-0.0.5.dev3.tar", last modified: Mon May 20 23:36:20 2024, max compression
```

## Comparing `nora_lib-0.0.5.dev2.tar` & `nora_lib-0.0.5.dev3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-20 22:44:00.315553 nora_lib-0.0.5.dev2/
--rw-r--r--   0 stefanc    (502) staff       (20)      412 2024-05-20 22:44:00.314954 nora_lib-0.0.5.dev2/PKG-INFO
--rw-r--r--   0 stefanc    (502) staff       (20)      887 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev2/README.md
-drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-20 22:44:00.302309 nora_lib-0.0.5.dev2/nora_lib/
--rw-r--r--   0 stefanc    (502) staff       (20)        0 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev2/nora_lib/__init__.py
-drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-20 22:44:00.306437 nora_lib-0.0.5.dev2/nora_lib/context/
--rw-r--r--   0 stefanc    (502) staff       (20)        0 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev2/nora_lib/context/__init__.py
--rw-r--r--   0 stefanc    (502) staff       (20)     1338 2024-05-17 21:59:16.000000 nora_lib-0.0.5.dev2/nora_lib/context/context_service.py
--rw-r--r--   0 stefanc    (502) staff       (20)      356 2024-05-17 21:59:16.000000 nora_lib-0.0.5.dev2/nora_lib/context/models.py
-drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-20 22:44:00.308104 nora_lib-0.0.5.dev2/nora_lib/interactions/
--rw-r--r--   0 stefanc    (502) staff       (20)        0 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev2/nora_lib/interactions/__init__.py
--rw-r--r--   0 stefanc    (502) staff       (20)     8680 2024-05-20 22:42:40.000000 nora_lib-0.0.5.dev2/nora_lib/interactions/interactions_service.py
--rw-r--r--   0 stefanc    (502) staff       (20)     4585 2024-05-20 22:41:44.000000 nora_lib-0.0.5.dev2/nora_lib/interactions/models.py
--rw-r--r--   0 stefanc    (502) staff       (20)        0 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev2/nora_lib/py.typed
-drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-20 22:44:00.310050 nora_lib-0.0.5.dev2/nora_lib/tasks/
--rw-r--r--   0 stefanc    (502) staff       (20)        0 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev2/nora_lib/tasks/__init__.py
--rw-r--r--   0 stefanc    (502) staff       (20)      925 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev2/nora_lib/tasks/models.py
--rw-r--r--   0 stefanc    (502) staff       (20)     1793 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev2/nora_lib/tasks/state.py
-drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-20 22:44:00.313071 nora_lib-0.0.5.dev2/nora_lib.egg-info/
--rw-r--r--   0 stefanc    (502) staff       (20)      412 2024-05-20 22:44:00.000000 nora_lib-0.0.5.dev2/nora_lib.egg-info/PKG-INFO
--rw-r--r--   0 stefanc    (502) staff       (20)      587 2024-05-20 22:44:00.000000 nora_lib-0.0.5.dev2/nora_lib.egg-info/SOURCES.txt
--rw-r--r--   0 stefanc    (502) staff       (20)        1 2024-05-20 22:44:00.000000 nora_lib-0.0.5.dev2/nora_lib.egg-info/dependency_links.txt
--rw-r--r--   0 stefanc    (502) staff       (20)       64 2024-05-20 22:44:00.000000 nora_lib-0.0.5.dev2/nora_lib.egg-info/requires.txt
--rw-r--r--   0 stefanc    (502) staff       (20)       15 2024-05-20 22:44:00.000000 nora_lib-0.0.5.dev2/nora_lib.egg-info/top_level.txt
--rw-r--r--   0 stefanc    (502) staff       (20)       90 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev2/pyproject.toml
--rw-r--r--   0 stefanc    (502) staff       (20)       38 2024-05-20 22:44:00.315782 nora_lib-0.0.5.dev2/setup.cfg
--rw-r--r--   0 stefanc    (502) staff       (20)      605 2024-05-20 22:31:51.000000 nora_lib-0.0.5.dev2/setup.py
-drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-20 22:44:00.310959 nora_lib-0.0.5.dev2/tests/
-drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-20 22:44:00.311944 nora_lib-0.0.5.dev2/tests/tasks/
--rw-r--r--   0 stefanc    (502) staff       (20)        0 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev2/tests/tasks/__init__.py
--rw-r--r--   0 stefanc    (502) staff       (20)     2670 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev2/tests/tasks/test_state.py
--rw-r--r--   0 stefanc    (502) staff       (20)      123 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev2/tests/test_placeholder.py
+drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-20 23:36:20.480638 nora_lib-0.0.5.dev3/
+-rw-r--r--   0 stefanc    (502) staff       (20)      412 2024-05-20 23:36:20.480174 nora_lib-0.0.5.dev3/PKG-INFO
+-rw-r--r--   0 stefanc    (502) staff       (20)      887 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev3/README.md
+drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-20 23:36:20.469108 nora_lib-0.0.5.dev3/nora_lib/
+-rw-r--r--   0 stefanc    (502) staff       (20)        0 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev3/nora_lib/__init__.py
+drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-20 23:36:20.472757 nora_lib-0.0.5.dev3/nora_lib/context/
+-rw-r--r--   0 stefanc    (502) staff       (20)        0 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev3/nora_lib/context/__init__.py
+-rw-r--r--   0 stefanc    (502) staff       (20)     1338 2024-05-17 21:59:16.000000 nora_lib-0.0.5.dev3/nora_lib/context/context_service.py
+-rw-r--r--   0 stefanc    (502) staff       (20)      356 2024-05-17 21:59:16.000000 nora_lib-0.0.5.dev3/nora_lib/context/models.py
+drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-20 23:36:20.474534 nora_lib-0.0.5.dev3/nora_lib/interactions/
+-rw-r--r--   0 stefanc    (502) staff       (20)        0 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev3/nora_lib/interactions/__init__.py
+-rw-r--r--   0 stefanc    (502) staff       (20)     8656 2024-05-20 23:35:45.000000 nora_lib-0.0.5.dev3/nora_lib/interactions/interactions_service.py
+-rw-r--r--   0 stefanc    (502) staff       (20)     4672 2024-05-20 23:33:58.000000 nora_lib-0.0.5.dev3/nora_lib/interactions/models.py
+-rw-r--r--   0 stefanc    (502) staff       (20)        0 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev3/nora_lib/py.typed
+drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-20 23:36:20.476363 nora_lib-0.0.5.dev3/nora_lib/tasks/
+-rw-r--r--   0 stefanc    (502) staff       (20)        0 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev3/nora_lib/tasks/__init__.py
+-rw-r--r--   0 stefanc    (502) staff       (20)      925 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev3/nora_lib/tasks/models.py
+-rw-r--r--   0 stefanc    (502) staff       (20)     1793 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev3/nora_lib/tasks/state.py
+drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-20 23:36:20.479012 nora_lib-0.0.5.dev3/nora_lib.egg-info/
+-rw-r--r--   0 stefanc    (502) staff       (20)      412 2024-05-20 23:36:20.000000 nora_lib-0.0.5.dev3/nora_lib.egg-info/PKG-INFO
+-rw-r--r--   0 stefanc    (502) staff       (20)      587 2024-05-20 23:36:20.000000 nora_lib-0.0.5.dev3/nora_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 stefanc    (502) staff       (20)        1 2024-05-20 23:36:20.000000 nora_lib-0.0.5.dev3/nora_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 stefanc    (502) staff       (20)       64 2024-05-20 23:36:20.000000 nora_lib-0.0.5.dev3/nora_lib.egg-info/requires.txt
+-rw-r--r--   0 stefanc    (502) staff       (20)       15 2024-05-20 23:36:20.000000 nora_lib-0.0.5.dev3/nora_lib.egg-info/top_level.txt
+-rw-r--r--   0 stefanc    (502) staff       (20)       90 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev3/pyproject.toml
+-rw-r--r--   0 stefanc    (502) staff       (20)       38 2024-05-20 23:36:20.480734 nora_lib-0.0.5.dev3/setup.cfg
+-rw-r--r--   0 stefanc    (502) staff       (20)      605 2024-05-20 23:33:58.000000 nora_lib-0.0.5.dev3/setup.py
+drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-20 23:36:20.477162 nora_lib-0.0.5.dev3/tests/
+drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-20 23:36:20.478140 nora_lib-0.0.5.dev3/tests/tasks/
+-rw-r--r--   0 stefanc    (502) staff       (20)        0 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev3/tests/tasks/__init__.py
+-rw-r--r--   0 stefanc    (502) staff       (20)     2670 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev3/tests/tasks/test_state.py
+-rw-r--r--   0 stefanc    (502) staff       (20)      123 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev3/tests/test_placeholder.py
```

### Comparing `nora_lib-0.0.5.dev2/README.md` & `nora_lib-0.0.5.dev3/README.md`

 * *Files identical despite different names*

### Comparing `nora_lib-0.0.5.dev2/nora_lib/context/context_service.py` & `nora_lib-0.0.5.dev3/nora_lib/context/context_service.py`

 * *Files identical despite different names*

### Comparing `nora_lib-0.0.5.dev2/nora_lib/interactions/interactions_service.py` & `nora_lib-0.0.5.dev3/nora_lib/interactions/interactions_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,15 +126,15 @@
         except Exception as e:  # pylint: disable=broad-except
             logging.exception(
                 "Failed to fetch forked thread messages for message %s: %s",
                 message_id,
                 e,
             )
 
-        messages_with_events.sort(key=lambda x: datetime.fromisoformat(x.ts))
+        messages_with_events.sort(key=lambda x: x.ts)
         return messages_with_events
 
     def fetch_thread_messages_and_events_for_message(
         self, message_id: str, event_types: list[str]
     ) -> ThreadRelationsResponse:
         """Fetch messages sorted by timestamp and events for agent context"""
         message_url = f"{self.base_url}/interaction/v1/search/message"
```

### Comparing `nora_lib-0.0.5.dev2/nora_lib/interactions/models.py` & `nora_lib-0.0.5.dev3/nora_lib/interactions/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,15 +54,17 @@
         return ts.isoformat()
 
 
 class EventType(str, Enum):
     """Event types for the interactions service"""
 
     AGENT_CONTEXT = "agent:message_context"
+    S2_ANNOTATION = "s2_annotation"
     THREAD_FORK = "thread_fork"
+    UI_INTERACTION = "ui_interaction"
 
 
 class Event(BaseModel):
     """event object to be sent to the interactions service; requires association with a message, thread or channel id"""
 
     type: str
     actor_id: UUID = Field(
@@ -84,17 +86,17 @@
         return timestamp.isoformat()
 
 
 class ReturnedMessage(BaseModel):
     """Message format returned by interaction service"""
 
     message_id: str
-    actor_id: str
+    actor_id: UUID
     text: str
-    ts: str
+    ts: datetime
     annotated_text: Optional[str] = None
     events: List[Event] = Field(default_factory=list)
     thread_id: Optional[str] = None
     channel_id: Optional[str] = None
     annotations: Optional[List[Annotation]] = None
 
 
@@ -107,25 +109,25 @@
     tool_call_id: Optional[str] = None  # llm-provided thread
     tool_name: Optional[str] = None  # llm identifier for tool
 
 
 class ReturnedAgentContextEvent(BaseModel):
     """Event format returned by interaction service for agent context events"""
 
-    actor_id: str  # agent that saved this context
-    timestamp: str
+    actor_id: UUID  # agent that saved this context
+    timestamp: datetime
     data: AgentMessageData
     type: str
 
 
 class ReturnedAgentContextMessage(BaseModel):
     """Message format returned by interaction service for search by thread"""
 
     message_id: str
-    actor_id: str
+    actor_id: UUID
     text: str
     ts: str
     annotated_text: Optional[str] = None
     events: Optional[List[ReturnedAgentContextEvent]] = None
 
 
 class ThreadForkEventData(BaseModel):
```

### Comparing `nora_lib-0.0.5.dev2/nora_lib/tasks/models.py` & `nora_lib-0.0.5.dev3/nora_lib/tasks/models.py`

 * *Files identical despite different names*

### Comparing `nora_lib-0.0.5.dev2/nora_lib/tasks/state.py` & `nora_lib-0.0.5.dev3/nora_lib/tasks/state.py`

 * *Files identical despite different names*

### Comparing `nora_lib-0.0.5.dev2/nora_lib.egg-info/SOURCES.txt` & `nora_lib-0.0.5.dev3/nora_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nora_lib-0.0.5.dev2/setup.py` & `nora_lib-0.0.5.dev3/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 runtime_requirements = ["pydantic>=2,<3", "requests"]
 
 # For running tests, linting, etc
 dev_requirements = ["mypy", "pytest", "black", "types-requests"]
 
 setuptools.setup(
     name="nora_lib",
-    version="0.0.5.dev2",
+    version="0.0.5.dev3",
     description="For making and coordinating agents and tools",
     url="https://github.com/allenai/nora_lib",
     packages=setuptools.find_packages(exclude=(["tests"])),
     install_requires=runtime_requirements,
     package_data={
         "nora_lib": ["py.typed"],
     },
```

### Comparing `nora_lib-0.0.5.dev2/tests/tasks/test_state.py` & `nora_lib-0.0.5.dev3/tests/tasks/test_state.py`

 * *Files identical despite different names*

