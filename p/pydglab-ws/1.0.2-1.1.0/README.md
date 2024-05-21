# Comparing `tmp/pydglab_ws-1.0.2.tar.gz` & `tmp/pydglab_ws-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydglab_ws-1.0.2.tar", max compression
+gzip compressed data, was "pydglab_ws-1.1.0.tar", max compression
```

## Comparing `pydglab_ws-1.0.2.tar` & `pydglab_ws-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1535 2024-05-20 06:36:18.807150 pydglab_ws-1.0.2/LICENSE
--rw-r--r--   0        0        0     6092 2024-05-20 06:36:18.807150 pydglab_ws-1.0.2/README.md
--rw-r--r--   0        0        0      179 2024-05-20 06:36:18.811150 pydglab_ws-1.0.2/pydglab_ws/__init__.py
--rw-r--r--   0        0        0       82 2024-05-20 06:36:18.811150 pydglab_ws-1.0.2/pydglab_ws/client/__init__.py
--rw-r--r--   0        0        0     9795 2024-05-20 06:36:18.811150 pydglab_ws-1.0.2/pydglab_ws/client/base.py
--rw-r--r--   0        0        0      923 2024-05-20 06:36:18.811150 pydglab_ws-1.0.2/pydglab_ws/client/connect.py
--rw-r--r--   0        0        0     1552 2024-05-20 06:36:18.811150 pydglab_ws-1.0.2/pydglab_ws/client/local.py
--rw-r--r--   0        0        0     1910 2024-05-20 06:36:18.811150 pydglab_ws-1.0.2/pydglab_ws/client/ws.py
--rw-r--r--   0        0        0     3433 2024-05-20 06:36:18.811150 pydglab_ws-1.0.2/pydglab_ws/enums.py
--rw-r--r--   0        0        0      724 2024-05-20 06:36:18.811150 pydglab_ws-1.0.2/pydglab_ws/exceptions.py
--rw-r--r--   0        0        0     3214 2024-05-20 06:36:18.811150 pydglab_ws-1.0.2/pydglab_ws/models.py
--rw-r--r--   0        0        0       22 2024-05-20 06:36:18.811150 pydglab_ws-1.0.2/pydglab_ws/server/__init__.py
--rw-r--r--   0        0        0    17992 2024-05-20 06:36:18.811150 pydglab_ws-1.0.2/pydglab_ws/server/server.py
--rw-r--r--   0        0        0      755 2024-05-20 06:36:18.811150 pydglab_ws-1.0.2/pydglab_ws/typing.py
--rw-r--r--   0        0        0     4032 2024-05-20 06:36:18.811150 pydglab_ws-1.0.2/pydglab_ws/utils.py
--rw-r--r--   0        0        0     1293 2024-05-20 06:36:18.811150 pydglab_ws-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     7176 1970-01-01 00:00:00.000000 pydglab_ws-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1535 2024-05-21 13:57:42.662510 pydglab_ws-1.1.0/LICENSE
+-rw-r--r--   0        0        0     6092 2024-05-21 13:57:42.662510 pydglab_ws-1.1.0/README.md
+-rw-r--r--   0        0        0      179 2024-05-21 13:57:42.666510 pydglab_ws-1.1.0/pydglab_ws/__init__.py
+-rw-r--r--   0        0        0       82 2024-05-21 13:57:42.666510 pydglab_ws-1.1.0/pydglab_ws/client/__init__.py
+-rw-r--r--   0        0        0    10837 2024-05-21 13:57:42.666510 pydglab_ws-1.1.0/pydglab_ws/client/base.py
+-rw-r--r--   0        0        0     1182 2024-05-21 13:57:42.666510 pydglab_ws-1.1.0/pydglab_ws/client/connect.py
+-rw-r--r--   0        0        0     1552 2024-05-21 13:57:42.666510 pydglab_ws-1.1.0/pydglab_ws/client/local.py
+-rw-r--r--   0        0        0     2335 2024-05-21 13:57:42.666510 pydglab_ws-1.1.0/pydglab_ws/client/ws.py
+-rw-r--r--   0        0        0     3433 2024-05-21 13:57:42.666510 pydglab_ws-1.1.0/pydglab_ws/enums.py
+-rw-r--r--   0        0        0      919 2024-05-21 13:57:42.666510 pydglab_ws-1.1.0/pydglab_ws/exceptions.py
+-rw-r--r--   0        0        0     3304 2024-05-21 13:57:42.666510 pydglab_ws-1.1.0/pydglab_ws/models.py
+-rw-r--r--   0        0        0       22 2024-05-21 13:57:42.666510 pydglab_ws-1.1.0/pydglab_ws/server/__init__.py
+-rw-r--r--   0        0        0    18028 2024-05-21 13:57:42.666510 pydglab_ws-1.1.0/pydglab_ws/server/server.py
+-rw-r--r--   0        0        0      755 2024-05-21 13:57:42.666510 pydglab_ws-1.1.0/pydglab_ws/typing.py
+-rw-r--r--   0        0        0     4826 2024-05-21 13:57:42.666510 pydglab_ws-1.1.0/pydglab_ws/utils.py
+-rw-r--r--   0        0        0     1293 2024-05-21 13:57:42.666510 pydglab_ws-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     7176 1970-01-01 00:00:00.000000 pydglab_ws-1.1.0/PKG-INFO
```

### Comparing `pydglab_ws-1.0.2/LICENSE` & `pydglab_ws-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydglab_ws-1.0.2/README.md` & `pydglab_ws-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pydglab_ws-1.0.2/pydglab_ws/client/base.py` & `pydglab_ws-1.1.0/pydglab_ws/client/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -107,26 +107,28 @@
             client_id=self._client_id,
             target_id=self._target_id,
             message=msg
         )
         await self._send(message)
 
     @staticmethod
