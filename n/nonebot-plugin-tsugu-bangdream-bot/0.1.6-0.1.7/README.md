# Comparing `tmp/nonebot_plugin_tsugu_bangdream_bot-0.1.6.tar.gz` & `tmp/nonebot_plugin_tsugu_bangdream_bot-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_tsugu_bangdream_bot-0.1.6.tar", last modified: Tue May 21 06:53:58 2024, max compression
+gzip compressed data, was "nonebot_plugin_tsugu_bangdream_bot-0.1.7.tar", last modified: Tue May 21 13:56:26 2024, max compression
```

## Comparing `nonebot_plugin_tsugu_bangdream_bot-0.1.6.tar` & `nonebot_plugin_tsugu_bangdream_bot-0.1.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1067 2024-05-21 06:53:34.798290 nonebot_plugin_tsugu_bangdream_bot-0.1.6/LICENSE
--rw-r--r--   0        0        0     6897 2024-05-21 06:53:34.798290 nonebot_plugin_tsugu_bangdream_bot-0.1.6/README.md
--rw-r--r--   0        0        0    31702 2024-05-21 06:53:34.798290 nonebot_plugin_tsugu_bangdream_bot-0.1.6/nonebot_plugin_tsugu_bangdream_bot/__init__.py
--rw-r--r--   0        0        0    18309 2024-05-21 06:53:34.798290 nonebot_plugin_tsugu_bangdream_bot-0.1.6/nonebot_plugin_tsugu_bangdream_bot/_commands.py
--rw-r--r--   0        0        0     7846 2024-05-21 06:53:34.798290 nonebot_plugin_tsugu_bangdream_bot-0.1.6/nonebot_plugin_tsugu_bangdream_bot/_utils.py
--rw-r--r--   0        0        0     2456 2024-05-21 06:53:34.798290 nonebot_plugin_tsugu_bangdream_bot-0.1.6/nonebot_plugin_tsugu_bangdream_bot/config.py
--rw-r--r--   0        0        0      569 2024-05-21 06:53:58.018528 nonebot_plugin_tsugu_bangdream_bot-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     7337 1970-01-01 00:00:00.000000 nonebot_plugin_tsugu_bangdream_bot-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-21 13:56:03.189422 nonebot_plugin_tsugu_bangdream_bot-0.1.7/LICENSE
+-rw-r--r--   0        0        0     6897 2024-05-21 13:56:03.189422 nonebot_plugin_tsugu_bangdream_bot-0.1.7/README.md
+-rw-r--r--   0        0        0    29262 2024-05-21 13:56:03.189422 nonebot_plugin_tsugu_bangdream_bot-0.1.7/nonebot_plugin_tsugu_bangdream_bot/__init__.py
+-rw-r--r--   0        0        0    18299 2024-05-21 13:56:03.189422 nonebot_plugin_tsugu_bangdream_bot-0.1.7/nonebot_plugin_tsugu_bangdream_bot/_commands.py
+-rw-r--r--   0        0        0     7329 2024-05-21 13:56:03.189422 nonebot_plugin_tsugu_bangdream_bot-0.1.7/nonebot_plugin_tsugu_bangdream_bot/_utils.py
+-rw-r--r--   0        0        0     2456 2024-05-21 13:56:03.189422 nonebot_plugin_tsugu_bangdream_bot-0.1.7/nonebot_plugin_tsugu_bangdream_bot/config.py
+-rw-r--r--   0        0        0      569 2024-05-21 13:56:26.029316 nonebot_plugin_tsugu_bangdream_bot-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     7337 1970-01-01 00:00:00.000000 nonebot_plugin_tsugu_bangdream_bot-0.1.7/PKG-INFO
```

### Comparing `nonebot_plugin_tsugu_bangdream_bot-0.1.6/LICENSE` & `nonebot_plugin_tsugu_bangdream_bot-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tsugu_bangdream_bot-0.1.6/README.md` & `nonebot_plugin_tsugu_bangdream_bot-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tsugu_bangdream_bot-0.1.6/nonebot_plugin_tsugu_bangdream_bot/__init__.py` & `nonebot_plugin_tsugu_bangdream_bot-0.1.7/nonebot_plugin_tsugu_bangdream_bot/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,29 @@
-from typing import Any, List, Tuple, Union, Optional
+from typing import Any, List, Tuple, Union
 
 from nonebot.log import logger
 from nonebot.adapters import Bot, Event, Message
 from nonebot.params import RegexGroup, ArgPlainText
 from nonebot import on_regex, get_driver, get_plugin_config
 from nonebot.plugin import PluginMetadata, require, inherit_supported_adapters
 
 require("nonebot_plugin_alconna")
 
-from nonebot.typing import T_State
-from nonebot_plugin_alconna import Alconna, load_builtin_plugin
-from nonebot_plugin_alconna import Command, Arparma, Extension, store_true
+from nonebot_plugin_alconna import Match, Query, Alconna, load_builtin_plugin
+from nonebot_plugin_alconna import Command, Extension, store_true, CommandMeta
 from nonebot_plugin_alconna.uniseg import At, Text, Image, Reply, Segment, UniMessage
 
 load_builtin_plugin("help")
 
 require("nonebot_plugin_userinfo")
 
 from nonebot_plugin_userinfo import get_user_info
 
 from .config import Config
