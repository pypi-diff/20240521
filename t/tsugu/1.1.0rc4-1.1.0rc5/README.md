# Comparing `tmp/tsugu-1.1.0rc4.tar.gz` & `tmp/tsugu-1.1.0rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsugu-1.1.0rc4.tar", last modified: Tue May 21 07:51:35 2024, max compression
+gzip compressed data, was "tsugu-1.1.0rc5.tar", last modified: Tue May 21 10:06:26 2024, max compression
```

## Comparing `tsugu-1.1.0rc4.tar` & `tsugu-1.1.0rc5.tar`

### file list

```diff
@@ -1,98 +1,137 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:51:35.665378 tsugu-1.1.0rc4/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6443 2024-05-21 07:51:35.665378 tsugu-1.1.0rc4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4482 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 07:51:35.665378 tsugu-1.1.0rc4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:51:35.653378 tsugu-1.1.0rc4/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/test/test_async.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:51:35.653378 tsugu-1.1.0rc4/tsugu/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:51:35.653378 tsugu-1.1.0rc4/tsugu/src/
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:51:35.653378 tsugu-1.1.0rc4/tsugu/src/bandoristation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu/src/bandoristation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu/src/bandoristation/rooms_forward.py
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu/src/bandoristation/ycm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:51:35.653378 tsugu-1.1.0rc4/tsugu/src/help/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu/src/help/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu/src/help/help.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:51:35.657378 tsugu-1.1.0rc4/tsugu/src/remote/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu/src/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu/src/remote/bind_player.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu/src/remote/bind_player_verification_off.py
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu/src/remote/bind_player_verification_on.py
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu/src/remote/change_default_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu/src/remote/change_server_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu/src/remote/player_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu/src/remote/switch_car_forwarding_off.py
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu/src/remote/switch_car_forwarding_on.py
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu/src/remote/unbind_player.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:51:35.657378 tsugu-1.1.0rc4/tsugu/src/universal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu/src/universal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu/src/universal/event_stage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu/src/universal/gacha_simulate.py
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu/src/universal/get_card_illustration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu/src/universal/lsycx.py
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu/src/universal/search_card.py
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu/src/universal/search_character.py
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu/src/universal/search_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu/src/universal/search_gacha.py
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu/src/universal/search_player.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu/src/universal/search_song.py
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu/src/universal/song_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu/src/universal/song_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu/src/universal/ycx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu/src/universal/ycx_all.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:51:35.657378 tsugu-1.1.0rc4/tsugu/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     3292 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:51:35.653378 tsugu-1.1.0rc4/tsugu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6443 2024-05-21 07:51:35.000000 tsugu-1.1.0rc4/tsugu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-05-21 07:51:35.000000 tsugu-1.1.0rc4/tsugu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 07:51:35.000000 tsugu-1.1.0rc4/tsugu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-21 07:51:35.000000 tsugu-1.1.0rc4/tsugu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-21 07:51:35.000000 tsugu-1.1.0rc4/tsugu.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:51:35.657378 tsugu-1.1.0rc4/tsugu_async/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu_async/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu_async/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu_async/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:51:35.657378 tsugu-1.1.0rc4/tsugu_async/src/
--rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu_async/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:51:35.661378 tsugu-1.1.0rc4/tsugu_async/src/bandoristation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu_async/src/bandoristation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu_async/src/bandoristation/rooms_forward.py
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu_async/src/bandoristation/ycm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:51:35.661378 tsugu-1.1.0rc4/tsugu_async/src/help/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu_async/src/help/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu_async/src/help/help.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:51:35.661378 tsugu-1.1.0rc4/tsugu_async/src/remote/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu_async/src/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu_async/src/remote/bind_player.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu_async/src/remote/bind_player_verification_off.py
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu_async/src/remote/bind_player_verification_on.py
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu_async/src/remote/change_default_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu_async/src/remote/change_server_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu_async/src/remote/player_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu_async/src/remote/switch_car_forwarding_off.py
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu_async/src/remote/switch_car_forwarding_on.py
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu_async/src/remote/unbind_player.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:51:35.665378 tsugu-1.1.0rc4/tsugu_async/src/universal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu_async/src/universal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu_async/src/universal/event_stage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu_async/src/universal/gacha_simulate.py
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu_async/src/universal/get_card_illustration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu_async/src/universal/lsycx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu_async/src/universal/search_card.py
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu_async/src/universal/search_character.py
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu_async/src/universal/search_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu_async/src/universal/search_gacha.py
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu_async/src/universal/search_player.py
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu_async/src/universal/search_song.py
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu_async/src/universal/song_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu_async/src/universal/song_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu_async/src/universal/ycx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu_async/src/universal/ycx_all.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:51:35.665378 tsugu-1.1.0rc4/tsugu_async/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu_async/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:26.384228 tsugu-1.1.0rc5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6716 2024-05-21 10:06:26.384228 tsugu-1.1.0rc5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 10:06:26.384228 tsugu-1.1.0rc5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:26.372228 tsugu-1.1.0rc5/tsugu/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:26.372228 tsugu-1.1.0rc5/tsugu/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:26.372228 tsugu-1.1.0rc5/tsugu/src/bandoristation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu/src/bandoristation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu/src/bandoristation/rooms_forward.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu/src/bandoristation/ycm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:26.372228 tsugu-1.1.0rc5/tsugu/src/help/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu/src/help/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu/src/help/help.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:26.372228 tsugu-1.1.0rc5/tsugu/src/remote/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu/src/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu/src/remote/bind_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu/src/remote/bind_player_verification_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu/src/remote/bind_player_verification_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu/src/remote/change_default_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu/src/remote/change_server_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu/src/remote/player_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu/src/remote/switch_car_forwarding_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu/src/remote/switch_car_forwarding_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu/src/remote/unbind_player.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:26.376228 tsugu-1.1.0rc5/tsugu/src/universal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu/src/universal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu/src/universal/event_stage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu/src/universal/gacha_simulate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu/src/universal/get_card_illustration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu/src/universal/lsycx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu/src/universal/search_card.py
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu/src/universal/search_character.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu/src/universal/search_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu/src/universal/search_gacha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu/src/universal/search_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu/src/universal/search_song.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu/src/universal/song_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu/src/universal/song_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu/src/universal/ycx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu/src/universal/ycx_all.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:26.376228 tsugu-1.1.0rc5/tsugu/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     3292 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:26.372228 tsugu-1.1.0rc5/tsugu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6716 2024-05-21 10:06:26.000000 tsugu-1.1.0rc5/tsugu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4139 2024-05-21 10:06:26.000000 tsugu-1.1.0rc5/tsugu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 10:06:26.000000 tsugu-1.1.0rc5/tsugu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-21 10:06:26.000000 tsugu-1.1.0rc5/tsugu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-21 10:06:26.000000 tsugu-1.1.0rc5/tsugu.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:26.376228 tsugu-1.1.0rc5/tsugu_async/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_async/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_async/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_async/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:26.376228 tsugu-1.1.0rc5/tsugu_async/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_async/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:26.376228 tsugu-1.1.0rc5/tsugu_async/src/bandoristation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_async/src/bandoristation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_async/src/bandoristation/rooms_forward.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_async/src/bandoristation/ycm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:26.376228 tsugu-1.1.0rc5/tsugu_async/src/help/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_async/src/help/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_async/src/help/help.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:26.380228 tsugu-1.1.0rc5/tsugu_async/src/remote/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_async/src/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_async/src/remote/bind_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_async/src/remote/bind_player_verification_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_async/src/remote/bind_player_verification_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_async/src/remote/change_default_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_async/src/remote/change_server_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_async/src/remote/player_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_async/src/remote/switch_car_forwarding_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_async/src/remote/switch_car_forwarding_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_async/src/remote/unbind_player.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:26.380228 tsugu-1.1.0rc5/tsugu_async/src/universal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_async/src/universal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_async/src/universal/event_stage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_async/src/universal/gacha_simulate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_async/src/universal/get_card_illustration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_async/src/universal/lsycx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_async/src/universal/search_card.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_async/src/universal/search_character.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_async/src/universal/search_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_async/src/universal/search_gacha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_async/src/universal/search_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_async/src/universal/search_song.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_async/src/universal/song_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_async/src/universal/song_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_async/src/universal/ycx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_async/src/universal/ycx_all.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:26.380228 tsugu-1.1.0rc5/tsugu_async/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_async/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:26.380228 tsugu-1.1.0rc5/tsugu_thread/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_thread/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_thread/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:26.380228 tsugu-1.1.0rc5/tsugu_thread/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_thread/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:26.380228 tsugu-1.1.0rc5/tsugu_thread/src/bandoristation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_thread/src/bandoristation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_thread/src/bandoristation/rooms_forward.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_thread/src/bandoristation/ycm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:26.380228 tsugu-1.1.0rc5/tsugu_thread/src/help/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_thread/src/help/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_thread/src/help/help.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:26.384228 tsugu-1.1.0rc5/tsugu_thread/src/remote/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_thread/src/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_thread/src/remote/bind_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_thread/src/remote/bind_player_verification_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_thread/src/remote/bind_player_verification_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_thread/src/remote/change_default_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_thread/src/remote/change_server_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_thread/src/remote/player_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_thread/src/remote/switch_car_forwarding_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_thread/src/remote/switch_car_forwarding_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_thread/src/remote/unbind_player.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:26.384228 tsugu-1.1.0rc5/tsugu_thread/src/universal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_thread/src/universal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_thread/src/universal/event_stage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_thread/src/universal/gacha_simulate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_thread/src/universal/get_card_illustration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_thread/src/universal/lsycx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_thread/src/universal/search_card.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_thread/src/universal/search_character.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_thread/src/universal/search_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_thread/src/universal/search_gacha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_thread/src/universal/search_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_thread/src/universal/search_song.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_thread/src/universal/song_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_thread/src/universal/song_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_thread/src/universal/ycx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_thread/src/universal/ycx_all.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:26.384228 tsugu-1.1.0rc5/tsugu_thread/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     3237 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_thread/utils/__init__.py
```

### Comparing `tsugu-1.1.0rc4/LICENSE` & `tsugu-1.1.0rc5/LICENSE`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc4/PKG-INFO` & `tsugu-1.1.0rc5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu
-Version: 1.1.0rc4
+Version: 1.1.0rc5
 Summary: Tsugu Python Frontend
 Home-page: https://github.com/kumoSleeping/ChatTsuguPy
 Author: kumoSleeping
 Author-email: zjr2992@outlook.com
 License: MIT
 Description: 
         <h1 align="center"> Chat Tsugu Py <img src="./logo.jpg" width="30" width="30" height="30" alt="tmrn"/> </h1>
@@ -27,22 +27,30 @@
         <a href="https://pypi.org/project/tsugu/">
             <img src="https://img.shields.io/pypi/v/tsugu.svg" alt="license">
           </a>
         </p>
         
         ---
         
+        - [x] tsugu
+        - [x] tsugu_async
+        - [x] tsugu_thread
+        
+        
+        - `tsugu_thread` 中避免了在多线程环境中使用 `Alconna`，但同时不再支持 'compact' 配置项，`tsugu_thread` 不一定会一直维护。
+        
         
         ```shell
         pip install tsugu
         ```
         
         > API powered by  <a href="https://github.com/WindowsSov8forUs/tsugu-api-python?tab=readme-ov-file">tsugu-api-python</a>
         
         > Command matching provided by <a href="https://github.com/ArcletProject/Alconna">Alconna</a>
+        
         ***
         
         ## handler
         
         - `handler` 用于直接处理用户输入的自然语言并返回查询结果: 
         
         ```python
