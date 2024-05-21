# Comparing `tmp/tsugu-1.1.0rc5.tar.gz` & `tmp/tsugu-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsugu-1.1.0rc5.tar", last modified: Tue May 21 10:06:26 2024, max compression
+gzip compressed data, was "tsugu-2.0.0.tar", last modified: Tue May 21 12:25:15 2024, max compression
```

## Comparing `tsugu-1.1.0rc5.tar` & `tsugu-2.0.0.tar`

### file list

```diff
@@ -1,137 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:26.384228 tsugu-1.1.0rc5/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6716 2024-05-21 10:06:26.384228 tsugu-1.1.0rc5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 10:06:26.384228 tsugu-1.1.0rc5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:26.372228 tsugu-1.1.0rc5/tsugu/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:26.372228 tsugu-1.1.0rc5/tsugu/src/
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:26.372228 tsugu-1.1.0rc5/tsugu/src/bandoristation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu/src/bandoristation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu/src/bandoristation/rooms_forward.py
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu/src/bandoristation/ycm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:26.372228 tsugu-1.1.0rc5/tsugu/src/help/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu/src/help/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu/src/help/help.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:26.372228 tsugu-1.1.0rc5/tsugu/src/remote/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu/src/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu/src/remote/bind_player.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu/src/remote/bind_player_verification_off.py
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu/src/remote/bind_player_verification_on.py
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu/src/remote/change_default_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu/src/remote/change_server_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu/src/remote/player_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu/src/remote/switch_car_forwarding_off.py
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu/src/remote/switch_car_forwarding_on.py
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu/src/remote/unbind_player.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:26.376228 tsugu-1.1.0rc5/tsugu/src/universal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu/src/universal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu/src/universal/event_stage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu/src/universal/gacha_simulate.py
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu/src/universal/get_card_illustration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu/src/universal/lsycx.py
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu/src/universal/search_card.py
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu/src/universal/search_character.py
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu/src/universal/search_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu/src/universal/search_gacha.py
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu/src/universal/search_player.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu/src/universal/search_song.py
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu/src/universal/song_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu/src/universal/song_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu/src/universal/ycx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu/src/universal/ycx_all.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:26.376228 tsugu-1.1.0rc5/tsugu/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     3292 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:26.372228 tsugu-1.1.0rc5/tsugu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6716 2024-05-21 10:06:26.000000 tsugu-1.1.0rc5/tsugu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4139 2024-05-21 10:06:26.000000 tsugu-1.1.0rc5/tsugu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 10:06:26.000000 tsugu-1.1.0rc5/tsugu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-21 10:06:26.000000 tsugu-1.1.0rc5/tsugu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-21 10:06:26.000000 tsugu-1.1.0rc5/tsugu.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:26.376228 tsugu-1.1.0rc5/tsugu_async/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_async/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_async/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_async/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:26.376228 tsugu-1.1.0rc5/tsugu_async/src/
--rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_async/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:26.376228 tsugu-1.1.0rc5/tsugu_async/src/bandoristation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_async/src/bandoristation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_async/src/bandoristation/rooms_forward.py
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_async/src/bandoristation/ycm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:26.376228 tsugu-1.1.0rc5/tsugu_async/src/help/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_async/src/help/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_async/src/help/help.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:26.380228 tsugu-1.1.0rc5/tsugu_async/src/remote/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_async/src/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_async/src/remote/bind_player.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_async/src/remote/bind_player_verification_off.py
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_async/src/remote/bind_player_verification_on.py
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_async/src/remote/change_default_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_async/src/remote/change_server_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_async/src/remote/player_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_async/src/remote/switch_car_forwarding_off.py
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_async/src/remote/switch_car_forwarding_on.py
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_async/src/remote/unbind_player.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:26.380228 tsugu-1.1.0rc5/tsugu_async/src/universal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_async/src/universal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_async/src/universal/event_stage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_async/src/universal/gacha_simulate.py
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_async/src/universal/get_card_illustration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_async/src/universal/lsycx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_async/src/universal/search_card.py
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_async/src/universal/search_character.py
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_async/src/universal/search_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_async/src/universal/search_gacha.py
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_async/src/universal/search_player.py
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_async/src/universal/search_song.py
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_async/src/universal/song_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_async/src/universal/song_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_async/src/universal/ycx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_async/src/universal/ycx_all.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:26.380228 tsugu-1.1.0rc5/tsugu_async/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_async/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:26.380228 tsugu-1.1.0rc5/tsugu_thread/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_thread/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_thread/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:26.380228 tsugu-1.1.0rc5/tsugu_thread/src/
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_thread/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:26.380228 tsugu-1.1.0rc5/tsugu_thread/src/bandoristation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_thread/src/bandoristation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_thread/src/bandoristation/rooms_forward.py
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_thread/src/bandoristation/ycm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:26.380228 tsugu-1.1.0rc5/tsugu_thread/src/help/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_thread/src/help/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_thread/src/help/help.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:26.384228 tsugu-1.1.0rc5/tsugu_thread/src/remote/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_thread/src/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_thread/src/remote/bind_player.py
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_thread/src/remote/bind_player_verification_off.py
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_thread/src/remote/bind_player_verification_on.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_thread/src/remote/change_default_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_thread/src/remote/change_server_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_thread/src/remote/player_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_thread/src/remote/switch_car_forwarding_off.py
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_thread/src/remote/switch_car_forwarding_on.py
--rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_thread/src/remote/unbind_player.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:26.384228 tsugu-1.1.0rc5/tsugu_thread/src/universal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_thread/src/universal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_thread/src/universal/event_stage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_thread/src/universal/gacha_simulate.py
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_thread/src/universal/get_card_illustration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_thread/src/universal/lsycx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_thread/src/universal/search_card.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_thread/src/universal/search_character.py
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_thread/src/universal/search_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_thread/src/universal/search_gacha.py
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_thread/src/universal/search_player.py
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_thread/src/universal/search_song.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_thread/src/universal/song_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_thread/src/universal/song_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_thread/src/universal/ycx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_thread/src/universal/ycx_all.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:26.384228 tsugu-1.1.0rc5/tsugu_thread/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     3237 2024-05-21 10:06:16.000000 tsugu-1.1.0rc5/tsugu_thread/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:25:15.090217 tsugu-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-21 12:25:02.000000 tsugu-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-05-21 12:25:15.090217 tsugu-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-05-21 12:25:02.000000 tsugu-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 12:25:15.090217 tsugu-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-21 12:25:02.000000 tsugu-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:25:15.086217 tsugu-2.0.0/tsugu/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-21 12:25:02.000000 tsugu-2.0.0/tsugu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-05-21 12:25:02.000000 tsugu-2.0.0/tsugu/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:25:15.086217 tsugu-2.0.0/tsugu/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-05-21 12:25:02.000000 tsugu-2.0.0/tsugu/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:25:15.086217 tsugu-2.0.0/tsugu/src/bandoristation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 12:25:02.000000 tsugu-2.0.0/tsugu/src/bandoristation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4068 2024-05-21 12:25:02.000000 tsugu-2.0.0/tsugu/src/bandoristation/rooms_forward.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-05-21 12:25:02.000000 tsugu-2.0.0/tsugu/src/bandoristation/ycm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:25:15.086217 tsugu-2.0.0/tsugu/src/help/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 12:25:02.000000 tsugu-2.0.0/tsugu/src/help/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-05-21 12:25:02.000000 tsugu-2.0.0/tsugu/src/help/help.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:25:15.090217 tsugu-2.0.0/tsugu/src/remote/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 12:25:02.000000 tsugu-2.0.0/tsugu/src/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-21 12:25:02.000000 tsugu-2.0.0/tsugu/src/remote/bind_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-21 12:25:02.000000 tsugu-2.0.0/tsugu/src/remote/bind_player_verification_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-05-21 12:25:02.000000 tsugu-2.0.0/tsugu/src/remote/bind_player_verification_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-21 12:25:02.000000 tsugu-2.0.0/tsugu/src/remote/change_default_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-21 12:25:02.000000 tsugu-2.0.0/tsugu/src/remote/change_server_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5267 2024-05-21 12:25:02.000000 tsugu-2.0.0/tsugu/src/remote/player_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-21 12:25:02.000000 tsugu-2.0.0/tsugu/src/remote/switch_car_forwarding_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-21 12:25:02.000000 tsugu-2.0.0/tsugu/src/remote/switch_car_forwarding_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-05-21 12:25:02.000000 tsugu-2.0.0/tsugu/src/remote/unbind_player.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:25:15.090217 tsugu-2.0.0/tsugu/src/universal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 12:25:02.000000 tsugu-2.0.0/tsugu/src/universal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-21 12:25:02.000000 tsugu-2.0.0/tsugu/src/universal/event_stage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-05-21 12:25:02.000000 tsugu-2.0.0/tsugu/src/universal/gacha_simulate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-21 12:25:02.000000 tsugu-2.0.0/tsugu/src/universal/get_card_illustration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-21 12:25:02.000000 tsugu-2.0.0/tsugu/src/universal/lsycx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-05-21 12:25:02.000000 tsugu-2.0.0/tsugu/src/universal/search_card.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-21 12:25:02.000000 tsugu-2.0.0/tsugu/src/universal/search_character.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-21 12:25:02.000000 tsugu-2.0.0/tsugu/src/universal/search_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-21 12:25:02.000000 tsugu-2.0.0/tsugu/src/universal/search_gacha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-21 12:25:02.000000 tsugu-2.0.0/tsugu/src/universal/search_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-05-21 12:25:02.000000 tsugu-2.0.0/tsugu/src/universal/search_song.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-05-21 12:25:02.000000 tsugu-2.0.0/tsugu/src/universal/song_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-05-21 12:25:02.000000 tsugu-2.0.0/tsugu/src/universal/song_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-05-21 12:25:02.000000 tsugu-2.0.0/tsugu/src/universal/ycx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-21 12:25:02.000000 tsugu-2.0.0/tsugu/src/universal/ycx_all.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:25:15.090217 tsugu-2.0.0/tsugu/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     5067 2024-05-21 12:25:02.000000 tsugu-2.0.0/tsugu/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:25:15.086217 tsugu-2.0.0/tsugu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-05-21 12:25:14.000000 tsugu-2.0.0/tsugu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-21 12:25:14.000000 tsugu-2.0.0/tsugu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 12:25:14.000000 tsugu-2.0.0/tsugu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-21 12:25:14.000000 tsugu-2.0.0/tsugu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-21 12:25:14.000000 tsugu-2.0.0/tsugu.egg-info/top_level.txt
```

### Comparing `tsugu-1.1.0rc5/LICENSE` & `tsugu-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tsugu-1.1.0rc5/setup.py` & `tsugu-2.0.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r') as readme:
     long_description = readme.read()
 
 setup(
     name='tsugu',
-    version='1.1.0-rc5',
+    version='2.0.0',
     author='kumoSleeping',
     author_email='zjr2992@outlook.com',
     license="MIT",
     description='Tsugu Python Frontend',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/kumoSleeping/ChatTsuguPy',
@@ -18,13 +18,13 @@
         'Programming Language :: Python :: 3.8',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent'
     ],
     install_requires=[
             "loguru==0.7.2",
             "tsugu-api-python==1.2.0",
-            "arclet-alconna==1.8.12",
+            "arclet-alconna==1.8.13",
         ],
     python_requires='>=3.8',
     include_package_data=False,
 
 )
