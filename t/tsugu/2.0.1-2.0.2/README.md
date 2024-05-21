# Comparing `tmp/tsugu-2.0.1.tar.gz` & `tmp/tsugu-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsugu-2.0.1.tar", last modified: Tue May 21 13:43:32 2024, max compression
+gzip compressed data, was "tsugu-2.0.2.tar", last modified: Tue May 21 15:17:54 2024, max compression
```

## Comparing `tsugu-2.0.1.tar` & `tsugu-2.0.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:43:32.772018 tsugu-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-21 13:43:22.000000 tsugu-2.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-05-21 13:43:32.772018 tsugu-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-05-21 13:43:22.000000 tsugu-2.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 13:43:32.772018 tsugu-2.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-21 13:43:22.000000 tsugu-2.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:43:32.768018 tsugu-2.0.1/tsugu/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-21 13:43:22.000000 tsugu-2.0.1/tsugu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-05-21 13:43:22.000000 tsugu-2.0.1/tsugu/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:43:32.768018 tsugu-2.0.1/tsugu/src/
--rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-05-21 13:43:22.000000 tsugu-2.0.1/tsugu/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:43:32.768018 tsugu-2.0.1/tsugu/src/bandoristation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 13:43:22.000000 tsugu-2.0.1/tsugu/src/bandoristation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4068 2024-05-21 13:43:22.000000 tsugu-2.0.1/tsugu/src/bandoristation/rooms_forward.py
--rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-05-21 13:43:22.000000 tsugu-2.0.1/tsugu/src/bandoristation/ycm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:43:32.768018 tsugu-2.0.1/tsugu/src/help/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 13:43:22.000000 tsugu-2.0.1/tsugu/src/help/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-05-21 13:43:22.000000 tsugu-2.0.1/tsugu/src/help/help.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:43:32.768018 tsugu-2.0.1/tsugu/src/remote/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 13:43:22.000000 tsugu-2.0.1/tsugu/src/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-21 13:43:22.000000 tsugu-2.0.1/tsugu/src/remote/bind_player.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-21 13:43:22.000000 tsugu-2.0.1/tsugu/src/remote/bind_player_verification_off.py
--rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-05-21 13:43:22.000000 tsugu-2.0.1/tsugu/src/remote/bind_player_verification_on.py
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-21 13:43:22.000000 tsugu-2.0.1/tsugu/src/remote/change_default_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-21 13:43:22.000000 tsugu-2.0.1/tsugu/src/remote/change_server_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-05-21 13:43:22.000000 tsugu-2.0.1/tsugu/src/remote/player_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-21 13:43:22.000000 tsugu-2.0.1/tsugu/src/remote/switch_car_forwarding_off.py
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-21 13:43:22.000000 tsugu-2.0.1/tsugu/src/remote/switch_car_forwarding_on.py
--rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-05-21 13:43:22.000000 tsugu-2.0.1/tsugu/src/remote/unbind_player.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:43:32.772018 tsugu-2.0.1/tsugu/src/universal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 13:43:22.000000 tsugu-2.0.1/tsugu/src/universal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-21 13:43:22.000000 tsugu-2.0.1/tsugu/src/universal/event_stage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-05-21 13:43:22.000000 tsugu-2.0.1/tsugu/src/universal/gacha_simulate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-21 13:43:22.000000 tsugu-2.0.1/tsugu/src/universal/get_card_illustration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-21 13:43:22.000000 tsugu-2.0.1/tsugu/src/universal/lsycx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-05-21 13:43:22.000000 tsugu-2.0.1/tsugu/src/universal/search_card.py
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-21 13:43:22.000000 tsugu-2.0.1/tsugu/src/universal/search_character.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-21 13:43:22.000000 tsugu-2.0.1/tsugu/src/universal/search_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-21 13:43:22.000000 tsugu-2.0.1/tsugu/src/universal/search_gacha.py
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-21 13:43:22.000000 tsugu-2.0.1/tsugu/src/universal/search_player.py
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-05-21 13:43:22.000000 tsugu-2.0.1/tsugu/src/universal/search_song.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-05-21 13:43:22.000000 tsugu-2.0.1/tsugu/src/universal/song_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-05-21 13:43:22.000000 tsugu-2.0.1/tsugu/src/universal/song_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-05-21 13:43:22.000000 tsugu-2.0.1/tsugu/src/universal/ycx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-21 13:43:22.000000 tsugu-2.0.1/tsugu/src/universal/ycx_all.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:43:32.772018 tsugu-2.0.1/tsugu/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     5067 2024-05-21 13:43:22.000000 tsugu-2.0.1/tsugu/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:43:32.768018 tsugu-2.0.1/tsugu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-05-21 13:43:32.000000 tsugu-2.0.1/tsugu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-21 13:43:32.000000 tsugu-2.0.1/tsugu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 13:43:32.000000 tsugu-2.0.1/tsugu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-21 13:43:32.000000 tsugu-2.0.1/tsugu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-21 13:43:32.000000 tsugu-2.0.1/tsugu.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:17:54.257714 tsugu-2.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-21 15:17:45.000000 tsugu-2.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-05-21 15:17:54.257714 tsugu-2.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-05-21 15:17:45.000000 tsugu-2.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 15:17:54.257714 tsugu-2.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-21 15:17:45.000000 tsugu-2.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:17:54.253714 tsugu-2.0.2/tsugu/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-21 15:17:45.000000 tsugu-2.0.2/tsugu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-05-21 15:17:45.000000 tsugu-2.0.2/tsugu/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:17:54.253714 tsugu-2.0.2/tsugu/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-05-21 15:17:45.000000 tsugu-2.0.2/tsugu/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:17:54.253714 tsugu-2.0.2/tsugu/src/bandoristation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 15:17:45.000000 tsugu-2.0.2/tsugu/src/bandoristation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4102 2024-05-21 15:17:45.000000 tsugu-2.0.2/tsugu/src/bandoristation/rooms_forward.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-05-21 15:17:45.000000 tsugu-2.0.2/tsugu/src/bandoristation/ycm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:17:54.253714 tsugu-2.0.2/tsugu/src/help/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 15:17:45.000000 tsugu-2.0.2/tsugu/src/help/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-21 15:17:45.000000 tsugu-2.0.2/tsugu/src/help/help.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:17:54.257714 tsugu-2.0.2/tsugu/src/remote/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 15:17:45.000000 tsugu-2.0.2/tsugu/src/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-05-21 15:17:45.000000 tsugu-2.0.2/tsugu/src/remote/bind_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-05-21 15:17:45.000000 tsugu-2.0.2/tsugu/src/remote/bind_player_verification_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-05-21 15:17:45.000000 tsugu-2.0.2/tsugu/src/remote/bind_player_verification_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-21 15:17:45.000000 tsugu-2.0.2/tsugu/src/remote/change_default_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-21 15:17:45.000000 tsugu-2.0.2/tsugu/src/remote/change_server_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-05-21 15:17:45.000000 tsugu-2.0.2/tsugu/src/remote/player_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-21 15:17:45.000000 tsugu-2.0.2/tsugu/src/remote/switch_car_forwarding_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-05-21 15:17:45.000000 tsugu-2.0.2/tsugu/src/remote/switch_car_forwarding_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-05-21 15:17:45.000000 tsugu-2.0.2/tsugu/src/remote/unbind_player.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:17:54.257714 tsugu-2.0.2/tsugu/src/universal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 15:17:45.000000 tsugu-2.0.2/tsugu/src/universal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-21 15:17:45.000000 tsugu-2.0.2/tsugu/src/universal/event_stage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-21 15:17:45.000000 tsugu-2.0.2/tsugu/src/universal/gacha_simulate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-21 15:17:45.000000 tsugu-2.0.2/tsugu/src/universal/get_card_illustration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-05-21 15:17:45.000000 tsugu-2.0.2/tsugu/src/universal/lsycx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-21 15:17:45.000000 tsugu-2.0.2/tsugu/src/universal/search_card.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-21 15:17:45.000000 tsugu-2.0.2/tsugu/src/universal/search_character.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-21 15:17:45.000000 tsugu-2.0.2/tsugu/src/universal/search_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-21 15:17:45.000000 tsugu-2.0.2/tsugu/src/universal/search_gacha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-21 15:17:45.000000 tsugu-2.0.2/tsugu/src/universal/search_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-21 15:17:45.000000 tsugu-2.0.2/tsugu/src/universal/search_song.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-21 15:17:45.000000 tsugu-2.0.2/tsugu/src/universal/song_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-21 15:17:45.000000 tsugu-2.0.2/tsugu/src/universal/song_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-21 15:17:45.000000 tsugu-2.0.2/tsugu/src/universal/ycx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-21 15:17:45.000000 tsugu-2.0.2/tsugu/src/universal/ycx_all.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:17:54.257714 tsugu-2.0.2/tsugu/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     5067 2024-05-21 15:17:45.000000 tsugu-2.0.2/tsugu/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:17:54.253714 tsugu-2.0.2/tsugu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-05-21 15:17:54.000000 tsugu-2.0.2/tsugu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-21 15:17:54.000000 tsugu-2.0.2/tsugu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 15:17:54.000000 tsugu-2.0.2/tsugu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-21 15:17:54.000000 tsugu-2.0.2/tsugu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-21 15:17:54.000000 tsugu-2.0.2/tsugu.egg-info/top_level.txt
```

### Comparing `tsugu-2.0.1/LICENSE` & `tsugu-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.1/PKG-INFO` & `tsugu-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu
-Version: 2.0.1
+Version: 2.0.2
 Summary: Tsugu Python Frontend
 Home-page: https://github.com/kumoSleeping/ChatTsuguPy
 Author: kumoSleeping
 Author-email: zjr2992@outlook.com
 License: MIT
 Description: 
         <h1 align="center"> Chat Tsugu Py <img src="./logo.jpg" width="30" width="30" height="30" alt="tmrn"/> </h1>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tsugu Version: 2.0.1 Summary: Tsugu Python Frontend
