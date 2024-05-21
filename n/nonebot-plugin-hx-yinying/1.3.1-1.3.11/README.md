# Comparing `tmp/nonebot-plugin-hx-yinying-1.3.1.tar.gz` & `tmp/nonebot-plugin-hx-yinying-1.3.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-hx-yinying-1.3.1.tar", last modified: Mon May 20 07:01:17 2024, max compression
+gzip compressed data, was "nonebot-plugin-hx-yinying-1.3.11.tar", last modified: Mon May 20 16:44:30 2024, max compression
```

## Comparing `nonebot-plugin-hx-yinying-1.3.1.tar` & `nonebot-plugin-hx-yinying-1.3.11.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 07:01:17.769565 nonebot-plugin-hx-yinying-1.3.1/
--rw-rw-rw-   0        0        0     1098 2024-04-16 15:27:11.000000 nonebot-plugin-hx-yinying-1.3.1/LICENSE
--rw-rw-rw-   0        0        0     6502 2024-05-20 07:01:17.770568 nonebot-plugin-hx-yinying-1.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     6062 2024-04-28 16:24:12.000000 nonebot-plugin-hx-yinying-1.3.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-20 07:01:16.919557 nonebot-plugin-hx-yinying-1.3.1/nonebot_plugin_hx_yinying/
--rw-rw-rw-   0        0        0    56210 2024-05-15 15:18:50.000000 nonebot-plugin-hx-yinying-1.3.1/nonebot_plugin_hx_yinying/__init__.py
--rw-rw-rw-   0        0        0    75749 2024-05-20 06:58:45.000000 nonebot-plugin-hx-yinying-1.3.1/nonebot_plugin_hx_yinying/chat.py
--rw-rw-rw-   0        0        0     1533 2024-05-20 06:59:25.000000 nonebot-plugin-hx-yinying-1.3.1/nonebot_plugin_hx_yinying/config.py
--rw-rw-rw-   0        0        0     2549 2024-05-11 16:56:48.000000 nonebot-plugin-hx-yinying-1.3.1/nonebot_plugin_hx_yinying/image_check.py
--rw-rw-rw-   0        0        0     5372 2024-05-15 12:55:21.000000 nonebot-plugin-hx-yinying-1.3.1/nonebot_plugin_hx_yinying/report.py
--rw-rw-rw-   0        0        0     5032 2024-05-12 17:16:42.000000 nonebot-plugin-hx-yinying-1.3.1/nonebot_plugin_hx_yinying/smms.py
-drwxrwxrwx   0        0        0        0 2024-05-20 07:01:17.762548 nonebot-plugin-hx-yinying-1.3.1/nonebot_plugin_hx_yinying.egg-info/
--rw-rw-rw-   0        0        0     6502 2024-05-20 07:01:15.000000 nonebot-plugin-hx-yinying-1.3.1/nonebot_plugin_hx_yinying.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      499 2024-05-20 07:01:15.000000 nonebot-plugin-hx-yinying-1.3.1/nonebot_plugin_hx_yinying.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 07:01:15.000000 nonebot-plugin-hx-yinying-1.3.1/nonebot_plugin_hx_yinying.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      274 2024-05-20 07:01:15.000000 nonebot-plugin-hx-yinying-1.3.1/nonebot_plugin_hx_yinying.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-05-20 07:01:15.000000 nonebot-plugin-hx-yinying-1.3.1/nonebot_plugin_hx_yinying.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2024-05-20 07:01:17.777568 nonebot-plugin-hx-yinying-1.3.1/setup.cfg
--rw-rw-rw-   0        0        0     1003 2024-05-20 07:00:39.000000 nonebot-plugin-hx-yinying-1.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 16:44:30.020673 nonebot-plugin-hx-yinying-1.3.11/
+-rw-rw-rw-   0        0        0     1098 2024-04-16 15:27:11.000000 nonebot-plugin-hx-yinying-1.3.11/LICENSE
+-rw-rw-rw-   0        0        0     6677 2024-05-20 16:44:30.024588 nonebot-plugin-hx-yinying-1.3.11/PKG-INFO
+-rw-rw-rw-   0        0        0     6236 2024-05-20 15:06:16.000000 nonebot-plugin-hx-yinying-1.3.11/README.md
+drwxrwxrwx   0        0        0        0 2024-05-20 16:44:29.910614 nonebot-plugin-hx-yinying-1.3.11/nonebot_plugin_hx_yinying/
+-rw-rw-rw-   0        0        0    55243 2024-05-20 16:29:51.000000 nonebot-plugin-hx-yinying-1.3.11/nonebot_plugin_hx_yinying/__init__.py
+-rw-rw-rw-   0        0        0    76462 2024-05-20 16:20:43.000000 nonebot-plugin-hx-yinying-1.3.11/nonebot_plugin_hx_yinying/chat.py
+-rw-rw-rw-   0        0        0     1638 2024-05-20 16:34:24.000000 nonebot-plugin-hx-yinying-1.3.11/nonebot_plugin_hx_yinying/config.py
+-rw-rw-rw-   0        0        0     2549 2024-05-11 16:56:48.000000 nonebot-plugin-hx-yinying-1.3.11/nonebot_plugin_hx_yinying/image_check.py
+-rw-rw-rw-   0        0        0     3889 2024-05-20 15:22:24.000000 nonebot-plugin-hx-yinying-1.3.11/nonebot_plugin_hx_yinying/report.py
+-rw-rw-rw-   0        0        0     5032 2024-05-12 17:16:42.000000 nonebot-plugin-hx-yinying-1.3.11/nonebot_plugin_hx_yinying/smms.py
+drwxrwxrwx   0        0        0        0 2024-05-20 16:44:30.007673 nonebot-plugin-hx-yinying-1.3.11/nonebot_plugin_hx_yinying.egg-info/
+-rw-rw-rw-   0        0        0     6677 2024-05-20 16:44:29.000000 nonebot-plugin-hx-yinying-1.3.11/nonebot_plugin_hx_yinying.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      499 2024-05-20 16:44:29.000000 nonebot-plugin-hx-yinying-1.3.11/nonebot_plugin_hx_yinying.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 16:44:29.000000 nonebot-plugin-hx-yinying-1.3.11/nonebot_plugin_hx_yinying.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      274 2024-05-20 16:44:29.000000 nonebot-plugin-hx-yinying-1.3.11/nonebot_plugin_hx_yinying.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-05-20 16:44:29.000000 nonebot-plugin-hx-yinying-1.3.11/nonebot_plugin_hx_yinying.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2024-05-20 16:44:30.056152 nonebot-plugin-hx-yinying-1.3.11/setup.cfg
+-rw-rw-rw-   0        0        0     1003 2024-05-20 15:03:45.000000 nonebot-plugin-hx-yinying-1.3.11/setup.py
```

### Comparing `nonebot-plugin-hx-yinying-1.3.1/LICENSE` & `nonebot-plugin-hx-yinying-1.3.11/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-hx-yinying-1.3.1/PKG-INFO` & `nonebot-plugin-hx-yinying-1.3.11/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-hx-yinying
-Version: 1.3.1
+Version: 1.3.11
 Summary: chat with yinying
 Home-page: https://github.com/huanxin996/nonebot_plugin_hx-yinying
 Author: Huan Xin
 Author-email: mc.xiaolang@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -205,24 +205,32 @@
 
 ### smms_password
 - 类型：`str`
 - 默认值：`None`
 - 说明：这里是smms的密码（图床）
 - 重要：非必填（若smm_token为空，则需要填写账号密码）
 
