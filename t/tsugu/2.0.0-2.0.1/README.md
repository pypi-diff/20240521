# Comparing `tmp/tsugu-2.0.0.tar.gz` & `tmp/tsugu-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsugu-2.0.0.tar", last modified: Tue May 21 12:25:15 2024, max compression
+gzip compressed data, was "tsugu-2.0.1.tar", last modified: Tue May 21 13:43:32 2024, max compression
```

## Comparing `tsugu-2.0.0.tar` & `tsugu-2.0.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:25:15.090217 tsugu-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-21 12:25:02.000000 tsugu-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-05-21 12:25:15.090217 tsugu-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-05-21 12:25:02.000000 tsugu-2.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 12:25:15.090217 tsugu-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-21 12:25:02.000000 tsugu-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:25:15.086217 tsugu-2.0.0/tsugu/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-21 12:25:02.000000 tsugu-2.0.0/tsugu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-05-21 12:25:02.000000 tsugu-2.0.0/tsugu/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:25:15.086217 tsugu-2.0.0/tsugu/src/
--rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-05-21 12:25:02.000000 tsugu-2.0.0/tsugu/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:25:15.086217 tsugu-2.0.0/tsugu/src/bandoristation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 12:25:02.000000 tsugu-2.0.0/tsugu/src/bandoristation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4068 2024-05-21 12:25:02.000000 tsugu-2.0.0/tsugu/src/bandoristation/rooms_forward.py
--rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-05-21 12:25:02.000000 tsugu-2.0.0/tsugu/src/bandoristation/ycm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:25:15.086217 tsugu-2.0.0/tsugu/src/help/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 12:25:02.000000 tsugu-2.0.0/tsugu/src/help/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-05-21 12:25:02.000000 tsugu-2.0.0/tsugu/src/help/help.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:25:15.090217 tsugu-2.0.0/tsugu/src/remote/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 12:25:02.000000 tsugu-2.0.0/tsugu/src/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-21 12:25:02.000000 tsugu-2.0.0/tsugu/src/remote/bind_player.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-21 12:25:02.000000 tsugu-2.0.0/tsugu/src/remote/bind_player_verification_off.py
--rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-05-21 12:25:02.000000 tsugu-2.0.0/tsugu/src/remote/bind_player_verification_on.py
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-21 12:25:02.000000 tsugu-2.0.0/tsugu/src/remote/change_default_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-21 12:25:02.000000 tsugu-2.0.0/tsugu/src/remote/change_server_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     5267 2024-05-21 12:25:02.000000 tsugu-2.0.0/tsugu/src/remote/player_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-21 12:25:02.000000 tsugu-2.0.0/tsugu/src/remote/switch_car_forwarding_off.py
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-21 12:25:02.000000 tsugu-2.0.0/tsugu/src/remote/switch_car_forwarding_on.py
--rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-05-21 12:25:02.000000 tsugu-2.0.0/tsugu/src/remote/unbind_player.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:25:15.090217 tsugu-2.0.0/tsugu/src/universal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 12:25:02.000000 tsugu-2.0.0/tsugu/src/universal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-21 12:25:02.000000 tsugu-2.0.0/tsugu/src/universal/event_stage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-05-21 12:25:02.000000 tsugu-2.0.0/tsugu/src/universal/gacha_simulate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-21 12:25:02.000000 tsugu-2.0.0/tsugu/src/universal/get_card_illustration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-21 12:25:02.000000 tsugu-2.0.0/tsugu/src/universal/lsycx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-05-21 12:25:02.000000 tsugu-2.0.0/tsugu/src/universal/search_card.py
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-21 12:25:02.000000 tsugu-2.0.0/tsugu/src/universal/search_character.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-21 12:25:02.000000 tsugu-2.0.0/tsugu/src/universal/search_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-21 12:25:02.000000 tsugu-2.0.0/tsugu/src/universal/search_gacha.py
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-21 12:25:02.000000 tsugu-2.0.0/tsugu/src/universal/search_player.py
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-05-21 12:25:02.000000 tsugu-2.0.0/tsugu/src/universal/search_song.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-05-21 12:25:02.000000 tsugu-2.0.0/tsugu/src/universal/song_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-05-21 12:25:02.000000 tsugu-2.0.0/tsugu/src/universal/song_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-05-21 12:25:02.000000 tsugu-2.0.0/tsugu/src/universal/ycx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-21 12:25:02.000000 tsugu-2.0.0/tsugu/src/universal/ycx_all.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:25:15.090217 tsugu-2.0.0/tsugu/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     5067 2024-05-21 12:25:02.000000 tsugu-2.0.0/tsugu/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:25:15.086217 tsugu-2.0.0/tsugu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-05-21 12:25:14.000000 tsugu-2.0.0/tsugu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-21 12:25:14.000000 tsugu-2.0.0/tsugu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 12:25:14.000000 tsugu-2.0.0/tsugu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-21 12:25:14.000000 tsugu-2.0.0/tsugu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-21 12:25:14.000000 tsugu-2.0.0/tsugu.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:43:32.772018 tsugu-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-21 13:43:22.000000 tsugu-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-05-21 13:43:32.772018 tsugu-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-05-21 13:43:22.000000 tsugu-2.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 13:43:32.772018 tsugu-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-21 13:43:22.000000 tsugu-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:43:32.768018 tsugu-2.0.1/tsugu/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-21 13:43:22.000000 tsugu-2.0.1/tsugu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-05-21 13:43:22.000000 tsugu-2.0.1/tsugu/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:43:32.768018 tsugu-2.0.1/tsugu/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-05-21 13:43:22.000000 tsugu-2.0.1/tsugu/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:43:32.768018 tsugu-2.0.1/tsugu/src/bandoristation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 13:43:22.000000 tsugu-2.0.1/tsugu/src/bandoristation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4068 2024-05-21 13:43:22.000000 tsugu-2.0.1/tsugu/src/bandoristation/rooms_forward.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-05-21 13:43:22.000000 tsugu-2.0.1/tsugu/src/bandoristation/ycm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:43:32.768018 tsugu-2.0.1/tsugu/src/help/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 13:43:22.000000 tsugu-2.0.1/tsugu/src/help/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-05-21 13:43:22.000000 tsugu-2.0.1/tsugu/src/help/help.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:43:32.768018 tsugu-2.0.1/tsugu/src/remote/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 13:43:22.000000 tsugu-2.0.1/tsugu/src/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-21 13:43:22.000000 tsugu-2.0.1/tsugu/src/remote/bind_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-21 13:43:22.000000 tsugu-2.0.1/tsugu/src/remote/bind_player_verification_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-05-21 13:43:22.000000 tsugu-2.0.1/tsugu/src/remote/bind_player_verification_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-21 13:43:22.000000 tsugu-2.0.1/tsugu/src/remote/change_default_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-21 13:43:22.000000 tsugu-2.0.1/tsugu/src/remote/change_server_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-05-21 13:43:22.000000 tsugu-2.0.1/tsugu/src/remote/player_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-21 13:43:22.000000 tsugu-2.0.1/tsugu/src/remote/switch_car_forwarding_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-21 13:43:22.000000 tsugu-2.0.1/tsugu/src/remote/switch_car_forwarding_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-05-21 13:43:22.000000 tsugu-2.0.1/tsugu/src/remote/unbind_player.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:43:32.772018 tsugu-2.0.1/tsugu/src/universal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 13:43:22.000000 tsugu-2.0.1/tsugu/src/universal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-21 13:43:22.000000 tsugu-2.0.1/tsugu/src/universal/event_stage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-05-21 13:43:22.000000 tsugu-2.0.1/tsugu/src/universal/gacha_simulate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-21 13:43:22.000000 tsugu-2.0.1/tsugu/src/universal/get_card_illustration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-21 13:43:22.000000 tsugu-2.0.1/tsugu/src/universal/lsycx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-05-21 13:43:22.000000 tsugu-2.0.1/tsugu/src/universal/search_card.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-21 13:43:22.000000 tsugu-2.0.1/tsugu/src/universal/search_character.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-21 13:43:22.000000 tsugu-2.0.1/tsugu/src/universal/search_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-21 13:43:22.000000 tsugu-2.0.1/tsugu/src/universal/search_gacha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-21 13:43:22.000000 tsugu-2.0.1/tsugu/src/universal/search_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-05-21 13:43:22.000000 tsugu-2.0.1/tsugu/src/universal/search_song.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-05-21 13:43:22.000000 tsugu-2.0.1/tsugu/src/universal/song_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-05-21 13:43:22.000000 tsugu-2.0.1/tsugu/src/universal/song_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-05-21 13:43:22.000000 tsugu-2.0.1/tsugu/src/universal/ycx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-21 13:43:22.000000 tsugu-2.0.1/tsugu/src/universal/ycx_all.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:43:32.772018 tsugu-2.0.1/tsugu/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     5067 2024-05-21 13:43:22.000000 tsugu-2.0.1/tsugu/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:43:32.768018 tsugu-2.0.1/tsugu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-05-21 13:43:32.000000 tsugu-2.0.1/tsugu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-21 13:43:32.000000 tsugu-2.0.1/tsugu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 13:43:32.000000 tsugu-2.0.1/tsugu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-21 13:43:32.000000 tsugu-2.0.1/tsugu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-21 13:43:32.000000 tsugu-2.0.1/tsugu.egg-info/top_level.txt
```

### Comparing `tsugu-2.0.0/LICENSE` & `tsugu-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.0/PKG-INFO` & `tsugu-2.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu
-Version: 2.0.0
+Version: 2.0.1
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
-Metadata-Version: 2.1 Name: tsugu Version: 2.0.0 Summary: Tsugu Python Frontend
+Metadata-Version: 2.1 Name: tsugu Version: 2.0.1 Summary: Tsugu Python Frontend
 Home-page: https://github.com/kumoSleeping/ChatTsuguPy Author: kumoSleeping
 Author-email: zjr2992@outlook.com License: MIT Description:
                        ************ CChhaatt TTssuugguu PPyy[[ttmmrrnn]] ************
 _â¨ Python ç¼åç [TsuguBanGDreamBot](https://github.com/Yamamoto-2/tsugu-
          bangdream-bot?tab=readme-ov-file) èªç¶è¯­è¨äº¤äºåº â¨_
                           _[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]
 --- ## ð¦ å®è£ ```shell pip install tsugu --upgrade ``` > API powered by
