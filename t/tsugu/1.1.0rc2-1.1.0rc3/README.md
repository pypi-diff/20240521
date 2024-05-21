# Comparing `tmp/tsugu-1.1.0rc2.tar.gz` & `tmp/tsugu-1.1.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsugu-1.1.0rc2.tar", last modified: Tue May 21 02:56:22 2024, max compression
+gzip compressed data, was "tsugu-1.1.0rc3.tar", last modified: Tue May 21 03:40:11 2024, max compression
```

## Comparing `tsugu-1.1.0rc2.tar` & `tsugu-1.1.0rc3.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 02:56:22.221635 tsugu-1.1.0rc2/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6443 2024-05-21 02:56:22.221635 tsugu-1.1.0rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4482 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 02:56:22.221635 tsugu-1.1.0rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 02:56:22.209635 tsugu-1.1.0rc2/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/test/test_async.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 02:56:22.209635 tsugu-1.1.0rc2/tsugu/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 02:56:22.209635 tsugu-1.1.0rc2/tsugu/router/
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu/router/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 02:56:22.209635 tsugu-1.1.0rc2/tsugu/router/bandoristation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu/router/bandoristation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2841 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu/router/bandoristation/rooms_forward.py
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu/router/bandoristation/ycm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 02:56:22.213635 tsugu-1.1.0rc2/tsugu/router/remote/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu/router/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu/router/remote/bind_player.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu/router/remote/bind_player_verification_off.py
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu/router/remote/bind_player_verification_on.py
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu/router/remote/change_default_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu/router/remote/change_server_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu/router/remote/player_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu/router/remote/switch_car_forwarding_off.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu/router/remote/switch_car_forwarding_on.py
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu/router/remote/unbind_player.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 02:56:22.213635 tsugu-1.1.0rc2/tsugu/router/universal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu/router/universal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu/router/universal/event_stage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu/router/universal/gacha_simulate.py
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu/router/universal/get_card_illustration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu/router/universal/lsycx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu/router/universal/search_card.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu/router/universal/search_character.py
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu/router/universal/search_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu/router/universal/search_gacha.py
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu/router/universal/search_player.py
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu/router/universal/search_song.py
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu/router/universal/song_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu/router/universal/song_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu/router/universal/ycx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu/router/universal/ycx_all.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 02:56:22.213635 tsugu-1.1.0rc2/tsugu/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 02:56:22.209635 tsugu-1.1.0rc2/tsugu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6443 2024-05-21 02:56:22.000000 tsugu-1.1.0rc2/tsugu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-05-21 02:56:22.000000 tsugu-1.1.0rc2/tsugu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 02:56:22.000000 tsugu-1.1.0rc2/tsugu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-21 02:56:22.000000 tsugu-1.1.0rc2/tsugu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-21 02:56:22.000000 tsugu-1.1.0rc2/tsugu.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 02:56:22.217635 tsugu-1.1.0rc2/tsugu_async/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu_async/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu_async/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu_async/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 02:56:22.217635 tsugu-1.1.0rc2/tsugu_async/router/
--rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu_async/router/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 02:56:22.217635 tsugu-1.1.0rc2/tsugu_async/router/bandoristation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu_async/router/bandoristation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu_async/router/bandoristation/rooms_forward.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu_async/router/bandoristation/ycm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 02:56:22.217635 tsugu-1.1.0rc2/tsugu_async/router/remote/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu_async/router/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu_async/router/remote/bind_player.py
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu_async/router/remote/bind_player_verification_off.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu_async/router/remote/bind_player_verification_on.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu_async/router/remote/change_default_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu_async/router/remote/change_server_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu_async/router/remote/player_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu_async/router/remote/switch_car_forwarding_off.py
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu_async/router/remote/switch_car_forwarding_on.py
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu_async/router/remote/unbind_player.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 02:56:22.221635 tsugu-1.1.0rc2/tsugu_async/router/universal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu_async/router/universal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu_async/router/universal/event_stage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu_async/router/universal/gacha_simulate.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu_async/router/universal/get_card_illustration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu_async/router/universal/lsycx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu_async/router/universal/search_card.py
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu_async/router/universal/search_character.py
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu_async/router/universal/search_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu_async/router/universal/search_gacha.py
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu_async/router/universal/search_player.py
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu_async/router/universal/search_song.py
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu_async/router/universal/song_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu_async/router/universal/song_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu_async/router/universal/ycx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu_async/router/universal/ycx_all.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 02:56:22.221635 tsugu-1.1.0rc2/tsugu_async/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-05-21 02:56:13.000000 tsugu-1.1.0rc2/tsugu_async/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 03:40:11.114071 tsugu-1.1.0rc3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6443 2024-05-21 03:40:11.114071 tsugu-1.1.0rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4482 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 03:40:11.114071 tsugu-1.1.0rc3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 03:40:11.106071 tsugu-1.1.0rc3/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/test/test_async.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 03:40:11.106071 tsugu-1.1.0rc3/tsugu/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 03:40:11.106071 tsugu-1.1.0rc3/tsugu/router/
+-rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu/router/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 03:40:11.106071 tsugu-1.1.0rc3/tsugu/router/bandoristation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu/router/bandoristation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2841 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu/router/bandoristation/rooms_forward.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu/router/bandoristation/ycm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 03:40:11.106071 tsugu-1.1.0rc3/tsugu/router/remote/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu/router/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu/router/remote/bind_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu/router/remote/bind_player_verification_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu/router/remote/bind_player_verification_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu/router/remote/change_default_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu/router/remote/change_server_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu/router/remote/player_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu/router/remote/switch_car_forwarding_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu/router/remote/switch_car_forwarding_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu/router/remote/unbind_player.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 03:40:11.110071 tsugu-1.1.0rc3/tsugu/router/universal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu/router/universal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu/router/universal/event_stage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu/router/universal/gacha_simulate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu/router/universal/get_card_illustration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu/router/universal/lsycx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu/router/universal/search_card.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu/router/universal/search_character.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu/router/universal/search_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu/router/universal/search_gacha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu/router/universal/search_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu/router/universal/search_song.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu/router/universal/song_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu/router/universal/song_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu/router/universal/ycx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu/router/universal/ycx_all.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 03:40:11.110071 tsugu-1.1.0rc3/tsugu/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 03:40:11.106071 tsugu-1.1.0rc3/tsugu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6443 2024-05-21 03:40:10.000000 tsugu-1.1.0rc3/tsugu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-05-21 03:40:11.000000 tsugu-1.1.0rc3/tsugu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 03:40:10.000000 tsugu-1.1.0rc3/tsugu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-21 03:40:10.000000 tsugu-1.1.0rc3/tsugu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-21 03:40:10.000000 tsugu-1.1.0rc3/tsugu.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 03:40:11.110071 tsugu-1.1.0rc3/tsugu_async/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu_async/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu_async/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu_async/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 03:40:11.110071 tsugu-1.1.0rc3/tsugu_async/router/
+-rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu_async/router/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 03:40:11.110071 tsugu-1.1.0rc3/tsugu_async/router/bandoristation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu_async/router/bandoristation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu_async/router/bandoristation/rooms_forward.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu_async/router/bandoristation/ycm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 03:40:11.110071 tsugu-1.1.0rc3/tsugu_async/router/remote/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu_async/router/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu_async/router/remote/bind_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu_async/router/remote/bind_player_verification_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu_async/router/remote/bind_player_verification_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu_async/router/remote/change_default_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu_async/router/remote/change_server_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu_async/router/remote/player_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu_async/router/remote/switch_car_forwarding_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu_async/router/remote/switch_car_forwarding_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu_async/router/remote/unbind_player.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 03:40:11.114071 tsugu-1.1.0rc3/tsugu_async/router/universal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu_async/router/universal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu_async/router/universal/event_stage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu_async/router/universal/gacha_simulate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu_async/router/universal/get_card_illustration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu_async/router/universal/lsycx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu_async/router/universal/search_card.py
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu_async/router/universal/search_character.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu_async/router/universal/search_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu_async/router/universal/search_gacha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu_async/router/universal/search_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu_async/router/universal/search_song.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu_async/router/universal/song_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu_async/router/universal/song_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu_async/router/universal/ycx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu_async/router/universal/ycx_all.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 03:40:11.114071 tsugu-1.1.0rc3/tsugu_async/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-05-21 03:39:58.000000 tsugu-1.1.0rc3/tsugu_async/utils/__init__.py
```

### Comparing `tsugu-1.1.0rc2/LICENSE` & `tsugu-1.1.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc2/PKG-INFO` & `tsugu-1.1.0rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu
-Version: 1.1.0rc2
+Version: 1.1.0rc3
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
-Metadata-Version: 2.1 Name: tsugu Version: 1.1.0rc2 Summary: Tsugu Python
+Metadata-Version: 2.1 Name: tsugu Version: 1.1.0rc3 Summary: Tsugu Python
 Frontend Home-page: https://github.com/kumoSleeping/ChatTsuguPy Author:
 kumoSleeping Author-email: zjr2992@outlook.com License: MIT Description:
                        ************ CChhaatt TTssuugguu PPyy[[ttmmrrnn]] ************
 _â¨ Python ç¼åç [TsuguBanGDreamBot](https://github.com/Yamamoto-2/tsugu-
          bangdream-bot?tab=readme-ov-file) èªç¶è¯­è¨äº¤äºåº â¨_
                           _[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]
 --- ```shell pip install tsugu ``` > API powered by _t_s_u_g_u_-_a_p_i_-_p_y_t_h_o_n > Command