+
+### hx_chatcommand
+- 类型：`list`
+- 默认值：`["hx","chat"]`
+- 说明：这里是聊天自定义命令头
+- 重要：非必填
+
 </details>
 <br>
 
 配置文件示例（默认模板）
 
 ```dotenv
 yinying_appid=你的appid
 yinying_token=你的token(不带bearer)
 hx_path=C:\Users\user\Desktop
 SUPERUSERS=["114514"]
+hx_chatcommand = ["hx","chat"]
 image_check_appid=你的appid
 image_check_token=你的token
 smms_token=你获取到的token
 smms_username=114514
 smms_password=114514
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 1.3.1 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 1.3.11 Summary:
 chat with yinying Home-page: https://github.com/huanxin996/nonebot_plugin_hx-
 yinying Author: Huan Xin Author-email: mc.xiaolang@foxmail.com Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Description-Content-
 Type: text/markdown License-File: LICENSE [![All Contributors](https://
 img.shields.io/badge/all_contributors-2-orange.svg?style=flat-square)]
 (#contributors-) * @Author : huanxin996 * @Date : 2024-4-17 * @LastEditors :
@@ -60,17 +60,19 @@
 è¯´æï¼è¿éæ¯smmsçtokenï¼å¾åºï¼ -
 éè¦ï¼éå¿å¡«ï¼å¯å¨å¡«åsmms_usernameåsmms_passwordï¼åéè¿botçªå£è·åã
 ### smms_username - ç±»åï¼`str` - é»è®¤å¼ï¼`None` -
 è¯´æï¼è¿éæ¯smmsçè´¦å·idï¼å¾åºï¼ -
 éè¦ï¼éå¿å¡«å¿å¡«ï¼è¥smm_tokenä¸ºç©ºï¼åéè¦å¡«åè´¦å·å¯ç ï¼
 ### smms_password - ç±»åï¼`str` - é»è®¤å¼ï¼`None` -
 è¯´æï¼è¿éæ¯smmsçå¯ç ï¼å¾åºï¼ -
-éè¦ï¼éå¿å¡«ï¼è¥smm_tokenä¸ºç©ºï¼åéè¦å¡«åè´¦å·å¯ç ï¼
+éè¦ï¼éå¿å¡«ï¼è¥smm_tokenä¸ºç©ºï¼åéè¦å¡«åè´¦å·å¯ç ï¼ ###
+hx_chatcommand - ç±»åï¼`list` - é»è®¤å¼ï¼`["hx","chat"]` -
+è¯´æï¼è¿éæ¯èå¤©èªå®ä¹å½ä»¤å¤´ - éè¦ï¼éå¿å¡«
 éç½®æä»¶ç¤ºä¾ï¼é»è®¤æ¨¡æ¿ï¼ ```dotenv yinying_appid=ä½ çappid
 yinying_token=ä½ çtoken(ä¸å¸¦bearer) hx_path=C:\Users\user\Desktop
-SUPERUSERS=["114514"] image_check_appid=ä½ çappid
-image_check_token=ä½ çtoken smms_token=ä½ è·åå°çtoken
-smms_username=114514 smms_password=114514 ``` ## æ¬å°åç±»configè¯¦è§£
-ccoonnffiigg__gglloobbaall..jjssoonn å¨åäºå¨åäº
+SUPERUSERS=["114514"] hx_chatcommand = ["hx","chat"]
+image_check_appid=ä½ çappid image_check_token=ä½ çtoken
+smms_token=ä½ è·åå°çtoken smms_username=114514 smms_password=114514 ```
+## æ¬å°åç±»configè¯¦è§£ ccoonnffiigg__gglloobbaall..jjssoonn å¨åäºå¨åäº
 ccoonnffiigg__ggrroouupp..jjssoonn å¨åäºå¨åäº
 ccoonnffiigg__uusseerr..jjssoonn å¨åäºå¨åäº
 ## Contributors â¨
```

### Comparing `nonebot-plugin-hx-yinying-1.3.1/README.md` & `nonebot-plugin-hx-yinying-1.3.11/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -192,24 +192,32 @@
 
 ### smms_password
 - 类型：`str`
 - 默认值：`None`
 - 说明：这里是smms的密码（图床）
 - 重要：非必填（若smm_token为空，则需要填写账号密码）
 
+
+### hx_chatcommand
+- 类型：`list`
+- 默认值：`["hx","chat"]`
+- 说明：这里是聊天自定义命令头
+- 重要：非必填
+
 </details>
 <br>
 
 配置文件示例（默认模板）
 
 ```dotenv
 yinying_appid=你的appid
 yinying_token=你的token(不带bearer)
 hx_path=C:\Users\user\Desktop
 SUPERUSERS=["114514"]
+hx_chatcommand = ["hx","chat"]
 image_check_appid=你的appid
 image_check_token=你的token
 smms_token=你获取到的token
 smms_username=114514
 smms_password=114514
 ```
```

#### html2text {}

```diff
@@ -54,17 +54,19 @@
 è¯´æï¼è¿éæ¯smmsçtokenï¼å¾åºï¼ -
 éè¦ï¼éå¿å¡«ï¼å¯å¨å¡«åsmms_usernameåsmms_passwordï¼åéè¿botçªå£è·åã
 ### smms_username - ç±»åï¼`str` - é»è®¤å¼ï¼`None` -
 è¯´æï¼è¿éæ¯smmsçè´¦å·idï¼å¾åºï¼ -
 éè¦ï¼éå¿å¡«å¿å¡«ï¼è¥smm_tokenä¸ºç©ºï¼åéè¦å¡«åè´¦å·å¯ç ï¼
 ### smms_password - ç±»åï¼`str` - é»è®¤å¼ï¼`None` -
 è¯´æï¼è¿éæ¯smmsçå¯ç ï¼å¾åºï¼ -
-éè¦ï¼éå¿å¡«ï¼è¥smm_tokenä¸ºç©ºï¼åéè¦å¡«åè´¦å·å¯ç ï¼
+éè¦ï¼éå¿å¡«ï¼è¥smm_tokenä¸ºç©ºï¼åéè¦å¡«åè´¦å·å¯ç ï¼ ###
+hx_chatcommand - ç±»åï¼`list` - é»è®¤å¼ï¼`["hx","chat"]` -
+è¯´æï¼è¿éæ¯èå¤©èªå®ä¹å½ä»¤å¤´ - éè¦ï¼éå¿å¡«
 éç½®æä»¶ç¤ºä¾ï¼é»è®¤æ¨¡æ¿ï¼ ```dotenv yinying_appid=ä½ çappid
 yinying_token=ä½ çtoken(ä¸å¸¦bearer) hx_path=C:\Users\user\Desktop
-SUPERUSERS=["114514"] image_check_appid=ä½ çappid
-image_check_token=ä½ çtoken smms_token=ä½ è·åå°çtoken
-smms_username=114514 smms_password=114514 ``` ## æ¬å°åç±»configè¯¦è§£
-ccoonnffiigg__gglloobbaall..jjssoonn å¨åäºå¨åäº
+SUPERUSERS=["114514"] hx_chatcommand = ["hx","chat"]
+image_check_appid=ä½ çappid image_check_token=ä½ çtoken
+smms_token=ä½ è·åå°çtoken smms_username=114514 smms_password=114514 ```
+## æ¬å°åç±»configè¯¦è§£ ccoonnffiigg__gglloobbaall..jjssoonn å¨åäºå¨åäº
 ccoonnffiigg__ggrroouupp..jjssoonn å¨åäºå¨åäº
 ccoonnffiigg__uusseerr..jjssoonn å¨åäºå¨åäº
 ## Contributors â¨
```

