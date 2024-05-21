# Comparing `tmp/nonebot_plugin_tsugu_bangdream_bot-0.1.5.tar.gz` & `tmp/nonebot_plugin_tsugu_bangdream_bot-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_tsugu_bangdream_bot-0.1.5.tar", last modified: Sat May 18 08:18:26 2024, max compression
+gzip compressed data, was "nonebot_plugin_tsugu_bangdream_bot-0.1.6.tar", last modified: Tue May 21 06:53:58 2024, max compression
```

## Comparing `nonebot_plugin_tsugu_bangdream_bot-0.1.5.tar` & `nonebot_plugin_tsugu_bangdream_bot-0.1.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1067 2024-05-18 08:18:01.324943 nonebot_plugin_tsugu_bangdream_bot-0.1.5/LICENSE
--rw-r--r--   0        0        0     6897 2024-05-18 08:18:01.324943 nonebot_plugin_tsugu_bangdream_bot-0.1.5/README.md
--rw-r--r--   0        0        0    36868 2024-05-18 08:18:01.324943 nonebot_plugin_tsugu_bangdream_bot-0.1.5/nonebot_plugin_tsugu_bangdream_bot/__init__.py
--rw-r--r--   0        0        0    14448 2024-05-18 08:18:01.324943 nonebot_plugin_tsugu_bangdream_bot-0.1.5/nonebot_plugin_tsugu_bangdream_bot/_commands.py
--rw-r--r--   0        0        0     7846 2024-05-18 08:18:01.324943 nonebot_plugin_tsugu_bangdream_bot-0.1.5/nonebot_plugin_tsugu_bangdream_bot/_utils.py
--rw-r--r--   0        0        0     2456 2024-05-18 08:18:01.324943 nonebot_plugin_tsugu_bangdream_bot-0.1.5/nonebot_plugin_tsugu_bangdream_bot/config.py
--rw-r--r--   0        0        0      569 2024-05-18 08:18:26.424777 nonebot_plugin_tsugu_bangdream_bot-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     7337 1970-01-01 00:00:00.000000 nonebot_plugin_tsugu_bangdream_bot-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-21 06:53:34.798290 nonebot_plugin_tsugu_bangdream_bot-0.1.6/LICENSE
+-rw-r--r--   0        0        0     6897 2024-05-21 06:53:34.798290 nonebot_plugin_tsugu_bangdream_bot-0.1.6/README.md
+-rw-r--r--   0        0        0    31702 2024-05-21 06:53:34.798290 nonebot_plugin_tsugu_bangdream_bot-0.1.6/nonebot_plugin_tsugu_bangdream_bot/__init__.py
+-rw-r--r--   0        0        0    18309 2024-05-21 06:53:34.798290 nonebot_plugin_tsugu_bangdream_bot-0.1.6/nonebot_plugin_tsugu_bangdream_bot/_commands.py
+-rw-r--r--   0        0        0     7846 2024-05-21 06:53:34.798290 nonebot_plugin_tsugu_bangdream_bot-0.1.6/nonebot_plugin_tsugu_bangdream_bot/_utils.py
+-rw-r--r--   0        0        0     2456 2024-05-21 06:53:34.798290 nonebot_plugin_tsugu_bangdream_bot-0.1.6/nonebot_plugin_tsugu_bangdream_bot/config.py
+-rw-r--r--   0        0        0      569 2024-05-21 06:53:58.018528 nonebot_plugin_tsugu_bangdream_bot-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     7337 1970-01-01 00:00:00.000000 nonebot_plugin_tsugu_bangdream_bot-0.1.6/PKG-INFO
```

### Comparing `nonebot_plugin_tsugu_bangdream_bot-0.1.5/LICENSE` & `nonebot_plugin_tsugu_bangdream_bot-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tsugu_bangdream_bot-0.1.5/README.md` & `nonebot_plugin_tsugu_bangdream_bot-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tsugu_bangdream_bot-0.1.5/nonebot_plugin_tsugu_bangdream_bot/_commands.py` & `nonebot_plugin_tsugu_bangdream_bot-0.1.6/nonebot_plugin_tsugu_bangdream_bot/_commands.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,14 +6,30 @@
 import tsugu_api_async
 from tsugu_api_core._typing import _Server, _ServerId, _TsuguUser, _DifficultyText
 
 from .config import CAR, FAKE
 
 from ._utils import server_id_to_full_name
 
