# Comparing `tmp/feeluown-4.1.3.tar.gz` & `tmp/feeluown-4.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feeluown-4.1.3.tar", last modified: Sun Apr 21 10:24:43 2024, max compression
+gzip compressed data, was "feeluown-4.1.4.tar", last modified: Tue May 21 15:53:38 2024, max compression
```

## Comparing `feeluown-4.1.3.tar` & `feeluown-4.1.4.tar`

### file list

```diff
@@ -1,286 +1,287 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:43.329369 feeluown-4.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-04-21 10:24:42.000000 feeluown-4.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4711 2024-04-21 10:24:43.329369 feeluown-4.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-04-21 10:24:42.000000 feeluown-4.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:43.297368 feeluown-4.1.3/feeluown/
--rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      158 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:43.297368 feeluown-4.1.3/feeluown/app/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10370 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/app/app.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/app/cli_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/app/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5643 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/app/gui_app.py
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/app/mixed_app.py
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/app/mode.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/app/once_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/app/server_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     6008 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/argparser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:43.297368 feeluown-4.1.3/feeluown/cli/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7402 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/cli/cli.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4208 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/cli/install.py
--rw-r--r--   0 runner    (1001) docker     (127)    13808 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/consts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:43.297368 feeluown-4.1.3/feeluown/entry_points/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/entry_points/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/entry_points/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/entry_points/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     6977 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/entry_points/run_app.py
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/entry_points/run_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/excs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:43.297368 feeluown-4.1.3/feeluown/fuoexec/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/fuoexec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/fuoexec/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/fuoexec/fuoexec.py
--rw-r--r--   0 runner    (1001) docker     (127)     4921 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/fuoexec/signal_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:43.301368 feeluown-4.1.3/feeluown/gui/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:43.293368 feeluown-4.1.3/feeluown/gui/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:43.305369 feeluown-4.1.3/feeluown/gui/assets/icons/
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/assets/icons/already_download.png
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/assets/icons/already_downloaded_dark.png
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/assets/icons/cur_playlist.png
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/assets/icons/cur_playlist_dark.png
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/assets/icons/download.png
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/assets/icons/download_dark.png
--rwxr-xr-x   0 runner    (1001) docker     (127)   303153 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/assets/icons/feeluown.icns
--rw-r--r--   0 runner    (1001) docker     (127)   112526 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/assets/icons/feeluown.ico
--rw-r--r--   0 runner    (1001) docker     (127)    35773 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/assets/icons/feeluown.png
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/assets/icons/like.png
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/assets/icons/like_checked.png
--rw-r--r--   0 runner    (1001) docker     (127)      980 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/assets/icons/like_checked_dark.png
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/assets/icons/like_dark.png
--rw-r--r--   0 runner    (1001) docker     (127)     7730 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/assets/icons/tray-dark.png
--rw-r--r--   0 runner    (1001) docker     (127)     7712 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/assets/icons/tray-light.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:43.305369 feeluown-4.1.3/feeluown/gui/assets/themes/
--rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/assets/themes/common.qss
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/assets/themes/dark.qss
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/assets/themes/light.qss
--rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/assets/themes/macos_dark.colors
--rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/base_renderer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7771 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/browser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:43.305369 feeluown-4.1.3/feeluown/gui/components/
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6291 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/components/avatar.py
--rw-r--r--   0 runner    (1001) docker     (127)     7084 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/components/btns.py
--rw-r--r--   0 runner    (1001) docker     (127)     3649 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/components/collections.py
--rw-r--r--   0 runner    (1001) docker     (127)     5608 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/components/line_song.py
--rw-r--r--   0 runner    (1001) docker     (127)     5187 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/components/menu.py
--rw-r--r--   0 runner    (1001) docker     (127)     8901 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/components/nowplaying.py
--rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/components/player_playlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/components/player_progress.py
--rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/components/playlist_btn.py
--rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/components/song_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/components/volume_slider.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)    13876 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/drawers.py
--rw-r--r--   0 runner    (1001) docker     (127)    20611 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/hotkey.py
--rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/mimedata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:43.305369 feeluown-4.1.3/feeluown/gui/page_containers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/page_containers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/page_containers/scroll_area.py
--rw-r--r--   0 runner    (1001) docker     (127)    20407 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/page_containers/table.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:43.309368 feeluown-4.1.3/feeluown/gui/pages/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/pages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/pages/coll_mixed.py
--rw-r--r--   0 runner    (1001) docker     (127)     4901 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/pages/homepage.py
--rw-r--r--   0 runner    (1001) docker     (127)     8315 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/pages/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/pages/my_fav.py
--rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/pages/provider_home.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/pages/recently_played.py
--rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/pages/recommendation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/pages/recommendation_daily_songs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5432 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/pages/search.py
--rw-r--r--   0 runner    (1001) docker     (127)    13654 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/pages/song_explore.py
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/pages/template.py
--rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/provider_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     5263 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/theme.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/tips.py
--rw-r--r--   0 runner    (1001) docker     (127)     7682 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/tray.py
--rw-r--r--   0 runner    (1001) docker     (127)     3658 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:43.309368 feeluown-4.1.3/feeluown/gui/uimain/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/uimain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10284 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/uimain/floating_box.py
--rw-r--r--   0 runner    (1001) docker     (127)    15321 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/uimain/lyric.py
--rw-r--r--   0 runner    (1001) docker     (127)     7981 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/uimain/nowplaying_overlay.py
--rw-r--r--   0 runner    (1001) docker     (127)    12168 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/uimain/page_view.py
--rw-r--r--   0 runner    (1001) docker     (127)     8284 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/uimain/player_bar.py
--rw-r--r--   0 runner    (1001) docker     (127)     7272 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/uimain/playlist_overlay.py
--rw-r--r--   0 runner    (1001) docker     (127)    13016 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/uimain/sidebar.py
--rw-r--r--   0 runner    (1001) docker     (127)     4653 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/uimain/toolbar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:43.309368 feeluown-4.1.3/feeluown/gui/uimodels/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/uimodels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/uimodels/my_music.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/uimodels/playlist.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/uimodels/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     7443 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/watch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:43.317369 feeluown-4.1.3/feeluown/gui/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/widgets/accordion.py
--rw-r--r--   0 runner    (1001) docker     (127)     8150 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/widgets/comment_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/widgets/cover_label.py
--rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/widgets/frameless.py
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/widgets/header.py
--rw-r--r--   0 runner    (1001) docker     (127)    16619 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/widgets/img_card_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/widgets/labels.py
--rw-r--r--   0 runner    (1001) docker     (127)     9674 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/widgets/login.py
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/widgets/lyric.py
--rw-r--r--   0 runner    (1001) docker     (127)     4150 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/widgets/magicbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/widgets/messageline.py
--rw-r--r--   0 runner    (1001) docker     (127)     7558 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/widgets/meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     5747 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/widgets/mpv_.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/widgets/my_music.py
--rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/widgets/playlist_button.py
--rw-r--r--   0 runner    (1001) docker     (127)     5097 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/widgets/playlists.py
--rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/widgets/progress_slider.py
--rw-r--r--   0 runner    (1001) docker     (127)     5599 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/widgets/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)    17587 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/widgets/selfpaint_btn.py
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/widgets/separator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3178 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/widgets/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/widgets/size_grip.py
--rw-r--r--   0 runner    (1001) docker     (127)    10623 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/widgets/song_minicard_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    27444 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/widgets/songs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4101 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/widgets/statusline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:43.317369 feeluown-4.1.3/feeluown/gui/widgets/statusline_items/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/widgets/statusline_items/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/widgets/statusline_items/notify.py
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/widgets/statusline_items/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     7314 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/widgets/tabbar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3599 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/widgets/table_toolbar.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/widgets/textbtn.py
--rw-r--r--   0 runner    (1001) docker     (127)     4356 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/widgets/textlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     6609 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/widgets/video.py
--rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/widgets/volume_button.py
--rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/widgets/weblogin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:43.317369 feeluown-4.1.3/feeluown/library/
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/library/abc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3894 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/library/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/library/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/library/excs.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/library/flags.py
--rw-r--r--   0 runner    (1001) docker     (127)    14832 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/library/library.py
--rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/library/model_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/library/model_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    15060 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/library/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4969 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/library/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)    10825 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/library/provider_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     8946 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/library/uri.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:43.317369 feeluown-4.1.3/feeluown/local/
--rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16282 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/local/db.py
--rw-r--r--   0 runner    (1001) docker     (127)     5229 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/local/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/local/provider_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/local/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/local/ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     7630 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/media.py
--rw-r--r--   0 runner    (1001) docker     (127)    79978 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/mpv.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:43.321369 feeluown-4.1.3/feeluown/nowplaying/
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/nowplaying/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:43.321369 feeluown-4.1.3/feeluown/nowplaying/linux/
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/nowplaying/linux/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/nowplaying/linux/introspect.xml
--rw-r--r--   0 runner    (1001) docker     (127)     9226 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/nowplaying/linux/mpris2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/nowplaying/macos.py
--rw-r--r--   0 runner    (1001) docker     (127)     5732 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/nowplaying/nowplaying.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:43.321369 feeluown-4.1.3/feeluown/player/
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/player/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6859 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/player/base_player.py
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/player/delegate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/player/fm.py
--rw-r--r--   0 runner    (1001) docker     (127)     6755 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/player/lyric.py
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/player/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    12750 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/player/mpvplayer.py
--rw-r--r--   0 runner    (1001) docker     (127)    25849 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/player/playlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/player/radio.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/player/recently_played.py
--rw-r--r--   0 runner    (1001) docker     (127)     7324 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:43.321369 feeluown-4.1.3/feeluown/pyinstaller/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/pyinstaller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/pyinstaller/hook.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/pyinstaller/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:43.321369 feeluown-4.1.3/feeluown/serializers/
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/serializers/_plain_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/serializers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/serializers/json_.py
--rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/serializers/model_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/serializers/objs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8154 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/serializers/plain.py
--rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/serializers/python.py
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/serializers/typename.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:43.325369 feeluown-4.1.3/feeluown/server/
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/server/data_structure.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:43.325369 feeluown-4.1.3/feeluown/server/dslv1/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/server/dslv1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/server/dslv1/codegen.py
--rw-r--r--   0 runner    (1001) docker     (127)     5448 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/server/dslv1/lexer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7315 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/server/dslv1/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     6299 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/server/dslv2.py
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/server/excs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:43.325369 feeluown-4.1.3/feeluown/server/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/server/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/server/handlers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/server/handlers/cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/server/handlers/excs.py
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/server/handlers/exec_.py
--rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/server/handlers/handle.py
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/server/handlers/help.py
--rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/server/handlers/player.py
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/server/handlers/playlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/server/handlers/search.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/server/handlers/set_.py
--rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/server/handlers/show.py
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/server/handlers/status.py
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/server/handlers/sub.py
--rw-r--r--   0 runner    (1001) docker     (127)     9176 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/server/protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:43.329369 feeluown-4.1.3/feeluown/server/pubsub/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/server/pubsub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/server/pubsub/gateway.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/server/pubsub/publishers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:43.329369 feeluown-4.1.3/feeluown/server/rpc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/server/rpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/server/server.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/server/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     4145 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:43.329369 feeluown-4.1.3/feeluown/uimodels/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/uimodels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/uimodels/my_music.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/uimodels/playlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/uimodels/provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:43.329369 feeluown-4.1.3/feeluown/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/utils/aio.py
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/utils/audio.py
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/utils/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4585 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/utils/dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/utils/lang.py
--rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/utils/patch.py
--rw-r--r--   0 runner    (1001) docker     (127)    12691 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/utils/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/utils/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/utils/router.py
--rw-r--r--   0 runner    (1001) docker     (127)    13634 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/utils/sync.py
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/utils/typing_.py
--rw-r--r--   0 runner    (1001) docker     (127)     7700 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    54535 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/utils/yt_dlp_cookies.py
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:43.329369 feeluown-4.1.3/feeluown/webserver/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/webserver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/webserver/jsonrpc_.py
--rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/webserver/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:43.297368 feeluown-4.1.3/feeluown.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4711 2024-04-21 10:24:43.000000 feeluown-4.1.3/feeluown.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7817 2024-04-21 10:24:43.000000 feeluown-4.1.3/feeluown.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 10:24:43.000000 feeluown-4.1.3/feeluown.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-21 10:24:43.000000 feeluown-4.1.3/feeluown.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-21 10:24:43.000000 feeluown-4.1.3/feeluown.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-21 10:24:43.000000 feeluown-4.1.3/feeluown.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-21 10:24:43.333369 feeluown-4.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-04-21 10:24:42.000000 feeluown-4.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:38.112632 feeluown-4.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-05-21 15:53:36.000000 feeluown-4.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4711 2024-05-21 15:53:38.112632 feeluown-4.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-05-21 15:53:36.000000 feeluown-4.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:38.076632 feeluown-4.1.4/feeluown/
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      158 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:38.080632 feeluown-4.1.4/feeluown/app/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10370 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/app/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/app/cli_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/app/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5643 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/app/gui_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/app/mixed_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/app/mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/app/once_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/app/server_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6008 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/argparser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:38.080632 feeluown-4.1.4/feeluown/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7402 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/cli/cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4208 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/cli/install.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13808 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/consts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:38.080632 feeluown-4.1.4/feeluown/entry_points/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/entry_points/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/entry_points/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/entry_points/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6977 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/entry_points/run_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/entry_points/run_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/excs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:38.080632 feeluown-4.1.4/feeluown/fuoexec/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/fuoexec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/fuoexec/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/fuoexec/fuoexec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4921 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/fuoexec/signal_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:38.084632 feeluown-4.1.4/feeluown/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:38.072632 feeluown-4.1.4/feeluown/gui/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:38.084632 feeluown-4.1.4/feeluown/gui/assets/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/assets/icons/already_download.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/assets/icons/already_downloaded_dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/assets/icons/cur_playlist.png
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/assets/icons/cur_playlist_dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/assets/icons/download.png
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/assets/icons/download_dark.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)   303153 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/assets/icons/feeluown.icns
+-rw-r--r--   0 runner    (1001) docker     (127)   112526 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/assets/icons/feeluown.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    35773 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/assets/icons/feeluown.png
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/assets/icons/like.png
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/assets/icons/like_checked.png
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/assets/icons/like_checked_dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/assets/icons/like_dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7730 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/assets/icons/tray-dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7712 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/assets/icons/tray-light.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:38.084632 feeluown-4.1.4/feeluown/gui/assets/themes/
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/assets/themes/common.qss
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/assets/themes/dark.qss
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/assets/themes/light.qss
+-rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/assets/themes/macos_dark.colors
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/base_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7885 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/browser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:38.088632 feeluown-4.1.4/feeluown/gui/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7315 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/components/avatar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7084 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/components/btns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3649 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/components/collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5608 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/components/line_song.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5187 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/components/menu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8901 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/components/nowplaying.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/components/player_playlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/components/player_progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/components/playlist_btn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/components/song_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/components/volume_slider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14378 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/drawers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20611 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/hotkey.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/mimedata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:38.088632 feeluown-4.1.4/feeluown/gui/page_containers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/page_containers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/page_containers/scroll_area.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20407 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/page_containers/table.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:38.088632 feeluown-4.1.4/feeluown/gui/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/pages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/pages/coll_mixed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5554 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/pages/homepage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8315 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/pages/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/pages/my_fav.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/pages/provider_home.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/pages/recently_played.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3634 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/pages/recommendation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/pages/recommendation_daily_songs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5432 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/pages/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13654 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/pages/song_explore.py
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/pages/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/pages/toplist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/provider_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5263 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/theme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/tips.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7682 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/tray.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3658 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:38.092632 feeluown-4.1.4/feeluown/gui/uimain/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/uimain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10284 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/uimain/floating_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15321 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/uimain/lyric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7981 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/uimain/nowplaying_overlay.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12168 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/uimain/page_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8284 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/uimain/player_bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7272 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/uimain/playlist_overlay.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13716 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/uimain/sidebar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/uimain/toolbar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:38.092632 feeluown-4.1.4/feeluown/gui/uimodels/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/uimodels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/uimodels/my_music.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/uimodels/playlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/uimodels/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7443 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/watch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:38.096632 feeluown-4.1.4/feeluown/gui/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/widgets/accordion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8150 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/widgets/comment_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/widgets/cover_label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/widgets/frameless.py
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/widgets/header.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16619 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/widgets/img_card_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/widgets/labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9674 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/widgets/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/widgets/lyric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4150 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/widgets/magicbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/widgets/messageline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7558 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/widgets/meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5747 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/widgets/mpv_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/widgets/my_music.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/widgets/playlist_button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5097 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/widgets/playlists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/widgets/progress_slider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5599 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/widgets/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17587 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/widgets/selfpaint_btn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/widgets/separator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3178 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/widgets/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/widgets/size_grip.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10623 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/widgets/song_minicard_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27444 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/widgets/songs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4101 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/widgets/statusline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:38.096632 feeluown-4.1.4/feeluown/gui/widgets/statusline_items/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/widgets/statusline_items/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/widgets/statusline_items/notify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/widgets/statusline_items/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7314 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/widgets/tabbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3599 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/widgets/table_toolbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/widgets/textbtn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4356 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/widgets/textlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6609 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/widgets/video.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/widgets/volume_button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/widgets/weblogin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:38.100632 feeluown-4.1.4/feeluown/library/
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/library/abc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3894 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/library/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/library/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/library/excs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/library/flags.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14832 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/library/library.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/library/model_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/library/model_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15060 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/library/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4969 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/library/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11387 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/library/provider_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8946 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/library/uri.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:38.100632 feeluown-4.1.4/feeluown/local/
+-rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16282 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/local/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5229 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/local/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/local/provider_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/local/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/local/ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7630 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/media.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79978 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/mpv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:38.100632 feeluown-4.1.4/feeluown/nowplaying/
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/nowplaying/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:38.100632 feeluown-4.1.4/feeluown/nowplaying/linux/
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/nowplaying/linux/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/nowplaying/linux/introspect.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     9226 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/nowplaying/linux/mpris2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/nowplaying/macos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5732 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/nowplaying/nowplaying.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:38.104632 feeluown-4.1.4/feeluown/player/
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/player/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6859 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/player/base_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/player/delegate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/player/fm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6755 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/player/lyric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/player/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13238 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/player/mpvplayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25849 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/player/playlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/player/radio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/player/recently_played.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7324 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:38.104632 feeluown-4.1.4/feeluown/pyinstaller/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/pyinstaller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/pyinstaller/hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/pyinstaller/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:38.104632 feeluown-4.1.4/feeluown/serializers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/serializers/_plain_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/serializers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/serializers/json_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/serializers/model_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/serializers/objs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8154 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/serializers/plain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/serializers/python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/serializers/typename.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:38.104632 feeluown-4.1.4/feeluown/server/
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/server/data_structure.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:38.104632 feeluown-4.1.4/feeluown/server/dslv1/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/server/dslv1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/server/dslv1/codegen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5448 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/server/dslv1/lexer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7315 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/server/dslv1/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6299 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/server/dslv2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/server/excs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:38.108632 feeluown-4.1.4/feeluown/server/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/server/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/server/handlers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/server/handlers/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/server/handlers/excs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/server/handlers/exec_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/server/handlers/handle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/server/handlers/help.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/server/handlers/player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/server/handlers/playlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/server/handlers/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/server/handlers/set_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/server/handlers/show.py
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/server/handlers/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/server/handlers/sub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9176 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/server/protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:38.108632 feeluown-4.1.4/feeluown/server/pubsub/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/server/pubsub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/server/pubsub/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/server/pubsub/publishers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:38.108632 feeluown-4.1.4/feeluown/server/rpc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/server/rpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/server/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/server/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4145 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:38.108632 feeluown-4.1.4/feeluown/uimodels/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/uimodels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/uimodels/my_music.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/uimodels/playlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/uimodels/provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:38.112632 feeluown-4.1.4/feeluown/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/utils/aio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/utils/audio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/utils/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4585 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/utils/dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/utils/lang.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/utils/patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12691 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/utils/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/utils/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/utils/router.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13634 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/utils/sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/utils/typing_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7700 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54535 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/utils/yt_dlp_cookies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:38.112632 feeluown-4.1.4/feeluown/webserver/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/webserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/webserver/jsonrpc_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/webserver/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:38.076632 feeluown-4.1.4/feeluown.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4711 2024-05-21 15:53:37.000000 feeluown-4.1.4/feeluown.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7847 2024-05-21 15:53:38.000000 feeluown-4.1.4/feeluown.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 15:53:37.000000 feeluown-4.1.4/feeluown.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-21 15:53:37.000000 feeluown-4.1.4/feeluown.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-21 15:53:37.000000 feeluown-4.1.4/feeluown.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-21 15:53:37.000000 feeluown-4.1.4/feeluown.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-21 15:53:38.112632 feeluown-4.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-05-21 15:53:36.000000 feeluown-4.1.4/setup.py
```

### Comparing `feeluown-4.1.3/LICENSE` & `feeluown-4.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/PKG-INFO` & `feeluown-4.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feeluown
-Version: 4.1.3
+Version: 4.1.4
 Summary: *nix music player
 Home-page: https://github.com/feeluown/FeelUOwn
 Author: feeluown
 Author-email: yinshaowen241@gmail.com
 License: GPL-3.0
 Description: ## FeelUOwn - feel your own
