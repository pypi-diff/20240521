# Comparing `tmp/composio_julep-0.2.60.tar.gz` & `tmp/composio_julep-0.2.61.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_julep-0.2.60.tar", last modified: Tue May 14 10:58:45 2024, max compression
+gzip compressed data, was "composio_julep-0.2.61.tar", last modified: Tue May 21 20:13:22 2024, max compression
```

## Comparing `composio_julep-0.2.60.tar` & `composio_julep-0.2.61.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 sawradip   (501) staff       (20)        0 2024-05-14 10:58:45.138768 composio_julep-0.2.60/
--rw-r--r--   0 sawradip   (501) staff       (20)     4463 2024-05-14 10:58:45.138579 composio_julep-0.2.60/PKG-INFO
--rw-r--r--   0 sawradip   (501) staff       (20)     3933 2024-05-02 07:57:45.000000 composio_julep-0.2.60/README.md
-drwxr-xr-x   0 sawradip   (501) staff       (20)        0 2024-05-14 10:58:45.137236 composio_julep-0.2.60/composio_julep/
--rw-r--r--   0 sawradip   (501) staff       (20)      157 2024-05-02 07:57:45.000000 composio_julep-0.2.60/composio_julep/__init__.py
--rw-r--r--   0 sawradip   (501) staff       (20)     1624 2024-05-14 10:32:07.000000 composio_julep-0.2.60/composio_julep/julep_toolspec.py
-drwxr-xr-x   0 sawradip   (501) staff       (20)        0 2024-05-14 10:58:45.138325 composio_julep-0.2.60/composio_julep.egg-info/
--rw-r--r--   0 sawradip   (501) staff       (20)     4463 2024-05-14 10:58:45.000000 composio_julep-0.2.60/composio_julep.egg-info/PKG-INFO
--rw-r--r--   0 sawradip   (501) staff       (20)      267 2024-05-14 10:58:45.000000 composio_julep-0.2.60/composio_julep.egg-info/SOURCES.txt
--rw-r--r--   0 sawradip   (501) staff       (20)        1 2024-05-14 10:58:45.000000 composio_julep-0.2.60/composio_julep.egg-info/dependency_links.txt
--rw-r--r--   0 sawradip   (501) staff       (20)       38 2024-05-14 10:58:45.000000 composio_julep-0.2.60/composio_julep.egg-info/requires.txt
--rw-r--r--   0 sawradip   (501) staff       (20)       15 2024-05-14 10:58:45.000000 composio_julep-0.2.60/composio_julep.egg-info/top_level.txt
--rw-r--r--   0 sawradip   (501) staff       (20)       38 2024-05-14 10:58:45.138810 composio_julep-0.2.60/setup.cfg
--rw-r--r--   0 sawradip   (501) staff       (20)      842 2024-05-14 10:58:34.000000 composio_julep-0.2.60/setup.py
+drwxr-xr-x   0 sawradip   (501) staff       (20)        0 2024-05-21 20:13:22.055943 composio_julep-0.2.61/
+-rw-r--r--   0 sawradip   (501) staff       (20)     4458 2024-05-21 20:13:22.055748 composio_julep-0.2.61/PKG-INFO
+-rw-r--r--   0 sawradip   (501) staff       (20)     3928 2024-05-21 04:53:37.000000 composio_julep-0.2.61/README.md
+drwxr-xr-x   0 sawradip   (501) staff       (20)        0 2024-05-21 20:13:22.054668 composio_julep-0.2.61/composio_julep/
+-rw-r--r--   0 sawradip   (501) staff       (20)      158 2024-05-20 14:09:13.000000 composio_julep-0.2.61/composio_julep/__init__.py
+-rw-r--r--   0 sawradip   (501) staff       (20)     1397 2024-05-20 14:09:13.000000 composio_julep-0.2.61/composio_julep/julep_toolspec.py
+drwxr-xr-x   0 sawradip   (501) staff       (20)        0 2024-05-21 20:13:22.055463 composio_julep-0.2.61/composio_julep.egg-info/
+-rw-r--r--   0 sawradip   (501) staff       (20)     4458 2024-05-21 20:13:22.000000 composio_julep-0.2.61/composio_julep.egg-info/PKG-INFO
+-rw-r--r--   0 sawradip   (501) staff       (20)      267 2024-05-21 20:13:22.000000 composio_julep-0.2.61/composio_julep.egg-info/SOURCES.txt
+-rw-r--r--   0 sawradip   (501) staff       (20)        1 2024-05-21 20:13:22.000000 composio_julep-0.2.61/composio_julep.egg-info/dependency_links.txt
+-rw-r--r--   0 sawradip   (501) staff       (20)       38 2024-05-21 20:13:22.000000 composio_julep-0.2.61/composio_julep.egg-info/requires.txt
+-rw-r--r--   0 sawradip   (501) staff       (20)       15 2024-05-21 20:13:22.000000 composio_julep-0.2.61/composio_julep.egg-info/top_level.txt
+-rw-r--r--   0 sawradip   (501) staff       (20)       38 2024-05-21 20:13:22.055982 composio_julep-0.2.61/setup.cfg
+-rw-r--r--   0 sawradip   (501) staff       (20)      820 2024-05-21 20:12:30.000000 composio_julep-0.2.61/setup.py
```

### Comparing `composio_julep-0.2.60/PKG-INFO` & `composio_julep-0.2.61/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_julep
-Version: 0.2.60
+Version: 0.2.61
 Summary: Use Composio to get an array of tools with your Julep wokflow.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9,<4
 Description-Content-Type: text/markdown
