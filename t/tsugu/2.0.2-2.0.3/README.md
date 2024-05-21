# Comparing `tmp/tsugu-2.0.2.tar.gz` & `tmp/tsugu-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsugu-2.0.2.tar", last modified: Tue May 21 15:17:54 2024, max compression
+gzip compressed data, was "tsugu-2.0.3.tar", last modified: Tue May 21 15:32:59 2024, max compression
```

## Comparing `tsugu-2.0.2.tar` & `tsugu-2.0.3.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:17:54.257714 tsugu-2.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-21 15:17:45.000000 tsugu-2.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-05-21 15:17:54.257714 tsugu-2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-05-21 15:17:45.000000 tsugu-2.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 15:17:54.257714 tsugu-2.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-21 15:17:45.000000 tsugu-2.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:17:54.253714 tsugu-2.0.2/tsugu/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-21 15:17:45.000000 tsugu-2.0.2/tsugu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-05-21 15:17:45.000000 tsugu-2.0.2/tsugu/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:17:54.253714 tsugu-2.0.2/tsugu/src/
--rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-05-21 15:17:45.000000 tsugu-2.0.2/tsugu/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:17:54.253714 tsugu-2.0.2/tsugu/src/bandoristation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 15:17:45.000000 tsugu-2.0.2/tsugu/src/bandoristation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4102 2024-05-21 15:17:45.000000 tsugu-2.0.2/tsugu/src/bandoristation/rooms_forward.py
--rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-05-21 15:17:45.000000 tsugu-2.0.2/tsugu/src/bandoristation/ycm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:17:54.253714 tsugu-2.0.2/tsugu/src/help/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 15:17:45.000000 tsugu-2.0.2/tsugu/src/help/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-21 15:17:45.000000 tsugu-2.0.2/tsugu/src/help/help.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:17:54.257714 tsugu-2.0.2/tsugu/src/remote/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 15:17:45.000000 tsugu-2.0.2/tsugu/src/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-05-21 15:17:45.000000 tsugu-2.0.2/tsugu/src/remote/bind_player.py
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-05-21 15:17:45.000000 tsugu-2.0.2/tsugu/src/remote/bind_player_verification_off.py
--rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-05-21 15:17:45.000000 tsugu-2.0.2/tsugu/src/remote/bind_player_verification_on.py
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-21 15:17:45.000000 tsugu-2.0.2/tsugu/src/remote/change_default_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-21 15:17:45.000000 tsugu-2.0.2/tsugu/src/remote/change_server_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-05-21 15:17:45.000000 tsugu-2.0.2/tsugu/src/remote/player_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-21 15:17:45.000000 tsugu-2.0.2/tsugu/src/remote/switch_car_forwarding_off.py
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-05-21 15:17:45.000000 tsugu-2.0.2/tsugu/src/remote/switch_car_forwarding_on.py
--rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-05-21 15:17:45.000000 tsugu-2.0.2/tsugu/src/remote/unbind_player.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:17:54.257714 tsugu-2.0.2/tsugu/src/universal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 15:17:45.000000 tsugu-2.0.2/tsugu/src/universal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-21 15:17:45.000000 tsugu-2.0.2/tsugu/src/universal/event_stage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-21 15:17:45.000000 tsugu-2.0.2/tsugu/src/universal/gacha_simulate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-21 15:17:45.000000 tsugu-2.0.2/tsugu/src/universal/get_card_illustration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-05-21 15:17:45.000000 tsugu-2.0.2/tsugu/src/universal/lsycx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-21 15:17:45.000000 tsugu-2.0.2/tsugu/src/universal/search_card.py
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-21 15:17:45.000000 tsugu-2.0.2/tsugu/src/universal/search_character.py
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-21 15:17:45.000000 tsugu-2.0.2/tsugu/src/universal/search_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-21 15:17:45.000000 tsugu-2.0.2/tsugu/src/universal/search_gacha.py
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-21 15:17:45.000000 tsugu-2.0.2/tsugu/src/universal/search_player.py
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-21 15:17:45.000000 tsugu-2.0.2/tsugu/src/universal/search_song.py
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-21 15:17:45.000000 tsugu-2.0.2/tsugu/src/universal/song_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-21 15:17:45.000000 tsugu-2.0.2/tsugu/src/universal/song_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-21 15:17:45.000000 tsugu-2.0.2/tsugu/src/universal/ycx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-21 15:17:45.000000 tsugu-2.0.2/tsugu/src/universal/ycx_all.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:17:54.257714 tsugu-2.0.2/tsugu/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     5067 2024-05-21 15:17:45.000000 tsugu-2.0.2/tsugu/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:17:54.253714 tsugu-2.0.2/tsugu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-05-21 15:17:54.000000 tsugu-2.0.2/tsugu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-21 15:17:54.000000 tsugu-2.0.2/tsugu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 15:17:54.000000 tsugu-2.0.2/tsugu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-21 15:17:54.000000 tsugu-2.0.2/tsugu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-21 15:17:54.000000 tsugu-2.0.2/tsugu.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:32:59.317789 tsugu-2.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-21 15:32:50.000000 tsugu-2.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-05-21 15:32:59.317789 tsugu-2.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-05-21 15:32:50.000000 tsugu-2.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 15:32:59.317789 tsugu-2.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-21 15:32:50.000000 tsugu-2.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:32:59.313789 tsugu-2.0.3/tsugu/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-21 15:32:50.000000 tsugu-2.0.3/tsugu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-05-21 15:32:50.000000 tsugu-2.0.3/tsugu/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:32:59.313789 tsugu-2.0.3/tsugu/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-05-21 15:32:50.000000 tsugu-2.0.3/tsugu/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:32:59.313789 tsugu-2.0.3/tsugu/src/bandoristation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 15:32:50.000000 tsugu-2.0.3/tsugu/src/bandoristation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4102 2024-05-21 15:32:50.000000 tsugu-2.0.3/tsugu/src/bandoristation/rooms_forward.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-05-21 15:32:50.000000 tsugu-2.0.3/tsugu/src/bandoristation/ycm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:32:59.313789 tsugu-2.0.3/tsugu/src/help/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 15:32:50.000000 tsugu-2.0.3/tsugu/src/help/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-21 15:32:50.000000 tsugu-2.0.3/tsugu/src/help/help.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:32:59.317789 tsugu-2.0.3/tsugu/src/remote/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 15:32:50.000000 tsugu-2.0.3/tsugu/src/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-05-21 15:32:50.000000 tsugu-2.0.3/tsugu/src/remote/bind_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-05-21 15:32:50.000000 tsugu-2.0.3/tsugu/src/remote/bind_player_verification_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-05-21 15:32:50.000000 tsugu-2.0.3/tsugu/src/remote/bind_player_verification_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-21 15:32:50.000000 tsugu-2.0.3/tsugu/src/remote/change_default_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-21 15:32:50.000000 tsugu-2.0.3/tsugu/src/remote/change_server_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5275 2024-05-21 15:32:50.000000 tsugu-2.0.3/tsugu/src/remote/player_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-21 15:32:50.000000 tsugu-2.0.3/tsugu/src/remote/switch_car_forwarding_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-05-21 15:32:50.000000 tsugu-2.0.3/tsugu/src/remote/switch_car_forwarding_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-05-21 15:32:50.000000 tsugu-2.0.3/tsugu/src/remote/unbind_player.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:32:59.317789 tsugu-2.0.3/tsugu/src/universal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 15:32:50.000000 tsugu-2.0.3/tsugu/src/universal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-21 15:32:50.000000 tsugu-2.0.3/tsugu/src/universal/event_stage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-21 15:32:50.000000 tsugu-2.0.3/tsugu/src/universal/gacha_simulate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-21 15:32:50.000000 tsugu-2.0.3/tsugu/src/universal/get_card_illustration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-05-21 15:32:50.000000 tsugu-2.0.3/tsugu/src/universal/lsycx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-21 15:32:50.000000 tsugu-2.0.3/tsugu/src/universal/search_card.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-21 15:32:50.000000 tsugu-2.0.3/tsugu/src/universal/search_character.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-21 15:32:50.000000 tsugu-2.0.3/tsugu/src/universal/search_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-21 15:32:50.000000 tsugu-2.0.3/tsugu/src/universal/search_gacha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-21 15:32:50.000000 tsugu-2.0.3/tsugu/src/universal/search_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-21 15:32:50.000000 tsugu-2.0.3/tsugu/src/universal/search_song.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-21 15:32:50.000000 tsugu-2.0.3/tsugu/src/universal/song_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-21 15:32:50.000000 tsugu-2.0.3/tsugu/src/universal/song_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-21 15:32:50.000000 tsugu-2.0.3/tsugu/src/universal/ycx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-05-21 15:32:50.000000 tsugu-2.0.3/tsugu/src/universal/ycx_all.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:32:59.317789 tsugu-2.0.3/tsugu/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     5067 2024-05-21 15:32:50.000000 tsugu-2.0.3/tsugu/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:32:59.313789 tsugu-2.0.3/tsugu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-05-21 15:32:59.000000 tsugu-2.0.3/tsugu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-21 15:32:59.000000 tsugu-2.0.3/tsugu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 15:32:59.000000 tsugu-2.0.3/tsugu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-21 15:32:59.000000 tsugu-2.0.3/tsugu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-21 15:32:59.000000 tsugu-2.0.3/tsugu.egg-info/top_level.txt
```

### Comparing `tsugu-2.0.2/LICENSE` & `tsugu-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.2/PKG-INFO` & `tsugu-2.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu
-Version: 2.0.2
+Version: 2.0.3
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
-Metadata-Version: 2.1 Name: tsugu Version: 2.0.2 Summary: Tsugu Python Frontend
+Metadata-Version: 2.1 Name: tsugu Version: 2.0.3 Summary: Tsugu Python Frontend
 Home-page: https://github.com/kumoSleeping/ChatTsuguPy Author: kumoSleeping
 Author-email: zjr2992@outlook.com License: MIT Description:
                        ************ CChhaatt TTssuugguu PPyy[[ttmmrrnn]] ************
 _â¨ Python ç¼åç [TsuguBanGDreamBot](https://github.com/Yamamoto-2/tsugu-
          bangdream-bot?tab=readme-ov-file) èªç¶è¯­è¨äº¤äºåº â¨_
                           _[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]
 --- ## ð¦ å®è£ ```shell pip install tsugu --upgrade ``` > API powered by