```

### Comparing `feeluown-4.1.3/README.md` & `feeluown-4.1.4/README.md`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/__init__.py` & `feeluown-4.1.4/feeluown/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import logging
 import logging.config
 
 from .consts import LOG_FILE
 
 
-__version__ = '4.1.3'
+__version__ = '4.1.4'
 
 
 dict_config = {
     'version': 1,
     'disable_existing_loggers': False,
     'formatters': {
         'standard': {
```

### Comparing `feeluown-4.1.3/feeluown/app/app.py` & `feeluown-4.1.4/feeluown/app/app.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/app/cli_app.py` & `feeluown-4.1.4/feeluown/app/cli_app.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/app/config.py` & `feeluown-4.1.4/feeluown/app/config.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/app/gui_app.py` & `feeluown-4.1.4/feeluown/app/gui_app.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/app/server_app.py` & `feeluown-4.1.4/feeluown/app/server_app.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/argparser.py` & `feeluown-4.1.4/feeluown/argparser.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/cli/cli.py` & `feeluown-4.1.4/feeluown/cli/cli.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/cli/install.py` & `feeluown-4.1.4/feeluown/cli/install.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/collection.py` & `feeluown-4.1.4/feeluown/collection.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/config.py` & `feeluown-4.1.4/feeluown/config.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/entry_points/base.py` & `feeluown-4.1.4/feeluown/entry_points/base.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/entry_points/run.py` & `feeluown-4.1.4/feeluown/entry_points/run.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/entry_points/run_app.py` & `feeluown-4.1.4/feeluown/entry_points/run_app.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/excs.py` & `feeluown-4.1.4/feeluown/excs.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/fuoexec/functions.py` & `feeluown-4.1.4/feeluown/fuoexec/functions.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/fuoexec/fuoexec.py` & `feeluown-4.1.4/feeluown/fuoexec/fuoexec.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/fuoexec/signal_manager.py` & `feeluown-4.1.4/feeluown/fuoexec/signal_manager.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/assets/icons/already_download.png` & `feeluown-4.1.4/feeluown/gui/assets/icons/already_download.png`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/assets/icons/already_downloaded_dark.png` & `feeluown-4.1.4/feeluown/gui/assets/icons/already_downloaded_dark.png`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/assets/icons/cur_playlist.png` & `feeluown-4.1.4/feeluown/gui/assets/icons/cur_playlist.png`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/assets/icons/cur_playlist_dark.png` & `feeluown-4.1.4/feeluown/gui/assets/icons/cur_playlist_dark.png`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/assets/icons/download.png` & `feeluown-4.1.4/feeluown/gui/assets/icons/download.png`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/assets/icons/download_dark.png` & `feeluown-4.1.4/feeluown/gui/assets/icons/download_dark.png`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/assets/icons/feeluown.icns` & `feeluown-4.1.4/feeluown/gui/assets/icons/feeluown.icns`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/assets/icons/feeluown.ico` & `feeluown-4.1.4/feeluown/gui/assets/icons/feeluown.ico`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/assets/icons/feeluown.png` & `feeluown-4.1.4/feeluown/gui/assets/icons/feeluown.png`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/assets/icons/like.png` & `feeluown-4.1.4/feeluown/gui/assets/icons/like.png`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/assets/icons/like_checked.png` & `feeluown-4.1.4/feeluown/gui/assets/icons/like_checked.png`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/assets/icons/like_checked_dark.png` & `feeluown-4.1.4/feeluown/gui/assets/icons/like_checked_dark.png`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/assets/icons/like_dark.png` & `feeluown-4.1.4/feeluown/gui/assets/icons/like_dark.png`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/assets/icons/tray-dark.png` & `feeluown-4.1.4/feeluown/gui/assets/icons/tray-dark.png`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/assets/icons/tray-light.png` & `feeluown-4.1.4/feeluown/gui/assets/icons/tray-light.png`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/assets/themes/common.qss` & `feeluown-4.1.4/feeluown/gui/assets/themes/common.qss`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 QWidget {
     /* font-size: 13px; */
     /* tips: you can turn on border for debugging */
     /* border: 1px solid red; */
 }
 