-Requires-Dist: composio_openai===0.2.60
+Requires-Dist: composio_openai===0.2.61
 Requires-Dist: julep>=0.3.2
 
 ## 🚀🔗 Integrating Composio with Julep
 
 Streamline the integration of Composio within the Julep agentic framework to enhance the interaction capabilities of Julep agents with external applications, significantly extending their operational range and efficiency.
 
 ### Objective
@@ -22,16 +22,16 @@
 - **Facilitate the automation of starring a GitHub repository** through the use of conversational commands within the Julep framework, leveraging Composio's OpenAI Function Calls.
 
 ### Installation and Setup
 
 Ensure you have the necessary packages installed and connect your GitHub account to allow your agents to utilize GitHub functionalities.
 
 ```bash
-# Install Composio LangChain package
-pip install composio-openai
+# Install Composio Julep package
+pip install composio-julep
 
 # Connect your GitHub account
 composio-cli add github
 
 # View available applications you can connect with
 composio-cli show-apps
 ```
```

### Comparing `composio_julep-0.2.60/README.md` & `composio_julep-0.2.61/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 - **Facilitate the automation of starring a GitHub repository** through the use of conversational commands within the Julep framework, leveraging Composio's OpenAI Function Calls.
 
 ### Installation and Setup
 
 Ensure you have the necessary packages installed and connect your GitHub account to allow your agents to utilize GitHub functionalities.
 
 ```bash
-# Install Composio LangChain package
-pip install composio-openai
+# Install Composio Julep package
+pip install composio-julep
 
 # Connect your GitHub account
 composio-cli add github
 
 # View available applications you can connect with
 composio-cli show-apps
 ```
```

### Comparing `composio_julep-0.2.60/composio_julep/julep_toolspec.py` & `composio_julep-0.2.61/composio_julep/julep_toolspec.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,48 +1,45 @@
-
 import json
-from json.decoder import JSONDecoder
-from composio import FrameworkEnum
-from composio_openai import OpenaiStyleToolsetBase
 
+from composio_openai import OpenaiStyleToolsetBase
 from julep.api.types import ChatResponse
-        
+
+from composio import FrameworkEnum
+
+
 class ComposioToolset(OpenaiStyleToolsetBase):
     def __init__(self, *args, framework=FrameworkEnum.JULEP, **kwargs):
         super().__init__(*args, framework=framework, **kwargs)
-        
-    
-    def handle_tool_calls(self,
-                        llm_response: ChatResponse,
-                        entity_id: str = "default") -> list[any]:
 
+    def handle_tool_calls(
+        self, llm_response: ChatResponse, entity_id: str = "default"
+    ) -> list[any]:
         entity_id = self.finalize_entity_id(entity_id)
-        outputs = []        
+        outputs = []
 
         for responses in llm_response.response:
             for response in responses:
                 try:
                     function = json.loads(response.content)
                     action_name_to_execute = function["name"]
                     action = self.client.sdk.get_action_enum_without_tool(
                         action_name=action_name_to_execute
                     )
                     arguments = json.loads(function["arguments"])
-                    # account = entity.get_connection(app_name=action.service)
                     output = self.client.execute_action(action, arguments, entity_id)
-                    
+
                 except json.JSONDecodeError:
                     output = response.content
-                    
+
                 outputs.append(output)
 
         return outputs
-    
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     from pprint import pprint
+
     from composio import App
-    
+
     toolset = ComposioToolset()
     out = toolset.get_tools(tools=App.GITHUB)
     pprint(out)
```

### Comparing `composio_julep-0.2.60/composio_julep.egg-info/PKG-INFO` & `composio_julep-0.2.61/composio_julep.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_julep
-Version: 0.2.60
+Version: 0.2.61
 Summary: Use Composio to get an array of tools with your Julep wokflow.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9,<4
 Description-Content-Type: text/markdown
-Requires-Dist: composio_openai===0.2.60
+Requires-Dist: composio_openai===0.2.61
 Requires-Dist: julep>=0.3.2
 
 ## 🚀🔗 Integrating Composio with Julep
 
 Streamline the integration of Composio within the Julep agentic framework to enhance the interaction capabilities of Julep agents with external applications, significantly extending their operational range and efficiency.
 
 ### Objective
@@ -22,16 +22,16 @@
 - **Facilitate the automation of starring a GitHub repository** through the use of conversational commands within the Julep framework, leveraging Composio's OpenAI Function Calls.
 
 ### Installation and Setup
 
 Ensure you have the necessary packages installed and connect your GitHub account to allow your agents to utilize GitHub functionalities.
 
 ```bash
-# Install Composio LangChain package
-pip install composio-openai
+# Install Composio Julep package
+pip install composio-julep
 
 # Connect your GitHub account
 composio-cli add github
 
 # View available applications you can connect with
 composio-cli show-apps
 ```
```

### Comparing `composio_julep-0.2.60/setup.py` & `composio_julep-0.2.61/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,26 +5,23 @@
 from pathlib import Path
 
 from setuptools import setup
 
 
 setup(
     name="composio_julep",
-    version="0.2.60",
+    version="0.2.61",
     author="Sawradip",
     author_email="sawradip@composio.dev",
     description="Use Composio to get an array of tools with your Julep wokflow.",
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
-        "composio_openai===0.2.60",
-        "julep>=0.3.2"
-    ],
+    install_requires=["composio_openai===0.2.61", "julep>=0.3.2"],
     include_package_data=True,
 )
```

