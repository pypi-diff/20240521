# Comparing `tmp/toot-tooi-0.9.0.tar.gz` & `tmp/toot-tooi-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toot-tooi-0.9.0.tar", last modified: Thu Feb  1 14:04:34 2024, max compression
+gzip compressed data, was "toot-tooi-0.9.1.tar", last modified: Fri Feb  2 10:03:47 2024, max compression
```

## Comparing `toot-tooi-0.9.0.tar` & `toot-tooi-0.9.1.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-02-01 14:04:34.615181 toot-tooi-0.9.0/
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       31 2023-08-11 10:29:49.000000 toot-tooi-0.9.0/.flake8
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       43 2024-01-15 08:10:01.000000 toot-tooi-0.9.0/.gitignore
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1065 2024-01-06 19:11:36.000000 toot-tooi-0.9.0/LICENSE
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      159 2024-01-10 21:38:44.000000 toot-tooi-0.9.0/Makefile
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     4683 2024-02-01 14:04:34.614181 toot-tooi-0.9.0/PKG-INFO
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2434 2024-01-28 08:05:41.000000 toot-tooi-0.9.0/README.md
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1280 2024-02-01 10:32:24.000000 toot-tooi-0.9.0/pyproject.toml
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       38 2024-02-01 14:04:34.615181 toot-tooi-0.9.0/setup.cfg
-drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-02-01 14:04:34.606181 toot-tooi-0.9.0/tooi/
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      149 2024-01-09 12:48:14.000000 toot-tooi-0.9.0/tooi/__init__.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       34 2023-08-13 10:26:48.000000 toot-tooi-0.9.0/tooi/__main__.py
-drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-02-01 14:04:34.607181 toot-tooi-0.9.0/tooi/api/
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2827 2024-02-01 12:23:54.000000 toot-tooi-0.9.0/tooi/api/__init__.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1008 2024-01-28 08:07:21.000000 toot-tooi-0.9.0/tooi/api/accounts.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1054 2024-01-16 08:33:14.000000 toot-tooi-0.9.0/tooi/api/instance.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      377 2024-01-16 08:33:14.000000 toot-tooi-0.9.0/tooi/api/search.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2906 2024-02-01 13:52:15.000000 toot-tooi-0.9.0/tooi/api/statuses.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    13083 2024-01-28 08:07:21.000000 toot-tooi-0.9.0/tooi/api/streaming.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    20909 2024-01-28 08:07:21.000000 toot-tooi-0.9.0/tooi/api/timeline.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      991 2023-12-31 08:30:09.000000 toot-tooi-0.9.0/tooi/api/types.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      346 2024-02-01 10:48:02.000000 toot-tooi-0.9.0/tooi/app.css
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     8138 2024-02-01 13:19:20.000000 toot-tooi-0.9.0/tooi/app.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1960 2024-01-17 07:10:48.000000 toot-tooi-0.9.0/tooi/asyncio.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1832 2024-02-01 12:03:02.000000 toot-tooi-0.9.0/tooi/auth.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2357 2024-02-01 12:19:26.000000 toot-tooi-0.9.0/tooi/cli.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1012 2024-02-01 13:20:23.000000 toot-tooi-0.9.0/tooi/context.py
-drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-02-01 14:04:34.608181 toot-tooi-0.9.0/tooi/data/
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)        0 2023-12-31 08:33:59.000000 toot-tooi-0.9.0/tooi/data/__init__.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1671 2024-02-01 13:52:15.000000 toot-tooi-0.9.0/tooi/data/events.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     3034 2024-01-28 08:07:21.000000 toot-tooi-0.9.0/tooi/data/instance.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     9620 2024-01-28 08:07:21.000000 toot-tooi-0.9.0/tooi/entities.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    11837 2023-08-11 10:29:49.000000 toot-tooi-0.9.0/tooi/lorem.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1997 2024-02-01 13:02:27.000000 toot-tooi-0.9.0/tooi/messages.py
-drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-02-01 14:04:34.609181 toot-tooi-0.9.0/tooi/screens/
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)        0 2023-12-31 08:33:59.000000 toot-tooi-0.9.0/tooi/screens/__init__.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     3036 2024-01-23 10:39:11.000000 toot-tooi-0.9.0/tooi/screens/account.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    10530 2024-02-01 10:50:46.000000 toot-tooi-0.9.0/tooi/screens/compose.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2640 2024-01-13 19:58:50.000000 toot-tooi-0.9.0/tooi/screens/goto.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      739 2024-01-06 12:54:11.000000 toot-tooi-0.9.0/tooi/screens/help.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1790 2024-01-15 11:33:59.000000 toot-tooi-0.9.0/tooi/screens/instance.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      688 2024-01-15 11:33:59.000000 toot-tooi-0.9.0/tooi/screens/loading.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     3584 2024-01-23 10:39:11.000000 toot-tooi-0.9.0/tooi/screens/main.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     4107 2024-02-01 13:59:37.000000 toot-tooi-0.9.0/tooi/screens/media.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      826 2024-01-15 11:33:59.000000 toot-tooi-0.9.0/tooi/screens/messagebox.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      914 2024-02-01 10:50:46.000000 toot-tooi-0.9.0/tooi/screens/modal.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      875 2023-12-31 08:30:09.000000 toot-tooi-0.9.0/tooi/screens/source.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1675 2024-01-15 11:33:59.000000 toot-tooi-0.9.0/tooi/screens/status_context.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2977 2024-01-28 08:07:21.000000 toot-tooi-0.9.0/tooi/settings.py
-drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-02-01 14:04:34.610181 toot-tooi-0.9.0/tooi/tabs/
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     4114 2024-01-18 06:45:52.000000 toot-tooi-0.9.0/tooi/tabs/search.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    10816 2024-02-01 13:52:15.000000 toot-tooi-0.9.0/tooi/tabs/timeline.py
-drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-02-01 14:04:34.611181 toot-tooi-0.9.0/tooi/utils/
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)        0 2023-07-27 18:12:42.000000 toot-tooi-0.9.0/tooi/utils/__init__.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      763 2024-01-15 08:10:01.000000 toot-tooi-0.9.0/tooi/utils/datetime.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1279 2024-02-01 14:01:24.000000 toot-tooi-0.9.0/tooi/utils/file.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2183 2024-01-23 10:39:11.000000 toot-tooi-0.9.0/tooi/utils/from_dict.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      568 2023-12-31 08:30:09.000000 toot-tooi-0.9.0/tooi/utils/html.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2479 2024-02-01 04:51:04.000000 toot-tooi-0.9.0/tooi/utils/images.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      290 2023-12-31 08:30:09.000000 toot-tooi-0.9.0/tooi/utils/string.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2026 2024-01-23 10:39:11.000000 toot-tooi-0.9.0/tooi/utils/temp.py
-drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-02-01 14:04:34.613181 toot-tooi-0.9.0/tooi/widgets/
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)        0 2023-07-27 18:12:42.000000 toot-tooi-0.9.0/tooi/widgets/__init__.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      765 2024-01-28 08:07:21.000000 toot-tooi-0.9.0/tooi/widgets/account.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2803 2024-02-01 10:52:01.000000 toot-tooi-0.9.0/tooi/widgets/compose.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1341 2024-02-01 13:52:15.000000 toot-tooi-0.9.0/tooi/widgets/dialog.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2126 2024-01-28 08:07:21.000000 toot-tooi-0.9.0/tooi/widgets/event_detail.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     5715 2024-02-01 13:52:15.000000 toot-tooi-0.9.0/tooi/widgets/event_list.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      358 2023-08-13 10:26:49.000000 toot-tooi-0.9.0/tooi/widgets/header.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1365 2024-02-01 05:01:17.000000 toot-tooi-0.9.0/tooi/widgets/image.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      811 2024-01-15 11:33:59.000000 toot-tooi-0.9.0/tooi/widgets/link.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      772 2024-01-29 08:32:00.000000 toot-tooi-0.9.0/tooi/widgets/list_view.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      327 2023-12-31 08:32:23.000000 toot-tooi-0.9.0/tooi/widgets/markdown.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2011 2024-01-29 08:32:00.000000 toot-tooi-0.9.0/tooi/widgets/menu.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1730 2024-01-28 08:07:21.000000 toot-tooi-0.9.0/tooi/widgets/notification_detail.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2344 2024-01-15 11:33:59.000000 toot-tooi-0.9.0/tooi/widgets/poll.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      438 2024-01-10 21:52:40.000000 toot-tooi-0.9.0/tooi/widgets/status_bar.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     7096 2024-01-29 08:48:01.000000 toot-tooi-0.9.0/tooi/widgets/status_detail.py
-drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-02-01 14:04:34.614181 toot-tooi-0.9.0/toot_tooi.egg-info/
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     4683 2024-02-01 14:04:34.000000 toot-tooi-0.9.0/toot_tooi.egg-info/PKG-INFO
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1594 2024-02-01 14:04:34.000000 toot-tooi-0.9.0/toot_tooi.egg-info/SOURCES.txt
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)        1 2024-02-01 14:04:34.000000 toot-tooi-0.9.0/toot_tooi.egg-info/dependency_links.txt
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       39 2024-02-01 14:04:34.000000 toot-tooi-0.9.0/toot_tooi.egg-info/entry_points.txt
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      162 2024-02-01 14:04:34.000000 toot-tooi-0.9.0/toot_tooi.egg-info/requires.txt
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)        5 2024-02-01 14:04:34.000000 toot-tooi-0.9.0/toot_tooi.egg-info/top_level.txt
+drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-02-02 10:03:47.950022 toot-tooi-0.9.1/
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       31 2023-08-11 10:29:49.000000 toot-tooi-0.9.1/.flake8
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       43 2024-01-15 08:10:01.000000 toot-tooi-0.9.1/.gitignore
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1065 2024-01-06 19:11:36.000000 toot-tooi-0.9.1/LICENSE
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      159 2024-01-10 21:38:44.000000 toot-tooi-0.9.1/Makefile
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     6263 2024-02-02 10:03:47.950022 toot-tooi-0.9.1/PKG-INFO
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     4014 2024-02-02 09:51:03.000000 toot-tooi-0.9.1/README.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1280 2024-02-01 10:32:24.000000 toot-tooi-0.9.1/pyproject.toml
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       38 2024-02-02 10:03:47.950022 toot-tooi-0.9.1/setup.cfg
+drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-02-02 10:03:47.943021 toot-tooi-0.9.1/tooi/
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      149 2024-01-09 12:48:14.000000 toot-tooi-0.9.1/tooi/__init__.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       34 2023-08-13 10:26:48.000000 toot-tooi-0.9.1/tooi/__main__.py
+drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-02-02 10:03:47.943021 toot-tooi-0.9.1/tooi/api/
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2827 2024-02-01 12:23:54.000000 toot-tooi-0.9.1/tooi/api/__init__.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1008 2024-01-28 08:07:21.000000 toot-tooi-0.9.1/tooi/api/accounts.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1054 2024-01-16 08:33:14.000000 toot-tooi-0.9.1/tooi/api/instance.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      377 2024-01-16 08:33:14.000000 toot-tooi-0.9.1/tooi/api/search.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2906 2024-02-01 13:52:15.000000 toot-tooi-0.9.1/tooi/api/statuses.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    13083 2024-01-28 08:07:21.000000 toot-tooi-0.9.1/tooi/api/streaming.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    20909 2024-01-28 08:07:21.000000 toot-tooi-0.9.1/tooi/api/timeline.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      991 2023-12-31 08:30:09.000000 toot-tooi-0.9.1/tooi/api/types.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      346 2024-02-01 10:48:02.000000 toot-tooi-0.9.1/tooi/app.css
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     8138 2024-02-01 13:19:20.000000 toot-tooi-0.9.1/tooi/app.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1960 2024-01-17 07:10:48.000000 toot-tooi-0.9.1/tooi/asyncio.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1935 2024-02-02 09:20:49.000000 toot-tooi-0.9.1/tooi/auth.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2714 2024-02-02 09:42:12.000000 toot-tooi-0.9.1/tooi/cli.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1012 2024-02-01 13:20:23.000000 toot-tooi-0.9.1/tooi/context.py
+drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-02-02 10:03:47.944022 toot-tooi-0.9.1/tooi/data/
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)        0 2023-12-31 08:33:59.000000 toot-tooi-0.9.1/tooi/data/__init__.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1671 2024-02-01 13:52:15.000000 toot-tooi-0.9.1/tooi/data/events.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     3034 2024-01-28 08:07:21.000000 toot-tooi-0.9.1/tooi/data/instance.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     9620 2024-01-28 08:07:21.000000 toot-tooi-0.9.1/tooi/entities.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    11837 2023-08-11 10:29:49.000000 toot-tooi-0.9.1/tooi/lorem.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1997 2024-02-01 13:02:27.000000 toot-tooi-0.9.1/tooi/messages.py
+drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-02-02 10:03:47.945021 toot-tooi-0.9.1/tooi/screens/
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)        0 2023-12-31 08:33:59.000000 toot-tooi-0.9.1/tooi/screens/__init__.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     3036 2024-01-23 10:39:11.000000 toot-tooi-0.9.1/tooi/screens/account.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    10530 2024-02-01 10:50:46.000000 toot-tooi-0.9.1/tooi/screens/compose.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2640 2024-01-13 19:58:50.000000 toot-tooi-0.9.1/tooi/screens/goto.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      739 2024-01-06 12:54:11.000000 toot-tooi-0.9.1/tooi/screens/help.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1790 2024-01-15 11:33:59.000000 toot-tooi-0.9.1/tooi/screens/instance.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      688 2024-01-15 11:33:59.000000 toot-tooi-0.9.1/tooi/screens/loading.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     3584 2024-01-23 10:39:11.000000 toot-tooi-0.9.1/tooi/screens/main.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     4107 2024-02-01 13:59:37.000000 toot-tooi-0.9.1/tooi/screens/media.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      826 2024-01-15 11:33:59.000000 toot-tooi-0.9.1/tooi/screens/messagebox.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      914 2024-02-01 10:50:46.000000 toot-tooi-0.9.1/tooi/screens/modal.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      875 2023-12-31 08:30:09.000000 toot-tooi-0.9.1/tooi/screens/source.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1675 2024-01-15 11:33:59.000000 toot-tooi-0.9.1/tooi/screens/status_context.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2977 2024-01-28 08:07:21.000000 toot-tooi-0.9.1/tooi/settings.py
+drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-02-02 10:03:47.945021 toot-tooi-0.9.1/tooi/tabs/
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     4114 2024-01-18 06:45:52.000000 toot-tooi-0.9.1/tooi/tabs/search.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    10816 2024-02-01 13:52:15.000000 toot-tooi-0.9.1/tooi/tabs/timeline.py
+drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-02-02 10:03:47.946021 toot-tooi-0.9.1/tooi/utils/
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)        0 2023-07-27 18:12:42.000000 toot-tooi-0.9.1/tooi/utils/__init__.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      763 2024-01-15 08:10:01.000000 toot-tooi-0.9.1/tooi/utils/datetime.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1279 2024-02-01 14:01:24.000000 toot-tooi-0.9.1/tooi/utils/file.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2183 2024-01-23 10:39:11.000000 toot-tooi-0.9.1/tooi/utils/from_dict.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      568 2023-12-31 08:30:09.000000 toot-tooi-0.9.1/tooi/utils/html.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2479 2024-02-01 04:51:04.000000 toot-tooi-0.9.1/tooi/utils/images.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      290 2023-12-31 08:30:09.000000 toot-tooi-0.9.1/tooi/utils/string.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2026 2024-01-23 10:39:11.000000 toot-tooi-0.9.1/tooi/utils/temp.py
+drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-02-02 10:03:47.948022 toot-tooi-0.9.1/tooi/widgets/
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)        0 2023-07-27 18:12:42.000000 toot-tooi-0.9.1/tooi/widgets/__init__.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      765 2024-01-28 08:07:21.000000 toot-tooi-0.9.1/tooi/widgets/account.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2803 2024-02-01 10:52:01.000000 toot-tooi-0.9.1/tooi/widgets/compose.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1341 2024-02-01 13:52:15.000000 toot-tooi-0.9.1/tooi/widgets/dialog.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2126 2024-01-28 08:07:21.000000 toot-tooi-0.9.1/tooi/widgets/event_detail.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     5715 2024-02-01 13:52:15.000000 toot-tooi-0.9.1/tooi/widgets/event_list.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      358 2023-08-13 10:26:49.000000 toot-tooi-0.9.1/tooi/widgets/header.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1365 2024-02-01 05:01:17.000000 toot-tooi-0.9.1/tooi/widgets/image.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      811 2024-01-15 11:33:59.000000 toot-tooi-0.9.1/tooi/widgets/link.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      772 2024-01-29 08:32:00.000000 toot-tooi-0.9.1/tooi/widgets/list_view.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      327 2023-12-31 08:32:23.000000 toot-tooi-0.9.1/tooi/widgets/markdown.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2011 2024-01-29 08:32:00.000000 toot-tooi-0.9.1/tooi/widgets/menu.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1730 2024-01-28 08:07:21.000000 toot-tooi-0.9.1/tooi/widgets/notification_detail.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2344 2024-01-15 11:33:59.000000 toot-tooi-0.9.1/tooi/widgets/poll.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      438 2024-01-10 21:52:40.000000 toot-tooi-0.9.1/tooi/widgets/status_bar.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     7096 2024-01-29 08:48:01.000000 toot-tooi-0.9.1/tooi/widgets/status_detail.py
+drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-02-02 10:03:47.949021 toot-tooi-0.9.1/toot_tooi.egg-info/
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     6263 2024-02-02 10:03:47.000000 toot-tooi-0.9.1/toot_tooi.egg-info/PKG-INFO
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1594 2024-02-02 10:03:47.000000 toot-tooi-0.9.1/toot_tooi.egg-info/SOURCES.txt
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)        1 2024-02-02 10:03:47.000000 toot-tooi-0.9.1/toot_tooi.egg-info/dependency_links.txt
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       39 2024-02-02 10:03:47.000000 toot-tooi-0.9.1/toot_tooi.egg-info/entry_points.txt
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      162 2024-02-02 10:03:47.000000 toot-tooi-0.9.1/toot_tooi.egg-info/requires.txt
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)        5 2024-02-02 10:03:47.000000 toot-tooi-0.9.1/toot_tooi.egg-info/top_level.txt
```

### Comparing `toot-tooi-0.9.0/LICENSE` & `toot-tooi-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `toot-tooi-0.9.0/pyproject.toml` & `toot-tooi-0.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `toot-tooi-0.9.0/tooi/api/__init__.py` & `toot-tooi-0.9.1/tooi/api/__init__.py`

 * *Files identical despite different names*

### Comparing `toot-tooi-0.9.0/tooi/api/accounts.py` & `toot-tooi-0.9.1/tooi/api/accounts.py`

 * *Files identical despite different names*

### Comparing `toot-tooi-0.9.0/tooi/api/instance.py` & `toot-tooi-0.9.1/tooi/api/instance.py`

 * *Files identical despite different names*

### Comparing `toot-tooi-0.9.0/tooi/api/statuses.py` & `toot-tooi-0.9.1/tooi/api/statuses.py`

 * *Files identical despite different names*

### Comparing `toot-tooi-0.9.0/tooi/api/streaming.py` & `toot-tooi-0.9.1/tooi/api/streaming.py`

 * *Files identical despite different names*

### Comparing `toot-tooi-0.9.0/tooi/api/timeline.py` & `toot-tooi-0.9.1/tooi/api/timeline.py`

 * *Files identical despite different names*

### Comparing `toot-tooi-0.9.0/tooi/api/types.py` & `toot-tooi-0.9.1/tooi/api/types.py`

 * *Files identical despite different names*

### Comparing `toot-tooi-0.9.0/tooi/app.py` & `toot-tooi-0.9.1/tooi/app.py`

 * *Files identical despite different names*

### Comparing `toot-tooi-0.9.0/tooi/asyncio.py` & `toot-tooi-0.9.1/tooi/asyncio.py`

 * *Files identical despite different names*

### Comparing `toot-tooi-0.9.0/tooi/auth.py` & `toot-tooi-0.9.1/tooi/auth.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,24 @@
-import asyncio
-from typing import Any
 import aiohttp