-LeftPanel QLabel {
+LeftPanel QLabel, LeftPanel TriagleButton, LeftPanel PlusButton {
     color: #888;
 }
 
 LeftPanel QLabel {
     padding-top: 3px;
     padding-bottom: 3px;
 }
```

### Comparing `feeluown-4.1.3/feeluown/gui/assets/themes/dark.qss` & `feeluown-4.1.4/feeluown/gui/assets/themes/dark.qss`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/assets/themes/light.qss` & `feeluown-4.1.4/feeluown/gui/assets/themes/light.qss`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/assets/themes/macos_dark.colors` & `feeluown-4.1.4/feeluown/gui/assets/themes/macos_dark.colors`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/base_renderer.py` & `feeluown-4.1.4/feeluown/gui/base_renderer.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/browser.py` & `feeluown-4.1.4/feeluown/gui/browser.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,14 +194,15 @@
         from feeluown.gui.pages.provider_home import render as render_provider_home
         from feeluown.gui.pages.recently_played import render as render_recently_played
         from feeluown.gui.pages.recommendation import render as render_rec
         from feeluown.gui.pages.recommendation_daily_songs import \
             render as render_rec_daily_songs
         from feeluown.gui.pages.my_fav import render as render_my_fav
         from feeluown.gui.pages.homepage import render as render_homepage
+        from feeluown.gui.pages.toplist import render as render_toplist
 
         model_prefix = f'{MODEL_PAGE_PREFIX}<provider>'
 
         async def dummy_render(req, *args, **kwargs):
             warnings.warn(f'This route:{req.rule} will be removed.')
 
         urlpatterns = [
@@ -214,10 +215,11 @@
             ('/providers/<identifier>', render_provider_home),
             ('/recently_played', render_recently_played),
             ('/search', render_search),
             ('/rec', render_rec),
             ('/homepage', render_homepage),
             ('/rec/daily_songs', render_rec_daily_songs),
             ('/my_fav', render_my_fav),
+            ('/toplist', render_toplist),
         ]
         for url, renderer in urlpatterns:
             self.route(url)(renderer)
```

### Comparing `feeluown-4.1.3/feeluown/gui/components/__init__.py` & `feeluown-4.1.4/feeluown/gui/components/__init__.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/components/avatar.py` & `feeluown-4.1.4/feeluown/gui/components/avatar.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,48 @@
 from typing import TYPE_CHECKING
 
+from PyQt5.QtCore import QRect
 from PyQt5.QtWidgets import QMenu, QAction
 from PyQt5.QtGui import QPainter, QIcon, QPalette, QContextMenuEvent
 
 from feeluown.library import UserModel, SupportsCurrentUser
 from feeluown.library import reverse
 from feeluown.utils.aio import run_afn, run_fn
 from feeluown.gui.provider_ui import UISupportsLoginOrGoHome, ProviderUiItem, \
     UISupportsLoginEvent
-from feeluown.gui.widgets import SelfPaintAbstractSquareButton
-from feeluown.gui.drawers import PixmapDrawer, AvatarIconDrawer
+from feeluown.gui.widgets import SelfPaintAbstractIconTextButton
+from feeluown.gui.drawers import SizedPixmapDrawer, AvatarIconDrawer
+from feeluown.gui.helpers import painter_save
 
 if TYPE_CHECKING:
     from feeluown.app.gui_app import GuiApp
 
 
-class Avatar(SelfPaintAbstractSquareButton):
+class Avatar(SelfPaintAbstractIconTextButton):
     """
     When no provider is selected, click this button will popup a menu,
     and let user select a provider. When a provider is selected, click this
     button will trigger `UISupportsLoginOrGoHome`. If the provider has
     a current user, this tries to show the user avatar.
     """
 
     def __init__(self, app: 'GuiApp', *args, **kwargs):
-        super().__init__(*args, **kwargs)
+        super().__init__('未登录', *args, **kwargs)
 
         self._app = app
         self._avatar_drawer = None
-        self._icon_drawer = AvatarIconDrawer(self.width(), self._padding)
+        # In order to make the avatar/icon align to the left edge,
+        # translate the painter to -self._padding and set different padding
+        # for avatar-icon and avatar-image.
+        self._avatar_padding = self._padding // 2
+        # Leave 1px to draw line itself.
+        # Theoretically, the line itself costs 1.5px and only 0.75px is needed.
+        self._translate_x = 1 - self._padding
+        self._avatar_translate_x = -self._avatar_padding
+        self._icon_drawer = AvatarIconDrawer(self.height(), self._padding)
         self.clicked.connect(self.on_clicked)
         self.setToolTip('点击登陆资源提供方')
 
     def on_clicked(self):
         pvd_ui = self._app.current_pvd_ui_mgr.get()
         if pvd_ui is not None:
             if isinstance(pvd_ui, UISupportsLoginOrGoHome):
@@ -112,36 +122,49 @@
         provider = self._app.library.get(source)
         assert provider is not None
         user = None
         if isinstance(provider, SupportsCurrentUser):
             user = await run_fn(provider.get_current_user_or_none)
 
         if user is None:
+            self._text = '未登录'
             return None
         if isinstance(user, UserModel) and user.avatar_url:
+            self._text = user.name
             img_data = await run_afn(self._app.img_mgr.get, user.avatar_url,
                                      reverse(user))
             if img_data:
-                self._avatar_drawer = PixmapDrawer.from_img_data(img_data,
-                                                                 self,
-                                                                 radius=0.5)
+                p = self._avatar_padding
+                w = self.height() - 2 * p
+                rect = QRect(p, p, w, w)
+                self._avatar_drawer = SizedPixmapDrawer.from_img_data(
+                    img_data, rect, radius=0.5)
         return user
 
-    def paintEvent(self, _):
-        painter = QPainter(self)
-        painter.setRenderHint(QPainter.Antialiasing)
-        self.paint_round_bg_when_hover(painter)
+    def paint_border_bg_when_hover(self, *_, **__):
+        pass
 
+    def draw_text(self, painter):
+        with painter_save(painter):
+            if not self._avatar_drawer:
+                painter.translate(self._translate_x, 0)
+            super().draw_text(painter)
+
+    def draw_icon(self, painter: QPainter):
         if self._avatar_drawer:
-            self._avatar_drawer.draw(painter)
+            with painter_save(painter):
+                painter.translate(self._avatar_translate_x, 0)
+                self._avatar_drawer.draw(painter)
         else:
-            # If a provider is selected, draw a highlight circle.
-            if self._app.current_pvd_ui_mgr.get_either() is not None:
-                self._icon_drawer.fg_color = self.palette().color(QPalette.Highlight)
-            self._icon_drawer.draw(painter)
+            with painter_save(painter):
+                painter.translate(self._translate_x, 0)
+                # If a provider is selected, draw a highlight circle.
+                if self._app.current_pvd_ui_mgr.get_either() is not None:
+                    self._icon_drawer.fg_color = self.palette().color(QPalette.Highlight)
+                self._icon_drawer.draw(painter)
 
 
 if __name__ == '__main__':
     from unittest.mock import MagicMock
     from feeluown.gui.debug import simple_layout, mock_app
 
     length = 400
@@ -157,8 +180,8 @@
             ProviderUiItem(
                 '',
                 'Hello PyQt5',
                 '',
                 'Hello PyQt5',
             )
         ])
