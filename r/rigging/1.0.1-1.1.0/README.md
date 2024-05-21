# Comparing `tmp/rigging-1.0.1.tar.gz` & `tmp/rigging-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rigging-1.0.1.tar", max compression
+gzip compressed data, was "rigging-1.1.0.tar", max compression
```

## Comparing `rigging-1.0.1.tar` & `rigging-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,21 @@
--rw-r--r--   0        0        0     1066 2024-05-16 22:53:46.951126 rigging-1.0.1/LICENSE
--rw-r--r--   0        0        0     1477 2024-05-16 22:53:46.951126 rigging-1.0.1/README.md
--rw-r--r--   0        0        0     2392 2024-05-16 22:53:46.955127 rigging-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      818 2024-05-16 22:53:46.955127 rigging-1.0.1/rigging/__init__.py
--rw-r--r--   0        0        0    41725 2024-05-16 22:53:46.955127 rigging-1.0.1/rigging/chat.py
--rw-r--r--   0        0        0    26509 2024-05-16 22:53:46.955127 rigging-1.0.1/rigging/completion.py
--rw-r--r--   0        0        0     3028 2024-05-16 22:53:46.955127 rigging-1.0.1/rigging/data.py
--rw-r--r--   0        0        0      865 2024-05-16 22:53:46.955127 rigging-1.0.1/rigging/error.py
--rw-r--r--   0        0        0    19086 2024-05-16 22:53:46.955127 rigging-1.0.1/rigging/generator.py
--rw-r--r--   0        0        0     1791 2024-05-16 22:53:46.955127 rigging-1.0.1/rigging/logging.py
--rw-r--r--   0        0        0    13768 2024-05-16 22:53:46.955127 rigging-1.0.1/rigging/message.py
--rw-r--r--   0        0        0    12579 2024-05-16 22:53:46.955127 rigging-1.0.1/rigging/model.py
--rw-r--r--   0        0        0     3748 2024-05-16 22:53:46.955127 rigging-1.0.1/rigging/parsing.py
--rw-r--r--   0        0        0     1090 2024-05-16 22:53:46.955127 rigging-1.0.1/rigging/prompt.py
--rw-r--r--   0        0        0        0 2024-05-16 22:53:46.955127 rigging-1.0.1/rigging/py.typed
--rw-r--r--   0        0        0    10466 2024-05-16 22:53:46.955127 rigging-1.0.1/rigging/tool.py
--rw-r--r--   0        0        0     2249 1970-01-01 00:00:00.000000 rigging-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-21 05:41:47.605232 rigging-1.1.0/LICENSE
+-rw-r--r--   0        0        0     1477 2024-05-21 05:41:47.605232 rigging-1.1.0/README.md
+-rw-r--r--   0        0        0     2609 2024-05-21 05:41:47.613232 rigging-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      879 2024-05-21 05:41:47.613232 rigging-1.1.0/rigging/__init__.py
+-rw-r--r--   0        0        0    41679 2024-05-21 05:41:47.613232 rigging-1.1.0/rigging/chat.py
+-rw-r--r--   0        0        0    26465 2024-05-21 05:41:47.613232 rigging-1.1.0/rigging/completion.py
+-rw-r--r--   0        0        0     3116 2024-05-21 05:41:47.613232 rigging-1.1.0/rigging/data.py
+-rw-r--r--   0        0        0      865 2024-05-21 05:41:47.613232 rigging-1.1.0/rigging/error.py
+-rw-r--r--   0        0        0      762 2024-05-21 05:41:47.613232 rigging-1.1.0/rigging/generator/__init__.py
+-rw-r--r--   0        0        0    14788 2024-05-21 05:41:47.613232 rigging-1.1.0/rigging/generator/base.py
+-rw-r--r--   0        0        0     6459 2024-05-21 05:41:47.613232 rigging-1.1.0/rigging/generator/litellm_.py
+-rw-r--r--   0        0        0     7168 2024-05-21 05:41:47.613232 rigging-1.1.0/rigging/generator/transformers_.py
+-rw-r--r--   0        0        0     5628 2024-05-21 05:41:47.613232 rigging-1.1.0/rigging/generator/vllm_.py
+-rw-r--r--   0        0        0     1791 2024-05-21 05:41:47.613232 rigging-1.1.0/rigging/logging.py
+-rw-r--r--   0        0        0    13703 2024-05-21 05:41:47.613232 rigging-1.1.0/rigging/message.py
+-rw-r--r--   0        0        0    13325 2024-05-21 05:41:47.613232 rigging-1.1.0/rigging/model.py
+-rw-r--r--   0        0        0     3748 2024-05-21 05:41:47.613232 rigging-1.1.0/rigging/parsing.py
+-rw-r--r--   0        0        0     1090 2024-05-21 05:41:47.613232 rigging-1.1.0/rigging/prompt.py
+-rw-r--r--   0        0        0        0 2024-05-21 05:41:47.613232 rigging-1.1.0/rigging/py.typed
+-rw-r--r--   0        0        0    10466 2024-05-21 05:41:47.613232 rigging-1.1.0/rigging/tool.py
+-rw-r--r--   0        0        0     2440 1970-01-01 00:00:00.000000 rigging-1.1.0/PKG-INFO
```

### Comparing `rigging-1.0.1/LICENSE` & `rigging-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rigging-1.0.1/README.md` & `rigging-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `rigging-1.0.1/pyproject.toml` & `rigging-1.1.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,34 @@
 [tool.poetry]
 name = "rigging"
-version = "1.0.1"
+version = "1.1.0"
 description = "LLM Interaction Framework"
 authors = ["Nick Landers <monoxgas@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/dreadnode/rigging"
 readme = "README.md"
 packages = [
     {include = "rigging"}
 ]
 
 [tool.poetry.dependencies]
-python = "<3.13,>=3.10"
+python = "^3.10"
 pydantic = "2.5.3"
 pydantic-xml = "2.7.0"
 loguru = "^0.7.2"
 litellm = "1.35.21"
 pandas = "^2.2.2"
 
+vllm = { version = "0.4.2", optional = true }
+transformers = { version = "^4.41.0", optional = true }
+accelerate = { version = "^0.30.1", optional = true }
+
+[tool.poetry.extras]
+all = ["vllm", "transformers", "accelerate"]
+
 [tool.poetry.group.dev.dependencies]
 ipykernel = "^6.27.1"
 mypy = "^1.8.0"
 ruff = "^0.1.14"
 pytest = "^8.0.0"
 pandas = "^2.2.2"
 pandas-stubs = "^2.2.1.240316"
```

