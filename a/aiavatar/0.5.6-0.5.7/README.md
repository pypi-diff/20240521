# Comparing `tmp/aiavatar-0.5.6-py3-none-any.whl.zip` & `tmp/aiavatar-0.5.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 43702 bytes, number of entries: 33
+Zip file size: 47116 bytes, number of entries: 33
 -rw-r--r--  2.0 unx      712 b- defN 24-May-12 07:19 aiavatar/__init__.py
 -rw-r--r--  2.0 unx     3407 b- defN 24-May-12 13:20 aiavatar/avatar.py
 -rw-r--r--  2.0 unx     8161 b- defN 24-May-19 01:20 aiavatar/bot.py
 -rw-r--r--  2.0 unx     2196 b- defN 24-May-12 06:14 aiavatar/animation/__init__.py
 -rw-r--r--  2.0 unx     1535 b- defN 24-May-12 06:14 aiavatar/animation/vrchat.py
 -rw-r--r--  2.0 unx        0 b- defN 24-May-05 04:55 aiavatar/api/__init__.py
 -rw-r--r--  2.0 unx    10425 b- defN 24-May-15 15:19 aiavatar/api/router.py
@@ -14,22 +14,22 @@
 -rw-r--r--  2.0 unx     8372 b- defN 24-May-19 01:56 aiavatar/listeners/__init__.py
 -rw-r--r--  2.0 unx     2773 b- defN 24-May-05 04:46 aiavatar/listeners/azurevoicerequest.py
 -rw-r--r--  2.0 unx     4951 b- defN 24-May-05 04:46 aiavatar/listeners/azurewakeword.py
 -rw-r--r--  2.0 unx     1655 b- defN 24-May-13 17:33 aiavatar/listeners/openailisteners.py
 -rw-r--r--  2.0 unx      976 b- defN 24-May-12 04:21 aiavatar/listeners/voicerequest.py
 -rw-r--r--  2.0 unx     1132 b- defN 24-May-12 04:21 aiavatar/listeners/wakeword.py
 -rw-r--r--  2.0 unx      178 b- defN 24-Apr-14 09:42 aiavatar/processors/__init__.py
--rw-r--r--  2.0 unx     9911 b- defN 24-May-19 14:51 aiavatar/processors/chatgpt.py
--rw-r--r--  2.0 unx     3110 b- defN 24-May-05 11:34 aiavatar/processors/claude.py
--rw-r--r--  2.0 unx     3388 b- defN 24-May-19 14:52 aiavatar/processors/gemini.py
+-rw-r--r--  2.0 unx     9911 b- defN 24-May-21 08:45 aiavatar/processors/chatgpt.py
+-rw-r--r--  2.0 unx    10457 b- defN 24-May-21 15:33 aiavatar/processors/claude.py
+-rw-r--r--  2.0 unx    10397 b- defN 24-May-21 15:12 aiavatar/processors/gemini.py
 -rw-r--r--  2.0 unx     2712 b- defN 24-May-15 15:19 aiavatar/speech/__init__.py
 -rw-r--r--  2.0 unx     1887 b- defN 24-May-05 01:03 aiavatar/speech/azurespeech.py
 -rw-r--r--  2.0 unx     1474 b- defN 24-May-13 17:33 aiavatar/speech/openaispeech.py
 -rw-r--r--  2.0 unx     1348 b- defN 24-May-13 13:48 aiavatar/speech/voicevox.py
 -rw-r--r--  2.0 unx      220 b- defN 24-Apr-16 15:07 aiavatar/speech/soundplayers/__init__.py
 -rw-r--r--  2.0 unx     2175 b- defN 24-May-19 14:54 aiavatar/speech/soundplayers/sounddevice_player.py