-        layout.addWidget(Avatar(mockapp, length=length))
+        layout.addWidget(Avatar(mockapp, height=length))
```

### Comparing `feeluown-4.1.3/feeluown/gui/components/btns.py` & `feeluown-4.1.4/feeluown/gui/components/btns.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/components/collections.py` & `feeluown-4.1.4/feeluown/gui/components/collections.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/components/line_song.py` & `feeluown-4.1.4/feeluown/gui/components/line_song.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/components/menu.py` & `feeluown-4.1.4/feeluown/gui/components/menu.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/components/nowplaying.py` & `feeluown-4.1.4/feeluown/gui/components/nowplaying.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/components/player_playlist.py` & `feeluown-4.1.4/feeluown/gui/components/player_playlist.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/components/player_progress.py` & `feeluown-4.1.4/feeluown/gui/components/player_progress.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/components/playlist_btn.py` & `feeluown-4.1.4/feeluown/gui/components/playlist_btn.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/consts.py` & `feeluown-4.1.4/feeluown/gui/consts.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/debug.py` & `feeluown-4.1.4/feeluown/gui/debug.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/drawers.py` & `feeluown-4.1.4/feeluown/gui/drawers.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,110 +4,132 @@
 from PyQt5.QtCore import Qt, QRect, QPoint, QPointF
 from PyQt5.QtGui import QPainter, QBrush, QPixmap, QImage, QColor, QPolygonF, QPalette
 from PyQt5.QtWidgets import QWidget
 
 from feeluown.gui.helpers import random_solarized_color, painter_save
 
 
-class PixmapDrawer:
-    """Draw pixmap on a widget with radius.
-
-    The pixmap will be scaled to the width of the widget.
-    """
-    def __init__(self, img, widget: QWidget, radius: int = 0):
+class SizedPixmapDrawer:
+    def __init__(self, img, rect: QRect, radius: int = 0):
         """
         :param widget: a object which has width() and height() method.
         """
-        self._widget_last_width = widget.width()
-        self._widget = widget
+        self._rect = rect
+        self._img_old_width = rect.width()
         self._radius = radius
 
         if img is None:
             self._color = random_solarized_color()
             self._img = None
             self._pixmap = None
         else:
             self._img = img
             self._color = None
-            new_img = img.scaledToWidth(self._widget_last_width, Qt.SmoothTransformation)
+            new_img = img.scaledToWidth(self._img_old_width, Qt.SmoothTransformation)
             self._pixmap = QPixmap(new_img)
 
+    def get_radius(self):
+        return self._radius if self._radius >= 1 else \
+            self.get_rect().width() * self._radius
+
+    def get_rect(self):
+        return self._rect
+
+    def maybe_update_pixmap(self):
+        pass
+
     @classmethod
     def from_img_data(cls, img_data, *args, **kwargs):
         img = QImage()
         img.loadFromData(img_data)
         return cls(img, *args, **kwargs)
 
     def get_img(self) -> Optional[QImage]:
         return self._img
 
     def get_pixmap(self) -> Optional[QPixmap]:
         return self._pixmap
 
-    def maybe_update_pixmap(self):
-        if self._widget.width() != self._widget_last_width:
-            self._widget_last_width = self._widget.width()
-            assert self._img is not None
-            new_img = self._img.scaledToWidth(self._widget_last_width,
-                                              Qt.SmoothTransformation)
-            self._pixmap = QPixmap(new_img)
-
-    def draw(self, painter):
+    def draw(self, painter: QPainter):
         painter.save()
         painter.setRenderHint(QPainter.Antialiasing)
         painter.setRenderHint(QPainter.SmoothPixmapTransform)
         if self._pixmap is None:
             self._draw_random_color(painter)
         else:
             self._draw_pixmap(painter)
         painter.restore()
 
-    def _get_radius(self):
-        return self._radius if self._radius >= 1 else self._widget.width() * self._radius
-
     def _draw_random_color(self, painter: QPainter):
         brush = QBrush(self._color)
         painter.setBrush(brush)
         painter.setPen(Qt.NoPen)
-        rect = self._widget.rect()
-        if self._radius == 0:
+        rect = self.get_rect()
+        radius = self.get_radius()
+        if radius == 0:
             painter.drawRect(rect)
         else:
-            radius = self._get_radius()
             painter.drawRoundedRect(rect, radius, radius)
 
     def _draw_pixmap(self, painter: QPainter):
         assert self._pixmap is not None
 
         self.maybe_update_pixmap()
         brush = QBrush(self._pixmap)
         painter.setBrush(brush)
         painter.setPen(Qt.NoPen)
-        radius = self._radius
+        radius = self.get_radius()
         size = self._pixmap.size()
-        y = (size.height() - self._widget.height()) // 2
+        target_rect = self.get_rect()
+        y = (size.height() - target_rect.height()) // 2
         painter.save()
+        painter.translate(target_rect.x(), target_rect.y())
         painter.translate(0, -y)
-        rect = QRect(0, 0, self._widget.width(), size.height())
+        rect = QRect(0, 0, target_rect.width(), size.height())
         if radius == 0:
             painter.drawRect(rect)
         else:
-            radius = radius if self._radius >= 1 else self._widget.width() * self._radius
             painter.drawRoundedRect(rect, radius, radius)
         painter.restore()
 
 
+class PixmapDrawer(SizedPixmapDrawer):
+    """Draw pixmap on a widget with radius.
+
+    The pixmap will be scaled to the width of the widget.
+
+    TODO: rename this drawer to WidgetPixmapDrawer?
+    """
+    def __init__(self, img, widget: QWidget, radius: int = 0):
+        """
+        :param widget: a object which has width() and height() method.
+        """
+        super().__init__(img, widget.rect(), radius)
+        self._widget = widget
+
+    def get_rect(self):
+        return self._widget.rect()
+
+    def maybe_update_pixmap(self):
+        if self._widget.width() != self._img_old_width:
+            self._img_old_width = self._widget.width()
+            assert self._img is not None
+            new_img = self._img.scaledToWidth(self._img_old_width,
+                                              Qt.SmoothTransformation)
+            self._pixmap = QPixmap(new_img)
+
+
 class AvatarIconDrawer:
     def __init__(self, length, padding, fg_color=None):
         self._length = length
         self._padding = padding
 
         self.fg_color = fg_color
 
-    def draw(self, painter):
+    def draw(self, painter: QPainter):
         pen = painter.pen()
         pen.setWidthF(1.5)
         painter.setPen(pen)
 
         if self.fg_color:
             painter.setPen(QColor(self.fg_color))
```

### Comparing `feeluown-4.1.3/feeluown/gui/helpers.py` & `feeluown-4.1.4/feeluown/gui/helpers.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/hotkey.py` & `feeluown-4.1.4/feeluown/gui/hotkey.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/image.py` & `feeluown-4.1.4/feeluown/gui/image.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/mimedata.py` & `feeluown-4.1.4/feeluown/gui/mimedata.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/page_containers/scroll_area.py` & `feeluown-4.1.4/feeluown/gui/page_containers/scroll_area.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/page_containers/table.py` & `feeluown-4.1.4/feeluown/gui/page_containers/table.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/pages/coll_mixed.py` & `feeluown-4.1.4/feeluown/gui/pages/coll_mixed.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/pages/homepage.py` & `feeluown-4.1.4/feeluown/gui/pages/recommendation.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,143 +1,97 @@
-import logging
 from typing import TYPE_CHECKING
 
-from PyQt5.QtWidgets import QWidget, QVBoxLayout
+from PyQt5.QtWidgets import QWidget, QVBoxLayout, QHBoxLayout
+from feeluown.library.provider_protocol import SupportsToplist
 
-from feeluown.library import SupportsRecListDailyPlaylists, SupportsRecACollectionOfSongs
 from feeluown.utils.reader import create_reader
-from feeluown.utils.aio import run_fn, as_completed
-from feeluown.gui.widgets.header import LargeHeader
+from feeluown.utils.aio import run_fn
+from feeluown.gui.widgets.header import LargeHeader, MidHeader
 from feeluown.gui.widgets.img_card_list import (
-    PlaylistCardListView,
-    PlaylistCardListModel,
-    PlaylistFilterProxyModel,
+    PlaylistCardListView, PlaylistCardListModel, PlaylistFilterProxyModel,
     PlaylistCardListDelegate,
 )
-from feeluown.gui.widgets.song_minicard_list import (
-    SongMiniCardListView,
-    SongMiniCardListDelegate,
-    SongMiniCardListModel,
-)
-from feeluown.gui.page_containers.scroll_area import ScrollArea
-from feeluown.gui.helpers import fetch_cover_wrapper, BgTransparentMixin
+
+from feeluown.library import SupportsRecListDailyPlaylists, SupportsRecListDailySongs
+
+from feeluown.gui.widgets import CalendarButton, RankButton
+from feeluown.gui.helpers import fetch_cover_wrapper
+
 
 if TYPE_CHECKING:
     from feeluown.app.gui_app import GuiApp
 
-logger = logging.getLogger(__name__)
-
 
 async def render(req, **kwargs):
     app: 'GuiApp' = req.ctx['app']
 
     view = View(app)
-    scroll_area = ScrollArea()
-    scroll_area.setWidget(view)
-    app.ui.right_panel.set_body(scroll_area)
+    app.ui.right_panel.set_body(view)
     await view.render()
 
 
-class View(QWidget, BgTransparentMixin):
-
+class View(QWidget):
     def __init__(self, app: 'GuiApp'):
         super().__init__(parent=None)
         self._app = app
 
-        self.header_playlist_list = LargeHeader('一些歌单')
-        self.header_songs_list = LargeHeader('随便听听')
-        self.playlist_list_view = PlaylistCardListView(no_scroll_v=True)
+        self.header_title = LargeHeader()
+        self.header_playlist_list = MidHeader()
+        self.playlist_list_view = PlaylistCardListView(fixed_row_count=1)
         self.playlist_list_view.setItemDelegate(
-            PlaylistCardListDelegate(
-                self.playlist_list_view,
-                card_min_width=150,
-            )
-        )
-        self.songs_list_view = SongMiniCardListView(no_scroll_v=True)
-        self.songs_list_view.setItemDelegate(
-            SongMiniCardListDelegate(self.songs_list_view, )
-        )
+            PlaylistCardListDelegate(self.playlist_list_view,
+                                     card_min_width=100,))
+        self.daily_songs_btn = CalendarButton('每日推荐', parent=self)
+        self.rank_btn = RankButton(parent=self)
+        self.daily_songs_btn.setMinimumWidth(150)
+        self.rank_btn.setMinimumWidth(150)
+
+        self.header_title.setText('发现音乐')
+        self.header_playlist_list.setText('个性化推荐')
 
         self._layout = QVBoxLayout(self)
         self._setup_ui()
 
         self.playlist_list_view.show_playlist_needed.connect(
-            lambda model: self._app.browser.goto(model=model)
-        )
-        self.songs_list_view.play_song_needed.connect(self._app.playlist.play_model)
+            lambda model: self._app.browser.goto(model=model))
+        self.daily_songs_btn.clicked.connect(
+            lambda: self._app.browser.goto(page='/rec/daily_songs'))
+        self.rank_btn.clicked.connect(
+            lambda: self._app.browser.goto(page='/toplist'))
 
     def _setup_ui(self):
+        self._h_layout = QHBoxLayout()
+        self._h_layout.addWidget(self.daily_songs_btn)
+        self._h_layout.addSpacing(10)
+        self._h_layout.addWidget(self.rank_btn)
+        self._h_layout.addStretch(0)
+
         self._layout.setContentsMargins(20, 10, 20, 0)
         self._layout.setSpacing(0)
+        self._layout.addWidget(self.header_title)
+        self._layout.addSpacing(10)
+        self._layout.addLayout(self._h_layout)
+        self._layout.addSpacing(30)
         self._layout.addWidget(self.header_playlist_list)
         self._layout.addSpacing(10)
         self._layout.addWidget(self.playlist_list_view)