### Comparing `nonebot-plugin-hx-yinying-1.3.1/nonebot_plugin_hx_yinying/__init__.py` & `nonebot-plugin-hx-yinying-1.3.11/nonebot_plugin_hx_yinying/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -73,27 +73,28 @@
     logger.opt(colors=True).error(f"【Hx】定时任务加载失败！！，联系开发者！错误捕获{e}")
 
 
 
 
 #主要命令列表
 msg_at = on_message(rule=Rule(chek_rule_base)&to_me(), priority=10,  block=True)
-msg_ml = on_command("hx", aliases={"chat","yinying","yy"},rule=Rule(chek_rule_base),  priority=10, block=True)
+msg_ml = on_command("yinying_chat", aliases=hx_config.hx_chatcommand,rule=Rule(chek_rule_base),  priority=15, block=True)
 clear =  on_command("刷新对话", aliases={"clear"},rule=Rule(chek_rule_base),  priority=0, block=True)
 history_get = on_command("导出对话", aliases={"getchat"},rule=Rule(chek_rule_base),  priority=0, block=True)
 set_global_config = on_command("设置全局配置", aliases={"设置配置全局","globalset"},rule=Rule(chek_rule_admin),  priority=0, block=True)
 model_list = on_command("模型列表", aliases={"modellist","chat模型列表"},rule=Rule(chek_rule_base),  priority=0, block=True)
 model_handoff = on_command("切换模型", aliases={"qhmodel","切换chat模型","模型切换"},rule=Rule(chek_rule_base),  priority=0, block=True)
 easycyber_set = on_command("easycyber", aliases={"easycyber设置","hxworld"},rule=Rule(chek_rule_base),  priority=0, block=True)
 cyber_set = on_command("cyber", aliases={"cyber设置","Hxworld"},rule=Rule(chek_rule_base),  priority=0, block=True)
 admin_set = on_command("控制台操作", aliases={"管理控制台","setstart"},rule=Rule(chek_rule_admin),  priority=0, block=True)
 verision = on_command("确认版本", aliases={"旅行伙伴确认","版本确认"},rule=Rule(chek_rule_base),  priority=0, block=True)
 character = on_command("sd", aliases={"旅行伙伴加入","设定加入"},rule=Rule(chek_rule_base),  priority=0, block=True)
 chat_ne = on_command("加入订阅", aliases={"旅行伙伴觉醒","订阅加入"},rule=Rule(chek_rule_base),  priority=0, block=True)
 time_noend = on_command("切换时间线", aliases={"切换模式"},rule=Rule(chek_rule_base),  priority=0, block=True)
+gloubalblack_add = on_command("全局拉黑", aliases={"银影不要理"},rule=Rule(chek_rule_admin),  priority=0, block=True)
 ces = on_command("测试服务", aliases={"测试报错"},rule=Rule(chek_rule_base), priority=0, block=True)
 
 #生命模式-无限时间(仅供cyber和easycyber使用)
 @time_noend.got(
     "msg",
     prompt=f"请输入时间线\n当前仅支持\n无限-overworld\n普通-nether\n请输入全称：无限-overworld",
 )
@@ -112,14 +113,41 @@
         with open(f'{log_dir}/config/config_user.json','w',encoding='utf-8') as file:
             json.dump(config_1,file)
         msg = "..载入成功"
     else:
         msg = "时间线重叠..."
     await send_msg(matcher,event,msg)
 
+#拉黑用户、
+@gloubalblack_add.handle()
+async def gloubalblack_add(matcher: Matcher,bot:Bot,event: MessageEvent, msg: Message = CommandArg()):
+    text = msg.extract_plain_text()
+    groupid = event.group_id
+    config_1 = config_in_global()
+    user_config = json_get(config_1,"blacklist_user")
+    if not text:
+        id = await extract_member_at(groupid,msg,bot)
+        for num in id:
+            if num in user_config:
+                logger.warning(f"{num}已在黑名单内")
+            else:
+                user_config.append(num)
+        config_1["blacklist_user"] = user_config
+        with open(f'{log_dir}/config/config_global.json','w',encoding='utf-8') as file:
+            json.dump(config_1,file)
+        msg= f"{id}\n拉黑成功"
+    else:
+        if text in user_config:
+            await send_msg(matcher, event, "该用户已在黑名单内")
+        user_config.append(text)
+        config_1["blacklist_user"] = user_config
+        with open(f'{log_dir}/config/config_global.json','w',encoding='utf-8') as file:
+            json.dump(config_1,file)
+            msg= f"{text}拉黑成功"
+    await send_msg(matcher, event, msg)
 
 
 #自定义自己的设定
 @character.handle()
 async def character(matcher: Matcher,bot:Bot, event: MessageEvent, msg: Message = CommandArg()):
     user = get_id(event)
     nick = await get_nick(bot,event)
@@ -485,196 +513,166 @@
     "msg",
     prompt=f"发送以下选项执行相应功能\n投稿 #投稿自定义预设(不允许同名)\n载入 #载入自定义预设(不允许不存在)\n查看列表 #列出所有公开的自定义预设\n退出 #退出设置\n发送非预期命令则退出",
 )
 async def _(matcher: Matcher, bot:Bot, event: MessageEvent, s: T_State,events: Event):
     id = get_id(event)
     text = unescape(event.get_plaintext().strip())
     easycyber_package = {}
+    if text == "退出":
+        s["last"] = True
+        msg = "已退出"
+        await send_msg(matcher,event,msg) 
     if "last" not in s:
         s["last"] = ""
     if s["last"]:
         if s["last"] == "增加":
             if text == "Hx" or text == "HX" or text == "幻歆":
                 s["last"] = True
                 msg = "easycyber预设“Hx”不能删除或修改，如要改动请改源码"
                 await send_msg(matcher,event,msg)
-            elif text == "退出":
-                s["last"] = True
-                msg = "已退出"
-                await send_msg(matcher,event,msg)
             elif text in easycyber_in_tg(text,False) or text in easycyber_in(text,False) or not text:
                 s["last"] = "增加"
                 msg = "该预设角色名称已经存在，请不要重复使用该昵称，请重新输入，如需退出请发送退出"
                 await send_msg_reject(matcher,event,msg)
             else:
                 s["cfnickname"] = text
                 s["last"] = "cfSpecies"
                 msg = "请输入角色物种"
                 await send_msg_reject(matcher,event,msg)
         if s["last"] == "cfSpecies":