+import asyncio
 import httpx
 import json
 
 from dataclasses import dataclass, field
 from os import path
+from typing import Any
 
 
 AUTH_CONTEXT_PATH = path.expanduser("~/.config/toot/config.json")
 
 
+class NotLoggedInError(Exception):
+    ...
+
+
 @dataclass
 class AuthContext:
     acct: str
     domain: str
     base_url: str
     access_token: str
     client: httpx.AsyncClient
@@ -29,23 +33,26 @@
                     base_url=self.base_url,
                     headers={"Authorization": f"Bearer {self.access_token}"},
                 )
 
             return self.aio_client
 
 
-
 # TODO: uses toot config
 def load_auth_context() -> AuthContext:
     actx = _read_auth_context()
     return _parse_auth_context(actx)
 
 
 def _parse_auth_context(config: dict[str, Any]):
     active_user = config["active_user"]
+
+    if not active_user:
+        raise NotLoggedInError()
+
     user_data = config["users"][active_user]
     instance_data = config["apps"][user_data["instance"]]
     domain = instance_data["instance"]
     base_url = instance_data["base_url"]
     access_token = user_data["access_token"]
 
     # TODO: close client on exiting app
```

### Comparing `toot-tooi-0.9.0/tooi/cli.py` & `toot-tooi-0.9.1/tooi/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import click
-import logging
 import dataclasses