--rw-r--r--  2.0 unx    11324 b- defN 24-May-19 14:55 aiavatar-0.5.6.dist-info/LICENSE
--rw-r--r--  2.0 unx    27979 b- defN 24-May-19 14:55 aiavatar-0.5.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-19 14:55 aiavatar-0.5.6.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 24-May-19 14:55 aiavatar-0.5.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     2787 b- defN 24-May-19 14:55 aiavatar-0.5.6.dist-info/RECORD
-33 files, 130796 bytes uncompressed, 39230 bytes compressed:  70.0%
+-rw-r--r--  2.0 unx    11324 b- defN 24-May-21 15:33 aiavatar-0.5.7.dist-info/LICENSE
+-rw-r--r--  2.0 unx    28121 b- defN 24-May-21 15:33 aiavatar-0.5.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-21 15:33 aiavatar-0.5.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 24-May-21 15:33 aiavatar-0.5.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     2789 b- defN 24-May-21 15:33 aiavatar-0.5.7.dist-info/RECORD
+33 files, 145296 bytes uncompressed, 42644 bytes compressed:  70.7%
```

## zipnote {}

```diff
@@ -78,23 +78,23 @@
 
 Filename: aiavatar/speech/soundplayers/__init__.py
 Comment: 
 
 Filename: aiavatar/speech/soundplayers/sounddevice_player.py
 Comment: 
 
-Filename: aiavatar-0.5.6.dist-info/LICENSE
+Filename: aiavatar-0.5.7.dist-info/LICENSE
 Comment: 
 
-Filename: aiavatar-0.5.6.dist-info/METADATA
+Filename: aiavatar-0.5.7.dist-info/METADATA
 Comment: 
 
-Filename: aiavatar-0.5.6.dist-info/WHEEL
+Filename: aiavatar-0.5.7.dist-info/WHEEL
 Comment: 
 
-Filename: aiavatar-0.5.6.dist-info/top_level.txt
+Filename: aiavatar-0.5.7.dist-info/top_level.txt
 Comment: 
 
-Filename: aiavatar-0.5.6.dist-info/RECORD
+Filename: aiavatar-0.5.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aiavatar/processors/claude.py