```

#### html2text {}

```diff
@@ -1,16 +1,19 @@
-Metadata-Version: 2.1 Name: tsugu Version: 1.1.0rc4 Summary: Tsugu Python
+Metadata-Version: 2.1 Name: tsugu Version: 1.1.0rc5 Summary: Tsugu Python
 Frontend Home-page: https://github.com/kumoSleeping/ChatTsuguPy Author:
 kumoSleeping Author-email: zjr2992@outlook.com License: MIT Description:
                        ************ CChhaatt TTssuugguu PPyy[[ttmmrrnn]] ************
 _â¨ Python ç¼åç [TsuguBanGDreamBot](https://github.com/Yamamoto-2/tsugu-
          bangdream-bot?tab=readme-ov-file) èªç¶è¯­è¨äº¤äºåº â¨_
                           _[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]
---- ```shell pip install tsugu ``` > API powered by _t_s_u_g_u_-_a_p_i_-_p_y_t_h_o_n > Command
-matching provided by _A_l_c_o_n_n_a *** ## handler - `handler`
+--- - [x] tsugu - [x] tsugu_async - [x] tsugu_thread - `tsugu_thread`
+ä¸­é¿åäºå¨å¤çº¿ç¨ç¯å¢ä¸­ä½¿ç¨ `Alconna`ï¼ä½åæ¶ä¸åæ¯æ
+'compact' éç½®é¡¹ï¼`tsugu_thread` ä¸ä¸å®ä¼ä¸ç´ç»´æ¤ã ```shell pip
+install tsugu ``` > API powered by _t_s_u_g_u_-_a_p_i_-_p_y_t_h_o_n > Command matching provided
+by _A_l_c_o_n_n_a *** ## handler - `handler`
 ç¨äºç´æ¥å¤çç¨æ·è¾å¥çèªç¶è¯­è¨å¹¶è¿åæ¥è¯¢ç»æ: ```python
 import tsugu # åä¸ªåæ°ï¼åå«æå³ç æ¶æ¯åå®¹ ç¨æ·id å¹³å°
 é¢éid for i in tsugu.handler(message='æ¥å¡ ars 1x', user_id='1528593481',
 platform='red', channel_id='666808414'): print('ææ¬: ',i) if isinstance(i,
 str) else None print(f"[å¾ç]") if isinstance(i, bytes) else None ```
 ```python import tsugu_async ... ``` > å¨å¸¸ç¨çqqbotä¸­ï¼ç¾¤å·å°±æ¯
 `channel_id`ã > å½ä½ ä½¿ç¨QQå·ä½ä¸º `user_id` æ¶ï¼`platform`