```

### Comparing `tsugu-1.1.0rc5/tsugu/handler.py` & `tsugu-2.0.0/tsugu/handler.py`

 * *Files 11% similar despite different names*

```diff
@@ -43,11 +43,49 @@
     try:
         return r if (r := src.handler(message, user_id, platform, channel_id)) else None
     except Exception as e:
         logger.error(f'Error: {e}')
         raise e
 
 
+async def handler_async(message: str, user_id: str, platform: str, channel_id: str) -> List[Union[bytes, str]]:
+    '''
+    Tsugu Handler Async
+    异步支持
+    处理用户输入的自然语言，返回处理后的结果
+
+    :param message: 用户消息
+    :param user_id: 用户ID
+    :param platform: 平台名称 一般为 red
+    :param channel_id: 频道ID / 群号
+    :return: List[Union[bytes, str]]
+    '''
+    try:
+        data = await handler_raw_async(message, user_id, platform, channel_id)
+        response = []
+        if not data:
+            return response
+        for item in data:
+            response.append(item['string']) if item['type'] == 'string' else None
+            response.append(base64.b64decode(item['string'].encode('utf-8')) if item['type'] == 'base64' else None)
+        return response
+    except Exception as e:
+        raise e
 
 
+async def handler_raw_async(message: str, user_id: str, platform: str, channel_id: str) -> List[Dict[str, str]]:
+    '''
+    handler_raw_async 除了返回的数据类型不同外，其他与 handler_async 函数一致
+    返回格式为 Tsugu 标准数据格式
+    :param message: 用户消息
+    :param user_id: 用户ID
+    :param platform: 平台名称 一般为 red
+    :param channel_id: 频道ID / 群号
+    :return: List[Dict[str, str]]
+    '''
+    try:
+        return r if (r := await src.handler_async(message, user_id, platform, channel_id)) else None
+    except Exception as e:
+        logger.error(f'Error: {e}')
+        raise e
```

### Comparing `tsugu-1.1.0rc5/tsugu/src/__init__.py` & `tsugu-2.0.0/tsugu/src/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import importlib
 from arclet.alconna import Arparma, output_manager, command_manager