```diff
@@ -1,86 +1,257 @@
+from abc import abstractmethod
+import base64
 from datetime import datetime
+import json
 from logging import getLogger, NullHandler
 import traceback
-from typing import AsyncGenerator
+from typing import Callable, AsyncGenerator
 from anthropic import AsyncAnthropic
 from . import ChatProcessor
 
+
+class ClaudeFunction:
+    def __init__(self, name: str, description: str=None, input_schema: dict=None, func: Callable=None):
+        self.name = name
+        self.description = description
+        self.input_schema = input_schema
+        self.func = func
+    
+    def get_spec(self):
+        return {
+            "name": self.name,
+            "description": self.description,
+            "input_schema": self.input_schema
+        }
+
+
 class ClaudeProcessor(ChatProcessor):
     def __init__(self, *, api_key: str, model: str="claude-3-sonnet-20240229", temperature: float=1.0, max_tokens: int=200, functions: dict=None, system_message_content: str=None, history_count: int=10, history_timeout: float=60.0):
         self.logger = getLogger(__name__)
         self.logger.addHandler(NullHandler())
 
         self.api_key = api_key
         self.model = model
         self.temperature = temperature
         self.max_tokens = max_tokens
+        self.functions = functions
         self.system_message_content = system_message_content
         self.history_count = history_count
         self.history_timeout = history_timeout
         self.histories = []
         self.last_chat_at = datetime.utcnow()
         self.on_start_processing = None
 
     def reset_histories(self):
         self.histories.clear()
 
-    def build_messages(self, text):
+    async def build_messages(self, text):
         messages = []
         try:
             # Histories
             messages.extend(self.histories[-1 * self.history_count:])
 
             # Current user message
-            messages.append({"role": "user", "content": text})
+            messages.append({"role": "user", "content": [{"type": "text", "text": text}]})
         
         except Exception as ex:
             self.logger.error(f"Error at build_messages: {ex}\n{traceback.format_exc()}")
 
         return messages
 
+    async def messages_create_stream(self, async_client: AsyncAnthropic, messages: list, call_functions: bool=True):
+        params = {
+            "messages": messages,
+            "model": self.model,
+            "temperature": self.temperature,
+            "max_tokens": self.max_tokens,
+            "stream": True,
+        }
+
+        if self.system_message_content:
+            params["system"] = self.system_message_content
+
+        if call_functions and self.functions:
+            params["tools"] = [v.get_spec() for _, v in self.functions.items()]
+
+        return await async_client.beta.tools.messages.create(**params)
+
     async def chat(self, text: str) -> AsyncGenerator[str, None]:
         try:
             async_client = AsyncAnthropic(api_key=self.api_key)
 
             if (datetime.utcnow() - self.last_chat_at).total_seconds() > self.history_timeout:
                 self.reset_histories()
 
             if self.on_start_processing:
                 await self.on_start_processing()
 
             # Get context
-            messages = self.build_messages(text)
+            messages = await self.build_messages(text)
 
-            # Params
-            params = {
-                "messages": messages,
-                "model": self.model,
-                "temperature": self.temperature,
-                "max_tokens": self.max_tokens,
-                "stream": True,
-            }
-            if self.system_message_content:
-                params["system"] = self.system_message_content
+            # Process stream response
+            stream_resp = await self.messages_create_stream(async_client, messages)
 
-            # Stream
+            content_block_type = ""
             response_text = ""
-            stream_resp = await async_client.messages.create(**params)
+            tool_use_id = ""
+            function_name = ""
+            function_arguments_str = ""
+
             async for chunk in stream_resp:
-                if chunk.type == "content_block_delta":
-                    content = chunk.delta.text
-                    response_text += content
-                    yield content
-            
-            # Save context
+                if chunk.type == "content_block_start":
+                    content_block_type = chunk.content_block.type
+                    if content_block_type == "tool_use":
+                        # Set tool info from start block
+                        tool_use_id = chunk.content_block.id
+                        function_name = chunk.content_block.name
+
+                elif chunk.type == "content_block_delta":
+                    if content_block_type == "text":
+                        # yield content
+                        content = chunk.delta.text
+                        response_text += content
+                        yield content
+                    elif content_block_type == "tool_use":
+                        # correct chunked args
+                        function_arguments_str += chunk.delta.partial_json
+
+                elif chunk.type == "content_block_stop":
+                    if content_block_type == "tool_use":
+                        function_arguments = json.loads(function_arguments_str)
+
+                        # Make context
+                        contents = []
+                        if response_text:
+                            # Add text content response includes text message before function
+                            contents.append({
+                                "type": "text",
+                                "text": response_text
+                            })
+
+                        contents.append({
+                            "type": "tool_use",
+                            "id": tool_use_id,
+                            "name": function_name,
+                            "input": function_arguments
+                        })
+
+                        messages.append({
+                            "role": "assistant",
+                            "content": contents
+                        })
+
+                        # Add messages to history
+                        self.histories.append(messages[-2])
+                        self.histories.append(messages[-1])
+
+                        # Call function
+                        api_resp = await self.functions[function_name].func(**function_arguments)
+
+                        # Convert API response to human friendly response
+                        messages.append({
+                            "role": "user",
+                            "content": [{
+                                "type": "tool_result",
+                                "tool_use_id": tool_use_id,
+                                "content": json.dumps(api_resp)
+                            }]
+                        })
+
+                        response_text = ""
+                        stream_resp = await self.messages_create_stream(async_client, messages)
+
+                        async for chunk in stream_resp:
+                            if chunk.type == "content_block_delta":
+                                content = chunk.delta.text
+                                response_text += content
+                                yield content
+
+            # Save context after receiving stream
             if response_text:
                 self.histories.append(messages[-1])
                 self.histories.append({"role": "assistant", "content": response_text})
 
         except Exception as ex:
             self.logger.error(f"Error at chat: {str(ex)}\n{traceback.format_exc()}")
             raise ex
         
         finally:
             self.last_chat_at = datetime.utcnow()
             if not async_client.is_closed():
                 await async_client.close()
+
+
+class ClaudeProcessorWithVisionBase(ClaudeProcessor):
+    def __init__(self, *, api_key: str, model: str = "claude-3-sonnet-20240229", temperature: float = 1, max_tokens: int = 200, functions: dict = None, system_message_content: str = None, history_count: int = 10, history_timeout: float = 60, use_vision: bool = True):
+        super().__init__(api_key=api_key, model=model, temperature=temperature, max_tokens=max_tokens, functions=functions, system_message_content=system_message_content, history_count=history_count, history_timeout=history_timeout)
+        self.use_vision = use_vision
+        self.is_vision_required_func = {
+            "name": "is_vision_required",
+            "description": "Determine whether the vision input is required to process the user input.",
+            "input_schema": {
+                "type": "object",
+                "properties": {
+                    "is_required": {"type": "boolean"}
+                },
+                "required": ["is_required"]
+            }
+        }
+
+    @abstractmethod
+    async def get_image(self) -> bytes:
+        pass
+
+    async def build_messages(self, text):
+        messages = await super().build_messages(text)
+        if not self.use_vision:
+            return messages
+
+        if len(self.histories) > 1:
+            last_user_message = self.histories[-2:-1][0]
+            if isinstance(last_user_message["content"], list):
+                for i in range(len(last_user_message["content"]) - 1, -1, -1):
+                    # Remove image from last request
+                    if last_user_message["content"][i]["type"] == "image":
+                        del last_user_message["content"][i]
+
+        async_client = AsyncAnthropic(api_key=self.api_key)
+        try:
+            # Determine whether the vision input is required to process the user input
+            params = {
+                "messages": messages[:-1] + [{
+                    "role": "user",
+                    "content": f"以下はユーザーからの入力内容です。このメッセージを処理するために新たな画像の入力が必要か判断してください。\n\n入力: {text}"
+                }],
+                "model": self.model,
+                "temperature": self.temperature,
+                "max_tokens": self.max_tokens,
+                "system": self.system_message_content,
+                "tools": [self.is_vision_required_func],
+                "tool_choice": {"type": "tool", "name": "is_vision_required"},
+                "stream": False,
+            }
+
+            resp = await async_client.beta.tools.messages.create(**params)
+
+            if resp.content[0].input["is_required"] is True:
+                self.logger.info("Vision input is required")
+                image_bytes = await self.get_image()
+                image_b64 = base64.b64encode(image_bytes).decode("utf-8")
+                messages[-1]["content"].append({
+                    "type": "image",
+                    "source": {
+                        "type": "base64",
+                        "media_type": "image/png",
+                        "data": image_b64,
+                    }
+                })
+
+        except Exception as ex:
+            self.logger.error(f"Error at build_messages: {str(ex)}\n{traceback.format_exc()}")
+
+        finally:
+            self.last_chat_at = datetime.utcnow()
+            if not async_client.is_closed():
+                await async_client.close()
+
+        return messages
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## aiavatar/processors/gemini.py

```diff
@@ -1,86 +1,240 @@
+from abc import abstractmethod
+import base64
 from datetime import datetime
 from logging import getLogger, NullHandler
 import traceback
