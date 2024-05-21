# Comparing `tmp/stencila_plugin-2.0.0a30.tar.gz` & `tmp/stencila_plugin-2.0.0a31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stencila_plugin-2.0.0a30.tar", last modified: Tue May 21 01:57:31 2024, max compression
+gzip compressed data, was "stencila_plugin-2.0.0a31.tar", last modified: Tue May 21 03:32:05 2024, max compression
```

## Comparing `stencila_plugin-2.0.0a30.tar` & `stencila_plugin-2.0.0a31.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0      890 2024-03-26 01:26:24.321915 stencila_plugin-2.0.0a30/README.md
--rw-r--r--   0        0        0     1865 2024-05-21 01:57:31.072257 stencila_plugin-2.0.0a30/pyproject.toml
--rw-r--r--   0        0        0       86 2024-05-20 23:13:11.799305 stencila_plugin-2.0.0a30/src/stencila_plugin/__init__.py
--rw-r--r--   0        0        0     5721 2024-03-26 03:21:24.057751 stencila_plugin-2.0.0a30/src/stencila_plugin/kernel.py
--rw-r--r--   0        0        0    10468 2024-05-20 23:13:11.799623 stencila_plugin-2.0.0a30/src/stencila_plugin/plugin.py
--rw-r--r--   0        0        0     8224 2024-03-26 01:26:24.323664 stencila_plugin-2.0.0a30/src/stencila_plugin/testing.py
--rw-r--r--   0        0        0        0 2024-03-26 01:26:24.323733 stencila_plugin-2.0.0a30/tests/__init__.py
--rw-r--r--   0        0        0      875 2024-03-26 01:26:24.323815 stencila_plugin-2.0.0a30/tests/conftest.py
--rw-r--r--   0        0        0      723 2024-05-20 23:13:11.799874 stencila_plugin-2.0.0a30/tests/plugin_example.py
--rw-r--r--   0        0        0     1775 2024-05-20 23:13:11.800071 stencila_plugin-2.0.0a30/tests/test_plugin.py
--rw-r--r--   0        0        0     1744 1970-01-01 00:00:00.000000 stencila_plugin-2.0.0a30/PKG-INFO
+-rw-r--r--   0        0        0      890 2024-03-26 01:26:24.321915 stencila_plugin-2.0.0a31/README.md
+-rw-r--r--   0        0        0     1865 2024-05-21 03:32:05.556001 stencila_plugin-2.0.0a31/pyproject.toml
+-rw-r--r--   0        0        0      319 2024-05-21 03:23:15.043705 stencila_plugin-2.0.0a31/src/stencila_plugin/__init__.py
+-rw-r--r--   0        0        0     4085 2024-05-21 03:23:15.043904 stencila_plugin-2.0.0a31/src/stencila_plugin/assistant.py
+-rw-r--r--   0        0        0     5721 2024-03-26 03:21:24.057751 stencila_plugin-2.0.0a31/src/stencila_plugin/kernel.py
+-rw-r--r--   0        0        0    12223 2024-05-21 03:23:15.044355 stencila_plugin-2.0.0a31/src/stencila_plugin/plugin.py
+-rw-r--r--   0        0        0     8224 2024-03-26 01:26:24.323664 stencila_plugin-2.0.0a31/src/stencila_plugin/testing.py
+-rw-r--r--   0        0        0        0 2024-03-26 01:26:24.323733 stencila_plugin-2.0.0a31/tests/__init__.py
+-rw-r--r--   0        0        0      875 2024-03-26 01:26:24.323815 stencila_plugin-2.0.0a31/tests/conftest.py
+-rw-r--r--   0        0        0     1126 2024-05-21 03:23:15.044616 stencila_plugin-2.0.0a31/tests/plugin_example.py
+-rw-r--r--   0        0        0     3261 2024-05-21 03:23:15.045065 stencila_plugin-2.0.0a31/tests/test_plugin.py
+-rw-r--r--   0        0        0     1744 1970-01-01 00:00:00.000000 stencila_plugin-2.0.0a31/PKG-INFO
```

### Comparing `stencila_plugin-2.0.0a30/README.md` & `stencila_plugin-2.0.0a31/README.md`

 * *Files identical despite different names*

### Comparing `stencila_plugin-2.0.0a30/pyproject.toml` & `stencila_plugin-2.0.0a31/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "stencila_plugin"
-version = "2.0.0a30"
+version = "2.0.0a31"
 description = "Library for building Stencila Plugins"
 readme = "README.md"
 authors = [
     { name = "Nokome Bentley", email = "nokome@stencila.io" },
     { name = "Brett Calcott", email = "brett@dragonfly.co.nz" },
 ]
 dependencies = [
```

### Comparing `stencila_plugin-2.0.0a30/src/stencila_plugin/kernel.py` & `stencila_plugin-2.0.0a31/src/stencila_plugin/kernel.py`

 * *Files identical despite different names*

### Comparing `stencila_plugin-2.0.0a30/src/stencila_plugin/plugin.py` & `stencila_plugin-2.0.0a31/src/stencila_plugin/plugin.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,37 +3,63 @@
 import os
 import sys
 import time
 import uuid
 from collections.abc import Sequence
 from typing import Any
 
-import cattrs
 from aiohttp import web
-from beartype import beartype
+from stencila_types import types as T
 from stencila_types.types import (
     ExecutionMessage,
     MessageLevel,
     Node,
     SoftwareApplication,
     SoftwareSourceCode,
     Variable,
 )
+from stencila_types.utilities import from_value, make_stencila_converter
 
+from .assistant import (
+    Assistant,
+    AssistantId,
+    GenerateOptions,
+    GenerateOutput,
+    GenerateTask,
+)
 from .kernel import Kernel, KernelId, KernelInstance, KernelName
 
 # https://github.com/kevinheavey/jsonalias
 Json = dict[str, "Json"] | list["Json"] | str | int | float | bool | None
 JsonDict = dict[str, Json]
 
 # According to the JSON-RPC spec, the id can be a string, integer, or null.
 IdType = str | int | None
 ParamsType = list | dict | None
 
 
+def make_rpc_converter():
+    """
+    Add some additional hooks for local unions that are NOT in the
+    stencila_types module.
+
+    SO AWKWARD!
+    """
+    converter = make_stencila_converter()
+    converter.register_structure_hook(
+        T.InstructionBlock | T.InstructionInline, lambda o, _: from_value(o)
+    )
+    return converter
+
+
+CONVERTER = make_rpc_converter()
+structure = CONVERTER.structure
+unstructure = CONVERTER.unstructure
+
+
 # TODO: We should really raise exceptions in the python code.
 class RPCErrorCodes:
     """JSON-RPC error codes.
 
     See https://www.jsonrpc.org/specification
     """
 
@@ -56,28 +82,37 @@
     return {
         "jsonrpc": "2.0",
         "error": {"code": code, "message": message},
         "id": msg_id,
     }
 
 
-@beartype
+# @beartype
 class Plugin:
     """A Stencila plugin.
 
     This routes the requests to the Kernel instances (and other APIs that are coming).
     """
 
-    def __init__(self, kernels: list[type[Kernel]] | None = None):
+    def __init__(
+        self,
+        kernels: list[type[Kernel]] | None = None,
+        assistants: list[type[Assistant]] | None = None,
+    ):
         kernels = kernels or []
         self.kernels: dict[KernelName, type[Kernel]] = {
             k.get_name(): k for k in kernels
         }
         self.kernel_instances: dict[KernelId, Kernel] = {}
 
+        # These are created per assistant (unlike kernels).
+        self.assistants: dict[AssistantId, Assistant] = (
+            {cls.get_name(): cls() for cls in assistants} if assistants else {}
+        )
+
     async def health(self) -> Json:
         """Get the health of the plugin.
 
         At present this method is only used to check communication with the
         plugin. In the future, the expected response object may be used for
         more detailed statistics about resource usage etc by the plugin.
         """
@@ -154,14 +189,41 @@
             await kernel.set_variable(name, value)
 
     async def kernel_remove(self, name: str, instance: str):
         kernel = self.kernel_instances.get(instance)
         if kernel:
             await kernel.remove_variable(name)
 
+        kernel = self.kernel_instances.get(instance)
+        if kernel:
+            await kernel.remove_variable(name)
+
+    async def assistant_system_prompt(
+        self, task: GenerateTask, options: GenerateOptions, assistant: AssistantId
+    ) -> str | None:
+        instance = self.assistants.get(assistant)
+        # Error?
+        if instance is None:
+            return None
+        task = structure(task, GenerateTask)
+        options = structure(options, GenerateOptions)
+        return await instance.system_prompt(task, options)
+
+    async def assistant_perform_task(
+        self, task: dict[str, Any], options: dict[str, Any], assistant: AssistantId
+    ) -> GenerateOutput:
+        instance = self.assistants.get(assistant)
+        if instance is None:
+            # TODO: Unclear how errors are handled here.
+            return None
+
+        task = structure(task, GenerateTask)
+        options = structure(options, GenerateOptions)
+        return await instance.perform_task(task, options)
+
     async def run(self) -> None:
         """Invoke the plugin.
 
         This method should be called by the plugin's `__main__` module.
         """
         protocol = os.environ.get("STENCILA_TRANSPORT")
         if protocol == "stdio":
@@ -202,22 +264,14 @@
     if not isinstance(params, dict):
         return _error(None, RPCErrorCodes.INVALID_PARAMS, "")
 
     # Hm. Still struggling with typing here.
     return await _handle_rpc(plugin, method, params=params, msg_id=msg_id)  # type: ignore
 
 
-def _make_jsonable(result: Json):
-    if isinstance(result, bool | int | float | str | None):
-        return result
-
-    dct = cattrs.unstructure(result)
-    return dct
-
-
 async def _handle_rpc(
     plugin: Plugin,
     method: str,
     *,
     params: ParamsType,
     msg_id: IdType = None,
 ) -> Json:
@@ -239,22 +293,22 @@
         )
 
     func = getattr(plugin, method, None)
     if callable(func):
         try:
             result = await func(*args, **kwargs)
             try:
-                dct_result = _make_jsonable(result)
+                json_result = unstructure(result)
             except Exception as e:
                 return _error(
                     msg_id,
                     RPCErrorCodes.INTERNAL_ERROR,
                     f"Cannot convert result to JSON {e}",
                 )
-            return _success(msg_id, dct_result)
+            return _success(msg_id, json_result)
         except Exception as e:
             return _error(msg_id, RPCErrorCodes.INTERNAL_ERROR, f"Internal error: {e}")
     else:
         return _error(
             msg_id, RPCErrorCodes.METHOD_NOT_FOUND, f"Method `{method}` not found"
         )
```

### Comparing `stencila_plugin-2.0.0a30/src/stencila_plugin/testing.py` & `stencila_plugin-2.0.0a31/src/stencila_plugin/testing.py`

 * *Files identical despite different names*

### Comparing `stencila_plugin-2.0.0a30/tests/conftest.py` & `stencila_plugin-2.0.0a31/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `stencila_plugin-2.0.0a30/tests/plugin_example.py` & `stencila_plugin-2.0.0a31/tests/plugin_example.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 import asyncio
 
 from stencila_types import shortcuts as S
 from stencila_types import types as T
 
+from stencila_plugin.assistant import (
+    Assistant,
+    GenerateOptions,
+    GenerateOutput,
+    GenerateTask,
+)
 from stencila_plugin.kernel import Kernel
 from stencila_plugin.plugin import Plugin
 
 
 class MyKernel(Kernel):
     @classmethod
     def get_name(cls) -> str:
@@ -17,11 +23,22 @@
             name="MyKernel",
             version="0.1.0",
             abstract=[S.p("A simple kernel for testing")],
             authors=[T.Person(name="Fred Flintstone")],
         )
 
 
+class MyAssistant(Assistant):
+    @classmethod
+    def get_name(cls) -> str:
+        return "test"
+
+    async def perform_task(
+        self, task: GenerateTask, options: GenerateOptions
+    ) -> GenerateOutput:
+        return GenerateOutput(content="hello")
+
+
 if __name__ == "__main__":
     """This is essential, as we are running the plugin as a script."""
-    plugin = Plugin(kernels=[MyKernel])
+    plugin = Plugin(kernels=[MyKernel], assistants=[MyAssistant])
     asyncio.run(plugin.run())
```

### Comparing `stencila_plugin-2.0.0a30/PKG-INFO` & `stencila_plugin-2.0.0a31/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stencila_plugin
-Version: 2.0.0a30
+Version: 2.0.0a31
 Summary: Library for building Stencila Plugins
 Keywords: programmable,reproducible,interactive,documents,python,SDK
 Author-Email: Nokome Bentley <nokome@stencila.io>, Brett Calcott <brett@dragonfly.co.nz>
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