-        self._layout.addSpacing(10)
-        self._layout.addWidget(self.header_songs_list)
-        self._layout.addSpacing(10)
-        self._layout.addWidget(self.songs_list_view)
         self._layout.addStretch(0)
 
-    async def _get_daily_playlists(self):
-        providers = self._app.library.list()
-        playlists_list = []
-        for coro in as_completed([
-            run_fn(provider.rec_list_daily_playlists) for provider in providers
-            if isinstance(provider, SupportsRecListDailyPlaylists)
-        ]):
-            try:
-                playlists_ = await coro
-            except:  # noqa
-                logger.exception('get recommended daily playlists failed')
-            else:
-                playlists_list.append(playlists_)
-
-        playlists = []
-        finished = [False] * len(playlists_list)
-        while True:
-            for i, playlists_ in enumerate(playlists_list):
-                try:
-                    playlist = playlists_.pop(0)
-                except IndexError:
-                    finished[i] = True
-                else:
-                    playlists.append(playlist)
-            if all(finished):
-                break
-        return playlists
-
-    async def _get_rec_songs(self):
-        providers = self._app.library.list()
-        titles = []
-        songs = []
-        for coro in as_completed([
-            run_fn(provider.rec_a_collection) for provider in providers
-            if isinstance(provider, SupportsRecACollectionOfSongs)
-        ]):
-            try:
-                title, songs_ = await coro
-            except:  # noqa
-                logger.exception('get rec songs failed')
-            else:
-                songs.extend(songs_)
-                titles.append(title)
-        return titles, songs
-
     async def render(self):
-        playlists = await self._get_daily_playlists()
-        model = PlaylistCardListModel(
-            create_reader(playlists), fetch_cover_wrapper(self._app),
-            {p.identifier: p.name
-             for p in self._app.library.list()}
-        )
-        filter_model = PlaylistFilterProxyModel()
-        filter_model.setSourceModel(model)
-        self.playlist_list_view.setModel(filter_model)
-
-        titles, songs = await self._get_rec_songs()
-        songs_model = SongMiniCardListModel(
-            create_reader(songs),
-            fetch_image=fetch_cover_wrapper(self._app),
-        )
-        self.songs_list_view.setModel(songs_model)
-        if titles:
-            self.header_songs_list.setText(titles[0])
+        pvd_ui = self._app.current_pvd_ui_mgr.get()
+        if pvd_ui is None:
+            self._app.show_msg('wtf!')
+            return
+
+        provider = pvd_ui.provider
+        if isinstance(provider, SupportsRecListDailyPlaylists):
+            playlists = await run_fn(provider.rec_list_daily_playlists)
+            model = PlaylistCardListModel(
+                create_reader(playlists),
+                fetch_cover_wrapper(self._app),
+                {p.identifier: p.name for p in self._app.library.list()})
+            filter_model = PlaylistFilterProxyModel()
+            filter_model.setSourceModel(model)
+            self.playlist_list_view.setModel(filter_model)
+
+        self.daily_songs_btn.setEnabled(isinstance(provider, SupportsRecListDailySongs))
+        self.rank_btn.setEnabled(isinstance(provider, SupportsToplist))
```

### Comparing `feeluown-4.1.3/feeluown/gui/pages/model.py` & `feeluown-4.1.4/feeluown/gui/pages/model.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/pages/my_fav.py` & `feeluown-4.1.4/feeluown/gui/pages/my_fav.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/pages/provider_home.py` & `feeluown-4.1.4/feeluown/gui/pages/provider_home.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/pages/recently_played.py` & `feeluown-4.1.4/feeluown/gui/pages/recently_played.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/pages/recommendation.py` & `feeluown-4.1.4/feeluown/gui/ui.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,98 +1,94 @@
-from typing import TYPE_CHECKING
+import logging
+from PyQt5.QtWidgets import QSizePolicy, QSplitter, QVBoxLayout
 
-from PyQt5.QtWidgets import QWidget, QVBoxLayout, QHBoxLayout
+from feeluown.gui.widgets.separator import Separator
+from feeluown.gui.widgets.settings import SettingsDialog
+from feeluown.gui.widgets.messageline import MessageLine
+from feeluown.gui.widgets.mpv_ import MpvOpenGLWidget
 
-from feeluown.utils.reader import create_reader
-from feeluown.utils.aio import run_fn
-from feeluown.gui.widgets.header import LargeHeader, MidHeader
-from feeluown.gui.widgets.img_card_list import (
-    PlaylistCardListView, PlaylistCardListModel, PlaylistFilterProxyModel,
-    PlaylistCardListDelegate,
-)
+from feeluown.gui.uimain.lyric import LyricWindow
+from feeluown.gui.uimain.sidebar import LeftPanel
+from feeluown.gui.uimain.page_view import RightPanel
+from feeluown.gui.uimain.player_bar import TopPanel
+from feeluown.gui.uimain.playlist_overlay import PlaylistOverlay
+from feeluown.gui.uimain.nowplaying_overlay import NowplayingOverlay
 
-from feeluown.library import SupportsRecListDailyPlaylists, SupportsRecListDailySongs
+logger = logging.getLogger(__name__)
 
-from feeluown.gui.widgets import CalendarButton, RankButton
-from feeluown.gui.helpers import fetch_cover_wrapper
 
+class Ui:
 
-if TYPE_CHECKING:
-    from feeluown.app.gui_app import GuiApp
-
-
-async def render(req, **kwargs):
-    app: 'GuiApp' = req.ctx['app']
-
-    view = View(app)
-    app.ui.right_panel.set_body(view)
-    await view.render()
-
-
-class View(QWidget):
-    def __init__(self, app: 'GuiApp'):
-        super().__init__(parent=None)
+    def __init__(self, app):
         self._app = app
+        # Let the following widgets access ui object during init.
+        self._app.ui = self
+        self._layout = QVBoxLayout(app)
+        self._top_separator = Separator(app)
+        self._splitter = QSplitter(app)
+
+        # Create widgets that don't rely on other widgets first.
+        self.lyric_window = LyricWindow(self._app)
+        self.lyric_window.hide()
+
+        # NOTE: 以位置命名的部件应该只用来组织界面布局，不要
+        # 给其添加任何功能性的函数
+        self._message_line = MessageLine()
+        self.top_panel = TopPanel(app, app)
+        self.sidebar = self._left_panel_con = LeftPanel(self._app)
+        self.left_panel = self._left_panel_con.p
+        self.page_view = self.right_panel = RightPanel(self._app, self._splitter)
+        self.toolbar = self.bottom_panel = self.right_panel.bottom_panel
+        self.mpv_widget = MpvOpenGLWidget(self._app)
+        self.playlist_overlay = PlaylistOverlay(app, parent=app)
+        self.nowplaying_overlay = NowplayingOverlay(app, parent=app)
+
+        # alias
+        self.magicbox = self.bottom_panel.magicbox
+        self.player_bar = self.pc_panel = self.top_panel.pc_panel
+        self.table_container = self.right_panel.table_container
+        # backward compatible, old name is songs_table_container
+        self.songs_table_container = self.table_container
+        self.songs_table = self.table_container.songs_table
+        self.back_btn = self.bottom_panel.back_btn
+        self.forward_btn = self.bottom_panel.forward_btn
 
-        self.header_title = LargeHeader()
-        self.header_playlist_list = MidHeader()
-        self.playlist_list_view = PlaylistCardListView(fixed_row_count=1)
-        self.playlist_list_view.setItemDelegate(
-            PlaylistCardListDelegate(self.playlist_list_view,
-                                     card_min_width=100,))
-        self.daily_songs_btn = CalendarButton('每日推荐', parent=self)
-        self.rank_btn = RankButton(parent=self)
-        self.daily_songs_btn.setMinimumWidth(150)
-        self.rank_btn.setMinimumWidth(150)
-
-        self.header_title.setText('发现音乐')
-        self.header_playlist_list.setText('个性化推荐')
-        self.rank_btn.setDisabled(True)
-        self.rank_btn.setToolTip('未实现，欢迎 PR！')
+        self.toolbar.settings_btn.clicked.connect(self._open_settings_dialog)
 
-        self._layout = QVBoxLayout(self)
         self._setup_ui()
 
-        self.playlist_list_view.show_playlist_needed.connect(
-            lambda model: self._app.browser.goto(model=model))
-        self.daily_songs_btn.clicked.connect(
-            lambda: self._app.browser.goto(page='/rec/daily_songs'))
-        self.rank_btn.clicked.connect(
-            lambda: self._app.show_msg('未实现，欢迎 PR！'))
-
     def _setup_ui(self):
-        self._h_layout = QHBoxLayout()
-        self._h_layout.addWidget(self.daily_songs_btn)
-        self._h_layout.addSpacing(10)
-        self._h_layout.addWidget(self.rank_btn)
-        self._h_layout.addStretch(0)
+        self._app.setSizePolicy(QSizePolicy.Preferred, QSizePolicy.Preferred)
 
-        self._layout.setContentsMargins(20, 10, 20, 0)
-        self._layout.setSpacing(0)
-        self._layout.addWidget(self.header_title)
-        self._layout.addSpacing(10)
-        self._layout.addLayout(self._h_layout)
-        self._layout.addSpacing(30)
-        self._layout.addWidget(self.header_playlist_list)
-        self._layout.addSpacing(10)
-        self._layout.addWidget(self.playlist_list_view)
-        self._layout.addStretch(0)
-
-    async def render(self):
-        pvd_ui = self._app.current_pvd_ui_mgr.get()
-        if pvd_ui is None:
-            self._app.show_msg('wtf!')
-            return
-
-        provider = pvd_ui.provider
-        if isinstance(provider, SupportsRecListDailyPlaylists):
-            playlists = await run_fn(provider.rec_list_daily_playlists)
-            model = PlaylistCardListModel(
-                create_reader(playlists),
-                fetch_cover_wrapper(self._app),
-                {p.identifier: p.name for p in self._app.library.list()})
-            filter_model = PlaylistFilterProxyModel()
-            filter_model.setSourceModel(model)
-            self.playlist_list_view.setModel(filter_model)
+        self._splitter.setHandleWidth(0)
+        self._splitter.addWidget(self._left_panel_con)
+        self._splitter.addWidget(self.right_panel)
+        self._message_line.hide()
+        self.playlist_overlay.hide()
+        self.nowplaying_overlay.hide()
+
+        self.right_panel.setSizePolicy(QSizePolicy.Expanding, QSizePolicy.Expanding)
+
+        self._layout.addWidget(self._splitter)
+        self._layout.addWidget(self.mpv_widget)
+        self._layout.addWidget(self._message_line)
+        self._layout.addWidget(self._top_separator)
+        self._layout.addWidget(self.top_panel)
 
