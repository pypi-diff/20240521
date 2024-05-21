# Comparing `tmp/composio_openai-0.2.60.tar.gz` & `tmp/composio_openai-0.2.61.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_openai-0.2.60.tar", last modified: Tue May 14 10:58:49 2024, max compression
+gzip compressed data, was "composio_openai-0.2.61.tar", last modified: Tue May 21 20:13:27 2024, max compression
```

## Comparing `composio_openai-0.2.60.tar` & `composio_openai-0.2.61.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 sawradip   (501) staff       (20)        0 2024-05-14 10:58:49.871009 composio_openai-0.2.60/
--rw-r--r--   0 sawradip   (501) staff       (20)     2615 2024-05-14 10:58:49.870779 composio_openai-0.2.60/PKG-INFO
--rw-r--r--   0 sawradip   (501) staff       (20)     2107 2024-05-02 07:57:45.000000 composio_openai-0.2.60/README.md
-drwxr-xr-x   0 sawradip   (501) staff       (20)        0 2024-05-14 10:58:49.869200 composio_openai-0.2.60/composio_openai/
--rw-r--r--   0 sawradip   (501) staff       (20)      182 2024-05-02 07:57:45.000000 composio_openai-0.2.60/composio_openai/__init__.py
--rw-r--r--   0 sawradip   (501) staff       (20)     5625 2024-05-14 10:37:23.000000 composio_openai-0.2.60/composio_openai/openai_toolspec.py
-drwxr-xr-x   0 sawradip   (501) staff       (20)        0 2024-05-14 10:58:49.870468 composio_openai-0.2.60/composio_openai.egg-info/
--rw-r--r--   0 sawradip   (501) staff       (20)     2615 2024-05-14 10:58:49.000000 composio_openai-0.2.60/composio_openai.egg-info/PKG-INFO
--rw-r--r--   0 sawradip   (501) staff       (20)      275 2024-05-14 10:58:49.000000 composio_openai-0.2.60/composio_openai.egg-info/SOURCES.txt
--rw-r--r--   0 sawradip   (501) staff       (20)        1 2024-05-14 10:58:49.000000 composio_openai-0.2.60/composio_openai.egg-info/dependency_links.txt
--rw-r--r--   0 sawradip   (501) staff       (20)       23 2024-05-14 10:58:49.000000 composio_openai-0.2.60/composio_openai.egg-info/requires.txt
--rw-r--r--   0 sawradip   (501) staff       (20)       16 2024-05-14 10:58:49.000000 composio_openai-0.2.60/composio_openai.egg-info/top_level.txt
--rw-r--r--   0 sawradip   (501) staff       (20)       38 2024-05-14 10:58:49.871058 composio_openai-0.2.60/setup.cfg
--rw-r--r--   0 sawradip   (501) staff       (20)      825 2024-05-14 10:58:34.000000 composio_openai-0.2.60/setup.py
+drwxr-xr-x   0 sawradip   (501) staff       (20)        0 2024-05-21 20:13:27.728754 composio_openai-0.2.61/
+-rw-r--r--   0 sawradip   (501) staff       (20)     2615 2024-05-21 20:13:27.728551 composio_openai-0.2.61/PKG-INFO
+-rw-r--r--   0 sawradip   (501) staff       (20)     2107 2024-05-02 07:57:45.000000 composio_openai-0.2.61/README.md
+drwxr-xr-x   0 sawradip   (501) staff       (20)        0 2024-05-21 20:13:27.727485 composio_openai-0.2.61/composio_openai/
+-rw-r--r--   0 sawradip   (501) staff       (20)      213 2024-05-20 14:09:13.000000 composio_openai-0.2.61/composio_openai/__init__.py
+-rw-r--r--   0 sawradip   (501) staff       (20)     5403 2024-05-21 20:07:08.000000 composio_openai-0.2.61/composio_openai/openai_toolspec.py
+drwxr-xr-x   0 sawradip   (501) staff       (20)        0 2024-05-21 20:13:27.728309 composio_openai-0.2.61/composio_openai.egg-info/
+-rw-r--r--   0 sawradip   (501) staff       (20)     2615 2024-05-21 20:13:27.000000 composio_openai-0.2.61/composio_openai.egg-info/PKG-INFO
+-rw-r--r--   0 sawradip   (501) staff       (20)      275 2024-05-21 20:13:27.000000 composio_openai-0.2.61/composio_openai.egg-info/SOURCES.txt
+-rw-r--r--   0 sawradip   (501) staff       (20)        1 2024-05-21 20:13:27.000000 composio_openai-0.2.61/composio_openai.egg-info/dependency_links.txt
+-rw-r--r--   0 sawradip   (501) staff       (20)       23 2024-05-21 20:13:27.000000 composio_openai-0.2.61/composio_openai.egg-info/requires.txt
+-rw-r--r--   0 sawradip   (501) staff       (20)       16 2024-05-21 20:13:27.000000 composio_openai-0.2.61/composio_openai.egg-info/top_level.txt
+-rw-r--r--   0 sawradip   (501) staff       (20)       38 2024-05-21 20:13:27.728793 composio_openai-0.2.61/setup.cfg
+-rw-r--r--   0 sawradip   (501) staff       (20)      811 2024-05-21 20:12:30.000000 composio_openai-0.2.61/setup.py
```

### Comparing `composio_openai-0.2.60/PKG-INFO` & `composio_openai-0.2.61/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_openai
-Version: 0.2.60
+Version: 0.2.61
 Summary: Use Composio to get an array of tools with your OpenAI Function Call.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9,<4
 Description-Content-Type: text/markdown