-from ..utils import text_response, get_user
+from ..utils import text_response
 
 
 # 主要功能
 universal_list = [
     "get_card_illustration",
     "search_player",
     "gacha_simulate",
@@ -52,36 +52,58 @@
 
 # 导入模块
 [require(f'.universal.{cmd}', cmd) for cmd in universal_list]
 [require(f'.remote.{cmd}', cmd) for cmd in remote_commands]
 [require(f'.bandoristation.{cmd}', cmd) for cmd in bandoristation_commands]
 [require(f'.help.{cmd}', cmd) for cmd in help_command]
 
+output_manager.set_action(lambda *_: None)
+
 
 def handler(message, user_id, platform, channel_id):
-    user = get_user(user_id, platform)
-    output_manager.set_action(lambda *_: None)
     union_list = universal_list + remote_commands + bandoristation_commands + help_command
 
     for i in union_list:
-        result = getattr(globals()[i], 'handler')(message, user, platform, channel_id)
+        result = getattr(globals()[i], 'handler')(message, user_id, platform, channel_id)
 
         # 未生成结果
         if isinstance(result, Arparma):
             # 匹配了命令头
             if result.head_matched:
 
                 # 帮助信息
                 if result.error_data == ['-h']:
-                    return getattr(globals()['help'], 'handler')('help ' + result.header_result, user, platform, channel_id)
+                    return getattr(globals()['help'], 'handler')('help ' + result.header_result, user_id, platform, channel_id)
                 # 错误信息
                 else:
                     return text_response(result.error_info)
 
         # 已生成结果
         if isinstance(result, list):
             return result
 
     return None
 
 
+async def handler_async(message, user_id, platform, channel_id):
+    union_list = universal_list + remote_commands + bandoristation_commands + help_command
+
+    for i in union_list:
+        result = await getattr(globals()[i], 'handler_async')(message, user_id, platform, channel_id)
+
+        # 未生成结果
+        if isinstance(result, Arparma):
+            # 匹配了命令头
+            if result.head_matched:
+
+                # 帮助信息
+                if result.error_data == ['-h']:
+                    return await getattr(globals()['help'], 'handler_async')('help ' + result.header_result, user_id, platform, channel_id)
+                # 错误信息
+                else:
+                    return text_response(result.error_info)
+
+        # 已生成结果
+        if isinstance(result, list):
+            return result
 
+    return None
```

### Comparing `tsugu-1.1.0rc5/tsugu/src/bandoristation/rooms_forward.py` & `tsugu-2.0.0/tsugu/src/bandoristation/rooms_forward.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,64 @@
-from ...utils import text_response, User, get_user
-import tsugu_api
+from ...utils import text_response, User, get_user, get_user_async
 from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager
 import re
-
+import tsugu_api
+import tsugu_api_async
 
 # 虚空注册
 alc = Alconna(["上传车牌"],meta=CommandMeta(description="上传车牌",))
 
 
-def handler(message: str, user: User, platform: str, channel_id: str):
+def handler(message: str, user_id: str, platform: str, channel_id: str):
+    if message.startswith("上传车牌"):
+        message = message[4:].strip()
+
+    # 检查car_config['car']中的关键字
+    for keyword in _car_config["car"]:
+        if str(keyword) in message:
+            break
+    else:
+        return None
+
+    # 检查car_config['fake']中的关键字
+    for keyword in _car_config["fake"]:
+        if str(keyword) in message:
+            return None
+
+    pattern = r"^\d{5}(\D|$)|^\d{6}(\D|$)"
+    if not re.match(pattern, message):
+        return None
+
+    user = get_user(user_id, platform)
+
+    # 获取用户数据
+    try:
+        if platform:
+            if not user.car:
+                return None
+    except Exception as e:
+        # 默认不开启关闭车牌，继续提交
+        pass
+
+    try:
+        car_id = message[:6]
+        if not car_id.isdigit() and car_id[:5].isdigit():
+            car_id = car_id[:5]
+        if user.user_id.isdigit():
+            car_user_id = user.user_id
+        else:
+            car_user_id = '3889000770'
+        tsugu_api.submit_room_number(number=int(car_id), user_id=car_user_id, raw_message=message, source="Tsugu", token="ZtV4EX2K9Onb")
+        return None
+
+    except Exception as e:
+        return None
+
+
+async def handler_async(message: str, user_id: str, platform: str, channel_id: str):
     if message.startswith("上传车牌"):
         message = message[4:].strip()
 
     # 检查car_config['car']中的关键字
     for keyword in _car_config["car"]:
         if str(keyword) in message:
             break
@@ -24,15 +70,15 @@
         if str(keyword) in message:
             return None
 
     pattern = r"^\d{5}(\D|$)|^\d{6}(\D|$)"
     if not re.match(pattern, message):
         return None
 
-    user = get_user(user.user_id, platform)
+    user = await get_user_async(user_id, platform)
 
     # 获取用户数据
     try:
         if platform:
             if not user.car:
                 return None
     except Exception as e:
@@ -43,15 +89,15 @@
         car_id = message[:6]
         if not car_id.isdigit() and car_id[:5].isdigit():
             car_id = car_id[:5]
         if user.user_id.isdigit():
             car_user_id = user.user_id
         else:
             car_user_id = '3889000770'
-        tsugu_api.submit_room_number(number=int(car_id), user_id=car_user_id, raw_message=message, source=config.bandori_station_token_name, token=config.bandori_station_token)
+        await tsugu_api_async.submit_room_number(number=int(car_id), user_id=car_user_id, raw_message=message, source="Tsugu", token="ZtV4EX2K9Onb")
         return None
 
     except Exception as e:
         return None
 
 
 _car_config = {
```

### Comparing `tsugu-1.1.0rc5/tsugu/src/bandoristation/ycm.py` & `tsugu-2.0.0/tsugu/src/bandoristation/ycm.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,74 @@
-from ...utils import text_response, User, config
+from ...utils import get_user, text_response, User, server_id_2_server_name, server_name_2_server_id
 import tsugu_api
+import tsugu_api_async
 from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager
 
 
-def handler(message: str, user: User, platform: str, channel_id: str):
-    res = Alconna(
+alc = Alconna(
         ["ycm", "车来", "有车吗"],
         meta=CommandMeta(
-            compact=config.compact, description="获取车牌",
+            compact=True, description="获取车牌",
         )
-    ).parse(message)
+    )
+
+
+def handler(message: str, user_id: str, platform: str, channel_id: str):
+    res = alc.parse(message)
 
     if res.matched:
-        return car_search()
+        try:
+            data = tsugu_api.query_room_number()
+        except Exception as e:
+            return text_response('获取房间信息失败，请稍后再试')
+        if not data:
+            return text_response('myc')
+
+        new_data = []
+        for i in data:
+            if isinstance(i['number'], str):
+                i['number'] = int(i['number'])
+            i['source'] = i['source_info']['name']
+            i['userId'] = i['user_info']['user_id']
+            i['time'] = i['time']
+            i['avanter'] = i['user_info']['avatar']
+            i['userName'] = i['user_info']['username']
+            i['rawMessage'] = i['raw_message']
+            new_data.append(i)
+        # 过滤掉 number 相同的
+        new_data = list({v['number']: v for v in new_data}.values())
+
+        return tsugu_api.room_list(new_data)
+
     return res
 
 
-def car_search():
-    try:
-        data = tsugu_api.query_room_number()
-    except Exception as e:
-        return text_response('获取房间信息失败，请稍后再试')
-    if not data:
-        return text_response('myc')
-
-    new_data = []
-    for i in data:
-        if isinstance(i['number'], str):
-            i['number'] = int(i['number'])
-        i['source'] = i['source_info']['name']
-        i['userId'] = i['user_info']['user_id']
-        i['time'] = i['time']
-        i['avanter'] = i['user_info']['avatar']
-        i['userName'] = i['user_info']['username']
-        i['rawMessage'] = i['raw_message']
-        new_data.append(i)
-    # 过滤掉 number 相同的
-    new_data = list({v['number']: v for v in new_data}.values())
+async def handler_async(message: str, user_id: str, platform: str, channel_id: str):
+    res = alc.parse(message)
+
+    if res.matched:
+        try:
+            data = await tsugu_api_async.query_room_number()
+        except Exception as e:
+            return text_response('获取房间信息失败，请稍后再试')
+        if not data:
+            return text_response('myc')
+
+        new_data = []
+        for i in data:
+            if isinstance(i['number'], str):
+                i['number'] = int(i['number'])
+            i['source'] = i['source_info']['name']
+            i['userId'] = i['user_info']['user_id']
+            i['time'] = i['time']
+            i['avanter'] = i['user_info']['avatar']
+            i['userName'] = i['user_info']['username']
+            i['rawMessage'] = i['raw_message']
+            new_data.append(i)
+        # 过滤掉 number 相同的
+        new_data = list({v['number']: v for v in new_data}.values())
+
+        return await tsugu_api_async.room_list(new_data)
+
+    return res
 
-    return tsugu_api.room_list(new_data)
```

### Comparing `tsugu-1.1.0rc5/tsugu/src/help/help.py` & `tsugu-2.0.0/tsugu/src/universal/search_gacha.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,36 @@
-from ...utils import config, text_response, User, server_id_2_server_name, server_name_2_server_id, server_exists
-from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager, MultiVar, AllParam
+from ...utils import get_user, text_response, User, server_id_2_server_name, server_name_2_server_id
+import tsugu_api
+from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager
+import tsugu_api_async
 
 
-def handler(message: str, user: User, platform: str, channel_id: str):
-    res = Alconna(
-        ["help"],
-        Args["cmd;?#命令", str],
+alc = Alconna(
+        ["查卡池"],
+        Args["gachaId#可以通过查活动、查卡等获取", str],
         meta=CommandMeta(
-            compact=config.compact, description="Chat Tsugu Py 帮助",)
-    ).parse(message)
+            compact=True, description="查卡池",
+            usage='根据卡池ID查询卡池信息',
+        )
+    )
+
+
+def handler(message: str, user_id: str, platform: str, channel_id: str):
+    res = alc.parse(message)
+
+    if res.matched:
+        user = get_user(user_id, platform)
+        return tsugu_api.search_gacha(user.default_server, res.gachaId)
+
+    return res
+
+
+async def handler_async(message: str, user_id: str, platform: str, channel_id: str):
+    res = alc.parse(message)
 
     if res.matched:
-        if not res.cmd:
-            return text_response(command_manager.all_command_help())
+        user = get_user(user_id, platform)
+        return await tsugu_api_async.search_gacha(user.default_server, res.gachaId)
+
+    return res
 
-        try:
-            cmd = command_manager.command_help(res.cmd)
-            return text_response(cmd)
-
-        except KeyError:
-            # return text_response('未找到该命令')
-            return None
-
-        except Exception as e:
-            # return text_response('未知错误')
-            return None
 
-    return None
```

### Comparing `tsugu-1.1.0rc5/tsugu/src/remote/bind_player.py` & `tsugu-2.0.0/tsugu/src/remote/bind_player.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,43 @@
-from ...utils import config, text_response, User, server_id_2_server_name, server_name_2_server_id, server_exists
+from ...utils import get_user, text_response, User, server_id_2_server_name, server_name_2_server_id
 import tsugu_api
 from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager, MultiVar, AllParam
+import tsugu_api_async
 
 
-def handler(message: str, user: User, platform: str, channel_id: str):
-    res = Alconna(
+alc = Alconna(
         ["绑定玩家"],
-    Args["args;?", AllParam],
-    meta=CommandMeta(
-            compact=config.compact, description="绑定玩家",
+        Args["args;?", AllParam],
+        meta=CommandMeta(
+            compact=True, description="绑定玩家",
             usage="只需发送‘绑定玩家’。",
         ),
-    ).parse(message)
+    )
+
+
+def handler(message: str, user_id: str, platform: str, channel_id: str):
+    res = alc.parse(message)
 
     if res.matched:
+        user = get_user(user_id, platform)
         r = tsugu_api.bind_player_request(platform, user.user_id, user.server_mode, False)
         if r.get('status') != 'success':
             return text_response(r.get('data'))
         return text_response(
             f'''正在绑定账号，请将 评论(个性签名) 或者 当前使用的 乐队编队名称改为\n{r.get('data')['verifyCode']}\n稍等片刻等待同步后，发送\n验证绑定 你的玩家ID(数字) 服务器名(字母缩写)\n例如：验证绑定 114****514 cn''')
 
     return res
 
+
+async def handler_async(message: str, user_id: str, platform: str, channel_id: str):
+    res = alc.parse(message)
+
+    if res.matched:
+        user = get_user(user_id, platform)
+        r = await tsugu_api_async.bind_player_request(platform, user.user_id, user.server_mode, False)
+        if r.get('status') != 'success':
+            return text_response(r.get('data'))
+        return text_response(
+            f'''正在绑定账号，请将 评论(个性签名) 或者 当前使用的 乐队编队名称改为\n{r.get('data')['verifyCode']}\n稍等片刻等待同步后，发送\n验证绑定 你的玩家ID(数字) 服务器名(字毝缩写)\n例如：验证绑定 114****514 cn''')
+
+    return res
+
```

### Comparing `tsugu-1.1.0rc5/tsugu/src/remote/bind_player_verification_off.py` & `tsugu-2.0.0/tsugu/src/universal/search_player.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,47 @@
-from ...utils import text_response, User, server_id_2_server_name, server_name_2_server_id, server_exists, config
+from ...utils import get_user, text_response, User, server_id_2_server_name, server_name_2_server_id
+from tsugu_api_core._typing import _ServerName
 import tsugu_api
 from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager
+import tsugu_api_async
 
 
-def handler(message: str, user: User, platform: str, channel_id: str):
-    res = Alconna(
-        ["验证解绑"],
-        Args["index#要解绑的绑定编号", int],
+alc = Alconna(
+        ["查玩家", "查寻玩家"],
+        Args["playerId#你的游戏账号(数字)", int]["serverName;?#省略服务器名时，默认从你当前的主服务器查询。", _ServerName.__args__],
         meta=CommandMeta(
-            compact=config.compact, description="验证解绑",
-            usage="验证解绑 记录编号(数字)",
-            example="验证解绑 1 : 解绑第一个记录"
-        ),
-    ).parse(message)
+            compact=True, description="查询玩家信息",
+            usage='查询指定ID玩家的信息。查询指定ID玩家的信息。',
+            example='查玩家 40474621 jp : 查询日服玩家ID为40474621的玩家信息。\n查玩家 10000000 : 查询你当前默认服务器中，玩家ID为10000000的玩家信息。',
+        )
+    )
+
+
+def handler(message: str, user_id: str, platform: str, channel_id: str):
+    res = alc.parse(message)
+
+    if res.matched:
+        user = get_user(user_id, platform)
+        if res.serverName:
+            server = res.serverName
+        else:
+            server = user.server_mode
+        return tsugu_api.search_player(res.playerId, server)
+
+    return res
+
+
+async def handler_async(message: str, user_id: str, platform: str, channel_id: str):
+    res = alc.parse(message)
 
     if res.matched:
-        if len(user.game_ids) < int(res.index):
-            return text_response('未找到记录')
-        player_id = user.game_ids[int(res.index) - 1].get("game_id")
-        server_mode = user.game_ids[int(res.index) - 1].get("server")
-        r = tsugu_api.bind_player_verification(platform, user.user_id, server_mode, player_id, False)
-        if r.get('status') != 'success':
-            return text_response(r.get('data'))
-        return text_response('解绑成功！')
-    
+        user = get_user(user_id, platform)
+        if res.serverName:
+            server = res.serverName
+        else:
+            server = user.server_mode
+        return await tsugu_api_async.search_player(res.playerId, server)
+
     return res
 
 
+
```

### Comparing `tsugu-1.1.0rc5/tsugu/src/remote/change_default_server.py` & `tsugu-2.0.0/tsugu/src/remote/change_server_mode.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,42 @@
-from ...utils import text_response, User, server_id_2_server_name, server_names_2_server_ids, server_exists, config
+from ...utils import get_user, text_response, User, server_id_2_server_name, server_name_2_server_id
 import tsugu_api
 from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager, MultiVar
 from tsugu_api_core._typing import _ServerName
 
 
-def handler(message: str, user: User, platform: str, channel_id: str):
-    res = Alconna(
-        ["设置默认服务器", "默认服务器"],
-        Args["serverList#使用空格分隔服务器列表。", MultiVar(_ServerName)],
+alc = Alconna(
+        ["主服务器", "设置主服务器"],
+    Args["serverName#服务器名", _ServerName],
         meta=CommandMeta(
-            compact=config.compact, description="设定信息显示中的默认服务器排序",
-            example="""设置默认服务器 cn jp : 将国服设置为第一服务器，日服设置为第二服务器。"""
+            compact=True, description="主服务器",
+            usage="将指定的服务器设置为你的主服务器。",
+            example="""主服务器 cn : 将国服设置为主服务器。"""
 
         )
-    ).parse(message)
+    )
+
+
+def handler(message: str, user_id: str, platform: str, channel_id: str):
+    res = alc.parse(message)
 
     if res.matched:
-        r = tsugu_api.change_user_data(platform, user.user_id, {'default_server': server_names_2_server_ids(res.serverList)})
+        user = get_user(user_id, platform)
+        r = tsugu_api.change_user_data(platform, user.user_id, {'server_mode': server_name_2_server_id(res.serverName)})
         if r.get('status') != 'success':
             return text_response(r.get('data'))
-        return text_response('默认服务器已设置为 ' + ' '.join(res.serverList))
-    
+        return text_response('主服务器已设置为 ' + res.serverName)
     return res
+
+
+async def handler_async(message: str, user_id: str, platform: str, channel_id: str):
+    res = alc.parse(message)
+
+    if res.matched:
+        user = get_user(user_id, platform)
+        r = await tsugu_api.change_user_data(platform, user.user_id, {'server_mode': server_name_2_server_id(res.serverName)})
+        if r.get('status') != 'success':
+            return text_response(r.get('data'))
+        return text_response('主服务器已设置为 ' + res.serverName)
+    return res
+
+
```

### Comparing `tsugu-1.1.0rc5/tsugu/src/remote/change_server_mode.py` & `tsugu-2.0.0/tsugu/src/remote/switch_car_forwarding_off.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,40 @@
-from ...utils import text_response, User, server_id_2_server_name, server_name_2_server_id, server_exists, config
+from ...utils import get_user, text_response, User, server_id_2_server_name, server_name_2_server_id
 import tsugu_api
-from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager, MultiVar
-from tsugu_api_core._typing import _ServerName
+from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager
+import tsugu_api_async
 
 
-def handler(message: str, user: User, platform: str, channel_id: str):
-    res = Alconna(
-        ["主服务器", "设置主服务器"],
-    Args["serverName#服务器名", _ServerName],
+alc = Alconna(
+        ["关闭车牌转发", "关闭个人车牌转发"],
         meta=CommandMeta(
-            compact=config.compact, description="主服务器",
-            usage="将指定的服务器设置为你的主服务器。",
-            example="""主服务器 cn : 将国服设置为主服务器。"""
+            compact=True, description="关闭车牌转发",)
+    )
 
-        )
-    ).parse(message)
+
+def handler(message: str, user_id: str, platform: str, channel_id: str):
+    res = alc.parse(message)
+
+    if res.matched:
+        user = get_user(user_id, platform)
+        update = {'car': False, }
+        r = tsugu_api.change_user_data(platform, user.user_id, update)
+        if r.get('status') != 'success':
+            return text_response(r.get('data'))
+        return text_response('关闭车牌转发成功！')
+    return res
+
+
+async def handler_async(message: str, user_id: str, platform: str, channel_id: str):
+    res = alc.parse(message)
 
     if res.matched:
-        r = tsugu_api.change_user_data(platform, user.user_id, {'server_mode': server_name_2_server_id(res.serverName)})
+        user = get_user(user_id, platform)
+        update = {'car': False, }
+        r = await tsugu_api_async.change_user_data(platform, user.user_id, update)
         if r.get('status') != 'success':
             return text_response(r.get('data'))
-        return text_response('主服务器已设置为 ' + res.serverName)
+        return text_response('关闭车牌转发成功！')
     return res
 
+
+
```

### Comparing `tsugu-1.1.0rc5/tsugu/src/remote/player_status.py` & `tsugu-2.0.0/tsugu/src/remote/bind_player_verification_off.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,71 +1,50 @@
-from ...utils import text_response, User, server_id_2_server_name, server_name_2_server_id, server_exists, config
+from ...utils import get_user, text_response, User, server_id_2_server_name, server_name_2_server_id
 import tsugu_api
 from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager
-from tsugu_api_core._typing import _ServerName
+import tsugu_api_async
 
 
-def handler(message: str, user: User, platform: str, channel_id: str):
-    res = Alconna(
-        ["玩家状态"],
-        Args["serverName", _ServerName.__args__, None]["serverIndex", int, None],
+alc = Alconna(
+        ["验证解绑"],
+        Args["index#要解绑的绑定编号", int],
         meta=CommandMeta(
-            compact=config.compact, description="查询自己的玩家状态",
-            usage='根据关键词或活动ID查询活动信息',
-            example='''玩家状态 :返回玩家状态(优先当前服务器下第一条记录)
-玩家状态 1 :返回绑定的第一条记录的状态
-玩家状态 jp :返回绑定的cn服务器的记录的状态'''
-        )
-    ).parse(message)
+            compact=True, description="验证解绑",
+            usage="验证解绑 记录编号(数字)",
+            example="验证解绑 1 : 解绑第一个记录"
+        ),
+    )
+
+
+def handler(message: str, user_id: str, platform: str, channel_id: str):
+    res = alc.parse(message)
 
     if res.matched:
-        if res.serverName:
-            return _case_server(user, res.serverName)
-        elif res.serverIndex:
-            return _case_index(user, res.serverIndex)
-        else:
-            return _case_default(user)
+        user = get_user(user_id, platform)
+        if len(user.game_ids) < int(res.index):
+            return text_response('未找到记录')
+        player_id = user.game_ids[int(res.index) - 1].get("game_id")
+        server_mode = user.game_ids[int(res.index) - 1].get("server")
+        r = tsugu_api.bind_player_verification(platform, user.user_id, server_mode, player_id, False)
+        if r.get('status') != 'success':
+            return text_response(r.get('data'))
+        return text_response('解绑成功！')
+    
     return res
 
 
+async def handler_async(message: str, user_id: str, platform: str, channel_id: str):
+    res = alc.parse(message)
 
-def _utils_search_player_by_game_id(game_id, additional_text=""):
-    player_id = str(game_id.get("game_id"))
-    server = int(game_id.get("server"))
-    response = tsugu_api.search_player(int(player_id), server)
-    return response + text_response(additional_text)
-
-
-def _case_default(user: User):
-    # 优先当前服务器
-    for game_id in user.game_ids:
-        if game_id.get("server") == user.server_mode:
-            text = f'已查找默认服务器 {server_id_2_server_name(user.server_mode)} 的记录。'
-            return _utils_search_player_by_game_id(game_id, text)
-    # 兜底逻辑：使用第一个记录
-    if user.game_ids:
-        game_id = user.game_ids[0]
-        text = f'已查找第一个记录。'
-        return _utils_search_player_by_game_id(game_id, text)
-    return text_response('未绑定任何记录，可以使用 绑定玩家 进行绑定')
-
-
-def _case_server(user: User, server_name: str):
-    server_id = server_name_2_server_id(server_name)
-    # 服务器不存在
-    if not server_exists(server_id):
-        return text_response(f'服务器 {server_name} 不存在。')
-    # 查找记录
-    for game_id in user.game_ids:
-        if game_id.get("server") == server_id:
-            # 找到记录
-            return _utils_search_player_by_game_id(game_id)
-    # 未找到记录
-    return text_response(f'未在记录中找到服务器 {server_name} 的记录。')
-
-
-def _case_index(user: User, index: int):
-    if index > len(user.game_ids) or index < 1:
-        return text_response(f'未找到记录 {index}。')
-    return _utils_search_player_by_game_id(user.game_ids[index - 1])
+    if res.matched:
+        user = get_user(user_id, platform)
+        if len(user.game_ids) < int(res.index):
+            return text_response('未找到记录')
+        player_id = user.game_ids[int(res.index) - 1].get("game_id")
+        server_mode = user.game_ids[int(res.index) - 1].get("server")
+        r = await tsugu_api_async.bind_player_verification(platform, user.user_id, server_mode, player_id, False)
+        if r.get('status') != 'success':
+            return text_response(r.get('data'))
+        return text_response('解绑成功！')
 
+    return res
```

### Comparing `tsugu-1.1.0rc5/tsugu/src/remote/switch_car_forwarding_off.py` & `tsugu-2.0.0/tsugu/src/remote/switch_car_forwarding_on.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,39 @@
-from ...utils import text_response, User, server_id_2_server_name, server_name_2_server_id, server_exists, config
+from ...utils import get_user, text_response, User, server_id_2_server_name, server_name_2_server_id
 import tsugu_api
 from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager
+import tsugu_api_async
 
 
-def handler(message: str, user: User, platform: str, channel_id: str):
-    res =  Alconna(
-        ["关闭车牌转发", "关闭个人车牌转发"],
+alc = Alconna(
+        ["开启车牌转发", "开启个人车牌转发"],
         meta=CommandMeta(
-            compact=config.compact, description="关闭车牌转发",)
-    ).parse(message)
+            compact=True, description="开启车牌转发",)
+    )
+
+
+def handler(message: str, user_id: str, platform: str, channel_id: str):
+    res = alc.parse(message)
 
     if res.matched:
-        update = {'car': False, }
+        user = get_user(user_id, platform)
+        update = {'car': True, }
         r = tsugu_api.change_user_data(platform, user.user_id, update)
         if r.get('status') != 'success':
             return text_response(r.get('data'))
-        return text_response('关闭车牌转发成功！')
+        return text_response('开启车牌转发成功！')
+    return res
+
+
+async def handler_async(message: str, user_id: str, platform: str, channel_id: str):
+    res = alc.parse(message)
+
+    if res.matched:
+        user = get_user(user_id, platform)
+        update = {'car': True, }
+        r = await tsugu_api_async.change_user_data(platform, user.user_id, update)
+        if r.get('status') != 'success':
+            return text_response(r.get('data'))
+        return text_response('开启车牌转发成功！')
     return res
 
+
```

### Comparing `tsugu-1.1.0rc5/tsugu/src/remote/unbind_player.py` & `tsugu-2.0.0/tsugu/src/remote/change_default_server.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,43 +1,44 @@
-from ...utils import text_response, User, server_id_2_server_name, server_name_2_server_id, server_exists, config
+from ...utils import get_user, text_response, User, server_id_2_server_name, server_names_2_server_ids
 import tsugu_api
-from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager
+from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager, MultiVar
+from tsugu_api_core._typing import _ServerName
+import tsugu_api_async
 
 
-def handler(message: str, user: User, platform: str, channel_id: str):
-    res = Alconna(
-        ["解除绑定"],
-        Args["index#要解绑的绑定编号", int, None],
+alc = Alconna(
+        ["设置默认服务器", "默认服务器"],
+        Args["serverList#使用空格分隔服务器列表。", MultiVar(_ServerName)],
         meta=CommandMeta(
-            compact=config.compact, description="解除绑定",
-            usage="验证解绑 记录编号(数字)",
-            example="验证解绑 1 : 解绑第一个记录"
-        ),
-    ).parse(message)
+            compact=True, description="设定信息显示中的默认服务器排序",
+            example="""设置默认服务器 cn jp : 将国服设置为第一服务器，日服设置为第二服务器。"""
 
-    if res.matched:
-        if not res.index:
-            bind_record = '\n'.join([f'{i + 1}. {mask_data(x.get("game_id"))} {server_id_2_server_name(x.get("server"))}' for i, x in enumerate(user.game_ids)])
-            return text_response('请输入正确的记录(数字)\n例如: 解除绑定 1\n当前的绑定记录如下:\n' + bind_record)
+        )
+    )
 
-        if len(user.game_ids) < int(res.index):
-            return text_response('未找到记录')
 
-        server_mode = user.game_ids[int(res.index) - 1].get("server")
+def handler(message: str, user_id: str, platform: str, channel_id: str):
+    res = alc.parse(message)
 