```

### Comparing `tsugu-1.1.0rc4/README.md` & `tsugu-1.1.0rc5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -19,22 +19,30 @@
 <a href="https://pypi.org/project/tsugu/">
     <img src="https://img.shields.io/pypi/v/tsugu.svg" alt="license">
   </a>
 </p>
 
 ---
 
+- [x] tsugu
+- [x] tsugu_async
+- [x] tsugu_thread
+
+
+- `tsugu_thread` 中避免了在多线程环境中使用 `Alconna`，但同时不再支持 'compact' 配置项，`tsugu_thread` 不一定会一直维护。
+
 
 ```shell
 pip install tsugu
 ```
 
 > API powered by  <a href="https://github.com/WindowsSov8forUs/tsugu-api-python?tab=readme-ov-file">tsugu-api-python</a>
 
 > Command matching provided by <a href="https://github.com/ArcletProject/Alconna">Alconna</a>
+
 ***
 
 ## handler
 
 - `handler` 用于直接处理用户输入的自然语言并返回查询结果: 
 
 ```python
```

#### html2text {}

```diff
@@ -1,13 +1,16 @@
                        ************ CChhaatt TTssuugguu PPyy[[ttmmrrnn]] ************
 _â¨ Python ç¼åç [TsuguBanGDreamBot](https://github.com/Yamamoto-2/tsugu-
          bangdream-bot?tab=readme-ov-file) èªç¶è¯­è¨äº¤äºåº â¨_
                           _[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]
---- ```shell pip install tsugu ``` > API powered by _t_s_u_g_u_-_a_p_i_-_p_y_t_h_o_n > Command
-matching provided by _A_l_c_o_n_n_a *** ## handler - `handler`
+--- - [x] tsugu - [x] tsugu_async - [x] tsugu_thread - `tsugu_thread`
+ä¸­é¿åäºå¨å¤çº¿ç¨ç¯å¢ä¸­ä½¿ç¨ `Alconna`ï¼ä½åæ¶ä¸åæ¯æ
+'compact' éç½®é¡¹ï¼`tsugu_thread` ä¸ä¸å®ä¼ä¸ç´ç»´æ¤ã ```shell pip
+install tsugu ``` > API powered by _t_s_u_g_u_-_a_p_i_-_p_y_t_h_o_n > Command matching provided
+by _A_l_c_o_n_n_a *** ## handler - `handler`
 ç¨äºç´æ¥å¤çç¨æ·è¾å¥çèªç¶è¯­è¨å¹¶è¿åæ¥è¯¢ç»æ: ```python
 import tsugu # åä¸ªåæ°ï¼åå«æå³ç æ¶æ¯åå®¹ ç¨æ·id å¹³å°
 é¢éid for i in tsugu.handler(message='æ¥å¡ ars 1x', user_id='1528593481',
 platform='red', channel_id='666808414'): print('ææ¬: ',i) if isinstance(i,
 str) else None print(f"[å¾ç]") if isinstance(i, bytes) else None ```
 ```python import tsugu_async ... ``` > å¨å¸¸ç¨çqqbotä¸­ï¼ç¾¤å·å°±æ¯
 `channel_id`ã > å½ä½ ä½¿ç¨QQå·ä½ä¸º `user_id` æ¶ï¼`platform`
```

