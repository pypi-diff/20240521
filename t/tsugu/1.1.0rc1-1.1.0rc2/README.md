# Comparing `tmp/tsugu-1.1.0rc1.tar.gz` & `tmp/tsugu-1.1.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsugu-1.1.0rc1.tar", last modified: Mon May 20 19:00:58 2024, max compression
+gzip compressed data, was "tsugu-1.1.0rc2.tar", last modified: Tue May 21 02:56:22 2024, max compression
```

## Comparing `tsugu-1.1.0rc1.tar` & `tsugu-1.1.0rc2.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:00:58.832085 tsugu-1.1.0rc1/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6401 2024-05-20 19:00:58.828085 tsugu-1.1.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4448 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 19:00:58.832085 tsugu-1.1.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:00:58.820085 tsugu-1.1.0rc1/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/test/test_async.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:00:58.820085 tsugu-1.1.0rc1/tsugu/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:00:58.820085 tsugu-1.1.0rc1/tsugu/router/
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu/router/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:00:58.820085 tsugu-1.1.0rc1/tsugu/router/bandoristation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu/router/bandoristation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2841 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu/router/bandoristation/rooms_forward.py
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu/router/bandoristation/ycm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:00:58.824085 tsugu-1.1.0rc1/tsugu/router/remote/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu/router/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu/router/remote/bind_player.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu/router/remote/bind_player_verification_off.py
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu/router/remote/bind_player_verification_on.py
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu/router/remote/change_default_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu/router/remote/change_server_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu/router/remote/player_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu/router/remote/switch_car_forwarding_off.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu/router/remote/switch_car_forwarding_on.py
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu/router/remote/unbind_player.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:00:58.824085 tsugu-1.1.0rc1/tsugu/router/universal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu/router/universal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu/router/universal/event_stage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu/router/universal/gacha_simulate.py
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu/router/universal/get_card_illustration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu/router/universal/lsycx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu/router/universal/search_card.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu/router/universal/search_character.py
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu/router/universal/search_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu/router/universal/search_gacha.py
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu/router/universal/search_player.py
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu/router/universal/search_song.py
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu/router/universal/song_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu/router/universal/song_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu/router/universal/ycx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu/router/universal/ycx_all.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:00:58.824085 tsugu-1.1.0rc1/tsugu/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:00:58.820085 tsugu-1.1.0rc1/tsugu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6401 2024-05-20 19:00:58.000000 tsugu-1.1.0rc1/tsugu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-05-20 19:00:58.000000 tsugu-1.1.0rc1/tsugu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 19:00:58.000000 tsugu-1.1.0rc1/tsugu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-20 19:00:58.000000 tsugu-1.1.0rc1/tsugu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-20 19:00:58.000000 tsugu-1.1.0rc1/tsugu.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:00:58.824085 tsugu-1.1.0rc1/tsugu_async/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu_async/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu_async/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu_async/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:00:58.824085 tsugu-1.1.0rc1/tsugu_async/router/
--rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu_async/router/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:00:58.824085 tsugu-1.1.0rc1/tsugu_async/router/bandoristation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu_async/router/bandoristation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu_async/router/bandoristation/rooms_forward.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu_async/router/bandoristation/ycm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:00:58.828085 tsugu-1.1.0rc1/tsugu_async/router/remote/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu_async/router/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu_async/router/remote/bind_player.py
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu_async/router/remote/bind_player_verification_off.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu_async/router/remote/bind_player_verification_on.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu_async/router/remote/change_default_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu_async/router/remote/change_server_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu_async/router/remote/player_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu_async/router/remote/switch_car_forwarding_off.py
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu_async/router/remote/switch_car_forwarding_on.py
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu_async/router/remote/unbind_player.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:00:58.828085 tsugu-1.1.0rc1/tsugu_async/router/universal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu_async/router/universal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu_async/router/universal/event_stage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu_async/router/universal/gacha_simulate.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu_async/router/universal/get_card_illustration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu_async/router/universal/lsycx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu_async/router/universal/search_card.py
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu_async/router/universal/search_character.py
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu_async/router/universal/search_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu_async/router/universal/search_gacha.py
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu_async/router/universal/search_player.py
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu_async/router/universal/search_song.py
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu_async/router/universal/song_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu_async/router/universal/song_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu_async/router/universal/ycx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu_async/router/universal/ycx_all.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:00:58.828085 tsugu-1.1.0rc1/tsugu_async/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu_async/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 02:56:22.221635 tsugu-1.1.0rc2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6443 2024-05-21 02:56:22.221635 tsugu-1.1.0rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4482 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 02:56:22.221635 tsugu-1.1.0rc2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 02:56:22.209635 tsugu-1.1.0rc2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/test/test_async.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 02:56:22.209635 tsugu-1.1.0rc2/tsugu/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 02:56:22.209635 tsugu-1.1.0rc2/tsugu/router/
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu/router/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 02:56:22.209635 tsugu-1.1.0rc2/tsugu/router/bandoristation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu/router/bandoristation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2841 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu/router/bandoristation/rooms_forward.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu/router/bandoristation/ycm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 02:56:22.213635 tsugu-1.1.0rc2/tsugu/router/remote/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu/router/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu/router/remote/bind_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu/router/remote/bind_player_verification_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu/router/remote/bind_player_verification_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu/router/remote/change_default_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu/router/remote/change_server_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu/router/remote/player_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu/router/remote/switch_car_forwarding_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu/router/remote/switch_car_forwarding_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu/router/remote/unbind_player.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 02:56:22.213635 tsugu-1.1.0rc2/tsugu/router/universal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu/router/universal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu/router/universal/event_stage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu/router/universal/gacha_simulate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu/router/universal/get_card_illustration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu/router/universal/lsycx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu/router/universal/search_card.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu/router/universal/search_character.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu/router/universal/search_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu/router/universal/search_gacha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu/router/universal/search_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu/router/universal/search_song.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu/router/universal/song_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu/router/universal/song_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu/router/universal/ycx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu/router/universal/ycx_all.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 02:56:22.213635 tsugu-1.1.0rc2/tsugu/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 02:56:22.209635 tsugu-1.1.0rc2/tsugu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6443 2024-05-21 02:56:22.000000 tsugu-1.1.0rc2/tsugu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-05-21 02:56:22.000000 tsugu-1.1.0rc2/tsugu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 02:56:22.000000 tsugu-1.1.0rc2/tsugu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-21 02:56:22.000000 tsugu-1.1.0rc2/tsugu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-21 02:56:22.000000 tsugu-1.1.0rc2/tsugu.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 02:56:22.217635 tsugu-1.1.0rc2/tsugu_async/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu_async/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu_async/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu_async/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 02:56:22.217635 tsugu-1.1.0rc2/tsugu_async/router/
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu_async/router/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 02:56:22.217635 tsugu-1.1.0rc2/tsugu_async/router/bandoristation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu_async/router/bandoristation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu_async/router/bandoristation/rooms_forward.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu_async/router/bandoristation/ycm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 02:56:22.217635 tsugu-1.1.0rc2/tsugu_async/router/remote/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu_async/router/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu_async/router/remote/bind_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu_async/router/remote/bind_player_verification_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu_async/router/remote/bind_player_verification_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu_async/router/remote/change_default_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu_async/router/remote/change_server_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu_async/router/remote/player_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu_async/router/remote/switch_car_forwarding_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu_async/router/remote/switch_car_forwarding_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu_async/router/remote/unbind_player.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 02:56:22.221635 tsugu-1.1.0rc2/tsugu_async/router/universal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu_async/router/universal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu_async/router/universal/event_stage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu_async/router/universal/gacha_simulate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu_async/router/universal/get_card_illustration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu_async/router/universal/lsycx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu_async/router/universal/search_card.py
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu_async/router/universal/search_character.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu_async/router/universal/search_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu_async/router/universal/search_gacha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu_async/router/universal/search_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu_async/router/universal/search_song.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu_async/router/universal/song_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu_async/router/universal/song_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu_async/router/universal/ycx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu_async/router/universal/ycx_all.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 02:56:22.221635 tsugu-1.1.0rc2/tsugu_async/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu_async/utils/__init__.py
```

### Comparing `tsugu-1.1.0rc1/LICENSE` & `tsugu-1.1.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc1/PKG-INFO` & `tsugu-1.1.0rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu
-Version: 1.1.0rc1
+Version: 1.1.0rc2
 Summary: Tsugu Python Frontend
 Home-page: https://github.com/kumoSleeping/ChatTsuguPy
 Author: kumoSleeping
 Author-email: zjr2992@outlook.com
 License: MIT
 Description: 
         <h1 align="center"> Chat Tsugu Py <img src="./logo.jpg" width="30" width="30" height="30" alt="tmrn"/> </h1>