```

### Comparing `tsugu-1.1.0rc2/README.md` & `tsugu-1.1.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc2/setup.py` & `tsugu-1.1.0rc3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r') as readme:
     long_description = readme.read()
 
 setup(
     name='tsugu',
-    version='1.1.0-rc2',
+    version='1.1.0-rc3',
     author='kumoSleeping',
     author_email='zjr2992@outlook.com',
     license="MIT",
     description='Tsugu Python Frontend',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/kumoSleeping/ChatTsuguPy',
```

### Comparing `tsugu-1.1.0rc2/test/test_async.py` & `tsugu-1.1.0rc3/test/test_async.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,21 +24,21 @@
         # from tsugu_api_async import settings
         # settings.backend_url = 'http://127.0.0.1:8010'
         from tsugu_api_async import settings
 
         # settings.backend_url = 'http://124.221.153.148:3000'
         # settings.userdata_backend_url = 'http://127.0.0.1:3001'
 
-        msg1 = await tsugu_async.handler('查活动 蓝 ag', '1528593481', 'red', '666808414')
+        msg1 = await tsugu_async.handler('查活动 -h', '1528593481', 'red', '666808414')
         await show_back_msg(msg1)
 
-        # msg2 = await tsugu_async.handler('ycm', '1528593481', 'red', '666808414')
-        # await show_back_msg(msg2)
+        msg2 = await tsugu_async.handler('查活动 -h', '1528593481', 'red', '666808414')
+        await show_back_msg(msg2)
 
-        # msg3 = await tsugu_async.handler('12324 测q1试', '1528593481', 'red', '666808414')
-        # await show_back_msg(msg3)
+        msg3 = await tsugu_async.handler('查活动 -h', '1528593481', 'red', '666808414')
+        await show_back_msg(msg3)
 
         # print(tsugu_api.get_user_data('red', '1528593481'))
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `tsugu-1.1.0rc2/tsugu/handler.py` & `tsugu-1.1.0rc3/tsugu/handler.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc2/tsugu/router/__init__.py` & `tsugu-1.1.0rc3/tsugu/router/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import importlib
 from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, output_manager, command_manager
 from ..utils import text_response, get_user
+import threading
 
 
 def require(module_path, cmd):
     globals()[cmd] = importlib.import_module(module_path.format(cmd=cmd), __package__)
 
 
 universal_list = [
@@ -44,31 +45,44 @@
 
 # 导入模块
 [require(f'.universal.{cmd}', cmd) for cmd in universal_list]
 [require(f'.remote.{cmd}', cmd) for cmd in remote_commands]
 [require(f'.bandoristation.{cmd}', cmd) for cmd in bandoristation_commands]
 
 
+class ThisValue:
+    def __init__(self):
+        self.local_data = threading.local()
+
+    def set_h(self, value):
+        self.local_data.h = value
+
+    def get_h(self):
+        return getattr(self.local_data, 'h', None)
+
+
+this_value = ThisValue()
+
+
 def handler(message, user_id, platform, channel_id):
     user = get_user(user_id, platform)
-    alc_output = None
 
     def set_output_str(arg):
-        nonlocal alc_output
-        alc_output = arg
+        # 为每个线程设置独立的 h 值
+        this_value.set_h(arg)
 
     output_manager.set_action(set_output_str)
 
     def handler_feats(cmd_list):
         for i in cmd_list:
             result = getattr(globals()[i], 'handler')(message, user, platform, channel_id)
             if not result:
                 continue
             if result[0].get('type') == 'string' and result[0].get('string') == 'help':
-                return text_response(alc_output)
+                return text_response(this_value.get_h())
             return result
         return None
 
     res = handler_feats(universal_list)
     if res:
         return res
```

### Comparing `tsugu-1.1.0rc2/tsugu/router/bandoristation/rooms_forward.py` & `tsugu-1.1.0rc3/tsugu/router/bandoristation/rooms_forward.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc2/tsugu/router/bandoristation/ycm.py` & `tsugu-1.1.0rc3/tsugu/router/bandoristation/ycm.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc2/tsugu/router/remote/bind_player.py` & `tsugu-1.1.0rc3/tsugu/router/remote/bind_player.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc2/tsugu/router/remote/bind_player_verification_off.py` & `tsugu-1.1.0rc3/tsugu/router/remote/bind_player_verification_off.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc2/tsugu/router/remote/bind_player_verification_on.py` & `tsugu-1.1.0rc3/tsugu/router/remote/bind_player_verification_on.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc2/tsugu/router/remote/change_default_server.py` & `tsugu-1.1.0rc3/tsugu/router/remote/change_default_server.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc2/tsugu/router/remote/change_server_mode.py` & `tsugu-1.1.0rc3/tsugu/router/remote/change_server_mode.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc2/tsugu/router/remote/player_status.py` & `tsugu-1.1.0rc3/tsugu/router/remote/player_status.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc2/tsugu/router/remote/switch_car_forwarding_off.py` & `tsugu-1.1.0rc3/tsugu/router/remote/switch_car_forwarding_off.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc2/tsugu/router/remote/switch_car_forwarding_on.py` & `tsugu-1.1.0rc3/tsugu/router/remote/switch_car_forwarding_on.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc2/tsugu/router/remote/unbind_player.py` & `tsugu-1.1.0rc3/tsugu/router/remote/unbind_player.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc2/tsugu/router/universal/event_stage.py` & `tsugu-1.1.0rc3/tsugu/router/universal/event_stage.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc2/tsugu/router/universal/gacha_simulate.py` & `tsugu-1.1.0rc3/tsugu/router/universal/gacha_simulate.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc2/tsugu/router/universal/get_card_illustration.py` & `tsugu-1.1.0rc3/tsugu/router/universal/get_card_illustration.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc2/tsugu/router/universal/lsycx.py` & `tsugu-1.1.0rc3/tsugu/router/universal/lsycx.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc2/tsugu/router/universal/search_card.py` & `tsugu-1.1.0rc3/tsugu/router/universal/search_card.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc2/tsugu/router/universal/search_character.py` & `tsugu-1.1.0rc3/tsugu/router/universal/search_character.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc2/tsugu/router/universal/search_event.py` & `tsugu-1.1.0rc3/tsugu/router/universal/search_event.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc2/tsugu/router/universal/search_gacha.py` & `tsugu-1.1.0rc3/tsugu/router/universal/search_gacha.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc2/tsugu/router/universal/search_player.py` & `tsugu-1.1.0rc3/tsugu/router/universal/search_player.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc2/tsugu/router/universal/search_song.py` & `tsugu-1.1.0rc3/tsugu/router/universal/search_song.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc2/tsugu/router/universal/song_chart.py` & `tsugu-1.1.0rc3/tsugu/router/universal/song_chart.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc2/tsugu/router/universal/song_meta.py` & `tsugu-1.1.0rc3/tsugu/router/universal/song_meta.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc2/tsugu/router/universal/ycx.py` & `tsugu-1.1.0rc3/tsugu/router/universal/ycx.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc2/tsugu/router/universal/ycx_all.py` & `tsugu-1.1.0rc3/tsugu/router/universal/ycx_all.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc2/tsugu/utils/__init__.py` & `tsugu-1.1.0rc3/tsugu/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc2/tsugu.egg-info/PKG-INFO` & `tsugu-1.1.0rc3/tsugu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu
-Version: 1.1.0rc2
+Version: 1.1.0rc3
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
-Metadata-Version: 2.1 Name: tsugu Version: 1.1.0rc2 Summary: Tsugu Python
+Metadata-Version: 2.1 Name: tsugu Version: 1.1.0rc3 Summary: Tsugu Python
 Frontend Home-page: https://github.com/kumoSleeping/ChatTsuguPy Author:
 kumoSleeping Author-email: zjr2992@outlook.com License: MIT Description:
                        ************ CChhaatt TTssuugguu PPyy[[ttmmrrnn]] ************
 _â¨ Python ç¼åç [TsuguBanGDreamBot](https://github.com/Yamamoto-2/tsugu-
          bangdream-bot?tab=readme-ov-file) èªç¶è¯­è¨äº¤äºåº â¨_
                           _[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]
 --- ```shell pip install tsugu ``` > API powered by _t_s_u_g_u_-_a_p_i_-_p_y_t_h_o_n > Command
```

### Comparing `tsugu-1.1.0rc2/tsugu.egg-info/SOURCES.txt` & `tsugu-1.1.0rc3/tsugu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc2/tsugu_async/handler.py` & `tsugu-1.1.0rc3/tsugu_async/handler.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc2/tsugu_async/router/__init__.py` & `tsugu-1.1.0rc3/tsugu_async/router/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import importlib
 from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, output_manager, command_manager
 from ..utils import text_response, get_user
+from contextvars import ContextVar
+from typing import Optional
 
 
 def require(module_path, cmd):
     globals()[cmd] = importlib.import_module(module_path.format(cmd=cmd), __package__)
 
 
 universal_list = [
@@ -44,31 +46,32 @@
 
 # 导入模块
 [require(f'.universal.{cmd}', cmd) for cmd in universal_list]
 [require(f'.remote.{cmd}', cmd) for cmd in remote_commands]
 [require(f'.bandoristation.{cmd}', cmd) for cmd in bandoristation_commands]
 
 
+this_value_h: ContextVar[Optional[str]] = ContextVar('this_value_h', default=None)
+
+
 async def handler(message, user_id, platform, channel_id):
     user = await get_user(user_id, platform)
-    alc_output = None
 
     def set_output_str(arg):
-        nonlocal alc_output
-        alc_output = arg
+        this_value_h.set(arg)
 
     output_manager.set_action(set_output_str)
 
     async def handler_feats(cmd_list):
         for i in cmd_list:
             result = await getattr(globals()[i], 'handler')(message, user, platform, channel_id)
             if not result:
                 continue
             if result[0].get('type') == 'string' and result[0].get('string') == 'help':
-                return text_response(alc_output)
+                return text_response(this_value_h.get())
             return result
         return None
 
     res = await handler_feats(universal_list)
     if res:
         return res
 
@@ -77,10 +80,10 @@
         return res
 
     res = await handler_feats(bandoristation_commands)
     if res:
         return res
 
     if message in ["help", "帮助"]:
-        return text_response(command_manager.all_command_help(show_index=True))
+        return text_response(command_manager.all_command_help(show_index=True) + "例如: 查卡 -h")
 
     return None
```

### Comparing `tsugu-1.1.0rc2/tsugu_async/router/bandoristation/rooms_forward.py` & `tsugu-1.1.0rc3/tsugu_async/router/bandoristation/rooms_forward.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc2/tsugu_async/router/bandoristation/ycm.py` & `tsugu-1.1.0rc3/tsugu_async/router/bandoristation/ycm.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc2/tsugu_async/router/remote/bind_player.py` & `tsugu-1.1.0rc3/tsugu_async/router/remote/bind_player.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc2/tsugu_async/router/remote/bind_player_verification_off.py` & `tsugu-1.1.0rc3/tsugu_async/router/remote/bind_player_verification_off.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc2/tsugu_async/router/remote/bind_player_verification_on.py` & `tsugu-1.1.0rc3/tsugu_async/router/remote/bind_player_verification_on.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc2/tsugu_async/router/remote/change_default_server.py` & `tsugu-1.1.0rc3/tsugu_async/router/remote/change_default_server.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc2/tsugu_async/router/remote/change_server_mode.py` & `tsugu-1.1.0rc3/tsugu_async/router/remote/change_server_mode.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc2/tsugu_async/router/remote/player_status.py` & `tsugu-1.1.0rc3/tsugu_async/router/remote/player_status.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc2/tsugu_async/router/remote/switch_car_forwarding_off.py` & `tsugu-1.1.0rc3/tsugu_async/router/remote/switch_car_forwarding_off.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc2/tsugu_async/router/remote/switch_car_forwarding_on.py` & `tsugu-1.1.0rc3/tsugu_async/router/remote/switch_car_forwarding_on.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc2/tsugu_async/router/remote/unbind_player.py` & `tsugu-1.1.0rc3/tsugu_async/router/remote/unbind_player.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc2/tsugu_async/router/universal/event_stage.py` & `tsugu-1.1.0rc3/tsugu_async/router/universal/event_stage.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc2/tsugu_async/router/universal/gacha_simulate.py` & `tsugu-1.1.0rc3/tsugu_async/router/universal/gacha_simulate.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc2/tsugu_async/router/universal/get_card_illustration.py` & `tsugu-1.1.0rc3/tsugu_async/router/universal/get_card_illustration.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc2/tsugu_async/router/universal/lsycx.py` & `tsugu-1.1.0rc3/tsugu_async/router/universal/lsycx.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc2/tsugu_async/router/universal/search_card.py` & `tsugu-1.1.0rc3/tsugu_async/router/universal/search_card.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc2/tsugu_async/router/universal/search_character.py` & `tsugu-1.1.0rc3/tsugu_async/router/universal/search_character.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc2/tsugu_async/router/universal/search_event.py` & `tsugu-1.1.0rc3/tsugu_async/router/universal/search_event.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc2/tsugu_async/router/universal/search_gacha.py` & `tsugu-1.1.0rc3/tsugu_async/router/universal/search_gacha.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc2/tsugu_async/router/universal/search_player.py` & `tsugu-1.1.0rc3/tsugu_async/router/universal/search_player.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc2/tsugu_async/router/universal/search_song.py` & `tsugu-1.1.0rc3/tsugu_async/router/universal/search_song.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc2/tsugu_async/router/universal/song_chart.py` & `tsugu-1.1.0rc3/tsugu_async/router/universal/song_chart.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc2/tsugu_async/router/universal/song_meta.py` & `tsugu-1.1.0rc3/tsugu_async/router/universal/song_meta.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc2/tsugu_async/router/universal/ycx.py` & `tsugu-1.1.0rc3/tsugu_async/router/universal/ycx.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc2/tsugu_async/router/universal/ycx_all.py` & `tsugu-1.1.0rc3/tsugu_async/router/universal/ycx_all.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc2/tsugu_async/utils/__init__.py` & `tsugu-1.1.0rc3/tsugu_async/utils/__init__.py`

 * *Files identical despite different names*