### Comparing `tsugu-1.1.0rc4/setup.py` & `tsugu-1.1.0rc5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r') as readme:
     long_description = readme.read()
 
 setup(
     name='tsugu',
-    version='1.1.0-rc4',
+    version='1.1.0-rc5',
     author='kumoSleeping',
     author_email='zjr2992@outlook.com',
     license="MIT",
     description='Tsugu Python Frontend',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/kumoSleeping/ChatTsuguPy',
```

### Comparing `tsugu-1.1.0rc4/tsugu/handler.py` & `tsugu-1.1.0rc5/tsugu/handler.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc4/tsugu/src/__init__.py` & `tsugu-1.1.0rc5/tsugu/src/__init__.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc4/tsugu/src/bandoristation/rooms_forward.py` & `tsugu-1.1.0rc5/tsugu/src/bandoristation/rooms_forward.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc4/tsugu/src/bandoristation/ycm.py` & `tsugu-1.1.0rc5/tsugu/src/bandoristation/ycm.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc4/tsugu/src/help/help.py` & `tsugu-1.1.0rc5/tsugu/src/help/help.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc4/tsugu/src/remote/bind_player.py` & `tsugu-1.1.0rc5/tsugu/src/remote/bind_player.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc4/tsugu/src/remote/bind_player_verification_off.py` & `tsugu-1.1.0rc5/tsugu/src/remote/bind_player_verification_off.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc4/tsugu/src/remote/bind_player_verification_on.py` & `tsugu-1.1.0rc5/tsugu/src/remote/bind_player_verification_on.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc4/tsugu/src/remote/change_default_server.py` & `tsugu-1.1.0rc5/tsugu/src/remote/change_default_server.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc4/tsugu/src/remote/change_server_mode.py` & `tsugu-1.1.0rc5/tsugu/src/remote/change_server_mode.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc4/tsugu/src/remote/player_status.py` & `tsugu-1.1.0rc5/tsugu/src/remote/player_status.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc4/tsugu/src/remote/switch_car_forwarding_off.py` & `tsugu-1.1.0rc5/tsugu/src/remote/switch_car_forwarding_off.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc4/tsugu/src/remote/switch_car_forwarding_on.py` & `tsugu-1.1.0rc5/tsugu/src/remote/switch_car_forwarding_on.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc4/tsugu/src/remote/unbind_player.py` & `tsugu-1.1.0rc5/tsugu/src/remote/unbind_player.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc4/tsugu/src/universal/event_stage.py` & `tsugu-1.1.0rc5/tsugu/src/universal/event_stage.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,11 +18,11 @@
     ).parse(message)
 
     if res.matched:
         if res.meta:
             meta = True
         else:
             meta = False