### Comparing `rigging-1.0.1/rigging/__init__.py` & `rigging-1.1.0/rigging/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from rigging.chat import Chat, PendingChat
 from rigging.completion import Completion, PendingCompletion
 from rigging.data import chats_to_df, df_to_chats
 from rigging.generator import GenerateParams, Generator, chat, complete, get_generator, register_generator
 from rigging.message import Message, MessageDict, Messages
-from rigging.model import Model, attr, element, wrapped
+from rigging.model import Model, attr, element, make_primitive, wrapped
 from rigging.tool import Tool
 
+__version__ = "1.1.0"
+
 __all__ = [
     "get_generator",
     "Message",
     "MessageDict",
     "Messages",
     "Tool",
     "Model",
@@ -23,12 +25,13 @@
     "chat",
     "complete",
     "Completion",
     "PendingCompletion",
     "register_generator",
     "chats_to_df",
     "df_to_chats",
+    "make_primitive",
 ]
 
 from loguru import logger
 
 logger.disable("rigging")
```

### Comparing `rigging-1.0.1/rigging/chat.py` & `rigging-1.1.0/rigging/chat.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,35 +9,25 @@
 from copy import deepcopy
 from dataclasses import dataclass
 from datetime import datetime
 from typing import runtime_checkable
 from uuid import UUID, uuid4
 
 from loguru import logger
-from pydantic import (
-    BaseModel,
-    ConfigDict,
-    Field,
-    ValidationError,
-    computed_field,
-)
+from pydantic import BaseModel, ConfigDict, Field, ValidationError, computed_field
 
 from rigging.error import ExhaustedMaxRoundsError
 from rigging.generator import GenerateParams, Generator, get_generator
 from rigging.message import Message, MessageDict, Messages