@@ -32,18 +32,17 @@
         ---
         
         
         ```shell
         pip install tsugu
         ```
         
+        > API powered by  <a href="https://github.com/WindowsSov8forUs/tsugu-api-python?tab=readme-ov-file">tsugu-api-python</a>
         
-        > API Powered by  <a href="https://github.com/WindowsSov8forUs/tsugu-api-python?tab=readme-ov-file">tsugu-api-python</a>
-        
-        > Command matching by <a href="https://github.com/ArcletProject/Alconna">Alconna</a>
+        > Command matching provided by <a href="https://github.com/ArcletProject/Alconna">Alconna</a>
         ***
         
         ## handler
         
         - `handler` 用于直接处理用户输入的自然语言并返回查询结果: 
         
         ```python
@@ -137,15 +136,15 @@
         '''
         是否压缩返回数据，压缩可减少返回数据大小。
         默认为 True，即压缩返回数据。若不压缩返回数据，可将此项设置为 False。
         '''
         
         ```
         
-        ### tsugu_async config
+        ### tsugu config
         
         ```py
         from tsugu import config
         
         
         config.compact = True
         '''
@@ -168,18 +167,20 @@
         
         config.disable_gacha_simulate_group_ids = []
         '''
         需要关闭模拟抽卡的群
         '''
         ```
         
