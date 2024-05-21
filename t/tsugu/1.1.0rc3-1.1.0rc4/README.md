# Comparing `tmp/tsugu-1.1.0rc3.tar.gz` & `tmp/tsugu-1.1.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsugu-1.1.0rc3.tar", last modified: Tue May 21 03:40:11 2024, max compression
+gzip compressed data, was "tsugu-1.1.0rc4.tar", last modified: Tue May 21 07:51:35 2024, max compression
```

## Comparing `tsugu-1.1.0rc3.tar` & `tsugu-1.1.0rc4.tar`

### file list

```diff
@@ -1,92 +1,98 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 03:40:11.114071 tsugu-1.1.0rc3/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6443 2024-05-21 03:40:11.114071 tsugu-1.1.0rc3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4482 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 03:40:11.114071 tsugu-1.1.0rc3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 03:40:11.106071 tsugu-1.1.0rc3/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/test/test_async.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 03:40:11.106071 tsugu-1.1.0rc3/tsugu/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 03:40:11.106071 tsugu-1.1.0rc3/tsugu/router/
--rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu/router/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 03:40:11.106071 tsugu-1.1.0rc3/tsugu/router/bandoristation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu/router/bandoristation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2841 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu/router/bandoristation/rooms_forward.py
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu/router/bandoristation/ycm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 03:40:11.106071 tsugu-1.1.0rc3/tsugu/router/remote/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu/router/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu/router/remote/bind_player.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu/router/remote/bind_player_verification_off.py
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu/router/remote/bind_player_verification_on.py
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu/router/remote/change_default_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu/router/remote/change_server_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu/router/remote/player_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu/router/remote/switch_car_forwarding_off.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu/router/remote/switch_car_forwarding_on.py
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu/router/remote/unbind_player.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 03:40:11.110071 tsugu-1.1.0rc3/tsugu/router/universal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu/router/universal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu/router/universal/event_stage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu/router/universal/gacha_simulate.py
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu/router/universal/get_card_illustration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu/router/universal/lsycx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu/router/universal/search_card.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu/router/universal/search_character.py
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu/router/universal/search_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu/router/universal/search_gacha.py
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu/router/universal/search_player.py
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu/router/universal/search_song.py
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu/router/universal/song_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu/router/universal/song_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu/router/universal/ycx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu/router/universal/ycx_all.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 03:40:11.110071 tsugu-1.1.0rc3/tsugu/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 03:40:11.106071 tsugu-1.1.0rc3/tsugu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6443 2024-05-21 03:40:10.000000 tsugu-1.1.0rc3/tsugu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-05-21 03:40:11.000000 tsugu-1.1.0rc3/tsugu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 03:40:10.000000 tsugu-1.1.0rc3/tsugu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-21 03:40:10.000000 tsugu-1.1.0rc3/tsugu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-21 03:40:10.000000 tsugu-1.1.0rc3/tsugu.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 03:40:11.110071 tsugu-1.1.0rc3/tsugu_async/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu_async/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu_async/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu_async/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 03:40:11.110071 tsugu-1.1.0rc3/tsugu_async/router/
--rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu_async/router/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 03:40:11.110071 tsugu-1.1.0rc3/tsugu_async/router/bandoristation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu_async/router/bandoristation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu_async/router/bandoristation/rooms_forward.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu_async/router/bandoristation/ycm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 03:40:11.110071 tsugu-1.1.0rc3/tsugu_async/router/remote/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu_async/router/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu_async/router/remote/bind_player.py
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu_async/router/remote/bind_player_verification_off.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu_async/router/remote/bind_player_verification_on.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu_async/router/remote/change_default_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu_async/router/remote/change_server_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu_async/router/remote/player_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu_async/router/remote/switch_car_forwarding_off.py
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu_async/router/remote/switch_car_forwarding_on.py
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu_async/router/remote/unbind_player.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 03:40:11.114071 tsugu-1.1.0rc3/tsugu_async/router/universal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu_async/router/universal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu_async/router/universal/event_stage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu_async/router/universal/gacha_simulate.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu_async/router/universal/get_card_illustration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu_async/router/universal/lsycx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu_async/router/universal/search_card.py
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu_async/router/universal/search_character.py
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu_async/router/universal/search_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu_async/router/universal/search_gacha.py
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu_async/router/universal/search_player.py
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu_async/router/universal/search_song.py
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu_async/router/universal/song_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu_async/router/universal/song_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu_async/router/universal/ycx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu_async/router/universal/ycx_all.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 03:40:11.114071 tsugu-1.1.0rc3/tsugu_async/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu_async/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:51:35.665378 tsugu-1.1.0rc4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6443 2024-05-21 07:51:35.665378 tsugu-1.1.0rc4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4482 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 07:51:35.665378 tsugu-1.1.0rc4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:51:35.653378 tsugu-1.1.0rc4/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/test/test_async.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:51:35.653378 tsugu-1.1.0rc4/tsugu/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:51:35.653378 tsugu-1.1.0rc4/tsugu/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:51:35.653378 tsugu-1.1.0rc4/tsugu/src/bandoristation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu/src/bandoristation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu/src/bandoristation/rooms_forward.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu/src/bandoristation/ycm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:51:35.653378 tsugu-1.1.0rc4/tsugu/src/help/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu/src/help/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu/src/help/help.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:51:35.657378 tsugu-1.1.0rc4/tsugu/src/remote/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu/src/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu/src/remote/bind_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu/src/remote/bind_player_verification_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu/src/remote/bind_player_verification_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu/src/remote/change_default_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu/src/remote/change_server_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu/src/remote/player_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu/src/remote/switch_car_forwarding_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu/src/remote/switch_car_forwarding_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu/src/remote/unbind_player.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:51:35.657378 tsugu-1.1.0rc4/tsugu/src/universal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu/src/universal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu/src/universal/event_stage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu/src/universal/gacha_simulate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu/src/universal/get_card_illustration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu/src/universal/lsycx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu/src/universal/search_card.py
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu/src/universal/search_character.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu/src/universal/search_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu/src/universal/search_gacha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu/src/universal/search_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu/src/universal/search_song.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu/src/universal/song_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu/src/universal/song_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu/src/universal/ycx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu/src/universal/ycx_all.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:51:35.657378 tsugu-1.1.0rc4/tsugu/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     3292 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:51:35.653378 tsugu-1.1.0rc4/tsugu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6443 2024-05-21 07:51:35.000000 tsugu-1.1.0rc4/tsugu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-05-21 07:51:35.000000 tsugu-1.1.0rc4/tsugu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 07:51:35.000000 tsugu-1.1.0rc4/tsugu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-21 07:51:35.000000 tsugu-1.1.0rc4/tsugu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-21 07:51:35.000000 tsugu-1.1.0rc4/tsugu.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:51:35.657378 tsugu-1.1.0rc4/tsugu_async/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu_async/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu_async/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu_async/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:51:35.657378 tsugu-1.1.0rc4/tsugu_async/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu_async/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:51:35.661378 tsugu-1.1.0rc4/tsugu_async/src/bandoristation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu_async/src/bandoristation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu_async/src/bandoristation/rooms_forward.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu_async/src/bandoristation/ycm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:51:35.661378 tsugu-1.1.0rc4/tsugu_async/src/help/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu_async/src/help/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu_async/src/help/help.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:51:35.661378 tsugu-1.1.0rc4/tsugu_async/src/remote/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu_async/src/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu_async/src/remote/bind_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu_async/src/remote/bind_player_verification_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu_async/src/remote/bind_player_verification_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu_async/src/remote/change_default_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu_async/src/remote/change_server_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu_async/src/remote/player_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu_async/src/remote/switch_car_forwarding_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu_async/src/remote/switch_car_forwarding_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu_async/src/remote/unbind_player.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:51:35.665378 tsugu-1.1.0rc4/tsugu_async/src/universal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu_async/src/universal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu_async/src/universal/event_stage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu_async/src/universal/gacha_simulate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu_async/src/universal/get_card_illustration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu_async/src/universal/lsycx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu_async/src/universal/search_card.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu_async/src/universal/search_character.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu_async/src/universal/search_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu_async/src/universal/search_gacha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu_async/src/universal/search_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu_async/src/universal/search_song.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu_async/src/universal/song_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu_async/src/universal/song_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu_async/src/universal/ycx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu_async/src/universal/ycx_all.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:51:35.665378 tsugu-1.1.0rc4/tsugu_async/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-05-21 07:51:23.000000 tsugu-1.1.0rc4/tsugu_async/utils/__init__.py
```

### Comparing `tsugu-1.1.0rc3/LICENSE` & `tsugu-1.1.0rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc3/PKG-INFO` & `tsugu-1.1.0rc4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu
-Version: 1.1.0rc3
+Version: 1.1.0rc4
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
-Metadata-Version: 2.1 Name: tsugu Version: 1.1.0rc3 Summary: Tsugu Python
+Metadata-Version: 2.1 Name: tsugu Version: 1.1.0rc4 Summary: Tsugu Python
 Frontend Home-page: https://github.com/kumoSleeping/ChatTsuguPy Author:
 kumoSleeping Author-email: zjr2992@outlook.com License: MIT Description:
                        ************ CChhaatt TTssuugguu PPyy[[ttmmrrnn]] ************
 _â¨ Python ç¼åç [TsuguBanGDreamBot](https://github.com/Yamamoto-2/tsugu-
          bangdream-bot?tab=readme-ov-file) èªç¶è¯­è¨äº¤äºåº â¨_
                           _[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]
 --- ```shell pip install tsugu ``` > API powered by _t_s_u_g_u_-_a_p_i_-_p_y_t_h_o_n > Command
```

### Comparing `tsugu-1.1.0rc3/README.md` & `tsugu-1.1.0rc4/README.md`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc3/setup.py` & `tsugu-1.1.0rc4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r') as readme:
     long_description = readme.read()
 
 setup(
     name='tsugu',
-    version='1.1.0-rc3',
+    version='1.1.0-rc4',
     author='kumoSleeping',
     author_email='zjr2992@outlook.com',
     license="MIT",
     description='Tsugu Python Frontend',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/kumoSleeping/ChatTsuguPy',
```

### Comparing `tsugu-1.1.0rc3/test/test_async.py` & `tsugu-1.1.0rc4/test/test_async.py`

 * *Files 13% similar despite different names*

```diff
@@ -24,21 +24,16 @@
         # from tsugu_api_async import settings
         # settings.backend_url = 'http://127.0.0.1:8010'
         from tsugu_api_async import settings
 
         # settings.backend_url = 'http://124.221.153.148:3000'
         # settings.userdata_backend_url = 'http://127.0.0.1:3001'
 
-        msg1 = await tsugu_async.handler('查活动 -h', '1528593481', 'red', '666808414')
+        msg1 = await tsugu_async.handler('查活动 ksm ykn msr', '1528593481', 'red', '666808414')
         await show_back_msg(msg1)
 
-        msg2 = await tsugu_async.handler('查活动 -h', '1528593481', 'red', '666808414')
-        await show_back_msg(msg2)
-
-        msg3 = await tsugu_async.handler('查活动 -h', '1528593481', 'red', '666808414')
-        await show_back_msg(msg3)
 
         # print(tsugu_api.get_user_data('red', '1528593481'))
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `tsugu-1.1.0rc3/tsugu/handler.py` & `tsugu-1.1.0rc4/tsugu/handler.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import base64
 from typing import List, Union, Dict
 
 from .utils import *
 from loguru import logger
-from . import router
+from . import src
 
 
 def handler(message: str, user_id: str, platform: str, channel_id: str) -> List[Union[bytes, str]]:
     '''
     Tsugu Handler
     处理用户输入的自然语言，返回处理后的结果
 
@@ -37,15 +37,15 @@
     :param message: 用户消息
     :param user_id: 用户ID
     :param platform: 平台名称 一般为 red
     :param channel_id: 频道ID / 群号
     :return: List[Dict[str, str]]
     '''
     try:
-        return r if (r := router.handler(message, user_id, platform, channel_id)) else None
+        return r if (r := src.handler(message, user_id, platform, channel_id)) else None
     except Exception as e:
         logger.error(f'Error: {e}')
         raise e
```

### Comparing `tsugu-1.1.0rc3/tsugu/router/__init__.py` & `tsugu-1.1.0rc4/tsugu_async/src/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 import importlib
-from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, output_manager, command_manager
+from arclet.alconna import Arparma, output_manager, command_manager
 from ..utils import text_response, get_user
-import threading
-
-
-def require(module_path, cmd):
-    globals()[cmd] = importlib.import_module(module_path.format(cmd=cmd), __package__)
 
 
+# 主要功能
 universal_list = [
     "get_card_illustration",
     "search_player",
     "gacha_simulate",
     "search_gacha",
     "search_event",
     "search_song",
@@ -21,81 +17,71 @@
     "ycx_all",
     "ycx",
     "lsycx",
     "search_card",
     "event_stage",
 ]
 
+# 远程数据库相关功能
 remote_commands = [
     "player_status",
     "switch_car_forwarding_off",
     "switch_car_forwarding_on",
     "bind_player",
     "unbind_player",
     "change_server_mode",
     "change_default_server",
     "bind_player_verification_off",
     "bind_player_verification_on",
 ]
 