-    def _handle_msg(message: WebSocketMessage) -> Optional[Union[StrengthData, FeedbackButton]]:
+    def _handle_msg(message: WebSocketMessage) -> Optional[Union[StrengthData, FeedbackButton, RetCode]]:
         """
         处理类型为 ``msg`` 的消息
 
         :raise InvalidStrengthData: [`InvalidStrengthData`][pydglab_ws.exceptions.InvalidStrengthData]
         :raise InvalidFeedbackData: [`InvalidFeedbackData`][pydglab_ws.exceptions.InvalidFeedbackData]
         """
         if isinstance(message.message, str):
             if message.message.startswith(MessageDataHead.STRENGTH.value):
                 return parse_strength_data(message.message)
             elif message.message.startswith(MessageDataHead.FEEDBACK.value):
                 return parse_feedback_data(message.message)
+        elif isinstance(message.message, RetCode):
+            return message.message
         return None
 
     @staticmethod
     def _handle_break(message: WebSocketMessage) -> Optional[Literal[RetCode.CLIENT_DISCONNECTED]]:
         """处理类型为 ``break`` 的消息"""
         return message.message
 
@@ -162,24 +164,38 @@
         while self.not_bind:
             message = await self._recv_owned()
             if message.type == MessageType.BIND and isinstance(message.message, RetCode):
                 if message.message == RetCode.SUCCESS:
                     self._target_id = message.target_id
                 return message.message
 
+    async def rebind(self) -> RetCode:
+        """
+        清除 ``target_id``，重新等待与 DG-Lab App 的关系绑定，适合 App 断开连接后调用
+        :return: 响应码
+        """
+        self._target_id = None
+        while self.not_bind:
+            message = await self._recv_owned()
+            if message.type == MessageType.BIND and isinstance(message.message, RetCode):
+                if message.message == RetCode.SUCCESS:
+                    self._target_id = message.target_id
+                return message.message
+
     async def recv_data(self) -> Union[StrengthData, FeedbackButton, RetCode]:
         """
         获取 WebSocket 服务端的数据
 
         注意，获取到的是队列中最早的数据，可能不是最新的
 
         :return: 可能为 **强度数据** - [`StrengthData`][pydglab_ws.models.StrengthData]、 \
-            **App 反馈数据** - [`FeedbackButton`][pydglab_ws.enums.FeedbackButton] \
-            、**心跳** - [`RetCode.SUCCESS`][pydglab_ws.enums.RetCode]、 \
-            **App 断开连接** - [`RetCode.CLIENT_DISCONNECTED`][pydglab_ws.enums.RetCode]
+            **App 反馈数据** - [`FeedbackButton`][pydglab_ws.enums.FeedbackButton]、 \
+            **心跳** - [`RetCode.SUCCESS`][pydglab_ws.enums.RetCode.SUCCESS]、 \
+            **App 断开连接** - [`RetCode.CLIENT_DISCONNECTED`][pydglab_ws.enums.RetCode.CLIENT_DISCONNECTED]、\
+            **消息长度大于 1950** - [`RetCode.MESSAGE_TOO_LONG`][pydglab_ws.enums.RetCode.MESSAGE_TOO_LONG]
         :raise InvalidStrengthData: [`InvalidStrengthData`][pydglab_ws.exceptions.InvalidStrengthData]
         :raise InvalidFeedbackData: [`InvalidFeedbackData`][pydglab_ws.exceptions.InvalidFeedbackData]
         """
         await self.ensure_bind()
         while True:
             message = await self._recv_owned()
             handler = self._message_type_to_handler.get(message.type)