+        ### tsugu_async config
+        
         ```py
         from tsugu_async import config
         ...
-        # 与上面相同
+        # 与 tsugu config 相同
         ```
         
         
         
         ***
         
          <details>
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: tsugu Version: 1.1.0rc1 Summary: Tsugu Python
+Metadata-Version: 2.1 Name: tsugu Version: 1.1.0rc2 Summary: Tsugu Python
 Frontend Home-page: https://github.com/kumoSleeping/ChatTsuguPy Author:
 kumoSleeping Author-email: zjr2992@outlook.com License: MIT Description:
                        ************ CChhaatt TTssuugguu PPyy[[ttmmrrnn]] ************
 _â¨ Python ç¼åç [TsuguBanGDreamBot](https://github.com/Yamamoto-2/tsugu-
          bangdream-bot?tab=readme-ov-file) èªç¶è¯­è¨äº¤äºåº â¨_
                           _[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]
---- ```shell pip install tsugu ``` > API Powered by _t_s_u_g_u_-_a_p_i_-_p_y_t_h_o_n > Command
-matching by _A_l_c_o_n_n_a *** ## handler - `handler`
+--- ```shell pip install tsugu ``` > API powered by _t_s_u_g_u_-_a_p_i_-_p_y_t_h_o_n > Command
+matching provided by _A_l_c_o_n_n_a *** ## handler - `handler`
 ç¨äºç´æ¥å¤çç¨æ·è¾å¥çèªç¶è¯­è¨å¹¶è¿åæ¥è¯¢ç»æ: ```python
 import tsugu # åä¸ªåæ°ï¼åå«æå³ç æ¶æ¯åå®¹ ç¨æ·id å¹³å°
 é¢éid for i in tsugu.handler(message='æ¥å¡ ars 1x', user_id='1528593481',
 platform='red', channel_id='666808414'): print('ææ¬: ',i) if isinstance(i,
 str) else None print(f"[å¾ç]") if isinstance(i, bytes) else None ```
 ```python import tsugu_async ... ``` > å¨å¸¸ç¨çqqbotä¸­ï¼ç¾¤å·å°±æ¯
 `channel_id`ã > å½ä½ ä½¿ç¨QQå·ä½ä¸º `user_id` æ¶ï¼`platform`
@@ -38,21 +38,21 @@
 Falseã ''' settings.use_easy_bg = True '''
 æ¯å¦ä½¿ç¨ç®æèæ¯ï¼ä½¿ç¨å¯å¨éä½èæ¯è´¨éçåæä¸å å¿«ååºéåº¦ã
 é»è®¤ä¸º
 Trueï¼å³ä½¿ç¨ç®æèæ¯ãè¥ä¸ä½¿ç¨ç®æèæ¯ï¼å¯å°æ­¤é¡¹è®¾ç½®ä¸º
 Falseã ''' settings.compress = True '''
 æ¯å¦åç¼©è¿åæ°æ®ï¼åç¼©å¯åå°è¿åæ°æ®å¤§å°ã é»è®¤ä¸º
 Trueï¼å³åç¼©è¿åæ°æ®ãè¥ä¸åç¼©è¿åæ°æ®ï¼å¯å°æ­¤é¡¹è®¾ç½®ä¸º