-from rigging.model import (
-    Model,
-    ModelT,
-    SystemErrorModel,
-    ValidationErrorModel,
-)
+from rigging.model import Model, ModelT, SystemErrorModel, ValidationErrorModel
 from rigging.prompt import system_tool_extension
 from rigging.tool import Tool, ToolCalls, ToolDescriptionList, ToolResult, ToolResults
 
 DEFAULT_MAX_ROUNDS = 5
+"""Maximum number of internal callback rounds to attempt during generation before giving up."""
 
 
 class Chat(BaseModel):
     """
     Represents a completed chat conversation.
     """
 
@@ -942,15 +932,15 @@
         """
         states: list[RunState] = [RunState([], p, self._process()) for p in self._fit_params(count, params)]
         _ = [next(state.processor) for state in states]
 
         pending_states = states
         while pending_states:
             inbounds = self.generator.generate_messages(
-                [s.messages for s in pending_states], [s.params for s in pending_states], prefix=self.chat.all
+                [self.chat.all + s.messages for s in pending_states], [s.params for s in pending_states]
             )
 
             for inbound, state in zip(inbounds, pending_states, strict=True):
                 try:
                     state.messages = state.processor.send(inbound)
                 except StopIteration as stop:
                     state.done = True
@@ -980,15 +970,15 @@
         """async variant of the [rigging.chat.PendingChat.run_many][] method."""
         states: list[RunState] = [RunState([], p, self._process()) for p in self._fit_params(count, params)]
         _ = [next(state.processor) for state in states]
 
         pending_states = states
         while pending_states:
             inbounds = await self.generator.agenerate_messages(
-                [s.messages for s in pending_states], [s.params for s in pending_states], prefix=self.chat.all
+                [self.chat.all + s.messages for s in pending_states], [s.params for s in pending_states]
             )
 
             for inbound, state in zip(inbounds, pending_states, strict=True):
                 try:
                     state.messages = state.processor.send(inbound)
                 except StopIteration as stop:
                     state.done = True
@@ -1043,36 +1033,35 @@
             many = t.cast(t.Sequence[str] | t.Sequence[MessageDict], [many])
 
         count = max(len(many), len(params) if params is not None else 0)
         many = self._fit_many(count, many)
         params = self._fit_params(count, params)
 
         states: list[BatchRunState] = [
-            BatchRunState(m, [], p, self._process()) for m, p in zip(many, params, strict=True)
+            BatchRunState(self.chat.all + m, [], p, self._process()) for m, p in zip(many, params, strict=True)
         ]
         _ = [next(state.processor) for state in states]
 
         size = size or len(states)
 
         pending_states = states
         while pending_states:
             for chunk in [pending_states[i : i + size] for i in range(0, len(pending_states), size)]:
                 inbounds = self.generator.generate_messages(
                     [s.inputs + s.messages for s in chunk],
                     [s.params for s in chunk],
-                    prefix=self.chat.all,
                 )
 
                 for inbound, state in zip(inbounds, chunk, strict=True):
                     try:
                         state.messages = state.processor.send(inbound)
                     except StopIteration as stop:
                         state.done = True
                         state.chat = Chat(
-                            self.chat.all + state.inputs,
+                            state.inputs,
                             t.cast(list[Message], stop.value),
                             generator=self.generator,
                             metadata=self.metadata,
                             params=state.params,
                         )
                     except ExhaustedMaxRoundsError:
                         if not skip_failed:
@@ -1101,36 +1090,35 @@
             many = t.cast(t.Sequence[str] | t.Sequence[MessageDict], [many])
 
         count = max(len(many), len(params) if params is not None else 0)
         many = self._fit_many(count, many)
         params = self._fit_params(count, params)
 
         states: list[BatchRunState] = [
-            BatchRunState(m, [], p, self._process()) for m, p in zip(many, params, strict=True)
+            BatchRunState(self.chat.all + m, [], p, self._process()) for m, p in zip(many, params, strict=True)
         ]
         _ = [next(state.processor) for state in states]
 
         size = size or len(states)
 
         pending_states = states
         while pending_states:
             for chunk in [pending_states[i : i + size] for i in range(0, len(pending_states), size)]:
                 inbounds = await self.generator.agenerate_messages(
                     [s.inputs + s.messages for s in chunk],
                     [s.params for s in chunk],
-                    prefix=self.chat.all,
                 )
 
                 for inbound, state in zip(inbounds, chunk, strict=True):
                     try:
                         state.messages = state.processor.send(inbound)
                     except StopIteration as stop:
                         state.done = True
                         state.chat = Chat(
-                            self.chat.all + state.inputs,
+                            state.inputs,
                             t.cast(list[Message], stop.value),
                             generator=self.generator,
                             metadata=self.metadata,
                             params=state.params,
                         )
                     except ExhaustedMaxRoundsError:
                         if not skip_failed:
```

### Comparing `rigging-1.0.1/rigging/completion.py` & `rigging-1.1.0/rigging/completion.py`

 * *Files 1% similar despite different names*

```diff
@@ -676,17 +676,16 @@
         params = self._fit_params(len(many), params)
         states: list[RunState] = [RunState(m, p, self._process()) for m, p in zip(many, params, strict=True)]
         _ = [next(state.processor) for state in states]
 
         pending_states = states
         while pending_states:
             inbounds = self.generator.generate_texts(
-                [s.text for s in pending_states],
+                [self.text + s.text for s in pending_states],
                 [s.params for s in pending_states],
-                prefix=self.text,
             )
 
             for inbound, state in zip(inbounds, pending_states, strict=True):
                 try:
                     state.processor.send(inbound)
                 except StopIteration as stop:
                     state.done = True
@@ -717,17 +716,16 @@
         params = self._fit_params(len(many), params)
         states: list[RunState] = [RunState(m, p, self._process()) for m, p in zip(many, params, strict=True)]
         _ = [next(state.processor) for state in states]
 
         pending_states = states
         while pending_states:
             inbounds = await self.generator.agenerate_texts(
-                [s.text for s in pending_states],
+                [self.text + s.text for s in pending_states],
                 [s.params for s in pending_states],
-                prefix=self.text,
             )
 
             for inbound, state in zip(inbounds, pending_states, strict=True):
                 try:
                     state.processor.send(inbound)
                 except StopIteration as stop:
                     state.done = True
```

### Comparing `rigging-1.0.1/rigging/data.py` & `rigging-1.1.0/rigging/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,29 +3,31 @@
 
 import pandas as pd
 
 from rigging.chat import Chat
 from rigging.message import Message
 
 
-def chats_to_df(chats: list[Chat]) -> pd.DataFrame:
+def chats_to_df(chats: Chat | t.Sequence[Chat]) -> pd.DataFrame:
     """