-        if not isinstance(provider, SupportsRecListDailySongs):
-            self.daily_songs_btn.setDisabled(True)
+        self._layout.setSpacing(0)
+        self._layout.setContentsMargins(0, 0, 0, 0)
+        self.top_panel.layout().setSpacing(0)
+        self.top_panel.layout().setContentsMargins(0, 0, 0, 0)
+
+        self._app.resize(960, 600)
+
+    def _open_settings_dialog(self):
+        dialog = SettingsDialog(self._app, self._app)
+        dialog.exec()
+
+    def toggle_player_bar(self):
+        if self.top_panel.isVisible():
+            self.top_panel.hide()
+            self._top_separator.hide()
+        else:
+            self.top_panel.show()
+            self._top_separator.show()
```

### Comparing `feeluown-4.1.3/feeluown/gui/pages/recommendation_daily_songs.py` & `feeluown-4.1.4/feeluown/gui/pages/recommendation_daily_songs.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/pages/search.py` & `feeluown-4.1.4/feeluown/gui/pages/search.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/pages/song_explore.py` & `feeluown-4.1.4/feeluown/gui/pages/song_explore.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/provider_ui.py` & `feeluown-4.1.4/feeluown/gui/provider_ui.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/theme.py` & `feeluown-4.1.4/feeluown/gui/theme.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/tips.py` & `feeluown-4.1.4/feeluown/gui/tips.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/tray.py` & `feeluown-4.1.4/feeluown/gui/tray.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/ui.py` & `feeluown-4.1.4/feeluown/gui/widgets/settings.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,94 +1,94 @@
-import logging
-from PyQt5.QtWidgets import QSizePolicy, QSplitter, QVBoxLayout
+from PyQt5.QtCore import pyqtSignal
+from PyQt5.QtWidgets import QDialog, QWidget, QCheckBox, \
+    QVBoxLayout, QHBoxLayout
+
+from feeluown.gui.widgets.magicbox import KeySourceIn
+from feeluown.gui.widgets.header import MidHeader
+from feeluown.gui.components import LyricButton, WatchButton
+
+
+class _ProviderCheckBox(QCheckBox):
+    def set_identifier(self, identifier):
+        self.identifier = identifier  # pylint: disable=W0201
+
+
+class SearchProvidersFilter(QWidget):
+    checked_btn_changed = pyqtSignal(list)
+
+    def __init__(self, providers):
+        super().__init__()
+        self.providers = providers
+
+        self._btns = []
+        self._layout = QHBoxLayout(self)
+
+        for provider in self.providers:
+            btn = _ProviderCheckBox(provider.name, self)
+            btn.set_identifier(provider.identifier)
+            btn.clicked.connect(self.on_btn_clicked)
+            self._layout.addWidget(btn)
+            self._btns.append(btn)
+
+        # HELP: we add spacing between checkboxes because they
+        # will overlay each other on macOS by default. Why?
+        self._layout.setSpacing(10)
+        self._layout.addStretch(0)
+
+    def get_checked_providers(self):
+        identifiers = []
+        for btn in self._btns:
+            if btn.isChecked():
+                identifiers.append(btn.identifier)
+        return identifiers
+
+    def set_checked_providers(self, providers):
+        for provider in providers:
+            for btn in self._btns:
+                if provider == btn.identifier:
+                    btn.setChecked(True)
+                    break
+
+    def on_btn_clicked(self, _):
+        self.checked_btn_changed.emit(self.get_checked_providers())
+
+
+class PlayerSettings(QWidget):
+    def __init__(self, app, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
-from feeluown.gui.widgets.separator import Separator
-from feeluown.gui.widgets.settings import SettingsDialog
-from feeluown.gui.widgets.messageline import MessageLine
-from feeluown.gui.widgets.mpv_ import MpvOpenGLWidget
-
-from feeluown.gui.uimain.lyric import LyricWindow
-from feeluown.gui.uimain.sidebar import LeftPanel
-from feeluown.gui.uimain.page_view import RightPanel
-from feeluown.gui.uimain.player_bar import TopPanel
-from feeluown.gui.uimain.playlist_overlay import PlaylistOverlay
-from feeluown.gui.uimain.nowplaying_overlay import NowplayingOverlay
+        self._app = app
+        self.lyric_btn = LyricButton(app, height=16)
+        self.watch_btn = WatchButton(app, height=16)
+        self._layout = QHBoxLayout(self)
+        self._layout.addWidget(self.lyric_btn)
+        self._layout.addWidget(self.watch_btn)
+        self._layout.addStretch(0)
 
-logger = logging.getLogger(__name__)
 
+class SettingsDialog(QDialog):
+    def __init__(self, app, parent=None):
+        super().__init__(parent=parent)
+        self._app = app
 
-class Ui:
+        self.setWindowTitle('应用配置')
+        self.render()
 
-    def __init__(self, app):
-        self._app = app
-        # Let the following widgets access ui object during init.
-        self._app.ui = self
-        self._layout = QVBoxLayout(app)
-        self._top_separator = Separator(app)
-        self._splitter = QSplitter(app)
-
-        # Create widgets that don't rely on other widgets first.
-        self.lyric_window = LyricWindow(self._app)
-        self.lyric_window.hide()
-
-        # NOTE: 以位置命名的部件应该只用来组织界面布局，不要
-        # 给其添加任何功能性的函数
-        self._message_line = MessageLine()
-        self.top_panel = TopPanel(app, app)
-        self.sidebar = self._left_panel_con = LeftPanel(self._app)
-        self.left_panel = self._left_panel_con.p
-        self.page_view = self.right_panel = RightPanel(self._app, self._splitter)
-        self.toolbar = self.bottom_panel = self.right_panel.bottom_panel
-        self.mpv_widget = MpvOpenGLWidget(self._app)
-        self.playlist_overlay = PlaylistOverlay(app, parent=app)
-        self.nowplaying_overlay = NowplayingOverlay(app, parent=app)
-
-        # alias
-        self.magicbox = self.bottom_panel.magicbox
-        self.player_bar = self.pc_panel = self.top_panel.pc_panel
-        self.table_container = self.right_panel.table_container
-        # backward compatible, old name is songs_table_container
-        self.songs_table_container = self.table_container
-        self.songs_table = self.table_container.songs_table
-        self.back_btn = self.bottom_panel.back_btn
-        self.forward_btn = self.bottom_panel.forward_btn
-
-        self.toolbar.settings_btn.clicked.connect(self._open_settings_dialog)
-
-        self._setup_ui()
-
-    def _setup_ui(self):
-        self._app.setSizePolicy(QSizePolicy.Preferred, QSizePolicy.Preferred)
-
-        self._splitter.setHandleWidth(0)
-        self._splitter.addWidget(self._left_panel_con)
-        self._splitter.addWidget(self.right_panel)
-        self._message_line.hide()
-        self.playlist_overlay.hide()
-        self.nowplaying_overlay.hide()
-
-        self.right_panel.setSizePolicy(QSizePolicy.Expanding, QSizePolicy.Expanding)
-
-        self._layout.addWidget(self._splitter)
-        self._layout.addWidget(self.mpv_widget)
-        self._layout.addWidget(self._message_line)
-        self._layout.addWidget(self._top_separator)
-        self._layout.addWidget(self.top_panel)
-
-        self._layout.setSpacing(0)
-        self._layout.setContentsMargins(0, 0, 0, 0)
-        self.top_panel.layout().setSpacing(0)
-        self.top_panel.layout().setContentsMargins(0, 0, 0, 0)
-
-        self._app.resize(960, 600)
-
-    def _open_settings_dialog(self):
-        dialog = SettingsDialog(self._app, self._app)
-        dialog.exec()
-
-    def toggle_player_bar(self):
-        if self.top_panel.isVisible():
-            self.top_panel.hide()
-            self._top_separator.hide()
+    def render(self):
+        source_in_str = self._app.browser.local_storage.get(KeySourceIn)
+        if source_in_str is not None:
+            source_in = source_in_str.split(',')
         else:
-            self.top_panel.show()
-            self._top_separator.show()
+            source_in = [p.identifier for p in self._app.library.list()]
+        toolbar = SearchProvidersFilter(self._app.library.list())
+        toolbar.set_checked_providers(source_in)
+        toolbar.checked_btn_changed.connect(self.update_source_in)
+
+        self._layout = QVBoxLayout(self)
+        self._layout.addWidget(MidHeader('搜索来源'))
+        self._layout.addWidget(toolbar)
+        self._layout.addWidget(MidHeader('播放器'))
+        self._layout.addWidget(PlayerSettings(self._app))
+        self._layout.addStretch(0)
+
+    def update_source_in(self, source_in):
+        self._app.browser.local_storage[KeySourceIn] = ','.join(source_in)
```

### Comparing `feeluown-4.1.3/feeluown/gui/uimain/floating_box.py` & `feeluown-4.1.4/feeluown/gui/uimain/floating_box.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/uimain/lyric.py` & `feeluown-4.1.4/feeluown/gui/uimain/lyric.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/uimain/nowplaying_overlay.py` & `feeluown-4.1.4/feeluown/gui/uimain/nowplaying_overlay.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/uimain/page_view.py` & `feeluown-4.1.4/feeluown/gui/uimain/page_view.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/uimain/player_bar.py` & `feeluown-4.1.4/feeluown/gui/uimain/player_bar.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/uimain/playlist_overlay.py` & `feeluown-4.1.4/feeluown/gui/uimain/playlist_overlay.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/uimain/sidebar.py` & `feeluown-4.1.4/feeluown/gui/uimain/sidebar.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,24 +11,24 @@
     SupportsPlaylistCreateByName,
     SupportsCurrentUser,
 )
 from feeluown.collection import CollectionAlreadyExists, CollectionType
 from feeluown.utils import aio
 from feeluown.utils.reader import create_reader
 from feeluown.utils.aio import run_fn
+from feeluown.gui.components import Avatar, CollectionListView
 from feeluown.gui.widgets import (
     DiscoveryButton,
     HomeButton,
     PlusButton,
     TriagleButton,
     StarButton,
 )
-
+from feeluown.gui.widgets.separator import Separator
 from feeluown.gui.widgets.playlists import PlaylistsView
-from feeluown.gui.components import CollectionListView
 from feeluown.gui.widgets.my_music import MyMusicView
 
 if TYPE_CHECKING:
     from feeluown.app.gui_app import GuiApp
 
 
 class ListViewContainer(QFrame):
@@ -117,14 +117,16 @@
     def __init__(self, app: 'GuiApp', parent=None):
         super().__init__(parent)
         self._app = app
 
         self.home_btn = HomeButton(height=30, parent=self)
         self.discovery_btn = DiscoveryButton(height=30, padding=0.2, parent=self)
         self.fav_btn = StarButton('我的收藏', height=30, parent=self)
+        self.fold_top_btn = TriagleButton(length=14, padding=0.2)
+        self.fold_top_btn.setCheckable(True)
         self.collections_header = QLabel('本地收藏集', self)
         self.collections_header.setToolTip('我们可以在本地建立『收藏集』来收藏自己喜欢的音乐资源\n\n'
                                            '每个收藏集都以一个独立 .fuo 文件的存在，'
                                            '将鼠标悬浮在收藏集上，可以查看文件所在路径。\n'
                                            '新建 fuo 文件，则可以新建收藏集，文件名即是收藏集的名字。\n\n'
                                            '手动编辑 fuo 文件即可编辑收藏集中的音乐资源，也可以在界面上拖拽来增删歌曲。')
         self.playlists_header = QLabel('歌单列表', self)
