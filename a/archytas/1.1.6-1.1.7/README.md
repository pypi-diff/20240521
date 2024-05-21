# Comparing `tmp/archytas-1.1.6.tar.gz` & `tmp/archytas-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "archytas-1.1.6.tar", max compression
+gzip compressed data, was "archytas-1.1.7.tar", max compression
```

## Comparing `archytas-1.1.6.tar` & `archytas-1.1.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    32472 2024-05-13 18:12:00.873649 archytas-1.1.6/LICENSE
--rw-r--r--   0        0        0     2088 2024-05-13 18:12:00.873649 archytas-1.1.6/README.md
--rw-r--r--   0        0        0        0 2024-05-13 18:12:00.873649 archytas-1.1.6/archytas/__init__.py
--rw-r--r--   0        0        0    14651 2024-05-13 18:12:00.873649 archytas-1.1.6/archytas/agent.py
--rw-r--r--   0        0        0    10031 2024-05-13 18:12:00.873649 archytas-1.1.6/archytas/demo_tools.py
--rw-r--r--   0        0        0     4257 2024-05-13 18:12:00.873649 archytas-1.1.6/archytas/prompt.py
--rw-r--r--   0        0        0     3247 2024-05-13 18:12:00.873649 archytas-1.1.6/archytas/python.py
--rw-r--r--   0        0        0    13221 2024-05-13 18:12:00.873649 archytas-1.1.6/archytas/react.py
--rw-r--r--   0        0        0     2116 2024-05-13 18:12:00.873649 archytas-1.1.6/archytas/repl.py
--rw-r--r--   0        0        0    14435 2024-05-13 18:12:00.873649 archytas-1.1.6/archytas/tool_utils.py
--rw-r--r--   0        0        0     4560 2024-05-13 18:12:00.873649 archytas-1.1.6/archytas/tools.py
--rw-r--r--   0        0        0     1280 2024-05-13 18:12:00.873649 archytas-1.1.6/archytas/utils.py
--rw-r--r--   0        0        0      817 2024-05-13 18:12:00.905649 archytas-1.1.6/pyproject.toml
--rw-r--r--   0        0        0     2921 1970-01-01 00:00:00.000000 archytas-1.1.6/PKG-INFO
+-rw-r--r--   0        0        0    32472 2024-05-21 19:08:11.230422 archytas-1.1.7/LICENSE
+-rw-r--r--   0        0        0     2088 2024-05-21 19:08:11.230422 archytas-1.1.7/README.md
+-rw-r--r--   0        0        0        0 2024-05-21 19:08:11.230422 archytas-1.1.7/archytas/__init__.py
+-rw-r--r--   0        0        0    14651 2024-05-21 19:08:11.230422 archytas-1.1.7/archytas/agent.py
+-rw-r--r--   0        0        0    10031 2024-05-21 19:08:11.230422 archytas-1.1.7/archytas/demo_tools.py
+-rw-r--r--   0        0        0     4257 2024-05-21 19:08:11.230422 archytas-1.1.7/archytas/prompt.py
+-rw-r--r--   0        0        0     3247 2024-05-21 19:08:11.230422 archytas-1.1.7/archytas/python.py
+-rw-r--r--   0        0        0    13351 2024-05-21 19:08:11.230422 archytas-1.1.7/archytas/react.py
+-rw-r--r--   0        0        0     2116 2024-05-21 19:08:11.230422 archytas-1.1.7/archytas/repl.py
+-rw-r--r--   0        0        0    14637 2024-05-21 19:08:11.230422 archytas-1.1.7/archytas/tool_utils.py
+-rw-r--r--   0        0        0     4560 2024-05-21 19:08:11.230422 archytas-1.1.7/archytas/tools.py
+-rw-r--r--   0        0        0     1280 2024-05-21 19:08:11.230422 archytas-1.1.7/archytas/utils.py
+-rw-r--r--   0        0        0      818 2024-05-21 19:08:11.262422 archytas-1.1.7/pyproject.toml
+-rw-r--r--   0        0        0     2922 1970-01-01 00:00:00.000000 archytas-1.1.7/PKG-INFO
```

### Comparing `archytas-1.1.6/LICENSE` & `archytas-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `archytas-1.1.6/README.md` & `archytas-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `archytas-1.1.6/archytas/agent.py` & `archytas-1.1.7/archytas/agent.py`

 * *Files identical despite different names*

### Comparing `archytas-1.1.6/archytas/demo_tools.py` & `archytas-1.1.7/archytas/demo_tools.py`

 * *Files identical despite different names*

### Comparing `archytas-1.1.6/archytas/prompt.py` & `archytas-1.1.7/archytas/prompt.py`

 * *Files identical despite different names*

### Comparing `archytas-1.1.6/archytas/python.py` & `archytas-1.1.7/archytas/python.py`

 * *Files identical despite different names*

### Comparing `archytas-1.1.6/archytas/react.py` & `archytas-1.1.7/archytas/react.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from archytas.agent import Agent, Message, Role
 from archytas.prompt import build_prompt, build_all_tool_names
 from archytas.tools import ask_user
 from archytas.tool_utils import make_tool_dict
 import asyncio
+import inspect
 import json
 import pdb
 import sys
 import logging
 import typing
 
 logger = logging.Logger("archytas")