-
+# BandoriStation 相关功能
 bandoristation_commands = [
     "ycm",
     "rooms_forward",
 ]
 
-# 导入模块
-[require(f'.universal.{cmd}', cmd) for cmd in universal_list]
-[require(f'.remote.{cmd}', cmd) for cmd in remote_commands]
-[require(f'.bandoristation.{cmd}', cmd) for cmd in bandoristation_commands]
-
-
-class ThisValue:
-    def __init__(self):
-        self.local_data = threading.local()
-
-    def set_h(self, value):
-        self.local_data.h = value
-
-    def get_h(self):
-        return getattr(self.local_data, 'h', None)
+# 帮助信息
+help_command = [
+    "help",
+]
 
 
-this_value = ThisValue()
+def require(module_path, cmd):
+    globals()[cmd] = importlib.import_module(module_path.format(cmd=cmd), __package__)
 
 
-def handler(message, user_id, platform, channel_id):
-    user = get_user(user_id, platform)
+# 导入模块
+[require(f'.universal.{cmd}', cmd) for cmd in universal_list]
+[require(f'.remote.{cmd}', cmd) for cmd in remote_commands]
+[require(f'.bandoristation.{cmd}', cmd) for cmd in bandoristation_commands]
+[require(f'.help.{cmd}', cmd) for cmd in help_command]
 
-    def set_output_str(arg):
-        # 为每个线程设置独立的 h 值
-        this_value.set_h(arg)
 
-    output_manager.set_action(set_output_str)
+async def handler(message, user_id, platform, channel_id):
+    user = await get_user(user_id, platform)
+    output_manager.set_action(lambda *_: None)
+    union_list = universal_list + remote_commands + bandoristation_commands + help_command
+
+    for i in union_list:
+        result = await getattr(globals()[i], 'handler')(message, user, platform, channel_id)
+
+        # 未生成结果
+        if isinstance(result, Arparma):
+            # 匹配了命令头
+            if result.head_matched:
+
+                # 帮助信息
+                if result.error_data == ['-h']:
+                    return await getattr(globals()['help'], 'handler')('help ' + result.header_result, user, platform, channel_id)
+                # 错误信息
+                else:
+                    return text_response(result.error_info)
 
-    def handler_feats(cmd_list):
-        for i in cmd_list:
-            result = getattr(globals()[i], 'handler')(message, user, platform, channel_id)
-            if not result:
-                continue
-            if result[0].get('type') == 'string' and result[0].get('string') == 'help':
-                return text_response(this_value.get_h())
+        # 已生成结果
+        if isinstance(result, list):
             return result
-        return None
 
-    res = handler_feats(universal_list)
-    if res:
-        return res
-
-    res = handler_feats(remote_commands)
-    if res:
-        return res
-
-    res = handler_feats(bandoristation_commands)
-    if res:
-        return res
+    return None
 
-    if message in ["help", "帮助"]:
-        return text_response(command_manager.all_command_help(show_index=True))
 
-    return None
```

### Comparing `tsugu-1.1.0rc3/tsugu/router/bandoristation/rooms_forward.py` & `tsugu-1.1.0rc4/tsugu/src/bandoristation/rooms_forward.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,67 +1,61 @@
 from ...utils import text_response, User, get_user
 import tsugu_api
-from ...config import config
 from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager
 import re
 
 
 # 虚空注册
-alc = Alconna(
-        ["上传车牌"],
-        meta=CommandMeta(
-            compact=config.compact, description="上传车牌",
-        )
-    )
+alc = Alconna(["上传车牌"],meta=CommandMeta(description="上传车牌",))
 
 
 def handler(message: str, user: User, platform: str, channel_id: str):
     if message.startswith("上传车牌"):
         message = message[4:].strip()
 
     # 检查car_config['car']中的关键字
     for keyword in _car_config["car"]:
         if str(keyword) in message:
             break
     else:
-        return []
+        return None
 
     # 检查car_config['fake']中的关键字
     for keyword in _car_config["fake"]:
         if str(keyword) in message:
-            return []
+            return None
 
     pattern = r"^\d{5}(\D|$)|^\d{6}(\D|$)"
     if not re.match(pattern, message):
-        return []
+        return None
 
     user = get_user(user.user_id, platform)
 
     # 获取用户数据
     try:
         if platform:
             if not user.car:
-                return []
+                return None
     except Exception as e:
         # 默认不开启关闭车牌，继续提交
         pass
 
     try:
         car_id = message[:6]
         if not car_id.isdigit() and car_id[:5].isdigit():
             car_id = car_id[:5]
         if user.user_id.isdigit():
             car_user_id = user.user_id
         else:
             car_user_id = '3889000770'
         tsugu_api.submit_room_number(number=int(car_id), user_id=car_user_id, raw_message=message, source=config.bandori_station_token_name, token=config.bandori_station_token)
-        return []
+        return None
 
     except Exception as e:
-        return []
+        return None
 
 
 _car_config = {
     "car": [
         "q1",
         "q2",
         "q3",
```

### Comparing `tsugu-1.1.0rc3/tsugu/router/bandoristation/ycm.py` & `tsugu-1.1.0rc4/tsugu/src/bandoristation/ycm.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,23 @@
-from ...utils import text_response, User
+from ...utils import text_response, User, config
 import tsugu_api
-from ...config import config
 from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager
 
 
-alc = Alconna(
+def handler(message: str, user: User, platform: str, channel_id: str):
+    res = Alconna(
         ["ycm", "车来", "有车吗"],
         meta=CommandMeta(
             compact=config.compact, description="获取车牌",
         )
-    )
-
-
-def handler(message: str, user: User, platform: str, channel_id: str):
-    res = alc.parse(message)
+    ).parse(message)
 
     if res.matched:
         return car_search()
-    elif res.head_matched:
-        return text_response(res.error_info)
-    return None
+    return res
 
 
 def car_search():
     try:
         data = tsugu_api.query_room_number()
     except Exception as e:
         return text_response('获取房间信息失败，请稍后再试')
```

### Comparing `tsugu-1.1.0rc3/tsugu/router/remote/bind_player.py` & `tsugu-1.1.0rc4/tsugu_async/src/remote/bind_player.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,24 @@
-from ...utils import text_response, User, server_id_2_server_name, server_name_2_server_id, server_exists
-import tsugu_api
-from ...config import config
+from ...utils import config, text_response, User, server_id_2_server_name, server_name_2_server_id, server_exists
+import tsugu_api_async
 from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager, MultiVar, AllParam
-from tsugu_api_core._typing import _ServerName
 
 
-alc = Alconna(
+async def handler(message: str, user: User, platform: str, channel_id: str):
+    res = Alconna(
         ["绑定玩家"],
     Args["args;?", AllParam],
     meta=CommandMeta(
             compact=config.compact, description="绑定玩家",
             usage="只需发送‘绑定玩家’。",
         ),
-    )
-
-
-def handler(message: str, user: User, platform: str, channel_id: str):
-    res = alc.parse(message)
+    ).parse(message)
 
     if res.matched:
-        r = tsugu_api.bind_player_request(platform, user.user_id, user.server_mode, False)
+        r = await tsugu_api_async.bind_player_request(platform, user.user_id, user.server_mode, False)
         if r.get('status') != 'success':
             return text_response(r.get('data'))
         return text_response(
             f'''正在绑定账号，请将 评论(个性签名) 或者 当前使用的 乐队编队名称改为\n{r.get('data')['verifyCode']}\n稍等片刻等待同步后，发送\n验证绑定 你的玩家ID(数字) 服务器名(字母缩写)\n例如：验证绑定 114****514 cn''')
-    elif res.head_matched:
-        return text_response(res.error_info)
-    return None
+
+    return res
```

### Comparing `tsugu-1.1.0rc3/tsugu/router/remote/bind_player_verification_off.py` & `tsugu-1.1.0rc4/tsugu/src/remote/player_status.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,52 +1,71 @@
-from ...utils import text_response, User, server_id_2_server_name, server_name_2_server_id, server_exists
+from ...utils import text_response, User, server_id_2_server_name, server_name_2_server_id, server_exists, config
 import tsugu_api
-from ...config import config
 from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager
 from tsugu_api_core._typing import _ServerName
 
 
-alc = Alconna(
-        ["验证解绑"],
-    Args["index#要解绑的绑定编号", int],
+def handler(message: str, user: User, platform: str, channel_id: str):
+    res = Alconna(
+        ["玩家状态"],
+        Args["serverName", _ServerName.__args__, None]["serverIndex", int, None],
         meta=CommandMeta(
-            compact=config.compact, description="验证解绑",
-            usage="验证解绑 记录编号(数字)",
-            example="验证解绑 1 : 解绑第一个记录"
-        ),
-    )
+            compact=config.compact, description="查询自己的玩家状态",
+            usage='根据关键词或活动ID查询活动信息',
+            example='''玩家状态 :返回玩家状态(优先当前服务器下第一条记录)
+玩家状态 1 :返回绑定的第一条记录的状态
+玩家状态 jp :返回绑定的cn服务器的记录的状态'''
+        )
+    ).parse(message)
 
+    if res.matched:
+        if res.serverName:
+            return _case_server(user, res.serverName)
+        elif res.serverIndex:
+            return _case_index(user, res.serverIndex)
+        else:
+            return _case_default(user)
+    return res
+
+
+
+def _utils_search_player_by_game_id(game_id, additional_text=""):
+    player_id = str(game_id.get("game_id"))
+    server = int(game_id.get("server"))
+    response = tsugu_api.search_player(int(player_id), server)
+    return response + text_response(additional_text)
+
+
+def _case_default(user: User):
+    # 优先当前服务器
+    for game_id in user.game_ids:
+        if game_id.get("server") == user.server_mode:
+            text = f'已查找默认服务器 {server_id_2_server_name(user.server_mode)} 的记录。'
+            return _utils_search_player_by_game_id(game_id, text)
+    # 兜底逻辑：使用第一个记录
+    if user.game_ids:
+        game_id = user.game_ids[0]
+        text = f'已查找第一个记录。'
+        return _utils_search_player_by_game_id(game_id, text)
+    return text_response('未绑定任何记录，可以使用 绑定玩家 进行绑定')
+
+
+def _case_server(user: User, server_name: str):
+    server_id = server_name_2_server_id(server_name)
+    # 服务器不存在
+    if not server_exists(server_id):
+        return text_response(f'服务器 {server_name} 不存在。')
+    # 查找记录
+    for game_id in user.game_ids:
+        if game_id.get("server") == server_id:
+            # 找到记录
+            return _utils_search_player_by_game_id(game_id)
+    # 未找到记录
+    return text_response(f'未在记录中找到服务器 {server_name} 的记录。')
+
+
+def _case_index(user: User, index: int):
+    if index > len(user.game_ids) or index < 1:
+        return text_response(f'未找到记录 {index}。')
+    return _utils_search_player_by_game_id(user.game_ids[index - 1])
 
-def handler(message: str, user: User, platform: str, channel_id: str):
-    res = alc.parse(message)
 
-    if res.matched:
-        if len(user.game_ids) < int(res.index):
-            return text_response('未找到记录')
-        player_id = user.game_ids[int(res.index) - 1].get("game_id")
-        server_mode = user.game_ids[int(res.index) - 1].get("server")
-        r = tsugu_api.bind_player_verification(platform, user.user_id, server_mode, player_id, False)
-        if r.get('status') != 'success':
-            return text_response(r.get('data'))
-        return text_response('解绑成功！')
-    elif res.head_matched:
-        return text_response(res.error_info)
-    return None
-
-
-# def handler(user: User, res: MC, platform: str, channel_id: str):
-#     if not res.args or len(res.args) > 1:
-#         return text_response('请输入正确的格式：验证解绑 记录编号(数字)')
-#     if not res.args[0].isdigit():
-#         return text_response('请输入正确的格式：验证解绑 记录编号(数字)')
-#     if int(res.text) <= 0:
-#         return text_response('请输入正确的格式：验证解绑 记录编号(数字)，编号从1开始')
-#     if len(user.game_ids) < int(res.text):
-#         return text_response('未找到记录')
-#     player_id = user.game_ids[int(res.args[0]) - 1].get("game_id")
-#     server_mode = user.game_ids[int(res.args[0]) - 1].get("server")
-#     r = tsugu_api.bind_player_verification(platform, user.user_id, server_mode, player_id, False)
-#     if r.get('status') != 'success':
-#         return text_response(r.get('data'))
-#     return text_response('解绑成功！')
-#
-#
```

### Comparing `tsugu-1.1.0rc3/tsugu/router/remote/bind_player_verification_on.py` & `tsugu-1.1.0rc4/tsugu/src/remote/bind_player_verification_on.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,21 @@
-from ...utils import text_response, User, server_id_2_server_name, server_name_2_server_id, server_exists
+from ...utils import text_response, User, server_id_2_server_name, server_name_2_server_id, server_exists, config
 import tsugu_api
-from ...config import config
 from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager
 from tsugu_api_core._typing import _ServerName
 
-alc = Alconna(
+
+def handler(message: str, user: User, platform: str, channel_id: str):
+    res = Alconna(
         ["验证绑定"],
-    Args["playerID#你的玩家ID(数字)", int]["serverName#服务器名(字母缩写)", _ServerName],
+        Args["playerID#你的玩家ID(数字)", int]["serverName#服务器名(字母缩写)", _ServerName],
         meta=CommandMeta(
             compact=config.compact, description="验证绑定",)
-    )
-
-
-def handler(message: str, user: User, platform: str, channel_id: str):
-    res = alc.parse(message)
+    ).parse(message)
 
     if res.matched:
         server = server_name_2_server_id(res.serverName)
         r = tsugu_api.bind_player_verification(platform, user.user_id, server, res.playerID, True)
         if r.get('status') != 'success':
             return text_response(r.get('data'))
         return text_response('绑定成功！现在可以使用 玩家状态 {len(user.game_ids) + 1} 查看绑定的玩家状态')
-    elif res.head_matched:
-        return text_response(res.error_info)
-    return None
+    return res
```

### Comparing `tsugu-1.1.0rc3/tsugu/router/remote/change_default_server.py` & `tsugu-1.1.0rc4/tsugu_async/src/remote/bind_player_verification_off.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,29 @@
-from ...utils import text_response, User, server_names_2_server_ids
-import tsugu_api
-from ...config import config
-from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager, MultiVar
-from tsugu_api_core._typing import _ServerName
-
-alc = Alconna(
-        ["设置默认服务器", "默认服务器"],
-    Args["serverList#使用空格分隔服务器列表。", MultiVar(_ServerName)],
-        meta=CommandMeta(
-            compact=config.compact, description="设定信息显示中的默认服务器排序",
-            example="""设置默认服务器 cn jp : 将国服设置为第一服务器，日服设置为第二服务器。"""
-
-        )
-    )
+from ...utils import text_response, User, server_id_2_server_name, server_name_2_server_id, server_exists, config
+import tsugu_api_async
+from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager
 
 
-def handler(message: str, user: User, platform: str, channel_id: str):
-    res = alc.parse(message)
+async def handler(message: str, user: User, platform: str, channel_id: str):
+    res = Alconna(
+        ["验证解绑"],
+        Args["index#要解绑的绑定编号", int],
+        meta=CommandMeta(
+            compact=config.compact, description="验证解绑",
+            usage="验证解绑 记录编号(数字)",
+            example="验证解绑 1 : 解绑第一个记录"
+        ),
+    ).parse(message)
 
     if res.matched:
-        print(res.serverList)
-        print(server_names_2_server_ids(res.serverList))
-        r = tsugu_api.change_user_data(platform, user.user_id, {'default_server': server_names_2_server_ids(res.serverList)})
+        if len(user.game_ids) < int(res.index):
+            return text_response('未找到记录')
+        player_id = user.game_ids[int(res.index) - 1].get("game_id")
+        server_mode = user.game_ids[int(res.index) - 1].get("server")
+        r = await tsugu_api_async.bind_player_verification(platform, user.user_id, server_mode, player_id, False)
         if r.get('status') != 'success':
             return text_response(r.get('data'))
-        return text_response('默认服务器已设置为 ' + ' '.join(res.serverList))
-    elif res.head_matched:
-        return text_response(res.error_info)
-    return None
+        return text_response('解绑成功！')
+    
+    return res
+
+
```

### Comparing `tsugu-1.1.0rc3/tsugu/router/remote/change_server_mode.py` & `tsugu-1.1.0rc4/tsugu_async/src/remote/change_server_mode.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,25 @@
-from ...utils import text_response, User, server_name_2_server_id
-import tsugu_api
-from ...config import config
+from ...utils import text_response, User, server_id_2_server_name, server_name_2_server_id, server_exists, config
+import tsugu_api_async
 from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager, MultiVar
 from tsugu_api_core._typing import _ServerName
 
-alc = Alconna(
+
+async def handler(message: str, user: User, platform: str, channel_id: str):
+    res = Alconna(
         ["主服务器", "设置主服务器"],
     Args["serverName#服务器名", _ServerName],
         meta=CommandMeta(
             compact=config.compact, description="主服务器",
             usage="将指定的服务器设置为你的主服务器。",
             example="""主服务器 cn : 将国服设置为主服务器。"""
 
         )
-    )
-
-
-def handler(message: str, user: User, platform: str, channel_id: str):
-    res = alc.parse(message)
+    ).parse(message)
 
     if res.matched:
-        r = tsugu_api.change_user_data(platform, user.user_id, {'server_mode': server_name_2_server_id(res.serverName)})
+        r = await tsugu_api_async.change_user_data(platform, user.user_id, {'server_mode': server_name_2_server_id(res.serverName)})
         if r.get('status') != 'success':
             return text_response(r.get('data'))
         return text_response('主服务器已设置为 ' + res.serverName)
-    elif res.head_matched:
-        return text_response(res.error_info)
-    return None
+    return res
 
-#
-# def handler(user: User, res: MC, platform: str, channel_id: str):
-#     if res.args:
-#         server_mode = server_name_2_server_id(res.args[0])
-#         if not server_exists(server_mode):
-#             return text_response('未找到服务器，请输入正确的服务器名')
-#         update: _Update = {'server_mode': server_mode, }
-#         if r := tsugu_api.change_user_data(platform, user.user_id, update):
-#             if r.get('status') == 'success':
-#                 return text_response('主服务器已设置为 ' + server_id_2_server_name(server_mode))
-#             return text_response(r.get('data'))
-#
```

### Comparing `tsugu-1.1.0rc3/tsugu/router/remote/player_status.py` & `tsugu-1.1.0rc4/tsugu_async/src/remote/player_status.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,77 +1,71 @@
-from ...utils import text_response, User, server_id_2_server_name, server_name_2_server_id, server_exists
-import tsugu_api
-from ...config import config
+from ...utils import text_response, User, server_id_2_server_name, server_name_2_server_id, server_exists, config
+import tsugu_api_async
 from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager
 from tsugu_api_core._typing import _ServerName
 
 
-alc = Alconna(
+async def handler(message: str, user: User, platform: str, channel_id: str):
+    res = Alconna(
         ["玩家状态"],
         Args["serverName", _ServerName.__args__, None]["serverIndex", int, None],
         meta=CommandMeta(
             compact=config.compact, description="查询自己的玩家状态",
             usage='根据关键词或活动ID查询活动信息',
             example='''玩家状态 :返回玩家状态(优先当前服务器下第一条记录)
 玩家状态 1 :返回绑定的第一条记录的状态
 玩家状态 jp :返回绑定的cn服务器的记录的状态'''
         )
-    )
-
-
-def handler(message: str, user: User, platform: str, channel_id: str):
-    res = alc.parse(message)
+    ).parse(message)
 
     if res.matched:
         if res.serverName:
-            return _case_server(user, res.serverName)
+            return await _case_server(user, res.serverName)
         elif res.serverIndex:
-            return _case_index(user, res.serverIndex)
+            return await _case_index(user, res.serverIndex)
         else:
-            return _case_default(user)
-    elif res.head_matched:
-        return text_response(res.error_info)
-    return None
+            return await _case_default(user)
+    return res
 
 
 
-def _utils_search_player_by_game_id(game_id, additional_text=""):
+async def _utils_search_player_by_game_id(game_id, additional_text=""):
     player_id = str(game_id.get("game_id"))
     server = int(game_id.get("server"))
-    response = tsugu_api.search_player(int(player_id), server)
+    response = await tsugu_api_async.search_player(int(player_id), server)
     return response + text_response(additional_text)
 
 
-def _case_default(user: User):
+async def _case_default(user: User):
     # 优先当前服务器
     for game_id in user.game_ids:
         if game_id.get("server") == user.server_mode:
             text = f'已查找默认服务器 {server_id_2_server_name(user.server_mode)} 的记录。'
-            return _utils_search_player_by_game_id(game_id, text)
+            return await _utils_search_player_by_game_id(game_id, text)
     # 兜底逻辑：使用第一个记录
     if user.game_ids:
         game_id = user.game_ids[0]
         text = f'已查找第一个记录。'
-        return _utils_search_player_by_game_id(game_id, text)
+        return await _utils_search_player_by_game_id(game_id, text)
     return text_response('未绑定任何记录，可以使用 绑定玩家 进行绑定')
 
 
-def _case_server(user: User, server_name: str):
+async def _case_server(user: User, server_name: str):
     server_id = server_name_2_server_id(server_name)
     # 服务器不存在
     if not server_exists(server_id):
         return text_response(f'服务器 {server_name} 不存在。')
     # 查找记录
     for game_id in user.game_ids:
         if game_id.get("server") == server_id:
             # 找到记录
-            return _utils_search_player_by_game_id(game_id)
+            return await _utils_search_player_by_game_id(game_id)
     # 未找到记录
     return text_response(f'未在记录中找到服务器 {server_name} 的记录。')
 
 
-def _case_index(user: User, index: int):
+async def _case_index(user: User, index: int):
     if index > len(user.game_ids) or index < 1:
         return text_response(f'未找到记录 {index}。')
-    return _utils_search_player_by_game_id(user.game_ids[index - 1])
+    return await _utils_search_player_by_game_id(user.game_ids[index - 1])
```

### Comparing `tsugu-1.1.0rc3/tsugu/router/remote/switch_car_forwarding_off.py` & `tsugu-1.1.0rc4/tsugu_async/src/remote/switch_car_forwarding_off.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,20 @@
-from ...utils import text_response, User, server_id_2_server_name, server_name_2_server_id, server_exists
-import tsugu_api
-from ...config import config
+from ...utils import text_response, User, server_id_2_server_name, server_name_2_server_id, server_exists, config
+import tsugu_api_async
 from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager
 
 
-alc = Alconna(
+async def handler(message: str, user: User, platform: str, channel_id: str):
+    res =  Alconna(
         ["关闭车牌转发", "关闭个人车牌转发"],
         meta=CommandMeta(
             compact=config.compact, description="关闭车牌转发",)
-    )
-
-
-def handler(message: str, user: User, platform: str, channel_id: str):
-    res = alc.parse(message)
+    ).parse(message)
 
     if res.matched:
         update = {'car': False, }
-        r = tsugu_api.change_user_data(platform, user.user_id, update)
+        r = await tsugu_api_async.change_user_data(platform, user.user_id, update)
         if r.get('status') != 'success':
             return text_response(r.get('data'))
         return text_response('关闭车牌转发成功！')
-    elif res.head_matched:
-        return text_response(res.error_info)
-    return None
+    return res
```

### Comparing `tsugu-1.1.0rc3/tsugu/router/remote/switch_car_forwarding_on.py` & `tsugu-1.1.0rc4/tsugu/src/remote/switch_car_forwarding_on.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,20 @@
-from ...utils import text_response, User, server_id_2_server_name, server_name_2_server_id, server_exists
+from ...utils import text_response, User, server_id_2_server_name, server_name_2_server_id, server_exists, config
 import tsugu_api
-from ...config import config
 from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager
 
 
-alc = Alconna(
+def handler(message: str, user: User, platform: str, channel_id: str):
+    res = Alconna(
         ["开启车牌转发", "开启个人车牌转发"],
         meta=CommandMeta(
             compact=config.compact, description="开启车牌转发",)
-    )
-
-
-def handler(message: str, user: User, platform: str, channel_id: str):
-    res = alc.parse(message)
+    ).parse(message)
 
     if res.matched:
         update = {'car': True, }
         r = tsugu_api.change_user_data(platform, user.user_id, update)
         if r.get('status') != 'success':
             return text_response(r.get('data'))
         return text_response('开启车牌转发成功！')
-    elif res.head_matched:
-        return text_response(res.error_info)
-    return None
+    return res
```

### Comparing `tsugu-1.1.0rc3/tsugu/router/remote/unbind_player.py` & `tsugu-1.1.0rc4/tsugu/src/remote/unbind_player.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,22 @@
-from ...utils import text_response, User, server_id_2_server_name, server_name_2_server_id, server_exists
+from ...utils import text_response, User, server_id_2_server_name, server_name_2_server_id, server_exists, config
 import tsugu_api
-from ...config import config
 from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager
-from tsugu_api_core._typing import _ServerName
 
 
-alc = Alconna(
+def handler(message: str, user: User, platform: str, channel_id: str):
+    res = Alconna(
         ["解除绑定"],
-    Args["index#要解绑的绑定编号", int, None],
+        Args["index#要解绑的绑定编号", int, None],
         meta=CommandMeta(
             compact=config.compact, description="解除绑定",
             usage="验证解绑 记录编号(数字)",
             example="验证解绑 1 : 解绑第一个记录"
         ),
-    )
-
-
-def handler(message: str, user: User, platform: str, channel_id: str):
-    res = alc.parse(message)
+    ).parse(message)
 
     if res.matched:
         if not res.index:
             bind_record = '\n'.join([f'{i + 1}. {mask_data(x.get("game_id"))} {server_id_2_server_name(x.get("server"))}' for i, x in enumerate(user.game_ids)])
             return text_response('请输入正确的记录(数字)\n例如: 解除绑定 1\n当前的绑定记录如下:\n' + bind_record)
 
         if len(user.game_ids) < int(res.index):
@@ -29,17 +24,15 @@
 
         server_mode = user.game_ids[int(res.index) - 1].get("server")
 
         r = tsugu_api.bind_player_request(platform, user.user_id, server_mode, False)
         if r.get('status') != 'success':
             return text_response(r.get('data'))
         return text_response(f'''正在解除，请将 评论(个性签名) 或者 当前使用的 乐队编队名称改为\n{r.get('data')['verifyCode']}\n稍等片刻等待同步后，发送\n验证解绑 {res.index}\n来完成本次身份验证''')
-    elif res.head_matched:
-        return text_response(res.error_info)
-    return None
+    return res
 
 
 def mask_data(game_id: str):
     game_id = str(game_id)
     if len(game_id) < 6:
         return game_id[:3] + '*' * (len(game_id) - 3)
     elif len(game_id) < 3:
```

### Comparing `tsugu-1.1.0rc3/tsugu/router/universal/event_stage.py` & `tsugu-1.1.0rc4/tsugu/src/universal/event_stage.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,28 @@
-from ...utils import text_response, User, server_name_2_server_id
+from ...utils import text_response, User, server_id_2_server_name, server_name_2_server_id, server_exists, config
 import tsugu_api
-from ...config import config
 from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager
-from tsugu_api_core._typing import _ServerName
 
 
-alc = Alconna(
+def handler(message: str, user: User, platform: str, channel_id: str):
+    res = Alconna(
         ["查试炼", '查stage', '查舞台', '查festival', '查5v5'],
         Args["eventId;?#省略活动ID时查询当前活动。", [int]]["meta;?#歌曲meta。", ['-m']],
 
         meta=CommandMeta(
             compact=config.compact, description="查试炼",
             usage='查询当前服务器当前活动试炼信息。',
             example='''查试炼 157 -m :返回157号活动的试炼信息，包含歌曲meta。
 查试炼 -m :返回当前活动的试炼信息，包含歌曲meta。
 查试炼 :返回当前活动的试炼信息。'''
         )
-    )
-
-def handler(message: str, user: User, platform: str, channel_id: str):
-    res = alc.parse(message)
+    ).parse(message)
 
     if res.matched:
         if res.meta:
             meta = True
         else:
             meta = False
         print(meta)
         return tsugu_api.event_stage(user.server_mode, res.eventId, meta)
-    elif res.head_matched:
-        return text_response(res.error_info)
-    return None
+
+    return res
```

### Comparing `tsugu-1.1.0rc3/tsugu/router/universal/gacha_simulate.py` & `tsugu-1.1.0rc4/tsugu/src/universal/gacha_simulate.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,26 @@
-from ...utils import text_response, User
+from ...utils import text_response, User, server_id_2_server_name, server_name_2_server_id, server_exists, config
 import tsugu_api
-from ...config import config
 from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager
 
 
-alc = Alconna(
+def handler(message: str, user: User, platform: str, channel_id: str):
+    res = Alconna(
         ["抽卡模拟", "卡池模拟"],
         Args["times", int, 10]['gacha_id;?#如果没有卡池ID的话，卡池为当前活动的卡池。', int],
         meta=CommandMeta(
             compact=config.compact, description="抽卡模拟",
             usage='根据卡片ID查询卡片插画',
             example='抽卡模拟 300 922 :模拟抽卡300次，卡池为922号卡池。'
         )
-    )
-
-
-def handler(message: str, user: User, platform: str, channel_id: str):
-    res = alc.parse(message)
+    ).parse(message)
 
     if res.matched:
         if channel_id in config.disable_gacha_simulate_group_ids:
             return None
         if res.gacha_id:
             gacha_id = res.gacha_id
         else:
             gacha_id = None
         return tsugu_api.gacha_simulate(user.server_mode, res.times, gacha_id)
-    elif res.head_matched:
-        return text_response(res.error_info)
-    return None
+
+    return res
```

### Comparing `tsugu-1.1.0rc3/tsugu/router/universal/get_card_illustration.py` & `tsugu-1.1.0rc4/tsugu/src/universal/search_card.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,23 @@
-from ...utils import text_response, User
+from ...utils import text_response, User, server_id_2_server_name, server_name_2_server_id, server_exists, config
 import tsugu_api
-from ...config import config
-from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager
+from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager, MultiVar
 
 
-alc = Alconna(
-        ["查卡面", "查插画"],
-        Args["cardId", int],
+def handler(message: str, user: User, platform: str, channel_id: str):
+    res = Alconna(
+        ["查卡", "查卡牌"],
+        Args["word#请输入卡面ID，角色等查询参数，使用空格隔开", MultiVar(str)],
         meta=CommandMeta(
-            compact=config.compact, description="查卡面",
-            usage='根据卡片ID查询卡片插画',
-            example='查卡面 1399 :返回1399号卡牌的插画'
+            compact=config.compact, description="查询卡片信息。",
+            usage='根据关键词或卡牌ID查询卡片信息。',
+            example='''查卡 1399 :返回1399号卡牌的信息。
+    查卡面 1399 :返回1399号卡牌的插画。
+    查卡 红 ars 5x :返回角色 ars 的 5x 卡片的信息。'''
         )
-    )
-
-
-def handler(message: str, user: User, platform: str, channel_id: str):
-    res = alc.parse(message)
+    ).parse(message)
 
     if res.matched:
-        return tsugu_api.get_card_illustration(res.cardId)
-    elif res.head_matched:
-        return text_response(res.error_info)
-    return None
+        return tsugu_api.search_card(user.default_server, " ".join(res.word))
+
+    return res
```

### Comparing `tsugu-1.1.0rc3/tsugu/router/universal/lsycx.py` & `tsugu-1.1.0rc4/tsugu/src/universal/ycx_all.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,24 @@
-from ...utils import text_response, User, server_name_2_server_id
+from ...utils import text_response, User, server_id_2_server_name, server_name_2_server_id, server_exists, config
 import tsugu_api
-from ...config import config
 from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager
 from tsugu_api_core._typing import _ServerName
 
 
-alc = Alconna(
-        ["lsycx", "历史预测线"], ['/', ''],
-        Args['tier', int]['eventId;?#活动ID，省略时查询当前活动。', int]
+def handler(message: str, user: User, platform: str, channel_id: str):
+    res = Alconna(
+        ["ycxall", "ycx all"],
+        Args['eventId;?#活动ID，省略时查询当前活动。', int]
             ['serverName#省略服务器名时，默认从你当前的主服务器查询。活动ID不存在时，也可以作为第二个参数。', _ServerName.__args__, None],
         meta=CommandMeta(
-            compact=config.compact, description="查询指定档位的历史预测线。",
-            usage='查询指定档位的预测线与最近的4期活动类型相同的活动的档线数据。',
-            example='''lsycx 1000 :返回默认服务器当前活动的档线与预测线，与最近的4期活动类型相同的活动的档线数据。
-lsycx 1000 177 jp:返回日服177号活动1000档位档线与最近的4期活动类型相同的活动的档线数据。'''
+            compact=config.compact, description="查询指定档位的预测线",
+            usage='根据关键词或角色ID查询角色信息',
+            example='''ycx 1000 :返回默认服务器当前活动1000档位的档线与预测线。
+ycx 1000 177 jp:返回日服177号活动1000档位的档线与预测线。'''
         )
-    )
-
-
-def handler(message: str, user: User, platform: str, channel_id: str):
-    res = alc.parse(message)
+    ).parse(message)
 
     if res.matched:
         server = server_name_2_server_id(res.serverName) if res.serverName else user.server_mode
-        return tsugu_api.lsycx(server, res.tier, res.eventId)
-    elif res.head_matched:
-        return text_response(res.error_info)
-    return None
+        return tsugu_api.ycx_all(server, res.eventId)
+
+    return res
```

### Comparing `tsugu-1.1.0rc3/tsugu/router/universal/search_card.py` & `tsugu-1.1.0rc4/tsugu_async/src/universal/search_card.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,23 @@
-from ...utils import text_response, User
-import tsugu_api
-from ...config import config
+from ...utils import text_response, User, server_id_2_server_name, server_name_2_server_id, server_exists, config
+import tsugu_api_async
 from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager, MultiVar
 
 
-alc = Alconna(
+async def handler(message: str, user: User, platform: str, channel_id: str):
+    res = Alconna(
         ["查卡", "查卡牌"],
         Args["word#请输入卡面ID，角色等查询参数，使用空格隔开", MultiVar(str)],
         meta=CommandMeta(
             compact=config.compact, description="查询卡片信息。",
             usage='根据关键词或卡牌ID查询卡片信息。',
             example='''查卡 1399 :返回1399号卡牌的信息。
-查卡面 1399 :返回1399号卡牌的插画。
-查卡 红 ars 5x :返回角色 ars 的 5x 卡片的信息。'''
+    查卡面 1399 :返回1399号卡牌的插画。
+    查卡 红 ars 5x :返回角色 ars 的 5x 卡片的信息。'''
         )
-    )
-
-
-def handler(message: str, user: User, platform: str, channel_id: str):
-    res = alc.parse(message)
+    ).parse(message)
 
     if res.matched:
-        return tsugu_api.search_card(user.default_server, " ".join(res.word))
-    elif res.head_matched:
-        return text_response(res.error_info)
-    return None
+        return await tsugu_api_async.search_card(user.default_server, " ".join(res.word))
+
+    return res
```

### Comparing `tsugu-1.1.0rc3/tsugu/router/universal/search_character.py` & `tsugu-1.1.0rc4/tsugu/src/remote/bind_player_verification_off.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,29 @@
-from ...utils import text_response, User
+from ...utils import text_response, User, server_id_2_server_name, server_name_2_server_id, server_exists, config
 import tsugu_api
-from ...config import config
-from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, MultiVar
+from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager
 
 
-alc = Alconna(
-        ["查角色"],
-        Args["word#角色名，乐队，昵称等查询参数", MultiVar(str)],
+def handler(message: str, user: User, platform: str, channel_id: str):
+    res = Alconna(
+        ["验证解绑"],
+        Args["index#要解绑的绑定编号", int],
         meta=CommandMeta(
-            compact=config.compact, description="查询角色信息",
-            usage='根据关键词或角色ID查询角色信息',
-            example='''查角色 10 :返回10号角色的信息。
-查角色 吉他 :返回所有角色模糊搜索标签中包含吉他的角色列表。'''
-        )
-    )
+            compact=config.compact, description="验证解绑",
+            usage="验证解绑 记录编号(数字)",
+            example="验证解绑 1 : 解绑第一个记录"
+        ),
+    ).parse(message)
 
+    if res.matched:
+        if len(user.game_ids) < int(res.index):
+            return text_response('未找到记录')
+        player_id = user.game_ids[int(res.index) - 1].get("game_id")
+        server_mode = user.game_ids[int(res.index) - 1].get("server")
+        r = tsugu_api.bind_player_verification(platform, user.user_id, server_mode, player_id, False)
+        if r.get('status') != 'success':
+            return text_response(r.get('data'))
+        return text_response('解绑成功！')
+    
+    return res
 
-def handler(message: str, user: User, platform: str, channel_id: str):
-    res = alc.parse(message)
 
-    if res.matched:
-        return tsugu_api.search_character(user.default_server, " ".join(res.word))
-    elif res.head_matched:
-        return text_response(res.error_info)
-    return None
```

### Comparing `tsugu-1.1.0rc3/tsugu/router/universal/search_event.py` & `tsugu-1.1.0rc4/tsugu/src/universal/search_event.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,24 @@
-from ...utils import text_response, User
+from ...utils import text_response, User, server_id_2_server_name, server_name_2_server_id, server_exists, config
 import tsugu_api
-from ...config import config
 from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, MultiVar
 
 
-alc = Alconna(
+def handler(message: str, user: User, platform: str, channel_id: str):
+    res = Alconna(
         ["查活动"],
         Args["word#请输入活动名，乐队，活动ID等查询参数", MultiVar(str)],
         meta=CommandMeta(
             compact=config.compact, description="查活动",
             usage='根据关键词或活动ID查询活动信息',
             example='''查活动 绿 tsugu :返回所有属性加成为pure，且活动加成角色中包括羽泽鸫的活动列表
 查活动 177 :返回177号活动的信息
 查活动 >225 :查询大于225的活动
 查活动 220-225 :查询220到225的活动'''
         )
-    )
-
-
-def handler(message: str, user: User, platform: str, channel_id: str):
-    res = alc.parse(message)
+    ).parse(message)
 
     if res.matched:
         return tsugu_api.search_event(user.default_server, " ".join(res.word))
-    elif res.head_matched:
-        return text_response(res.error_info)
-    return None
+
+    return res
```

### Comparing `tsugu-1.1.0rc3/tsugu/router/universal/search_gacha.py` & `tsugu-1.1.0rc4/tsugu/src/universal/search_gacha.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,19 @@
-from ...utils import text_response, User
+from ...utils import text_response, User, server_id_2_server_name, server_name_2_server_id, server_exists, config
 import tsugu_api
-from ...config import config
 from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager
 
 
-alc = Alconna(
+def handler(message: str, user: User, platform: str, channel_id: str):
+    res = Alconna(
         ["查卡池"],
         Args["gachaId#可以通过查活动、查卡等获取", str],
         meta=CommandMeta(
             compact=config.compact, description="查卡池",
             usage='根据卡池ID查询卡池信息',
         )
-    )
-
-
-def handler(message: str, user: User, platform: str, channel_id: str):
-    res = alc.parse(message)
+    ).parse(message)
 
     if res.matched:
         return tsugu_api.search_gacha(user.default_server, res.gachaId)
-    elif res.head_matched:
-        return text_response(res.error_info)
-    return None
+
+    return res
```

### Comparing `tsugu-1.1.0rc3/tsugu/router/universal/search_player.py` & `tsugu-1.1.0rc4/tsugu_async/src/universal/search_player.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,28 @@
-from ...utils import text_response, User
+from ...utils import text_response, User, server_id_2_server_name, server_name_2_server_id, server_exists, config
 from tsugu_api_core._typing import _ServerName
-import tsugu_api
-from ...config import config
+import tsugu_api_async
 from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager
 
 
-alc = Alconna(
-    ["查玩家", "查寻玩家"],
-    Args["playerId#你的游戏账号(数字)", int]["serverName;?#省略服务器名时，默认从你当前的主服务器查询。", _ServerName.__args__],
-    meta=CommandMeta(
-        compact=config.compact, description="查询玩家信息",
-        usage='查询指定ID玩家的信息。查询指定ID玩家的信息。',
-        example='查玩家 40474621 jp : 查询日服玩家ID为40474621的玩家信息。\n查玩家 10000000 : 查询你当前默认服务器中，玩家ID为10000000的玩家信息。',
-    )
-)
-
-
-def handler(message: str, user: User, platform: str, channel_id: str):
-    res = alc.parse(message)
+async def handler(message: str, user: User, platform: str, channel_id: str):
+    res = Alconna(
+        ["查玩家", "查寻玩家"],
+        Args["playerId#你的游戏账号(数字)", int]["serverName;?#省略服务器名时，默认从你当前的主服务器查询。", _ServerName.__args__],
+        meta=CommandMeta(
+            compact=config.compact, description="查询玩家信息",
+            usage='查询指定ID玩家的信息。查询指定ID玩家的信息。',
+            example='查玩家 40474621 jp : 查询日服玩家ID为40474621的玩家信息。\n查玩家 10000000 : 查询你当前默认服务器中，玩家ID为10000000的玩家信息。',
+        )
+    ).parse(message)
 
     if res.matched:
         if res.serverName:
             server = res.serverName
         else:
             server = user.server_mode
-        return tsugu_api.search_player(res.playerId, server)
-    elif res.head_matched:
-        return text_response(res.error_info)
-    return None
+        return await tsugu_api_async.search_player(res.playerId, server)
+
+    return res
```

### Comparing `tsugu-1.1.0rc3/tsugu/router/universal/search_song.py` & `tsugu-1.1.0rc4/tsugu/src/universal/search_song.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,25 @@
-from ...utils import text_response, User
+from ...utils import text_response, User, server_id_2_server_name, server_name_2_server_id, server_exists, config
 import tsugu_api
-from ...config import config
 from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, MultiVar
 
 
-alc = Alconna(
+def handler(message: str, user: User, platform: str, channel_id: str):
+    res = Alconna(
         ["查曲"],
         Args["word#歌曲信息，名称，乐队，难度等。", MultiVar(str)],
         meta=CommandMeta(
             compact=config.compact, description="查曲",
             usage='根据关键词或曲目ID查询曲目信息。',
             example='''查曲 1 :返回1号曲的信息
 查曲 ag lv27 :返回所有难度为27的ag曲列表
 查曲 >27 :查询大于27的曲目
 查曲 滑滑蛋 :匹配歌曲 fuwa fuwa time'''
         )
-    )
-
-
-def handler(message: str, user: User, platform: str, channel_id: str):
-    res = alc.parse(message)
+    ).parse(message)
 
     if res.matched:
         return tsugu_api.search_song(user.default_server, " ".join(res.word))
-    elif res.head_matched:
-        return text_response(res.error_info)
-    return None
+
+    return res
```

### Comparing `tsugu-1.1.0rc3/tsugu/router/universal/song_chart.py` & `tsugu-1.1.0rc4/tsugu_async/src/universal/song_chart.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,27 @@
-from ...utils import text_response, User
-import tsugu_api
-from ...config import config
+from ...utils import text_response, User, server_id_2_server_name, server_name_2_server_id, server_exists, config
+import tsugu_api_async
 from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager
 
 
 difficulty_text_tuple = ('easy', 'ez', 'normal', 'nm', 'hard', 'hd', 'expert', 'ex', 'special', 'sp')
 
-alc = Alconna(
+
+async def handler(message: str, user: User, platform: str, channel_id: str):
+    res = Alconna(
         ["查谱面", "查铺面"],
         Args["songId", int]['difficultyText', difficulty_text_tuple, 'ex'],
         meta=CommandMeta(
             compact=config.compact, description="查谱面",
             usage='根据曲目ID与难度查询铺面信息。',
             example='''查谱面 1 :返回1号曲的ex难度谱面
 查谱面 128 special :返回128号曲的special难度谱面'''
         )
-    )
-
-
-def handler(message: str, user: User, platform: str, channel_id: str):
-    res = alc.parse(message)
+    ).parse(message)
 
     if res.matched:
-        return tsugu_api.song_chart(user.default_server, res.songId, res.difficultyText)
-    elif res.head_matched:
-        return text_response(res.error_info)
-    return None
+        return await tsugu_api_async.song_chart(user.default_server, res.songId, res.difficultyText)
+
+    return res
```

### Comparing `tsugu-1.1.0rc3/tsugu/router/universal/song_meta.py` & `tsugu-1.1.0rc4/tsugu_async/src/universal/song_meta.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,26 @@
-from ...utils import text_response, User, server_name_2_server_id
-import tsugu_api
-from ...config import config
+from ...utils import text_response, User, server_id_2_server_name, server_name_2_server_id, server_exists, config
+import tsugu_api_async
 from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager
 from tsugu_api_core._typing import _ServerName
 
 
-alc = Alconna(
+async def handler(message: str, user: User, platform: str, channel_id: str):
+    res = Alconna(
         ["查询分数表", '查分数表', '查询分数榜', '查分数榜'],
         Args["serverName;?#省略服务器名时，默认从你当前的主服务器查询。", _ServerName.__args__],
         meta=CommandMeta(
             compact=config.compact, description="查询分数表",
             usage='查询指定服务器的歌曲分数表。',
             example='''查询分数表 cn :返回国服的歌曲分数表'''
         )
-    )
-
-
-def handler(message: str, user: User, platform: str, channel_id: str):
-    res = alc.parse(message)
+    ).parse(message)
 
     if res.matched:
         if res.serverName:
             server = server_name_2_server_id(res.serverName)
         else:
             server = user.server_mode
-        return tsugu_api.song_meta(user.default_server, server)
-    elif res.head_matched:
-        return text_response(res.error_info)
-    return None
+        return await tsugu_api_async.song_meta(user.default_server, server)
+
+    return res
```

### Comparing `tsugu-1.1.0rc3/tsugu/router/universal/ycx.py` & `tsugu-1.1.0rc4/tsugu_async/src/universal/ycx_all.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,24 @@
-from ...utils import text_response, User, server_name_2_server_id
-import tsugu_api
-from ...config import config
+from ...utils import text_response, User, server_id_2_server_name, server_name_2_server_id, server_exists, config
+import tsugu_api_async
 from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager
 from tsugu_api_core._typing import _ServerName
 
 
-alc = Alconna(
-        ["ycx", "预测线"],
-        Args['tier', int]['eventId;?#活动ID，省略时查询当前活动。', int]
+async def handler(message: str, user: User, platform: str, channel_id: str):
+    res = Alconna(
+        ["ycxall", "ycx all"],
+        Args['eventId;?#活动ID，省略时查询当前活动。', int]
             ['serverName#省略服务器名时，默认从你当前的主服务器查询。活动ID不存在时，也可以作为第二个参数。', _ServerName.__args__, None],
         meta=CommandMeta(
             compact=config.compact, description="查询指定档位的预测线",
-            usage='查询指定档位的预测线。',
+            usage='根据关键词或角色ID查询角色信息',
             example='''ycx 1000 :返回默认服务器当前活动1000档位的档线与预测线。
 ycx 1000 177 jp:返回日服177号活动1000档位的档线与预测线。'''
         )
-    )
-
-
-def handler(message: str, user: User, platform: str, channel_id: str):
-    res = alc.parse(message)
+    ).parse(message)
 
     if res.matched:
         server = server_name_2_server_id(res.serverName) if res.serverName else user.server_mode
-        return tsugu_api.ycx(server, res.tier, res.eventId)
-    elif res.head_matched:
-        return text_response(res.error_info)
-    return None
+        return await tsugu_api_async.ycx_all(server, res.eventId)
 
+    return res
```

### Comparing `tsugu-1.1.0rc3/tsugu/router/universal/ycx_all.py` & `tsugu-1.1.0rc4/tsugu/src/remote/bind_player.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,24 @@
-from ...utils import text_response, User, server_name_2_server_id
+from ...utils import config, text_response, User, server_id_2_server_name, server_name_2_server_id, server_exists
 import tsugu_api
-from ...config import config
-from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager
-from tsugu_api_core._typing import _ServerName
-from typing import List, Tuple, Dict, Any, Union
-
-alc = Alconna(
-        ["ycxall", "ycx all"],
-        Args['eventId;?#活动ID，省略时查询当前活动。', int]
-            ['serverName#省略服务器名时，默认从你当前的主服务器查询。活动ID不存在时，也可以作为第二个参数。', _ServerName.__args__, None],
-        meta=CommandMeta(
-            compact=config.compact, description="查询指定档位的预测线",
-            usage='根据关键词或角色ID查询角色信息',
-            example='''ycx 1000 :返回默认服务器当前活动1000档位的档线与预测线。
-ycx 1000 177 jp:返回日服177号活动1000档位的档线与预测线。'''
-        )
-    )
+from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager, MultiVar, AllParam
 
 
 def handler(message: str, user: User, platform: str, channel_id: str):
-    res = alc.parse(message)
+    res = Alconna(
+        ["绑定玩家"],
+    Args["args;?", AllParam],
+    meta=CommandMeta(
+            compact=config.compact, description="绑定玩家",
+            usage="只需发送‘绑定玩家’。",
+        ),
+    ).parse(message)
 
     if res.matched:
-        server = server_name_2_server_id(res.serverName) if res.serverName else user.server_mode
-        return tsugu_api.ycx_all(server, res.eventId)
-    elif res.head_matched:
-        return text_response(res.error_info)
-    return None
+        r = tsugu_api.bind_player_request(platform, user.user_id, user.server_mode, False)
+        if r.get('status') != 'success':
+            return text_response(r.get('data'))
+        return text_response(
+            f'''正在绑定账号，请将 评论(个性签名) 或者 当前使用的 乐队编队名称改为\n{r.get('data')['verifyCode']}\n稍等片刻等待同步后，发送\n验证绑定 你的玩家ID(数字) 服务器名(字母缩写)\n例如：验证绑定 114****514 cn''')
+
+    return res
+
```

### Comparing `tsugu-1.1.0rc3/tsugu/utils/__init__.py` & `tsugu-1.1.0rc4/tsugu/utils/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import typing
 from typing import List
-
-from ..config import config
 import tsugu_api
 from loguru import logger
 import time
+from ..config import config
 
 from tsugu_api_core._typing import _ServerId
 
 
 _i_s = {0: "jp", 1: "en", 2: "tw", 3: "cn", 4: "kr"}
 _s_i = {"jp": 0, "en": 1, "tw": 2, "cn": 3, "kr": 4}
```

### Comparing `tsugu-1.1.0rc3/tsugu.egg-info/PKG-INFO` & `tsugu-1.1.0rc4/tsugu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu
-Version: 1.1.0rc3
+Version: 1.1.0rc4
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
-Metadata-Version: 2.1 Name: tsugu Version: 1.1.0rc3 Summary: Tsugu Python
+Metadata-Version: 2.1 Name: tsugu Version: 1.1.0rc4 Summary: Tsugu Python
 Frontend Home-page: https://github.com/kumoSleeping/ChatTsuguPy Author:
 kumoSleeping Author-email: zjr2992@outlook.com License: MIT Description:
                        ************ CChhaatt TTssuugguu PPyy[[ttmmrrnn]] ************
 _â¨ Python ç¼åç [TsuguBanGDreamBot](https://github.com/Yamamoto-2/tsugu-
          bangdream-bot?tab=readme-ov-file) èªç¶è¯­è¨äº¤äºåº â¨_
                           _[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]
 --- ```shell pip install tsugu ``` > API powered by _t_s_u_g_u_-_a_p_i_-_p_y_t_h_o_n > Command
```

### Comparing `tsugu-1.1.0rc3/tsugu_async/handler.py` & `tsugu-1.1.0rc4/tsugu_async/handler.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import base64
 from typing import List, Union, Dict
 
 from .utils import *
 from loguru import logger
 from tsugu_api import settings
-from . import router
+from . import src
 
 
 async def handler(message: str, user_id: str, platform: str, channel_id: str) -> List[Union[bytes, str]]:
     '''
     Tsugu Handler
     处理用户输入的自然语言，返回处理后的结果
 
@@ -39,15 +39,15 @@
     :param user_id: 用户ID
     :param platform: 平台名称 一般为 red
     :param channel_id: 频道ID / 群号
     :return: List[Dict[str, str]]
     '''
     try:
         # 使用远程服务器
-        res = await router.handler(message, user_id, platform, channel_id)
+        res = await src.handler(message, user_id, platform, channel_id)
         if not res:
             return []
         return res
     except Exception as e:
         logger.error(f'Error: {e}')
         raise e
```

### Comparing `tsugu-1.1.0rc3/tsugu_async/router/__init__.py` & `tsugu-1.1.0rc4/tsugu/src/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,13 @@
 import importlib
-from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, output_manager, command_manager
+from arclet.alconna import Arparma, output_manager, command_manager
 from ..utils import text_response, get_user
-from contextvars import ContextVar
-from typing import Optional
-
-
-def require(module_path, cmd):
-    globals()[cmd] = importlib.import_module(module_path.format(cmd=cmd), __package__)
 
 
+# 主要功能
 universal_list = [
     "get_card_illustration",
     "search_player",
     "gacha_simulate",
     "search_gacha",
     "search_event",
     "search_song",
@@ -22,68 +17,71 @@
     "ycx_all",
     "ycx",
     "lsycx",
     "search_card",
     "event_stage",
 ]
 
+# 远程数据库相关功能
 remote_commands = [
     "player_status",
     "switch_car_forwarding_off",
     "switch_car_forwarding_on",
     "bind_player",
     "unbind_player",
     "change_server_mode",
     "change_default_server",
     "bind_player_verification_off",
     "bind_player_verification_on",
 ]
 
-
+# BandoriStation 相关功能
 bandoristation_commands = [
     "ycm",
     "rooms_forward",
 ]
 
-# 导入模块
-[require(f'.universal.{cmd}', cmd) for cmd in universal_list]
-[require(f'.remote.{cmd}', cmd) for cmd in remote_commands]
-[require(f'.bandoristation.{cmd}', cmd) for cmd in bandoristation_commands]
+# 帮助信息
+help_command = [
+    "help",
+]
 
 
-this_value_h: ContextVar[Optional[str]] = ContextVar('this_value_h', default=None)
+def require(module_path, cmd):
+    globals()[cmd] = importlib.import_module(module_path.format(cmd=cmd), __package__)
 
 
-async def handler(message, user_id, platform, channel_id):
-    user = await get_user(user_id, platform)
+# 导入模块
+[require(f'.universal.{cmd}', cmd) for cmd in universal_list]
+[require(f'.remote.{cmd}', cmd) for cmd in remote_commands]
+[require(f'.bandoristation.{cmd}', cmd) for cmd in bandoristation_commands]
+[require(f'.help.{cmd}', cmd) for cmd in help_command]
 
-    def set_output_str(arg):
-        this_value_h.set(arg)
 
-    output_manager.set_action(set_output_str)
+def handler(message, user_id, platform, channel_id):
+    user = get_user(user_id, platform)
+    output_manager.set_action(lambda *_: None)
+    union_list = universal_list + remote_commands + bandoristation_commands + help_command
+
+    for i in union_list:
+        result = getattr(globals()[i], 'handler')(message, user, platform, channel_id)
+
+        # 未生成结果
+        if isinstance(result, Arparma):
+            # 匹配了命令头
+            if result.head_matched:
+
+                # 帮助信息
+                if result.error_data == ['-h']:
+                    return getattr(globals()['help'], 'handler')('help ' + result.header_result, user, platform, channel_id)
+                # 错误信息
+                else:
+                    return text_response(result.error_info)
 
-    async def handler_feats(cmd_list):
-        for i in cmd_list:
-            result = await getattr(globals()[i], 'handler')(message, user, platform, channel_id)
-            if not result:
-                continue
-            if result[0].get('type') == 'string' and result[0].get('string') == 'help':
-                return text_response(this_value_h.get())
+        # 已生成结果
+        if isinstance(result, list):
             return result
-        return None
 
-    res = await handler_feats(universal_list)
-    if res:
-        return res
-
-    res = await handler_feats(remote_commands)
-    if res:
-        return res
-
-    res = await handler_feats(bandoristation_commands)
-    if res:
-        return res
+    return None
+
 
-    if message in ["help", "帮助"]:
-        return text_response(command_manager.all_command_help(show_index=True) + "例如: 查卡 -h")
 
-    return None
```

### Comparing `tsugu-1.1.0rc3/tsugu_async/router/bandoristation/rooms_forward.py` & `tsugu-1.1.0rc4/tsugu_async/src/bandoristation/rooms_forward.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,65 +1,61 @@
 from ...utils import text_response, User, get_user
 import tsugu_api_async
-from ...config import config
 from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager
 import re
 
 
 # 虚空注册
-alc = Alconna(
-        ["上传车牌"],
-        meta=CommandMeta(
-            compact=config.compact, description="上传车牌",
-        )
-    )
+alc = Alconna(["上传车牌"],meta=CommandMeta(description="上传车牌",))
 
 
 async def handler(message: str, user: User, platform: str, channel_id: str):
     if message.startswith("上传车牌"):
         message = message[4:].strip()
 
     # 检查car_config['car']中的关键字
     for keyword in _car_config["car"]:
         if str(keyword) in message:
             break
     else:
-        return []
+        return None
 
     # 检查car_config['fake']中的关键字
     for keyword in _car_config["fake"]:
         if str(keyword) in message:
-            return []
+            return None
 
     pattern = r"^\d{5}(\D|$)|^\d{6}(\D|$)"
     if not re.match(pattern, message):
-        return []
+        return None
+
+    user = get_user(user.user_id, platform)
 
     # 获取用户数据
     try:
         if platform:
             if not user.car:
-                return []
+                return None
     except Exception as e:
         # 默认不开启关闭车牌，继续提交
         pass
 
     try:
         car_id = message[:6]
         if not car_id.isdigit() and car_id[:5].isdigit():
             car_id = car_id[:5]
         if user.user_id.isdigit():
             car_user_id = user.user_id
         else:
             car_user_id = '3889000770'
         await tsugu_api_async.submit_room_number(number=int(car_id), user_id=car_user_id, raw_message=message, source=config.bandori_station_token_name, token=config.bandori_station_token)
-        return []
+        return None
 
     except Exception as e:
-        return []
+        return None
 
 
 _car_config = {
     "car": [
         "q1",
         "q2",
         "q3",
```

### Comparing `tsugu-1.1.0rc3/tsugu_async/router/bandoristation/ycm.py` & `tsugu-1.1.0rc4/tsugu_async/src/bandoristation/ycm.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,23 @@
-from ...utils import text_response, User
+from ...utils import text_response, User, config
 import tsugu_api_async
-from ...config import config
 from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager
 
 
-alc = Alconna(
+async def handler(message: str, user: User, platform: str, channel_id: str):
+    res = Alconna(
         ["ycm", "车来", "有车吗"],
         meta=CommandMeta(
             compact=config.compact, description="获取车牌",
         )
-    )
-
-
-async def handler(message: str, user: User, platform: str, channel_id: str):
-    res = alc.parse(message)
+    ).parse(message)
 
     if res.matched:
-        return await car_search()
-    elif res.head_matched:
-        return text_response(res.error_info)
-    return None
+        return car_search()
+    return res
 
 
 async def car_search():
     try:
         data = await tsugu_api_async.query_room_number()
     except Exception as e:
         return text_response('获取房间信息失败，请稍后再试')
```

### Comparing `tsugu-1.1.0rc3/tsugu_async/router/remote/bind_player.py` & `tsugu-1.1.0rc4/tsugu/src/universal/ycx.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,25 @@
-from ...utils import text_response, User, server_id_2_server_name, server_name_2_server_id, server_exists
-import tsugu_api_async
-from ...config import config
-from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager, MultiVar, AllParam
+from ...utils import text_response, User, server_id_2_server_name, server_name_2_server_id, server_exists, config
+import tsugu_api
+from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager
 from tsugu_api_core._typing import _ServerName
 
 
-alc = Alconna(
-        ["绑定玩家"],
-    Args["args;?", AllParam],
-    meta=CommandMeta(
-            compact=config.compact, description="绑定玩家",
-            usage="只需发送‘绑定玩家’。",
-        ),
-    )
-
-
-async def handler(message: str, user: User, platform: str, channel_id: str):
-    res = alc.parse(message)
+def handler(message: str, user: User, platform: str, channel_id: str):
+    res = Alconna(
+        ["ycx", "预测线"],
+        Args['tier', int]['eventId;?#活动ID，省略时查询当前活动。', int]
+            ['serverName#省略服务器名时，默认从你当前的主服务器查询。活动ID不存在时，也可以作为第二个参数。', _ServerName.__args__, None],
+        meta=CommandMeta(
+            compact=config.compact, description="查询指定档位的预测线",
+            usage='查询指定档位的预测线。',
+            example='''ycx 1000 :返回默认服务器当前活动1000档位的档线与预测线。
+ycx 1000 177 jp:返回日服177号活动1000档位的档线与预测线。'''
+        )
+    ).parse(message)
 
     if res.matched:
-        r = await tsugu_api_async.bind_player_request(platform, user.user_id, user.server_mode, False)
-        if r.get('status') != 'success':
-            return text_response(r.get('data'))
-        return text_response(
-            f'''正在绑定账号，请将 评论(个性签名) 或者 当前使用的 乐队编队名称改为\n{r.get('data')['verifyCode']}\n稍等片刻等待同步后，发送\n验证绑定 你的玩家ID(数字) 服务器名(字母缩写)\n例如：验证绑定 114****514 cn''')
-    elif res.head_matched:
-        return text_response(res.error_info)
-    return None
+        server = server_name_2_server_id(res.serverName) if res.serverName else user.server_mode
+        return tsugu_api.ycx(server, res.tier, res.eventId)
+
+    return res
```

### Comparing `tsugu-1.1.0rc3/tsugu_async/router/remote/bind_player_verification_on.py` & `tsugu-1.1.0rc4/tsugu_async/src/universal/ycx.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,25 @@
-from ...utils import text_response, User, server_id_2_server_name, server_name_2_server_id, server_exists
+from ...utils import text_response, User, server_id_2_server_name, server_name_2_server_id, server_exists, config
 import tsugu_api_async
-from ...config import config
 from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager
 from tsugu_api_core._typing import _ServerName
 
-alc = Alconna(
-        ["验证绑定"],
-    Args["playerID#你的玩家ID(数字)", int]["serverName#服务器名(字母缩写)", _ServerName],
-        meta=CommandMeta(
-            compact=config.compact, description="验证绑定",)
-    )
-
 
 async def handler(message: str, user: User, platform: str, channel_id: str):
-    res = alc.parse(message)
+    res = Alconna(
+        ["ycx", "预测线"],
+        Args['tier', int]['eventId;?#活动ID，省略时查询当前活动。', int]
+            ['serverName#省略服务器名时，默认从你当前的主服务器查询。活动ID不存在时，也可以作为第二个参数。', _ServerName.__args__, None],
+        meta=CommandMeta(
+            compact=config.compact, description="查询指定档位的预测线",
+            usage='查询指定档位的预测线。',
+            example='''ycx 1000 :返回默认服务器当前活动1000档位的档线与预测线。
+ycx 1000 177 jp:返回日服177号活动1000档位的档线与预测线。'''
+        )
+    ).parse(message)
 
     if res.matched:
-        server = server_name_2_server_id(res.serverName)
-        r = await tsugu_api_async.bind_player_verification(platform, user.user_id, server, res.playerID, True)
-        if r.get('status') != 'success':
-            return text_response(r.get('data'))
-        return text_response('绑定成功！现在可以使用 玩家状态 {len(user.game_ids) + 1} 查看绑定的玩家状态')
-    elif res.head_matched:
-        return text_response(res.error_info)
-    return None
+        server = server_name_2_server_id(res.serverName) if res.serverName else user.server_mode
+        return await tsugu_api_async.ycx(server, res.tier, res.eventId)
+
+    return res
+
```

### Comparing `tsugu-1.1.0rc3/tsugu_async/router/remote/change_default_server.py` & `tsugu-1.1.0rc4/tsugu_async/src/remote/change_default_server.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,28 +1,24 @@
-from ...utils import text_response, User, server_names_2_server_ids
+from ...utils import text_response, User, server_id_2_server_name, server_names_2_server_ids, server_exists, config
 import tsugu_api_async
-from ...config import config
 from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager, MultiVar
 from tsugu_api_core._typing import _ServerName
 
-alc = Alconna(
+
+async def handler(message: str, user: User, platform: str, channel_id: str):
+    res = Alconna(
         ["设置默认服务器", "默认服务器"],
-    Args["serverList#使用空格分隔服务器列表。", MultiVar(_ServerName)],
+        Args["serverList#使用空格分隔服务器列表。", MultiVar(_ServerName)],
         meta=CommandMeta(
             compact=config.compact, description="设定信息显示中的默认服务器排序",
             example="""设置默认服务器 cn jp : 将国服设置为第一服务器，日服设置为第二服务器。"""
 
         )
-    )
-
-
-async def handler(message: str, user: User, platform: str, channel_id: str):
-    res = alc.parse(message)
+    ).parse(message)
 
     if res.matched:
         r = await tsugu_api_async.change_user_data(platform, user.user_id, {'default_server': server_names_2_server_ids(res.serverList)})
         if r.get('status') != 'success':
             return text_response(r.get('data'))
         return text_response('默认服务器已设置为 ' + ' '.join(res.serverList))
-    elif res.head_matched:
-        return text_response(res.error_info)
-    return None
+    
+    return res
```

### Comparing `tsugu-1.1.0rc3/tsugu_async/router/remote/change_server_mode.py` & `tsugu-1.1.0rc4/tsugu/src/remote/change_default_server.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,24 @@
-from ...utils import text_response, User, server_name_2_server_id
-import tsugu_api_async
-from ...config import config
+from ...utils import text_response, User, server_id_2_server_name, server_names_2_server_ids, server_exists, config
+import tsugu_api
 from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager, MultiVar
 from tsugu_api_core._typing import _ServerName
 
-alc = Alconna(
-        ["主服务器", "设置主服务器"],
-    Args["serverName#服务器名", _ServerName],
+
+def handler(message: str, user: User, platform: str, channel_id: str):
+    res = Alconna(
+        ["设置默认服务器", "默认服务器"],
+        Args["serverList#使用空格分隔服务器列表。", MultiVar(_ServerName)],
         meta=CommandMeta(
-            compact=config.compact, description="主服务器",
-            usage="将指定的服务器设置为你的主服务器。",
-            example="""主服务器 cn : 将国服设置为主服务器。"""
+            compact=config.compact, description="设定信息显示中的默认服务器排序",
+            example="""设置默认服务器 cn jp : 将国服设置为第一服务器，日服设置为第二服务器。"""
 
         )
-    )
-
-
-async def handler(message: str, user: User, platform: str, channel_id: str):
-    res = alc.parse(message)
+    ).parse(message)
 
     if res.matched:
-        r = await tsugu_api_async.change_user_data(platform, user.user_id, {'server_mode': server_name_2_server_id(res.serverName)})
+        r = tsugu_api.change_user_data(platform, user.user_id, {'default_server': server_names_2_server_ids(res.serverList)})
         if r.get('status') != 'success':
             return text_response(r.get('data'))
-        return text_response('主服务器已设置为 ' + res.serverName)
-    elif res.head_matched:
-        return text_response(res.error_info)
-    return None
-
-#
-# def handler(user: User, res: MC, platform: str, channel_id: str):
-#     if res.args:
-#         server_mode = server_name_2_server_id(res.args[0])
-#         if not server_exists(server_mode):
-#             return text_response('未找到服务器，请输入正确的服务器名')
-#         update: _Update = {'server_mode': server_mode, }
-#         if r := tsugu_api.change_user_data(platform, user.user_id, update):
-#             if r.get('status') == 'success':
-#                 return text_response('主服务器已设置为 ' + server_id_2_server_name(server_mode))
-#             return text_response(r.get('data'))
-#
+        return text_response('默认服务器已设置为 ' + ' '.join(res.serverList))
+    
+    return res
```

### Comparing `tsugu-1.1.0rc3/tsugu_async/router/remote/switch_car_forwarding_off.py` & `tsugu-1.1.0rc4/tsugu_async/src/remote/switch_car_forwarding_on.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,20 @@
-from ...utils import text_response, User, server_id_2_server_name, server_name_2_server_id, server_exists
+from ...utils import text_response, User, server_id_2_server_name, server_name_2_server_id, server_exists, config
 import tsugu_api_async
-from ...config import config
 from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager
 
 
-alc = Alconna(
-        ["关闭车牌转发", "关闭个人车牌转发"],
-        meta=CommandMeta(
-            compact=config.compact, description="关闭车牌转发",)
-    )
-
-
 async def handler(message: str, user: User, platform: str, channel_id: str):
-    res = alc.parse(message)
+    res = Alconna(
+        ["开启车牌转发", "开启个人车牌转发"],
+        meta=CommandMeta(
+            compact=config.compact, description="开启车牌转发",)
+    ).parse(message)
 
     if res.matched:
-        update = {'car': False, }
+        update = {'car': True, }
         r = await tsugu_api_async.change_user_data(platform, user.user_id, update)
         if r.get('status') != 'success':
             return text_response(r.get('data'))
-        return text_response('关闭车牌转发成功！')
-    elif res.head_matched:
-        return text_response(res.error_info)
-    return None
+        return text_response('开启车牌转发成功！')
+    return res
```

### Comparing `tsugu-1.1.0rc3/tsugu_async/router/remote/switch_car_forwarding_on.py` & `tsugu-1.1.0rc4/tsugu/src/help/help.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,29 @@
-from ...utils import text_response, User, server_id_2_server_name, server_name_2_server_id, server_exists
-import tsugu_api_async
-from ...config import config
-from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager
+from ...utils import config, text_response, User, server_id_2_server_name, server_name_2_server_id, server_exists
+from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager, MultiVar, AllParam
 
 
-alc = Alconna(
-        ["开启车牌转发", "开启个人车牌转发"],
+def handler(message: str, user: User, platform: str, channel_id: str):
+    res = Alconna(
+        ["help"],
+        Args["cmd;?#命令", str],
         meta=CommandMeta(
-            compact=config.compact, description="开启车牌转发",)
-    )
+            compact=config.compact, description="Chat Tsugu Py 帮助",)
+    ).parse(message)
 
+    if res.matched:
+        if not res.cmd:
+            return text_response(command_manager.all_command_help())
 
-async def handler(message: str, user: User, platform: str, channel_id: str):
-    res = alc.parse(message)
+        try:
+            cmd = command_manager.command_help(res.cmd)
+            return text_response(cmd)
+
+        except KeyError:
+            # return text_response('未找到该命令')
+            return None
+
+        except Exception as e:
+            # return text_response('未知错误')
+            return None
 
-    if res.matched:
-        update = {'car': True, }
-        r = await tsugu_api_async.change_user_data(platform, user.user_id, update)
-        if r.get('status') != 'success':
-            return text_response(r.get('data'))
-        return text_response('开启车牌转发成功！')
-    elif res.head_matched:
-        return text_response(res.error_info)
     return None
-
```

### Comparing `tsugu-1.1.0rc3/tsugu_async/router/remote/unbind_player.py` & `tsugu-1.1.0rc4/tsugu_async/src/remote/unbind_player.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,22 @@
-from ...utils import text_response, User, server_id_2_server_name, server_name_2_server_id, server_exists
+from ...utils import text_response, User, server_id_2_server_name, server_name_2_server_id, server_exists, config
 import tsugu_api_async
-from ...config import config
 from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager
-from tsugu_api_core._typing import _ServerName
 
 
-alc = Alconna(
+async def handler(message: str, user: User, platform: str, channel_id: str):
+    res = Alconna(
         ["解除绑定"],
-    Args["index#要解绑的绑定编号", int, None],
+        Args["index#要解绑的绑定编号", int, None],
         meta=CommandMeta(
             compact=config.compact, description="解除绑定",
             usage="验证解绑 记录编号(数字)",
             example="验证解绑 1 : 解绑第一个记录"
         ),
-    )
-
-
-async def handler(message: str, user: User, platform: str, channel_id: str):
-    res = alc.parse(message)
+    ).parse(message)
 
     if res.matched:
         if not res.index:
             bind_record = '\n'.join([f'{i + 1}. {mask_data(x.get("game_id"))} {server_id_2_server_name(x.get("server"))}' for i, x in enumerate(user.game_ids)])
             return text_response('请输入正确的记录(数字)\n例如: 解除绑定 1\n当前的绑定记录如下:\n' + bind_record)
 
         if len(user.game_ids) < int(res.index):
@@ -29,17 +24,15 @@
 
         server_mode = user.game_ids[int(res.index) - 1].get("server")
 
         r = await tsugu_api_async.bind_player_request(platform, user.user_id, server_mode, False)
         if r.get('status') != 'success':
             return text_response(r.get('data'))
         return text_response(f'''正在解除，请将 评论(个性签名) 或者 当前使用的 乐队编队名称改为\n{r.get('data')['verifyCode']}\n稍等片刻等待同步后，发送\n验证解绑 {res.index}\n来完成本次身份验证''')
-    elif res.head_matched:
-        return text_response(res.error_info)
-    return None
+    return res
 
 
 def mask_data(game_id: str):
     game_id = str(game_id)
     if len(game_id) < 6:
         return game_id[:3] + '*' * (len(game_id) - 3)
     elif len(game_id) < 3:
```

### Comparing `tsugu-1.1.0rc3/tsugu_async/router/universal/event_stage.py` & `tsugu-1.1.0rc4/tsugu_async/src/universal/event_stage.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,33 +1,28 @@
-from ...utils import text_response, User, server_name_2_server_id
+from ...utils import text_response, User, server_id_2_server_name, server_name_2_server_id, server_exists, config
 import tsugu_api_async
-from ...config import config
 from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager
-from tsugu_api_core._typing import _ServerName
 
 
-alc = Alconna(
+async def handler(message: str, user: User, platform: str, channel_id: str):
+    res = Alconna(
         ["查试炼", '查stage', '查舞台', '查festival', '查5v5'],
         Args["eventId;?#省略活动ID时查询当前活动。", [int]]["meta;?#歌曲meta。", ['-m']],
 
         meta=CommandMeta(
             compact=config.compact, description="查试炼",
             usage='查询当前服务器当前活动试炼信息。',
             example='''查试炼 157 -m :返回157号活动的试炼信息，包含歌曲meta。
 查试炼 -m :返回当前活动的试炼信息，包含歌曲meta。
 查试炼 :返回当前活动的试炼信息。'''
         )
-    )
-
-async def handler(message: str, user: User, platform: str, channel_id: str):
-    res = alc.parse(message)
+    ).parse(message)
 
     if res.matched:
         if res.meta:
             meta = True
         else:
             meta = False
         print(meta)
         return await tsugu_api_async.event_stage(user.server_mode, res.eventId, meta)
-    elif res.head_matched:
-        return text_response(res.error_info)
-    return None
+
+    return res
```

### Comparing `tsugu-1.1.0rc3/tsugu_async/router/universal/gacha_simulate.py` & `tsugu-1.1.0rc4/tsugu_async/src/universal/gacha_simulate.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,31 +1,26 @@
-from ...utils import text_response, User
+from ...utils import text_response, User, server_id_2_server_name, server_name_2_server_id, server_exists, config
 import tsugu_api_async
-from ...config import config
 from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager
 
 
-alc = Alconna(
+async def handler(message: str, user: User, platform: str, channel_id: str):
+    res = Alconna(
         ["抽卡模拟", "卡池模拟"],
         Args["times", int, 10]['gacha_id;?#如果没有卡池ID的话，卡池为当前活动的卡池。', int],
         meta=CommandMeta(
             compact=config.compact, description="抽卡模拟",
             usage='根据卡片ID查询卡片插画',
             example='抽卡模拟 300 922 :模拟抽卡300次，卡池为922号卡池。'
         )
-    )
-
-
-async def handler(message: str, user: User, platform: str, channel_id: str):
-    res = alc.parse(message)
+    ).parse(message)
 
     if res.matched:
         if channel_id in config.disable_gacha_simulate_group_ids:
             return None
         if res.gacha_id:
             gacha_id = res.gacha_id
         else:
             gacha_id = None
         return await tsugu_api_async.gacha_simulate(user.server_mode, res.times, gacha_id)
-    elif res.head_matched:
-        return text_response(res.error_info)
-    return None
+
+    return res
```

### Comparing `tsugu-1.1.0rc3/tsugu_async/router/universal/get_card_illustration.py` & `tsugu-1.1.0rc4/tsugu_async/src/universal/search_character.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,21 @@
-from ...utils import text_response, User
+from ...utils import text_response, User, server_id_2_server_name, server_name_2_server_id, server_exists, config
 import tsugu_api_async
-from ...config import config
-from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager
+from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, MultiVar
 
 
-alc = Alconna(
-        ["查卡面", "查插画"],
-        Args["cardId", int],
+async def handler(message: str, user: User, platform: str, channel_id: str):
+    res = Alconna(
+        ["查角色"],
+        Args["word#角色名，乐队，昵称等查询参数", MultiVar(str)],
         meta=CommandMeta(
-            compact=config.compact, description="查卡面",
-            usage='根据卡片ID查询卡片插画',
-            example='查卡面 1399 :返回1399号卡牌的插画'
+            compact=config.compact, description="查询角色信息",
+            usage='根据关键词或角色ID查询角色信息',
+            example='''查角色 10 :返回10号角色的信息。
+查角色 吉他 :返回所有角色模糊搜索标签中包含吉他的角色列表。'''
         )
-    )
-
-
-async def handler(message: str, user: User, platform: str, channel_id: str):
-    res = alc.parse(message)
+    ).parse(message)
 
     if res.matched:
-        return await tsugu_api_async.get_card_illustration(res.cardId)
-    elif res.head_matched:
-        return text_response(res.error_info)
-    return None
+        return await tsugu_api_async.search_character(user.default_server, " ".join(res.word))
 
+    return res
```

### Comparing `tsugu-1.1.0rc3/tsugu_async/router/universal/lsycx.py` & `tsugu-1.1.0rc4/tsugu_async/src/universal/lsycx.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,24 @@
-from ...utils import text_response, User, server_name_2_server_id
+from ...utils import text_response, User, server_id_2_server_name, server_name_2_server_id, server_exists, config
 import tsugu_api_async
-from ...config import config
 from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager
 from tsugu_api_core._typing import _ServerName
 
 
-alc = Alconna(
+async def handler(message: str, user: User, platform: str, channel_id: str):
+    res = Alconna(
         ["lsycx", "历史预测线"], ['/', ''],
         Args['tier', int]['eventId;?#活动ID，省略时查询当前活动。', int]
             ['serverName#省略服务器名时，默认从你当前的主服务器查询。活动ID不存在时，也可以作为第二个参数。', _ServerName.__args__, None],
         meta=CommandMeta(
             compact=config.compact, description="查询指定档位的历史预测线。",
             usage='查询指定档位的预测线与最近的4期活动类型相同的活动的档线数据。',
             example='''lsycx 1000 :返回默认服务器当前活动的档线与预测线，与最近的4期活动类型相同的活动的档线数据。
 lsycx 1000 177 jp:返回日服177号活动1000档位档线与最近的4期活动类型相同的活动的档线数据。'''
         )
-    )
-
-
-async def handler(message: str, user: User, platform: str, channel_id: str):
-    res = alc.parse(message)
+    ).parse(message)
 
     if res.matched:
         server = server_name_2_server_id(res.serverName) if res.serverName else user.server_mode
         return await tsugu_api_async.lsycx(server, res.tier, res.eventId)
-    elif res.head_matched:
-        return text_response(res.error_info)
-    return None
+
+    return res
```

### Comparing `tsugu-1.1.0rc3/tsugu_async/router/universal/search_character.py` & `tsugu-1.1.0rc4/tsugu_async/src/universal/search_song.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,25 @@
-from ...utils import text_response, User
+from ...utils import text_response, User, server_id_2_server_name, server_name_2_server_id, server_exists, config
 import tsugu_api_async
-from ...config import config
 from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, MultiVar
 
 
-alc = Alconna(
-        ["查角色"],
-        Args["word#角色名，乐队，昵称等查询参数", MultiVar(str)],
+async def handler(message: str, user: User, platform: str, channel_id: str):
+    res = Alconna(
+        ["查曲"],
+        Args["word#歌曲信息，名称，乐队，难度等。", MultiVar(str)],
         meta=CommandMeta(
-            compact=config.compact, description="查询角色信息",
-            usage='根据关键词或角色ID查询角色信息',
-            example='''查角色 10 :返回10号角色的信息。
-查角色 吉他 :返回所有角色模糊搜索标签中包含吉他的角色列表。'''
+            compact=config.compact, description="查曲",
+            usage='根据关键词或曲目ID查询曲目信息。',
+            example='''查曲 1 :返回1号曲的信息
+查曲 ag lv27 :返回所有难度为27的ag曲列表
+查曲 >27 :查询大于27的曲目
+查曲 滑滑蛋 :匹配歌曲 fuwa fuwa time'''
         )
-    )
+    ).parse(message)
 
+    if res.matched:
+        return await tsugu_api_async.search_song(user.default_server, " ".join(res.word))
+
+    return res
 
-async def handler(message: str, user: User, platform: str, channel_id: str):
-    res = alc.parse(message)
 
-    if res.matched:
-        return await tsugu_api_async.search_character(user.default_server, " ".join(res.word))
-    elif res.head_matched:
-        return text_response(res.error_info)
-    return None
```

### Comparing `tsugu-1.1.0rc3/tsugu_async/router/universal/search_event.py` & `tsugu-1.1.0rc4/tsugu_async/src/universal/search_event.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,24 @@
-from ...utils import text_response, User
+from ...utils import text_response, User, server_id_2_server_name, server_name_2_server_id, server_exists, config
 import tsugu_api_async
-from ...config import config
 from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, MultiVar
 
 
-alc = Alconna(
+async def handler(message: str, user: User, platform: str, channel_id: str):
+    res = Alconna(
         ["查活动"],
         Args["word#请输入活动名，乐队，活动ID等查询参数", MultiVar(str)],
         meta=CommandMeta(
             compact=config.compact, description="查活动",
             usage='根据关键词或活动ID查询活动信息',
             example='''查活动 绿 tsugu :返回所有属性加成为pure，且活动加成角色中包括羽泽鸫的活动列表
 查活动 177 :返回177号活动的信息
 查活动 >225 :查询大于225的活动
 查活动 220-225 :查询220到225的活动'''
         )
-    )
-
-
-async def handler(message: str, user: User, platform: str, channel_id: str):
-    res = alc.parse(message)
+    ).parse(message)
 
     if res.matched:
         return await tsugu_api_async.search_event(user.default_server, " ".join(res.word))
-    elif res.head_matched:
-        return text_response(res.error_info)
-    return None
+
+    return res
```

### Comparing `tsugu-1.1.0rc3/tsugu_async/router/universal/search_gacha.py` & `tsugu-1.1.0rc4/tsugu_async/src/universal/search_gacha.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,19 @@
-from ...utils import text_response, User
+from ...utils import text_response, User, server_id_2_server_name, server_name_2_server_id, server_exists, config
 import tsugu_api_async
-from ...config import config
 from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager
 
 
-alc = Alconna(
+async def handler(message: str, user: User, platform: str, channel_id: str):
+    res = Alconna(
         ["查卡池"],
         Args["gachaId#可以通过查活动、查卡等获取", str],
         meta=CommandMeta(
             compact=config.compact, description="查卡池",
             usage='根据卡池ID查询卡池信息',
         )
-    )
-
-
-async def handler(message: str, user: User, platform: str, channel_id: str):
-    res = alc.parse(message)
+    ).parse(message)
 
     if res.matched:
         return await tsugu_api_async.search_gacha(user.default_server, res.gachaId)
-    elif res.head_matched:
-        return text_response(res.error_info)
-    return None
+
+    return res
```

### Comparing `tsugu-1.1.0rc3/tsugu_async/router/universal/search_player.py` & `tsugu-1.1.0rc4/tsugu/src/universal/search_player.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,33 +1,28 @@
-from ...utils import text_response, User
+from ...utils import text_response, User, server_id_2_server_name, server_name_2_server_id, server_exists, config
 from tsugu_api_core._typing import _ServerName
-import tsugu_api_async
-from ...config import config
+import tsugu_api
 from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager
 
 
-alc = Alconna(
-    ["查玩家", "查寻玩家"],
-    Args["playerId#你的游戏账号(数字)", int]["serverName;?#省略服务器名时，默认从你当前的主服务器查询。", _ServerName.__args__],
-    meta=CommandMeta(
-        compact=config.compact, description="查询玩家信息",
-        usage='查询指定ID玩家的信息。查询指定ID玩家的信息。',
-        example='查玩家 40474621 jp : 查询日服玩家ID为40474621的玩家信息。\n查玩家 10000000 : 查询你当前默认服务器中，玩家ID为10000000的玩家信息。',
-    )
-)
-
-
-async def handler(message: str, user: User, platform: str, channel_id: str):
-    res = alc.parse(message)
+def handler(message: str, user: User, platform: str, channel_id: str):
+    res = Alconna(
+        ["查玩家", "查寻玩家"],
+        Args["playerId#你的游戏账号(数字)", int]["serverName;?#省略服务器名时，默认从你当前的主服务器查询。", _ServerName.__args__],
+        meta=CommandMeta(
+            compact=config.compact, description="查询玩家信息",
+            usage='查询指定ID玩家的信息。查询指定ID玩家的信息。',
+            example='查玩家 40474621 jp : 查询日服玩家ID为40474621的玩家信息。\n查玩家 10000000 : 查询你当前默认服务器中，玩家ID为10000000的玩家信息。',
+        )
+    ).parse(message)
 
     if res.matched:
         if res.serverName:
             server = res.serverName
         else:
             server = user.server_mode
-        return await tsugu_api_async.search_player(res.playerId, server)
-    elif res.head_matched:
-        return text_response(res.error_info)
-    return None
+        return tsugu_api.search_player(res.playerId, server)
+
+    return res
```

### Comparing `tsugu-1.1.0rc3/tsugu_async/router/universal/song_chart.py` & `tsugu-1.1.0rc4/tsugu/src/universal/song_chart.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,31 +1,27 @@
-from ...utils import text_response, User
-import tsugu_api_async
-from ...config import config
+from ...utils import text_response, User, server_id_2_server_name, server_name_2_server_id, server_exists, config
+import tsugu_api
 from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager
 
 
 difficulty_text_tuple = ('easy', 'ez', 'normal', 'nm', 'hard', 'hd', 'expert', 'ex', 'special', 'sp')
 
-alc = Alconna(
+
+def handler(message: str, user: User, platform: str, channel_id: str):
+    res = Alconna(
         ["查谱面", "查铺面"],
         Args["songId", int]['difficultyText', difficulty_text_tuple, 'ex'],
         meta=CommandMeta(
             compact=config.compact, description="查谱面",
             usage='根据曲目ID与难度查询铺面信息。',
             example='''查谱面 1 :返回1号曲的ex难度谱面
 查谱面 128 special :返回128号曲的special难度谱面'''
         )
-    )
-
-
-async def handler(message: str, user: User, platform: str, channel_id: str):
-    res = alc.parse(message)
+    ).parse(message)
 
     if res.matched:
-        return await tsugu_api_async.song_chart(user.default_server, res.songId, res.difficultyText)
-    elif res.head_matched:
-        return text_response(res.error_info)
-    return None
+        return tsugu_api.song_chart(user.default_server, res.songId, res.difficultyText)
+
+    return res
```

### Comparing `tsugu-1.1.0rc3/tsugu_async/router/universal/song_meta.py` & `tsugu-1.1.0rc4/tsugu/src/universal/song_meta.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,31 +1,26 @@
-from ...utils import text_response, User, server_name_2_server_id
-import tsugu_api_async
-from ...config import config
+from ...utils import text_response, User, server_id_2_server_name, server_name_2_server_id, server_exists, config
+import tsugu_api
 from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager
 from tsugu_api_core._typing import _ServerName
 
 
-alc = Alconna(
+def handler(message: str, user: User, platform: str, channel_id: str):
+    res = Alconna(
         ["查询分数表", '查分数表', '查询分数榜', '查分数榜'],
         Args["serverName;?#省略服务器名时，默认从你当前的主服务器查询。", _ServerName.__args__],
         meta=CommandMeta(
             compact=config.compact, description="查询分数表",
             usage='查询指定服务器的歌曲分数表。',
             example='''查询分数表 cn :返回国服的歌曲分数表'''
         )
-    )
-
-
-async def handler(message: str, user: User, platform: str, channel_id: str):
-    res = alc.parse(message)
+    ).parse(message)
 
     if res.matched:
         if res.serverName:
             server = server_name_2_server_id(res.serverName)
         else:
             server = user.server_mode
-        return await tsugu_api_async.song_meta(user.default_server, server)
-    elif res.head_matched:
-        return text_response(res.error_info)
-    return None
+        return tsugu_api.song_meta(user.default_server, server)
+
+    return res
```

### Comparing `tsugu-1.1.0rc3/tsugu_async/router/universal/ycx.py` & `tsugu-1.1.0rc4/tsugu/src/universal/lsycx.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,24 @@
-from ...utils import text_response, User, server_name_2_server_id
-import tsugu_api_async
-from ...config import config
+from ...utils import text_response, User, server_id_2_server_name, server_name_2_server_id, server_exists, config
+import tsugu_api
 from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager
 from tsugu_api_core._typing import _ServerName
 
 
-alc = Alconna(
-        ["ycx", "预测线"],
+def handler(message: str, user: User, platform: str, channel_id: str):
+    res = Alconna(
+        ["lsycx", "历史预测线"], ['/', ''],
         Args['tier', int]['eventId;?#活动ID，省略时查询当前活动。', int]
             ['serverName#省略服务器名时，默认从你当前的主服务器查询。活动ID不存在时，也可以作为第二个参数。', _ServerName.__args__, None],
         meta=CommandMeta(
-            compact=config.compact, description="查询指定档位的预测线",
-            usage='查询指定档位的预测线。',
-            example='''ycx 1000 :返回默认服务器当前活动1000档位的档线与预测线。
-ycx 1000 177 jp:返回日服177号活动1000档位的档线与预测线。'''
+            compact=config.compact, description="查询指定档位的历史预测线。",
+            usage='查询指定档位的预测线与最近的4期活动类型相同的活动的档线数据。',
+            example='''lsycx 1000 :返回默认服务器当前活动的档线与预测线，与最近的4期活动类型相同的活动的档线数据。
+lsycx 1000 177 jp:返回日服177号活动1000档位档线与最近的4期活动类型相同的活动的档线数据。'''
         )
-    )
-
-
-async def handler(message: str, user: User, platform: str, channel_id: str):
-    res = alc.parse(message)
+    ).parse(message)
 
     if res.matched:
         server = server_name_2_server_id(res.serverName) if res.serverName else user.server_mode
-        return await tsugu_api_async.ycx(server, res.tier, res.eventId)
-    elif res.head_matched:
-        return text_response(res.error_info)
-    return None
+        return tsugu_api.lsycx(server, res.tier, res.eventId)
 
+    return res
```

### Comparing `tsugu-1.1.0rc3/tsugu_async/utils/__init__.py` & `tsugu-1.1.0rc4/tsugu_async/utils/__init__.py`

 * *Files identical despite different names*