-    Convert a list of Chat objects into a pandas DataFrame.
+    Convert a Chat or list of Chat objects into a pandas DataFrame.
 
     Note:
         The messages will be flatted and can be joined by the
         chat_id column.
 
     Args:
-        chats: A list of Chat objects.
+        chats: A Chat or list of Chat objects.
 
     Returns:
         A pandas DataFrame containing the chat data.
 
     """
+    chats = [chats] if isinstance(chats, Chat) else chats
+
     data: list[dict[t.Any, t.Any]] = []
     for chat in chats:
         generator_id = chat.generator_id
         metadata = json.dumps(chat.metadata)
         generated = False
         for messages in [chat.messages, chat.generated]:
             for message in messages:
```

### Comparing `rigging-1.0.1/rigging/error.py` & `rigging-1.1.0/rigging/error.py`

 * *Files identical despite different names*

### Comparing `rigging-1.0.1/rigging/generator.py` & `rigging-1.1.0/rigging/generator/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,20 @@
-"""
-Generators produce completions for a given set of messages or text.
-"""
-
-import asyncio
+import inspect
 import typing as t
 
-import litellm  # type: ignore
 from loguru import logger
 from pydantic import BaseModel, ConfigDict, Field, field_validator
 
 from rigging.error import InvalidModelSpecifiedError
-from rigging.message import (
-    Message,
-    MessageDict,
-)
+from rigging.message import Message, MessageDict
 
 if t.TYPE_CHECKING:
     from rigging.chat import PendingChat
     from rigging.completion import PendingCompletion
 
-# We should probably let people configure
-# this independently, but for now we'll
-# fix it to prevent confusion
-litellm.drop_params = True
-
 # Global provider map
 g_providers: dict[str, type["Generator"]] = {}
 
 
 # TODO: Ideally we flex this to support arbitrary
 # generator params, but we'll limit things
 # for now until we understand the use cases
@@ -50,14 +37,17 @@
 
     temperature: float | None = None
     """The sampling temperature."""
 
     max_tokens: int | None = None
     """The maximum number of tokens to generate."""
 
+    top_k: int | None = None
+    """The top-k sampling parameter."""
+
     top_p: float | None = None
     """The nucleus sampling probability."""
 
     stop: list[str] | None = None
     """A list of stop sequences to stop generation at."""
 
     presence_penalty: float | None = None
@@ -157,81 +147,71 @@
         """
         return get_identifier(self, params)
 
     def generate_messages(
         self,
         messages: t.Sequence[t.Sequence[Message]],
         params: t.Sequence[GenerateParams],
-        *,
-        prefix: t.Sequence[Message] | None = None,
     ) -> t.Sequence[Message]:
         """
         Generate a batch of messages using the specified parameters.
 
         Note:
             The length of `params` must be the same as the length of `many`.
 
         Args:
             messages: A sequence of sequences of messages.
             params: A sequence of GenerateParams objects.
-            prefix: A sequence of fixed messages to be prefixed before every item of `many`.
 
         Returns:
             A sequence of generated messages.
 
         Raises:
             NotImplementedError: This method is not supported by this generator.
         """
         raise NotImplementedError("`generate_messages` is not supported by this generator.")
 
     async def agenerate_messages(
         self,
         messages: t.Sequence[t.Sequence[Message]],
         params: t.Sequence[GenerateParams],
-        *,
-        prefix: t.Sequence[Message] | None = None,
     ) -> t.Sequence[Message]:
         """async version of [rigging.generator.Generator.generate_messages][]"""
         raise NotImplementedError("`agenerate_messages` is not supported by this generator.")
 
     def generate_texts(
         self,
         texts: t.Sequence[str],
         params: t.Sequence[GenerateParams],
-        *,
-        prefix: str | None = None,
     ) -> t.Sequence[str]:
         """
         Generate a batch of text completions using the generator.
 
         Note:
             This method falls back to looping over the inputs and calling `generate_text` for each item.
 
         Note:
             If supplied, the length of `params` must be the same as the length of `many`.
 
         Args:
             texts: The input texts for generating the batch.
             params: Additional parameters for generating each text in the batch.
-            prefix: A fixed input text to be used as a prefix for all of `many`.
 
         Returns:
             The generated texts.
 
         Raises:
             NotImplementedError: This method is not supported by this generator.
         """
         raise NotImplementedError("`generate_texts` is not supported by this generator.")
 
     async def agenerate_texts(
         self,
         texts: t.Sequence[str],
         params: t.Sequence[GenerateParams],
-        *,
-        prefix: str | None = None,
     ) -> t.Sequence[str]:
         """async version of [rigging.generator.Generator.generate_texts][]"""
         raise NotImplementedError("`agenerate_texts` is not supported by this generator.")
 
     # Helper alternative to chat(generator) -> generator.chat(...)
     #
     # params seem odd, but mypy doesn't like the TypedDict in a list otherwise