-        r = tsugu_api.bind_player_request(platform, user.user_id, server_mode, False)
+    if res.matched:
+        user = get_user(user_id, platform)
+        r = tsugu_api.change_user_data(platform, user.user_id, {'default_server': server_names_2_server_ids(res.serverList)})
         if r.get('status') != 'success':
             return text_response(r.get('data'))
-        return text_response(f'''正在解除，请将 评论(个性签名) 或者 当前使用的 乐队编队名称改为\n{r.get('data')['verifyCode']}\n稍等片刻等待同步后，发送\n验证解绑 {res.index}\n来完成本次身份验证''')
+        return text_response('默认服务器已设置为 ' + ' '.join(res.serverList))
+    
     return res
 
 
-def mask_data(game_id: str):
-    game_id = str(game_id)
-    if len(game_id) < 6:
-        return game_id[:3] + '*' * (len(game_id) - 3)
-    elif len(game_id) < 3:
-        return '*' * len(game_id)
-    else:
-        game_id = game_id[:3] + '*' * (len(game_id) - 6) + game_id[-3:]
-    return game_id
+async def handler_async(message: str, user_id: str, platform: str, channel_id: str):
+    res = alc.parse(message)
+
+    if res.matched:
+        user = get_user(user_id, platform)
+        r = await tsugu_api_async.change_user_data(platform, user.user_id, {'default_server': server_names_2_server_ids(res.serverList)})
+        if r.get('status') != 'success':
+            return text_response(r.get('data'))
+        return text_response('默认服务器已设置为 ' + ' '.join(res.serverList))
+
+    return res
+
```

### Comparing `tsugu-1.1.0rc5/tsugu/src/universal/event_stage.py` & `tsugu-2.0.0/tsugu/src/universal/event_stage.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,47 @@
-from ...utils import text_response, User, server_id_2_server_name, server_name_2_server_id, server_exists, config
+from ...utils import get_user, text_response, User, server_id_2_server_name, server_name_2_server_id
 import tsugu_api
 from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager
+import tsugu_api_async
 
 
-def handler(message: str, user: User, platform: str, channel_id: str):
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
-
         return tsugu_api.event_stage(user.server_mode, res.eventId, meta)
 
     return res
+
+
+async def handler_async(message: str, user_id: str, platform: str, channel_id: str):
+    res = alc.parse(message)
+
+    if res.matched:
+        user = get_user(user_id, platform)
+        if res.meta:
+            meta = True
+        else:
+            meta = False
+        return await tsugu_api_async.event_stage(user.server_mode, res.eventId, meta)
+
+    return res
+
```

### Comparing `tsugu-1.1.0rc5/tsugu/src/universal/gacha_simulate.py` & `tsugu-2.0.0/tsugu/src/universal/gacha_simulate.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,45 @@
-from ...utils import text_response, User, server_id_2_server_name, server_name_2_server_id, server_exists, config
+from ...utils import get_user, text_response, User, server_id_2_server_name, server_name_2_server_id
 import tsugu_api
 from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager
+import tsugu_api_async
 
 
-def handler(message: str, user: User, platform: str, channel_id: str):
-    res = Alconna(
+alc = Alconna(
         ["抽卡模拟", "卡池模拟"],
         Args["times", int, 10]['gacha_id;?#如果没有卡池ID的话，卡池为当前活动的卡池。', int],
         meta=CommandMeta(
-            compact=config.compact, description="抽卡模拟",
+            compact=True, description="抽卡模拟",
             usage='根据卡片ID查询卡片插画',
             example='抽卡模拟 300 922 :模拟抽卡300次，卡池为922号卡池。'
         )
-    ).parse(message)
+    )
+
+
+def handler(message: str, user_id: str, platform: str, channel_id: str):
+    res = alc.parse(message)
 
     if res.matched:
-        if channel_id in config.disable_gacha_simulate_group_ids:
-            return None
+        user = get_user(user_id, platform)
         if res.gacha_id:
             gacha_id = res.gacha_id
         else:
             gacha_id = None
         return tsugu_api.gacha_simulate(user.server_mode, res.times, gacha_id)
 
     return res
+
+
+async def handler_async(message: str, user_id: str, platform: str, channel_id: str):
+    res = alc.parse(message)
+
+    if res.matched:
+        user = get_user(user_id, platform)
+        if res.gacha_id:
+            gacha_id = res.gacha_id
+        else:
+            gacha_id = None
+        return await tsugu_api_async.gacha_simulate(user.server_mode, res.times, gacha_id)
+
+    return res
+
+
```

### Comparing `tsugu-1.1.0rc5/tsugu/src/universal/lsycx.py` & `tsugu-2.0.0/tsugu/src/universal/ycx.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,42 @@
-from ...utils import text_response, User, server_id_2_server_name, server_name_2_server_id, server_exists, config
+from ...utils import get_user, text_response, User, server_id_2_server_name, server_name_2_server_id
 import tsugu_api
 from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager
 from tsugu_api_core._typing import _ServerName
+import tsugu_api_async
 
 
-def handler(message: str, user: User, platform: str, channel_id: str):
-    res = Alconna(
-        ["lsycx", "历史预测线"], ['/', ''],
+alc = Alconna(
+        ["ycx", "预测线"],
         Args['tier', int]['eventId;?#活动ID，省略时查询当前活动。', int]
             ['serverName#省略服务器名时，默认从你当前的主服务器查询。活动ID不存在时，也可以作为第二个参数。', _ServerName.__args__, None],
         meta=CommandMeta(
-            compact=config.compact, description="查询指定档位的历史预测线。",
-            usage='查询指定档位的预测线与最近的4期活动类型相同的活动的档线数据。',
-            example='''lsycx 1000 :返回默认服务器当前活动的档线与预测线，与最近的4期活动类型相同的活动的档线数据。
-lsycx 1000 177 jp:返回日服177号活动1000档位档线与最近的4期活动类型相同的活动的档线数据。'''
+            compact=True, description="查询指定档位的预测线",
+            usage='查询指定档位的预测线。',
+            example='''ycx 1000 :返回默认服务器当前活动1000档位的档线与预测线。
+ycx 1000 177 jp:返回日服177号活动1000档位的档线与预测线。'''
         )
-    ).parse(message)
+    )
+
+
+def handler(message: str, user_id: str, platform: str, channel_id: str):
+    res = alc.parse(message)
 
     if res.matched:
+        user = get_user(user_id, platform)
         server = server_name_2_server_id(res.serverName) if res.serverName else user.server_mode
-        return tsugu_api.lsycx(server, res.tier, res.eventId)
+        return tsugu_api.ycx(server, res.tier, res.eventId)
 
     return res
+
+
+async def handler_async(message: str, user_id: str, platform: str, channel_id: str):
+    res = alc.parse(message)
+
+    if res.matched:
+        user = get_user(user_id, platform)
+        server = server_name_2_server_id(res.serverName) if res.serverName else user.server_mode
+        return await tsugu_api_async.ycx(server, res.tier, res.eventId)
+
+    return res
+
+
```

### Comparing `tsugu-1.1.0rc5/tsugu/src/universal/search_card.py` & `tsugu-2.0.0/tsugu/src/universal/search_card.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,37 @@
-from ...utils import text_response, User, server_id_2_server_name, server_name_2_server_id, server_exists, config
+from ...utils import get_user, text_response, User, server_id_2_server_name, server_name_2_server_id
 import tsugu_api
-from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager, MultiVar
+from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager, AllParam
+import tsugu_api_async
 
 
-def handler(message: str, user: User, platform: str, channel_id: str):
-    res = Alconna(
+alc = Alconna(
         ["查卡", "查卡牌"],
-        Args["word#请输入卡面ID，角色等查询参数，使用空格隔开", MultiVar(str)],
+        Args["word#请输入卡面ID，角色等查询参数，使用空格隔开", AllParam],
         meta=CommandMeta(
-            compact=config.compact, description="查询卡片信息。",
+            compact=True, description="查询卡片信息。",
             usage='根据关键词或卡牌ID查询卡片信息。',
             example='''查卡 1399 :返回1399号卡牌的信息。
     查卡面 1399 :返回1399号卡牌的插画。
     查卡 红 ars 5x :返回角色 ars 的 5x 卡片的信息。'''
         )
-    ).parse(message)
+    )
+
+def handler(message: str, user_id: str, platform: str, channel_id: str):
+    res = alc.parse(message)
 
     if res.matched:
+        user = get_user(user_id, platform)
         return tsugu_api.search_card(user.default_server, " ".join(res.word))
 
     return res
 
+
+async def handler_async(message: str, user_id: str, platform: str, channel_id: str):
+    res = alc.parse(message)
+
+    if res.matched:
+        user = get_user(user_id, platform)
+        return await tsugu_api_async.search_card(user.default_server, " ".join(res.word))
+
+    return res
+
```

### Comparing `tsugu-1.1.0rc5/tsugu/src/universal/search_event.py` & `tsugu-2.0.0/tsugu/src/universal/search_event.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,39 @@
-from ...utils import text_response, User, server_id_2_server_name, server_name_2_server_id, server_exists, config
+from ...utils import get_user, text_response, User, server_id_2_server_name, server_name_2_server_id
 import tsugu_api
-from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, MultiVar
+from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, AllParam
+import tsugu_api_async
 
 
-def handler(message: str, user: User, platform: str, channel_id: str):
-    res = Alconna(
+alc = Alconna(
         ["查活动"],
-        Args["word#请输入活动名，乐队，活动ID等查询参数", MultiVar(str)],
+        Args["word#请输入活动名，乐队，活动ID等查询参数", AllParam],
         meta=CommandMeta(
-            compact=config.compact, description="查活动",
+            compact=True, description="查活动",
             usage='根据关键词或活动ID查询活动信息',
             example='''查活动 绿 tsugu :返回所有属性加成为pure，且活动加成角色中包括羽泽鸫的活动列表
 查活动 177 :返回177号活动的信息
 查活动 >225 :查询大于225的活动
 查活动 220-225 :查询220到225的活动'''
         )
-    ).parse(message)
+    )
+
+def handler(message: str, user_id: str, platform: str, channel_id: str):
+    res = alc.parse(message)
 
     if res.matched:
+        user = get_user(user_id, platform)
         return tsugu_api.search_event(user.default_server, " ".join(res.word))
 
     return res
 