@@ -240,14 +256,16 @@
         - 每条波形数据代表了 100ms 的数据，所以若每次发送的数据有 10 条，那么就是 1s 的数据。 \
           由于网络有一定延时，若要保证波形输出的连续性，建议波形数据的发送间隔略微小于波形数据的时间长度 (< 1s)
         - 数组最大长度为 100,也就是最多放置 10s 的数据，另外 App 中的波形队列最大长度为 500，即为 50s 的数据， \
           若后接收到的数据无法全部放入波形队列，多余的部分会丢弃。所以谨慎考虑您的数据长度和数据发送间隔
 
         :param channel: 通道选择
         :param pulses: 波形操作数据，最大长度为 100
+        :raise InvalidPulseOperation: [`InvalidPulseOperation`][pydglab_ws.exceptions.InvalidPulseOperation]
+        :raise PulseDataTooLong: 波形操作数据过长，最大长度应为 [`PULSE_DATA_MAX_LENGTH`][pydglab_ws.utils.PULSE_DATA_MAX_LENGTH]
         """
         await self.ensure_bind()
         await self._send_owned(
             MessageType.MSG,
             dump_add_pulses(channel, *pulses)
         )
```

### Comparing `pydglab_ws-1.0.2/pydglab_ws/client/connect.py` & `pydglab_ws-1.1.0/pydglab_ws/client/connect.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,21 +13,24 @@
     ```python3
     async with DGLabWSConnect("ws://localhost:5678") as client:
         await client.bind()
         print("成功绑定")
     ```
 
     :param uri: WebSocket 服务端 Uri
+    :param register_timeout: 终端注册（获取 ``clientId``）超时时间
     :param kwargs: :class:`websockets.client.connect` 的其他参数
+    :raise asyncio.Timeout: 终端注册（获取 ``clientId``）超时
     """
 
-    def __init__(self, uri: str, **kwargs):
+    def __init__(self, uri: str, register_timeout: float = None, **kwargs):
         self._connect = ws_connect(uri=uri, **kwargs)
+        self._register_timeout = register_timeout
 
     async def __aenter__(self) -> DGLabWSClient:
         websocket = await self._connect.__aenter__()
-        dg_lab_ws_client = DGLabWSClient(websocket)
-        await dg_lab_ws_client.register()
+        dg_lab_ws_client = DGLabWSClient(websocket, self._register_timeout)
+        await dg_lab_ws_client.__aenter__()
         return dg_lab_ws_client
 
     async def __aexit__(self, exc_type, exc_val, exc_tb):
         await self._connect.__aexit__(exc_type, exc_val, exc_tb)
```

### Comparing `pydglab_ws-1.0.2/pydglab_ws/client/local.py` & `pydglab_ws-1.1.0/pydglab_ws/client/local.py`

 * *Files identical despite different names*

### Comparing `pydglab_ws-1.0.2/pydglab_ws/client/ws.py` & `pydglab_ws-1.1.0/pydglab_ws/client/ws.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import asyncio
 import ipaddress
 from ssl import SSLSocket
 from typing import Optional
 
 from websockets import WebSocketClientProtocol
 
 from .base import DGLabClient
@@ -11,33 +12,39 @@
 
 
 class DGLabWSClient(DGLabClient):
     """
     DG-Lab WebSocket 终端
 
     :param websocket: 与 WebSocket 服务端的连接
+    :param register_timeout: 终端注册（获取 ``clientId``）超时时间
+    :raise asyncio.Timeout: 终端注册（获取 ``clientId``）超时
     """
 