+platform = "red"
+"""以 QQ 平台的历史遗留为准，默认所有平台皆为 red 平台，当有获取平台方法时再进行对应处理。"""
+
+async def _get_tsugu_user(user_id: str, platform: str) -> Union[_TsuguUser, str]:
+    try:
+        response = await tsugu_api_async.get_user_data(platform, user_id)
+    except Exception as exception:
+        return f"错误: {exception}"
+    
+    if response["status"] == "failed":
+        assert isinstance(response["data"], str)
+        return response["data"]
+    
+    assert isinstance(response["data"], dict)
+    return response["data"]
+
 async def forward_room(
     room_number: int,
     raw_message: str,
     tsugu_user: _TsuguUser,
     platform: str,
     user_id: str,
     user_name: str,
@@ -73,26 +89,23 @@
         return (
             "已"
             + ("开启" if mode else "关闭")
             + "车牌转发"
         )
 
 async def player_bind(user_id: str, server: Optional[_ServerId]=None) -> Tuple[str, bool, Optional[_ServerId]]:
+    try:
+        tsugu_user = await _get_tsugu_user(user_id, platform)
+    except Exception as exception:
+        return f"错误: {exception}", False, None
+    
+    if isinstance(tsugu_user, str):
+        return tsugu_user, False, None
+    
     if server is None:
-        try:
-            _response = await tsugu_api_async.get_user_data("red", user_id)
-        except Exception as exception:
-            return f"错误: {exception}", False, None
-        
-        if _response["status"] == "failed":
-            assert isinstance(_response["data"], str)
-            return _response["data"], False, None
-        
-        assert isinstance(_response["data"], dict)
-        tsugu_user = _response["data"]
         server = tsugu_user["server_mode"]
     
     try:
         response = await tsugu_api_async.bind_player_request("red", user_id, server, True)
     except Exception as exception:
         return f"错误: {exception}", False, None
     
@@ -106,24 +119,20 @@
         f"正在绑定 {server_id_to_full_name(server)} 账号，"
         + "请将你的\n评论(个性签名)\n或者\n你的当前使用的卡组的卡组名(乐队编队名称)\n改为以下数字后，直接发送你的玩家id\n"
         + f"{verify_code}"
     ), True, server
 
 async def player_unbind(user_id: str, server: Optional[_ServerId]=None) -> Tuple[str, bool, Optional[_ServerId], Optional[int]]:
     try:
-        _response = await tsugu_api_async.get_user_data("red", user_id)
+        tsugu_user = await _get_tsugu_user(user_id, platform)
     except Exception as exception:
         return f"错误: {exception}", False, None, None
     
-    if _response["status"] == "failed":
-        assert isinstance(_response["data"], str)
-        return _response["data"], False, None, None
-    
-    assert isinstance(_response["data"], dict)
-    tsugu_user = _response["data"]
+    if isinstance(tsugu_user, str):
+        return tsugu_user, False, None, None
     
     if server is None:
         server = tsugu_user["server_mode"]
     
     tsugu_user_server = tsugu_user["server_list"][server]
     
     try:
@@ -178,35 +187,42 @@
     
     return (
         f"成功切换默认服务器顺序: {', '.join(server_id_to_full_name(server) for server in servers)}"
     )
 
 async def player_info(user_id: str, server: Optional[_ServerId]=None) -> List[Union[str, bytes]]:
     try:
-        response = await tsugu_api_async.get_user_data("red", user_id)
+        tsugu_user = await _get_tsugu_user(user_id, platform)
     except Exception as exception:
         return [f"错误: {exception}"]
     
-    if response["status"] == "failed":
-        assert isinstance(response["data"], str)
-        return [response["data"]]
-    
-    assert isinstance(response["data"], dict)
-    tsugu_user = response["data"]
+    if isinstance(tsugu_user, str):
+        return [tsugu_user]
     
     if server is None:
         assert isinstance(tsugu_user["server_mode"], int)
         server = tsugu_user["server_mode"]
     
     if (user_server := tsugu_user["server_list"][server])["bindingStatus"] != 2:
         return [f"错误: 未检测到{server_id_to_full_name(server)}的玩家数据"]
     
-    return await search_player(user_server["playerId"], server)
+    return await search_player(user_id, user_server["playerId"], server)
+    
+async def search_player(user_id: str, player_id: int, server: Optional[_Server]=None) -> List[Union[str, bytes]]:
+    if server is None:
+        try:
+            tsugu_user = await _get_tsugu_user(user_id, platform)
+        except Exception as exception:
+            return [f"错误: {exception}"]
+        
+        if isinstance(tsugu_user, str):
+            return [tsugu_user]
+        
+        server = tsugu_user["server_mode"]
     