@@ -139,44 +141,44 @@
         self.playlists_con = ListViewContainer(self.playlists_header,
                                                self.playlists_view)
         self.my_music_con = ListViewContainer(self.my_music_header, self.my_music_view)
 
         self.playlists_view.setModel(self._app.pl_uimgr.model)
         self.my_music_view.setModel(self._app.mymusic_uimgr.model)
 
+        self._top_separator = Separator(self._app)
         self._layout = QVBoxLayout(self)
-        self._sub_layout = QVBoxLayout()
-        self._top_layout = QVBoxLayout()
+        self._avatar_layout = QHBoxLayout()
 
         self._layout.setSpacing(0)
-        self._layout.setContentsMargins(0, 0, 0, 0)
-        self._layout.addLayout(self._top_layout)
-        self._layout.addLayout(self._sub_layout)
-
-        self._top_layout.setContentsMargins(15, 16, 16, 0)
-        self._top_layout.addWidget(self.home_btn)
-        self._top_layout.addWidget(self.discovery_btn)
-        self._top_layout.addWidget(self.fav_btn)
-        self._sub_layout.setContentsMargins(16, 8, 16, 0)
-        self._sub_layout.addWidget(self.collections_con)
-        self._sub_layout.addWidget(self.my_music_con)
-        self._sub_layout.addWidget(self.playlists_con)
+        self._layout.setContentsMargins(16, 10, 16, 0)
+        self._layout.addWidget(self.home_btn)
+        self._layout.addWidget(self.collections_con)
+        self._layout.addWidget(self._top_separator)
+        self._layout.addLayout(self._avatar_layout)
+        self._avatar_layout.addWidget(Avatar(self._app, height=48))
+        self._avatar_layout.addWidget(self.fold_top_btn)
+        self._layout.addWidget(self.discovery_btn)
+        self._layout.addWidget(self.fav_btn)
+        self._layout.addWidget(self.my_music_con)
+        self._layout.addWidget(self.playlists_con)
         self._layout.addStretch(0)
 
         self.playlists_view.setFrameShape(QFrame.NoFrame)
         self.my_music_view.setFrameShape(QFrame.NoFrame)
         self.collections_view.setFrameShape(QFrame.NoFrame)
         self.setFrameShape(QFrame.NoFrame)
         self.collections_con.create_btn.show()
         # 让各个音乐库来决定是否显示这些组件
         self.playlists_con.hide()
         self.my_music_con.hide()
         self.discovery_btn.setDisabled(True)
         self.fav_btn.setDisabled(True)
         self.discovery_btn.setToolTip('当前资源提供方未知')
+        self.fold_top_btn.setToolTip('折叠/打开“主页和本地收藏集”功能')
 
         if self._app.config.ENABLE_NEW_HOMEPAGE is True:
             self.home_btn.clicked.connect(
                 lambda: self._app.browser.goto(page='/homepage'))
         else:
             self.home_btn.clicked.connect(self.show_library)
 
@@ -192,14 +194,26 @@
         self.playlists_con.create_btn.clicked.connect(self._create_playlist)
         self._app.current_pvd_ui_mgr.changed.connect(
             self.on_current_pvd_ui_changed)
         self.discovery_btn.clicked.connect(
             lambda: self._app.browser.goto(page='/rec'))
         self.fav_btn.clicked.connect(
             lambda: self._app.browser.goto(page='/my_fav'))
+        self.fold_top_btn.clicked.connect(self._toggle_top_layout)
+
+    def _toggle_top_layout(self, checked):
+        widgets = [self._top_separator, self.collections_con, self.home_btn]
+        if checked:
+            self.fold_top_btn.set_direction('down')
+            for w in widgets:
+                w.hide()
+        else:
+            self.fold_top_btn.set_direction('up')
+            for w in widgets:
+                w.show()
 
     def popup_collection_adding_dialog(self):
         dialog = QDialog(self)
         # Set WA_DeleteOnClose so that the dialog can be deleted (from self.children).
         dialog.setAttribute(Qt.WA_DeleteOnClose)
         layout = QFormLayout(dialog)
         id_edit = QLineEdit(dialog)
```

### Comparing `feeluown-4.1.3/feeluown/gui/uimain/toolbar.py` & `feeluown-4.1.4/feeluown/gui/uimain/toolbar.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from typing import TYPE_CHECKING
 
 from PyQt5.QtCore import Qt
 from PyQt5.QtWidgets import QWidget, QPushButton, QHBoxLayout, QStackedWidget
 
-from feeluown.gui.components import Avatar
 from feeluown.gui.widgets import (
     LeftArrowButton,
     RightArrowButton,
     SearchSwitchButton,
     SettingsButton,
 )
 from feeluown.gui.widgets.magicbox import MagicBox
@@ -42,15 +41,14 @@
         self._stack_switch.setToolTip("显示搜索框")
         self._stack_switch.setCheckable(True)
         self._stacked_widget = QStackedWidget(self)
         self._stacked_widget.addWidget(self.magicbox)
         self._stack_switch.hide()
 
         self.status_line = StatusLine(self._app)
-        self.avatar = Avatar(app, length=ButtonSize[0])
         self.settings_btn = SettingsButton(length=ButtonSize[0])
 
         # initialize widgets
         self.back_btn.setEnabled(False)
         self.forward_btn.setEnabled(False)
 
         self.back_btn.clicked.connect(self._app.browser.back)
@@ -68,15 +66,14 @@
         self._layout.addWidget(self.forward_btn)
 
         self._layout.addSpacing(80)
         self._layout.addWidget(self._stacked_widget)
         self._layout.addWidget(self._stack_switch)
         self._layout.addSpacing(40)
         self._layout.addWidget(self.status_line)
-        self._layout.addWidget(self.avatar)
         self._layout.addWidget(self.settings_btn)
 
         # assume the magicbox height is about 30
         # h_margin = 20(TableContainer h_spacing) - 30*0.25(back_btn padding)
         h_margin, v_margin = 11, 7
         height = self.magicbox.height()
```

### Comparing `feeluown-4.1.3/feeluown/gui/uimodels/my_music.py` & `feeluown-4.1.4/feeluown/gui/uimodels/my_music.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/uimodels/playlist.py` & `feeluown-4.1.4/feeluown/gui/uimodels/playlist.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/watch.py` & `feeluown-4.1.4/feeluown/gui/watch.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/widgets/accordion.py` & `feeluown-4.1.4/feeluown/gui/widgets/accordion.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/widgets/comment_list.py` & `feeluown-4.1.4/feeluown/gui/widgets/comment_list.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/widgets/cover_label.py` & `feeluown-4.1.4/feeluown/gui/widgets/cover_label.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/widgets/frameless.py` & `feeluown-4.1.4/feeluown/gui/widgets/frameless.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/widgets/header.py` & `feeluown-4.1.4/feeluown/gui/widgets/header.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/widgets/img_card_list.py` & `feeluown-4.1.4/feeluown/gui/widgets/img_card_list.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/widgets/labels.py` & `feeluown-4.1.4/feeluown/gui/widgets/labels.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/widgets/login.py` & `feeluown-4.1.4/feeluown/gui/widgets/login.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/widgets/lyric.py` & `feeluown-4.1.4/feeluown/gui/widgets/lyric.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/widgets/magicbox.py` & `feeluown-4.1.4/feeluown/gui/widgets/magicbox.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/widgets/messageline.py` & `feeluown-4.1.4/feeluown/gui/widgets/messageline.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/widgets/meta.py` & `feeluown-4.1.4/feeluown/gui/widgets/meta.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/widgets/mpv_.py` & `feeluown-4.1.4/feeluown/gui/widgets/mpv_.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/widgets/my_music.py` & `feeluown-4.1.4/feeluown/gui/widgets/my_music.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/widgets/playlist_button.py` & `feeluown-4.1.4/feeluown/gui/widgets/playlist_button.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/widgets/playlists.py` & `feeluown-4.1.4/feeluown/gui/widgets/playlists.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/widgets/progress_slider.py` & `feeluown-4.1.4/feeluown/gui/widgets/progress_slider.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/widgets/provider.py` & `feeluown-4.1.4/feeluown/gui/widgets/provider.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/widgets/selfpaint_btn.py` & `feeluown-4.1.4/feeluown/gui/widgets/selfpaint_btn.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/widgets/separator.py` & `feeluown-4.1.4/feeluown/gui/widgets/separator.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/widgets/song_minicard_list.py` & `feeluown-4.1.4/feeluown/gui/widgets/song_minicard_list.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/widgets/songs.py` & `feeluown-4.1.4/feeluown/gui/widgets/songs.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/widgets/statusline.py` & `feeluown-4.1.4/feeluown/gui/widgets/statusline.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/widgets/statusline_items/notify.py` & `feeluown-4.1.4/feeluown/gui/widgets/statusline_items/notify.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/widgets/statusline_items/plugin.py` & `feeluown-4.1.4/feeluown/gui/widgets/statusline_items/plugin.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/widgets/tabbar.py` & `feeluown-4.1.4/feeluown/gui/widgets/tabbar.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/widgets/table_toolbar.py` & `feeluown-4.1.4/feeluown/gui/widgets/table_toolbar.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/widgets/textlist.py` & `feeluown-4.1.4/feeluown/gui/widgets/textlist.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/widgets/video.py` & `feeluown-4.1.4/feeluown/gui/widgets/video.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/widgets/volume_button.py` & `feeluown-4.1.4/feeluown/gui/widgets/volume_button.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/gui/widgets/weblogin.py` & `feeluown-4.1.4/feeluown/gui/widgets/weblogin.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/library/__init__.py` & `feeluown-4.1.4/feeluown/library/__init__.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/library/base.py` & `feeluown-4.1.4/feeluown/library/base.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/library/collection.py` & `feeluown-4.1.4/feeluown/library/collection.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/library/flags.py` & `feeluown-4.1.4/feeluown/library/flags.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/library/library.py` & `feeluown-4.1.4/feeluown/library/library.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/library/model_protocol.py` & `feeluown-4.1.4/feeluown/library/model_protocol.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/library/model_state.py` & `feeluown-4.1.4/feeluown/library/model_state.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/library/models.py` & `feeluown-4.1.4/feeluown/library/models.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/library/provider.py` & `feeluown-4.1.4/feeluown/library/provider.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/library/provider_protocol.py` & `feeluown-4.1.4/feeluown/library/provider_protocol.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import runtime_checkable, Protocol, List, Tuple, Optional, Dict
 from abc import abstractmethod
 from feeluown.media import Quality, Media
 from feeluown.excs import NoUserLoggedIn
 from .models import (
     BriefCommentModel, SongModel, VideoModel, AlbumModel, ArtistModel,
     PlaylistModel, UserModel, ModelType, BriefArtistModel, BriefSongModel,
-    LyricModel, BriefVideoModel,
+    LyricModel, BriefVideoModel, BriefPlaylistModel,
 )
 from .collection import Collection
 
 from .flags import Flags as PF
 
 
 ID = str
@@ -371,14 +371,30 @@
 @runtime_checkable
 class SupportsCurrentUserFavVideosReader(Protocol):
     @abstractmethod
     def current_user_fav_create_videos_rd(self):
         pass
 
 