-    def __init__(self, websocket: WebSocketClientProtocol):
+    def __init__(self, websocket: WebSocketClientProtocol, register_timeout: float = None):
         super().__init__()
         self._websocket = websocket
+        self._register_timeout = register_timeout
 
     async def __aenter__(self) -> "DGLabWSClient":
-        await self.register()
+        if self._register_timeout is not None:
+            await asyncio.wait_for(self.register(), self._register_timeout)
+        else:
+            await self.register()
         return self
 
     async def __aexit__(self, exc_type, exc_val, exc_tb):
         pass
 
     async def _recv(self) -> WebSocketMessage:
         raw_message = await self._websocket.recv()
         return WebSocketMessage.model_validate_json(raw_message)
 
     async def _send(self, message: WebSocketMessage):
-        await self._websocket.send(message.model_dump_json(by_alias=True))
+        await self._websocket.send(message.model_dump_json(by_alias=True, context={"separators": (",", ":")}))
 
     def get_qrcode(self, uri: str = None) -> Optional[str]:
         if uri is None and (remote_address := self._websocket.remote_address):
             host, port = remote_address
             try:
                 is_v6 = ipaddress.ip_address(host).version == 6
             except ValueError:
```

### Comparing `pydglab_ws-1.0.2/pydglab_ws/enums.py` & `pydglab_ws-1.1.0/pydglab_ws/enums.py`

 * *Files identical despite different names*

### Comparing `pydglab_ws-1.0.2/pydglab_ws/exceptions.py` & `pydglab_ws-1.1.0/pydglab_ws/exceptions.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 此处定义了一些异常类
 """
-__all__ = ("InvalidStrengthData", "InvalidFeedbackData", "InvalidPulseOperation")
+__all__ = ("InvalidStrengthData", "InvalidFeedbackData", "InvalidPulseOperation", "PulseDataTooLong")
 
 from typing import Any
 
 
 class InvalidStrengthData(Exception):
     """强度数据不合法"""
 
@@ -21,7 +21,14 @@
 
 
 class InvalidPulseOperation(Exception):
     """波形操作数据不合法"""
 
     def __init__(self, pulse_operation: Any):
         super().__init__(f"Invalid pulse operation: {pulse_operation}")
+
+
+class PulseDataTooLong(Exception):
+    """波形操作数据列表过长"""
+
+    def __init__(self, length: int):
+        super().__init__(f"Pulse data too long: {length}")
```

### Comparing `pydglab_ws-1.0.2/pydglab_ws/models.py` & `pydglab_ws-1.1.0/pydglab_ws/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,18 @@
 from pydantic import BaseModel, UUID4, ConfigDict, field_serializer, AliasGenerator, model_validator, \
     field_validator
 from pydantic.alias_generators import to_camel, to_snake
 from pydantic_core.core_schema import SerializerFunctionWrapHandler, FieldSerializationInfo
 
 from .enums import MessageType, RetCode, MessageDataHead
 
-__all__ = ("WebSocketMessage", "StrengthData")
+__all__ = ("WS_MESSAGE_MAX_LENGTH", "WebSocketMessage", "StrengthData")
+
+WS_MESSAGE_MAX_LENGTH = 1950
+"""WebSocket 消息最大长度"""
 
 
 # noinspection PyNestedDecorators
 class WebSocketMessage(BaseModel):
     """
     WebSocket 消息
```

### Comparing `pydglab_ws-1.0.2/pydglab_ws/server/server.py` & `pydglab_ws-1.1.0/pydglab_ws/server/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,15 +169,15 @@
         发送 WebSocket 消息
 
         :param message: 要发送的消息
         :param wss: 发送目标连接
         """
         for websocket in wss:
             if websocket is not None:
-                await websocket.send(message.model_dump_json(by_alias=True))
+                await websocket.send(message.model_dump_json(by_alias=True, context={"separators": (",", ":")}))
         if to_local_client:
             if queue := self._client_id_to_queue.get(message.client_id):
                 await queue.put(message)
 
     async def _heartbeat_sender(self):
         """
         心跳包发送器