-Falseã ''' ``` ### tsugu_async config ```py from tsugu import config
-config.compact = True ''' æ¯å¦åè®¸å½ä»¤ä¸åæ°ä¹é´æ²¡æç©ºæ ¼ '''
+Falseã ''' ``` ### tsugu config ```py from tsugu import config config.compact
+= True ''' æ¯å¦åè®¸å½ä»¤ä¸åæ°ä¹é´æ²¡æç©ºæ ¼ '''
 config.remote_data_max_retry = 3 ''' è·åè¿ç¨ç¨æ·æ°æ®æå¤§éè¯æ¬¡æ°
 ''' config.bandori_station_token_name = "Tsugu" ''' bandori station token '''
 config.bandori_station_token = "ZtV4EX2K9Onb" ''' bandori station token '''
 config.disable_gacha_simulate_group_ids = [] ''' éè¦å³é­æ¨¡ææ½å¡çç¾¤
-''' ``` ```py from tsugu_async import config ... # ä¸ä¸é¢ç¸å ``` ***
-?å?®?¢?æ???ð???±?æ???å?¯?¼((?è?¿??é???å??¯?ä?»?¥?ç??¹?å??»))
+''' ``` ### tsugu_async config ```py from tsugu_async import config ... # ä¸
+tsugu config ç¸å ``` *** ?å?®?¢?æ???ð???±?æ???å?¯?¼((?è?¿??é???å??¯?ä?»?¥?ç??¹?å??»))
 **æ³¨æï¼å¦æä½ ä¸ç¥éä»ä¹æ¯BanGDreamï¼è¯·ä¸è¦éæå ç¾¤**
 **æ¬ç¾¤è¿æ¯æ¬¢è¿å ç¾¤çï¼** [BanGDreamBotå¼åèå¤©ç¾¤](https://
 qm.qq.com/q/zjUPQkrdpm) æ¸©é¦¨çèå¤©ç¯å¢ï½ --- Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8 Description-Content-Type: text/markdown
```

### Comparing `tsugu-1.1.0rc1/README.md` & `tsugu-1.1.0rc2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -24,18 +24,17 @@
 ---
 
 
 ```shell
 pip install tsugu
 ```
 
+> API powered by  <a href="https://github.com/WindowsSov8forUs/tsugu-api-python?tab=readme-ov-file">tsugu-api-python</a>
 
-> API Powered by  <a href="https://github.com/WindowsSov8forUs/tsugu-api-python?tab=readme-ov-file">tsugu-api-python</a>
-
-> Command matching by <a href="https://github.com/ArcletProject/Alconna">Alconna</a>
+> Command matching provided by <a href="https://github.com/ArcletProject/Alconna">Alconna</a>
 ***
 
 ## handler
 
 - `handler` 用于直接处理用户输入的自然语言并返回查询结果: 
 
 ```python
@@ -129,15 +128,15 @@
 '''
 是否压缩返回数据，压缩可减少返回数据大小。
 默认为 True，即压缩返回数据。若不压缩返回数据，可将此项设置为 False。
 '''
 
 ```
 
-### tsugu_async config
+### tsugu config
 
 ```py
 from tsugu import config
 
 
 config.compact = True
 '''
@@ -160,18 +159,20 @@
 
 config.disable_gacha_simulate_group_ids = []
 '''
 需要关闭模拟抽卡的群
 '''
 ```
 
+### tsugu_async config
+
 ```py
 from tsugu_async import config
 ...
-# 与上面相同
+# 与 tsugu config 相同
 ```
 
 
 
 ***
 
  <details>
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
                        ************ CChhaatt TTssuugguu PPyy[[ttmmrrnn]] ************
 _â¨ Python ç¼åç [TsuguBanGDreamBot](https://github.com/Yamamoto-2/tsugu-
          bangdream-bot?tab=readme-ov-file) èªç¶è¯­è¨äº¤äºåº â¨_
                           _[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]
---- ```shell pip install tsugu ``` > API Powered by _t_s_u_g_u_-_a_p_i_-_p_y_t_h_o_n > Command
-matching by _A_l_c_o_n_n_a *** ## handler - `handler`
+--- ```shell pip install tsugu ``` > API powered by _t_s_u_g_u_-_a_p_i_-_p_y_t_h_o_n > Command
+matching provided by _A_l_c_o_n_n_a *** ## handler - `handler`
 ç¨äºç´æ¥å¤çç¨æ·è¾å¥çèªç¶è¯­è¨å¹¶è¿åæ¥è¯¢ç»æ: ```python
 import tsugu # åä¸ªåæ°ï¼åå«æå³ç æ¶æ¯åå®¹ ç¨æ·id å¹³å°
 é¢éid for i in tsugu.handler(message='æ¥å¡ ars 1x', user_id='1528593481',
 platform='red', channel_id='666808414'): print('ææ¬: ',i) if isinstance(i,
 str) else None print(f"[å¾ç]") if isinstance(i, bytes) else None ```
 ```python import tsugu_async ... ``` > å¨å¸¸ç¨çqqbotä¸­ï¼ç¾¤å·å°±æ¯
 `channel_id`ã > å½ä½ ä½¿ç¨QQå·ä½ä¸º `user_id` æ¶ï¼`platform`
@@ -35,18 +35,18 @@
 Falseã ''' settings.use_easy_bg = True '''
 æ¯å¦ä½¿ç¨ç®æèæ¯ï¼ä½¿ç¨å¯å¨éä½èæ¯è´¨éçåæä¸å å¿«ååºéåº¦ã
 é»è®¤ä¸º
 Trueï¼å³ä½¿ç¨ç®æèæ¯ãè¥ä¸ä½¿ç¨ç®æèæ¯ï¼å¯å°æ­¤é¡¹è®¾ç½®ä¸º
 Falseã ''' settings.compress = True '''
 æ¯å¦åç¼©è¿åæ°æ®ï¼åç¼©å¯åå°è¿åæ°æ®å¤§å°ã é»è®¤ä¸º
 Trueï¼å³åç¼©è¿åæ°æ®ãè¥ä¸åç¼©è¿åæ°æ®ï¼å¯å°æ­¤é¡¹è®¾ç½®ä¸º
-Falseã ''' ``` ### tsugu_async config ```py from tsugu import config
-config.compact = True ''' æ¯å¦åè®¸å½ä»¤ä¸åæ°ä¹é´æ²¡æç©ºæ ¼ '''
+Falseã ''' ``` ### tsugu config ```py from tsugu import config config.compact
+= True ''' æ¯å¦åè®¸å½ä»¤ä¸åæ°ä¹é´æ²¡æç©ºæ ¼ '''
 config.remote_data_max_retry = 3 ''' è·åè¿ç¨ç¨æ·æ°æ®æå¤§éè¯æ¬¡æ°
 ''' config.bandori_station_token_name = "Tsugu" ''' bandori station token '''
 config.bandori_station_token = "ZtV4EX2K9Onb" ''' bandori station token '''
 config.disable_gacha_simulate_group_ids = [] ''' éè¦å³é­æ¨¡ææ½å¡çç¾¤