-        print(meta)
+
         return tsugu_api.event_stage(user.server_mode, res.eventId, meta)
 
     return res
```

### Comparing `tsugu-1.1.0rc4/tsugu/src/universal/gacha_simulate.py` & `tsugu-1.1.0rc5/tsugu/src/universal/gacha_simulate.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc4/tsugu/src/universal/get_card_illustration.py` & `tsugu-1.1.0rc5/tsugu/src/universal/get_card_illustration.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc4/tsugu/src/universal/lsycx.py` & `tsugu-1.1.0rc5/tsugu/src/universal/lsycx.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc4/tsugu/src/universal/search_card.py` & `tsugu-1.1.0rc5/tsugu/src/universal/search_card.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc4/tsugu/src/universal/search_character.py` & `tsugu-1.1.0rc5/tsugu/src/universal/search_character.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc4/tsugu/src/universal/search_event.py` & `tsugu-1.1.0rc5/tsugu/src/universal/search_event.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc4/tsugu/src/universal/search_gacha.py` & `tsugu-1.1.0rc5/tsugu/src/universal/search_gacha.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc4/tsugu/src/universal/search_player.py` & `tsugu-1.1.0rc5/tsugu/src/universal/search_player.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc4/tsugu/src/universal/search_song.py` & `tsugu-1.1.0rc5/tsugu/src/universal/search_song.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc4/tsugu/src/universal/song_chart.py` & `tsugu-1.1.0rc5/tsugu/src/universal/song_chart.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc4/tsugu/src/universal/song_meta.py` & `tsugu-1.1.0rc5/tsugu/src/universal/song_meta.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc4/tsugu/src/universal/ycx.py` & `tsugu-1.1.0rc5/tsugu/src/universal/ycx.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc4/tsugu/src/universal/ycx_all.py` & `tsugu-1.1.0rc5/tsugu/src/universal/ycx_all.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc4/tsugu/utils/__init__.py` & `tsugu-1.1.0rc5/tsugu/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc4/tsugu.egg-info/PKG-INFO` & `tsugu-1.1.0rc5/tsugu.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu
-Version: 1.1.0rc4
+Version: 1.1.0rc5
 Summary: Tsugu Python Frontend
 Home-page: https://github.com/kumoSleeping/ChatTsuguPy
 Author: kumoSleeping
 Author-email: zjr2992@outlook.com
 License: MIT
 Description: 
         <h1 align="center"> Chat Tsugu Py <img src="./logo.jpg" width="30" width="30" height="30" alt="tmrn"/> </h1>