-Requires-Dist: composio_core===0.2.60
+Requires-Dist: composio_core===0.2.61
 
 ## 🚀🔗 Leveraging OpenAI with Composio
 
 Facilitate the integration of OpenAI with Composio to empower OpenAI models to directly interact with external applications, broadening their capabilities and application scope.
 
 ### Objective
```

### Comparing `composio_openai-0.2.60/README.md` & `composio_openai-0.2.61/README.md`

 * *Files identical despite different names*

### Comparing `composio_openai-0.2.60/composio_openai/openai_toolspec.py` & `composio_openai-0.2.61/composio_openai/openai_toolspec.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,89 +1,92 @@
-import hashlib
+import json
 import logging
 import os
-import json
-import types
 import time
-from inspect import Signature
 from typing import List, Union
+
 from openai import Client
 from openai.types.beta import thread
 from openai.types.beta.threads import run
 from openai.types.chat.chat_completion import ChatCompletion
 
-from composio.sdk import format_schema, SchemaFormat
 from composio import Action, App, ComposioCore, FrameworkEnum, Tag
+from composio.sdk import SchemaFormat, format_schema
+
 
 logger = logging.getLogger(__name__)
 
 
 class OpenaiStyleToolsetBase:
-    def __init__(self, framework, entity_id: str = "default", schema_format = SchemaFormat.OPENAI):
+    def __init__(
+        self, framework, entity_id: str = "default", schema_format=SchemaFormat.OPENAI
+    ):
         self.entity_id = entity_id
         self.client = ComposioCore(
-                            framework=framework, api_key=os.environ.get("COMPOSIO_API_KEY")
-                            )
+            framework=framework, api_key=os.environ.get("COMPOSIO_API_KEY")
+        )
         self.schema_format = schema_format
 
     def finalize_entity_id(self, entity_id):
-        if self.entity_id != "default" and entity_id != "default" and self.entity_id != entity_id:
-            raise ValueError("Seperate `entity_id` can not be provided during intialization and handelling tool calls")
-        elif self.entity_id != "default" :
+        if (
+            self.entity_id != "default"
+            and entity_id != "default"
+            and self.entity_id != entity_id
+        ):
+            raise ValueError(
+                "Seperate `entity_id` can not be provided during intialization and handelling tool calls"
+            )
+        elif self.entity_id != "default":
             entity_id = self.entity_id
         return entity_id
 
     def get_actions(self, actions: Union[Action, List[Action]]):
         if isinstance(actions, Action):
             actions = [actions]
-        
+
         action_schemas = self.client.sdk.get_list_of_actions(actions=actions)
-        
-        formatted_schemas = [format_schema(action_schema, 
-                                           format=self.schema_format) for action_schema in action_schemas]
+
+        formatted_schemas = [
+            format_schema(action_schema, format=self.schema_format)
+            for action_schema in action_schemas
+        ]
         return formatted_schemas
-    
-    def get_tools(self, 
-        tools: Union[App, List[App]],
-        tags: List[Union[str, Tag]] = None):
 
+    def get_tools(
+        self, tools: Union[App, List[App]], tags: List[Union[str, Tag]] = None
+    ):
         if isinstance(tools, App):
             tools = [tools]
-        
-        action_schemas = self.client.sdk.get_list_of_actions(apps=tools, 
-                                                             tags=tags)
-        formatted_schemas = [format_schema(action_schema, 
-                                           format=self.schema_format) for action_schema in action_schemas]
+
+        action_schemas = self.client.sdk.get_list_of_actions(apps=tools, tags=tags)
+        formatted_schemas = [
+            format_schema(action_schema, format=self.schema_format)
+            for action_schema in action_schemas
+        ]
         return formatted_schemas
-    
-        
+
+
 class ComposioToolset(OpenaiStyleToolsetBase):
     def __init__(self, *args, framework=FrameworkEnum.OPENAI, **kwargs):
         super().__init__(*args, framework=framework, **kwargs)
 