-''' ``` ```py from tsugu_async import config ... # ä¸ä¸é¢ç¸å ``` ***
-?å?®?¢?æ???ð???±?æ???å?¯?¼((?è?¿??é???å??¯?ä?»?¥?ç??¹?å??»))
+''' ``` ### tsugu_async config ```py from tsugu_async import config ... # ä¸
+tsugu config ç¸å ``` *** ?å?®?¢?æ???ð???±?æ???å?¯?¼((?è?¿??é???å??¯?ä?»?¥?ç??¹?å??»))
 **æ³¨æï¼å¦æä½ ä¸ç¥éä»ä¹æ¯BanGDreamï¼è¯·ä¸è¦éæå ç¾¤**
 **æ¬ç¾¤è¿æ¯æ¬¢è¿å ç¾¤çï¼** [BanGDreamBotå¼åèå¤©ç¾¤](https://
 qm.qq.com/q/zjUPQkrdpm) æ¸©é¦¨çèå¤©ç¯å¢ï½ ---
```

### Comparing `tsugu-1.1.0rc1/setup.py` & `tsugu-1.1.0rc2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r') as readme:
     long_description = readme.read()
 
 setup(
     name='tsugu',
-    version='1.1.0-rc1',
+    version='1.1.0-rc2',
     author='kumoSleeping',
     author_email='zjr2992@outlook.com',
     license="MIT",
     description='Tsugu Python Frontend',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/kumoSleeping/ChatTsuguPy',
     packages=find_packages(exclude=('test','test*')),
     classifiers=[
         'Programming Language :: Python :: 3.8',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent'
     ],
     install_requires=[
-            "loguru",
+            "loguru==0.7.2",
             "tsugu-api-python==1.2.0",
-            "arclet-alconna",
+            "arclet-alconna==1.8.12",
         ],
     python_requires='>=3.8',
     include_package_data=False,
 
 )
```

### Comparing `tsugu-1.1.0rc1/test/test_async.py` & `tsugu-1.1.0rc2/test/test_async.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc1/tsugu/handler.py` & `tsugu-1.1.0rc2/tsugu/handler.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc1/tsugu/router/__init__.py` & `tsugu-1.1.0rc2/tsugu/router/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -76,11 +76,12 @@
     if res:
         return res
 
     res = handler_feats(bandoristation_commands)
     if res:
         return res
 
-    if Alconna(["help", "帮助"], meta=CommandMeta(description='Chat Tsugu Py 帮助')).parse(message).matched:
-        return text_response(command_manager.all_command_help()+"\n# 例如: 查卡 -h")
+    if message in ["help", "帮助"]:
+        return text_response(command_manager.all_command_help(show_index=True))
 
     return None