+Metadata-Version: 2.1 Name: tsugu Version: 2.0.2 Summary: Tsugu Python Frontend
 Home-page: https://github.com/kumoSleeping/ChatTsuguPy Author: kumoSleeping
 Author-email: zjr2992@outlook.com License: MIT Description:
                        ************ CChhaatt TTssuugguu PPyy[[ttmmrrnn]] ************
 _â¨ Python ç¼åç [TsuguBanGDreamBot](https://github.com/Yamamoto-2/tsugu-
          bangdream-bot?tab=readme-ov-file) èªç¶è¯­è¨äº¤äºåº â¨_
                           _[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]
 --- ## ð¦ å®è£ ```shell pip install tsugu --upgrade ``` > API powered by
```

### Comparing `tsugu-2.0.1/README.md` & `tsugu-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.1/setup.py` & `tsugu-2.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r') as readme:
     long_description = readme.read()
 
 setup(
     name='tsugu',
-    version='2.0.1',
+    version='2.0.2',
     author='kumoSleeping',
     author_email='zjr2992@outlook.com',
     license="MIT",
     description='Tsugu Python Frontend',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/kumoSleeping/ChatTsuguPy',
```

### Comparing `tsugu-2.0.1/tsugu/handler.py` & `tsugu-2.0.2/tsugu/handler.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.1/tsugu/src/__init__.py` & `tsugu-2.0.2/tsugu/src/__init__.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.1/tsugu/src/bandoristation/rooms_forward.py` & `tsugu-2.0.2/tsugu/src/bandoristation/rooms_forward.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 from ...utils import text_response, User, get_user, get_user_async
 from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager
 import re
 import tsugu_api
 import tsugu_api_async
 
+
 # 虚空注册
-alc = Alconna(["上传车牌"],meta=CommandMeta(description="上传车牌",))
+alc = Alconna(
+    ["上传车牌"],
+    meta=CommandMeta(
+        description="上传车牌",
+       ),
+    )
 
 
 def handler(message: str, user_id: str, platform: str, channel_id: str):
     if message.startswith("上传车牌"):
         message = message[4:].strip()
 
     # 检查car_config['car']中的关键字
```

### Comparing `tsugu-2.0.1/tsugu/src/bandoristation/ycm.py` & `tsugu-2.0.2/tsugu/src/bandoristation/ycm.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 import tsugu_api_async
 from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager
 
 
 alc = Alconna(
         ["ycm", "车来", "有车吗"],
         meta=CommandMeta(
-            compact=True, description="获取车牌",
+            compact=True,
+            description="获取车牌",
         )
     )
 
 
 def handler(message: str, user_id: str, platform: str, channel_id: str):
     res = alc.parse(message)
```

### Comparing `tsugu-2.0.1/tsugu/src/help/help.py` & `tsugu-2.0.2/tsugu/src/help/help.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager, MultiVar, AllParam
 
 
 alc = Alconna(
         ["help"],
         Args["cmd;?#命令", str],
         meta=CommandMeta(
-            compact=True, description="Chat Tsugu Py 帮助",)
+            compact=True,
+            description="Chat Tsugu Py 帮助",)
     )
 
 
 def handler(message: str, user_id: str, platform: str, channel_id: str):
     res = alc.parse(message)
 
     if res.matched:
```

### Comparing `tsugu-2.0.1/tsugu/src/remote/bind_player.py` & `tsugu-2.0.2/tsugu/src/remote/bind_player.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 import tsugu_api_async
 
 
 alc = Alconna(
         ["绑定玩家"],
         Args["args;?", AllParam],
         meta=CommandMeta(
-            compact=True, description="绑定玩家",
+            compact=True,
+            description="绑定玩家",
             usage="只需发送‘绑定玩家’。",
         ),
     )
 
 
 def handler(message: str, user_id: str, platform: str, channel_id: str):
     res = alc.parse(message)
```

### Comparing `tsugu-2.0.1/tsugu/src/remote/bind_player_verification_off.py` & `tsugu-2.0.2/tsugu/src/remote/bind_player_verification_off.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 import tsugu_api_async
 
 
 alc = Alconna(
         ["验证解绑"],
         Args["index#要解绑的绑定编号", int],
         meta=CommandMeta(
-            compact=True, description="验证解绑",
+            compact=True,
+            description="验证解绑",
             usage="验证解绑 记录编号(数字)",
             example="验证解绑 1 : 解绑第一个记录"
         ),
     )
 
 
 def handler(message: str, user_id: str, platform: str, channel_id: str):
```

### Comparing `tsugu-2.0.1/tsugu/src/remote/bind_player_verification_on.py` & `tsugu-2.0.2/tsugu/src/remote/bind_player_verification_on.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 import tsugu_api_async
 
 
 alc = Alconna(
         ["验证绑定"],
         Args["playerID#你的玩家ID(数字)", int]["serverName#服务器名(字母缩写)", _ServerName],
         meta=CommandMeta(
-            compact=True, description="验证绑定",)
+            compact=True,
+            description="验证绑定",)
     )
 
 
 def handler(message: str, user_id: str, platform: str, channel_id: str):
     res = alc.parse(message)
 
     if res.matched:
```

### Comparing `tsugu-2.0.1/tsugu/src/remote/change_default_server.py` & `tsugu-2.0.2/tsugu/src/remote/change_default_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 import tsugu_api_async
 
 
 alc = Alconna(
         ["设置默认服务器", "默认服务器"],
         Args["serverList#使用空格分隔服务器列表。", MultiVar(_ServerName)],
         meta=CommandMeta(
-            compact=True, description="设定信息显示中的默认服务器排序",
+            compact=True,
+            description="设定信息显示中的默认服务器排序",
             example="""设置默认服务器 cn jp : 将国服设置为第一服务器，日服设置为第二服务器。"""
 
         )
     )
 
 
 def handler(message: str, user_id: str, platform: str, channel_id: str):
```

### Comparing `tsugu-2.0.1/tsugu/src/remote/change_server_mode.py` & `tsugu-2.0.2/tsugu/src/remote/change_server_mode.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 import tsugu_api
 from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager, MultiVar
 from tsugu_api_core._typing import _ServerName
 
 
 alc = Alconna(
         ["主服务器", "设置主服务器"],
-    Args["serverName#服务器名", _ServerName],
+        Args["serverName#服务器名", _ServerName],
         meta=CommandMeta(
-            compact=True, description="主服务器",
+            compact=True,
+            description="主服务器",
             usage="将指定的服务器设置为你的主服务器。",
             example="""主服务器 cn : 将国服设置为主服务器。"""
 
         )
     )