-from typing import AsyncGenerator
+from typing import Callable, AsyncGenerator
 import google.generativeai as genai
+import google.ai.generativelanguage as glm
+from google.protobuf.struct_pb2 import Struct
 from . import ChatProcessor
 
+
+class GeminiFunction:
+    def __init__(self, name: str, description: str=None, parameters: dict=None, func: Callable=None):
+        self.name = name
+        self.description = description
+        self.parameters = parameters
+        self.func = func
+    
+    def get_spec(self):
+        return genai.types.FunctionDeclaration(
+            name=self.name,
+            description=self.description,
+            parameters=self.parameters
+        )
+
+
 class GeminiProcessor(ChatProcessor):
-    def __init__(self, *, api_key: str, model: str="gemini-pro", temperature: float=1.0, max_tokens: int=200, functions: dict=None, system_message_content: str=None, system_message_content_acknowledgement_content: str="了解しました。", history_count: int=10, history_timeout: float=60.0):
+    def __init__(self, *, api_key: str, model: str="gemini-1.5-flash-latest", temperature: float=1.0, max_tokens: int=200, functions: dict=None, system_message_content: str=None, history_count: int=10, history_timeout: float=60.0):
         self.logger = getLogger(__name__)
         self.logger.addHandler(NullHandler())
 
         self.api_key = api_key
         self.model = model
         self.temperature = temperature
         self.max_tokens = max_tokens