+
```

### Comparing `tsugu-1.1.0rc1/tsugu/router/bandoristation/rooms_forward.py` & `tsugu-1.1.0rc2/tsugu/router/bandoristation/rooms_forward.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc1/tsugu/router/bandoristation/ycm.py` & `tsugu-1.1.0rc2/tsugu/router/bandoristation/ycm.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc1/tsugu/router/remote/bind_player.py` & `tsugu-1.1.0rc2/tsugu/router/remote/bind_player.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc1/tsugu/router/remote/bind_player_verification_off.py` & `tsugu-1.1.0rc2/tsugu/router/remote/bind_player_verification_off.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc1/tsugu/router/remote/bind_player_verification_on.py` & `tsugu-1.1.0rc2/tsugu/router/remote/bind_player_verification_on.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc1/tsugu/router/remote/change_default_server.py` & `tsugu-1.1.0rc2/tsugu/router/remote/change_default_server.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc1/tsugu/router/remote/change_server_mode.py` & `tsugu-1.1.0rc2/tsugu/router/remote/change_server_mode.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc1/tsugu/router/remote/player_status.py` & `tsugu-1.1.0rc2/tsugu/router/remote/player_status.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc1/tsugu/router/remote/switch_car_forwarding_off.py` & `tsugu-1.1.0rc2/tsugu/router/remote/switch_car_forwarding_off.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc1/tsugu/router/remote/switch_car_forwarding_on.py` & `tsugu-1.1.0rc2/tsugu/router/remote/switch_car_forwarding_on.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc1/tsugu/router/remote/unbind_player.py` & `tsugu-1.1.0rc2/tsugu/router/remote/unbind_player.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc1/tsugu/router/universal/event_stage.py` & `tsugu-1.1.0rc2/tsugu/router/universal/event_stage.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc1/tsugu/router/universal/gacha_simulate.py` & `tsugu-1.1.0rc2/tsugu/router/universal/gacha_simulate.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc1/tsugu/router/universal/get_card_illustration.py` & `tsugu-1.1.0rc2/tsugu/router/universal/get_card_illustration.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc1/tsugu/router/universal/lsycx.py` & `tsugu-1.1.0rc2/tsugu/router/universal/lsycx.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc1/tsugu/router/universal/search_card.py` & `tsugu-1.1.0rc2/tsugu/router/universal/search_card.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc1/tsugu/router/universal/search_character.py` & `tsugu-1.1.0rc2/tsugu/router/universal/search_character.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc1/tsugu/router/universal/search_event.py` & `tsugu-1.1.0rc2/tsugu/router/universal/search_event.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc1/tsugu/router/universal/search_gacha.py` & `tsugu-1.1.0rc2/tsugu/router/universal/search_gacha.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc1/tsugu/router/universal/search_player.py` & `tsugu-1.1.0rc2/tsugu/router/universal/search_player.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc1/tsugu/router/universal/search_song.py` & `tsugu-1.1.0rc2/tsugu/router/universal/search_song.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc1/tsugu/router/universal/song_chart.py` & `tsugu-1.1.0rc2/tsugu/router/universal/song_chart.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc1/tsugu/router/universal/song_meta.py` & `tsugu-1.1.0rc2/tsugu/router/universal/song_meta.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc1/tsugu/router/universal/ycx.py` & `tsugu-1.1.0rc2/tsugu/router/universal/ycx.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc1/tsugu/router/universal/ycx_all.py` & `tsugu-1.1.0rc2/tsugu/router/universal/ycx_all.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc1/tsugu/utils/__init__.py` & `tsugu-1.1.0rc2/tsugu/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc1/tsugu.egg-info/PKG-INFO` & `tsugu-1.1.0rc2/tsugu.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu
-Version: 1.1.0rc1
+Version: 1.1.0rc2
 Summary: Tsugu Python Frontend
 Home-page: https://github.com/kumoSleeping/ChatTsuguPy
 Author: kumoSleeping
 Author-email: zjr2992@outlook.com
 License: MIT
 Description: 
         <h1 align="center"> Chat Tsugu Py <img src="./logo.jpg" width="30" width="30" height="30" alt="tmrn"/> </h1>
@@ -32,18 +32,17 @@
         ---
         
         
         ```shell
         pip install tsugu
         ```
         
+        > API powered by  <a href="https://github.com/WindowsSov8forUs/tsugu-api-python?tab=readme-ov-file">tsugu-api-python</a>
         
-        > API Powered by  <a href="https://github.com/WindowsSov8forUs/tsugu-api-python?tab=readme-ov-file">tsugu-api-python</a>
-        
-        > Command matching by <a href="https://github.com/ArcletProject/Alconna">Alconna</a>
+        > Command matching provided by <a href="https://github.com/ArcletProject/Alconna">Alconna</a>
         ***
         
         ## handler
         
         - `handler` 用于直接处理用户输入的自然语言并返回查询结果: 
         
         ```python
@@ -137,15 +136,15 @@
         '''
         是否压缩返回数据，压缩可减少返回数据大小。
         默认为 True，即压缩返回数据。若不压缩返回数据，可将此项设置为 False。
         '''
         
         ```
         