```

### Comparing `pydglab_ws-1.0.2/pydglab_ws/typing.py` & `pydglab_ws-1.1.0/pydglab_ws/typing.py`

 * *Files identical despite different names*

### Comparing `pydglab_ws-1.0.2/pydglab_ws/utils.py` & `pydglab_ws-1.1.0/pydglab_ws/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,28 +2,40 @@
 此处提供一些工具函数
 """
 import json
 
 from pydantic import UUID4
 
 from .enums import StrengthOperationType, Channel, MessageDataHead, FeedbackButton
-from .exceptions import InvalidStrengthData, InvalidFeedbackData, InvalidPulseOperation
-from .models import StrengthData
+from .exceptions import InvalidStrengthData, InvalidFeedbackData, InvalidPulseOperation, PulseDataTooLong
+from .models import StrengthData, WS_MESSAGE_MAX_LENGTH
 from .typing import PulseOperation
 
 __all__ = (
+    "PULSE_DATA_MAX_LENGTH",
     "dump_pulse_operation",
     "dg_lab_client_qrcode",
     "dump_strength_operation",
     "parse_strength_data",
     "dump_add_pulses",
     "dump_clear_pulses",
     "parse_feedback_data"
 )
 
+# {"type":"msg","clientId":"","targetId":"","message":"pulse-A:[]"} - 65bit
+# {"type":"msg","clientId":"`32bit`","targetId":"`32bit`","message":"pulse-A:[]"} - 129bit
+# \"`16bit`\", - 21bit
+# {"type":"msg","clientId":"`32bit`","targetId":"`32bit`","message":"pulse-A:[\"`16bit`\",\"`16bit`\"]"}
+PULSE_DATA_MAX_LENGTH = (WS_MESSAGE_MAX_LENGTH - 129 + 1) // 21  # 86
+"""
+波形操作列表最大长度，计算结果为 ``86``
+
+``(WS_MESSAGE_MAX_LENGTH - 129 + 1) // 21``
+"""
+
 
 def parse_strength_data(data: str) -> StrengthData:
     """
     解析消息中的强度数据
 
     :param data: WebSocket 消息中的 ``message``
     :raise InvalidStrengthData: [`InvalidStrengthData`][pydglab_ws.exceptions.InvalidStrengthData]
@@ -108,16 +120,18 @@
     """
     生成下放波形操作的数据
 
     :param channel: 通道选择
     :param pulses: 波形操作数据
     :return: 返回数据可作为 WebSocket 消息中的 ``message``
     :raise InvalidPulseOperation: [`InvalidPulseOperation`][pydglab_ws.exceptions.InvalidPulseOperation]
+    :raise PulseDataTooLong: 波形操作数据过长，最大长度应为 [`PULSE_DATA_MAX_LENGTH`][pydglab_ws.utils.PULSE_DATA_MAX_LENGTH]
     """
-
+    if (pulses_length := len(pulses)) > PULSE_DATA_MAX_LENGTH:
+        raise PulseDataTooLong(pulses_length)
     return (f"{MessageDataHead.PULSE.value}-{channel.name}"
             f":{json.dumps([dump_pulse_operation(pulse) for pulse in pulses], separators=(',', ':'))}")
 
 
 def dg_lab_client_qrcode(uri: str, client_id: UUID4) -> str:
     """
     生成终端二维码，二维码图像需要自行生成
```

### Comparing `pydglab_ws-1.0.2/pyproject.toml` & `pydglab_ws-1.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydglab-ws"
-version = "1.0.2"
+version = "1.1.0"
 description = "一个通过 WebSocket 控制郊狼 DG-Lab 的 Python 库"
 authors = ["Ljzd-PRO <ljzd@office.ljzd-pro.asia>"]
 readme = "README.md"
 homepage = "https://pydglab-ws.readthedocs.io"
 repository = "https://github.com/Ljzd-PRO/PyDGLab-WS"
 documentation = "https://pydglab-ws.readthedocs.io"
```

### Comparing `pydglab_ws-1.0.2/PKG-INFO` & `pydglab_ws-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydglab-ws
-Version: 1.0.2
+Version: 1.1.0
 Summary: 一个通过 WebSocket 控制郊狼 DG-Lab 的 Python 库
 Home-page: https://pydglab-ws.readthedocs.io
 Keywords: dg-lab,dg-lab-v3,websocket,library,os-independent
 Author: Ljzd-PRO
 Author-email: ljzd@office.ljzd-pro.asia
 Requires-Python: >=3.8
 Classifier: Development Status :: 5 - Production/Stable
```