@@ -27,22 +27,30 @@
         <a href="https://pypi.org/project/tsugu/">
             <img src="https://img.shields.io/pypi/v/tsugu.svg" alt="license">
           </a>
         </p>
         
         ---
         
+        - [x] tsugu
+        - [x] tsugu_async
+        - [x] tsugu_thread
+        
+        
+        - `tsugu_thread` 中避免了在多线程环境中使用 `Alconna`，但同时不再支持 'compact' 配置项，`tsugu_thread` 不一定会一直维护。
+        
         
         ```shell
         pip install tsugu
         ```
         
         > API powered by  <a href="https://github.com/WindowsSov8forUs/tsugu-api-python?tab=readme-ov-file">tsugu-api-python</a>
         
         > Command matching provided by <a href="https://github.com/ArcletProject/Alconna">Alconna</a>
+        
         ***
         
         ## handler
         
         - `handler` 用于直接处理用户输入的自然语言并返回查询结果: 
         
         ```python
```

#### html2text {}

```diff
@@ -1,16 +1,19 @@
-Metadata-Version: 2.1 Name: tsugu Version: 1.1.0rc4 Summary: Tsugu Python
+Metadata-Version: 2.1 Name: tsugu Version: 1.1.0rc5 Summary: Tsugu Python
 Frontend Home-page: https://github.com/kumoSleeping/ChatTsuguPy Author:
 kumoSleeping Author-email: zjr2992@outlook.com License: MIT Description:
                        ************ CChhaatt TTssuugguu PPyy[[ttmmrrnn]] ************
 _â¨ Python ç¼åç [TsuguBanGDreamBot](https://github.com/Yamamoto-2/tsugu-
          bangdream-bot?tab=readme-ov-file) èªç¶è¯­è¨äº¤äºåº â¨_
                           _[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]
---- ```shell pip install tsugu ``` > API powered by _t_s_u_g_u_-_a_p_i_-_p_y_t_h_o_n > Command
-matching provided by _A_l_c_o_n_n_a *** ## handler - `handler`
+--- - [x] tsugu - [x] tsugu_async - [x] tsugu_thread - `tsugu_thread`
+ä¸­é¿åäºå¨å¤çº¿ç¨ç¯å¢ä¸­ä½¿ç¨ `Alconna`ï¼ä½åæ¶ä¸åæ¯æ
+'compact' éç½®é¡¹ï¼`tsugu_thread` ä¸ä¸å®ä¼ä¸ç´ç»´æ¤ã ```shell pip
+install tsugu ``` > API powered by _t_s_u_g_u_-_a_p_i_-_p_y_t_h_o_n > Command matching provided
+by _A_l_c_o_n_n_a *** ## handler - `handler`
 ç¨äºç´æ¥å¤çç¨æ·è¾å¥çèªç¶è¯­è¨å¹¶è¿åæ¥è¯¢ç»æ: ```python
 import tsugu # åä¸ªåæ°ï¼åå«æå³ç æ¶æ¯åå®¹ ç¨æ·id å¹³å°
 é¢éid for i in tsugu.handler(message='æ¥å¡ ars 1x', user_id='1528593481',
 platform='red', channel_id='666808414'): print('ææ¬: ',i) if isinstance(i,
 str) else None print(f"[å¾ç]") if isinstance(i, bytes) else None ```
 ```python import tsugu_async ... ``` > å¨å¸¸ç¨çqqbotä¸­ï¼ç¾¤å·å°±æ¯
 `channel_id`ã > å½ä½ ä½¿ç¨QQå·ä½ä¸º `user_id` æ¶ï¼`platform`
```