-        self.system_message_content = system_message_content
-        self.system_message_content_acknowledgement_content = system_message_content_acknowledgement_content
+        self.functions = functions
         self.history_count = history_count
         self.history_timeout = history_timeout
         self.histories = []
         self.last_chat_at = datetime.utcnow()
         self.on_start_processing = None
+        self.dump_messages = False
 
         genai.configure(api_key=self.api_key)
         self.client = genai.GenerativeModel(self.model)
+        # Set system_message_content after creating client
+        if system_message_content:
+            self.system_message_content = system_message_content
+
+    @property
+    def system_message_content(self):
+        if not self.client._system_instruction:
+            return None
+        return self.client._system_instruction["parts"][0]["text"]
+    
+    @system_message_content.setter
+    def system_message_content(self, value):
+        self.client._system_instruction = {"role": "user", "parts": [{"text": value}]}
+
+    def add_function(self, name: str, description: str=None, parameters: dict=None, func: Callable=None):
+        self.functions[name] = GeminiFunction(name=name, description=description, parameters=parameters, func=func)
 
     def reset_histories(self):
         self.histories.clear()
 
-    def build_messages(self, text):
+    async def build_messages(self, text):
         messages = []
         try:
-            # System message
-            if self.system_message_content:
-                messages.append({"role": "user", "parts": [{"text": self.system_message_content}]})
-                messages.append({"role": "model", "parts": [{"text": self.system_message_content_acknowledgement_content}]})
-
             # Histories
             messages.extend(self.histories[-1 * self.history_count:])
 
+            if len(messages) > 0:
+                part = messages[0]["parts"][0]
+                if isinstance(part, glm.Part) and part.function_response:
+                    # Invalid context if it starts with function_response
+                    del messages[0]
+
             # Current user message
             messages.append({"role": "user", "parts": [{"text": text}]})
         
         except Exception as ex:
             self.logger.error(f"Error at build_messages: {ex}\n{traceback.format_exc()}")
 
         return messages
 
+    async def generate_content_stream(self, messages: list, call_functions: bool=True):
+        # Params
+        generation_config = {
+            "temperature": self.temperature
+        }
+        if self.max_tokens:
+            generation_config["max_output_tokens"] = self.max_tokens
+
+        tools = [v.get_spec() for _, v in self.functions.items()] \
+            if call_functions and self.functions else None
+
+        if self.dump_messages:
+            self.logger.info(f"messages to generate_content:\n{messages}")
+
+        return await self.client.generate_content_async(
+            messages,
+            generation_config=generation_config,
+            tools=tools,
+            stream=True
+        )
+
     async def chat(self, text: str) -> AsyncGenerator[str, None]:
         try:
             if (datetime.utcnow() - self.last_chat_at).total_seconds() > self.history_timeout:
                 self.reset_histories()
 
             if self.on_start_processing:
                 await self.on_start_processing()
 
             # Get context
-            messages = self.build_messages(text)
+            messages = await self.build_messages(text)
 
-            # Params
-            generation_config = {
-                "temperature": self.temperature
-            }
-            if self.max_tokens:
-                generation_config["max_output_tokens"] = self.max_tokens
-
-            # Stream
+            # Process stream response
             response_text = ""
-            stream_resp = await self.client.generate_content_async(messages, generation_config=generation_config)
+            stream_resp = await self.generate_content_stream(messages)
+
             async for chunk in stream_resp:
-                content = chunk.candidates[0].content.parts[0].text
-                response_text += content
-                yield content
+                if chunk.candidates and chunk.candidates[0].content.parts:
+                    for part in chunk.candidates and chunk.candidates[0].content.parts:
+                        if function_call := part.function_call:
+                            # Make context
+                            parts = []
+                            if response_text:
+                                # Add text content response includes text message before function
+                                parts.append({"text": response_text})                            
+                            parts.append(part)
+                            messages.append({"role": "model", "parts": parts})
+
+                            # Add messages to history
+                            self.histories.append(messages[-2])
+                            self.histories.append(messages[-1])
+
+                            # Call function
+                            called_func = self.functions[function_call.name]
+                            api_resp = await called_func.func(**dict(function_call.args))
+
+                            # Build function response
+                            # See also: https://github.com/google-gemini/generative-ai-python/issues/243
+                            s = Struct()
+                            s.update({"result": api_resp})
+                            function_response = glm.Part(
+                                function_response=glm.FunctionResponse(name=function_call.name, response=s)
+                            )
+
+                            # Convert API response to human friendly response
+                            messages.append({"role": "user", "parts": [function_response]})
+
+                            response_text = ""
+                            stream_resp = await self.generate_content_stream(messages, False)
+
+                            async for chunk in stream_resp:
+                                if chunk.candidates and chunk.candidates[0].content.parts:
+                                    content = chunk.candidates[0].content.parts[0].text
+                                    response_text += content
+                                    yield content
+
+                        else:
+                            content = chunk.candidates[0].content.parts[0].text
+                            response_text += content
+                            yield content
 
-            # Save context
+            # Save context after receiving stream
             if response_text:
                 self.histories.append(messages[-1])
                 self.histories.append({"role": "model", "parts": [{"text": response_text}]})
 
         except Exception as ex:
             self.logger.error(f"Error at chat: {str(ex)}\n{traceback.format_exc()}")
             raise ex
         
         finally:
             self.last_chat_at = datetime.utcnow()