-async def search_player(player_id: int, server: _Server) -> List[Union[str, bytes]]:
     try:
         response = await tsugu_api_async.search_player(player_id, server)
     except Exception as exception:
         return [f"错误: {exception}"]
     
     result: List[Union[str, bytes]] = []
     for _r in response:
@@ -238,15 +254,25 @@
         if _r["type"] == "string":
             result.append(_r["string"])
         else:
             result.append(b64decode(_r["string"]))
     
     return result
 
-async def search_card(word: str, servers: Sequence[_Server]) -> List[Union[str, bytes]]:
+async def search_card(user_id: str, word: str) -> List[Union[str, bytes]]:
+    try:
+        tsugu_user = await _get_tsugu_user(user_id, platform)
+    except Exception as exception:
+        return [f"错误: {exception}"]
+    
+    if isinstance(tsugu_user, str):
+        return [tsugu_user]
+    
+    servers = tsugu_user["default_server"]
+    
     try:
         response = await tsugu_api_async.search_card(servers, word)
     except Exception as exception:
         return [f"错误: {exception}"]
     
     result: List[Union[str, bytes]] = []
     for _r in response:
@@ -268,165 +294,280 @@
         if _r["type"] == "string":
             result.append(_r["string"])
         else:
             result.append(b64decode(_r["string"]))
     
     return result
 
-async def search_character(text: str, servers: Sequence[_Server]) -> List[Union[str, bytes]]:
+async def search_character(user_id: str, text: str) -> List[Union[str, bytes]]:
+    try:
+        tsugu_user = await _get_tsugu_user(user_id, platform)
+    except Exception as exception:
+        return [f"错误: {exception}"]
+    
+    if isinstance(tsugu_user, str):
+        return [tsugu_user]
+    
+    servers = tsugu_user["default_server"]
+    
     try:
         response = await tsugu_api_async.search_character(servers, text)
     except Exception as exception:
         return [f"错误: {exception}"]
     
     result: List[Union[str, bytes]] = []
     for _r in response:
         if _r["type"] == "string":
             result.append(_r["string"])
         else:
             result.append(b64decode(_r["string"]))
     
     return result
 
-async def search_event(text: str, servers: Sequence[_Server]) -> List[Union[str, bytes]]:
+async def search_event(user_id: str, text: str) -> List[Union[str, bytes]]:
+    try:
+        tsugu_user = await _get_tsugu_user(user_id, platform)
+    except Exception as exception:
+        return [f"错误: {exception}"]
+    
+    if isinstance(tsugu_user, str):
+        return [tsugu_user]
+    
+    servers = tsugu_user["default_server"]
+
     try:
         response = await tsugu_api_async.search_event(servers, text)
     except Exception as exception:
         return [f"错误: {exception}"]
     
     result: List[Union[str, bytes]] = []
     for _r in response:
         if _r["type"] == "string":
             result.append(_r["string"])
         else:
             result.append(b64decode(_r["string"]))
     
     return result
 
-async def search_song(text: str, servers: Sequence[_Server]) -> List[Union[str, bytes]]:
+async def search_song(user_id: str, text: str) -> List[Union[str, bytes]]:
+    try:
+        tsugu_user = await _get_tsugu_user(user_id, platform)
+    except Exception as exception:
+        return [f"错误: {exception}"]
+    
+    if isinstance(tsugu_user, str):
+        return [tsugu_user]
+    
+    servers = tsugu_user["default_server"]
+    
     try:
         response = await tsugu_api_async.search_song(servers, text)
     except Exception as exception:
         return [f"错误: {exception}"]
     
     result: List[Union[str, bytes]] = []
     for _r in response:
         if _r["type"] == "string":
             result.append(_r["string"])
         else:
             result.append(b64decode(_r["string"]))
     
     return result
 
-async def song_chart(servers: Sequence[_Server], song_id: int, difficulty_text: _DifficultyText) -> List[Union[str, bytes]]:
+async def song_chart(user_id: str, song_id: int, difficulty_text: _DifficultyText) -> List[Union[str, bytes]]:
+    try:
+        tsugu_user = await _get_tsugu_user(user_id, platform)
+    except Exception as exception:
+        return [f"错误: {exception}"]
+    
+    if isinstance(tsugu_user, str):
+        return [tsugu_user]
+    
+    servers = tsugu_user["default_server"]
+
     try:
         response = await tsugu_api_async.song_chart(servers, song_id, difficulty_text)
     except Exception as exception:
         return [f"错误: {exception}"]
     
     result: List[Union[str, bytes]] = []
     for _r in response:
         if _r["type"] == "string":
             result.append(_r["string"])
         else:
             result.append(b64decode(_r["string"]))
     
     return result
 