### Comparing `tsugu-1.1.0rc4/tsugu.egg-info/SOURCES.txt` & `tsugu-1.1.0rc5/tsugu.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 LICENSE
 README.md
 setup.py
-test/test_async.py
 tsugu/__init__.py
 tsugu/config.py
 tsugu/handler.py
 tsugu.egg-info/PKG-INFO
 tsugu.egg-info/SOURCES.txt
 tsugu.egg-info/dependency_links.txt
 tsugu.egg-info/requires.txt
@@ -72,8 +71,42 @@
 tsugu_async/src/universal/search_gacha.py
 tsugu_async/src/universal/search_player.py
 tsugu_async/src/universal/search_song.py
 tsugu_async/src/universal/song_chart.py
 tsugu_async/src/universal/song_meta.py
 tsugu_async/src/universal/ycx.py
 tsugu_async/src/universal/ycx_all.py
-tsugu_async/utils/__init__.py
+tsugu_async/utils/__init__.py
+tsugu_thread/__init__.py
+tsugu_thread/handler.py
+tsugu_thread/src/__init__.py
+tsugu_thread/src/bandoristation/__init__.py
+tsugu_thread/src/bandoristation/rooms_forward.py
+tsugu_thread/src/bandoristation/ycm.py
+tsugu_thread/src/help/__init__.py
+tsugu_thread/src/help/help.py
+tsugu_thread/src/remote/__init__.py
+tsugu_thread/src/remote/bind_player.py
+tsugu_thread/src/remote/bind_player_verification_off.py
+tsugu_thread/src/remote/bind_player_verification_on.py
+tsugu_thread/src/remote/change_default_server.py
+tsugu_thread/src/remote/change_server_mode.py
+tsugu_thread/src/remote/player_status.py
+tsugu_thread/src/remote/switch_car_forwarding_off.py
+tsugu_thread/src/remote/switch_car_forwarding_on.py
+tsugu_thread/src/remote/unbind_player.py
+tsugu_thread/src/universal/__init__.py
+tsugu_thread/src/universal/event_stage.py
+tsugu_thread/src/universal/gacha_simulate.py
+tsugu_thread/src/universal/get_card_illustration.py
+tsugu_thread/src/universal/lsycx.py
+tsugu_thread/src/universal/search_card.py
+tsugu_thread/src/universal/search_character.py
+tsugu_thread/src/universal/search_event.py
+tsugu_thread/src/universal/search_gacha.py
+tsugu_thread/src/universal/search_player.py
+tsugu_thread/src/universal/search_song.py
+tsugu_thread/src/universal/song_chart.py
+tsugu_thread/src/universal/song_meta.py
+tsugu_thread/src/universal/ycx.py
+tsugu_thread/src/universal/ycx_all.py
+tsugu_thread/utils/__init__.py
```

### Comparing `tsugu-1.1.0rc4/tsugu_async/handler.py` & `tsugu-1.1.0rc5/tsugu_async/handler.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc4/tsugu_async/src/__init__.py` & `tsugu-1.1.0rc5/tsugu_async/src/__init__.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc4/tsugu_async/src/bandoristation/rooms_forward.py` & `tsugu-1.1.0rc5/tsugu_async/src/bandoristation/rooms_forward.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc4/tsugu_async/src/bandoristation/ycm.py` & `tsugu-1.1.0rc5/tsugu_async/src/bandoristation/ycm.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc4/tsugu_async/src/help/help.py` & `tsugu-1.1.0rc5/tsugu_async/src/help/help.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc4/tsugu_async/src/remote/bind_player.py` & `tsugu-1.1.0rc5/tsugu_async/src/remote/bind_player.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc4/tsugu_async/src/remote/bind_player_verification_off.py` & `tsugu-1.1.0rc5/tsugu_async/src/remote/bind_player_verification_off.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc4/tsugu_async/src/remote/bind_player_verification_on.py` & `tsugu-1.1.0rc5/tsugu_async/src/remote/bind_player_verification_on.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc4/tsugu_async/src/remote/change_default_server.py` & `tsugu-1.1.0rc5/tsugu_async/src/remote/change_default_server.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc4/tsugu_async/src/remote/change_server_mode.py` & `tsugu-1.1.0rc5/tsugu_async/src/remote/change_server_mode.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc4/tsugu_async/src/remote/player_status.py` & `tsugu-1.1.0rc5/tsugu_async/src/remote/player_status.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc4/tsugu_async/src/remote/switch_car_forwarding_off.py` & `tsugu-1.1.0rc5/tsugu_async/src/remote/switch_car_forwarding_off.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc4/tsugu_async/src/remote/switch_car_forwarding_on.py` & `tsugu-1.1.0rc5/tsugu_async/src/remote/switch_car_forwarding_on.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc4/tsugu_async/src/remote/unbind_player.py` & `tsugu-1.1.0rc5/tsugu_async/src/remote/unbind_player.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc4/tsugu_async/src/universal/event_stage.py` & `tsugu-1.1.0rc5/tsugu_thread/src/universal/event_stage.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,31 @@
-from ...utils import text_response, User, server_id_2_server_name, server_name_2_server_id, server_exists, config
-import tsugu_api_async
+from ...utils import get_user, text_response, User, server_id_2_server_name, server_name_2_server_id
+import tsugu_api
 from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager
 
 