@@ -349,14 +329,18 @@
     Returns:
         The identifier string for the generator.
     """
 
     provider = next(name for name, klass in g_providers.items() if isinstance(generator, klass))
     identifier = f"{provider}!{generator.model}"
 
+    extra_cls_args = generator.model_dump(exclude_unset=True, exclude={"model", "api_key", "params"})
+    if extra_cls_args:
+        identifier += f",{','.join([f'{k}={v}' for k, v in extra_cls_args.items()])}"
+
     merged_params = generator.params.merge_with(params)
     if merged_params.extra:
         logger.warning("Extra parameters are not supported in identifiers.")
         merged_params.extra = {}
 
     params_dict = merged_params.to_dict()
     if params_dict:
@@ -397,36 +381,64 @@
 
     Raises:
         InvalidModelSpecified: If the identifier is invalid.
     """
 
     provider: str = list(g_providers.keys())[0]
     model: str = identifier
-    api_key: str | None = None
     params: GenerateParams = GenerateParams()
 
     # Split provider, model, and kwargs
 
-    try:
-        if "!" in identifier:
+    if "!" in identifier:
+        try:
             provider, model = identifier.split("!")
+        except Exception as e:
+            raise InvalidModelSpecifiedError(identifier) from e
+
+    if provider not in g_providers:
+        raise InvalidModelSpecifiedError(identifier)
 