+
+async def handler_async(message: str, user_id: str, platform: str, channel_id: str):
+    res = alc.parse(message)
+
+    if res.matched:
+        user = get_user(user_id, platform)
+        return await tsugu_api_async.search_event(user.default_server, " ".join(res.word))
+
+    return res
+
+
```

### Comparing `tsugu-1.1.0rc5/tsugu/src/universal/search_gacha.py` & `tsugu-2.0.0/tsugu/src/universal/get_card_illustration.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,37 @@
-from ...utils import text_response, User, server_id_2_server_name, server_name_2_server_id, server_exists, config
+from ...utils import get_user, text_response, User, server_id_2_server_name, server_name_2_server_id
 import tsugu_api
 from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager
+import tsugu_api_async
 
 
-def handler(message: str, user: User, platform: str, channel_id: str):
-    res = Alconna(
-        ["查卡池"],
-        Args["gachaId#可以通过查活动、查卡等获取", str],
+alc = Alconna(
+        ["查卡面", "查插画"],
+        Args["cardId", int],
         meta=CommandMeta(
-            compact=config.compact, description="查卡池",
-            usage='根据卡池ID查询卡池信息',
+            compact=True, description="查卡面",
+            usage='根据卡片ID查询卡片插画',
+            example='查卡面 1399 :返回1399号卡牌的插画'
         )
-    ).parse(message)
+    )
+
+
+def handler(message: str, user_id: str, platform: str, channel_id: str):
+    res = alc.parse(message)
+
+    if res.matched:
+        user = get_user(user_id, platform)
+        return tsugu_api.get_card_illustration(res.cardId)
+
+    return res
+
+
+async def handler_async(message: str, user_id: str, platform: str, channel_id: str):
+    res = alc.parse(message)
 
     if res.matched:
-        return tsugu_api.search_gacha(user.default_server, res.gachaId)
+        user = get_user(user_id, platform)
+        return await tsugu_api_async.get_card_illustration(res.cardId)
 
     return res
+
+
```

### Comparing `tsugu-1.1.0rc5/tsugu/src/universal/song_meta.py` & `tsugu-2.0.0/tsugu/src/universal/song_chart.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,41 @@
-from ...utils import text_response, User, server_id_2_server_name, server_name_2_server_id, server_exists, config
+from ...utils import get_user, text_response, User, server_id_2_server_name, server_name_2_server_id
 import tsugu_api
 from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager
-from tsugu_api_core._typing import _ServerName
+import tsugu_api_async
 
 
-def handler(message: str, user: User, platform: str, channel_id: str):
-    res = Alconna(
-        ["查询分数表", '查分数表', '查询分数榜', '查分数榜'],
-        Args["serverName;?#省略服务器名时，默认从你当前的主服务器查询。", _ServerName.__args__],
+difficulty_text_tuple = ('easy', 'ez', 'normal', 'nm', 'hard', 'hd', 'expert', 'ex', 'special', 'sp')
+
+alc = Alconna(
+        ["查谱面", "查铺面"],
+        Args["songId", int]['difficultyText', difficulty_text_tuple, 'ex'],
         meta=CommandMeta(
-            compact=config.compact, description="查询分数表",
-            usage='查询指定服务器的歌曲分数表。',
-            example='''查询分数表 cn :返回国服的歌曲分数表'''
+            compact=True, description="查谱面",
+            usage='根据曲目ID与难度查询铺面信息。',
+            example='''查谱面 1 :返回1号曲的ex难度谱面
+查谱面 128 special :返回128号曲的special难度谱面'''
         )
-    ).parse(message)
+    )
+def handler(message: str, user_id: str, platform: str, channel_id: str):
+    res = alc.parse(message)
 
     if res.matched:
-        if res.serverName:
-            server = server_name_2_server_id(res.serverName)
-        else:
-            server = user.server_mode
-        return tsugu_api.song_meta(user.default_server, server)
+        user = get_user(user_id, platform)
+        return tsugu_api.song_chart(user.default_server, res.songId, res.difficultyText)
 
     return res
 
+
+async def handler_async(message: str, user_id: str, platform: str, channel_id: str):
+    res = alc.parse(message)
+
+    if res.matched:
+        user = get_user(user_id, platform)
+        return await tsugu_api_async.song_chart(user.default_server, res.songId, res.difficultyText)
+
+    return res
+
+
+
+
+
```

### Comparing `tsugu-1.1.0rc5/tsugu/src/universal/ycx.py` & `tsugu-2.0.0/tsugu/src/universal/ycx_all.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,41 @@
-from ...utils import text_response, User, server_id_2_server_name, server_name_2_server_id, server_exists, config
+from ...utils import get_user, text_response, User, server_id_2_server_name, server_name_2_server_id, server_exists
 import tsugu_api
 from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager
 from tsugu_api_core._typing import _ServerName
+import tsugu_api_async
 
 
-def handler(message: str, user: User, platform: str, channel_id: str):
-    res = Alconna(
-        ["ycx", "预测线"],
-        Args['tier', int]['eventId;?#活动ID，省略时查询当前活动。', int]
+alc = Alconna(
+        ["ycxall", "ycx all"],
+        Args['eventId;?#活动ID，省略时查询当前活动。', int]
             ['serverName#省略服务器名时，默认从你当前的主服务器查询。活动ID不存在时，也可以作为第二个参数。', _ServerName.__args__, None],
         meta=CommandMeta(
-            compact=config.compact, description="查询指定档位的预测线",
-            usage='查询指定档位的预测线。',
+            compact=True, description="查询指定档位的预测线",
+            usage='根据关键词或角色ID查询角色信息',
             example='''ycx 1000 :返回默认服务器当前活动1000档位的档线与预测线。
 ycx 1000 177 jp:返回日服177号活动1000档位的档线与预测线。'''
         )
-    ).parse(message)
+    )
+
+
+def handler(message: str, user_id: str, platform: str, channel_id: str):
+    res = alc.parse(message)
+
+    if res.matched:
+        user = get_user(user_id, platform)
+        server = server_name_2_server_id(res.serverName) if res.serverName else user.server_mode
+        return tsugu_api.ycx_all(server, res.eventId)
+
+    return res
+
+
+async def handler_async(message: str, user_id: str, platform: str, channel_id: str):
+    res = alc.parse(message)
 
     if res.matched:
+        user = get_user(user_id, platform)
         server = server_name_2_server_id(res.serverName) if res.serverName else user.server_mode
-        return tsugu_api.ycx(server, res.tier, res.eventId)
+        return await tsugu_api_async.ycx_all(server, res.eventId)
 
     return res
```

### Comparing `tsugu-1.1.0rc5/tsugu/src/universal/ycx_all.py` & `tsugu-2.0.0/tsugu/src/universal/lsycx.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,42 @@
-from ...utils import text_response, User, server_id_2_server_name, server_name_2_server_id, server_exists, config
+from ...utils import get_user, text_response, User, server_id_2_server_name, server_name_2_server_id
 import tsugu_api
 from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager
 from tsugu_api_core._typing import _ServerName
+import tsugu_api_async
 
 
-def handler(message: str, user: User, platform: str, channel_id: str):
-    res = Alconna(
-        ["ycxall", "ycx all"],
-        Args['eventId;?#活动ID，省略时查询当前活动。', int]
+alc = Alconna(
+        ["lsycx", "历史预测线"], ['/', ''],
+        Args['tier', int]['eventId;?#活动ID，省略时查询当前活动。', int]
             ['serverName#省略服务器名时，默认从你当前的主服务器查询。活动ID不存在时，也可以作为第二个参数。', _ServerName.__args__, None],
         meta=CommandMeta(
-            compact=config.compact, description="查询指定档位的预测线",
-            usage='根据关键词或角色ID查询角色信息',
-            example='''ycx 1000 :返回默认服务器当前活动1000档位的档线与预测线。
-ycx 1000 177 jp:返回日服177号活动1000档位的档线与预测线。'''
+            compact=True, description="查询指定档位的历史预测线。",
+            usage='查询指定档位的预测线与最近的4期活动类型相同的活动的档线数据。',
+            example='''lsycx 1000 :返回默认服务器当前活动的档线与预测线，与最近的4期活动类型相同的活动的档线数据。
+lsycx 1000 177 jp:返回日服177号活动1000档位档线与最近的4期活动类型相同的活动的档线数据。'''
         )
-    ).parse(message)
+    )
+
+
+def handler(message: str, user_id: str, platform: str, channel_id: str):
+    res = alc.parse(message)
 
     if res.matched:
+        user = get_user(user_id, platform)
         server = server_name_2_server_id(res.serverName) if res.serverName else user.server_mode
-        return tsugu_api.ycx_all(server, res.eventId)
+        return tsugu_api.lsycx(server, res.tier, res.eventId)
 
     return res
+
+
+async def handler_async(message: str, user_id: str, platform: str, channel_id: str):
+    res = alc.parse(message)
+
+    if res.matched:
+        user = get_user(user_id, platform)
+        server = server_name_2_server_id(res.serverName) if res.serverName else user.server_mode
+        return await tsugu_api_async.lsycx(server, res.tier, res.eventId)
+
+    return res
+
+
```

### Comparing `tsugu-1.1.0rc5/tsugu/utils/__init__.py` & `tsugu-2.0.0/tsugu/utils/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import typing
 from typing import List
 import tsugu_api
+import tsugu_api_async
 from loguru import logger
 import time
-from ..config import config
 
 from tsugu_api_core._typing import _ServerId
 
 
 _i_s = {0: "jp", 1: "en", 2: "tw", 3: "cn", 4: "kr"}
 _s_i = {"jp": 0, "en": 1, "tw": 2, "cn": 3, "kr": 4}
 