-async def handler(message: str, user: User, platform: str, channel_id: str):
-    res = Alconna(
+alc = Alconna(
         ["查试炼", '查stage', '查舞台', '查festival', '查5v5'],
         Args["eventId;?#省略活动ID时查询当前活动。", [int]]["meta;?#歌曲meta。", ['-m']],
 
         meta=CommandMeta(
-            compact=config.compact, description="查试炼",
+            compact=True, description="查试炼",
             usage='查询当前服务器当前活动试炼信息。',
             example='''查试炼 157 -m :返回157号活动的试炼信息，包含歌曲meta。
 查试炼 -m :返回当前活动的试炼信息，包含歌曲meta。
 查试炼 :返回当前活动的试炼信息。'''
         )
-    ).parse(message)
+    )
+
+
+def handler(message: str, user_id: str, platform: str, channel_id: str):
+    res = alc.parse(message)
 
     if res.matched:
+        user = get_user(user_id, platform)
         if res.meta:
             meta = True
         else:
             meta = False
-        print(meta)
-        return await tsugu_api_async.event_stage(user.server_mode, res.eventId, meta)
+        return tsugu_api.event_stage(user.server_mode, res.eventId, meta)
 
     return res
```

### Comparing `tsugu-1.1.0rc4/tsugu_async/src/universal/gacha_simulate.py` & `tsugu-1.1.0rc5/tsugu_async/src/universal/gacha_simulate.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc4/tsugu_async/src/universal/get_card_illustration.py` & `tsugu-1.1.0rc5/tsugu_async/src/universal/get_card_illustration.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc4/tsugu_async/src/universal/lsycx.py` & `tsugu-1.1.0rc5/tsugu_async/src/universal/lsycx.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc4/tsugu_async/src/universal/search_card.py` & `tsugu-1.1.0rc5/tsugu_async/src/universal/search_card.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc4/tsugu_async/src/universal/search_character.py` & `tsugu-1.1.0rc5/tsugu_async/src/universal/search_character.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc4/tsugu_async/src/universal/search_event.py` & `tsugu-1.1.0rc5/tsugu_async/src/universal/search_event.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc4/tsugu_async/src/universal/search_gacha.py` & `tsugu-1.1.0rc5/tsugu_async/src/universal/search_gacha.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc4/tsugu_async/src/universal/search_player.py` & `tsugu-1.1.0rc5/tsugu_async/src/universal/search_player.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc4/tsugu_async/src/universal/search_song.py` & `tsugu-1.1.0rc5/tsugu_async/src/universal/search_song.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc4/tsugu_async/src/universal/song_chart.py` & `tsugu-1.1.0rc5/tsugu_async/src/universal/song_chart.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc4/tsugu_async/src/universal/song_meta.py` & `tsugu-1.1.0rc5/tsugu_async/src/universal/song_meta.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc4/tsugu_async/src/universal/ycx.py` & `tsugu-1.1.0rc5/tsugu_async/src/universal/ycx.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc4/tsugu_async/src/universal/ycx_all.py` & `tsugu-1.1.0rc5/tsugu_async/src/universal/ycx_all.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc4/tsugu_async/utils/__init__.py` & `tsugu-1.1.0rc5/tsugu_async/utils/__init__.py`

 * *Files identical despite different names*