```

### Comparing `tsugu-2.0.2/README.md` & `tsugu-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.2/setup.py` & `tsugu-2.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r') as readme:
     long_description = readme.read()
 
 setup(
     name='tsugu',
-    version='2.0.2',
+    version='2.0.3',
     author='kumoSleeping',
     author_email='zjr2992@outlook.com',
     license="MIT",
     description='Tsugu Python Frontend',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/kumoSleeping/ChatTsuguPy',
```

### Comparing `tsugu-2.0.2/tsugu/handler.py` & `tsugu-2.0.3/tsugu/handler.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.2/tsugu/src/__init__.py` & `tsugu-2.0.3/tsugu/src/__init__.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.2/tsugu/src/bandoristation/rooms_forward.py` & `tsugu-2.0.3/tsugu/src/bandoristation/rooms_forward.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.2/tsugu/src/bandoristation/ycm.py` & `tsugu-2.0.3/tsugu/src/bandoristation/ycm.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.2/tsugu/src/help/help.py` & `tsugu-2.0.3/tsugu/src/help/help.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.2/tsugu/src/remote/bind_player.py` & `tsugu-2.0.3/tsugu/src/remote/bind_player.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.2/tsugu/src/remote/bind_player_verification_off.py` & `tsugu-2.0.3/tsugu/src/remote/bind_player_verification_off.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.2/tsugu/src/remote/bind_player_verification_on.py` & `tsugu-2.0.3/tsugu/src/remote/bind_player_verification_on.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.2/tsugu/src/remote/change_default_server.py` & `tsugu-2.0.3/tsugu/src/remote/change_default_server.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.2/tsugu/src/remote/change_server_mode.py` & `tsugu-2.0.3/tsugu/src/remote/change_server_mode.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.2/tsugu/src/remote/player_status.py` & `tsugu-2.0.3/tsugu/src/remote/player_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager
 from tsugu_api_core._typing import _ServerName
 import tsugu_api_async
 
 
 alc = Alconna(
         ["玩家状态"],
-        Args["serverName", _ServerName.__args__, None]["serverIndex", int, None],
+        Args["serverName;?", _ServerName.__args__]["serverIndex;?", int],
         meta=CommandMeta(
             compact=True,
             description="查询自己的玩家状态",
             usage='根据关键词或活动ID查询活动信息',
             example='''玩家状态 :返回玩家状态(优先当前服务器下第一条记录)
 玩家状态 1 :返回绑定的第一条记录的状态
 玩家状态 jp :返回绑定的cn服务器的记录的状态'''
```

### Comparing `tsugu-2.0.2/tsugu/src/remote/switch_car_forwarding_off.py` & `tsugu-2.0.3/tsugu/src/remote/switch_car_forwarding_off.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.2/tsugu/src/remote/switch_car_forwarding_on.py` & `tsugu-2.0.3/tsugu/src/remote/switch_car_forwarding_on.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.2/tsugu/src/remote/unbind_player.py` & `tsugu-2.0.3/tsugu/src/remote/unbind_player.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import tsugu_api
 from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager
 import tsugu_api_async
 
 
 alc = Alconna(
         ["解除绑定"],
-        Args["index#要解绑的绑定编号", int, None],
+        Args["index;?#要解绑的绑定编号", int],
         meta=CommandMeta(
             compact=True,
             description="解除绑定",
             usage="验证解绑 记录编号(数字)",
             example="验证解绑 1 : 解绑第一个记录"
         ),
     )
```

### Comparing `tsugu-2.0.2/tsugu/src/universal/event_stage.py` & `tsugu-2.0.3/tsugu/src/universal/event_stage.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.2/tsugu/src/universal/gacha_simulate.py` & `tsugu-2.0.3/tsugu/src/universal/gacha_simulate.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.2/tsugu/src/universal/get_card_illustration.py` & `tsugu-2.0.3/tsugu/src/universal/get_card_illustration.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.2/tsugu/src/universal/lsycx.py` & `tsugu-2.0.3/tsugu/src/universal/lsycx.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from tsugu_api_core._typing import _ServerName
 import tsugu_api_async
 
 
 alc = Alconna(
         ["lsycx", "历史预测线"], ['/', ''],
         Args['tier', int]['eventId;?#活动ID，省略时查询当前活动。', int]
-            ['serverName#省略服务器名时，默认从你当前的主服务器查询。', _ServerName.__args__, None],
+            ['serverName;?#省略服务器名时，默认从你当前的主服务器查询。', _ServerName.__args__],
         meta=CommandMeta(
             compact=True,
             description="查询指定档位的历史预测线。",
             usage='查询指定档位的预测线与最近的4期活动类型相同的活动的档线数据。',
             example='''lsycx 1000 
 lsycx 1000 177 jp'''
         )
```

### Comparing `tsugu-2.0.2/tsugu/src/universal/search_card.py` & `tsugu-2.0.3/tsugu/src/universal/search_card.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.2/tsugu/src/universal/search_character.py` & `tsugu-2.0.3/tsugu/src/universal/search_character.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.2/tsugu/src/universal/search_event.py` & `tsugu-2.0.3/tsugu/src/universal/search_event.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.2/tsugu/src/universal/search_gacha.py` & `tsugu-2.0.3/tsugu/src/universal/search_gacha.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.2/tsugu/src/universal/search_player.py` & `tsugu-2.0.3/tsugu/src/universal/search_player.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.2/tsugu/src/universal/search_song.py` & `tsugu-2.0.3/tsugu/src/universal/search_song.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.2/tsugu/src/universal/song_chart.py` & `tsugu-2.0.3/tsugu/src/universal/song_chart.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.2/tsugu/src/universal/song_meta.py` & `tsugu-2.0.3/tsugu/src/universal/song_meta.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.2/tsugu/src/universal/ycx.py` & `tsugu-2.0.3/tsugu/src/universal/ycx.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from tsugu_api_core._typing import _ServerName
 import tsugu_api_async
 
 
 alc = Alconna(
         ["ycx", "预测线"],
         Args['tier', int]['eventId;?#活动ID，省略时查询当前活动。', int]
-            ['serverName#省略服务器名时，默认从你当前的主服务器查询。', _ServerName.__args__, None],
+            ['serverName;?#省略服务器名时，默认从你当前的主服务器查询。', _ServerName.__args__],
         meta=CommandMeta(
             compact=True,
             description="查询指定档位的预测线",
             usage='查询指定档位的预测线。',
             example='''ycx 1000
 ycx 1000 177 jp'''
         )
```

### Comparing `tsugu-2.0.2/tsugu/src/universal/ycx_all.py` & `tsugu-2.0.3/tsugu/src/universal/ycx_all.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from tsugu_api_core._typing import _ServerName
 import tsugu_api_async
 
 
 alc = Alconna(
         ["ycxall", "ycx all"],
         Args['eventId;?#活动ID，省略时查询当前活动。', int]
-            ['serverName#省略服务器名时，默认从你当前的主服务器查询。活动ID不存在时，也可以作为第二个参数。', _ServerName.__args__, None],
+            ['serverName;?#省略服务器名时，默认从你当前的主服务器查询。活动ID不存在时，也可以作为第二个参数。', _ServerName.__args__],
         meta=CommandMeta(
             compact=True, description="查询指定档位的预测线",
             usage='根据关键词或角色ID查询角色信息',
             example='''ycx 1000 
 ycx 1000 177 jp'''
         )
     )
```

### Comparing `tsugu-2.0.2/tsugu/utils/__init__.py` & `tsugu-2.0.3/tsugu/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.2/tsugu.egg-info/PKG-INFO` & `tsugu-2.0.3/tsugu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu
-Version: 2.0.2
+Version: 2.0.3
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
-Metadata-Version: 2.1 Name: tsugu Version: 2.0.2 Summary: Tsugu Python Frontend
+Metadata-Version: 2.1 Name: tsugu Version: 2.0.3 Summary: Tsugu Python Frontend
 Home-page: https://github.com/kumoSleeping/ChatTsuguPy Author: kumoSleeping
 Author-email: zjr2992@outlook.com License: MIT Description:
                        ************ CChhaatt TTssuugguu PPyy[[ttmmrrnn]] ************
 _â¨ Python ç¼åç [TsuguBanGDreamBot](https://github.com/Yamamoto-2/tsugu-
          bangdream-bot?tab=readme-ov-file) èªç¶è¯­è¨äº¤äºåº â¨_
                           _[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]
 --- ## ð¦ å®è£ ```shell pip install tsugu --upgrade ``` > API powered by
```

### Comparing `tsugu-2.0.2/tsugu.egg-info/SOURCES.txt` & `tsugu-2.0.3/tsugu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