+import logging
+import sys
 
 from textual.logging import TextualHandler
 from typing import Optional
 
 from tooi.app import TooiApp
+from tooi.auth import NotLoggedInError
 from tooi.context import create_context, set_context
 from tooi.settings import get_settings
 
 
 def get_default_map():
     return dataclasses.asdict(get_settings().options)
 
@@ -53,27 +55,33 @@
 )
 def tooi(
         always_show_sensitive: Optional[bool],
         relative_timestamps: bool,
         timeline_refresh: int,
         streaming: bool):
 
-    ctx = create_context()
+    try:
+        ctx = create_context()
+    except NotLoggedInError:
+        click.secho("Not logged in. Please run `toot login`", fg="red")
+        click.secho("Note that tooi at this point requires toot for authentication.", fg="red")
+        click.secho("https://toot.bezdomni.net/installation.html", fg="red")
+        sys.exit(1)
+
     ctx.config = get_settings()
     ctx.config.options.always_show_sensitive = always_show_sensitive
     ctx.config.options.relative_timestamps = relative_timestamps
     ctx.config.options.timeline_refresh = timeline_refresh
     ctx.config.options.streaming = streaming
     # Streaming is not reliable, so if it's enabled, force timeline_refresh to be enabled as well;
     # this catches any events that streaming missed.
     if ctx.config.options.streaming and not ctx.config.options.timeline_refresh:
         ctx.config.options.timeline_refresh = 120
 
     set_context(ctx)