-            if text == "退出":
-                s["last"] = True
-                msg = "已退出"
-                await send_msg(matcher,event,msg)
-            else:
-                s["cfSpecies"] = text
-                s["last"] = "cfconage"
-                msg = "请输入角色表现:(比如\n child--[幼年]\n young--[青年]\n adult--[成年]\nps:只输入--前面的英文即可"
-                await send_msg_reject(matcher,event,msg)
+            s["cfSpecies"] = text
+            s["last"] = "cfconage"
+            msg = "请输入角色表现:(比如\n child--[幼年]\n young--[青年]\n adult--[成年]\nps:只输入--前面的英文即可"
+            await send_msg_reject(matcher,event,msg)
 
         if s["last"] == "cfconage":
-            if text == "退出":
-                s["last"] = True
-                msg = "已退出"
-                await send_msg(matcher,event,msg)
+            key = ['child','young','adult']
+            if not text in key:
+                s["last"] = "cfconage"
+                msg = "未找到该类型的角色聊天年龄!请重新输入，如需退出请发送：退出"
+                await send_msg_reject(matcher,event,msg)
             else:
-                key = ['child','young','adult']
-                if not text in key:
-                    s["last"] = "cfconage"
-                    msg = "未找到该类型的角色聊天年龄!请重新输入，如需退出请发送：退出"
-                    await send_msg_reject(matcher,event,msg)
-                else:
-                    s["cfconage"] = text
-                    s["last"] = "cfconstyle"
-                    msg = "请输入角色聊天风格:(比如\n vivid--[活泼]\n sentiment--[富有情感(共情大师？)]\n assistant--[助理]\n chilly--[冷酷无情]\n social_anxiety--[社恐]\nps:只输入--前面的英文即可"
-                    await send_msg_reject(matcher,event,msg)
+                s["cfconage"] = text
+                s["last"] = "cfconstyle"
+                msg = "请输入角色聊天风格:(比如\n vivid--[活泼]\n sentiment--[富有情感(共情大师？)]\n assistant--[助理]\n chilly--[冷酷无情]\n social_anxiety--[社恐]\nps:只输入--前面的英文即可"
+                await send_msg_reject(matcher,event,msg)
 
         if s["last"] == "cfconstyle":
-            if text == "退出":
-                s["last"] = True
-                msg = "已退出"
-                await send_msg(matcher,event,msg)
+            key = ['vivid','sentiment','assistant','chilly','social_anxiety']
+            if not text in key:
+                s["last"] = "cfconstyle"
+                msg = "未找到该类型的角色聊天风格！请重新输入，如需退出请发送：退出"
+                await send_msg_reject(matcher,event,msg)
             else:
-                key = ['vivid','sentiment','assistant','chilly','social_anxiety']
-                if not text in key:
-                    s["last"] = "cfconstyle"
-                    msg = "未找到该类型的角色聊天风格！请重新输入，如需退出请发送：退出"
-                    await send_msg_reject(matcher,event,msg)
-                else:
-                    s["cfconstyle"] = json_replace(text)
-                    s["last"] = "cfstory"
-                    msg = "请输入角色的背景故事（这对他真的很重要\n[胡言乱语：我要给他完整的一生！！！]"
-                    await send_msg_reject(matcher,event,msg)
+                s["cfconstyle"] = json_replace(text)
+                s["last"] = "cfstory"
+                msg = "请输入角色的背景故事（这对他真的很重要\n[胡言乱语：我要给他完整的一生！！！]"
+                await send_msg_reject(matcher,event,msg)
 
         if s["last"] == "cfstory":
-            if text == "退出":
-                s["last"] = True
-                msg = "已退出"
-                await send_msg(matcher,event,msg)
-            else:
-                s["cfstory"] = text
-                s["last"] = "public"
-                msg = "该角色是否公开？(最后一步)完成将发送到bot管理站进行审核，审核通过后即可使用,请发送是或否或者公开或不公开"
-                await send_msg_reject(matcher,event,msg)
+            s["cfstory"] = text
+            s["last"] = "public"
+            msg = "该角色是否公开？(最后一步)完成将发送到bot管理站进行审核，审核通过后即可使用,请发送是或否或者公开或不公开"
+            await send_msg_reject(matcher,event,msg)
 
         if s["last"] == "public":
-            if text == "退出":
-                s["last"] = True
-                msg = "已退出"
-                await send_msg(matcher,event,msg)
+            key = {"是":True,"否":False,"公开":True,"不公开":False}
+            if not text in key:
+                s["last"] = "public"
+                msg = "非正确格式！请重新输入，如需退出请发送：退出"
+                await send_msg_reject(matcher,event,msg)
             else:
-                key = {"是":True,"否":False,"公开":True,"不公开":False}
-                if not text in key:
-                    s["last"] = "public"
-                    msg = "非正确格式！请重新输入，如需退出请发送：退出"
-                    await send_msg_reject(matcher,event,msg)
+                name = s["cfnickname"]
+                species = s["cfSpecies"]
+                age = s["cfconage"]
+                stytle = s["cfconstyle"]
+                story = s["cfstory"]
+                easycyber_package["cfNickname"] = s["cfnickname"]
+                easycyber_package["cfSpecies"] = s["cfSpecies"]
+                easycyber_package["cfConAge"] = s["cfconage"]
+                easycyber_package["cfConStyle"] = s["cfconstyle"]
+                easycyber_package["cfStory"] = s["cfstory"]
+                easycyber_package["public"] = key[f"{text}"]
+                easycyber_package["creator"] = int(id)
+                s["last"] = True
+                cybernick = s["cfnickname"]
+                g = json_get(config_in_global(),"admin_group")
+                u = json_get(config_in_global(),"admin_pro")
+                g_k = json_get(config_in_global(),"admin_group_switch")
+                u_k = json_get(config_in_global(),"admin_user_switch")
+                msg_tg = f"新投稿！\n来源于QQ[{id}]\n以下为设定内容\n===========\n昵称:{name}\n物种:{species}\n年龄:{age}\n回复风格:{stytle}\n角色故事:{story}\n==========="
+                msg = "投稿成功！，等待审核(问就是权限还没写好)]"
+                if not g and not u:
+                    msg ="bot管理者未配置，超级管理员和bot控制台,审核失败！"
+                elif not u and g:
+                    easycyber_in_tg(cybernick,easycyber_package)
+                    await bot.call_api("send_group_msg",group_id=g, message=msg_tg)
+                elif not g and u:
+                    easycyber_in_tg(cybernick,easycyber_package)
+                    await bot.call_api("send_private_msg",user_id=u, message=msg_tg)
+                elif u_k and g_k:
+                    easycyber_in_tg(cybernick,easycyber_package)
+                    await bot.call_api("send_group_msg",group_id=g, message=msg_tg)
+                    await bot.call_api("send_private_msg",user_id=u, message=msg_tg)
+                elif u_k:
+                    easycyber_in_tg(cybernick,easycyber_package)
+                    adminid = json_get(config_in_global(),"admin_pro")
+                    await bot.call_api("send_private_msg",user_id=u, message=msg_tg)
                 else:
-                    name = s["cfnickname"]
-                    species = s["cfSpecies"]
-                    age = s["cfconage"]
-                    stytle = s["cfconstyle"]
-                    story = s["cfstory"]
-                    easycyber_package["cfNickname"] = s["cfnickname"]
-                    easycyber_package["cfSpecies"] = s["cfSpecies"]
-                    easycyber_package["cfConAge"] = s["cfconage"]
-                    easycyber_package["cfConStyle"] = s["cfconstyle"]
-                    easycyber_package["cfStory"] = s["cfstory"]
-                    easycyber_package["public"] = key[f"{text}"]
-                    easycyber_package["creator"] = int(id)
-                    s["last"] = True
-                    cybernick = s["cfnickname"]
-                    g = json_get(config_in_global(),"admin_group")
-                    u = json_get(config_in_global(),"admin_pro")
-                    g_k = json_get(config_in_global(),"admin_group_switch")
-                    u_k = json_get(config_in_global(),"admin_user_switch")
-                    msg_tg = f"新投稿！\n来源于QQ[{id}]\n以下为设定内容\n===========\n昵称:{name}\n物种:{species}\n年龄:{age}\n回复风格:{stytle}\n角色故事:{story}\n==========="
-                    msg = "投稿成功！，等待审核(问就是权限还没写好)]"
-                    if not g and not u:
-                        msg ="bot管理者未配置，超级管理员和bot控制台,审核失败！"
-                    elif not u and g:
-                        easycyber_in_tg(cybernick,easycyber_package)
-                        await bot.call_api("send_group_msg",group_id=g, message=msg_tg)
-                    elif not g and u:
-                        easycyber_in_tg(cybernick,easycyber_package)
-                        await bot.call_api("send_private_msg",user_id=u, message=msg_tg)
-                    elif u_k and g_k:
-                        easycyber_in_tg(cybernick,easycyber_package)
-                        await bot.call_api("send_group_msg",group_id=g, message=msg_tg)
-                        await bot.call_api("send_private_msg",user_id=u, message=msg_tg)
-                    elif u_k:
-                        easycyber_in_tg(cybernick,easycyber_package)
-                        adminid = json_get(config_in_global(),"admin_pro")
-                        await bot.call_api("send_private_msg",user_id=u, message=msg_tg)
-                    else:
-                        easycyber_in_tg(cybernick,easycyber_package)
-                        await bot.call_api("send_group_msg",group_id=g, message=msg_tg)
-                    await send_msg(matcher,event,msg)
+                    easycyber_in_tg(cybernick,easycyber_package)
+                    await bot.call_api("send_group_msg",group_id=g, message=msg_tg)
+                await send_msg(matcher,event,msg)
 
 
         if s["last"] == "载入":
-            if text == "退出":
-                s["last"] = True
-                msg = "已退出"
-                await send_msg(matcher,event,msg)
-            else:
-                s["last"] = True
-                if isinstance(events, GroupMessageEvent):
-                    groupid = get_groupid(event)
-                    config = config_in_group(groupid)
-                    config_group = json_get(config,groupid)
-                    promte = json_get(easycyber_in(False,False),f"{text}")
-                    public = json_get(promte,"public")
-                    if not public:
-                        msg = f"{text}模型拒绝被加载(可能是模型不存在或者模型非公开！)"      
+            s["last"] = True
+            if isinstance(events, GroupMessageEvent):
+                groupid = get_groupid(event)
+                config = config_in_group(groupid)
+                config_group = json_get(config,groupid)
+                promte = json_get(easycyber_in(False,False),f"{text}")
+                public = json_get(promte,"public")
+                if not public:
+                    msg = f"{text}模型拒绝被加载(可能是模型不存在或者模型非公开！)"      
+                else:
+                    if config_group["easycharacter_in"] == text:
+                        msg = f"{text}模型已加载，请勿重新加载"  
                     else:
-                        if config_group["easycharacter_in"] == text:
-                            msg = f"{text}模型已加载，请勿重新加载"  
-                        else:
-                            config_group["easycharacter_in"] = f"{text}"
-                            config[f"{groupid}"] = config_group
-                            with open(f'{log_dir}/config/config_group.json','w',encoding='utf-8') as file:
-                                json.dump(config,file)
-                                msg = f"{text}加载成功！" 
-                else:
-                    config_user = config_in_user(id,False)
-                    user = json_get(config_user,f"{id}")
-                    promte = json_get(easycyber_in(False,False),f"{text}")
-                    public = json_get(promte,"public")
-                    creator = json_get(promte,"creator")
-                    if creator == id:
-                        if user["easycharacter_in"]== text:
-                            msg = f"{text}模型已加载，请勿重新加载"  
-                        else:
-                            user["easycharacter_in"] = f"{text}"
-                            config_user[f"{id}"] = user
-                            with open(f'{log_dir}/config/config_user.json','w',encoding='utf-8') as file:
-                                json.dump(config_user,file)
-                                msg = f"{text}加载成功！"
-                    elif not public:
-                        msg = f"{text}模型拒绝被加载(可能是模型不存在或者模型非公开！)"      
+                        config_group["easycharacter_in"] = f"{text}"
+                        config[f"{groupid}"] = config_group
+                        with open(f'{log_dir}/config/config_group.json','w',encoding='utf-8') as file:
+                            json.dump(config,file)
+                            msg = f"{text}加载成功！" 
+            else:
+                config_user = config_in_user(id,False)
+                user = json_get(config_user,f"{id}")
+                promte = json_get(easycyber_in(False,False),f"{text}")
+                public = json_get(promte,"public")
+                creator = json_get(promte,"creator")
+                if creator == id:
+                    if user["easycharacter_in"]== text:
+                        msg = f"{text}模型已加载，请勿重新加载"  
                     else:
-                        if user["easycharacter_in"] == text:
-                            msg = f"{text}模型已加载，请勿重新加载"  
-                        else:
-                            user["easycharacter_in"] = f"{text}"
-                            config_user[f"{id}"] = user
-                            with open(f'{log_dir}/config/config_user.json','w',encoding='utf-8') as file:
-                                json.dump(config_user,file)
-                                msg = f"{text}加载成功！" 
-                await send_msg(matcher,event,msg)
+                        user["easycharacter_in"] = f"{text}"
+                        config_user[f"{id}"] = user
+                        with open(f'{log_dir}/config/config_user.json','w',encoding='utf-8') as file:
+                            json.dump(config_user,file)
+                            msg = f"{text}加载成功！"
+                elif not public:
+                    msg = f"{text}模型拒绝被加载(可能是模型不存在或者模型非公开！)"      
+                else:
+                    if user["easycharacter_in"] == text:
+                        msg = f"{text}模型已加载，请勿重新加载"  
+                    else:
+                        user["easycharacter_in"] = f"{text}"
+                        config_user[f"{id}"] = user
+                        with open(f'{log_dir}/config/config_user.json','w',encoding='utf-8') as file:
+                            json.dump(config_user,file)
+                            msg = f"{text}加载成功！" 
+            await send_msg(matcher,event,msg)
     # 增加预设
     if text == "投稿":
         s["last"] = "增加"
         msg = "请输入角色昵称"
         await send_msg_reject(matcher,event,msg)
     if text == "载入":
         s["last"] = "载入"
@@ -708,14 +706,18 @@
     "msg",
     prompt=f"发送以下选项执行相应功能\n投稿 #投稿自定义预设(不允许同名)\n载入 #载入自定义预设(不允许不存在)\n查看列表 #列出所有公开的自定义预设\n退出 #退出设置\n发送非预期命令则退出",
 )
 async def _(matcher: Matcher, bot:Bot, event: MessageEvent, s: T_State,events: Event):
     id = get_id(event)
     text = unescape(event.get_plaintext().strip())
     easycyber_package = {}