+
+
+class GeminiProcessorWithVisionBase(GeminiProcessor):
+    def __init__(self, *, api_key: str, model: str = "gemini-1.5-flash-latest", temperature: float = 1, max_tokens: int = 200, functions: dict = None, system_message_content: str = None, history_count: int = 10, history_timeout: float = 60, use_vision: bool = True):
+        super().__init__(api_key=api_key, model=model, temperature=temperature, max_tokens=max_tokens, functions=functions, system_message_content=system_message_content, history_count=history_count, history_timeout=history_timeout)
+        self.use_vision = use_vision
+        self.is_vision_required_func = genai.types.FunctionDeclaration(
+            name="is_vision_required",
+            description="Determine whether the vision input is required to process the user input.",
+            parameters={
+                "type": "object",
+                "properties": {
+                    "is_required": {"type": "boolean"}
+                },
+                "required": ["is_required"]
+            }
+        )
+
+    @abstractmethod
+    async def get_image(self) -> bytes:
+        pass
+
+    async def build_messages(self, text):
+        messages = await super().build_messages(text)
+        if not self.use_vision:
+            return messages
+
+        if len(self.histories) > 1:
+            last_user_message = self.histories[-2:-1][0]
+            for i in range(len(last_user_message["parts"]) - 1, -1, -1):
+                # Remove image from last request
+                part = last_user_message["parts"][i]
+                if isinstance(part, dict) and part.get("mime_type"):
+                    del last_user_message["parts"][i]
+
+        try:
+            # Determine whether the vision input is required to process the user input
+            resp = await self.client.generate_content_async(
+                messages[:-1] + [{
+                    "role": "user",
+                    "parts": [{
+                        "text": f"以下はユーザーからの入力内容です。このメッセージを処理するために新たな画像の入力が必要か判断してください。\n\n入力: {text}"
+                    }]
+                }],
+                generation_config={"temperature": 0.0},
+                tools=[self.is_vision_required_func],
+                tool_config=glm.ToolConfig(function_calling_config=glm.FunctionCallingConfig(mode=glm.FunctionCallingConfig.Mode.ANY)),
+                stream=False
+            )
+
+            for part in resp.candidates[0].content.parts:
+                if part.function_call:
+                    if dict(part.function_call.args)["is_required"] is True:
+                        self.logger.info("Vision input is required")
+                        image_bytes = await self.get_image()
+                        image_b64 = base64.b64encode(image_bytes).decode("utf-8")
+                        messages[-1]["parts"].append({"mime_type": "image/png", "data": image_b64})
+
+        except Exception as ex:
+            self.logger.error(f"Error at build_messages: {str(ex)}\n{traceback.format_exc()}")
+
+        return messages
```

## Comparing `aiavatar-0.5.6.dist-info/LICENSE` & `aiavatar-0.5.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `aiavatar-0.5.6.dist-info/METADATA` & `aiavatar-0.5.7.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiavatar
-Version: 0.5.6
+Version: 0.5.7
 Summary: 🥰 Building AI-based conversational avatars lightning fast ⚡️💬
 Home-page: https://github.com/uezo/aiavatar
 Author: uezo
 Author-email: uezo@uezo.net
 Maintainer: uezo
 Maintainer-email: uezo@uezo.net
 License: Apache v2
@@ -91,15 +91,15 @@
   - [🎭 Custom Behavior](#-custom-behavior)
 - [🌎 Platform Guide](#-platform-guide)
   - [🐈 VRChat](#-vrchat)
   - [🍓 Raspberry Pi](#-raspberry-pi)
 - [🧩 RESTful APIs](#-restful-apis)
 - [🤿 Deep Dive](#-deep-dive)
   - [⚡️ Function Calling](#️-function-calling)
-  - [👀 Vision](#️-vision)
+  - [👀 Vision](#-vision)
 - [🔍 Other Tips](#-other-tips)
   - [🎤 Testing Audio I/O](#-testing-audio-io)
   - [🎚️ Noise Filter](#-noise-filter)
   - [🧪 LM Studio API](#-lm-studio-api)
   - [⚡️ Use Custom Listener](#️-use-custom-listener)
 
 
@@ -783,15 +783,15 @@
     "name": "get_weather"
 }
 ```
 
 
 ## 👀 Vision
 
-We provide the experimental support for vision input to ChatGPT. A new class, ChatGPTProcessorWithVisionBase, has been added to handle image inputs, inheriting from ChatGPTProcessor.
+We provide the experimental support for vision input to ChatGPT, Claude and Gemini. Add `ChatGPTProcessorWithVisionBase`, `ClaudeProcessorWithVisionBase` and `GeminiProcessorWithVisionBase` to handle image inputs, inheriting from processors.
 
 An example implementation, ChatGPTProcessorWithVisionScreenShot, demonstrates how to capture screenshots using pyautogui. This gives "eyes" to your AIAvatar in metaverse platforms like VRChat.
 
 ```python
 import io
 import pyautogui
 
@@ -814,14 +814,16 @@
 
 app = AIAvatar(
     google_api_key=GOOGLE_API_KEY,
     chat_processor=chat_processor
 )
 ```
 
+You can also adapt the same method for handling vision input with Claude and Gemini.
+
 **NOTE**
 
 * Only the latest image will be sent to ChatGPT to avoid performance issues.
 * The system uses function calling to determine if image retrieval is necessary, which adds approximately 500 milliseconds to 1 second to the processing time.
 
 
 # 🔍 Other Tips