-
     app = TooiApp()
     app.run()
 
 
 def main():
     logging.basicConfig(level=logging.INFO, handlers=[TextualHandler()])
     logging.getLogger("http").setLevel(logging.WARNING)
```

### Comparing `toot-tooi-0.9.0/tooi/context.py` & `toot-tooi-0.9.1/tooi/context.py`

 * *Files identical despite different names*

### Comparing `toot-tooi-0.9.0/tooi/data/events.py` & `toot-tooi-0.9.1/tooi/data/events.py`

 * *Files identical despite different names*

### Comparing `toot-tooi-0.9.0/tooi/data/instance.py` & `toot-tooi-0.9.1/tooi/data/instance.py`

 * *Files identical despite different names*

### Comparing `toot-tooi-0.9.0/tooi/entities.py` & `toot-tooi-0.9.1/tooi/entities.py`

 * *Files identical despite different names*

### Comparing `toot-tooi-0.9.0/tooi/lorem.py` & `toot-tooi-0.9.1/tooi/lorem.py`

 * *Files identical despite different names*

### Comparing `toot-tooi-0.9.0/tooi/messages.py` & `toot-tooi-0.9.1/tooi/messages.py`

 * *Files identical despite different names*

### Comparing `toot-tooi-0.9.0/tooi/screens/account.py` & `toot-tooi-0.9.1/tooi/screens/account.py`

 * *Files identical despite different names*

### Comparing `toot-tooi-0.9.0/tooi/screens/compose.py` & `toot-tooi-0.9.1/tooi/screens/compose.py`

 * *Files identical despite different names*

### Comparing `toot-tooi-0.9.0/tooi/screens/goto.py` & `toot-tooi-0.9.1/tooi/screens/goto.py`

 * *Files identical despite different names*

### Comparing `toot-tooi-0.9.0/tooi/screens/help.py` & `toot-tooi-0.9.1/tooi/screens/help.py`

 * *Files identical despite different names*

### Comparing `toot-tooi-0.9.0/tooi/screens/instance.py` & `toot-tooi-0.9.1/tooi/screens/instance.py`

 * *Files identical despite different names*

### Comparing `toot-tooi-0.9.0/tooi/screens/loading.py` & `toot-tooi-0.9.1/tooi/screens/loading.py`

 * *Files identical despite different names*

### Comparing `toot-tooi-0.9.0/tooi/screens/main.py` & `toot-tooi-0.9.1/tooi/screens/main.py`

 * *Files identical despite different names*

### Comparing `toot-tooi-0.9.0/tooi/screens/media.py` & `toot-tooi-0.9.1/tooi/screens/media.py`

 * *Files identical despite different names*

### Comparing `toot-tooi-0.9.0/tooi/screens/messagebox.py` & `toot-tooi-0.9.1/tooi/screens/messagebox.py`

 * *Files identical despite different names*

### Comparing `toot-tooi-0.9.0/tooi/screens/modal.py` & `toot-tooi-0.9.1/tooi/screens/modal.py`

 * *Files identical despite different names*

### Comparing `toot-tooi-0.9.0/tooi/screens/source.py` & `toot-tooi-0.9.1/tooi/screens/source.py`

 * *Files identical despite different names*

### Comparing `toot-tooi-0.9.0/tooi/screens/status_context.py` & `toot-tooi-0.9.1/tooi/screens/status_context.py`

 * *Files identical despite different names*

### Comparing `toot-tooi-0.9.0/tooi/settings.py` & `toot-tooi-0.9.1/tooi/settings.py`

 * *Files identical despite different names*

### Comparing `toot-tooi-0.9.0/tooi/tabs/search.py` & `toot-tooi-0.9.1/tooi/tabs/search.py`

 * *Files identical despite different names*

### Comparing `toot-tooi-0.9.0/tooi/tabs/timeline.py` & `toot-tooi-0.9.1/tooi/tabs/timeline.py`

 * *Files identical despite different names*

### Comparing `toot-tooi-0.9.0/tooi/utils/datetime.py` & `toot-tooi-0.9.1/tooi/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `toot-tooi-0.9.0/tooi/utils/file.py` & `toot-tooi-0.9.1/tooi/utils/file.py`

 * *Files identical despite different names*