-async def song_meta(servers: Sequence[_Server], server: _Server) -> List[Union[str, bytes]]:
+async def song_meta(user_id: str, server: Optional[_Server]=None) -> List[Union[str, bytes]]:
+    try:
+        tsugu_user = await _get_tsugu_user(user_id, platform)
+    except Exception as exception:
+        return [f"错误: {exception}"]
+    
+    if isinstance(tsugu_user, str):
+        return [tsugu_user]
+    
+    servers = tsugu_user["default_server"]
+    if server is None:
+        server = tsugu_user["server_mode"]
+
     try:
         response = await tsugu_api_async.song_meta(servers, server)
     except Exception as exception:
         return [f"错误: {exception}"]
 
     result: List[Union[str, bytes]] = []
     for _r in response:
         if _r["type"] == "string":
             result.append(_r["string"])
         else:
             result.append(b64decode(_r["string"]))
     
     return result
 
-async def event_stage(server: _Server, event_id: Optional[int]=None, meta: bool=False) -> List[Union[str, bytes]]:
+async def event_stage(user_id: str, event_id: Optional[int]=None, meta: bool=False) -> List[Union[str, bytes]]:
+    try:
+        tsugu_user = await _get_tsugu_user(user_id, platform)
+    except Exception as exception:
+        return [f"错误: {exception}"]
+    
+    if isinstance(tsugu_user, str):
+        return [tsugu_user]
+    
+    server = tsugu_user["server_mode"]
+
     try:
         response = await tsugu_api_async.event_stage(server, event_id, meta)
     except Exception as exception:
         return [f"错误: {exception}"]
 
     result: List[Union[str, bytes]] = []
     for _r in response:
         if _r["type"] == "string":
             result.append(_r["string"])
         else:
             result.append(b64decode(_r["string"]))
     
     return result
 
-async def search_gacha(servers: Sequence[_Server], gacha_id: int) -> List[Union[str, bytes]]:
+async def search_gacha(user_id: str, gacha_id: int) -> List[Union[str, bytes]]:
+    try:
+        tsugu_user = await _get_tsugu_user(user_id, platform)
+    except Exception as exception:
+        return [f"错误: {exception}"]
+    
+    if isinstance(tsugu_user, str):
+        return [tsugu_user]
+    
+    servers = tsugu_user["default_server"]
+
     try:
         response = await tsugu_api_async.search_gacha(servers, gacha_id)
     except Exception as exception:
         return [f"错误: {exception}"]
 
     result: List[Union[str, bytes]] = []
     for _r in response:
         if _r["type"] == "string":
             result.append(_r["string"])
         else:
             result.append(b64decode(_r["string"]))
     
     return result
 
-async def search_ycx(server: _Server, tier: int, event_id: Optional[int]=None) -> List[Union[str, bytes]]:
+async def search_ycx(user_id: str, tier: int, event_id: Optional[int]=None, server: Optional[_Server]=None) -> List[Union[str, bytes]]:
+    if server is None:
+        try:
+            tsugu_user = await _get_tsugu_user(user_id, platform)
+        except Exception as exception:
+            return [f"错误: {exception}"]
+        
+        if isinstance(tsugu_user, str):
+            return [tsugu_user]
+        
+        server = tsugu_user["server_mode"]
+    
     try:
         response = await tsugu_api_async.ycx(server, tier, event_id)
     except Exception as exception:
         return [f"错误: {exception}"]
 
     result: List[Union[str, bytes]] = []
     for _r in response:
         if _r["type"] == "string":
             result.append(_r["string"])
         else:
             result.append(b64decode(_r["string"]))
     
     return result
 
-async def search_ycx_all(server: _Server, event_id: Optional[int]=None) -> List[Union[str, bytes]]:
+async def search_ycx_all(user_id: str, server: Optional[_Server]=None, event_id: Optional[int]=None) -> List[Union[str, bytes]]:
+    if server is None:
+        try:
+            tsugu_user = await _get_tsugu_user(user_id, platform)
+        except Exception as exception:
+            return [f"错误: {exception}"]
+        
+        if isinstance(tsugu_user, str):
+            return [tsugu_user]
+        
+        server = tsugu_user["server_mode"]
+    
     try:
         response = await tsugu_api_async.ycx_all(server, event_id)
     except Exception as exception:
         return [f"错误: {exception}"]
 
     result: List[Union[str, bytes]] = []
     for _r in response:
         if _r["type"] == "string":
             result.append(_r["string"])
         else:
             result.append(b64decode(_r["string"]))
     
     return result
 