-        ### tsugu_async config
+        ### tsugu config
         
         ```py
         from tsugu import config
         
         
         config.compact = True
         '''
@@ -168,18 +167,20 @@
         
         config.disable_gacha_simulate_group_ids = []
         '''
         需要关闭模拟抽卡的群
         '''
         ```
         
+        ### tsugu_async config
+        
         ```py
         from tsugu_async import config
         ...
-        # 与上面相同
+        # 与 tsugu config 相同
         ```
         
         
         
         ***
         
          <details>
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: tsugu Version: 1.1.0rc1 Summary: Tsugu Python
+Metadata-Version: 2.1 Name: tsugu Version: 1.1.0rc2 Summary: Tsugu Python
 Frontend Home-page: https://github.com/kumoSleeping/ChatTsuguPy Author:
 kumoSleeping Author-email: zjr2992@outlook.com License: MIT Description:
                        ************ CChhaatt TTssuugguu PPyy[[ttmmrrnn]] ************
 _â¨ Python ç¼åç [TsuguBanGDreamBot](https://github.com/Yamamoto-2/tsugu-
          bangdream-bot?tab=readme-ov-file) èªç¶è¯­è¨äº¤äºåº â¨_
                           _[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]
---- ```shell pip install tsugu ``` > API Powered by _t_s_u_g_u_-_a_p_i_-_p_y_t_h_o_n > Command
-matching by _A_l_c_o_n_n_a *** ## handler - `handler`
+--- ```shell pip install tsugu ``` > API powered by _t_s_u_g_u_-_a_p_i_-_p_y_t_h_o_n > Command
+matching provided by _A_l_c_o_n_n_a *** ## handler - `handler`
 ç¨äºç´æ¥å¤çç¨æ·è¾å¥çèªç¶è¯­è¨å¹¶è¿åæ¥è¯¢ç»æ: ```python
 import tsugu # åä¸ªåæ°ï¼åå«æå³ç æ¶æ¯åå®¹ ç¨æ·id å¹³å°
 é¢éid for i in tsugu.handler(message='æ¥å¡ ars 1x', user_id='1528593481',
 platform='red', channel_id='666808414'): print('ææ¬: ',i) if isinstance(i,
 str) else None print(f"[å¾ç]") if isinstance(i, bytes) else None ```
 ```python import tsugu_async ... ``` > å¨å¸¸ç¨çqqbotä¸­ï¼ç¾¤å·å°±æ¯
 `channel_id`ã > å½ä½ ä½¿ç¨QQå·ä½ä¸º `user_id` æ¶ï¼`platform`
@@ -38,21 +38,21 @@
 Falseã ''' settings.use_easy_bg = True '''
 æ¯å¦ä½¿ç¨ç®æèæ¯ï¼ä½¿ç¨å¯å¨éä½èæ¯è´¨éçåæä¸å å¿«ååºéåº¦ã
 é»è®¤ä¸º
 Trueï¼å³ä½¿ç¨ç®æèæ¯ãè¥ä¸ä½¿ç¨ç®æèæ¯ï¼å¯å°æ­¤é¡¹è®¾ç½®ä¸º
 Falseã ''' settings.compress = True '''
 æ¯å¦åç¼©è¿åæ°æ®ï¼åç¼©å¯åå°è¿åæ°æ®å¤§å°ã é»è®¤ä¸º
 Trueï¼å³åç¼©è¿åæ°æ®ãè¥ä¸åç¼©è¿åæ°æ®ï¼å¯å°æ­¤é¡¹è®¾ç½®ä¸º