-        if "," in model:
+    generator_cls = g_providers[provider]
+
+    kwargs = {}
+    if "," in model:
+        try:
             model, kwargs_str = model.split(",", 1)
             kwargs = dict(arg.split("=") for arg in kwargs_str.split(","))
-            api_key = kwargs.pop("api_key", None)
-            params = GenerateParams(**kwargs)
+        except Exception as e:
+            raise InvalidModelSpecifiedError(identifier) from e
+
+    # See if any of the kwargs would apply to the cls constructor directly
+    init_signature = inspect.signature(generator_cls)
+    init_kwargs: dict[str, t.Any] = {k: kwargs.pop(k) for k in list(kwargs.keys())[:] if k in init_signature.parameters}
+
+    # Do some subtle type conversion
+    for k, v in init_kwargs.items():
+        try:
+            init_kwargs[k] = float(v)
+            continue
+        except ValueError:
+            pass
+
+        try:
+            init_kwargs[k] = int(v)
+            continue
+        except ValueError:
+            pass
+
+        if isinstance(v, str) and v.lower() in ["true", "false"]:
+            init_kwargs[k] = v.lower() == "true"
+
+    try:
+        params = GenerateParams(**kwargs)
     except Exception as e:
         raise InvalidModelSpecifiedError(identifier) from e
 
-    if provider not in g_providers:
-        raise InvalidModelSpecifiedError(identifier)
-
-    generator_cls = g_providers[provider]
-    return generator_cls(model=model, api_key=api_key, params=params)
+    return generator_cls(model=model, params=params, **init_kwargs)
 
 
 def register_generator(provider: str, generator_cls: type[Generator]) -> None:
     """
     Register a generator class for a provider id.
 
     This let's you use [rigging.generator.get_generator][] with a custom generator class.
@@ -465,132 +477,7 @@
 
     Returns:
         None
     """
     logger.trace(f"--- {title} ---")
     logger.trace(content)
     logger.trace("---")
