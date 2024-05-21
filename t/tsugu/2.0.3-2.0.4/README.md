# Comparing `tmp/tsugu-2.0.3.tar.gz` & `tmp/tsugu-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsugu-2.0.3.tar", last modified: Tue May 21 15:32:59 2024, max compression
+gzip compressed data, was "tsugu-2.0.4.tar", last modified: Tue May 21 16:22:52 2024, max compression
```

## Comparing `tsugu-2.0.3.tar` & `tsugu-2.0.4.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:32:59.317789 tsugu-2.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-21 15:32:50.000000 tsugu-2.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-05-21 15:32:59.317789 tsugu-2.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-05-21 15:32:50.000000 tsugu-2.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 15:32:59.317789 tsugu-2.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-21 15:32:50.000000 tsugu-2.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:32:59.313789 tsugu-2.0.3/tsugu/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-21 15:32:50.000000 tsugu-2.0.3/tsugu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-05-21 15:32:50.000000 tsugu-2.0.3/tsugu/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:32:59.313789 tsugu-2.0.3/tsugu/src/
--rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-05-21 15:32:50.000000 tsugu-2.0.3/tsugu/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:32:59.313789 tsugu-2.0.3/tsugu/src/bandoristation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 15:32:50.000000 tsugu-2.0.3/tsugu/src/bandoristation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4102 2024-05-21 15:32:50.000000 tsugu-2.0.3/tsugu/src/bandoristation/rooms_forward.py
--rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-05-21 15:32:50.000000 tsugu-2.0.3/tsugu/src/bandoristation/ycm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:32:59.313789 tsugu-2.0.3/tsugu/src/help/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 15:32:50.000000 tsugu-2.0.3/tsugu/src/help/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-21 15:32:50.000000 tsugu-2.0.3/tsugu/src/help/help.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:32:59.317789 tsugu-2.0.3/tsugu/src/remote/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 15:32:50.000000 tsugu-2.0.3/tsugu/src/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-05-21 15:32:50.000000 tsugu-2.0.3/tsugu/src/remote/bind_player.py
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-05-21 15:32:50.000000 tsugu-2.0.3/tsugu/src/remote/bind_player_verification_off.py
--rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-05-21 15:32:50.000000 tsugu-2.0.3/tsugu/src/remote/bind_player_verification_on.py
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-21 15:32:50.000000 tsugu-2.0.3/tsugu/src/remote/change_default_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-21 15:32:50.000000 tsugu-2.0.3/tsugu/src/remote/change_server_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     5275 2024-05-21 15:32:50.000000 tsugu-2.0.3/tsugu/src/remote/player_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-21 15:32:50.000000 tsugu-2.0.3/tsugu/src/remote/switch_car_forwarding_off.py
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-05-21 15:32:50.000000 tsugu-2.0.3/tsugu/src/remote/switch_car_forwarding_on.py
--rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-05-21 15:32:50.000000 tsugu-2.0.3/tsugu/src/remote/unbind_player.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:32:59.317789 tsugu-2.0.3/tsugu/src/universal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 15:32:50.000000 tsugu-2.0.3/tsugu/src/universal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-21 15:32:50.000000 tsugu-2.0.3/tsugu/src/universal/event_stage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-21 15:32:50.000000 tsugu-2.0.3/tsugu/src/universal/gacha_simulate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-21 15:32:50.000000 tsugu-2.0.3/tsugu/src/universal/get_card_illustration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-05-21 15:32:50.000000 tsugu-2.0.3/tsugu/src/universal/lsycx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-21 15:32:50.000000 tsugu-2.0.3/tsugu/src/universal/search_card.py
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-21 15:32:50.000000 tsugu-2.0.3/tsugu/src/universal/search_character.py
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-21 15:32:50.000000 tsugu-2.0.3/tsugu/src/universal/search_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-21 15:32:50.000000 tsugu-2.0.3/tsugu/src/universal/search_gacha.py
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-21 15:32:50.000000 tsugu-2.0.3/tsugu/src/universal/search_player.py
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-21 15:32:50.000000 tsugu-2.0.3/tsugu/src/universal/search_song.py
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-21 15:32:50.000000 tsugu-2.0.3/tsugu/src/universal/song_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-21 15:32:50.000000 tsugu-2.0.3/tsugu/src/universal/song_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-21 15:32:50.000000 tsugu-2.0.3/tsugu/src/universal/ycx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-05-21 15:32:50.000000 tsugu-2.0.3/tsugu/src/universal/ycx_all.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:32:59.317789 tsugu-2.0.3/tsugu/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     5067 2024-05-21 15:32:50.000000 tsugu-2.0.3/tsugu/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:32:59.313789 tsugu-2.0.3/tsugu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-05-21 15:32:59.000000 tsugu-2.0.3/tsugu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-21 15:32:59.000000 tsugu-2.0.3/tsugu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 15:32:59.000000 tsugu-2.0.3/tsugu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-21 15:32:59.000000 tsugu-2.0.3/tsugu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-21 15:32:59.000000 tsugu-2.0.3/tsugu.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 16:22:52.915636 tsugu-2.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-21 16:22:44.000000 tsugu-2.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-05-21 16:22:52.915636 tsugu-2.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-05-21 16:22:44.000000 tsugu-2.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 16:22:52.915636 tsugu-2.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-21 16:22:44.000000 tsugu-2.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 16:22:52.911636 tsugu-2.0.4/tsugu/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-21 16:22:44.000000 tsugu-2.0.4/tsugu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-05-21 16:22:44.000000 tsugu-2.0.4/tsugu/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 16:22:52.911636 tsugu-2.0.4/tsugu/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-05-21 16:22:44.000000 tsugu-2.0.4/tsugu/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 16:22:52.911636 tsugu-2.0.4/tsugu/src/bandoristation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 16:22:44.000000 tsugu-2.0.4/tsugu/src/bandoristation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4102 2024-05-21 16:22:44.000000 tsugu-2.0.4/tsugu/src/bandoristation/rooms_forward.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-05-21 16:22:44.000000 tsugu-2.0.4/tsugu/src/bandoristation/ycm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 16:22:52.911636 tsugu-2.0.4/tsugu/src/help/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 16:22:44.000000 tsugu-2.0.4/tsugu/src/help/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-21 16:22:44.000000 tsugu-2.0.4/tsugu/src/help/help.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 16:22:52.915636 tsugu-2.0.4/tsugu/src/remote/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 16:22:44.000000 tsugu-2.0.4/tsugu/src/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-05-21 16:22:44.000000 tsugu-2.0.4/tsugu/src/remote/bind_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-05-21 16:22:44.000000 tsugu-2.0.4/tsugu/src/remote/bind_player_verification_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-05-21 16:22:44.000000 tsugu-2.0.4/tsugu/src/remote/bind_player_verification_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-21 16:22:44.000000 tsugu-2.0.4/tsugu/src/remote/change_default_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-21 16:22:44.000000 tsugu-2.0.4/tsugu/src/remote/change_server_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5275 2024-05-21 16:22:44.000000 tsugu-2.0.4/tsugu/src/remote/player_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-21 16:22:44.000000 tsugu-2.0.4/tsugu/src/remote/switch_car_forwarding_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-05-21 16:22:44.000000 tsugu-2.0.4/tsugu/src/remote/switch_car_forwarding_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-05-21 16:22:44.000000 tsugu-2.0.4/tsugu/src/remote/unbind_player.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 16:22:52.915636 tsugu-2.0.4/tsugu/src/universal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 16:22:44.000000 tsugu-2.0.4/tsugu/src/universal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-21 16:22:44.000000 tsugu-2.0.4/tsugu/src/universal/event_stage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-21 16:22:44.000000 tsugu-2.0.4/tsugu/src/universal/gacha_simulate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-21 16:22:44.000000 tsugu-2.0.4/tsugu/src/universal/get_card_illustration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-05-21 16:22:44.000000 tsugu-2.0.4/tsugu/src/universal/lsycx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-21 16:22:44.000000 tsugu-2.0.4/tsugu/src/universal/search_card.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-21 16:22:44.000000 tsugu-2.0.4/tsugu/src/universal/search_character.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-21 16:22:44.000000 tsugu-2.0.4/tsugu/src/universal/search_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-21 16:22:44.000000 tsugu-2.0.4/tsugu/src/universal/search_gacha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-21 16:22:44.000000 tsugu-2.0.4/tsugu/src/universal/search_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-21 16:22:44.000000 tsugu-2.0.4/tsugu/src/universal/search_song.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-21 16:22:44.000000 tsugu-2.0.4/tsugu/src/universal/song_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-21 16:22:44.000000 tsugu-2.0.4/tsugu/src/universal/song_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-21 16:22:44.000000 tsugu-2.0.4/tsugu/src/universal/ycx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-05-21 16:22:44.000000 tsugu-2.0.4/tsugu/src/universal/ycx_all.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 16:22:52.915636 tsugu-2.0.4/tsugu/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     5067 2024-05-21 16:22:44.000000 tsugu-2.0.4/tsugu/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 16:22:52.911636 tsugu-2.0.4/tsugu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-05-21 16:22:52.000000 tsugu-2.0.4/tsugu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-21 16:22:52.000000 tsugu-2.0.4/tsugu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 16:22:52.000000 tsugu-2.0.4/tsugu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-21 16:22:52.000000 tsugu-2.0.4/tsugu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-21 16:22:52.000000 tsugu-2.0.4/tsugu.egg-info/top_level.txt
```

### Comparing `tsugu-2.0.3/LICENSE` & `tsugu-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.3/PKG-INFO` & `tsugu-2.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu
-Version: 2.0.3
+Version: 2.0.4
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
-Metadata-Version: 2.1 Name: tsugu Version: 2.0.3 Summary: Tsugu Python Frontend
+Metadata-Version: 2.1 Name: tsugu Version: 2.0.4 Summary: Tsugu Python Frontend
 Home-page: https://github.com/kumoSleeping/ChatTsuguPy Author: kumoSleeping
 Author-email: zjr2992@outlook.com License: MIT Description:
                        ************ CChhaatt TTssuugguu PPyy[[ttmmrrnn]] ************
 _â¨ Python ç¼åç [TsuguBanGDreamBot](https://github.com/Yamamoto-2/tsugu-
          bangdream-bot?tab=readme-ov-file) èªç¶è¯­è¨äº¤äºåº â¨_
                           _[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]
 --- ## ð¦ å®è£ ```shell pip install tsugu --upgrade ``` > API powered by