```

### Comparing `tsugu-2.0.1/tsugu/src/remote/player_status.py` & `tsugu-2.0.2/tsugu/src/remote/player_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 import tsugu_api_async
 
 
 alc = Alconna(
         ["玩家状态"],
         Args["serverName", _ServerName.__args__, None]["serverIndex", int, None],
         meta=CommandMeta(
-            compact=True, description="查询自己的玩家状态",
+            compact=True,
+            description="查询自己的玩家状态",
             usage='根据关键词或活动ID查询活动信息',
             example='''玩家状态 :返回玩家状态(优先当前服务器下第一条记录)
 玩家状态 1 :返回绑定的第一条记录的状态
 玩家状态 jp :返回绑定的cn服务器的记录的状态'''
         )
     )
```

### Comparing `tsugu-2.0.1/tsugu/src/remote/switch_car_forwarding_off.py` & `tsugu-2.0.2/tsugu/src/remote/switch_car_forwarding_off.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager
 import tsugu_api_async
 
 
 alc = Alconna(
         ["关闭车牌转发", "关闭个人车牌转发"],
         meta=CommandMeta(
-            compact=True, description="关闭车牌转发",)
+            compact=True,
+            description="关闭车牌转发",)
     )
 
 
 def handler(message: str, user_id: str, platform: str, channel_id: str):
     res = alc.parse(message)
 
     if res.matched:
```

### Comparing `tsugu-2.0.1/tsugu/src/remote/switch_car_forwarding_on.py` & `tsugu-2.0.2/tsugu/src/remote/switch_car_forwarding_on.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager
 import tsugu_api_async
 
 
 alc = Alconna(
         ["开启车牌转发", "开启个人车牌转发"],
         meta=CommandMeta(
-            compact=True, description="开启车牌转发",)
+            compact=True,
+            description="开启车牌转发",)
     )
 
 
 def handler(message: str, user_id: str, platform: str, channel_id: str):
     res = alc.parse(message)
 
     if res.matched:
```

### Comparing `tsugu-2.0.1/tsugu/src/remote/unbind_player.py` & `tsugu-2.0.2/tsugu/src/remote/unbind_player.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 import tsugu_api_async
 
 
 alc = Alconna(
         ["解除绑定"],
         Args["index#要解绑的绑定编号", int, None],
         meta=CommandMeta(
-            compact=True, description="解除绑定",
+            compact=True,
+            description="解除绑定",
             usage="验证解绑 记录编号(数字)",
             example="验证解绑 1 : 解绑第一个记录"
         ),
     )
 
 
 def handler(message: str, user_id: str, platform: str, channel_id: str):
```

### Comparing `tsugu-2.0.1/tsugu/src/universal/event_stage.py` & `tsugu-2.0.2/tsugu/src/universal/event_stage.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 
 
 alc = Alconna(
         ["查试炼", '查stage', '查舞台', '查festival', '查5v5'],
         Args["eventId;?#省略活动ID时查询当前活动。", [int]]["meta;?#歌曲meta。", ['-m']],
 
         meta=CommandMeta(
-            compact=True, description="查试炼",
+            compact=True,
+            description="查试炼",
             usage='查询当前服务器当前活动试炼信息。',
             example='''查试炼 157 -m :返回157号活动的试炼信息，包含歌曲meta。
 查试炼 -m :返回当前活动的试炼信息，包含歌曲meta。
 查试炼 :返回当前活动的试炼信息。'''
         )
     )
```

### Comparing `tsugu-2.0.1/tsugu/src/universal/gacha_simulate.py` & `tsugu-2.0.2/tsugu/src/universal/gacha_simulate.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 import tsugu_api_async
 
 
 alc = Alconna(
         ["抽卡模拟", "卡池模拟"],
         Args["times", int, 10]['gacha_id;?#如果没有卡池ID的话，卡池为当前活动的卡池。', int],
         meta=CommandMeta(
-            compact=True, description="抽卡模拟",
-            usage='根据卡片ID查询卡片插画',
+            compact=True,
+            description="抽卡模拟",
+            usage='模拟抽卡',
             example='抽卡模拟 300 922 :模拟抽卡300次，卡池为922号卡池。'
         )
     )
 
 
 def handler(message: str, user_id: str, platform: str, channel_id: str):
     res = alc.parse(message)