-
-
-class LiteLLMGenerator(Generator):
-    """
-    Generator backed by the LiteLLM library.
-
-    Note:
-        Find more information about supported models and formats [in their docs.](https://docs.litellm.ai/docs/providers).
-
-    Note:
-        Batching support is not performant and simply a loop over inputs.
-    """
-
-    def _generate_message(self, messages: t.Sequence[Message], params: GenerateParams) -> Message:
-        result = litellm.completion(
-            self.model,
-            [message.model_dump(include={"role", "content"}) for message in messages],
-            api_key=self.api_key,
-            **self.params.merge_with(params).to_dict(),
-        )
-        response = result.choices[-1].message.content.strip()
-        return Message(role="assistant", content=response)
-
-    async def _agenerate_message(self, messages: t.Sequence[Message], params: GenerateParams) -> Message:
-        result = await litellm.acompletion(
-            self.model,
-            [message.model_dump(include={"role", "content"}) for message in messages],
-            api_key=self.api_key,
-            **self.params.merge_with(params).to_dict(),
-        )
-        response = result.choices[-1].message.content.strip()
-        return Message(role="assistant", content=response)
-
-    def _generate_text(self, text: str, params: GenerateParams) -> str:
-        result = litellm.text_completion(
-            text, self.model, api_key=self.api_key, **self.params.merge_with(params).to_dict()
-        )
-        return t.cast(str, result.choices[-1]["text"])
-
-    async def _agenerate_text(self, text: str, params: GenerateParams) -> str:
-        result = await litellm.atext_completion(
-            text, self.model, api_key=self.api_key, **self.params.merge_with(params).to_dict()
-        )
-        return t.cast(str, result.choices[-1]["text"])
-
-    def generate_messages(
-        self,
-        messages: t.Sequence[t.Sequence[Message]],
-        params: t.Sequence[GenerateParams],
-        *,
-        prefix: t.Sequence[Message] | None = None,
-    ) -> t.Sequence[Message]:
-        if prefix is not None:
-            messages = [list(prefix) + list(messages) for messages in messages]
-
-        generated: list[Message] = []
-        for i, (_messages, _params) in enumerate(zip(messages, params, strict=True)):
-            trace_messages(_messages, f"Messages {i+1}/{len(messages)}")
-            next_message = self._generate_message(_messages, _params)
-            generated.append(next_message)
-            trace_messages([next_message], f"Response {i+1}/{len(messages)}")
-
-        return generated
-
-    async def agenerate_messages(
-        self,
-        messages: t.Sequence[t.Sequence[Message]],
-        params: t.Sequence[GenerateParams],
-        *,
-        prefix: t.Sequence[Message] | None = None,
-    ) -> t.Sequence[Message]:
-        if prefix is not None:
-            messages = [list(prefix) + list(messages) for messages in messages]
-
-        generated: list[Message] = await asyncio.gather(
-            *[self._agenerate_message(_messages, _params) for _messages, _params in zip(messages, params, strict=True)]
-        )
-
-        for i, (_messages, _generated) in enumerate(zip(messages, generated, strict=True)):
-            trace_messages(_messages, f"Messages {i+1}/{len(messages)}")
-            trace_messages([_generated], f"Response {i+1}/{len(messages)}")
-
-        return generated
-
-    def generate_texts(
-        self,
-        texts: t.Sequence[str],
-        params: t.Sequence[GenerateParams],
-        *,
-        prefix: str | None = None,
-    ) -> t.Sequence[str]:
-        if prefix is not None:
-            texts = [prefix + text for text in texts]
-
-        generated: list[str] = []
-        for i, (text, _params) in enumerate(zip(texts, params, strict=True)):
-            trace_str(text, f"Text {i+1}/{len(texts)}")
-            response = self._generate_text(text, _params)
-            generated.append(response)
-            trace_str(response, f"Generated {i+1}/{len(texts)}")
-
-        return generated
-
-    async def agenerate_texts(
-        self,
-        texts: t.Sequence[str],
-        params: t.Sequence[GenerateParams],
-        *,
-        prefix: str | None = None,
-    ) -> t.Sequence[str]:
-        if prefix is not None:
-            texts = [prefix + text for text in texts]
-
-        generated: list[str] = await asyncio.gather(
-            *[self._agenerate_text(text, _params) for text, _params in zip(texts, params, strict=True)]
-        )
-
-        for i, (text, response) in enumerate(zip(texts, generated, strict=True)):
-            trace_str(text, f"Text {i+1}/{len(texts)}")
-            trace_str(response, f"Generated {i+1}/{len(texts)}")
-
-        return generated
-
-
-g_providers["litellm"] = LiteLLMGenerator
```

### Comparing `rigging-1.0.1/rigging/logging.py` & `rigging-1.1.0/rigging/logging.py`

 * *Files identical despite different names*

### Comparing `rigging-1.0.1/rigging/message.py` & `rigging-1.1.0/rigging/message.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 This module covers core message objects and handling.
 """
 
 import copy
 import string
 import typing as t
+from textwrap import dedent
 from uuid import UUID, uuid4
 
 from pydantic import (
     BaseModel,
     ConfigDict,
     Field,
     FieldSerializationInfo,
@@ -90,17 +91,15 @@
 
     @computed_field  # type: ignore[misc]
     @property
     def content(self) -> str:
         """The content of the message."""
         # We used to sync the models and content each time it was accessed,
         # hence the getter. Now we just return the stored content.
-        # I'll leave it as is for now in case we want to add any
-        # logic here in the future.
-        return self._content
+        return dedent(self._content)
 
     @content.setter
     def content(self, value: str) -> None:
         # TODO: Maintain any parsed parts which are
         # still in the content - our move to slices for
         # tracking parsed parts makes this more complicated
         # so fow now I've opted to strip all parts
```

### Comparing `rigging-1.0.1/rigging/model.py` & `rigging-1.1.0/rigging/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Models are the core datatypes for structured parsing.
 """
 
 import re
 import typing as t
 from xml.etree import ElementTree as ET
 