### Comparing `toot-tooi-0.9.0/tooi/utils/from_dict.py` & `toot-tooi-0.9.1/tooi/utils/from_dict.py`

 * *Files identical despite different names*

### Comparing `toot-tooi-0.9.0/tooi/utils/html.py` & `toot-tooi-0.9.1/tooi/utils/html.py`

 * *Files identical despite different names*

### Comparing `toot-tooi-0.9.0/tooi/utils/images.py` & `toot-tooi-0.9.1/tooi/utils/images.py`

 * *Files identical despite different names*

### Comparing `toot-tooi-0.9.0/tooi/utils/temp.py` & `toot-tooi-0.9.1/tooi/utils/temp.py`

 * *Files identical despite different names*

### Comparing `toot-tooi-0.9.0/tooi/widgets/account.py` & `toot-tooi-0.9.1/tooi/widgets/account.py`

 * *Files identical despite different names*

### Comparing `toot-tooi-0.9.0/tooi/widgets/compose.py` & `toot-tooi-0.9.1/tooi/widgets/compose.py`

 * *Files identical despite different names*

### Comparing `toot-tooi-0.9.0/tooi/widgets/dialog.py` & `toot-tooi-0.9.1/tooi/widgets/dialog.py`

 * *Files identical despite different names*

### Comparing `toot-tooi-0.9.0/tooi/widgets/event_detail.py` & `toot-tooi-0.9.1/tooi/widgets/event_detail.py`

 * *Files identical despite different names*