+    if text == "退出":
+        s["last"] = True
+        msg = "已退出"
+        await send_msg(matcher,event,msg)  
     if "last" not in s:
         s["last"] = ""
     if s["last"]:
         if s["last"] == "增加":
             if text == "Hx" or text == "HX" or text == "幻歆":
                 s["last"] = True
                 msg = "cyber预设“Hx”不能删除或修改，如要改动请改源码"
@@ -727,120 +729,105 @@
             else:
                 s["name"] = text
                 s["last"] = "system"
                 msg = "该角色的systempromote是？"
                 await send_msg_reject(matcher,event,msg)
 
         if s["last"] == "system":
-            if text == "退出":
-                s["last"] = True
-                msg = "已退出"
-                await send_msg(matcher,event,msg)
-            else:
-                s["systempromote"] = text
-                s["last"] = "public"
-                msg = "该角色是否公开u\n请发送公开或不公开（也可以是是或否或者True或False）"
-                await send_msg_reject(matcher,event,msg)
+            s["systempromote"] = text
+            s["last"] = "public"
+            msg = "该角色是否公开u\n请发送公开或不公开（也可以是是或否或者True或False）"
+            await send_msg_reject(matcher,event,msg)
 
         if s["last"] == "public":
-            if text == "退出":
-                s["last"] = True
-                msg = "已退出"
-                await send_msg(matcher,event,msg)
+            key = {"是":True,"否":False,"公开":True,"不公开":False}
+            if not text in key:
+                s["last"] = "public"
+                msg = "非正确格式！请重新输入，如需退出请发送：退出"
+                await send_msg_reject(matcher,event,msg)
             else:
-                key = {"是":True,"否":False,"公开":True,"不公开":False}
-                if not text in key:
-                    s["last"] = "public"
-                    msg = "非正确格式！请重新输入，如需退出请发送：退出"
-                    await send_msg_reject(matcher,event,msg)
+                name = s["name"]
+                systempromote = s["systempromote"]
+                easycyber_package["system"] = s["systempromote"]
+                easycyber_package["public"] = key[f"{text}"]
+                easycyber_package["creator"] = int(id)
+                s["last"] = True
+                g = json_get(config_in_global(),"admin_group")
+                u = json_get(config_in_global(),"admin_pro")
+                g_k = json_get(config_in_global(),"admin_group_switch")
+                u_k = json_get(config_in_global(),"admin_user_switch")
+                msg_tg = f"新投稿！\n来源于QQ[{id}]\n以下为设定内容\n===========\n昵称:{name}\nsystem:{systempromote}\n\n==========="
+                msg = "投稿成功！，等待审核(问就是权限还没写好)]"
+                if not g and not u:
+                    logger.opt(colors=True).success(f"{g},{u}")
+                    msg ="bot管理者未配置，超级管理员和bot控制台,审核失败！"
+                elif not u and g:
+                    cyber_in_tg(name,easycyber_package)
+                    await bot.call_api("send_group_msg",group_id=g, message=msg_tg)
+                elif not g and u:
+                    cyber_in_tg(name,easycyber_package)
+                    await bot.call_api("send_private_msg",user_id=u, message=msg_tg)
+                elif u_k and g_k:
+                    cyber_in_tg(name,easycyber_package)
+                    await bot.call_api("send_group_msg",group_id=g, message=msg_tg)
+                    await bot.call_api("send_private_msg",user_id=u, message=msg_tg)
+                elif u_k:
+                    cyber_in_tg(name,easycyber_package)
+                    await bot.call_api("send_private_msg",user_id=u, message=msg_tg)
                 else:
-                    name = s["name"]
-                    systempromote = s["systempromote"]
-                    easycyber_package["system"] = s["systempromote"]
-                    easycyber_package["public"] = key[f"{text}"]
-                    easycyber_package["creator"] = int(id)
-                    s["last"] = True
-                    g = json_get(config_in_global(),"admin_group")
-                    u = json_get(config_in_global(),"admin_pro")
-                    g_k = json_get(config_in_global(),"admin_group_switch")
-                    u_k = json_get(config_in_global(),"admin_user_switch")
-                    msg_tg = f"新投稿！\n来源于QQ[{id}]\n以下为设定内容\n===========\n昵称:{name}\nsystem:{systempromote}\n\n==========="
-                    msg = "投稿成功！，等待审核(问就是权限还没写好)]"
-                    if not g and not u:
-                        logger.opt(colors=True).success(f"{g},{u}")
-                        msg ="bot管理者未配置，超级管理员和bot控制台,审核失败！"
-                    elif not u and g:
-                        cyber_in_tg(name,easycyber_package)
-                        await bot.call_api("send_group_msg",group_id=g, message=msg_tg)
-                    elif not g and u:
-                        cyber_in_tg(name,easycyber_package)
-                        await bot.call_api("send_private_msg",user_id=u, message=msg_tg)
-                    elif u_k and g_k:
-                        cyber_in_tg(name,easycyber_package)
-                        await bot.call_api("send_group_msg",group_id=g, message=msg_tg)
-                        await bot.call_api("send_private_msg",user_id=u, message=msg_tg)
-                    elif u_k:
-                        cyber_in_tg(name,easycyber_package)
-                        await bot.call_api("send_private_msg",user_id=u, message=msg_tg)
-                    else:
-                        cyber_in_tg(name,easycyber_package)
-                        await bot.call_api("send_group_msg",group_id=g, message=msg_tg)
-                    await send_msg(matcher,event,msg)
+                    cyber_in_tg(name,easycyber_package)
+                    await bot.call_api("send_group_msg",group_id=g, message=msg_tg)
+                await send_msg(matcher,event,msg)
 
         if s["last"] == "载入":
-            if text == "退出":
-                s["last"] = True
-                msg = "已退出"
-                await send_msg(matcher,event,msg)
-            else:
-                s["last"] = True
-                if isinstance(events, GroupMessageEvent):
-                    groupid = get_groupid(event)
-                    config = config_in_group(groupid)
-                    config_group = json_get(config,groupid)
-                    promte = json_get(cyber_in(False,False),f"{text}")
-                    public = json_get(promte,"public")
-                    if not public:
-                        msg = f"{text}模型拒绝被加载(可能是模型不存在或者模型非公开！)"      
+            s["last"] = True
+            if isinstance(events, GroupMessageEvent):
+                groupid = get_groupid(event)
+                config = config_in_group(groupid)
+                config_group = json_get(config,groupid)
+                promte = json_get(cyber_in(False,False),f"{text}")
+                public = json_get(promte,"public")
+                if not public:
+                    msg = f"{text}模型拒绝被加载(可能是模型不存在或者模型非公开！)"      
+                else:
+                    if config_group["character_in"] == text:
+                        msg = f"{text}模型已加载，请勿重新加载"  
                     else:
-                        if config_group["character_in"] == text:
-                            msg = f"{text}模型已加载，请勿重新加载"  
-                        else:
-                            config_group["character_in"] = f"{text}"
-                            config[f"{groupid}"] = config_group
-                            with open(f'{log_dir}/config/config_group.json','w',encoding='utf-8') as file:
-                                json.dump(config,file)
-                                msg = f"{text}加载成功！" 
-                else:
-                    config_user = config_in_user(id,False)
-                    user = json_get(config_user,f"{id}")
-                    promte = json_get(cyber_in(False,False),f"{text}")
-                    public = json_get(promte,"public")
-                    creator = json_get(promte,"creator")
-                    if creator == id:
-                        if user["character_in"]== text:
-                            msg = f"{text}模型已加载，请勿重新加载"  
-                        else:
-                            user["character_in"] = f"{text}"
-                            config_user[f"{id}"] = user
-                            with open(f'{log_dir}/config/config_user.json','w',encoding='utf-8') as file:
-                                json.dump(config_user,file)
-                                msg = f"{text}加载成功！"
-                    elif not public:
-                        msg = f"{text}模型拒绝被加载(可能是模型不存在或者模型非公开！)"      
+                        config_group["character_in"] = f"{text}"
+                        config[f"{groupid}"] = config_group
+                        with open(f'{log_dir}/config/config_group.json','w',encoding='utf-8') as file:
+                            json.dump(config,file)
+                            msg = f"{text}加载成功！" 
+            else:
+                config_user = config_in_user(id,False)
+                user = json_get(config_user,f"{id}")
+                promte = json_get(cyber_in(False,False),f"{text}")
+                public = json_get(promte,"public")
+                creator = json_get(promte,"creator")
+                if creator == id:
+                    if user["character_in"]== text:
+                        msg = f"{text}模型已加载，请勿重新加载"  
                     else:
-                        if user["character_in"] == text:
-                            msg = f"{text}模型已加载，请勿重新加载"  
-                        else:
-                            user["character_in"] = f"{text}"
-                            config_user[f"{id}"] = user
-                            with open(f'{log_dir}\config\config_user.json','w',encoding='utf-8') as file:
-                                json.dump(config_user,file)
-                                msg = f"{text}加载成功！" 
-                await send_msg(matcher,event,msg)
+                        user["character_in"] = f"{text}"
+                        config_user[f"{id}"] = user
+                        with open(f'{log_dir}/config/config_user.json','w',encoding='utf-8') as file:
+                            json.dump(config_user,file)
+                            msg = f"{text}加载成功！"
+                elif not public:
+                    msg = f"{text}模型拒绝被加载(可能是模型不存在或者模型非公开！)"      
+                else:
+                    if user["character_in"] == text:
+                        msg = f"{text}模型已加载，请勿重新加载"  
+                    else:
+                        user["character_in"] = f"{text}"
+                        config_user[f"{id}"] = user
+                        with open(f'{log_dir}\config\config_user.json','w',encoding='utf-8') as file:
+                            json.dump(config_user,file)
+                            msg = f"{text}加载成功！" 
+            await send_msg(matcher,event,msg)
     # 增加预设
     if text == "投稿":
         s["last"] = "增加"
         msg = "请输入角色昵称"
         await send_msg_reject(matcher,event,msg)
     if text == "载入":
         s["last"] = "载入"
```

### Comparing `nonebot-plugin-hx-yinying-1.3.1/nonebot_plugin_hx_yinying/chat.py` & `nonebot-plugin-hx-yinying-1.3.11/nonebot_plugin_hx_yinying/chat.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -- coding: utf-8 --**
 from nonebot.adapters.onebot.v11 import Bot, GroupMessageEvent ,MessageSegment ,Message,MessageEvent,Event,PrivateMessageEvent
 from html import unescape
-from typing import List
+from typing import List,Set
 import os,httpx, json, time, requests,platform
 from loguru import logger as lg
 from .config import Config
 import operator,nonebot,random
 from nonebot import get_plugin_config, logger, require,get_driver
 from pathlib import Path
 require("nonebot_plugin_localstore")
@@ -136,14 +136,37 @@
         except:
             fails += 1
             logger.warning("网络状况不佳，检查最新版本失败，正在重新尝试")
         else:
             break
     return verision,time
 
+#获取艾特的id
+async def extract_member_at(
+    group_id: int, message: Message, bot: Bot = None
+) -> Set[str]:
+    """提取消息中被艾特人的QQ号
+    参数:
+        message: 消息对象
+    返回:
+        被艾特集合
+    """
+    qq_list = (
+        await bot.get_group_member_list(group_id=group_id) if bot is not None else None
+    )
+    result = {
+        segment.data["qq"]
+        for segment in message
+        if segment.type == "at" and "qq" in segment.data
+    }
+    if "all" in result and qq_list is not None:
+        result.remove("all")
+        result |= {str(member["user_id"]) for member in qq_list}
+    return result
+
 #获取用户id
 def get_id(event) -> int:
     """获取会话id"""
     if isinstance(event, GroupMessageEvent):
             id = f"{event.user_id}"
     else:
         id = f"{event.user_id}"
@@ -356,16 +379,15 @@
             logger.warning("你要为你的行为负责，来自不知名开发者")
             logger.warning(f"报错捕获{e}")
             back = False
     return back
 
 #载入本地投稿的easycyber预设(载入失败会被清空
 def easycyber_in_tg(cybernick,json_1) -> str:
-    dt = time.time()
-    t = int(dt)
+    t = time.time()
     try:
         if os.path.exists(f"{log_dir}/file/easycyber_tg.json"):
             with open(f'{log_dir}/file/easycyber_tg.json','r',encoding='utf-8') as file:
                 json_data = json.load(file)
                 if cybernick in json_data or not json_1 or not cybernick:
                     back = json_data
                 else:
@@ -409,14 +431,16 @@
                 back = global_easycyberfurry
             else:
                 logger.error(f"加载本地投稿easycyberfurry时失败！，请不要随意修改bot插件本地文件。。。。！")
                 logger.warning("你要为你的行为负责，来自不知名开发者")
                 logger.warning(f"报错捕获{e}")
                 create_dir_usr(f"{log_dir}/file")
                 with open(f'{log_dir}/file/easycyber_tg.json','w',encoding='utf-8') as file:
+                    dt = time.time()
+                    t = int(dt)
                     global_easycyberfurry = {}
                     packages_easycyberfurry = json_1
                     packages_easycyberfurry["create_time"] = t
                     packages_easycyberfurry["last_update"] = t
                     packages_easycyberfurry["id"] = 0
                     global_easycyberfurry[f"{cybernick}"] = packages_easycyberfurry
                     json.dump(global_easycyberfurry,file)
@@ -488,16 +512,15 @@
             logger.warning("你要为你的行为负责，来自不知名开发者")
             logger.warning(f"报错捕获{e}")
             back = False
     return back
 
 #载入本地投稿的cyber预设(载入失败会被清空
 def cyber_in_tg(cybernick,json_1) -> str:
-    dt = time.time()
-    t = int(dt)
+    t = time.time()
     try:
         if os.path.exists(f"{log_dir}/file/cyber_tg.json"):
             with open(f'{log_dir}/file/cyber_tg.json','r',encoding='utf-8') as file:
                 json_data = json.load(file)
                 if cybernick in json_data or not json_1 or not cybernick:
                     back = json_data
                 else:
@@ -518,15 +541,15 @@
                 package_easycyberfurry["create_time"] = t
                 package_easycyberfurry["last_update"] = t
                 package_easycyberfurry["id"] = 0
                 global_easycyberfurry[f"{cybernick}"] = package_easycyberfurry
                 json.dump(global_easycyberfurry,file)
                 back = global_easycyberfurry
     except Exception as e:
-            if json_1 == False and cybernick == False:
+            if json_1 == False or cybernick == False:
                 easycyber_package = {}
                 global_easycyberfurry = {}
                 easycyber_package["systempromote"] = "你是一个个的"
                 easycyber_package["xml"] = None
                 easycyber_package["creator"] = 3485462167
                 easycyber_package["id"] = 0
                 global_easycyberfurry["保留查询"] = easycyber_package
```

### Comparing `nonebot-plugin-hx-yinying-1.3.1/nonebot_plugin_hx_yinying/config.py` & `nonebot-plugin-hx-yinying-1.3.11/nonebot_plugin_hx_yinying/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 __author__ = "HuanXin"
-from typing import List, Optional, Union
+from typing import List, Optional, Union, Set
 import nonebot
 from pydantic import BaseModel,AnyHttpUrl,Field
 
 
 class Config(BaseModel):
     # 插件版本号勿动！！！！
-    hx_version: Optional[str] = "1.3.01"
+    hx_version: Optional[str] = "1.3.11"
     # 秩乱v你的appid
     yinying_appid: Optional[str] = None
+    #自定义命令头，默认为hx chat
+    hx_chatcommand: Optional[Set[str]] = ["hx","chat"]
     # 秩乱给你的token
     yinying_token: Optional[str] = None
     # 插件数据文件存储路径，可不填。
     hx_path: Optional[str] = None
     # 图像检查api，爱来自阿里云
     image_check_appid: Optional[str] = None
     image_check_token: Optional[str] = None
```

### Comparing `nonebot-plugin-hx-yinying-1.3.1/nonebot_plugin_hx_yinying/image_check.py` & `nonebot-plugin-hx-yinying-1.3.11/nonebot_plugin_hx_yinying/image_check.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-hx-yinying-1.3.1/nonebot_plugin_hx_yinying/smms.py` & `nonebot-plugin-hx-yinying-1.3.11/nonebot_plugin_hx_yinying/smms.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-hx-yinying-1.3.1/nonebot_plugin_hx_yinying.egg-info/PKG-INFO` & `nonebot-plugin-hx-yinying-1.3.11/nonebot_plugin_hx_yinying.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-hx-yinying
-Version: 1.3.1
+Version: 1.3.11
 Summary: chat with yinying
 Home-page: https://github.com/huanxin996/nonebot_plugin_hx-yinying
 Author: Huan Xin
 Author-email: mc.xiaolang@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -205,24 +205,32 @@
 
 ### smms_password
 - 类型：`str`
 - 默认值：`None`
 - 说明：这里是smms的密码（图床）
 - 重要：非必填（若smm_token为空，则需要填写账号密码）
 
+
+### hx_chatcommand
+- 类型：`list`
+- 默认值：`["hx","chat"]`
+- 说明：这里是聊天自定义命令头
+- 重要：非必填
+
 </details>
 <br>
 
 配置文件示例（默认模板）
 
 ```dotenv
 yinying_appid=你的appid
 yinying_token=你的token(不带bearer)
 hx_path=C:\Users\user\Desktop
 SUPERUSERS=["114514"]
+hx_chatcommand = ["hx","chat"]
 image_check_appid=你的appid
 image_check_token=你的token
 smms_token=你获取到的token
 smms_username=114514
 smms_password=114514
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 1.3.1 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 1.3.11 Summary:
 chat with yinying Home-page: https://github.com/huanxin996/nonebot_plugin_hx-
 yinying Author: Huan Xin Author-email: mc.xiaolang@foxmail.com Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Description-Content-
 Type: text/markdown License-File: LICENSE [![All Contributors](https://
 img.shields.io/badge/all_contributors-2-orange.svg?style=flat-square)]
 (#contributors-) * @Author : huanxin996 * @Date : 2024-4-17 * @LastEditors :
@@ -60,17 +60,19 @@
 è¯´æï¼è¿éæ¯smmsçtokenï¼å¾åºï¼ -
 éè¦ï¼éå¿å¡«ï¼å¯å¨å¡«åsmms_usernameåsmms_passwordï¼åéè¿botçªå£è·åã
 ### smms_username - ç±»åï¼`str` - é»è®¤å¼ï¼`None` -
 è¯´æï¼è¿éæ¯smmsçè´¦å·idï¼å¾åºï¼ -
 éè¦ï¼éå¿å¡«å¿å¡«ï¼è¥smm_tokenä¸ºç©ºï¼åéè¦å¡«åè´¦å·å¯ç ï¼
 ### smms_password - ç±»åï¼`str` - é»è®¤å¼ï¼`None` -
 è¯´æï¼è¿éæ¯smmsçå¯ç ï¼å¾åºï¼ -
-éè¦ï¼éå¿å¡«ï¼è¥smm_tokenä¸ºç©ºï¼åéè¦å¡«åè´¦å·å¯ç ï¼
+éè¦ï¼éå¿å¡«ï¼è¥smm_tokenä¸ºç©ºï¼åéè¦å¡«åè´¦å·å¯ç ï¼ ###
+hx_chatcommand - ç±»åï¼`list` - é»è®¤å¼ï¼`["hx","chat"]` -
+è¯´æï¼è¿éæ¯èå¤©èªå®ä¹å½ä»¤å¤´ - éè¦ï¼éå¿å¡«
 éç½®æä»¶ç¤ºä¾ï¼é»è®¤æ¨¡æ¿ï¼ ```dotenv yinying_appid=ä½ çappid
 yinying_token=ä½ çtoken(ä¸å¸¦bearer) hx_path=C:\Users\user\Desktop
-SUPERUSERS=["114514"] image_check_appid=ä½ çappid
-image_check_token=ä½ çtoken smms_token=ä½ è·åå°çtoken
-smms_username=114514 smms_password=114514 ``` ## æ¬å°åç±»configè¯¦è§£
-ccoonnffiigg__gglloobbaall..jjssoonn å¨åäºå¨åäº
+SUPERUSERS=["114514"] hx_chatcommand = ["hx","chat"]
+image_check_appid=ä½ çappid image_check_token=ä½ çtoken
+smms_token=ä½ è·åå°çtoken smms_username=114514 smms_password=114514 ```
+## æ¬å°åç±»configè¯¦è§£ ccoonnffiigg__gglloobbaall..jjssoonn å¨åäºå¨åäº
 ccoonnffiigg__ggrroouupp..jjssoonn å¨åäºå¨åäº
 ccoonnffiigg__uusseerr..jjssoonn å¨åäºå¨åäº
 ## Contributors â¨
```

### Comparing `nonebot-plugin-hx-yinying-1.3.1/setup.py` & `nonebot-plugin-hx-yinying-1.3.11/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nonebot-plugin-hx-yinying",
-    version="1.3.01",
+    version="1.3.11",
     author="Huan Xin",
     author_email="mc.xiaolang@foxmail.com",
     description="chat with yinying",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/huanxin996/nonebot_plugin_hx-yinying",
     packages=setuptools.find_packages(),
```