@@ -58,24 +58,76 @@
     多次尝试获取用户数据
     兼容旧版用户数据
 
     :param user_id:
     :param platform:
     :return:
     '''
-    for i in range(0, config.remote_data_max_retry):
+    for i in range(0, 3):
         try:
             user_data_res = tsugu_api.get_user_data(platform, user_id)
             if user_data_res.get('status') == 'failed':
                 return text_response(user_data_res.get('data'))
             break
         except Exception as e:
             logger.error(f'Error: {e}')
             time.sleep(0.8)
             continue
+    else:
+        raise Exception('获取用户数据失败')
+
+    # 获取用户数据失败
+    if user_data_res.get('status') == 'failed':
+        return text_response(user_data_res.get('data'))
+    # 构建用户对象
+    user_data = user_data_res.get('data')
+
+    if user_data.get('game_ids') is None:
+
+        user_data['game_ids'] = []
+        for i in range(0, 5):
+            if user_data.get('server_list')[i]['playerId'] != 0:
+                new_game_id = {"game_id": user_data.get('server_list')[i]['playerId'], "server": i}
+                user_data['game_ids'].append(new_game_id)
+        verify_code_all = []
+        for i in range(0, 5):
+            if user_data.get('server_list')[i].get('verifyCode') is not None:
+                verify_code_all.append(i)
+
+    user = User(user_id=user_id,
+                platform=platform,
+                server_mode=user_data.get('server_mode'),
+                default_server=user_data.get('default_server'),
+                car=user_data.get('car'),
+                server_list=user_data.get('server_list', None),
+                game_ids=user_data.get('game_ids', []),
+                verify_code=user_data.get('verify_code'))
+    return user
+
+
+async def get_user_async(user_id: str, platform: str) -> User:
+    '''
+    获取用户数据
+    多次尝试获取用户数据
+    兼容旧版用户数据
+W
+    :param user_id:
+    :param platform:
+    :return:
+    '''
+    for i in range(0, 3):
+        try:
+            user_data_res = await tsugu_api_async.get_user_data(platform, user_id)
+            if user_data_res.get('status') == 'failed':
+                return text_response(user_data_res.get('data'))
+            break
+        except Exception as e:
+            logger.error(f'Error: {e}')
+            time.sleep(0.8)
+            continue
     else:
         raise Exception('获取用户数据失败')
 
     # 获取用户数据失败
     if user_data_res.get('status') == 'failed':
         return text_response(user_data_res.get('data'))
     # 构建用户对象
```

### Comparing `tsugu-1.1.0rc5/tsugu_async/src/help/help.py` & `tsugu-2.0.0/tsugu/src/help/help.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,43 @@
-from ...utils import config, text_response, User, server_id_2_server_name, server_name_2_server_id, server_exists
+from ...utils import get_user, text_response, User, server_id_2_server_name, server_name_2_server_id
 from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager, MultiVar, AllParam
 
 
-async def handler(message: str, user: User, platform: str, channel_id: str):
-    res = Alconna(
+alc = Alconna(
         ["help"],
         Args["cmd;?#命令", str],
         meta=CommandMeta(
-            compact=config.compact, description="Chat Tsugu Py 帮助",)
-    ).parse(message)
+            compact=True, description="Chat Tsugu Py 帮助",)
+    )
+
+
+def handler(message: str, user_id: str, platform: str, channel_id: str):
+    res = alc.parse(message)
+
+    if res.matched:
+        if not res.cmd:
+            return text_response(command_manager.all_command_help())
+
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
+
+    return None
+
+
+async def handler_async(message: str, user_id: str, platform: str, channel_id: str):
+    res = alc.parse(message)
 
     if res.matched:
         if not res.cmd:
             return text_response(command_manager.all_command_help())
 
         try:
             cmd = command_manager.command_help(res.cmd)
```

### Comparing `tsugu-1.1.0rc5/tsugu_async/src/remote/bind_player_verification_on.py` & `tsugu-2.0.0/tsugu/src/remote/bind_player_verification_on.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,42 @@
-from ...utils import text_response, User, server_id_2_server_name, server_name_2_server_id, server_exists, config
-import tsugu_api_async
+from ...utils import get_user, text_response, User, server_id_2_server_name, server_name_2_server_id
+import tsugu_api
 from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager
 from tsugu_api_core._typing import _ServerName
+import tsugu_api_async
 
 
-async def handler(message: str, user: User, platform: str, channel_id: str):
-    res = Alconna(
+alc = Alconna(
         ["验证绑定"],
         Args["playerID#你的玩家ID(数字)", int]["serverName#服务器名(字母缩写)", _ServerName],
         meta=CommandMeta(
-            compact=config.compact, description="验证绑定",)
-    ).parse(message)
+            compact=True, description="验证绑定",)
+    )
+
+
+def handler(message: str, user_id: str, platform: str, channel_id: str):
+    res = alc.parse(message)
+
+    if res.matched:
+        user = get_user(user_id, platform)
+        server = server_name_2_server_id(res.serverName)
+        r = tsugu_api.bind_player_verification(platform, user.user_id, server, res.playerID, True)
+        if r.get('status') != 'success':
+            return text_response(r.get('data'))
+        return text_response('绑定成功！现在可以使用 玩家状态 {len(user.game_ids) + 1} 查看绑定的玩家状态')
+    return res
+
+
+async def handler_async(message: str, user_id: str, platform: str, channel_id: str):
+    res = alc.parse(message)
 
     if res.matched:
+        user = get_user(user_id, platform)
         server = server_name_2_server_id(res.serverName)
         r = await tsugu_api_async.bind_player_verification(platform, user.user_id, server, res.playerID, True)
         if r.get('status') != 'success':
             return text_response(r.get('data'))
         return text_response('绑定成功！现在可以使用 玩家状态 {len(user.game_ids) + 1} 查看绑定的玩家状态')
     return res
+
+
+
```

### Comparing `tsugu-1.1.0rc5/tsugu_async/src/remote/player_status.py` & `tsugu-2.0.0/tsugu/src/remote/player_status.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,71 +1,122 @@
-from ...utils import text_response, User, server_id_2_server_name, server_name_2_server_id, server_exists, config
-import tsugu_api_async
+from ...utils import get_user, text_response, User, server_id_2_server_name, server_name_2_server_id, server_exists
+import tsugu_api
 from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager
 from tsugu_api_core._typing import _ServerName
+import tsugu_api_async
 
 
-async def handler(message: str, user: User, platform: str, channel_id: str):
-    res = Alconna(
+alc = Alconna(
         ["玩家状态"],
         Args["serverName", _ServerName.__args__, None]["serverIndex", int, None],
         meta=CommandMeta(
-            compact=config.compact, description="查询自己的玩家状态",
+            compact=True, description="查询自己的玩家状态",
             usage='根据关键词或活动ID查询活动信息',
             example='''玩家状态 :返回玩家状态(优先当前服务器下第一条记录)
 玩家状态 1 :返回绑定的第一条记录的状态
 玩家状态 jp :返回绑定的cn服务器的记录的状态'''
         )
-    ).parse(message)
+    )
+
+
+def handler(message: str, user_id: str, platform: str, channel_id: str):
+    def _utils_search_player_by_game_id(game_id, additional_text=""):
+        player_id = str(game_id.get("game_id"))
+        server = int(game_id.get("server"))
+        response = tsugu_api.search_player(int(player_id), server)
+        return response + text_response(additional_text)
+
+    def _case_default(user: User):
+        # 优先当前服务器
+        for game_id in user.game_ids:
+            if game_id.get("server") == user.server_mode:
+                text = f'已查找默认服务器 {server_id_2_server_name(user.server_mode)} 的记录。'
+                return _utils_search_player_by_game_id(game_id, text)
+        # 兜底逻辑：使用第一个记录
+        if user.game_ids:
+            game_id = user.game_ids[0]
+            text = f'已查找第一个记录。'
+            return _utils_search_player_by_game_id(game_id, text)
+        return text_response('未绑定任何记录，可以使用 绑定玩家 进行绑定')
+
+    def _case_server(user: User, server_name: str):
+        server_id = server_name_2_server_id(server_name)
+        # 服务器不存在
+        if not server_exists(server_id):
+            return text_response(f'服务器 {server_name} 不存在。')
+        # 查找记录
+        for game_id in user.game_ids:
+            if game_id.get("server") == server_id:
+                # 找到记录
+                return _utils_search_player_by_game_id(game_id)
+        # 未找到记录
+        return text_response(f'未在记录中找到服务器 {server_name} 的记录。')
+
+    def _case_index(user: User, index: int):
+        if index > len(user.game_ids) or index < 1:
+            return text_response(f'未找到记录 {index}。')
+        return _utils_search_player_by_game_id(user.game_ids[index - 1])
+
+    res = alc.parse(message)
 
     if res.matched:
+        user = get_user(user_id, platform)
         if res.serverName:
-            return await _case_server(user, res.serverName)
+            return _case_server(user, res.serverName)
         elif res.serverIndex:
-            return await _case_index(user, res.serverIndex)
+            return _case_index(user, res.serverIndex)
         else:
-            return await _case_default(user)
+            return _case_default(user)
     return res
 
 
+async def handler_async(message: str, user_id: str, platform: str, channel_id: str):
+    async def _utils_search_player_by_game_id(game_id, additional_text=""):
+        player_id = str(game_id.get("game_id"))
+        server = int(game_id.get("server"))
+        response = await tsugu_api_async.search_player(int(player_id), server)
+        return response + text_response(additional_text)
+
+    async def _case_default(user: User):
+        # 优先当前服务器
+        for game_id in user.game_ids:
+            if game_id.get("server") == user.server_mode:
+                text = f'已查找默认服务器 {server_id_2_server_name(user.server_mode)} 的记录。'
+                return await _utils_search_player_by_game_id(game_id, text)
+        # 兜底逻辑：使用第一个记录
+        if user.game_ids:
+            game_id = user.game_ids[0]
+            text = f'已查找第一个记录。'
+            return await _utils_search_player_by_game_id(game_id, text)
+        return text_response('未绑定任何记录，可以使用 绑定玩家 进行绑定')
 
-async def _utils_search_player_by_game_id(game_id, additional_text=""):
-    player_id = str(game_id.get("game_id"))
-    server = int(game_id.get("server"))
-    response = await tsugu_api_async.search_player(int(player_id), server)
-    return response + text_response(additional_text)
+    async def _case_server(user: User, server_name: str):
+        server_id = server_name_2_server_id(server_name)
+        # 服务器不存在
+        if not server_exists(server_id):
+            return text_response(f'服务器 {server_name} 不存在。')
+        # 查找记录
+        for game_id in user.game_ids:
+            if game_id.get("server") == server_id:
+                # 找到记录
+                return await _utils_search_player_by_game_id(game_id)
+        # 未找到记录
+        return text_response(f'未在记录中找到服务器 {server_name} 的记录。')
+
+    async def _case_index(user: User, index: int):
+        if index > len(user.game_ids) or index < 1:
+            return text_response(f'未找到记录 {index}。')
+        return await _utils_search_player_by_game_id(user.game_ids[index - 1])
 
+    res = alc.parse(message)
 
-async def _case_default(user: User):
-    # 优先当前服务器
-    for game_id in user.game_ids:
-        if game_id.get("server") == user.server_mode:
-            text = f'已查找默认服务器 {server_id_2_server_name(user.server_mode)} 的记录。'
-            return await _utils_search_player_by_game_id(game_id, text)
-    # 兜底逻辑：使用第一个记录
-    if user.game_ids:
-        game_id = user.game_ids[0]
-        text = f'已查找第一个记录。'
-        return await _utils_search_player_by_game_id(game_id, text)
-    return text_response('未绑定任何记录，可以使用 绑定玩家 进行绑定')
-
-
-async def _case_server(user: User, server_name: str):
-    server_id = server_name_2_server_id(server_name)
-    # 服务器不存在
-    if not server_exists(server_id):
-        return text_response(f'服务器 {server_name} 不存在。')
-    # 查找记录
-    for game_id in user.game_ids:
-        if game_id.get("server") == server_id:
-            # 找到记录
-            return await _utils_search_player_by_game_id(game_id)
-    # 未找到记录
-    return text_response(f'未在记录中找到服务器 {server_name} 的记录。')
-
-
-async def _case_index(user: User, index: int):
-    if index > len(user.game_ids) or index < 1:
-        return text_response(f'未找到记录 {index}。')
-    return await _utils_search_player_by_game_id(user.game_ids[index - 1])
+    if res.matched:
+        user = get_user(user_id, platform)
+        if res.serverName:
+            return await _case_server(user, res.serverName)
+        elif res.serverIndex:
+            return await _case_index(user, res.serverIndex)
+        else:
+            return await _case_default(user)
+    return res
```

### Comparing `tsugu-1.1.0rc5/tsugu_async/src/remote/unbind_player.py` & `tsugu-2.0.0/tsugu/src/remote/unbind_player.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,43 +1,77 @@
-from ...utils import text_response, User, server_id_2_server_name, server_name_2_server_id, server_exists, config
-import tsugu_api_async
+from ...utils import get_user, text_response, User, server_id_2_server_name, server_name_2_server_id
+import tsugu_api
 from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager
+import tsugu_api_async
 
 
-async def handler(message: str, user: User, platform: str, channel_id: str):
-    res = Alconna(
+alc = Alconna(
         ["解除绑定"],
         Args["index#要解绑的绑定编号", int, None],
         meta=CommandMeta(
-            compact=config.compact, description="解除绑定",
+            compact=True, description="解除绑定",
             usage="验证解绑 记录编号(数字)",
             example="验证解绑 1 : 解绑第一个记录"
         ),
-    ).parse(message)
+    )
+
+
+def handler(message: str, user_id: str, platform: str, channel_id: str):
+    def mask_data(game_id: str):
+        game_id = str(game_id)
+        if len(game_id) < 6:
+            return game_id[:3] + '*' * (len(game_id) - 3)
+        elif len(game_id) < 3:
+            return '*' * len(game_id)
+        else:
+            game_id = game_id[:3] + '*' * (len(game_id) - 6) + game_id[-3:]
+        return game_id
+
+    res = alc.parse(message)
 
     if res.matched:
+        user = get_user(user_id, platform)
         if not res.index:
             bind_record = '\n'.join([f'{i + 1}. {mask_data(x.get("game_id"))} {server_id_2_server_name(x.get("server"))}' for i, x in enumerate(user.game_ids)])
             return text_response('请输入正确的记录(数字)\n例如: 解除绑定 1\n当前的绑定记录如下:\n' + bind_record)
 
         if len(user.game_ids) < int(res.index):
             return text_response('未找到记录')
 
         server_mode = user.game_ids[int(res.index) - 1].get("server")
 
-        r = await tsugu_api_async.bind_player_request(platform, user.user_id, server_mode, False)
+        r = tsugu_api.bind_player_request(platform, user.user_id, server_mode, False)
         if r.get('status') != 'success':
             return text_response(r.get('data'))
         return text_response(f'''正在解除，请将 评论(个性签名) 或者 当前使用的 乐队编队名称改为\n{r.get('data')['verifyCode']}\n稍等片刻等待同步后，发送\n验证解绑 {res.index}\n来完成本次身份验证''')
     return res
 
 
-def mask_data(game_id: str):
-    game_id = str(game_id)
-    if len(game_id) < 6:
-        return game_id[:3] + '*' * (len(game_id) - 3)
-    elif len(game_id) < 3:
-        return '*' * len(game_id)
-    else:
-        game_id = game_id[:3] + '*' * (len(game_id) - 6) + game_id[-3:]
-    return game_id
+async def handler_async(message: str, user_id: str, platform: str, channel_id: str):
+    def mask_data(game_id: str):
+        game_id = str(game_id)
+        if len(game_id) < 6:
+            return game_id[:3] + '*' * (len(game_id) - 3)
+        elif len(game_id) < 3:
+            return '*' * len(game_id)
+        else:
+            game_id = game_id[:3] + '*' * (len(game_id) - 6) + game_id[-3:]
+        return game_id
 
+    res = alc.parse(message)
+
+    if res.matched:
+        user = get_user(user_id, platform)
+        if not res.index:
+            bind_record = '\n'.join([f'{i + 1}. {mask_data(x.get("game_id"))} {server_id_2_server_name(x.get("server"))}' for i, x in enumerate(user.game_ids)])
+            return text_response('请输入正确的记录(数字)\n例如: 解除绑定 1\n当前的绑定记录如下:\n' + bind_record)
+
+        if len(user.game_ids) < int(res.index):
+            return text_response('未找到记录')
+
+        server_mode = user.game_ids[int(res.index) - 1].get("server")
+
+        r = await tsugu_api_async.bind_player_request(platform, user.user_id, server_mode, False)
+        if r.get('status') != 'success':
+            return text_response(r.get('data'))
+        return text_response(f'''正在解除，请将 评论(个性签名) 或者 当前使用的 乐队编队名称改为\n{r.get('data')['verifyCode']}\n稍等片刻等待同步后，发送\n验证解绑 {res.index}\n来完成本次身份验证''')
+    return res
```

### Comparing `tsugu-1.1.0rc5/tsugu_async/src/universal/search_character.py` & `tsugu-2.0.0/tsugu/src/universal/search_character.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,37 @@
-from ...utils import text_response, User, server_id_2_server_name, server_name_2_server_id, server_exists, config
+from ...utils import get_user, text_response, User, server_id_2_server_name, server_name_2_server_id
+import tsugu_api
+from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, AllParam
 import tsugu_api_async
-from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, MultiVar
 
-
-async def handler(message: str, user: User, platform: str, channel_id: str):
-    res = Alconna(
+alc = Alconna(
         ["查角色"],
-        Args["word#角色名，乐队，昵称等查询参数", MultiVar(str)],
+        Args["word#角色名，乐队，昵称等查询参数", AllParam],
         meta=CommandMeta(
-            compact=config.compact, description="查询角色信息",
+            compact=True, description="查询角色信息",
             usage='根据关键词或角色ID查询角色信息',
             example='''查角色 10 :返回10号角色的信息。
 查角色 吉他 :返回所有角色模糊搜索标签中包含吉他的角色列表。'''
         )
-    ).parse(message)
+    )
+
+
+def handler(message: str, user_id: str, platform: str, channel_id: str):
+    res = alc.parse(message)
 
     if res.matched:
+        user = get_user(user_id, platform)
+        return tsugu_api.search_character(user.default_server, " ".join(res.word))
+
+    return res
+
+
+async def handler_async(message: str, user_id: str, platform: str, channel_id: str):
+    res = alc.parse(message)
+
+    if res.matched:
+        user = get_user(user_id, platform)
         return await tsugu_api_async.search_character(user.default_server, " ".join(res.word))
 
     return res
+
+
```

### Comparing `tsugu-1.1.0rc5/tsugu_thread/src/remote/bind_player_verification_off.py` & `tsugu-2.0.0/tsugu/src/universal/search_song.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,33 +1,40 @@
 from ...utils import get_user, text_response, User, server_id_2_server_name, server_name_2_server_id
 import tsugu_api
-from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager
+from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, AllParam
+import tsugu_api_async
 
 
 alc = Alconna(
-        ["验证解绑"],
-        Args["index#要解绑的绑定编号", int],
+        ["查曲"],
+        Args["word#歌曲信息，名称，乐队，难度等。", AllParam],
         meta=CommandMeta(
-            compact=True, description="验证解绑",
-            usage="验证解绑 记录编号(数字)",
-            example="验证解绑 1 : 解绑第一个记录"
-        ),
+            compact=True, description="查曲",
+            usage='根据关键词或曲目ID查询曲目信息。',
+            example='''查曲 1 :返回1号曲的信息
+查曲 ag lv27 :返回所有难度为27的ag曲列表
+查曲 >27 :查询大于27的曲目
+查曲 滑滑蛋 :匹配歌曲 fuwa fuwa time'''
+        )
     )
 
 
 def handler(message: str, user_id: str, platform: str, channel_id: str):
     res = alc.parse(message)
 
     if res.matched:
         user = get_user(user_id, platform)
-        if len(user.game_ids) < int(res.index):
-            return text_response('未找到记录')
-        player_id = user.game_ids[int(res.index) - 1].get("game_id")
-        server_mode = user.game_ids[int(res.index) - 1].get("server")
-        r = tsugu_api.bind_player_verification(platform, user.user_id, server_mode, player_id, False)
-        if r.get('status') != 'success':
-            return text_response(r.get('data'))
-        return text_response('解绑成功！')
-    
+        return tsugu_api.search_song(user.default_server, " ".join(res.word))
+
+    return res
+
+
+async def handler_async(message: str, user_id: str, platform: str, channel_id: str):
+    res = alc.parse(message)
+
+    if res.matched:
+        user = get_user(user_id, platform)
+        return await tsugu_api_async.search_song(user.default_server, " ".join(res.word))
+
     return res
```

### Comparing `tsugu-1.1.0rc5/tsugu_thread/src/universal/song_meta.py` & `tsugu-2.0.0/tsugu/src/universal/song_meta.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from ...utils import get_user, text_response, User, server_id_2_server_name, server_name_2_server_id
 import tsugu_api
 from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager
 from tsugu_api_core._typing import _ServerName
+import tsugu_api_async
 
 
 alc = Alconna(
         ["查询分数表", '查分数表', '查询分数榜', '查分数榜'],
         Args["serverName;?#省略服务器名时，默认从你当前的主服务器查询。", _ServerName.__args__],
         meta=CommandMeta(
             compact=True, description="查询分数表",
@@ -24,7 +25,22 @@
             server = server_name_2_server_id(res.serverName)
         else:
             server = user.server_mode
         return tsugu_api.song_meta(user.default_server, server)
 
     return res
 
+
+async def handler_async(message: str, user_id: str, platform: str, channel_id: str):
+    res = alc.parse(message)
+
+    if res.matched:
+        user = get_user(user_id, platform)
+        if res.serverName:
+            server = server_name_2_server_id(res.serverName)
+        else:
+            server = user.server_mode
+        return await tsugu_api_async.song_meta(user.default_server, server)
+
+    return res
+
+
```