```

### Comparing `tsugu-2.0.1/tsugu/src/universal/get_card_illustration.py` & `tsugu-2.0.2/tsugu/src/universal/get_card_illustration.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 import tsugu_api_async
 
 
 alc = Alconna(
         ["查卡面", "查插画"],
         Args["cardId", int],
         meta=CommandMeta(
-            compact=True, description="查卡面",
+            compact=True,
+            description="查卡面",
             usage='根据卡片ID查询卡片插画',
             example='查卡面 1399 :返回1399号卡牌的插画'
         )
     )
 
 
 def handler(message: str, user_id: str, platform: str, channel_id: str):
```

### Comparing `tsugu-2.0.1/tsugu/src/universal/lsycx.py` & `tsugu-2.0.2/tsugu/src/universal/lsycx.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,20 +4,21 @@
 from tsugu_api_core._typing import _ServerName
 import tsugu_api_async
 
 
 alc = Alconna(
         ["lsycx", "历史预测线"], ['/', ''],
         Args['tier', int]['eventId;?#活动ID，省略时查询当前活动。', int]
-            ['serverName#省略服务器名时，默认从你当前的主服务器查询。活动ID不存在时，也可以作为第二个参数。', _ServerName.__args__, None],
+            ['serverName#省略服务器名时，默认从你当前的主服务器查询。', _ServerName.__args__, None],
         meta=CommandMeta(
-            compact=True, description="查询指定档位的历史预测线。",
+            compact=True,
+            description="查询指定档位的历史预测线。",
             usage='查询指定档位的预测线与最近的4期活动类型相同的活动的档线数据。',
-            example='''lsycx 1000 :返回默认服务器当前活动的档线与预测线，与最近的4期活动类型相同的活动的档线数据。
-lsycx 1000 177 jp:返回日服177号活动1000档位档线与最近的4期活动类型相同的活动的档线数据。'''
+            example='''lsycx 1000 
+lsycx 1000 177 jp'''
         )
     )
 
 
 def handler(message: str, user_id: str, platform: str, channel_id: str):
     res = alc.parse(message)
```

### Comparing `tsugu-2.0.1/tsugu/src/universal/search_card.py` & `tsugu-2.0.2/tsugu/src/universal/search_card.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 import tsugu_api_async
 
 
 alc = Alconna(
         ["查卡", "查卡牌"],
         Args["word#请输入卡面ID，角色等查询参数，使用空格隔开", AllParam],
         meta=CommandMeta(
-            compact=True, description="查询卡片信息。",
+            compact=True,
+            description="查询卡片信息。",
             usage='根据关键词或卡牌ID查询卡片信息。',
             example='''查卡 1399 :返回1399号卡牌的信息。
     查卡面 1399 :返回1399号卡牌的插画。
     查卡 红 ars 5x :返回角色 ars 的 5x 卡片的信息。'''
         )
     )
```

### Comparing `tsugu-2.0.1/tsugu/src/universal/search_character.py` & `tsugu-2.0.2/tsugu/src/universal/search_character.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, AllParam
 import tsugu_api_async
 
 alc = Alconna(
         ["查角色"],
         Args["word#角色名，乐队，昵称等查询参数", AllParam],
         meta=CommandMeta(
-            compact=True, description="查询角色信息",
+            compact=True,
+            description="查询角色信息",
             usage='根据关键词或角色ID查询角色信息',
             example='''查角色 10 :返回10号角色的信息。
 查角色 吉他 :返回所有角色模糊搜索标签中包含吉他的角色列表。'''
         )
     )