+@runtime_checkable
+class SupportsToplist(Protocol):
+    @abstractmethod
+    def toplist_list(self) -> List[BriefPlaylistModel]:
+        """List all toplist(排行榜)."""
+
+    @abstractmethod
+    def toplist_get(self, toplist_id) -> PlaylistModel:
+        """Get toplist details.
+
+        For some providers, the toplist model(schema) may be different from the
+        PlaylistModel. They should think about a way to solve this. For example,
+        turn the identifier into `toplist_{id}` and do some hack in playlist_get API.
+        """
+
+
 #
 # Protocols for recommendation.
 #
 @runtime_checkable
 class SupportsRecListDailySongs(Protocol):
     @abstractmethod
     def rec_list_daily_songs(self) -> List[SongModel]:
```

### Comparing `feeluown-4.1.3/feeluown/library/uri.py` & `feeluown-4.1.4/feeluown/library/uri.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/local/__init__.py` & `feeluown-4.1.4/feeluown/local/__init__.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/local/db.py` & `feeluown-4.1.4/feeluown/local/db.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/local/provider.py` & `feeluown-4.1.4/feeluown/local/provider.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/local/provider_ui.py` & `feeluown-4.1.4/feeluown/local/provider_ui.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/local/schemas.py` & `feeluown-4.1.4/feeluown/local/schemas.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/local/ui.py` & `feeluown-4.1.4/feeluown/local/ui.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/media.py` & `feeluown-4.1.4/feeluown/media.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/mpv.py` & `feeluown-4.1.4/feeluown/mpv.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/nowplaying/__init__.py` & `feeluown-4.1.4/feeluown/nowplaying/__init__.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/nowplaying/linux/__init__.py` & `feeluown-4.1.4/feeluown/nowplaying/linux/__init__.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/nowplaying/linux/introspect.xml` & `feeluown-4.1.4/feeluown/nowplaying/linux/introspect.xml`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/nowplaying/linux/mpris2.py` & `feeluown-4.1.4/feeluown/nowplaying/linux/mpris2.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/nowplaying/macos.py` & `feeluown-4.1.4/feeluown/nowplaying/macos.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/nowplaying/nowplaying.py` & `feeluown-4.1.4/feeluown/nowplaying/nowplaying.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/player/__init__.py` & `feeluown-4.1.4/feeluown/player/__init__.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/player/base_player.py` & `feeluown-4.1.4/feeluown/player/base_player.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/player/delegate.py` & `feeluown-4.1.4/feeluown/player/delegate.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/player/fm.py` & `feeluown-4.1.4/feeluown/player/fm.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/player/lyric.py` & `feeluown-4.1.4/feeluown/player/lyric.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/player/metadata.py` & `feeluown-4.1.4/feeluown/player/metadata.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/player/mpvplayer.py` & `feeluown-4.1.4/feeluown/player/mpvplayer.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,28 +63,33 @@
         _mpv_set_property_string(self._mpv.handle, b'audio-device', audio_device)
         # old version libmpv(for example: (1, 20)) should set option by using
         # _mpv_set_option_string, while newer version can use _mpv_set_property_string
         _mpv_set_option_string(self._mpv.handle, b'user-agent',
                                b'Mozilla/5.0 (Windows NT 10.0; Win64; x64)')
 
         #: if video_format changes to None, there is no video available
-        self.video_format_changed = Signal()
+        self.video_format_changed = Signal()  # Optional[str]
+        self.audio_bitrate_changed = Signal()  # Optional[int], for example: 128001
 
         self._mpv.observe_property(
             'time-pos',
             lambda name, position: self._on_position_changed(position)
         )
         self._mpv.observe_property(
             'duration',
             lambda name, duration: self._on_duration_changed(duration)
         )
         self._mpv.observe_property(
             'video-format',
             lambda name, vformat: self._on_video_format_changed(vformat)
         )
+        self._mpv.observe_property(
+            'audio-bitrate',
+            lambda name, bitrate: self._on_audio_bitrate_changed(bitrate)
+        )
         # self._mpv.register_event_callback(lambda event: self._on_event(event))
         self._mpv._event_callbacks.append(self._on_event)
         logger.debug('Player initialize finished.')
 
         # this should always be `False` for fade=False,
         # because in that case `pause()` set status immediately
         self.pausing = False
@@ -256,14 +261,21 @@
 
     @AbstractPlayer.volume.setter  # type: ignore
     def volume(self, value):
         super(MpvPlayer, MpvPlayer).volume.__set__(self, value)
         self._mpv.volume = self.volume
 
     @property
+    def audio_bitrate(self):
+        """
+        .. versionadded: 4.1.4
+        """
+        return self._mpv.audio_bitrate
+
+    @property
     def video_format(self):
         return self._video_format
 
     @video_format.setter
     def video_format(self, vformat):
         self._video_format = vformat
         # Note, in current implementation, the video format is changed to None
@@ -285,14 +297,17 @@
         """listening to mpv duration change event"""
         logger.debug('Player receive duration changed signal')
         self.duration = duration
 
     def _on_video_format_changed(self, vformat):
         self.video_format = vformat
 
+    def _on_audio_bitrate_changed(self, bitrate):
+        self.audio_bitrate_changed.emit(bitrate)
+
     def _on_event(self, event):
         event_id = event['event_id']
         if event_id == MpvEventID.END_FILE:
             reason = event['event']['reason']
             logger.debug('Current song finished. reason: %d' % reason)
             if self.state != State.stopped and reason != MpvEventEndFile.ABORTED:
                 self.media_finished.emit()
```

### Comparing `feeluown-4.1.3/feeluown/player/playlist.py` & `feeluown-4.1.4/feeluown/player/playlist.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/player/radio.py` & `feeluown-4.1.4/feeluown/player/radio.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/player/recently_played.py` & `feeluown-4.1.4/feeluown/player/recently_played.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/plugin.py` & `feeluown-4.1.4/feeluown/plugin.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/serializers/__init__.py` & `feeluown-4.1.4/feeluown/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/serializers/_plain_formatter.py` & `feeluown-4.1.4/feeluown/serializers/_plain_formatter.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/serializers/base.py` & `feeluown-4.1.4/feeluown/serializers/base.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/serializers/json_.py` & `feeluown-4.1.4/feeluown/serializers/json_.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/serializers/model_helpers.py` & `feeluown-4.1.4/feeluown/serializers/model_helpers.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/serializers/objs.py` & `feeluown-4.1.4/feeluown/serializers/objs.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/serializers/plain.py` & `feeluown-4.1.4/feeluown/serializers/plain.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/serializers/python.py` & `feeluown-4.1.4/feeluown/serializers/python.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/serializers/typename.py` & `feeluown-4.1.4/feeluown/serializers/typename.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/server/__init__.py` & `feeluown-4.1.4/feeluown/server/__init__.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/server/data_structure.py` & `feeluown-4.1.4/feeluown/server/data_structure.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/server/dslv1/codegen.py` & `feeluown-4.1.4/feeluown/server/dslv1/codegen.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/server/dslv1/lexer.py` & `feeluown-4.1.4/feeluown/server/dslv1/lexer.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/server/dslv1/parser.py` & `feeluown-4.1.4/feeluown/server/dslv1/parser.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/server/dslv2.py` & `feeluown-4.1.4/feeluown/server/dslv2.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/server/excs.py` & `feeluown-4.1.4/feeluown/server/excs.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/server/handlers/base.py` & `feeluown-4.1.4/feeluown/server/handlers/base.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/server/handlers/exec_.py` & `feeluown-4.1.4/feeluown/server/handlers/exec_.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/server/handlers/handle.py` & `feeluown-4.1.4/feeluown/server/handlers/handle.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/server/handlers/help.py` & `feeluown-4.1.4/feeluown/server/handlers/help.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/server/handlers/player.py` & `feeluown-4.1.4/feeluown/server/handlers/player.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/server/handlers/playlist.py` & `feeluown-4.1.4/feeluown/server/handlers/playlist.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/server/handlers/search.py` & `feeluown-4.1.4/feeluown/server/handlers/search.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/server/handlers/show.py` & `feeluown-4.1.4/feeluown/server/handlers/show.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/server/handlers/sub.py` & `feeluown-4.1.4/feeluown/server/handlers/sub.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/server/protocol.py` & `feeluown-4.1.4/feeluown/server/protocol.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/server/pubsub/gateway.py` & `feeluown-4.1.4/feeluown/server/pubsub/gateway.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/server/pubsub/publishers.py` & `feeluown-4.1.4/feeluown/server/pubsub/publishers.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/server/server.py` & `feeluown-4.1.4/feeluown/server/server.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/task.py` & `feeluown-4.1.4/feeluown/task.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/utils/aio.py` & `feeluown-4.1.4/feeluown/utils/aio.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/utils/audio.py` & `feeluown-4.1.4/feeluown/utils/audio.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/utils/cache.py` & `feeluown-4.1.4/feeluown/utils/cache.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/utils/dispatch.py` & `feeluown-4.1.4/feeluown/utils/dispatch.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/utils/lang.py` & `feeluown-4.1.4/feeluown/utils/lang.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/utils/patch.py` & `feeluown-4.1.4/feeluown/utils/patch.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/utils/reader.py` & `feeluown-4.1.4/feeluown/utils/reader.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/utils/request.py` & `feeluown-4.1.4/feeluown/utils/request.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/utils/router.py` & `feeluown-4.1.4/feeluown/utils/router.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/utils/sync.py` & `feeluown-4.1.4/feeluown/utils/sync.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/utils/utils.py` & `feeluown-4.1.4/feeluown/utils/utils.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/utils/yt_dlp_cookies.py` & `feeluown-4.1.4/feeluown/utils/yt_dlp_cookies.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/version.py` & `feeluown-4.1.4/feeluown/version.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/webserver/jsonrpc_.py` & `feeluown-4.1.4/feeluown/webserver/jsonrpc_.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown/webserver/server.py` & `feeluown-4.1.4/feeluown/webserver/server.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/feeluown.egg-info/PKG-INFO` & `feeluown-4.1.4/feeluown.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feeluown
-Version: 4.1.3
+Version: 4.1.4
 Summary: *nix music player
 Home-page: https://github.com/feeluown/FeelUOwn
 Author: feeluown
 Author-email: yinshaowen241@gmail.com
 License: GPL-3.0
 Description: ## FeelUOwn - feel your own
```

### Comparing `feeluown-4.1.3/feeluown.egg-info/SOURCES.txt` & `feeluown-4.1.4/feeluown.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -99,14 +99,15 @@
 feeluown/gui/pages/provider_home.py
 feeluown/gui/pages/recently_played.py
 feeluown/gui/pages/recommendation.py
 feeluown/gui/pages/recommendation_daily_songs.py
 feeluown/gui/pages/search.py
 feeluown/gui/pages/song_explore.py
 feeluown/gui/pages/template.py
+feeluown/gui/pages/toplist.py
 feeluown/gui/uimain/__init__.py
 feeluown/gui/uimain/floating_box.py
 feeluown/gui/uimain/lyric.py
 feeluown/gui/uimain/nowplaying_overlay.py
 feeluown/gui/uimain/page_view.py
 feeluown/gui/uimain/player_bar.py
 feeluown/gui/uimain/playlist_overlay.py
```

### Comparing `feeluown-4.1.3/setup.cfg` & `feeluown-4.1.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.3/setup.py` & `feeluown-4.1.4/setup.py`

 * *Files identical despite different names*