```

### Comparing `tsugu-2.0.0/README.md` & `tsugu-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.0/setup.py` & `tsugu-2.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r') as readme:
     long_description = readme.read()
 
 setup(
     name='tsugu',
-    version='2.0.0',
+    version='2.0.1',
     author='kumoSleeping',
     author_email='zjr2992@outlook.com',
     license="MIT",
     description='Tsugu Python Frontend',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/kumoSleeping/ChatTsuguPy',
```

### Comparing `tsugu-2.0.0/tsugu/handler.py` & `tsugu-2.0.1/tsugu/handler.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.0/tsugu/src/__init__.py` & `tsugu-2.0.1/tsugu/src/__init__.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.0/tsugu/src/bandoristation/rooms_forward.py` & `tsugu-2.0.1/tsugu/src/bandoristation/rooms_forward.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.0/tsugu/src/bandoristation/ycm.py` & `tsugu-2.0.1/tsugu/src/bandoristation/ycm.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.0/tsugu/src/help/help.py` & `tsugu-2.0.1/tsugu/src/help/help.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.0/tsugu/src/remote/bind_player.py` & `tsugu-2.0.1/tsugu/src/remote/bind_player.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.0/tsugu/src/remote/bind_player_verification_off.py` & `tsugu-2.0.1/tsugu/src/remote/bind_player_verification_off.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.0/tsugu/src/remote/bind_player_verification_on.py` & `tsugu-2.0.1/tsugu/src/remote/bind_player_verification_on.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.0/tsugu/src/remote/change_default_server.py` & `tsugu-2.0.1/tsugu/src/remote/change_default_server.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.0/tsugu/src/remote/change_server_mode.py` & `tsugu-2.0.1/tsugu/src/remote/change_server_mode.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.0/tsugu/src/remote/player_status.py` & `tsugu-2.0.1/tsugu/src/remote/player_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,20 +25,20 @@
         response = tsugu_api.search_player(int(player_id), server)
         return response + text_response(additional_text)
 
     def _case_default(user: User):
         # 优先当前服务器
         for game_id in user.game_ids:
             if game_id.get("server") == user.server_mode:
-                text = f'已查找默认服务器 {server_id_2_server_name(user.server_mode)} 的记录。'
+                text = f' 已查找默认服务器 {server_id_2_server_name(user.server_mode)} 的记录。'
                 return _utils_search_player_by_game_id(game_id, text)
         # 兜底逻辑：使用第一个记录
         if user.game_ids:
             game_id = user.game_ids[0]
-            text = f'已查找第一个记录。'
+            text = f' 已查找第一个记录。'
             return _utils_search_player_by_game_id(game_id, text)
         return text_response('未绑定任何记录，可以使用 绑定玩家 进行绑定')
 
     def _case_server(user: User, server_name: str):
         server_id = server_name_2_server_id(server_name)
         # 服务器不存在
         if not server_exists(server_id):
@@ -76,20 +76,20 @@
         response = await tsugu_api_async.search_player(int(player_id), server)
         return response + text_response(additional_text)
 
     async def _case_default(user: User):
         # 优先当前服务器
         for game_id in user.game_ids:
             if game_id.get("server") == user.server_mode:
-                text = f'已查找默认服务器 {server_id_2_server_name(user.server_mode)} 的记录。'
+                text = f' 已查找默认服务器 {server_id_2_server_name(user.server_mode)} 的记录。'
                 return await _utils_search_player_by_game_id(game_id, text)
         # 兜底逻辑：使用第一个记录
         if user.game_ids:
             game_id = user.game_ids[0]
-            text = f'已查找第一个记录。'
+            text = f' 已查找第一个记录。'
             return await _utils_search_player_by_game_id(game_id, text)
         return text_response('未绑定任何记录，可以使用 绑定玩家 进行绑定')
 
     async def _case_server(user: User, server_name: str):
         server_id = server_name_2_server_id(server_name)
         # 服务器不存在
         if not server_exists(server_id):
```

### Comparing `tsugu-2.0.0/tsugu/src/remote/switch_car_forwarding_off.py` & `tsugu-2.0.1/tsugu/src/remote/switch_car_forwarding_off.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.0/tsugu/src/remote/switch_car_forwarding_on.py` & `tsugu-2.0.1/tsugu/src/remote/switch_car_forwarding_on.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.0/tsugu/src/remote/unbind_player.py` & `tsugu-2.0.1/tsugu/src/remote/unbind_player.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.0/tsugu/src/universal/event_stage.py` & `tsugu-2.0.1/tsugu/src/universal/event_stage.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.0/tsugu/src/universal/gacha_simulate.py` & `tsugu-2.0.1/tsugu/src/universal/gacha_simulate.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.0/tsugu/src/universal/get_card_illustration.py` & `tsugu-2.0.1/tsugu/src/universal/get_card_illustration.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.0/tsugu/src/universal/lsycx.py` & `tsugu-2.0.1/tsugu/src/universal/lsycx.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.0/tsugu/src/universal/search_card.py` & `tsugu-2.0.1/tsugu/src/universal/search_card.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.0/tsugu/src/universal/search_character.py` & `tsugu-2.0.1/tsugu/src/universal/search_character.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.0/tsugu/src/universal/search_event.py` & `tsugu-2.0.1/tsugu/src/universal/search_event.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.0/tsugu/src/universal/search_gacha.py` & `tsugu-2.0.1/tsugu/src/universal/search_gacha.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.0/tsugu/src/universal/search_player.py` & `tsugu-2.0.1/tsugu/src/universal/search_player.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.0/tsugu/src/universal/search_song.py` & `tsugu-2.0.1/tsugu/src/universal/search_song.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.0/tsugu/src/universal/song_chart.py` & `tsugu-2.0.1/tsugu/src/universal/song_chart.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.0/tsugu/src/universal/song_meta.py` & `tsugu-2.0.1/tsugu/src/universal/song_meta.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.0/tsugu/src/universal/ycx.py` & `tsugu-2.0.1/tsugu/src/universal/ycx.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.0/tsugu/src/universal/ycx_all.py` & `tsugu-2.0.1/tsugu/src/universal/ycx_all.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.0/tsugu/utils/__init__.py` & `tsugu-2.0.1/tsugu/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.0/tsugu.egg-info/PKG-INFO` & `tsugu-2.0.1/tsugu.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu
-Version: 2.0.0
+Version: 2.0.1
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
-Metadata-Version: 2.1 Name: tsugu Version: 2.0.0 Summary: Tsugu Python Frontend
+Metadata-Version: 2.1 Name: tsugu Version: 2.0.1 Summary: Tsugu Python Frontend
 Home-page: https://github.com/kumoSleeping/ChatTsuguPy Author: kumoSleeping
 Author-email: zjr2992@outlook.com License: MIT Description:
                        ************ CChhaatt TTssuugguu PPyy[[ttmmrrnn]] ************
 _â¨ Python ç¼åç [TsuguBanGDreamBot](https://github.com/Yamamoto-2/tsugu-
          bangdream-bot?tab=readme-ov-file) èªç¶è¯­è¨äº¤äºåº â¨_
                           _[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]
 --- ## ð¦ å®è£ ```shell pip install tsugu --upgrade ``` > API powered by
```

### Comparing `tsugu-2.0.0/tsugu.egg-info/SOURCES.txt` & `tsugu-2.0.1/tsugu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