### Comparing `toot-tooi-0.9.0/tooi/widgets/event_list.py` & `toot-tooi-0.9.1/tooi/widgets/event_list.py`

 * *Files identical despite different names*

### Comparing `toot-tooi-0.9.0/tooi/widgets/image.py` & `toot-tooi-0.9.1/tooi/widgets/image.py`

 * *Files identical despite different names*

### Comparing `toot-tooi-0.9.0/tooi/widgets/link.py` & `toot-tooi-0.9.1/tooi/widgets/link.py`

 * *Files identical despite different names*

### Comparing `toot-tooi-0.9.0/tooi/widgets/list_view.py` & `toot-tooi-0.9.1/tooi/widgets/list_view.py`

 * *Files identical despite different names*

### Comparing `toot-tooi-0.9.0/tooi/widgets/menu.py` & `toot-tooi-0.9.1/tooi/widgets/menu.py`

 * *Files identical despite different names*

### Comparing `toot-tooi-0.9.0/tooi/widgets/notification_detail.py` & `toot-tooi-0.9.1/tooi/widgets/notification_detail.py`

 * *Files identical despite different names*

### Comparing `toot-tooi-0.9.0/tooi/widgets/poll.py` & `toot-tooi-0.9.1/tooi/widgets/poll.py`

 * *Files identical despite different names*

### Comparing `toot-tooi-0.9.0/tooi/widgets/status_detail.py` & `toot-tooi-0.9.1/tooi/widgets/status_detail.py`

 * *Files identical despite different names*

### Comparing `toot-tooi-0.9.0/toot_tooi.egg-info/SOURCES.txt` & `toot-tooi-0.9.1/toot_tooi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