@@ -86,14 +87,15 @@
         """
 
         # create a dictionary for looking up tools by name
         tools = tools or []
         if allow_ask_user:
             tools.append(ask_user)
         tools.append(self)
+        self._raw_tools = tools
         self.tools = make_tool_dict(tools)
 
         if thought_handler is Undefined:
             self.thought_handler = self.thought_callback
         else:
             self.thought_handler = thought_handler
 
@@ -115,32 +117,35 @@
         self.errors = 0
         self.steps = 0
 
         # keep track of the last tool used (for error messages)
         self.last_tool_name = ""
 
     def update_prompt(self):
-        tool_list = list(self.tools.values())
-        self.prompt = build_prompt(tool_list)
+        self.prompt = build_prompt(self._raw_tools)
         self.system_message["content"] = self.prompt
-    
+
     def disable(self, *tool_names):
         if len(tool_names) == 0:
             return
         for tool_name in tool_names:
             if tool_name in self.tools:
-                self.tools.pop(tool_name)
+                setattr(self.tools[tool_name], '_disabled', True)
             elif "." not in tool_name:
                 matches = [name for name in self.tools.keys() if name.endswith(f".{tool_name}")]
                 if len(matches) > 1:
                     raise ValueError(f"Ambiguous name: Multiple tools called '{tool_name}'")
                 elif len(matches) == 1:
-                    self.tools.pop(matches[0])
+                    subtool_name = matches[0]
+                    method = self.tools[subtool_name]
+
+                    setattr(method.__func__, '_disabled', True)
+
         self.update_prompt()
-                
+
 
     def thought_callback(self, thought: str, tool_name: str, tool_input: str) -> None:
         if self.verbose:
             # TODO: better coloring
             self.print(
                 f"thought: {thought}\ntool: {tool_name}\ntool_input: {tool_input}\n"
             )
```

### Comparing `archytas-1.1.6/archytas/repl.py` & `archytas-1.1.7/archytas/repl.py`

 * *Files identical despite different names*

### Comparing `archytas-1.1.6/archytas/tool_utils.py` & `archytas-1.1.7/archytas/tool_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,14 +160,16 @@
 
 
 def get_prompt_description(obj: Callable | type | Any):
 
     # get the list of arguments
     chunks = []
     tab = "    "
+    if getattr(obj, '_disabled', False):
+        return ""
 
     if inspect.isfunction(obj) or inspect.ismethod(obj):
         args_list, ret, desc, injections = get_tool_signature(obj)
         args_list = args_list
         ret_name, ret_type, ret_description = ret
         short_desc, long_desc, examples = desc
 
@@ -208,15 +210,19 @@
             chunks.append("None")
         else:
             chunks.append(f"({ret_type.__name__}) {ret_description}")
 
         ############### EXAMPLES ###############
         # TODO: examples need to be parsed...
     else:
-        tool_methods = collect_tools_from_object(obj)
+        tool_methods = [
+                tool_method
+                for tool_method in collect_tools_from_object(obj)
+                if not getattr(tool_method, "_disabled", False)
+            ]
         if tool_methods:
             ############### NAME/DESCRIPTION ###############
             if inspect.isclass(obj):
                 chunks.append(f"{obj.__name__} (class):\n")
             else:
                 chunks.append(f"{obj.__class__.__name__} (class instance):\n")
             docstring = inspect.getdoc(obj)
```

### Comparing `archytas-1.1.6/archytas/tools.py` & `archytas-1.1.7/archytas/tools.py`

 * *Files identical despite different names*

### Comparing `archytas-1.1.6/archytas/utils.py` & `archytas-1.1.7/archytas/utils.py`

 * *Files identical despite different names*

### Comparing `archytas-1.1.6/pyproject.toml` & `archytas-1.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "archytas"
-version = "1.1.6"
+version = "1.1.7"
 description = "A library for pairing LLM agents with tools so they perform open ended tasks"
 authors = ["David Andrew Samson <david.andrew.engineer@gmail.com>", "Matthew Printz <matt@jataware.com>"]
 readme = "README.md"
 license = "GPL-3.0-or-later"
 
 [project.urls]
 "Homepage" = "https://github.com/jataware/archytas"
 "Bug Tracker" = "https://github.com/jataware/archytas/issues"
 
 [tool.poetry.scripts]
 chat-repl = "archytas.repl:start_repl"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-openai = "^1.3.9"
+openai = "^1.30.1"
 tenacity = "^8.2.2"
 rich = "^13.3.4"
 docstring-parser = "^0.15"
 pytz = "^2023.3"
 toml = "^0.10.2"
 frozendict = "^2.3.8"
```

### Comparing `archytas-1.1.6/PKG-INFO` & `archytas-1.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: archytas
-Version: 1.1.6
+Version: 1.1.7
 Summary: A library for pairing LLM agents with tools so they perform open ended tasks
 License: GPL-3.0-or-later
 Author: David Andrew Samson
 Author-email: david.andrew.engineer@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: docstring-parser (>=0.15,<0.16)
 Requires-Dist: frozendict (>=2.3.8,<3.0.0)
-Requires-Dist: openai (>=1.3.9,<2.0.0)
+Requires-Dist: openai (>=1.30.1,<2.0.0)
 Requires-Dist: pytz (>=2023.3,<2024.0)
 Requires-Dist: rich (>=13.3.4,<14.0.0)
 Requires-Dist: tenacity (>=8.2.2,<9.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Description-Content-Type: text/markdown
 
 # Archytas: A Tools Interface for AI Agents
```