-async def search_lsycx(server: _Server, tier: int, event_id: Optional[int]=None) -> List[Union[str, bytes]]:
+async def search_lsycx(user_id: str, tier: int, event_id: Optional[int]=None, server: Optional[_Server]=None) -> List[Union[str, bytes]]:
+    if server is None:
+        try:
+            tsugu_user = await _get_tsugu_user(user_id, platform)
+        except Exception as exception:
+            return [f"错误: {exception}"]
+        
+        if isinstance(tsugu_user, str):
+            return [tsugu_user]
+        
+        server = tsugu_user["server_mode"]
+    
     try:
         response = await tsugu_api_async.lsycx(server, tier, event_id)
     except Exception as exception:
         return [f"错误: {exception}"]
 
     result: List[Union[str, bytes]] = []
     for _r in response:
         if _r["type"] == "string":
             result.append(_r["string"])
         else:
             result.append(b64decode(_r["string"]))
     
     return result
 
-async def simulate_gacha(server: _Server, times: Optional[int]=None, gacha_id: Optional[int]=None) -> List[Union[str, bytes]]:
+async def simulate_gacha(user_id: str, times: Optional[int]=None, gacha_id: Optional[int]=None) -> List[Union[str, bytes]]:
+    try:
+        tsugu_user = await _get_tsugu_user(user_id, platform)
+    except Exception as exception:
+        return [f"错误: {exception}"]
+    
+    if isinstance(tsugu_user, str):
+        return [tsugu_user]
+    
+    server = tsugu_user["server_mode"]
+
     try:
         response = await tsugu_api_async.gacha_simulate(server, times, gacha_id)
     except Exception as exception:
         return [f"错误: {exception}"]
 
     result: List[Union[str, bytes]] = []
     for _r in response:
```

### Comparing `nonebot_plugin_tsugu_bangdream_bot-0.1.5/nonebot_plugin_tsugu_bangdream_bot/_utils.py` & `nonebot_plugin_tsugu_bangdream_bot-0.1.6/nonebot_plugin_tsugu_bangdream_bot/_utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tsugu_bangdream_bot-0.1.5/nonebot_plugin_tsugu_bangdream_bot/config.py` & `nonebot_plugin_tsugu_bangdream_bot-0.1.6/nonebot_plugin_tsugu_bangdream_bot/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tsugu_bangdream_bot-0.1.5/pyproject.toml` & `nonebot_plugin_tsugu_bangdream_bot-0.1.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-tsugu-bangdream-bot"
-version = "0.1.5"
+version = "0.1.6"
 description = "Koishi-Plugin-Tsugu-BanGDream-Bot 的 NoneBot2 实现"
 authors = [
     { name = "WindowsSov8forUs", email = "qwertyuiop2333@hotmail.com" },
 ]
 dependencies = [
     "nonebot2>=2.2.1",
     "nonebot-plugin-alconna>=0.42.4",
```

### Comparing `nonebot_plugin_tsugu_bangdream_bot-0.1.5/PKG-INFO` & `nonebot_plugin_tsugu_bangdream_bot-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-tsugu-bangdream-bot
-Version: 0.1.5
+Version: 0.1.6
 Summary: Koishi-Plugin-Tsugu-BanGDream-Bot 的 NoneBot2 实现
 Author-Email: WindowsSov8forUs <qwertyuiop2333@hotmail.com>
 License: MIT
 Requires-Python: >=3.8
 Requires-Dist: nonebot2>=2.2.1
 Requires-Dist: nonebot-plugin-alconna>=0.42.4
 Requires-Dist: tsugu-api-python>=1.2.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-tsugu-bangdream-bot Version: 0.1.5
+Metadata-Version: 2.1 Name: nonebot-plugin-tsugu-bangdream-bot Version: 0.1.6
 Summary: Koishi-Plugin-Tsugu-BanGDream-Bot ç NoneBot2 å®ç° Author-Email:
 WindowsSov8forUs
 hotmail.com> License: MIT Requires-Python: >=3.8 Requires-Dist: nonebot2>=2.2.1
 Requires-Dist: nonebot-plugin-alconna>=0.42.4 Requires-Dist: tsugu-api-
 python>=1.2.0 Requires-Dist: nonebot-plugin-userinfo>=0.2.4 Description-
 Content-Type: text/markdown
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
```