-
     def execute_tool_call(self, tool_call, entity_id):
         action_name_to_execute = tool_call.function.name
         action = self.client.sdk.get_action_enum_without_tool(
             action_name=action_name_to_execute
         )
         arguments = json.loads(tool_call.function.arguments)
         tool_response = self.client.execute_action(
-            action=action,
-            params=arguments,
-            entity_id=entity_id
+            action=action, params=arguments, entity_id=entity_id
         )
         return tool_response
 
-
-    def handle_tool_calls(self,
-                          llm_response: ChatCompletion, 
-                          entity_id: str = "default") -> list[any]:
-          
-
+    def handle_tool_calls(
+        self, llm_response: ChatCompletion, entity_id: str = "default"
+    ) -> list[any]:
         outputs = []
         entity_id = self.finalize_entity_id(entity_id)
 
         try:
             if llm_response.choices:
                 for choice in llm_response.choices:
                     if choice.message.tool_calls:
@@ -91,30 +94,36 @@
                             tool_response = self.execute_tool_call(tool_call, entity_id)
                             outputs.append(tool_response)
 
         except Exception as e:
             raise e from e
 
         return outputs
-    
 
-    def handle_assistant_tool_calls(self, 
-                                    run_object,
-                                    entity_id: str = "default") -> list[any]:
-
-        if self.entity_id != "default" and entity_id != "default" and self.entity_id != entity_id:
-            raise ValueError("Seperate `entity_id` can not be provided during intialization and handelling tool calls")
-        elif self.entity_id != "default" :
+    def handle_assistant_tool_calls(
+        self, run_object, entity_id: str = "default"
+    ) -> list[any]:
+        if (
+            self.entity_id != "default"
+            and entity_id != "default"
+            and self.entity_id != entity_id
+        ):
+            raise ValueError(
+                "Seperate `entity_id` can not be provided during intialization and handelling tool calls"
+            )
+        elif self.entity_id != "default":
             entity_id = self.entity_id
 
-
-        tool_calls = run_object["required_action"]['submit_tool_outputs']["tool_calls"]
+        # run_json = run_object.json()
+        # print(run_object)
+        # print(type(run_json))
+        tool_calls = run_object.required_action.submit_tool_outputs.tool_calls
         tool_outputs = []
+        
         for tool_call in tool_calls:
-            # tool_call_id = tool_call.pop("id")
             tool_response = self.execute_tool_call(tool_call, entity_id)
             tool_output = {
                 "tool_call_id": tool_call.id,
                 "output": json.dumps(tool_response),
             }
             tool_outputs.append(tool_output)
         return tool_outputs
@@ -127,28 +136,27 @@
         verbose: bool = False,
     ):
         run_object = run
         thread_object = thread
         while run_object.status in ("queued", "in_progress", "requires_action"):
             # Look here
             if run_object.status == "requires_action":
-                # print(run_object)
-                # print("***&*&*&*&S")
                 run_object = client.beta.threads.runs.submit_tool_outputs(
                     thread_id=thread_object.id,
                     run_id=run_object.id,
-                    tool_outputs=self.handle_assistant_tool_calls(run_object)
+                    tool_outputs=self.handle_assistant_tool_calls(run_object),
                 )
             else:
                 run_object = client.beta.threads.runs.retrieve(
                     thread_id=thread_object.id,
                     run_id=run_object.id,
                 )
                 time.sleep(0.5)
         return run_object
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     from pprint import pprint
-    
+
     toolset = ComposioToolset()
     out = toolset.get_tools(tools=App.GITHUB)
     pprint(out)
```

### Comparing `composio_openai-0.2.60/composio_openai.egg-info/PKG-INFO` & `composio_openai-0.2.61/composio_openai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_openai
-Version: 0.2.60
+Version: 0.2.61
 Summary: Use Composio to get an array of tools with your OpenAI Function Call.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9,<4
 Description-Content-Type: text/markdown
-Requires-Dist: composio_core===0.2.60
+Requires-Dist: composio_core===0.2.61
 
 ## 🚀🔗 Leveraging OpenAI with Composio
 
 Facilitate the integration of OpenAI with Composio to empower OpenAI models to directly interact with external applications, broadening their capabilities and application scope.
 
 ### Objective
```

### Comparing `composio_openai-0.2.60/setup.py` & `composio_openai-0.2.61/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,25 +5,23 @@
 from pathlib import Path
 
 from setuptools import setup
 
 
 setup(
     name="composio_openai",
-    version="0.2.60",
+    version="0.2.61",
     author="Sawradip",
     author_email="sawradip@composio.dev",
     description="Use Composio to get an array of tools with your OpenAI Function Call.",
     long_description=(Path(__file__).parent / "README.md").read_text(encoding="utf-8"),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.9,<4",
-    install_requires=[
-        "composio_core===0.2.60"
-    ],
+    install_requires=["composio_core===0.2.61"],
     include_package_data=True,
 )
```