```

### Comparing `tsugu-2.0.1/tsugu/src/universal/search_event.py` & `tsugu-2.0.2/tsugu/src/universal/search_event.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 import tsugu_api_async
 
 
 alc = Alconna(
         ["查活动"],
         Args["word#请输入活动名，乐队，活动ID等查询参数", AllParam],
         meta=CommandMeta(
-            compact=True, description="查活动",
+            compact=True,
+            description="查活动",
             usage='根据关键词或活动ID查询活动信息',
             example='''查活动 绿 tsugu :返回所有属性加成为pure，且活动加成角色中包括羽泽鸫的活动列表
 查活动 177 :返回177号活动的信息
 查活动 >225 :查询大于225的活动
 查活动 220-225 :查询220到225的活动'''
         )
     )
```

### Comparing `tsugu-2.0.1/tsugu/src/universal/search_gacha.py` & `tsugu-2.0.2/tsugu/src/universal/search_gacha.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 import tsugu_api_async
 
 
 alc = Alconna(
         ["查卡池"],
         Args["gachaId#可以通过查活动、查卡等获取", str],
         meta=CommandMeta(
-            compact=True, description="查卡池",
+            compact=True,
+            description="查卡池",
             usage='根据卡池ID查询卡池信息',
         )
     )
 
 
 def handler(message: str, user_id: str, platform: str, channel_id: str):
     res = alc.parse(message)
```

### Comparing `tsugu-2.0.1/tsugu/src/universal/search_player.py` & `tsugu-2.0.2/tsugu/src/universal/search_player.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 import tsugu_api_async
 
 
 alc = Alconna(
         ["查玩家", "查寻玩家"],
         Args["playerId#你的游戏账号(数字)", int]["serverName;?#省略服务器名时，默认从你当前的主服务器查询。", _ServerName.__args__],
         meta=CommandMeta(
-            compact=True, description="查询玩家信息",
+            compact=True,
+            description="查询玩家信息",
             usage='查询指定ID玩家的信息。查询指定ID玩家的信息。',
             example='查玩家 40474621 jp : 查询日服玩家ID为40474621的玩家信息。\n查玩家 10000000 : 查询你当前默认服务器中，玩家ID为10000000的玩家信息。',
         )
     )
 
 
 def handler(message: str, user_id: str, platform: str, channel_id: str):
```

### Comparing `tsugu-2.0.1/tsugu/src/universal/search_song.py` & `tsugu-2.0.2/tsugu/src/universal/search_song.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 import tsugu_api_async
 
 
 alc = Alconna(
         ["查曲"],
         Args["word#歌曲信息，名称，乐队，难度等。", AllParam],
         meta=CommandMeta(
-            compact=True, description="查曲",
+            compact=True,
+            description="查曲",
             usage='根据关键词或曲目ID查询曲目信息。',
             example='''查曲 1 :返回1号曲的信息
 查曲 ag lv27 :返回所有难度为27的ag曲列表
 查曲 >27 :查询大于27的曲目
 查曲 滑滑蛋 :匹配歌曲 fuwa fuwa time'''
         )
     )
```

### Comparing `tsugu-2.0.1/tsugu/src/universal/song_chart.py` & `tsugu-2.0.2/tsugu/src/universal/song_chart.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 
 difficulty_text_tuple = ('easy', 'ez', 'normal', 'nm', 'hard', 'hd', 'expert', 'ex', 'special', 'sp')
 
 alc = Alconna(
         ["查谱面", "查铺面"],
         Args["songId", int]['difficultyText', difficulty_text_tuple, 'ex'],
         meta=CommandMeta(
-            compact=True, description="查谱面",
+            compact=True,
+            description="查谱面",
             usage='根据曲目ID与难度查询铺面信息。',
             example='''查谱面 1 :返回1号曲的ex难度谱面
 查谱面 128 special :返回128号曲的special难度谱面'''
         )
     )
 def handler(message: str, user_id: str, platform: str, channel_id: str):
     res = alc.parse(message)
```

### Comparing `tsugu-2.0.1/tsugu/src/universal/song_meta.py` & `tsugu-2.0.2/tsugu/src/universal/song_meta.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 import tsugu_api_async
 
 
 alc = Alconna(
         ["查询分数表", '查分数表', '查询分数榜', '查分数榜'],
         Args["serverName;?#省略服务器名时，默认从你当前的主服务器查询。", _ServerName.__args__],
         meta=CommandMeta(
-            compact=True, description="查询分数表",
+            compact=True,
+            description="查询分数表",
             usage='查询指定服务器的歌曲分数表。',
             example='''查询分数表 cn :返回国服的歌曲分数表'''
         )
     )
 
 
 def handler(message: str, user_id: str, platform: str, channel_id: str):