```

## Comparing `aiavatar-0.5.6.dist-info/RECORD` & `aiavatar-0.5.7.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -14,20 +14,20 @@
 aiavatar/listeners/azurevoicerequest.py,sha256=3DHxZl9uPLEvVH2c1gpbBmwUcVFlPaOzyO35JrIXyoc,2773
 aiavatar/listeners/azurewakeword.py,sha256=2GP_bUi56oFjARXGKFHES_KztA_MBNdiXkbYkor1eCQ,4951
 aiavatar/listeners/openailisteners.py,sha256=hSsKDTkCFO80w7xt2Nq_zUHdohM9zbP5BmOKF_H5vBM,1655
 aiavatar/listeners/voicerequest.py,sha256=6h86YcMXUX_yFd5AAMo4zeQ80xhPTUwhSCQzgWd4ZuY,976
 aiavatar/listeners/wakeword.py,sha256=ZEGGKn5gmNZ8woSUKEbgLJX7o5iR3JD1rG3rRhoehoY,1132
 aiavatar/processors/__init__.py,sha256=k6qF1_UopWpaxQ89OxP7-dSVLgnrDCuuZH0Gom0JLLU,178
 aiavatar/processors/chatgpt.py,sha256=L5-DoXHdZ-BUro7af0yXT4i5BF-6En7Ch0meXuEkPSA,9911
-aiavatar/processors/claude.py,sha256=c56BtK4Qsi-I4tQw0J_Jvflgu9bNXpCVV-EMqZEMhV0,3110
-aiavatar/processors/gemini.py,sha256=9cRMEpxFHsoxABysoPch-CPMUkRdD0-gO5AaqxRsuYk,3388
+aiavatar/processors/claude.py,sha256=raAElJVOD4Zr0zEdRJjC5hltVUQ4jKyT0-A-uvwpw8E,10457
+aiavatar/processors/gemini.py,sha256=IWHYgN-w9Rccz1v2I27dEh8Te5zhBNINqLvY9sK9suE,10397
 aiavatar/speech/__init__.py,sha256=MugrpbtCQGpDOlBegVFZjuBMxNAx3azEsjoC8XsU9Ss,2712
 aiavatar/speech/azurespeech.py,sha256=P8lnUMj4j8BRnasxCxCb-xkkFA13BvHUG03aZ04RXNU,1887
 aiavatar/speech/openaispeech.py,sha256=IHVdK2o2yh7upZtu-JkQiSz2_OOdofjzzLRYbLSXSl0,1474
 aiavatar/speech/voicevox.py,sha256=HFrtZjE6Q8YNot-WTVEH6kTw8vpG5QxCvK2NUy1WTG4,1348
 aiavatar/speech/soundplayers/__init__.py,sha256=71xYi-8qaInz_Um8wV5zDaHpAB5sTJG9osn17aQAUKQ,220
 aiavatar/speech/soundplayers/sounddevice_player.py,sha256=dDMdlSVdgHFiDNiGxezTon3pLnm8vGia_ftX0URKEm0,2175
-aiavatar-0.5.6.dist-info/LICENSE,sha256=UOZ1F5fFDe3XXvG4oNnkL1-Ecun7zpHzRxjp-XsMeAo,11324
-aiavatar-0.5.6.dist-info/METADATA,sha256=5oP2uioH61UdQBN0UPCvAXGgdoP4hi5KyQludPxNAvY,27979
-aiavatar-0.5.6.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-aiavatar-0.5.6.dist-info/top_level.txt,sha256=B14WVaakM_kKuOkCeI-WRP83BJ6APkOyQrn6EXxs8kg,9
-aiavatar-0.5.6.dist-info/RECORD,,
+aiavatar-0.5.7.dist-info/LICENSE,sha256=UOZ1F5fFDe3XXvG4oNnkL1-Ecun7zpHzRxjp-XsMeAo,11324
+aiavatar-0.5.7.dist-info/METADATA,sha256=r3v0PipnqhTJbC33ou4rJ9JEaLQETWQCSVgWIAVrQYg,28121
+aiavatar-0.5.7.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+aiavatar-0.5.7.dist-info/top_level.txt,sha256=B14WVaakM_kKuOkCeI-WRP83BJ6APkOyQrn6EXxs8kg,9
+aiavatar-0.5.7.dist-info/RECORD,,
```