-Falseã ''' ``` ### tsugu_async config ```py from tsugu import config
-config.compact = True ''' æ¯å¦åè®¸å½ä»¤ä¸åæ°ä¹é´æ²¡æç©ºæ ¼ '''
+Falseã ''' ``` ### tsugu config ```py from tsugu import config config.compact
+= True ''' æ¯å¦åè®¸å½ä»¤ä¸åæ°ä¹é´æ²¡æç©ºæ ¼ '''
 config.remote_data_max_retry = 3 ''' è·åè¿ç¨ç¨æ·æ°æ®æå¤§éè¯æ¬¡æ°
 ''' config.bandori_station_token_name = "Tsugu" ''' bandori station token '''
 config.bandori_station_token = "ZtV4EX2K9Onb" ''' bandori station token '''
 config.disable_gacha_simulate_group_ids = [] ''' éè¦å³é­æ¨¡ææ½å¡çç¾¤
-''' ``` ```py from tsugu_async import config ... # ä¸ä¸é¢ç¸å ``` ***
-?å?®?¢?æ???ð???±?æ???å?¯?¼((?è?¿??é???å??¯?ä?»?¥?ç??¹?å??»))
+''' ``` ### tsugu_async config ```py from tsugu_async import config ... # ä¸
+tsugu config ç¸å ``` *** ?å?®?¢?æ???ð???±?æ???å?¯?¼((?è?¿??é???å??¯?ä?»?¥?ç??¹?å??»))
 **æ³¨æï¼å¦æä½ ä¸ç¥éä»ä¹æ¯BanGDreamï¼è¯·ä¸è¦éæå ç¾¤**
 **æ¬ç¾¤è¿æ¯æ¬¢è¿å ç¾¤çï¼** [BanGDreamBotå¼åèå¤©ç¾¤](https://
 qm.qq.com/q/zjUPQkrdpm) æ¸©é¦¨çèå¤©ç¯å¢ï½ --- Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8 Description-Content-Type: text/markdown
```

### Comparing `tsugu-1.1.0rc1/tsugu.egg-info/SOURCES.txt` & `tsugu-1.1.0rc2/tsugu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc1/tsugu_async/handler.py` & `tsugu-1.1.0rc2/tsugu_async/handler.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc1/tsugu_async/router/bandoristation/rooms_forward.py` & `tsugu-1.1.0rc2/tsugu_async/router/bandoristation/rooms_forward.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc1/tsugu_async/router/bandoristation/ycm.py` & `tsugu-1.1.0rc2/tsugu_async/router/bandoristation/ycm.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc1/tsugu_async/router/remote/bind_player.py` & `tsugu-1.1.0rc2/tsugu_async/router/remote/bind_player.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc1/tsugu_async/router/remote/bind_player_verification_off.py` & `tsugu-1.1.0rc2/tsugu_async/router/remote/bind_player_verification_off.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc1/tsugu_async/router/remote/bind_player_verification_on.py` & `tsugu-1.1.0rc2/tsugu_async/router/remote/bind_player_verification_on.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc1/tsugu_async/router/remote/change_default_server.py` & `tsugu-1.1.0rc2/tsugu_async/router/remote/change_default_server.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc1/tsugu_async/router/remote/change_server_mode.py` & `tsugu-1.1.0rc2/tsugu_async/router/remote/change_server_mode.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc1/tsugu_async/router/remote/player_status.py` & `tsugu-1.1.0rc2/tsugu_async/router/remote/player_status.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc1/tsugu_async/router/remote/switch_car_forwarding_off.py` & `tsugu-1.1.0rc2/tsugu_async/router/remote/switch_car_forwarding_off.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc1/tsugu_async/router/remote/switch_car_forwarding_on.py` & `tsugu-1.1.0rc2/tsugu_async/router/remote/switch_car_forwarding_on.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc1/tsugu_async/router/remote/unbind_player.py` & `tsugu-1.1.0rc2/tsugu_async/router/remote/unbind_player.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc1/tsugu_async/router/universal/event_stage.py` & `tsugu-1.1.0rc2/tsugu_async/router/universal/event_stage.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc1/tsugu_async/router/universal/gacha_simulate.py` & `tsugu-1.1.0rc2/tsugu_async/router/universal/gacha_simulate.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc1/tsugu_async/router/universal/get_card_illustration.py` & `tsugu-1.1.0rc2/tsugu_async/router/universal/get_card_illustration.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc1/tsugu_async/router/universal/lsycx.py` & `tsugu-1.1.0rc2/tsugu_async/router/universal/lsycx.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc1/tsugu_async/router/universal/search_card.py` & `tsugu-1.1.0rc2/tsugu_async/router/universal/search_card.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc1/tsugu_async/router/universal/search_character.py` & `tsugu-1.1.0rc2/tsugu_async/router/universal/search_character.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc1/tsugu_async/router/universal/search_event.py` & `tsugu-1.1.0rc2/tsugu_async/router/universal/search_event.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc1/tsugu_async/router/universal/search_gacha.py` & `tsugu-1.1.0rc2/tsugu_async/router/universal/search_gacha.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc1/tsugu_async/router/universal/search_player.py` & `tsugu-1.1.0rc2/tsugu_async/router/universal/search_player.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc1/tsugu_async/router/universal/search_song.py` & `tsugu-1.1.0rc2/tsugu_async/router/universal/search_song.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc1/tsugu_async/router/universal/song_chart.py` & `tsugu-1.1.0rc2/tsugu_async/router/universal/song_chart.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc1/tsugu_async/router/universal/song_meta.py` & `tsugu-1.1.0rc2/tsugu_async/router/universal/song_meta.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc1/tsugu_async/router/universal/ycx.py` & `tsugu-1.1.0rc2/tsugu_async/router/universal/ycx.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc1/tsugu_async/router/universal/ycx_all.py` & `tsugu-1.1.0rc2/tsugu_async/router/universal/ycx_all.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc1/tsugu_async/utils/__init__.py` & `tsugu-1.1.0rc2/tsugu_async/utils/__init__.py`

 * *Files identical despite different names*