```

### Comparing `tsugu-2.0.1/tsugu/src/universal/ycx.py` & `tsugu-2.0.2/tsugu/src/universal/ycx_all.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,41 @@
-from ...utils import get_user, text_response, User, server_id_2_server_name, server_name_2_server_id
+from ...utils import get_user, text_response, User, server_id_2_server_name, server_name_2_server_id, server_exists
 import tsugu_api
 from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager
 from tsugu_api_core._typing import _ServerName
 import tsugu_api_async
 
 
 alc = Alconna(
-        ["ycx", "预测线"],
-        Args['tier', int]['eventId;?#活动ID，省略时查询当前活动。', int]
+        ["ycxall", "ycx all"],
+        Args['eventId;?#活动ID，省略时查询当前活动。', int]
             ['serverName#省略服务器名时，默认从你当前的主服务器查询。活动ID不存在时，也可以作为第二个参数。', _ServerName.__args__, None],
         meta=CommandMeta(
             compact=True, description="查询指定档位的预测线",
-            usage='查询指定档位的预测线。',
-            example='''ycx 1000 :返回默认服务器当前活动1000档位的档线与预测线。
-ycx 1000 177 jp:返回日服177号活动1000档位的档线与预测线。'''
+            usage='根据关键词或角色ID查询角色信息',
+            example='''ycx 1000 
+ycx 1000 177 jp'''
         )
     )
 
 
 def handler(message: str, user_id: str, platform: str, channel_id: str):
     res = alc.parse(message)
 
     if res.matched:
         user = get_user(user_id, platform)
         server = server_name_2_server_id(res.serverName) if res.serverName else user.server_mode
-        return tsugu_api.ycx(server, res.tier, res.eventId)
+        return tsugu_api.ycx_all(server, res.eventId)
 
     return res
 
 
 async def handler_async(message: str, user_id: str, platform: str, channel_id: str):
     res = alc.parse(message)
 
     if res.matched:
         user = get_user(user_id, platform)
         server = server_name_2_server_id(res.serverName) if res.serverName else user.server_mode
-        return await tsugu_api_async.ycx(server, res.tier, res.eventId)
+        return await tsugu_api_async.ycx_all(server, res.eventId)
 
     return res
 
-
```

### Comparing `tsugu-2.0.1/tsugu/utils/__init__.py` & `tsugu-2.0.2/tsugu/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.1/tsugu.egg-info/PKG-INFO` & `tsugu-2.0.2/tsugu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu
-Version: 2.0.1
+Version: 2.0.2
 Summary: Tsugu Python Frontend
 Home-page: https://github.com/kumoSleeping/ChatTsuguPy
 Author: kumoSleeping
 Author-email: zjr2992@outlook.com
 License: MIT
 Description: 
         <h1 align="center"> Chat Tsugu Py <img src="./logo.jpg" width="30" width="30" height="30" alt="tmrn"/> </h1>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tsugu Version: 2.0.1 Summary: Tsugu Python Frontend
+Metadata-Version: 2.1 Name: tsugu Version: 2.0.2 Summary: Tsugu Python Frontend
 Home-page: https://github.com/kumoSleeping/ChatTsuguPy Author: kumoSleeping
 Author-email: zjr2992@outlook.com License: MIT Description:
                        ************ CChhaatt TTssuugguu PPyy[[ttmmrrnn]] ************
 _â¨ Python ç¼åç [TsuguBanGDreamBot](https://github.com/Yamamoto-2/tsugu-
          bangdream-bot?tab=readme-ov-file) èªç¶è¯­è¨äº¤äºåº â¨_
                           _[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]
 --- ## ð¦ å®è£ ```shell pip install tsugu --upgrade ``` > API powered by
```

### Comparing `tsugu-2.0.1/tsugu.egg-info/SOURCES.txt` & `tsugu-2.0.2/tsugu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