-from pydantic import ValidationError, field_validator
+from pydantic import ValidationError, create_model, field_validator
 from pydantic.alias_generators import to_snake
 from pydantic_xml import BaseXmlModel
 from pydantic_xml import attr as attr
 from pydantic_xml import element as element
 from pydantic_xml import wrapped as wrapped
 from pydantic_xml.element import SearchMode  # type: ignore [attr-defined]
 from pydantic_xml.typedefs import EntityLocation, NsMap
@@ -84,15 +84,15 @@
         Converts the model to a pretty XML string with indents and newlines.
 
         Returns:
             The pretty XML representation of the model.
         """
         tree = self.to_xml_tree()
         ET.indent(tree, "  ")
-        pretty_encoded_xml = ET.tostring(tree).decode()
+        pretty_encoded_xml = ET.tostring(tree, short_empty_elements=False).decode()
 
         if self.__class__.is_simple():
             return unescape_xml(pretty_encoded_xml)
         else:
             return pretty_encoded_xml
 
     # XML parsing gets weird when the interior text contains tags like <br>.
@@ -256,14 +256,43 @@
         matches = cls.from_text(content)  # type: ignore [var-annotated]
         if fail_on_many and len(matches) > 1:
             raise ValidationError("Multiple matches found with 'fail_on_many=True'")
         return max(matches, key=lambda x: x[1].stop - x[1].start)
 
 
 #
+# Functional Constructor
+#
+
+
+class PrimitiveModel(Model, tag="primitive"):
+    content: str
+
+
+def make_primitive(
+    name: str, *, tag: str | None = None, doc: str | None = None, validator: t.Callable[[str], str | None] | None = None
+) -> type[PrimitiveModel]:
+    """ """
+
+    def _validate(value: str) -> str:
+        if validator is not None:
+            return validator(value) or value
+        return value
+
+    return create_model(
+        name,
+        __base__=PrimitiveModel,
+        __doc__=doc,
+        __cls_kwargs__={"tag": tag},
+        content=(str, ...),
+        __validators__={"content_validator": field_validator("content")(_validate)} if validator else {},  # type: ignore
+    )
+
+
+#
 # Helpers for passing structured errors to models
 #
 
 
 class ErrorModel(Model, tag="error"):
     content: str
```

### Comparing `rigging-1.0.1/rigging/parsing.py` & `rigging-1.1.0/rigging/parsing.py`

 * *Files identical despite different names*

### Comparing `rigging-1.0.1/rigging/prompt.py` & `rigging-1.1.0/rigging/prompt.py`

 * *Files identical despite different names*

### Comparing `rigging-1.0.1/rigging/tool.py` & `rigging-1.1.0/rigging/tool.py`

 * *Files identical despite different names*

### Comparing `rigging-1.0.1/PKG-INFO` & `rigging-1.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 Metadata-Version: 2.1
 Name: rigging
-Version: 1.0.1
+Version: 1.1.0
 Summary: LLM Interaction Framework
 Home-page: https://github.com/dreadnode/rigging
 License: MIT
 Author: Nick Landers
 Author-email: monoxgas@gmail.com
-Requires-Python: >=3.10,<3.13
+Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Provides-Extra: all
+Requires-Dist: accelerate (>=0.30.1,<0.31.0) ; extra == "all"
 Requires-Dist: litellm (==1.35.21)
 Requires-Dist: loguru (>=0.7.2,<0.8.0)
 Requires-Dist: pandas (>=2.2.2,<3.0.0)
 Requires-Dist: pydantic (==2.5.3)
 Requires-Dist: pydantic-xml (==2.7.0)
+Requires-Dist: transformers (>=4.41.0,<5.0.0) ; extra == "all"
+Requires-Dist: vllm (==0.4.2) ; extra == "all"
 Project-URL: Repository, https://github.com/dreadnode/rigging
 Description-Content-Type: text/markdown
 
 # Rigging
 
 Rigging is a lightweight LLM interaction framework built on Pydantic XML. The goal is to make leveraging LLMs in production pipelines as simple and effictive as possible. Here are the highlights:
```