```

### Comparing `tsugu-2.0.3/README.md` & `tsugu-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.3/setup.py` & `tsugu-2.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r') as readme:
     long_description = readme.read()
 
 setup(
     name='tsugu',
-    version='2.0.3',
+    version='2.0.4',
     author='kumoSleeping',
     author_email='zjr2992@outlook.com',
     license="MIT",
     description='Tsugu Python Frontend',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/kumoSleeping/ChatTsuguPy',
```

### Comparing `tsugu-2.0.3/tsugu/handler.py` & `tsugu-2.0.4/tsugu/handler.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.3/tsugu/src/__init__.py` & `tsugu-2.0.4/tsugu/src/__init__.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.3/tsugu/src/bandoristation/rooms_forward.py` & `tsugu-2.0.4/tsugu/src/bandoristation/rooms_forward.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.3/tsugu/src/bandoristation/ycm.py` & `tsugu-2.0.4/tsugu/src/bandoristation/ycm.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.3/tsugu/src/help/help.py` & `tsugu-2.0.4/tsugu/src/help/help.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.3/tsugu/src/remote/bind_player.py` & `tsugu-2.0.4/tsugu/src/remote/bind_player.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,16 @@
 
 
 def handler(message: str, user_id: str, platform: str, channel_id: str):
     res = alc.parse(message)
 
     if res.matched:
         user = get_user(user_id, platform)
-        r = tsugu_api.bind_player_request(platform, user.user_id, user.server_mode, False)
+        r = tsugu_api.bind_player_request(platform, user_id, user.server_mode, True)
+        print(r)
         if r.get('status') != 'success':
             return text_response(r.get('data'))
         return text_response(
             f'''正在绑定账号，请将 评论(个性签名) 或者 当前使用的 乐队编队名称改为\n{r.get('data')['verifyCode']}\n稍等片刻等待同步后，发送\n验证绑定 你的玩家ID(数字) 服务器名(字母缩写)\n例如：验证绑定 114****514 cn''')
 
     return res
```

### Comparing `tsugu-2.0.3/tsugu/src/remote/bind_player_verification_off.py` & `tsugu-2.0.4/tsugu/src/remote/bind_player_verification_off.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.3/tsugu/src/remote/bind_player_verification_on.py` & `tsugu-2.0.4/tsugu/src/remote/bind_player_verification_on.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.3/tsugu/src/remote/change_default_server.py` & `tsugu-2.0.4/tsugu/src/remote/change_default_server.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.3/tsugu/src/remote/change_server_mode.py` & `tsugu-2.0.4/tsugu/src/remote/change_server_mode.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.3/tsugu/src/remote/player_status.py` & `tsugu-2.0.4/tsugu/src/remote/player_status.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.3/tsugu/src/remote/switch_car_forwarding_off.py` & `tsugu-2.0.4/tsugu/src/remote/switch_car_forwarding_off.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.3/tsugu/src/remote/switch_car_forwarding_on.py` & `tsugu-2.0.4/tsugu/src/remote/switch_car_forwarding_on.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.3/tsugu/src/remote/unbind_player.py` & `tsugu-2.0.4/tsugu/src/remote/unbind_player.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.3/tsugu/src/universal/event_stage.py` & `tsugu-2.0.4/tsugu/src/universal/event_stage.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.3/tsugu/src/universal/gacha_simulate.py` & `tsugu-2.0.4/tsugu/src/universal/gacha_simulate.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.3/tsugu/src/universal/get_card_illustration.py` & `tsugu-2.0.4/tsugu/src/universal/get_card_illustration.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.3/tsugu/src/universal/lsycx.py` & `tsugu-2.0.4/tsugu/src/universal/lsycx.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.3/tsugu/src/universal/search_card.py` & `tsugu-2.0.4/tsugu/src/universal/search_card.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.3/tsugu/src/universal/search_character.py` & `tsugu-2.0.4/tsugu/src/universal/search_character.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.3/tsugu/src/universal/search_event.py` & `tsugu-2.0.4/tsugu/src/universal/search_event.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.3/tsugu/src/universal/search_gacha.py` & `tsugu-2.0.4/tsugu/src/universal/search_gacha.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.3/tsugu/src/universal/search_player.py` & `tsugu-2.0.4/tsugu/src/universal/search_player.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.3/tsugu/src/universal/search_song.py` & `tsugu-2.0.4/tsugu/src/universal/search_song.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.3/tsugu/src/universal/song_chart.py` & `tsugu-2.0.4/tsugu/src/universal/song_chart.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.3/tsugu/src/universal/song_meta.py` & `tsugu-2.0.4/tsugu/src/universal/song_meta.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.3/tsugu/src/universal/ycx.py` & `tsugu-2.0.4/tsugu/src/universal/ycx.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.3/tsugu/src/universal/ycx_all.py` & `tsugu-2.0.4/tsugu/src/universal/ycx_all.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.3/tsugu/utils/__init__.py` & `tsugu-2.0.4/tsugu/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.3/tsugu.egg-info/PKG-INFO` & `tsugu-2.0.4/tsugu.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu
-Version: 2.0.3
+Version: 2.0.4
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
-Metadata-Version: 2.1 Name: tsugu Version: 2.0.3 Summary: Tsugu Python Frontend
+Metadata-Version: 2.1 Name: tsugu Version: 2.0.4 Summary: Tsugu Python Frontend
 Home-page: https://github.com/kumoSleeping/ChatTsuguPy Author: kumoSleeping
 Author-email: zjr2992@outlook.com License: MIT Description:
                        ************ CChhaatt TTssuugguu PPyy[[ttmmrrnn]] ************
 _â¨ Python ç¼åç [TsuguBanGDreamBot](https://github.com/Yamamoto-2/tsugu-
          bangdream-bot?tab=readme-ov-file) èªç¶è¯­è¨äº¤äºåº â¨_
                           _[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]
 --- ## ð¦ å®è£ ```shell pip install tsugu --upgrade ``` > API powered by
```

### Comparing `tsugu-2.0.3/tsugu.egg-info/SOURCES.txt` & `tsugu-2.0.4/tsugu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