-from ._utils import USAGES, COMMAND_KEYWORDS, server_name_to_id, tier_list_of_server_to_string
+from ._utils import USAGES, server_name_to_id, tier_list_of_server_to_string
 from ._commands import (
     platform,
     room_list,
     song_meta,
     song_chart,
     search_ycx,
     event_stage,
@@ -52,15 +51,15 @@
 from tsugu_api_core._typing import _ServerId
 
 config = get_plugin_config(Config)
 
 __plugin_meta__ = PluginMetadata(
     name="nonebot-plugin-tsugu-bangdream-bot",
     description="Koishi-Plugin-Tsugu-BanGDream-Bot 的 NoneBot2 实现",
-    usage="\n".join([f"{key}: {value}" for key, value in USAGES.items()]),
+    usage="\n\n".join([f"{key}: {value}" for key, value in USAGES.items()]),
     type="application",
     homepage="https://github.com/WindowsSov8forUs/nonebot-plugin-tsugu-bangdream-bot",
     config=Config,
     supported_adapters=inherit_supported_adapters(
         "nonebot_plugin_alconna", "nonebot_plugin_userinfo"
     )
 )
@@ -70,37 +69,17 @@
     def priority(self) -> int:
         return 10
     
     @property
     def id(self) -> str:
         return "TsuguExtension"
     
-    def __init__(self, reply: bool, at: bool, no_space: bool) -> None:
+    def __init__(self, reply: bool, at: bool) -> None:
         self.reply = reply
         self.at = at
-        self.no_space = no_space
-    
-    async def message_provider(self, event: Event, state: T_State, bot: Bot, use_origin: bool = False) -> Optional[Union[Message, UniMessage]]:
-        msg = await super().message_provider(event, state, bot, use_origin)
-        
-        if msg is None:
-            return None
-        
-        if self.no_space:
-            msg = msg.extract_plain_text().strip()
-            for keyword in COMMAND_KEYWORDS:
-                if msg.startswith(keyword):
-                    if not msg.startswith(keyword + " "):
-                        msg = msg.replace(keyword, keyword + " ", 1)
-                    
-                    break
-            
-            return UniMessage(msg)
-        else:
-            return msg
     
     async def permission_check(self, bot: Bot, event: Event, command: Alconna) -> bool:
         # 规避机器人自身的消息
         try:
             user_id = event.get_user_id()
         except:
             return True
@@ -141,15 +120,16 @@
     tsugu_api_async.settings.userdata_backend_url = config.tsugu_data_backend_url
 
 tsugu_api_async.settings.proxy = config.tsugu_proxy
 tsugu_api_async.settings.backend_proxy = config.tsugu_backend_proxy
 tsugu_api_async.settings.userdata_backend_proxy = config.tsugu_data_backend_proxy
 tsugu_api_async.settings.timeout = config.tsugu_timeout
 
-extension = TsuguExtension(config.tsugu_reply, config.tsugu_at, config.tsugu_no_space)
+extension = TsuguExtension(config.tsugu_reply, config.tsugu_at)
+meta = CommandMeta(compact=config.tsugu_no_space)
 
 car_forwarding = on_regex(r"(^(\d{5,6})(.*)$)")
 
 @car_forwarding.handle()
 async def _(bot: Bot, event: Event, group: Tuple[Any, ...] = RegexGroup()) -> None:
     user_info = await get_user_info(bot, event, event.get_user_id())
     
@@ -176,45 +156,41 @@
     except Exception as exception:
         logger.warning(f"Failed to submit room number: {exception}")
         car_forwarding.skip()
     
     if is_forwarded:
         logger.debug(f"Submitted room number: {group[0]}")
 
-open_forward = Command("开启车牌转发", "开启车牌转发").build(auto_send_output=True, aliases=config.tsugu_open_forward_aliases, extensions=[extension])
+open_forward = Command("开启车牌转发", "开启车牌转发", meta=meta).build(auto_send_output=True, aliases=config.tsugu_open_forward_aliases, extensions=[extension], use_cmd_start=True)
 
 @open_forward.handle()
 async def _(event: Event) -> None:
     user_id = event.get_user_id()
     await open_forward.send(await switch_forward(user_id, True))
 
-close_forward = Command("关闭车牌转发", "关闭车牌转发").build(auto_send_output=True, aliases=config.tsugu_close_forward_aliases, extensions=[extension])
+close_forward = Command("关闭车牌转发", "关闭车牌转发", meta=meta).build(auto_send_output=True, aliases=config.tsugu_close_forward_aliases, extensions=[extension], use_cmd_start=True)
 
 @close_forward.handle()
 async def _(event: Event) -> None:
     user_id = event.get_user_id()
     await close_forward.send(await switch_forward(user_id, False))
 
 bind_player = (
-    Command("绑定玩家 [server_name:str]", "绑定玩家信息")
+    Command("绑定玩家 [server_name:str]", "绑定玩家信息", meta=meta)
     .usage('开始玩家数据绑定流程，请不要在"绑定玩家"指令后添加玩家ID。省略服务器名时，默认为绑定到你当前的主服务器。请在获得临时验证数字后，将玩家签名改为该数字，并回复你的玩家ID')
-    .build(auto_send_output=True, aliases=config.tsugu_bind_player_aliases, extensions=[extension])
+    .build(auto_send_output=True, aliases=config.tsugu_bind_player_aliases, extensions=[extension], use_cmd_start=True)
 )
 
 @bind_player.handle()
-async def _(arp: Arparma, event: Event) -> None:
-    if arp.find("server_name"):
-        server = arp.query[str]("server_name")
-        if server is None:
-            _server = None
-        else:
-            try:
-                _server = server_name_to_id(server)
-            except ValueError:
-                await bind_player.finish("错误: 服务器不存在，请不要在参数中添加玩家ID")
+async def _(server_name: Match[str], event: Event) -> None:
+    if server_name.available:
+        try:
+            _server = server_name_to_id(server_name.result)
+        except ValueError:
+            await bind_player.finish("错误: 服务器不存在，请不要在参数中添加玩家ID")
     else:
         _server = None
     
     reply, available, server = await player_bind(event.get_user_id(), _server)
     
     if not available:
         await bind_player.finish(reply)
@@ -231,30 +207,26 @@
     assert server is not None
     
     response = await tsugu_api_async.bind_player_verification("red", event.get_user_id(), server, int(player_id), True)
     
     await bind_player.finish(response["data"])
 
 unbind_player = (
-    Command("解除绑定 [server_name:str]", "解除当前服务器的玩家绑定").alias("解绑玩家")
+    Command("解除绑定 [server_name:str]", "解除当前服务器的玩家绑定", meta=meta).alias("解绑玩家")
     .usage("解除指定服务器的玩家数据绑定。省略服务器名时，默认为当前的主服务器")
-    .build(auto_send_output=True, aliases=config.tsugu_unbind_player_aliases, extensions=[extension])
+    .build(auto_send_output=True, aliases=config.tsugu_unbind_player_aliases, extensions=[extension], use_cmd_start=True)
 )
 
 @unbind_player.handle()
-async def _(arp: Arparma, event: Event) -> None:
-    if arp.find("server_name"):
-        server = arp.query[str]("server_name")
-        if server is None:
-            _server = None
-        else:
-            try:
-                _server = server_name_to_id(server)
-            except ValueError:
-                await unbind_player.finish("错误: 服务器不存在，请不要在参数中添加玩家ID")
+async def _(server_name: Match[str], event: Event) -> None:
+    if server_name.available:
+        try:
+            _server = server_name_to_id(server_name.result)
+        except ValueError:
+            await unbind_player.finish("错误: 服务器不存在，请不要在参数中添加玩家ID")
     else:
         _server = None
     
     reply, available, server, player_id = await player_unbind(event.get_user_id(), _server)
     
     if not available:
         await unbind_player.finish(reply)
@@ -272,51 +244,45 @@
     assert player_id is not None
     
     response = await tsugu_api_async.bind_player_verification("red", event.get_user_id(), server, int(player_id), False)
     
     await unbind_player.finish(response["data"])
 
 main_server = (
-    Command("主服务器 <server_name:str>", "设置主服务器")
+    Command("主服务器 <server_name:str>", "设置主服务器", meta=meta)
     .alias("服务器模式").alias("切换服务器")
     .usage("将指定的服务器设置为你的主服务器")
     .example("主服务器 cn : 将国服设置为主服务器")
     .example("日服模式 : 将日服设置为主服务器")
     .shortcut(r"^(.+服)模式$", {"args": ["{0}"]})
-    .build(auto_send_output=True, aliases=config.tsugu_main_server_aliases, extensions=[extension])
+    .build(auto_send_output=True, aliases=config.tsugu_main_server_aliases, extensions=[extension], use_cmd_start=True)
 )
 
 @main_server.handle()
-async def _(arp: Arparma, event: Event) -> None:
-    if arp.find("server_name"):
-        server = arp.query[str]("server_name")
-        if server is None:
-            await main_server.finish("错误: 未指定服务器")
+async def _(server_name: Match[str], event: Event) -> None:
+    if server_name.available:
         try:
-            _server = server_name_to_id(server)
+            _server = server_name_to_id(server_name.result)
         except ValueError:
             await main_server.finish("错误: 服务器不存在")
         await main_server.finish(await switch_main_server(event.get_user_id(), _server))
     else:
         await main_server.finish("错误: 未指定服务器")
 
 default_servers = (
-    Command("设置默认服务器 <server_list:str+:>", "设定信息显示中的默认服务器排序")
+    Command("设置默认服务器 <server_list:str*>", "设定信息显示中的默认服务器排序", meta=meta)
     .alias("默认服务器")
     .usage("使用空格分隔服务器列表")
     .example("设置默认服务器 国服 日服 : 将国服设置为第一服务器，日服设置为第二服务器")
-    .build(auto_send_output=True, aliases=config.tsugu_default_servers_aliases, extensions=[extension])
+    .build(auto_send_output=True, aliases=config.tsugu_default_servers_aliases, extensions=[extension], use_cmd_start=True)
 )
 
 @default_servers.handle()
-async def _(arp: Arparma, event: Event) -> None:
-    if arp.find("server_list"):
-        server_list = arp.query[List[str]]("server_list")
-        if server_list is None:
-            await default_servers.finish("错误: 请指定至少一个服务器")
+async def _(server_list: List[str], event: Event) -> None:
+    if len(server_list) > 0:
         servers: List[_ServerId] = []
         for _server in server_list:
             try:
                 _id = server_name_to_id(_server)
             except ValueError:
                 await default_servers.finish("错误: 指定了不存在的服务器")
             if _id in servers:
@@ -326,310 +292,252 @@
             await default_servers.finish("错误: 请指定至少一个服务器")
         
         await default_servers.finish(await set_default_servers(event.get_user_id(), servers))
     else:
         await default_servers.finish("错误: 请指定至少一个服务器")
 
 player_status = (
-    Command("玩家状态 [server_name:str]", "查询自己的玩家状态")
+    Command("玩家状态 [server_name:str]", "查询自己的玩家状态", meta=meta)
     .shortcut(r"^(.+服)玩家状态$", {"args": ["{0}"]})
-    .build(auto_send_output=True, aliases=config.tsugu_player_status_aliases, extensions=[extension])
+    .build(auto_send_output=True, aliases=config.tsugu_player_status_aliases, extensions=[extension], use_cmd_start=True)
 )
 
 @player_status.handle()
-async def _(arp: Arparma, event: Event) -> None:
-    if arp.find("server_name"):
-        server = arp.query[str]("server_name")
-        if server is None:
-            _server = None
-        else:
-            try:
-                _server = server_name_to_id(server)
-            except ValueError:
-                await player_status.finish("错误: 服务器不存在")
+async def _(server_name: Match[str], event: Event) -> None:
+    if server_name.available:
+        try:
+            _server = server_name_to_id(server_name.result)
+        except ValueError:
+            await player_status.finish("错误: 服务器不存在")
     else:
         _server = None
     
     result = await player_info(event.get_user_id(), _server)
     segments: List[Segment] = []
     for _r in result:
         if isinstance(_r, str):
             segments.append(Text(_r))
         else:
             segments.append(Image(raw=_r))
     
     await player_status.finish(UniMessage(segments))
 
 ycm = (
-    Command("ycm <keyword:str*>", "获取车牌")
+    Command("ycm <keyword:str*>", "获取车牌", meta=meta)
     .alias("有车吗").alias("车来")
     .usage("获取所有车牌车牌，可以通过关键词过滤")
     .example("ycm : 获取所有车牌").example('ycm 大分: 获取所有车牌，其中包含"大分"关键词的车牌')
-    .build(auto_send_output=True, aliases=config.tsugu_ycm_aliases, extensions=[extension])
+    .build(auto_send_output=True, aliases=config.tsugu_ycm_aliases, extensions=[extension], use_cmd_start=True)
 )
 
 @ycm.handle()
-async def _(arp: Arparma) -> None:
-    if arp.find("keyword"):
-        keywords = arp.query[List[str]]("keyword", [])
-        keyword = " ".join(keywords)
+async def _(keyword: List[str]) -> None:
+    if len(keyword) > 0:
+        _keyword = " ".join(keyword)
     else:
-        keyword = None
+        _keyword = None
     
     try:
-        response = await room_list(keyword)
+        response = await room_list(_keyword)
     except Exception as exception:
         await ycm.finish(f"错误: {exception}")
     
     segments: List[Segment] = []
     for _r in response:
         if isinstance(_r, str):
             segments.append(Text(_r))
         else:
             segments.append(Image(raw=_r))
     
     await ycm.finish(UniMessage(segments))
 
 player_search = (
-    Command("查玩家 <player_id:int> [server_name:str]", "查询玩家信息")
+    Command("查玩家 <player_id:int> [server_name:str]", "查询玩家信息", meta=meta)
     .alias("查询玩家")
     .usage("查询指定ID玩家的信息。省略服务器名时，默认从你当前的主服务器查询")
     .example("查玩家 10000000 : 查询你当前默认服务器中，玩家ID为10000000的玩家信息")
     .example("查玩家 40474621 jp : 查询日服玩家ID为40474621的玩家信息")
-    .build(auto_send_output=True, aliases=config.tsugu_search_player_aliases, extensions=[extension])
+    .build(auto_send_output=True, aliases=config.tsugu_search_player_aliases, extensions=[extension], use_cmd_start=True)
 )
 
 @player_search.handle()
-async def _(arp: Arparma, event: Event) -> None:
-    if arp.find("player_id"):
-        player_id = arp.query[int]("player_id")
-    else:
+async def _(player_id: Match[int], server_name: Match[str], event: Event) -> None:
+    if not player_id.available:
         await player_search.finish("错误: 未指定玩家ID")
     
-    assert player_id is not None
-    
-    if arp.find("server_name"):
-        server = arp.query[str]("server_name")
-        if server is None:
-            _server = None
-        else:
-            try:
-                _server = server_name_to_id(server)
-            except ValueError:
-                await player_search.finish("错误: 服务器不存在")
+    if server_name.available:
+        try:
+            _server = server_name_to_id(server_name.result)
+        except ValueError:
+            await player_search.finish("错误: 服务器不存在")
     else:
         _server = None
     
-    result = await search_player(event.get_user_id(), player_id, _server)
+    result = await search_player(event.get_user_id(), player_id.result, _server)
     segments: List[Segment] = []
     for _r in result:
         if isinstance(_r, str):
             segments.append(Text(_r))
         else:
             segments.append(Image(raw=_r))
     
     await player_search.finish(UniMessage(segments))
 
 card_search = (
-    Command("查卡 <word:str*>", "查卡").alias("查卡牌")
+    Command("查卡 <word:str*>", "查卡", meta=meta).alias("查卡牌")
     .usage("根据关键词或卡牌ID查询卡片信息，请使用空格隔开所有参数")
     .example("查卡 1399 :返回1399号卡牌的信息")
     .example("查卡 绿 tsugu :返回所有属性为pure的羽泽鸫的卡牌列表")
-    .build(auto_send_output=True, aliases=config.tsugu_search_card_aliases, extensions=[extension])
+    .build(auto_send_output=True, aliases=config.tsugu_search_card_aliases, extensions=[extension], use_cmd_start=True)
 )
 
 @card_search.handle()
-async def _(arp: Arparma, event: Event) -> None:
-    if arp.find("word"):
-        words = arp.query[str]("word", [])
-        word = " ".join(words)
-    else:
-        word = ""
-    
+async def _(word: List[str], event: Event) -> None:
     try:
-        response = await search_card(event.get_user_id(), word)
+        response = await search_card(event.get_user_id(), " ".join(word))
     except Exception as exception:
         await card_search.finish(f"错误: {exception}")
     
     segments: List[Segment] = []
     for _r in response:
         if isinstance(_r, str):
             segments.append(Text(_r))
         else:
             segments.append(Image(raw=_r))
     
     await card_search.finish(UniMessage(segments))
 
 card_illustration = (
-    Command("查卡面 <card_id:int>", "查卡面").alias("查卡插画").alias("查插画")
+    Command("查卡面 <card_id:int>", "查卡面", meta=meta).alias("查卡插画").alias("查插画")
     .usage("根据卡片ID查询卡片插画").example("查卡面 1399 :返回1399号卡牌的插画")
-    .build(auto_send_output=True, aliases=config.tsugu_card_illustration_aliases, extensions=[extension])
+    .build(auto_send_output=True, aliases=config.tsugu_card_illustration_aliases, extensions=[extension], use_cmd_start=True)
 )
 
 @card_illustration.handle()
-async def _(arp: Arparma) -> None:
-    if arp.find("card_id"):
-        card_id = arp.query[int]("card_id")
-    else:
-        card_id = None
-    
-    if card_id is None:
+async def _(card_id: Match[int]) -> None:
+    if not card_id.available:
         await card_illustration.finish("错误: 参数错误")
     
     try:
-        response = await get_card_illustration(card_id)
+        response = await get_card_illustration(card_id.result)
     except Exception as exception:
         await card_illustration.finish(f"错误: {exception}")
     
     segments: List[Segment] = []
     for _r in response:
         if isinstance(_r, str):
             segments.append(Text(_r))
         else:
             segments.append(Image(raw=_r))
     
     await card_illustration.finish(UniMessage(segments))
 
 character_search = (
-    Command("查角色 <word:str+>", "查角色").usage("根据关键词或角色ID查询角色信息")
+    Command("查角色 <word:str*>", "查角色", meta=meta).usage("根据关键词或角色ID查询角色信息")
     .example("查角色 10 :返回10号角色的信息").example("查角色 吉他 :返回所有角色模糊搜索标签中包含吉他的角色列表")
-    .build(auto_send_output=True, aliases=config.tsugu_search_character_aliases, extensions=[extension])
+    .build(auto_send_output=True, aliases=config.tsugu_search_character_aliases, extensions=[extension], use_cmd_start=True)
 )
 
 @character_search.handle()
-async def _(arp: Arparma, event: Event) -> None:
-    if arp.find("word"):
-        words = arp.query[List[str]]("word", [])
-        word = " ".join(words)
-    else:
-        word = ""
-    
+async def _(word: List[str], event: Event) -> None:
     try:
-        response = await search_character(event.get_user_id(), word)
+        response = await search_character(event.get_user_id(), " ".join(word))
     except Exception as exception:
         await character_search.finish(f"错误: {exception}")
     
     segments: List[Segment] = []
     for _r in response:
         if isinstance(_r, str):
             segments.append(Text(_r))
         else:
             segments.append(Image(raw=_r))
     
     await character_search.finish(UniMessage(segments))
 
 event_search = (
-    Command("查活动 <word:str+>", "查活动").usage("根据关键词或活动ID查询活动信息")
+    Command("查活动 <word:str*>", "查活动", meta=meta).usage("根据关键词或活动ID查询活动信息")
     .example("查活动 177 :返回177号活动的信息").example("查活动 绿 tsugu :返回所有属性加成为pure，且活动加成角色中包括羽泽鸫的活动列表")
-    .build(auto_send_output=True, aliases=config.tsugu_search_event_aliases, extensions=[extension])
+    .build(auto_send_output=True, aliases=config.tsugu_search_event_aliases, extensions=[extension], use_cmd_start=True)
 )
 
 @event_search.handle()
-async def _(arp: Arparma, event: Event) -> None:
-    if arp.find("word"):
-        words = arp.query[List[str]]("word", [])
-        word = " ".join(words)
-    else:
-        word = ""
-    
+async def _(word: List[str], event: Event) -> None:
     try:
-        response = await search_event(event.get_user_id(), word)
+        response = await search_event(event.get_user_id(), " ".join(word))
     except Exception as exception:
         await event_search.finish(f"错误: {exception}")
     
     segments: List[Segment] = []
     for _r in response:
         if isinstance(_r, str):
             segments.append(Text(_r))
         else:
             segments.append(Image(raw=_r))
     
     await event_search.finish(UniMessage(segments))
 
 song_search = (
-    Command("查曲 <word:str+>", "查曲").usage("根据关键词或曲目ID查询曲目信息")
+    Command("查曲 <word:str*>", "查曲", meta=meta).usage("根据关键词或曲目ID查询曲目信息")
     .example("查曲 1 :返回1号曲的信息").example("查曲 ag lv27 :返回所有难度为27的ag曲列表")
-    .build(auto_send_output=True, aliases=config.tsugu_search_song_aliases, extensions=[extension])
+    .build(auto_send_output=True, aliases=config.tsugu_search_song_aliases, extensions=[extension], use_cmd_start=True)
 )
 
 @song_search.handle()
-async def _(arp: Arparma, event: Event) -> None:
-    if arp.find("word"):
-        words = arp.query[List[str]]("word", [])
-        word = " ".join(words)
-    else:
-        word = ""
-    
+async def _(word: List[str], event: Event) -> None:
     try:
-        response = await search_song(event.get_user_id(), word)
+        response = await search_song(event.get_user_id(), " ".join(word))
     except Exception as exception:
         await song_search.finish(f"错误: {exception}")
     
     segments: List[Segment] = []
     for _r in response:
         if isinstance(_r, str):
             segments.append(Text(_r))
         else:
             segments.append(Image(raw=_r))
     
     await song_search.finish(UniMessage(segments))
 
 chart_search = (
-    Command("查谱面 <song_id:int> [difficulty:str]", "查谱面").usage("根据曲目ID与难度查询谱面信息")
+    Command("查谱面 <song_id:int> [difficulty:str]", "查谱面", meta=meta).usage("根据曲目ID与难度查询谱面信息")
     .example("查谱面 1 :返回1号曲的所有谱面").example("查谱面 1 expert :返回1号曲的expert难度谱面")
-    .build(auto_send_output=True, aliases=config.tsugu_song_chart_aliases, extensions=[extension])
+    .build(auto_send_output=True, aliases=config.tsugu_song_chart_aliases, extensions=[extension], use_cmd_start=True)
 )
 
 @chart_search.handle()
-async def _(arp: Arparma, event: Event) -> None:
-    if arp.find("song_id"):
-        song_id = arp.query[int]("song_id")
-    else:
-        song_id = None
-    
-    if arp.find("difficulty"):
-        difficulty = arp.query[str]("difficulty", "expert")
-    else:
-        difficulty = "expert"
-    
-    if song_id is None:
+async def _(song_id: Match[int], event: Event, difficulty: str = "expert") -> None:
+    if not song_id.available:
         await chart_search.finish("错误: 未指定曲目ID")
     
     try:
-        response = await song_chart(event.get_user_id(), song_id, difficulty) # type: ignore
+        response = await song_chart(event.get_user_id(), song_id.result, difficulty) # type: ignore
     except Exception as exception:
         await chart_search.finish(f"错误: {exception}")
     
     segments: List[Segment] = []
     for _r in response:
         if isinstance(_r, str):
             segments.append(Text(_r))
         else:
             segments.append(Image(raw=_r))
     
     await chart_search.finish(UniMessage(segments))
 
 meta_search = (
-    Command("查询分数表 <word:str*>", "查询分数表").usage("查询指定服务器的歌曲分数表，如果没有服务器名的话，服务器为用户的默认服务器")
+    Command("查询分数表 <word:str>", "查询分数表", meta=meta).usage("查询指定服务器的歌曲分数表，如果没有服务器名的话，服务器为用户的默认服务器")
     .alias("查分数表").alias("查询分数榜").alias("查分数榜")
     .example("查询分数表 cn :返回国服的歌曲分数表")
-    .build(auto_send_output=True, aliases=config.tsugu_song_meta_aliases, extensions=[extension])
+    .build(auto_send_output=True, aliases=config.tsugu_song_meta_aliases, extensions=[extension], use_cmd_start=True)
 )
 
 @meta_search.handle()
-async def _(arp: Arparma, event: Event) -> None:
-    if arp.find("word"):
-        words = arp.query[List[str]]("word", [])
-        word = " ".join(words)
-    else:
-        word = ""
-    
-    if len(word) < 1:
+async def _(word: Match[str], event: Event) -> None:
+    if word.available:
         try:
-            _server = server_name_to_id(word)
+            _server = server_name_to_id(word.result)
         except ValueError:
             await meta_search.finish("错误: 服务器不存在")
     else:
         _server = None
     
     try:
         response = await song_meta(event.get_user_id(), _server)
@@ -642,236 +550,204 @@
             segments.append(Text(_r))
         else:
             segments.append(Image(raw=_r))
     
     await meta_search.finish(UniMessage(segments))
 
 stage_search = (
-    Command("查试炼 [event_id:int]", "查试炼").usage("查询当前服务器当前活动试炼信息\n可以自定义活动ID\n参数:-m 显示歌曲meta(相对效率)")
+    Command("查试炼 [event_id:int]", "查试炼", meta=meta).usage("查询当前服务器当前活动试炼信息\n可以自定义活动ID\n参数:-m 显示歌曲meta(相对效率)")
     .alias("查stage").alias("查舞台").alias("查festival").alias("查5v5")
     .example("查试炼 157 -m :返回157号活动的试炼信息，包含歌曲meta")
     .example("查试炼 -m :返回当前活动的试炼信息，包含歌曲meta")
     .example("查试炼 :返回当前活动的试炼信息")
     .option("meta", "-m", False, store_true)
-    .build(auto_send_output=True, aliases=config.tsugu_event_stage_aliases, extensions=[extension])
+    .build(auto_send_output=True, aliases=config.tsugu_event_stage_aliases, extensions=[extension], use_cmd_start=True)
 )
 
 @stage_search.handle()
-async def _(arp: Arparma, event: Event) -> None:
-    if arp.find("event_id"):
-        event_id = arp.query[int]("event_id")
+async def _(event_id: Match[int], event: Event, meta: Query[bool]=Query("meta.value", False)) -> None:
+    if event_id.available:
+        _event_id = event_id.result
     else:
-        event_id = None
-    
-    if (option := arp.options.get("meta", None)) is None:
-        meta = False
-    else:
-        meta: bool = option.value
+        _event_id = None
     
     try:
-        response = await event_stage(event.get_user_id(), event_id, meta)
+        response = await event_stage(event.get_user_id(), _event_id, meta.result)
     except Exception as exception:
         await stage_search.finish(f"错误: {exception}")
     
     segments: List[Segment] = []
     for _r in response:
         if isinstance(_r, str):
             segments.append(Text(_r))
         else:
             segments.append(Image(raw=_r))
     
     await stage_search.finish(UniMessage(segments))
 
 gacha_search = (
-    Command("查卡池 <gacha_id:int>", "查卡池").usage("根据卡池ID查询卡池信息")
-    .build(auto_send_output=True, aliases=config.tsugu_search_gacha_aliases, extensions=[extension])
+    Command("查卡池 <gacha_id:int>", "查卡池", meta=meta).usage("根据卡池ID查询卡池信息")
+    .build(auto_send_output=True, aliases=config.tsugu_search_gacha_aliases, extensions=[extension], use_cmd_start=True)
 )
 
 @gacha_search.handle()
-async def _(arp: Arparma, event: Event) -> None:
-    if arp.find("gacha_id"):
-        gacha_id = arp.query[int]("gacha_id")
-    else:
-        gacha_id = None
-    
-    if gacha_id is None:
+async def _(gacha_id: Match[int], event: Event) -> None:
+    if not gacha_id.available:
         await gacha_search.finish("错误: 未指定卡池ID")
     
     try:
-        response = await search_gacha(event.get_user_id(), gacha_id)
+        response = await search_gacha(event.get_user_id(), gacha_id.result)
     except Exception as exception:
         await gacha_search.finish(f"错误: {exception}")
     
     segments: List[Segment] = []
     for _r in response:
         if isinstance(_r, str):
             segments.append(Text(_r))
         else:
             segments.append(Image(raw=_r))
     
     await gacha_search.finish(UniMessage(segments))
 
 ycx = (
-    Command("ycx <tier:int> [event_id:int] [server_name:str]", "查询指定档位的预测线")
+    Command("ycx <tier:int> [event_id:int] [server_name:str]", "查询指定档位的预测线", meta=meta)
     .usage(f"查询指定档位的预测线，如果没有服务器名的话，服务器为用户的默认服务器。如果没有活动ID的话，活动为当前活动\n可用档线:\n{tier_list_of_server_to_string()}")
     .example("ycx 1000 :返回默认服务器当前活动1000档位的档线与预测线")
     .example("ycx 1000 177 jp:返回日服177号活动1000档位的档线与预测线")
-    .build(auto_send_output=True, aliases=config.tsugu_ycx_aliases, extensions=[extension])
+    .build(auto_send_output=True, aliases=config.tsugu_ycx_aliases, extensions=[extension], use_cmd_start=True)
 )
 
 @ycx.handle()
-async def _(arp: Arparma, event: Event) -> None:
-    if arp.find("tier"):
-        tier = arp.query[int]("tier")
-    else:
-        tier = None
-    
-    if tier is None:
+async def _(tier: Match[int], event_id: Match[int], server_name: Match[str], event: Event) -> None:
+    if not tier.available:
         await ycx.finish("请输入排名")
     
-    if arp.find("event_id"):
-        event_id = arp.query[int]("event_id")
+    if event_id.available:
+        _event_id = event_id.result
     else:
-        event_id = None
+        _event_id = None
     
-    if arp.find("server_name"):
-        server = arp.query[str]("server_name")
-        if server is None:
-            _server = None
-        else:
-            try:
-                _server = server_name_to_id(server)
-            except ValueError:
-                await ycx.finish("错误: 服务器不存在")
+    if server_name.available:
+        try:
+            _server = server_name_to_id(server_name.result)
+        except ValueError:
+            await ycx.finish("错误: 服务器不存在")
     else:
         _server = None
     
     try:
-        response = await search_ycx(event.get_user_id(), tier, event_id, _server)
+        response = await search_ycx(event.get_user_id(), tier.result, _event_id, _server)
     except Exception as exception:
         await ycx.finish(f"错误: {exception}")
     
     segments: List[Segment] = []
     for _r in response:
         if isinstance(_r, str):
             segments.append(Text(_r))
         else:
             segments.append(Image(raw=_r))
     
     await ycx.finish(UniMessage(segments))
 
 ycx_all = (
-    Command("ycxall [event_id:int] [server_name:str]", "查询所有档位的预测线")
+    Command("ycxall [event_id:int] [server_name:str]", "查询所有档位的预测线", meta=meta)
     .usage(f"查询所有档位的预测线，如果没有服务器名的话，服务器为用户的默认服务器。如果没有活动ID的话，活动为当前活动\n可用档线:\n{tier_list_of_server_to_string()}")
     .alias("myycx")
-    .build(auto_send_output=True, aliases=config.tsugu_ycx_all_aliases, extensions=[extension])
+    .build(auto_send_output=True, aliases=config.tsugu_ycx_all_aliases, extensions=[extension], use_cmd_start=True)
 )
 
 @ycx_all.handle()
-async def _(arp: Arparma, event: Event) -> None:
-    if arp.find("event_id"):
-        event_id = arp.query[int]("event_id")
-    else:
-        event_id = None
-    
-    if arp.find("server_name"):
-        server = arp.query[str]("server_name")
-        if server is None:
-            _server = None
-        else:
-            try:
-                _server = server_name_to_id(server)
-            except ValueError:
-                await ycx_all.finish("错误: 服务器不存在")
+async def _(event_id: Match[int], server_name: Match[str], event: Event) -> None:
+    if event_id.available:
+        _event_id = event_id.result
+    else:
+        _event_id = None
+    
+    if server_name.available:
+        try:
+            _server = server_name_to_id(server_name.result)
+        except ValueError:
+            await ycx_all.finish("错误: 服务器不存在")
     else:
         _server = None
     
     try:
-        response = await search_ycx_all(event.get_user_id(), _server, event_id)
+        response = await search_ycx_all(event.get_user_id(), _server, _event_id)
     except Exception as exception:
         await ycx_all.finish(f"错误: {exception}")
     
     segments: List[Segment] = []
     for _r in response:
         if isinstance(_r, str):
             segments.append(Text(_r))
         else:
             segments.append(Image(raw=_r))
     
     await ycx_all.finish(UniMessage(segments))
 
 lsycx = (
-    Command("lsycx <tier:int> [event_id:int] [server_name:str]", "查询指定档位的预测线")
+    Command("lsycx <tier:int> [event_id:int] [server_name:str]", "查询指定档位的预测线", meta=meta)
     .usage(f"查询指定档位的预测线，与最近的4期活动类型相同的活动的档线数据，如果没有服务器名的话，服务器为用户的默认服务器。如果没有活动ID的话，活动为当前活动\n可用档线:\n{tier_list_of_server_to_string()}")
     .example("lsycx 1000 :返回默认服务器当前活动的档线与预测线，与最近的4期活动类型相同的活动的档线数据")
     .example("lsycx 1000 177 jp:返回日服177号活动1000档位档线与最近的4期活动类型相同的活动的档线数据")
-    .build(auto_send_output=True, aliases=config.tsugu_lsycx_aliases, extensions=[extension])
+    .build(auto_send_output=True, aliases=config.tsugu_lsycx_aliases, extensions=[extension], use_cmd_start=True)
 )
 
 @lsycx.handle()
-async def _(arp: Arparma, event: Event) -> None:
-    if arp.find("tier"):
-        tier = arp.query[int]("tier")
-    else:
-        tier = None
-    
-    if tier is None:
+async def _(tier: Match[int], event_id: Match[int], server_name: Match[str], event: Event) -> None:
+    if not tier.available:
         await lsycx.finish("请输入排名")
     
-    if arp.find("event_id"):
-        event_id = arp.query[int]("event_id")
+    if event_id.available:
+        _event_id = event_id.result
     else:
-        event_id = None
+        _event_id = None
     
-    if arp.find("server_name"):
-        server = arp.query[str]("server_name")
-        if server is None:
-            _server = None
-        else:
-            try:
-                _server = server_name_to_id(server)
-            except ValueError:
-                await lsycx.finish("错误: 服务器不存在")
+    if server_name.available:
+        try:
+            _server = server_name_to_id(server_name.result)
+        except ValueError:
+            await lsycx.finish("错误: 服务器不存在")
     else:
         _server = None
     
     try:
-        response = await search_lsycx(event.get_user_id(), tier, event_id, _server)
+        response = await search_lsycx(event.get_user_id(), tier.result, _event_id, _server)
     except Exception as exception:
         await lsycx.finish(f"错误: {exception}")
     
     segments: List[Segment] = []
     for _r in response:
         if isinstance(_r, str):
             segments.append(Text(_r))
         else:
             segments.append(Image(raw=_r))
     
     await lsycx.finish(UniMessage(segments))
 
 gacha_simulate = (
-    Command("抽卡模拟 [times:int] [gacha_id:int]").usage("模拟抽卡，如果没有卡池ID的话，卡池为当前活动的卡池")
+    Command("抽卡模拟 [times:int] [gacha_id:int]", meta=meta).usage("模拟抽卡，如果没有卡池ID的话，卡池为当前活动的卡池")
     .example("抽卡模拟:模拟抽卡10次").example("抽卡模拟 300 922 :模拟抽卡300次，卡池为922号卡池")
-    .build(auto_send_output=True, aliases=config.tsugu_gacha_simulate_aliases, extensions=[extension])
+    .build(auto_send_output=True, aliases=config.tsugu_gacha_simulate_aliases, extensions=[extension], use_cmd_start=True)
 )
 
 @gacha_simulate.handle()
-async def _(arp: Arparma, event: Event) -> None:
-    if arp.find("times"):
-        times = arp.query[int]("times")
+async def _(times: Match[int], gacha_id: Match[int], event: Event) -> None:
+    if times.available:
+        _times = times.result
     else:
-        times = None
+        _times = None
     
-    if arp.find("gacha_id"):
-        gacha_id = arp.query[int]("gacha_id")
+    if gacha_id.available:
+        _gacha_id = gacha_id.result
     else:
-        gacha_id = None
+        _gacha_id = None
     
     try:
-        response = await simulate_gacha(event.get_user_id(), times, gacha_id)
+        response = await simulate_gacha(event.get_user_id(), _times, _gacha_id)
     except Exception as exception:
         await gacha_simulate.finish(f"错误: {exception}")
     
     segments: List[Segment] = []
     for _r in response:
         if isinstance(_r, str):
             segments.append(Text(_r))
```

### Comparing `nonebot_plugin_tsugu_bangdream_bot-0.1.6/nonebot_plugin_tsugu_bangdream_bot/_commands.py` & `nonebot_plugin_tsugu_bangdream_bot-0.1.7/nonebot_plugin_tsugu_bangdream_bot/_commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from base64 import b64decode
-from typing import List, Tuple, Union, Optional, Sequence
+from typing import List, Tuple, Union, Optional
 
 from nonebot import logger
 
 import tsugu_api_async
 from tsugu_api_core._typing import _Server, _ServerId, _TsuguUser, _DifficultyText
 
 from .config import CAR, FAKE
```

### Comparing `nonebot_plugin_tsugu_bangdream_bot-0.1.6/nonebot_plugin_tsugu_bangdream_bot/_utils.py` & `nonebot_plugin_tsugu_bangdream_bot-0.1.7/nonebot_plugin_tsugu_bangdream_bot/_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,50 +1,24 @@
-from tsugu_api_core._typing import _ServerId, _ServerName
+from typing import List
 
-_COMMAND_KEYWORDS = [
-    '查询玩家',
-    '查卡面',
-    '查玩家',
-    '查卡',
-    '查角色',
-    '查活动',
-    '查分数表',
-    '查询分数榜',
-    '查分数榜',
-    '查曲',
-    '查谱面',
-    '查卡池',
-    '查询分数表',
-    'ycx',
-    'ycxall',
-    'lsycx',
-    '抽卡模拟',
-    '绑定玩家',
-    '解除绑定',
-    '主服务器',
-    '设置默认服务器',
-    '玩家状态',
-    '开启车牌转发',
-    '关闭车牌转发'
-]
-COMMAND_KEYWORDS = sorted(_COMMAND_KEYWORDS, key=lambda x: len(x), reverse=True)
+from tsugu_api_core._typing import _ServerId, _ServerName
 
-tier_lists = {
+TIER_LISTS = {
     "jp": [20, 30, 40, 50, 100, 200, 300, 400, 500, 1000, 2000, 5000, 10000, 20000, 30000, 50000],
     "tw": [100, 500],
     "en": [50, 100, 300, 500, 1000, 2000, 2500],
     "kr": [100],
     "cn": [20, 30, 40, 50, 100, 200, 300, 400, 500, 1000, 2000, 3000, 4000, 5000, 10000, 20000, 30000, 50000]
 }
 
 def tier_list_of_server_to_string() -> str:
-    result: str = ""
-    for server, tiers in tier_lists.items():
-        result += server + " : " + ", ".join(str(tier) for tier in tiers) + "\n"
-    return result
+    results: List[str] = []
+    for server, tiers in TIER_LISTS.items():
+        results.append(server + " : " + ", ".join(str(tier) for tier in tiers))
+    return "\n".join(results)
 
 USAGES = {
     "开启车牌转发": "开启车牌转发",
     "关闭车牌转发": "关闭车牌转发",
     "绑定玩家信息": """绑定玩家 [server_name:str]
 开始玩家数据绑定流程，请不要在"绑定玩家"指令后添加玩家ID。省略服务器名时，默认为绑定到你当前的主服务器。请在获得临时验证数字后，将玩家签名改为该数字，并回复你的玩家ID""",
     "解除当前服务器的玩家绑定": """解除绑定 [server_name:str]
```

### Comparing `nonebot_plugin_tsugu_bangdream_bot-0.1.6/nonebot_plugin_tsugu_bangdream_bot/config.py` & `nonebot_plugin_tsugu_bangdream_bot-0.1.7/nonebot_plugin_tsugu_bangdream_bot/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tsugu_bangdream_bot-0.1.6/pyproject.toml` & `nonebot_plugin_tsugu_bangdream_bot-0.1.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [project]
 name = "nonebot-plugin-tsugu-bangdream-bot"
-version = "0.1.6"
+version = "0.1.7"
 description = "Koishi-Plugin-Tsugu-BanGDream-Bot 的 NoneBot2 实现"
 authors = [
     { name = "WindowsSov8forUs", email = "qwertyuiop2333@hotmail.com" },
 ]
 dependencies = [
     "nonebot2>=2.2.1",
-    "nonebot-plugin-alconna>=0.42.4",
+    "nonebot-plugin-alconna>=0.46.1",
     "tsugu-api-python>=1.2.0",
     "nonebot-plugin-userinfo>=0.2.4",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
 
 [project.license]
```

### Comparing `nonebot_plugin_tsugu_bangdream_bot-0.1.6/PKG-INFO` & `nonebot_plugin_tsugu_bangdream_bot-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-tsugu-bangdream-bot
-Version: 0.1.6
+Version: 0.1.7
 Summary: Koishi-Plugin-Tsugu-BanGDream-Bot 的 NoneBot2 实现
 Author-Email: WindowsSov8forUs <qwertyuiop2333@hotmail.com>
 License: MIT
 Requires-Python: >=3.8
 Requires-Dist: nonebot2>=2.2.1
-Requires-Dist: nonebot-plugin-alconna>=0.42.4
+Requires-Dist: nonebot-plugin-alconna>=0.46.1
 Requires-Dist: tsugu-api-python>=1.2.0
 Requires-Dist: nonebot-plugin-userinfo>=0.2.4
 Description-Content-Type: text/markdown
 
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-tsugu-bangdream-bot Version: 0.1.6
+Metadata-Version: 2.1 Name: nonebot-plugin-tsugu-bangdream-bot Version: 0.1.7
 Summary: Koishi-Plugin-Tsugu-BanGDream-Bot ç NoneBot2 å®ç° Author-Email:
 WindowsSov8forUs
 hotmail.com> License: MIT Requires-Python: >=3.8 Requires-Dist: nonebot2>=2.2.1
-Requires-Dist: nonebot-plugin-alconna>=0.42.4 Requires-Dist: tsugu-api-
+Requires-Dist: nonebot-plugin-alconna>=0.46.1 Requires-Dist: tsugu-api-
 python>=1.2.0 Requires-Dist: nonebot-plugin-userinfo>=0.2.4 Description-
 Content-Type: text/markdown
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
  # NoneBot-Plugin-Tsugu-BanGDream-Bot _â¨ [Koishi-Plugin-Tsugu-BanGDream-Bot]
  (https://github.com/Yamamoto-2/tsugu-bangdream-bot) ç NoneBot2 å®ç° â¨_
                        _[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]_[_p_y_p_i_][python]
```

