# Comparing `tmp/datapools-1.0.57.tar.gz` & `tmp/datapools-1.0.58.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datapools-1.0.57.tar", last modified: Sat May 18 14:06:59 2024, max compression
+gzip compressed data, was "datapools-1.0.58.tar", last modified: Tue May 21 06:04:22 2024, max compression
```

## Comparing `datapools-1.0.57.tar` & `datapools-1.0.58.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:06:59.148393 datapools-1.0.57/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-18 14:06:50.000000 datapools-1.0.57/Containerfile
--rw-r--r--   0 runner    (1001) docker     (127)    19488 2024-05-18 14:06:50.000000 datapools-1.0.57/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (127)     7560 2024-05-18 14:06:50.000000 datapools-1.0.57/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-18 14:06:50.000000 datapools-1.0.57/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-18 14:06:59.148393 datapools-1.0.57/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-18 14:06:50.000000 datapools-1.0.57/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:06:59.132394 datapools-1.0.57/datapools/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-18 14:06:50.000000 datapools-1.0.57/datapools/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-18 14:06:50.000000 datapools-1.0.57/datapools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-18 14:06:50.000000 datapools-1.0.57/datapools/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-05-18 14:06:50.000000 datapools-1.0.57/datapools/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-05-18 14:06:50.000000 datapools-1.0.57/datapools/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:06:59.136394 datapools-1.0.57/datapools/common/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-18 14:06:50.000000 datapools-1.0.57/datapools/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-05-18 14:06:50.000000 datapools-1.0.57/datapools/common/backend_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-18 14:06:50.000000 datapools-1.0.57/datapools/common/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:06:59.136394 datapools-1.0.57/datapools/common/queues/
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-18 14:06:50.000000 datapools-1.0.57/datapools/common/queues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12022 2024-05-18 14:06:50.000000 datapools-1.0.57/datapools/common/queues/rabbitmq.py
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-05-18 14:06:50.000000 datapools-1.0.57/datapools/common/queues/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     6241 2024-05-18 14:06:50.000000 datapools-1.0.57/datapools/common/session_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-18 14:06:50.000000 datapools-1.0.57/datapools/common/stoppable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:06:59.136394 datapools-1.0.57/datapools/common/storage/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-18 14:06:50.000000 datapools-1.0.57/datapools/common/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-18 14:06:50.000000 datapools-1.0.57/datapools/common/storage/base_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-18 14:06:50.000000 datapools-1.0.57/datapools/common/storage/file_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:06:59.136394 datapools-1.0.57/datapools/common/tasks_db/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-18 14:06:50.000000 datapools-1.0.57/datapools/common/tasks_db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-05-18 14:06:50.000000 datapools-1.0.57/datapools/common/tasks_db/redis.py.bak
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-05-18 14:06:50.000000 datapools-1.0.57/datapools/common/tasks_db/tasks_db.py
--rw-r--r--   0 runner    (1001) docker     (127)     9091 2024-05-18 14:06:50.000000 datapools-1.0.57/datapools/common/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:06:59.136394 datapools-1.0.57/datapools/producer/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-18 14:06:50.000000 datapools-1.0.57/datapools/producer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6288 2024-05-18 14:06:50.000000 datapools-1.0.57/datapools/producer/base_producer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:06:59.136394 datapools-1.0.57/datapools/scheduler/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-18 14:06:50.000000 datapools-1.0.57/datapools/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12842 2024-05-18 14:06:50.000000 datapools-1.0.57/datapools/scheduler/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:06:59.140394 datapools-1.0.57/datapools/worker/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-18 14:06:50.000000 datapools-1.0.57/datapools/worker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:06:59.140394 datapools-1.0.57/datapools/worker/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 14:06:50.000000 datapools-1.0.57/datapools/worker/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12311 2024-05-18 14:06:50.000000 datapools-1.0.57/datapools/worker/plugins/base_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:06:59.140394 datapools-1.0.57/datapools/worker/plugins/dataphoenix_info/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-18 14:06:50.000000 datapools-1.0.57/datapools/worker/plugins/dataphoenix_info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6865 2024-05-18 14:06:50.000000 datapools-1.0.57/datapools/worker/plugins/dataphoenix_info/dataphoenix_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:06:59.140394 datapools-1.0.57/datapools/worker/plugins/default/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-18 14:06:50.000000 datapools-1.0.57/datapools/worker/plugins/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8761 2024-05-18 14:06:50.000000 datapools-1.0.57/datapools/worker/plugins/default/default.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:06:59.140394 datapools-1.0.57/datapools/worker/plugins/deutsche_welle/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-18 14:06:50.000000 datapools-1.0.57/datapools/worker/plugins/deutsche_welle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4693 2024-05-18 14:06:50.000000 datapools-1.0.57/datapools/worker/plugins/deutsche_welle/deutsche_welle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:06:59.140394 datapools-1.0.57/datapools/worker/plugins/freesound_org/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-18 14:06:50.000000 datapools-1.0.57/datapools/worker/plugins/freesound_org/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7619 2024-05-18 14:06:50.000000 datapools-1.0.57/datapools/worker/plugins/freesound_org/freesound_org.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:06:59.140394 datapools-1.0.57/datapools/worker/plugins/google_drive/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-18 14:06:50.000000 datapools-1.0.57/datapools/worker/plugins/google_drive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9636 2024-05-18 14:06:50.000000 datapools-1.0.57/datapools/worker/plugins/google_drive/google_drive.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:06:59.140394 datapools-1.0.57/datapools/worker/plugins/imageshack/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-18 14:06:50.000000 datapools-1.0.57/datapools/worker/plugins/imageshack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10173 2024-05-18 14:06:50.000000 datapools-1.0.57/datapools/worker/plugins/imageshack/imageshack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:06:59.140394 datapools-1.0.57/datapools/worker/plugins/s3/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-18 14:06:50.000000 datapools-1.0.57/datapools/worker/plugins/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-05-18 14:06:50.000000 datapools-1.0.57/datapools/worker/plugins/s3/s3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:06:59.144394 datapools-1.0.57/datapools/worker/plugins/theguardian/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-18 14:06:50.000000 datapools-1.0.57/datapools/worker/plugins/theguardian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-05-18 14:06:50.000000 datapools-1.0.57/datapools/worker/plugins/theguardian/theguardian.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:06:59.144394 datapools-1.0.57/datapools/worker/plugins/washingtonpost/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-18 14:06:50.000000 datapools-1.0.57/datapools/worker/plugins/washingtonpost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6550 2024-05-18 14:06:50.000000 datapools-1.0.57/datapools/worker/plugins/washingtonpost/washingtonpost.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:06:59.144394 datapools-1.0.57/datapools/worker/plugins/wikipedia/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-18 14:06:50.000000 datapools-1.0.57/datapools/worker/plugins/wikipedia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7519 2024-05-18 14:06:50.000000 datapools-1.0.57/datapools/worker/plugins/wikipedia/wikipedia.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:06:59.144394 datapools-1.0.57/datapools/worker/plugins/youtube_channel/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-18 14:06:50.000000 datapools-1.0.57/datapools/worker/plugins/youtube_channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10015 2024-05-18 14:06:50.000000 datapools-1.0.57/datapools/worker/plugins/youtube_channel/youtube_channel.py
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-18 14:06:50.000000 datapools-1.0.57/datapools/worker/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-18 14:06:50.000000 datapools-1.0.57/datapools/worker/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16573 2024-05-18 14:06:50.000000 datapools-1.0.57/datapools/worker/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:06:59.144394 datapools-1.0.57/datapools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-18 14:06:59.000000 datapools-1.0.57/datapools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-05-18 14:06:59.000000 datapools-1.0.57/datapools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 14:06:59.000000 datapools-1.0.57/datapools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-18 14:06:59.000000 datapools-1.0.57/datapools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-18 14:06:59.000000 datapools-1.0.57/datapools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-18 14:06:59.000000 datapools-1.0.57/datapools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 14:06:59.148393 datapools-1.0.57/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-18 14:06:50.000000 datapools-1.0.57/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:06:59.144394 datapools-1.0.57/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 14:06:50.000000 datapools-1.0.57/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-18 14:06:50.000000 datapools-1.0.57/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-18 14:06:50.000000 datapools-1.0.57/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-18 14:06:50.000000 datapools-1.0.57/tests/test_session_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:04:22.659753 datapools-1.0.58/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-21 06:04:14.000000 datapools-1.0.58/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    19742 2024-05-21 06:04:14.000000 datapools-1.0.58/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7560 2024-05-21 06:04:14.000000 datapools-1.0.58/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-21 06:04:14.000000 datapools-1.0.58/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-21 06:04:22.659753 datapools-1.0.58/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-21 06:04:14.000000 datapools-1.0.58/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:04:22.647753 datapools-1.0.58/datapools/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:04:22.651753 datapools-1.0.58/datapools/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/common/backend_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/common/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:04:22.651753 datapools-1.0.58/datapools/common/queues/
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/common/queues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12022 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/common/queues/rabbitmq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/common/queues/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6661 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/common/session_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/common/stoppable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:04:22.651753 datapools-1.0.58/datapools/common/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/common/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/common/storage/base_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/common/storage/file_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:04:22.651753 datapools-1.0.58/datapools/common/tasks_db/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/common/tasks_db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/common/tasks_db/redis.py.bak
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/common/tasks_db/tasks_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9129 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/common/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:04:22.651753 datapools-1.0.58/datapools/producer/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/producer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6383 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/producer/base_producer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:04:22.651753 datapools-1.0.58/datapools/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12853 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/scheduler/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:04:22.655753 datapools-1.0.58/datapools/worker/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/worker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:04:22.655753 datapools-1.0.58/datapools/worker/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/worker/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11750 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/worker/plugins/base_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:04:22.655753 datapools-1.0.58/datapools/worker/plugins/dataphoenix_info/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/worker/plugins/dataphoenix_info/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6975 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/worker/plugins/dataphoenix_info/dataphoenix_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:04:22.655753 datapools-1.0.58/datapools/worker/plugins/default/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/worker/plugins/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7631 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/worker/plugins/default/default.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:04:22.655753 datapools-1.0.58/datapools/worker/plugins/deutsche_welle/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/worker/plugins/deutsche_welle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/worker/plugins/deutsche_welle/deutsche_welle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:04:22.655753 datapools-1.0.58/datapools/worker/plugins/freesound_org/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/worker/plugins/freesound_org/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6771 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/worker/plugins/freesound_org/freesound_org.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:04:22.655753 datapools-1.0.58/datapools/worker/plugins/google_drive/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/worker/plugins/google_drive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9695 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/worker/plugins/google_drive/google_drive.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:04:22.655753 datapools-1.0.58/datapools/worker/plugins/imageshack/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/worker/plugins/imageshack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/worker/plugins/imageshack/imageshack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:04:22.655753 datapools-1.0.58/datapools/worker/plugins/s3/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/worker/plugins/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5444 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/worker/plugins/s3/s3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:04:22.655753 datapools-1.0.58/datapools/worker/plugins/theguardian/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/worker/plugins/theguardian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/worker/plugins/theguardian/theguardian.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:04:22.659753 datapools-1.0.58/datapools/worker/plugins/washingtonpost/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/worker/plugins/washingtonpost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6649 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/worker/plugins/washingtonpost/washingtonpost.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:04:22.659753 datapools-1.0.58/datapools/worker/plugins/wikipedia/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/worker/plugins/wikipedia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7619 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/worker/plugins/wikipedia/wikipedia.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:04:22.659753 datapools-1.0.58/datapools/worker/plugins/youtube_channel/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/worker/plugins/youtube_channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10203 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/worker/plugins/youtube_channel/youtube_channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/worker/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/worker/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17785 2024-05-21 06:04:14.000000 datapools-1.0.58/datapools/worker/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:04:22.659753 datapools-1.0.58/datapools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-21 06:04:22.000000 datapools-1.0.58/datapools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-05-21 06:04:22.000000 datapools-1.0.58/datapools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 06:04:22.000000 datapools-1.0.58/datapools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-21 06:04:22.000000 datapools-1.0.58/datapools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-21 06:04:22.000000 datapools-1.0.58/datapools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-21 06:04:22.000000 datapools-1.0.58/datapools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 06:04:22.663753 datapools-1.0.58/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-21 06:04:14.000000 datapools-1.0.58/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:04:22.659753 datapools-1.0.58/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 06:04:14.000000 datapools-1.0.58/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-21 06:04:14.000000 datapools-1.0.58/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-21 06:04:14.000000 datapools-1.0.58/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-21 06:04:14.000000 datapools-1.0.58/tests/test_session_manager.py
```

### Comparing `datapools-1.0.57/HISTORY.md` & `datapools-1.0.58/HISTORY.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,24 @@
 Changelog
 =========
 
 
 (unreleased)
 ------------
+- Merge pull request #76 from torrentsai/sergpsu-async-redis. [S]
+
+  Async redis and thinner plugins
+- . [sergpsu]
+- . [sergpsu]
+- Async redis, thinner plugins. [sergpsu]
+
+
+1.0.57 (2024-05-18)
+-------------------
+- Release: version 1.0.57 🚀 [sergpsu]
 - Merge pull request #75 from torrentsai/sergpsu-session-updates. [S]
 
   last_reported_status
 - Last_reported_status. [sergpsu]
 - Merge pull request #74 from torrentsai/1.0.56. [S]
 
   1.0.56
```

### Comparing `datapools-1.0.57/LICENSE` & `datapools-1.0.58/LICENSE`

 * *Files identical despite different names*

### Comparing `datapools-1.0.57/PKG-INFO` & `datapools-1.0.58/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datapools
-Version: 1.0.57
+Version: 1.0.58
 Summary: Awesome datapools created by openlicenseai
 Home-page: https://github.com/openlicenseai/datapools/
 Author: openlicenseai
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydantic==2.6.1
 Requires-Dist: pydantic-settings==2.2.1
```

### Comparing `datapools-1.0.57/README.md` & `datapools-1.0.58/README.md`

 * *Files identical despite different names*

### Comparing `datapools-1.0.57/datapools/api.py` & `datapools-1.0.58/datapools/api.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.57/datapools/cli.py` & `datapools-1.0.58/datapools/cli.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.57/datapools/common/backend_api.py` & `datapools-1.0.58/datapools/common/backend_api.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.57/datapools/common/queues/__init__.py` & `datapools-1.0.58/datapools/common/queues/__init__.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.57/datapools/common/queues/rabbitmq.py` & `datapools-1.0.58/datapools/common/queues/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.57/datapools/common/queues/types.py` & `datapools-1.0.58/datapools/common/queues/types.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.57/datapools/common/session_manager.py` & `datapools-1.0.58/datapools/common/session_manager.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import time
 from enum import Enum
 from hashlib import md5
 from typing import List, Optional
 
-import redis
+from redis.asyncio import Redis, ConnectionError as RedisConnectionError
 
 from .logger import logger
 from .types import CrawlerHintURLStatus
 
 # from ..logger import logger
 
 SESSION_METADATA_KEY_PREFIX = "crawler_session_meta_"  # hash
@@ -18,21 +18,21 @@
 class SessionStatus(Enum):
     NORMAL = 0
     STOPPED = 1
 
 
 class Session:
     id: str
-    r: redis.Redis
+    r: Redis
     meta_key: str
     urls_key: str
     content_key: str
     stats_channel: str
 
-    def __init__(self, session_id, redis_inst: redis.Redis):
+    def __init__(self, session_id, redis_inst: Redis):
         self.id = session_id
         self.r = redis_inst
         self.meta_key = SessionManager.get_meta_key(self.id)
         self.urls_key = SessionManager.get_urls_key(self.id)
         self.content_key = SessionManager.get_content_key(self.id)
         self.stats_channel = Session.get_stats_channel(self.id)
 
@@ -44,102 +44,106 @@
     def get_stats_channel_mask():
         return Session.get_stats_channel("*")
 
     @staticmethod
     def get_session_id_by_channel(channel_name):
         return channel_name[14:]
 
-    def get_meta(self):
-        raw = self.r.hgetall(self.meta_key)
+    async def get_meta(self):
+        raw = await self.r.hgetall(self.meta_key)
         res = {
             "hint_id": raw[b"hint_id"].decode(),
             "url": raw[b"url"].decode(),
             "total_tasks": int(raw[b"total_tasks"]),
             "complete_tasks": int(raw[b"complete_tasks"]),
             "failed_tasks": int(raw[b"failed_tasks"]),
             "rejected_tasks": int(raw[b"rejected_tasks"]),
             "crawled_content": int(raw[b"crawled_content"]),
             "evaluated_content": int(raw[b"evaluated_content"]),
             "status": int(raw[b"status"] if b"status" in raw else SessionStatus.NORMAL.value),
         }
         return res
 
-    def set_status(self, status: SessionStatus):
-        self.r.hset(self.meta_key, "status", status.value)
-        self.r.publish(self.stats_channel, "status_change")
+    async def set_status(self, status: SessionStatus):
+        await self.r.hset(self.meta_key, "status", status.value)
+        await self.r.publish(self.stats_channel, "status_change")
 
-    def is_stopped(self):
-        status = self.r.hget(self.meta_key, "status")
+    async def is_stopped(self):
+        status = await self.r.hget(self.meta_key, "status")
         return status is not None and int(status) == SessionStatus.STOPPED.value
 
-    def add_url(self, url):
+    async def add_url(self, url):
         # urls are stored in sets
-        res = self.r.sadd(self.urls_key, url)
+        res = await self.r.sadd(self.urls_key, url)
         if res:
-            self.r.hincrby(self.meta_key, "total_tasks", 1)
+            await self.r.hincrby(self.meta_key, "total_tasks", 1)
         return res == 1
 
-    def has_url(self, url):
-        res = self.r.sismember(self.urls_key, url)
+    async def has_url(self, url):
+        res = await self.r.sismember(self.urls_key, url)
         # logger.info( f'has_url {res=} {type(res)=}')
         return res
 
-    def add_content(self, url):
-        return self.r.sadd(self.content_key, url)
+    async def add_content(self, url):
+        return await self.r.sadd(self.content_key, url)
 
-    def has_content(self, url):
-        return self.r.sismember(self.content_key, url)
+    async def has_content(self, url):
+        return await self.r.sismember(self.content_key, url)
 
-    def inc_complete_urls(self):
-        self.r.hincrby(self.meta_key, "complete_tasks", 1)
-        self.r.publish(self.stats_channel, "complete_tasks")
-
-    def inc_failed_urls(self):
-        self.r.hincrby(self.meta_key, "failed_tasks", 1)
-        self.r.publish(self.stats_channel, "failed_tasks")
-
-    def inc_rejected_urls(self):
-        self.r.hincrby(self.meta_key, "rejected_tasks", 1)
-        self.r.publish(self.stats_channel, "rejected_tasks")
-
-    def inc_crawled_content(self):
-        self.r.hincrby(self.meta_key, "crawled_content", 1)
-        self.r.publish(self.stats_channel, "crawled_content")
-
-    def inc_evaluated_content(self):
-        self.r.hincrby(self.meta_key, "evaluated_content", 1)
-        self.r.publish(self.stats_channel, "evaluated_content")
+    async def inc_complete_urls(self):
+        await self.r.hincrby(self.meta_key, "complete_tasks", 1)
+        await self.r.publish(self.stats_channel, "complete_tasks")
+
+    async def inc_failed_urls(self):
+        await self.r.hincrby(self.meta_key, "failed_tasks", 1)
+        await self.r.publish(self.stats_channel, "failed_tasks")
+
+    async def inc_rejected_urls(self):
+        await self.r.hincrby(self.meta_key, "rejected_tasks", 1)
+        await self.r.publish(self.stats_channel, "rejected_tasks")
+
+    async def inc_crawled_content(self):
+        await self.r.hincrby(self.meta_key, "crawled_content", 1)
+        await self.r.publish(self.stats_channel, "crawled_content")
+
+    async def inc_evaluated_content(self):
+        await self.r.hincrby(self.meta_key, "evaluated_content", 1)
+        await self.r.publish(self.stats_channel, "evaluated_content")
 
-    def exists(self):
-        res = self.r.exists(self.meta_key)
+    async def exists(self):
+        res = await self.r.exists(self.meta_key)
         return res
 
-    def set_last_reported_status(self, status: CrawlerHintURLStatus):
-        self.r.hset(self.meta_key, "last_reported_status", status.value)
+    async def set_last_reported_status(self, status: CrawlerHintURLStatus):
+        await self.r.hset(self.meta_key, "last_reported_status", status.value)
 
-    def get_last_reported_status(self):
-        bres = self.r.hget(self.meta_key, "last_reported_status")
+    async def get_last_reported_status(self):
+        bres = await self.r.hget(self.meta_key, "last_reported_status")
         if bres is not None:
             return CrawlerHintURLStatus(int(bres.decode()))
 
 
 class SessionManager:
-    def __init__(self, host, port=6379, db=0, protocol=3):
-        self.r = redis.Redis(host=host, port=port, db=db, protocol=protocol)
+    def __init__(self, host, port=6379, db=0):
+        self.r = Redis(host=host, port=port, db=db)
 
-    def is_ready(self) -> bool:
+    async def stop(self):
+        await self.r.connection_pool.aclose()
+        del self.r
+
+    async def is_ready(self) -> bool:
         try:
-            self.r.ping()
+            await self.r.ping()
             return True
-        except redis.exceptions.ConnectionError:
+        except RedisConnectionError:
             return False
 
-    def create(self, hint_id=0, url="") -> Session:
+    async def create(self, hint_id=0, url="") -> Session:
         session_id = self.gen_session_id()
-        self.r.hset(
+        await self.r.hset(
             SessionManager.get_meta_key(session_id),
             mapping={
                 "hint_id": hint_id,
                 "url": url,
                 "total_tasks": 0,
                 "complete_tasks": 0,
                 "failed_tasks": 0,
@@ -148,26 +152,28 @@
                 "evaluated_content": 0,
                 "status": SessionStatus.NORMAL.value,
             },
         )
         # logger.info( f'hset result {r=} {type(r)=}')
         return Session(session_id, self.r)
 
-    def has(self, session_id) -> bool:
-        res = self.r.exists(SessionManager.get_meta_key(session_id))
+    async def has(self, session_id) -> bool:
+        res = await self.r.exists(SessionManager.get_meta_key(session_id))
         # logger.info( f'sessionmanager.has {res=} {type(res)=}')
         return res
 
-    def get(self, session_id) -> Optional[Session]:
-        return Session(session_id, self.r) if self.has(session_id) else None
-
-    def remove(self, session_id):
-        self.r.delete(SessionManager.get_meta_key(session_id))
-        self.r.delete(SessionManager.get_urls_key(session_id))
-        self.r.delete(SessionManager.get_content_key(session_id))
+    async def get(self, session_id) -> Optional[Session]:
+        if await self.has(session_id):
+            return Session(session_id, self.r)
+        return None
+
+    async def remove(self, session_id):
+        await self.r.delete(SessionManager.get_meta_key(session_id))
+        await self.r.delete(SessionManager.get_urls_key(session_id))
+        await self.r.delete(SessionManager.get_content_key(session_id))
 
     def gen_session_id(self) -> str:
         # TODO: add existance check
         return md5(str(time.time()).encode()).hexdigest()
 
     @staticmethod
     def get_meta_key(session_id):
@@ -177,13 +183,13 @@
     def get_urls_key(session_id):
         return f"{SESSION_URLS_KEY_PREFIX}{session_id}"
 
     @staticmethod
     def get_content_key(session_id):
         return f"{SESSION_CONTENT_KEY_PREFIX}{session_id}"
 
-    def get_ids(self, limit) -> List[str]:
-        keys = self.r.keys(f"{SESSION_METADATA_KEY_PREFIX}*")
+    async def get_ids(self, limit) -> List[str]:
+        keys = await self.r.keys(f"{SESSION_METADATA_KEY_PREFIX}*")
         if len(keys) > limit:
             keys = keys[0:limit]
         n = len(SESSION_METADATA_KEY_PREFIX)
         return [k[n:] for k in keys]
```

### Comparing `datapools-1.0.57/datapools/common/stoppable.py` & `datapools-1.0.58/datapools/common/stoppable.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.57/datapools/common/storage/base_storage.py` & `datapools-1.0.58/datapools/common/storage/base_storage.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,10 +15,9 @@
     async def remove(self, storage_id):
         raise Exception("implement remove()")
 
     @abstractmethod
     async def has(self, storage_id):
         raise Exception("implement has()")
 
-    @staticmethod
-    def gen_id(data):
+    def gen_id(self, data):
         return md5(data.encode()).hexdigest()
```

### Comparing `datapools-1.0.57/datapools/common/storage/file_storage.py` & `datapools-1.0.58/datapools/common/storage/file_storage.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 import os
 
 from ..logger import logger
 from .base_storage import BaseStorage
 
 
 class FileStorage(BaseStorage):
-    def __init__(self, dst_path):
+    def __init__(self, dst_path, must_exist=False):
+        if must_exist is False:
+            os.makedirs(dst_path, exist_ok=True)
+        else:
+            if not os.path.exists(dst_path):
+                raise FileNotFoundError()
         self.dst_path = dst_path
 
     async def put(self, storage_id, content):
         with open(self.get_path(storage_id), "wb") as f:
             if type(content) is str:
                 content = content.encode()
             f.write(content)
```

### Comparing `datapools-1.0.57/datapools/common/tasks_db/redis.py.bak` & `datapools-1.0.58/datapools/common/tasks_db/redis.py.bak`

 * *Files identical despite different names*

### Comparing `datapools-1.0.57/datapools/common/tasks_db/tasks_db.py` & `datapools-1.0.58/datapools/common/tasks_db/tasks_db.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.57/datapools/common/types.py` & `datapools-1.0.58/datapools/common/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from abc import abstractmethod
 from enum import Enum, IntEnum
 from typing import Any, List, NamedTuple, Optional, TypeAlias, Union
 
 from pydantic import AnyUrl, BaseModel
 from pydantic_settings import BaseSettings
 
-from .storage import FileStorage
+# from .storage import FileStorage
 
 DEFAULT_QUEUE_WORKER_TASKS = "worker_tasks"
 DEFAULT_QUEUE_REPORTS = "worker_reports"
 DEFAULT_QUEUE_EVAL_TASKS = "eval_tasks"
 DEFAULT_QUEUE_TOPICS = "topics"
 
 DEFAULT_RABBITMQ_HOST = "rabbitmq.openlicense"
@@ -250,17 +250,18 @@
     tag_id: Optional[str] = None
     tag_keepout: Optional[bool] = False
     copyright_tag_id: Optional[str] = None
     copyright_tag_keepout: Optional[bool] = False
     platform_tag_id: Optional[str] = None
     platform_tag_keepout: Optional[bool] = False
     type: DatapoolContentType
-    storage_id: Any
+    # storage_id: Any
     url: Union[str, AnyUrl]
     priority_timestamp: Optional[int] = None
+    content: Optional[Any] = None
 
     def to_dict(self):
         res = self.__dict__
         res["type"] = res["type"].value
         return res
```

### Comparing `datapools-1.0.57/datapools/producer/base_producer.py` & `datapools-1.0.58/datapools/producer/base_producer.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from ..common.logger import logger
 from ..common.queues import GenericQueue, QueueMessage, QueueMessageType, QueueRole, QueueTopicMessage
 from ..common.session_manager import SessionManager, Session
 from ..common.stoppable import Stoppable
 from ..common.storage.file_storage import FileStorage
 from ..common.types import BaseProducerSettings, InvalidUsageException
 from ..worker.utils import get_storage_invalidation_topic
+from ..worker.worker import WorkerFileStorage
 
 # from .rules import DatapoolRulesChecker
 
 
 class BaseProducer(Stoppable):
     def __init__(self, cfg: Optional[BaseProducerSettings] = None):
         super().__init__()
@@ -82,27 +83,27 @@
     async def router_loop(self):
         try:
             while not await self.is_stopped():
                 message = await self.eval_queue.pop(timeout=1)
                 if message:
                     qm = QueueMessage.decode(message.body)
                     try:
-                        session = self.session_manager.get(qm.session_id)
-                        if session is None or session.is_stopped():
+                        session = await self.session_manager.get(qm.session_id)
+                        if session is None or await session.is_stopped():
                             logger.info(f"session is deleted or stopped {qm.session_id=} {message.message_id}")
                             await self.eval_queue.mark_done(message)
                             continue
 
                         if qm.type == QueueMessageType.Task:
                             task = qm.data
                             logger.info(f"Producer got: {task}")
 
                             # TODO: this storage must be associated with the worker!
                             #   For example, storage path or url can be formatted accordingly to worker id
-                            worker_storage = FileStorage(self.cfg.WORKER_STORAGE_PATH)
+                            worker_storage = WorkerFileStorage(self.cfg.WORKER_STORAGE_PATH, task["worker_id"])
                             raw_data = await worker_storage.get(task["storage_id"])
                             await self.process_content(session, raw_data, task)
 
                             if not self.is_shared_storage():
                                 # tell worker that his storage item can be removed
                                 await self.topics_queue.push(
                                     QueueTopicMessage(
@@ -137,12 +138,12 @@
             path = self.cfg.STORAGE_PATH
             if not os.path.exists(path):  # type: ignore
                 os.mkdir(path)  # type: ignore
             storage = FileStorage(path)
             # put data into persistent storage
             await storage.put(task["storage_id"], raw_data)
 
-        if session.exists():  # session may have been deleted while processing content
-            session.inc_evaluated_content()
+        if await session.exists():  # session may have been deleted while processing content
+            await session.inc_evaluated_content()
 
     def is_shared_storage(self):
         return self.cfg.STORAGE_PATH is None or self.cfg.WORKER_STORAGE_PATH == self.cfg.STORAGE_PATH
```

### Comparing `datapools-1.0.57/datapools/scheduler/scheduler.py` & `datapools-1.0.58/datapools/scheduler/scheduler.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,17 +58,14 @@
             role=QueueRole.Receiver,
             url=self.cfg.QUEUE_CONNECTION_URL,
             name=self.cfg.WORKER_REPORTS_QUEUE_NAME,
         )
         logger.info("created receiver reports")
 
         if self.cfg.CLI_MODE:
-            self.cli_session = self.session_manager.create()
-            logger.info(f"created session {self.cli_session.id}")
-
             # TODO: this mechanism will not work for multiple workers/producers
             self.stop_task_processed = asyncio.Event()
 
     async def wait(self):
         """for CLI mode usage only"""
         if not self.cfg.CLI_MODE:
             logger.error("scheduler invalid usage")
@@ -99,44 +96,44 @@
         await super().stop()
         logger.info("super stopped")
 
     async def _set_task_status(self, session_id, data):
         # hash, status: CrawlerHintURLStatus, contents
         logger.info(f"set_task_status: {session_id=} {data=}")
 
-        session = self.session_manager.get(session_id)
+        session = await self.session_manager.get(session_id)
         if session is None:
             return False
 
-        meta = session.get_meta()
+        meta = await session.get_meta()
         logger.info(f"{meta=}")
         if not meta:
             return False
 
         status = CrawlerHintURLStatus(data["status"])
 
         if status in (CrawlerHintURLStatus.Success, CrawlerHintURLStatus.Failure, CrawlerHintURLStatus.Rejected):
             if status == CrawlerHintURLStatus.Success:
-                session.inc_complete_urls()
+                await session.inc_complete_urls()
             elif status == CrawlerHintURLStatus.Failure:
-                session.inc_failed_urls()
+                await session.inc_failed_urls()
             else:
-                session.inc_rejected_urls()
+                await session.inc_rejected_urls()
 
-            last_reported_status = session.get_last_reported_status()
+            last_reported_status = await session.get_last_reported_status()
             if last_reported_status == CrawlerHintURLStatus.Processing:  # make sure that report is sent once only
                 logger.info(f'COMPLETE: {meta["complete_tasks"]} vs MAX: {self.cfg.MAX_COMPLETE_TASKS}')
                 need_hard_stop = (
-                    not session.is_stopped()
+                    not await session.is_stopped()
                     and self.cfg.MAX_COMPLETE_TASKS is not None
                     and meta["complete_tasks"] >= self.cfg.MAX_COMPLETE_TASKS
                 )
                 if need_hard_stop:
                     logger.info(f"HARD STOP {session_id}")
-                    session.set_status(SessionStatus.STOPPED)
+                    await session.set_status(SessionStatus.STOPPED)
 
                 if (
                     (
                         meta["total_tasks"]
                         == meta["complete_tasks"] + meta["failed_tasks"] + meta["rejected_tasks"] + 1
                         or need_hard_stop
                     )
@@ -147,30 +144,26 @@
                     if not self.cfg.CLI_MODE:
                         await self._set_hint_url_status(meta["hint_id"], status, session)
             else:
                 logger.info(f"hint status report was already sent: {last_reported_status=}")
 
     async def _set_hint_url_status(self, hint_id, status: CrawlerHintURLStatus, session: Session):
         await self.api.set_hint_url_status(hint_id, status, session.id)
-        session.set_last_reported_status(status)
+        await session.set_last_reported_status(status)
 
     async def _add_task(self, session_id, task: dict):
-        if not self.session_manager.has(session_id):
-            logger.error(f"Session not found: {session_id=}")
-            return False
-
-        session = self.session_manager.get(session_id)
-        if session is None or session.is_stopped():
-            logger.info(f"Session is stopped {session_id=}")
+        session = await self.session_manager.get(session_id)
+        if session is None or await session.is_stopped():
+            logger.info(f"Session not found or is stopped {session_id=}")
             return False
 
         if "url" in task:
             # logger.info( f'{task["url"]=}')
-            if not session.has_url(task["url"]):
-                session.add_url(task["url"])
+            if not await session.has_url(task["url"]):
+                await session.add_url(task["url"])
 
                 await self.todo_queue.push(QueueMessage(session_id, QueueMessageType.Task, data=task))
             else:
                 # logger.info('task exists, ignored')
                 return False
         elif "stop_running" in task:
             await self.todo_queue.push(QueueMessage(session_id, QueueMessageType.Stop))
@@ -193,15 +186,15 @@
     async def _get_hints(self):
         hints = None
         if not self.cfg.CLI_MODE:
             # deployment mode
             try:
                 hints = await self.api.get_hint_urls(limit=10)
                 for hint in hints:
-                    session = self.session_manager.create(hint_id=hint.get("id", 0), url=hint.get("url", ""))
+                    session = await self.session_manager.create(hint_id=hint.get("id", 0), url=hint.get("url", ""))
                     hint["session_id"] = session.id
 
             except Exception as e:
                 logger.error(f"Failed get hints: {e}")
         else:
             # cli mode
             try:
@@ -212,39 +205,44 @@
                     hints = [{"stop_running": True, "session_id": self.cli_session.id}]
             except asyncio.TimeoutError:
                 pass
         return hints
 
     async def hints_loop(self):
         # infinitely fetching URL hints by calling backend api
+
+        if self.cfg.CLI_MODE:
+            self.cli_session = await self.session_manager.create()
+            logger.info(f"created session {self.cli_session.id}")
+
         try:
             while not await self.is_stopped():
-                if self.session_manager.is_ready():
+                if await self.session_manager.is_ready():
                     hints = await self._get_hints()
                     if hints is not None:
                         for hint in hints:
                             logger.info(f"got hint: {hint}")
 
                             added = await self._add_task(hint.get("session_id"), hint)
                             # catching set_hint_url_status BackendAPIException: if backend fails then trying again and again
                             while not await self.is_stopped():
                                 try:
-                                    session = self.session_manager.get(hint["session_id"])
+                                    session = await self.session_manager.get(hint["session_id"])
                                     if added:
                                         if "id" in hint:
                                             await self._set_hint_url_status(
                                                 hint["id"], CrawlerHintURLStatus.Processing, session
                                             )
                                     else:
                                         logger.error("failed add task, REJECTING")
                                         if "id" in hint:
                                             await self._set_hint_url_status(
                                                 hint["id"], CrawlerHintURLStatus.Rejected, session
                                             )
-                                            self.session_manager.remove(hint["session_id"])
+                                            await self.session_manager.remove(hint["session_id"])
                                     break
                                 except BackendAPIException as e:
                                     logger.error("Catched BackendAPIException")
                                     logger.error(traceback.format_exc())
                                     await asyncio.sleep(5)
                                     # ..and loop again
                     if not self.cfg.CLI_MODE:
```

### Comparing `datapools-1.0.57/datapools/worker/plugins/base_plugin.py` & `datapools-1.0.58/datapools/worker/plugins/base_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,30 +134,14 @@
             async with httpx.AsyncClient(max_redirects=max_redirects) as client:
                 r = await client.get(url, follow_redirects=follow_redirects, headers=headers)
                 return r.content
 
         except Exception as e:
             logger.error(f"failed get content of {url}: {e}")
 
-    async def download_content(self, url, content_type: DatapoolContentType):
-        storage_id = BaseStorage.gen_id(url)
-
-        if not await self.is_content_processed(url):
-            content = await self.download(url)
-            if content:
-                logger.info(f"putting to {storage_id=}")
-                await self.ctx.storage.put(storage_id, content)
-
-                return CrawlerContent(
-                    type=content_type,
-                    storage_id=storage_id,
-                    url=url,
-                )
-        return CrawlerNop()
-
     @staticmethod
     def parse_url(url):
         return urlparse(url)
 
     @staticmethod
     @abstractmethod
     def is_supported(url):
@@ -315,15 +299,15 @@
             else:
                 # check if <meta/> tag exists with our tag
                 header_tag = await BasePlugin.parse_meta_tag(content, meta_name)
                 self.platform_tag_cache.set(header_tag)
         return self.platform_tag_cache.get()
 
     async def is_content_processed(self, url):
-        if self.ctx.session.has_content(url):
+        if await self.ctx.session.has_content(url):
             logger.info("content was processed already")
             return True
         return False
 
     @staticmethod
     async def get_webpage_image_bytes(img_locator):
         """for playwright only"""
```

### Comparing `datapools-1.0.57/datapools/worker/plugins/dataphoenix_info/dataphoenix_info.py` & `datapools-1.0.58/datapools/worker/plugins/dataphoenix_info/dataphoenix_info.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 
 # from bs4 import BeautifulSoup
 # from playwright.async_api import Locator, Page
 from playwright.async_api import TimeoutError as PlaywriteTimeoutError
 from playwright.async_api import async_playwright, expect
 
 from ....common.logger import logger
-from ....common.storage import BaseStorage
+
+# from ....common.storage import BaseStorage
 from ....common.types import CrawlerBackTask, CrawlerContent, CrawlerNop, DatapoolContentType
 from ..base_plugin import BasePlugin
 from ...worker import WorkerTask
 
 # import traceback
 
 
@@ -84,25 +85,26 @@
             excerpt = ""
 
         body = ""
         ps = await self.page.locator("section.c-content > p").all()
         for p in ps:
             body += await p.inner_text() + "\n"
 
-        storage_id = BaseStorage.gen_id(url)
-        logger.info(f"putting article into {storage_id=}")
+        # storage_id = self.ctx.storage.gen_id(url)
+        # logger.info(f"putting article into {storage_id=}")
 
-        await self.ctx.storage.put(storage_id, BasePlugin.make_text_storage_value(body, header=header, excerpt=excerpt))
+        # await self.ctx.storage.put(storage_id, BasePlugin.make_text_storage_value(body, header=header, excerpt=excerpt))
 
         yield CrawlerContent(
             tag_id=str(self.header_tag_id),
             tag_keepout=self.header_tag_id.is_keepout(),
             type=DatapoolContentType.Text,
-            storage_id=storage_id,
+            # storage_id=storage_id,
             url=url,
+            content=BasePlugin.make_text_storage_value(body, header=header, excerpt=excerpt),
         )
 
     async def _process_feed(self, url):
         total_news = 0
         while True:
             # logger.info( 'scrolling  to bottom')
             # await self.page.evaluate("window.scrollTo(0, document.body.scrollHeight)")
```

### Comparing `datapools-1.0.57/datapools/worker/plugins/default/default.py` & `datapools-1.0.58/datapools/worker/plugins/default/default.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,49 +1,56 @@
 import asyncio
-import traceback
+
+# import traceback
 
 # import time
 from playwright.async_api import TimeoutError as PlaywriteTimeoutError
 from playwright.async_api import async_playwright
 
 from ....common.logger import logger
-from ....common.storage import BaseStorage
+
+# from ....common.storage import BaseStorage
 from ....common.types import CrawlerBackTask, CrawlerContent, DatapoolContentType
 from ...utils import canonicalize_url
 from ..base_plugin import BasePlugin
 from ...worker import WorkerTask
 
 
 class DefaultPlugin(BasePlugin):
-    def __init__(self, ctx):
-        super().__init__(ctx)
+    # def __init__(self, ctx):
+    #     super().__init__(ctx)
 
     @staticmethod
     def is_supported(url):
         u = BasePlugin.parse_url(url)
         return u.scheme in ("https", "http")
 
     async def process(self, task: WorkerTask):
         logger.info(f"BasePlugin::process({task.url})")
 
         if task.content_type in (DatapoolContentType.Image, DatapoolContentType.Video, DatapoolContentType.Audio):
-            yield await self.download_content(task.url, task.content_type)
+            # simply let worker to download and process content
+            yield CrawlerContent(
+                type=task.content_type,
+                # storage_id=storage_id,
+                url=task.url,
+            )
             return
 
         async with async_playwright() as playwright:
             webkit = playwright.chromium
             browser = await webkit.launch()
             viewport_height = 1024
             context = await browser.new_context(viewport={"width": 1920, "height": viewport_height})
 
             page = await context.new_page()
             await page.goto(str(task.url))
 
             real_url = page.url
-            session_meta = self.ctx.session.get_meta()
+            session_meta = await self.ctx.session.get_meta()
             if not self.get_local_url(real_url, session_meta["url"]):
                 logger.info("redirected to different domain")
                 return
 
             url = real_url
 
             p = BasePlugin.parse_url(url)
@@ -94,56 +101,34 @@
                             logger.info("--------------------------------------")
                             outerHTML = await images[n_images - 1].evaluate("el => el.outerHTML")
                             logger.info(f"{outerHTML=}")
                             continue
 
                         full_local_url = BasePlugin.get_local_url(src, session_meta["url"])
                         if full_local_url:
-                            logger.info(full_local_url)
-                            if await self.is_content_processed(full_local_url):
-                                continue
-
-                            storage_id = BaseStorage.gen_id(full_local_url)
-
                             # TODO: getting image from browser works somehow but
                             #   requires image type detection, quality check, crossOrigin understading etc
                             #   So for now let's do not in optimal way
-                            content = await self.download(full_local_url)
+                            # content = await self.download(full_local_url)
                             # getting content from browser page instead of downloading it again
                             # content = await BasePlugin.get_webpage_image_bytes(images[n_images-1])
-                            if content:
-                                image_tag = BasePlugin.parse_image_tag(content)
+                            # if content:
+                            # TODO: parse copyright_tag_id somehow?
 
-                                # TODO: parse copyright_tag_id somehow?
-                                if image_tag is None and platform_tag is None:
-                                    logger.info("no tag available")
-                                    continue
-
-                                try:
-                                    logger.info(f"putting to {storage_id=}")
-                                    await self.ctx.storage.put(storage_id, content)
-
-                                    yield CrawlerContent(
-                                        tag_id=str(image_tag) if image_tag is not None else None,
-                                        tag_keepout=image_tag.is_keepout() if image_tag is not None else False,
-                                        platform_tag_id=str(platform_tag) if platform_tag is not None else None,
-                                        platform_tag_keepout=(
-                                            platform_tag.is_keepout() if platform_tag is not None else None
-                                        ),
-                                        type=DatapoolContentType.Image,
-                                        storage_id=storage_id,
-                                        url=full_local_url,
-                                    )
-                                except Exception as e:
-                                    logger.error(f"failed put to storage {e}")
-                                    logger.error(traceback.format_exc())
+                            yield CrawlerContent(
+                                platform_tag_id=str(platform_tag) if platform_tag is not None else None,
+                                platform_tag_keepout=(platform_tag.is_keepout() if platform_tag is not None else None),
+                                type=DatapoolContentType.Image,
+                                # storage_id=storage_id,
+                                url=full_local_url,
+                            )
                         else:
                             logger.info(f'non local: {src=} {session_meta["url"]=}')
 
-                    except PlaywriteTimeoutError as e:
+                    except PlaywriteTimeoutError:
                         # element may be not ready yet, no problems, will get it on the next iteration
                         # logger.info( 'get_attribute timeout' )
                         expect_changes = True
                         break
 
                 # 3. hrefs
                 hrefs = await page.locator("a").all()
@@ -165,15 +150,15 @@
 
                             # logger.info( f'---------yielding {video_url=}')
                             yield CrawlerBackTask(url=full_local_url)
                             # logger.info( f'---------yielded {video_url=}')
                         else:
                             logger.info(f'non local: {href=} {session_meta["url"]=}')
 
-                    except PlaywriteTimeoutError as e:
+                    except PlaywriteTimeoutError:
                         # element may be not ready yet, no problems, will get it on the next iteration
                         # logger.info( 'get_attribute timeout' )
                         expect_changes = True
                         break
 
                 scroll_height1 = await page.evaluate("document.body.scrollHeight")
                 await page.mouse.wheel(0, viewport_height * 0.8)
```

### Comparing `datapools-1.0.57/datapools/worker/plugins/deutsche_welle/deutsche_welle.py` & `datapools-1.0.58/datapools/worker/plugins/deutsche_welle/deutsche_welle.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 from urllib.parse import urlparse, urlunparse
 
 import requests
 from bs4 import BeautifulSoup, Comment
 from html2text import HTML2Text
 
 from ....common.logger import logger
-from ....common.storage import BaseStorage
+
+# from ....common.storage import BaseStorage
 from ....common.types import CrawlerBackTask, CrawlerContent, DatapoolContentType
 from ...utils import canonicalize_url
 from ..base_plugin import BasePlugin, BaseTag
 
 DOMAIN = "www.dw.com"
 
 
@@ -28,26 +29,26 @@
         u = BasePlugin.parse_url(url)
         # logger.info( f'dw.is_supported {url=} {u.netloc=} {DOMAIN=}')
         return u.netloc == DOMAIN
 
     def is_article(self, url):
         path = urlparse(url).path
         pattern = "^/en/.+/a-\d+/$"
-        return True  # bool(re.match(pattern, path))
+        return bool(re.match(pattern, path))
 
     def normalize(self, url):
         parts = list(urlparse(url))
         parts[5] = ""  # remove fragment
         clean_url = urlunparse(parts)
         return clean_url
 
     def extract(self, soup):
         content = soup.find("article")
         if not content:
-            logger.debug(f"No <article>. Skipped.")
+            logger.debug("No <article>. Skipped.")
             return None
 
         # remove ads
         for element in content.find_all("div"):
             for v in element.attrs.values():
                 if "advertisement" in v:
                     element.extract()
@@ -101,38 +102,39 @@
         soup = BeautifulSoup(response.content, "html.parser")
 
         if not self.demo_tag.is_valid():
             platform_tag = await self.get_platform_tag(DOMAIN, soup, 3600)
         else:
             platform_tag = self.demo_tag
 
-        logger.debug(f"Adding new links...")
+        logger.debug("Adding new links...")
         for link in soup.find_all("a", href=True):
             href = link["href"]
             # next_url = urljoin(url, href)
             # next_url = self.normalize(next_url)
 
             full_local_url = BasePlugin.get_local_url(href, url)
             if full_local_url:
                 full_local_url = canonicalize_url(full_local_url)
                 logger.info(full_local_url)
                 yield CrawlerBackTask(url=full_local_url)
 
         if self.is_article(url):
             content = self.extract(soup)
             if content:
-                storage_id = BaseStorage.gen_id(url)
-                logger.info(f"putting article into {storage_id=}")
+                # storage_id = self.ctx.storage.gen_id(url)
+                # logger.info(f"putting article into {storage_id=}")
 
-                await self.ctx.storage.put(
-                    storage_id,
-                    BasePlugin.make_text_storage_value(content),
-                )
+                # await self.ctx.storage.put(
+                #     storage_id,
+                #     BasePlugin.make_text_storage_value(content),
+                # )
                 yield CrawlerContent(
                     platform_tag_id=str(platform_tag) if platform_tag is not None else None,
                     platform_keepout=platform_tag.is_keepout() if platform_tag is not None else None,
                     type=DatapoolContentType.Text,
-                    storage_id=storage_id,
+                    # storage_id=storage_id,
                     url=url,
+                    content=BasePlugin.make_text_storage_value(content),
                 )
             else:
                 logger.info("NO CONTENT")
```

### Comparing `datapools-1.0.57/datapools/worker/plugins/freesound_org/freesound_org.py` & `datapools-1.0.58/datapools/worker/plugins/freesound_org/freesound_org.py`

 * *Files 12% similar despite different names*

```diff
@@ -39,27 +39,27 @@
             await page.goto(str(task.url))
 
             if not self.demo_tag.is_valid():
                 platform_tag = await self.get_platform_tag(DOMAIN, page, 3600)
             else:
                 platform_tag = self.demo_tag
 
-            session_meta = self.ctx.session.get_meta()
+            session_meta = await self.ctx.session.get_meta()
             logger.info(f"{session_meta=}")
 
             logger.debug(f"Adding new links...")
             links = await page.locator("a").all()
             for link in links:
                 href = await link.get_attribute("href")
                 if href is None:
                     continue
                 full_local_url = BasePlugin.get_local_url(href, session_meta["url"])
                 if full_local_url:
                     full_local_url = canonicalize_url(full_local_url)
-                    if self.is_supported(full_local_url) and not self.ctx.session.has_url(full_local_url):
+                    if self.is_supported(full_local_url) and not await self.ctx.session.has_url(full_local_url):
                         logger.info(full_local_url)
                         yield CrawlerBackTask(url=full_local_url)
 
             sounds = await page.locator(".bw-search__result").all()
             for sound in sounds:
 
                 copyright_owner_tag = None
@@ -117,45 +117,25 @@
                 # downloading audio content
                 player = sound.locator(".bw-player").first
                 mp3_url = await player.get_attribute("data-mp3")  # TODO: also ogg available as "data-ogg"
 
                 full_mp3_url = BasePlugin.get_local_url(mp3_url, session_meta["url"])
                 logger.info(full_mp3_url)
 
-                if await self.is_content_processed(full_mp3_url):
-                    logger.info(f"Already processed {full_mp3_url=}")
-                    continue
-
-                mp3 = await self.download(full_mp3_url)
-                if mp3 is None:
-                    logger.error(f"Failed load {full_mp3_url=}")
-                    continue
-
-                # put to storage and yield content
-                storage_id = BaseStorage.gen_id(full_mp3_url)
-                try:
-                    logger.info(f"putting to {storage_id=}")
-                    await self.ctx.storage.put(storage_id, mp3)
-
-                    yield CrawlerContent(
-                        copyright_tag_id=(str(copyright_owner_tag) if copyright_owner_tag is not None else None),
-                        copyright_tag_keepout=(
-                            copyright_owner_tag.is_keepout() if copyright_owner_tag is not None else False
-                        ),
-                        platform_tag_id=str(platform_tag) if platform_tag is not None else None,
-                        platform_tag_keepout=(platform_tag.is_keepout() if platform_tag is not None else False),
-                        type=DatapoolContentType.Audio,
-                        storage_id=storage_id,
-                        url=full_mp3_url,
-                        priority_timestamp=date,
-                    )
-
-                except Exception as e:
-                    logger.error(f"failed put to storage {e}")
-                    logger.error(traceback.format_exc())
+                yield CrawlerContent(
+                    copyright_tag_id=(str(copyright_owner_tag) if copyright_owner_tag is not None else None),
+                    copyright_tag_keepout=(
+                        copyright_owner_tag.is_keepout() if copyright_owner_tag is not None else False
+                    ),
+                    platform_tag_id=str(platform_tag) if platform_tag is not None else None,
+                    platform_tag_keepout=(platform_tag.is_keepout() if platform_tag is not None else False),
+                    type=DatapoolContentType.Audio,
+                    url=full_mp3_url,
+                    priority_timestamp=date,
+                )
 
     async def parse_user_profile(self, href, session_meta) -> Union[BaseTag, None]:
         username = href.split("/")[-2]
         if not BasePlugin.copyright_tags_cache.contains(username, 3600):
             # getting full profile url
             url = canonicalize_url(BasePlugin.get_local_url(href, session_meta["url"]))
```

### Comparing `datapools-1.0.57/datapools/worker/plugins/google_drive/google_drive.py` & `datapools-1.0.58/datapools/worker/plugins/google_drive/google_drive.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 
 # from google.auth.transport.requests import Request
 # from google.oauth2.credentials import Credentials
 # from google_auth_oauthlib.flow import InstalledAppFlow
 from googleapiclient.discovery import build
 
 from ....common.logger import logger
-from ....common.storage import BaseStorage
+
+# from ....common.storage import BaseStorage
 from ....common.types import CrawlerContent, DatapoolContentType, CrawlerDemoUser
 from ..base_plugin import BasePlugin, BasePluginException, BaseTag
 from ...worker import WorkerTask
 
 # from googleapiclient.http import MediaIoBaseDownload
 
 
@@ -212,25 +213,26 @@
 
                         author_tag = None
                         if datapool_content_type == DatapoolContentType.Image:
                             author_tag = BasePlugin.parse_image_tag(content)
 
                         # obj_url = f'https://drive.google.com/file/d/{file_id}/view'
                         obj_url = url
-                        storage_id = BaseStorage.gen_id(obj_url)
-                        await self.ctx.storage.put(storage_id, content)
+                        # storage_id = self.ctx.storage.gen_id(obj_url)
+                        # await self.ctx.storage.put(storage_id, content)
 
                         yield CrawlerContent(
                             tag_id=str(author_tag) if author_tag is not None else None,
                             tag_keepout=author_tag.is_keepout() if author_tag is not None else None,
                             copyright_tag_id=str(self.tag_id),
                             copyright_tag_keepout=self.tag_id.is_keepout(),
                             type=datapool_content_type,
-                            storage_id=storage_id,
+                            # storage_id=storage_id,
                             url=obj_url,
+                            content=content,
                         )
 
                 # baseImage = cv2.imdecode(np.fromstring(fhContents, dtype=np.uint8), cv2.IMREAD_COLOR)
             if page_token is None:
                 break
 
     def _match_structure_rules(self, path):
```

### Comparing `datapools-1.0.57/datapools/worker/plugins/imageshack/imageshack.py` & `datapools-1.0.58/datapools/worker/plugins/imageshack/imageshack.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import asyncio
-import traceback
+
+# import traceback
 from typing import Union
 
 # import httpx
 from bs4 import BeautifulSoup
 from playwright.async_api import TimeoutError as PlaywriteTimeoutError
 from playwright.async_api import async_playwright
 
 from ....common.logger import logger
-from ....common.storage import BaseStorage
+
+# from ....common.storage import BaseStorage
 from ....common.types import CrawlerBackTask, CrawlerContent, CrawlerDemoUser, DatapoolContentType
 from ...utils import canonicalize_url
 from ..base_plugin import BasePlugin, BaseTag
 from ...worker import WorkerTask
 
 # from typing import List
 
@@ -43,15 +45,15 @@
             await page.goto(str(task.url))
 
             if not self.demo_tag.is_valid():
                 platform_tag = await self.get_platform_tag(DOMAIN, page, 3600)
             else:
                 platform_tag = self.demo_tag
 
-            session_meta = self.ctx.session.get_meta()
+            session_meta = await self.ctx.session.get_meta()
 
             n_images = 0
             n_hrefs = 0
             expect_changes = True
             while expect_changes:
                 expect_changes = False
 
@@ -72,15 +74,15 @@
                             full_local_url = canonicalize_url(full_local_url)
                             logger.info(f"adding task: {full_local_url}")
 
                             yield CrawlerBackTask(url=full_local_url)
                         else:
                             logger.info(f'non local: {href=} {session_meta["url"]=}')
 
-                    except PlaywriteTimeoutError as __e:
+                    except PlaywriteTimeoutError:
                         # element may be not ready yet, no problems, will get it on the next iteration
                         # logger.info( 'get_attribute timeout' )
                         expect_changes = True
                         break
 
                 # 2. search for single photo IMAGE
                 images = await page.locator("img#lp-image").all()
@@ -101,16 +103,14 @@
                             continue
 
                         full_local_url = BasePlugin.get_local_url(src, session_meta["url"])
                         logger.info(full_local_url)
                         if await self.is_content_processed(full_local_url):
                             continue
 
-                        storage_id = BaseStorage.gen_id(full_local_url)
-
                         copyright_owner_tag = None
 
                         # check for user license on his public profile page
                         profile_link = await page.locator("a.profile-link").all()
                         if len(profile_link):
                             # profile_link['href'] = '/user/sergpsu' test
                             href = await profile_link[0].get_attribute("href")
@@ -134,53 +134,28 @@
 
                         if copyright_owner_tag is not None:
                             logger.info(f"found {copyright_owner_tag=}")
 
                         # TODO: getting image from browser works somehow but
                         #   requires image type detection, quality check, crossOrigin understading etc
                         #   So for now let's do not in optimal way
-                        content = await self.download(full_local_url)
+                        # content = await self.download(full_local_url)
                         # getting content from browser page instead of downloading it again
                         # content = await BasePlugin.get_webpage_image_bytes(images[n_images-1])
-                        if content:
-                            image_tag = BasePlugin.parse_image_tag(content)
-                            if image_tag is not None:
-                                logger.info(f"found image tag {image_tag=}")
-
-                            if image_tag is None and platform_tag is None and copyright_owner_tag is None:
-                                logger.info("no tag available")
-                                continue
-
-                            try:
-                                logger.info(f"putting to {storage_id=}")
-                                await self.ctx.storage.put(storage_id, content)
-
-                                yield CrawlerContent(
-                                    tag_id=str(image_tag) if image_tag is not None else None,
-                                    tag_keepout=image_tag.is_keepout() if image_tag is not None else False,
-                                    copyright_tag_id=(
-                                        str(copyright_owner_tag) if copyright_owner_tag is not None else None
-                                    ),
-                                    copyright_tag_keepout=(
-                                        copyright_owner_tag.is_keepout() if copyright_owner_tag is not None else False
-                                    ),
-                                    platform_tag_id=str(platform_tag) if platform_tag is not None else None,
-                                    platform_tag_keepout=(
-                                        platform_tag.is_keepout() if platform_tag is not None else False
-                                    ),
-                                    type=DatapoolContentType.Image,
-                                    storage_id=storage_id,
-                                    url=full_local_url,
-                                )
-
-                            except Exception as e:
-                                logger.error(f"failed put to storage {e}")
-                                logger.error(traceback.format_exc())
-                        else:
-                            logger.error("failed download image")
+                        # if content:
+                        yield CrawlerContent(
+                            copyright_tag_id=(str(copyright_owner_tag) if copyright_owner_tag is not None else None),
+                            copyright_tag_keepout=(
+                                copyright_owner_tag.is_keepout() if copyright_owner_tag is not None else False
+                            ),
+                            platform_tag_id=str(platform_tag) if platform_tag is not None else None,
+                            platform_tag_keepout=(platform_tag.is_keepout() if platform_tag is not None else False),
+                            type=DatapoolContentType.Image,
+                            url=full_local_url,
+                        )
 
                     except PlaywriteTimeoutError:
                         # element may be not ready yet, no problems, will get it on the next iteration
                         # logger.info( 'get_attribute timeout' )
                         expect_changes = True
                         break
```

### Comparing `datapools-1.0.57/datapools/worker/plugins/s3/s3.py` & `datapools-1.0.58/datapools/worker/plugins/s3/s3.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,38 +99,39 @@
                 # THIS IS PURE API ACCESS URL
                 obj_url = f"https://s3.console.aws.amazon.com/s3/buckets/{self.bucket_name}/{obj.key}"
             else:
                 # THIS IS DIRECT URL ( FOR PUBLIC BUCKETS )
                 # TODO: region?
                 obj_url = f"https://{self.bucket_name}.s3.amazonaws.com/{obj.key}"
 
-            storage_id = BaseStorage.gen_id(obj_url)
+            # storage_id = self.ctx.storage.gen_id(obj_url)
 
             content = self._download(obj.key)
 
             try:
                 content_type = self._get_datapool_content_type(content)
 
                 tag = None
                 if content_type == DatapoolContentType.Image:
                     tag = BasePlugin.parse_image_tag(content)
 
                 if tag is None and copyright_tag is None:
                     continue
 
-                await self.ctx.storage.put(storage_id, content)
+                # await self.ctx.storage.put(storage_id, content)
 
                 yield CrawlerContent(
                     tag_id=str(tag) if tag is not None else None,
                     tag_keepout=tag.is_keepout() if tag is not None else False,
                     copyright_tag_id=str(copyright_tag) if copyright_tag is not None else None,
                     copyright_tag_keepout=copyright_tag.is_keepout() if copyright_tag is not None else False,
                     type=content_type,
-                    storage_id=storage_id,
+                    # storage_id=storage_id,
                     url=obj_url,
+                    content=content,
                 )
             except S3Exception as e:
                 logger.info(f"mime type not supported/detected: {e}")
 
     def _download(self, key):
         with tempfile.NamedTemporaryFile() as tmp:
             self.s3_client.download_fileobj(self.bucket_name, key, tmp)
```

### Comparing `datapools-1.0.57/datapools/worker/plugins/theguardian/theguardian.py` & `datapools-1.0.58/datapools/worker/plugins/theguardian/theguardian.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 from urllib.parse import urlparse, urlunparse
 
 import requests
 from bs4 import BeautifulSoup, Comment
 from html2text import HTML2Text
 
 from ....common.logger import logger
-from ....common.storage import BaseStorage
+
+# from ....common.storage import BaseStorage
 from ....common.types import CrawlerBackTask, CrawlerContent, DatapoolContentType
 from ...utils import canonicalize_url
 from ..base_plugin import BasePlugin, BaseTag
 from ...worker import WorkerTask
 
 DOMAIN = "www.theguardian.com"
 
@@ -97,33 +98,34 @@
         soup = BeautifulSoup(response.content, "html.parser")
 
         if not self.demo_tag.is_valid():
             platform_tag = await self.get_platform_tag(DOMAIN, soup, 3600)
         else:
             platform_tag = self.demo_tag
 
-        logger.debug(f"Adding new links...")
+        logger.debug("Adding new links...")
         for link in soup.find_all("a", href=True):
             href = link["href"]
             full_local_url = BasePlugin.get_local_url(href, url)
             if full_local_url:
                 full_local_url = canonicalize_url(full_local_url)
                 logger.info(full_local_url)
                 yield CrawlerBackTask(url=full_local_url)
 
         if self.is_article(url):
             content = self.extract(soup)
             if content:
-                storage_id = BaseStorage.gen_id(url)
-                logger.info(f"putting article into {storage_id=}")
+                # storage_id = self.ctx.storage.gen_id(url)
+                # logger.info(f"putting article into {storage_id=}")
 
-                await self.ctx.storage.put(
-                    storage_id,
-                    BasePlugin.make_text_storage_value(content),
-                )
+                # await self.ctx.storage.put(
+                #     storage_id,
+                #     BasePlugin.make_text_storage_value(content),
+                # )
                 yield CrawlerContent(
                     platform_tag_id=str(platform_tag) if platform_tag is not None else None,
                     platform_tag_keepout=platform_tag.is_keepout() if platform_tag is not None else False,
                     type=DatapoolContentType.Text,
-                    storage_id=storage_id,
+                    # storage_id=storage_id,
                     url=url,
+                    content=BasePlugin.make_text_storage_value(content),
                 )
```

### Comparing `datapools-1.0.57/datapools/worker/plugins/washingtonpost/washingtonpost.py` & `datapools-1.0.58/datapools/worker/plugins/washingtonpost/washingtonpost.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 from urllib.parse import urlparse, urlunparse
 
 import requests
 from bs4 import BeautifulSoup, Comment
 from html2text import HTML2Text
 
 from ....common.logger import logger
-from ....common.storage import BaseStorage
+
+# from ....common.storage import BaseStorage
 from ....common.types import CrawlerBackTask, CrawlerContent, CrawlerDemoUser, DatapoolContentType
 from ...utils import canonicalize_url
 from ..base_plugin import BasePlugin, BaseTag, CachedPairs
 from ...worker import WorkerTask
 
 DOMAIN = "www.washingtonpost.com"
 
@@ -121,29 +122,30 @@
                 if self.demo_tag and user_name and author_tag and author_tag.is_valid():
                     yield CrawlerDemoUser(
                         user_name=user_name, short_tag_id=str(author_tag), platform="washingtonpost.com"
                     )
 
                 content = self.extract(soup)
                 if content:
-                    storage_id = BaseStorage.gen_id(url)
-                    logger.info(f"putting article into {storage_id=}")
+                    # storage_id = self.ctx.storage.gen_id(url)
+                    # logger.info(f"putting article into {storage_id=}")
 
-                    await self.ctx.storage.put(
-                        storage_id,
-                        BasePlugin.make_text_storage_value(content),
-                    )
+                    # await self.ctx.storage.put(
+                    #     storage_id,
+                    #     BasePlugin.make_text_storage_value(content),
+                    # )
                     yield CrawlerContent(
                         tag_id=str(author_tag) if author_tag is not None else None,
                         tag_keepout=author_tag.is_keepout() if author_tag is not None else False,
                         platform_tag_id=str(platform_tag) if platform_tag is not None else None,
                         platform_tag_keepout=platform_tag.is_keepout() if platform_tag is not None else False,
                         type=DatapoolContentType.Text,
-                        storage_id=storage_id,
+                        # storage_id=storage_id,
                         url=url,
+                        content=BasePlugin.make_text_storage_value(content),
                     )
 
     def _get_author_tag(self, soup, url):
         author_link = soup.find_all("a", attrs={"data-qa": "author-name"}, href=True)
         if len(author_link) > 0:
             logger.info(f"Author link {author_link} {author_link[0].text}")
             user_name = author_link[0].text
```

### Comparing `datapools-1.0.57/datapools/worker/plugins/wikipedia/wikipedia.py` & `datapools-1.0.58/datapools/worker/plugins/wikipedia/wikipedia.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Optional, Tuple
 
 from playwright.async_api import async_playwright, Page
 
 from ....common.logger import logger
-from ....common.storage import BaseStorage
+
+# from ....common.storage import BaseStorage
 from ....common.types import CrawlerContent, CrawlerDemoUser, DatapoolContentType
 from ..base_plugin import BasePlugin, BaseTag, CachedPairs
 from ...worker import WorkerTask
 
 
 class WikipediaPlugin(BasePlugin):
     users = CachedPairs()
@@ -54,45 +55,46 @@
                 history_url = await history_url_loc[0].get_attribute("href")
                 history_url = BasePlugin.get_local_url(history_url, task.url)
                 # TODO: shared ownership to be implemented later
                 #       for now use the creator of the article as the copyright owner.
                 #       Commented code below is more or less valid
                 # users = await self._collect_users(history_url)
                 # if len(users) > 0:
-                #     storage_id = BaseStorage.gen_id(task.url)
+                #     storage_id = self.ctx.storage.gen_id(task.url)
                 #     logger.info(f"putting article into {storage_id=}")
 
                 #     await self.ctx.storage.put(
                 #         storage_id,
                 #         json.dumps(
                 #             {"body": body_text, "users": users}
                 #         ),  # TODO: structure
                 #     )
 
                 # TODO: until shared ownership is not supported, we use creator of the article as the copyright owner
                 (creator_tag, user_name) = await self._get_article_creator(history_url)
                 if creator_tag or platform_tag:
-                    storage_id = BaseStorage.gen_id(task.url)
-                    logger.info(f"putting article into {storage_id=}")
+                    # storage_id = self.ctx.storage.gen_id(task.url)
+                    # logger.info(f"putting article into {storage_id=}")
 
-                    await self.ctx.storage.put(storage_id, BasePlugin.make_text_storage_value(body_text))
+                    # await self.ctx.storage.put(storage_id, BasePlugin.make_text_storage_value(body_text))
 
                     if self.demo_tag and user_name and creator_tag and creator_tag.is_valid():
                         yield CrawlerDemoUser(
                             user_name=user_name, short_tag_id=str(creator_tag), platform="wikipedia.org"
                         )
 
                     yield CrawlerContent(
                         platform_tag_id=str(platform_tag) if platform_tag is not None else None,
                         platform_tag_keepout=platform_tag.is_keepout() if platform_tag is not None else False,
                         tag_id=str(creator_tag) if creator_tag is not None else None,
                         tag_keepout=creator_tag.is_keepout() if creator_tag is not None else False,
                         type=DatapoolContentType.Text,
-                        storage_id=storage_id,
+                        # storage_id=storage_id,
                         url=task.url,
+                        content=BasePlugin.make_text_storage_value(body_text),
                     )
 
             # parsing links as back tasks
             async for yielded in self.parse_links(page):
                 yield yielded
 
     async def _get_article_creator(self, history_url) -> Tuple[Optional[BaseTag], Optional[str]]:
```

### Comparing `datapools-1.0.57/datapools/worker/plugins/youtube_channel/youtube_channel.py` & `datapools-1.0.58/datapools/worker/plugins/youtube_channel/youtube_channel.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import asyncio
 
 import os
 import time
 from http.client import HTTPException
 from threading import Thread
 from typing import Dict, Tuple, TypeAlias
+import tempfile
 
 from playwright.async_api import TimeoutError as PlaywriteTimeoutError
 from playwright.async_api import async_playwright
 from pytube import YouTube
 from pytube.exceptions import AgeRestrictedError as PytubeAgeRestrictedError
 
 from ....common.logger import logger
-from ....common.storage import BaseStorage
+
+# from ....common.storage import BaseStorage
 from ....common.types import CrawlerBackTask, CrawlerContent, CrawlerNop, DatapoolContentType
 from ..base_plugin import BasePlugin
 from ...worker import WorkerTask
 
 URL: TypeAlias = str
 TagID: TypeAlias = str
 Timestamp: TypeAlias = float
@@ -26,14 +28,15 @@
     CHANNEL_CACHE_TTL = 3600  # seconds
     channel_tag_cache: Dict[URL, Tuple[Timestamp, TagID]] = {}
     channel_cache_lock: Dict[URL, asyncio.Lock] = {}
     channel_cache_lock_protection = asyncio.Lock()
 
     def __init__(self, ctx):
         super().__init__(ctx)
+        self.tempdir = tempfile.gettempdir()
 
     @staticmethod
     def is_supported(url):
         u = BasePlugin.parse_url(url)
         # logger.info( f'dataphoenix.info {u=}')
         if u.netloc == "youtube.com" or u.netloc == "www.youtube.com":
             if u.path[0:2] == "/@":
@@ -93,33 +96,35 @@
             else:
                 raise Exception("not implemented")
 
             await page.close()
 
     async def download_content(self, url, type: DatapoolContentType):
         if not await self.is_content_processed(url):
-            storage_id = await self.download_video(url)
-            if storage_id:
+            content = await self.download_video(url)
+            if content:
                 return CrawlerContent(
                     type=type,
-                    storage_id=storage_id,
+                    # storage_id=storage_id,
                     url=url,
+                    content=content,
                 )
         return CrawlerNop()
 
     def _download_thread(self, url, storage_id, state: dict):
         logger.info(f"_download_thread: {url=} {storage_id=}")
 
         youtube = YouTube(url)
         state["tmp_path"] = None
         try:
             video = youtube.streams.filter(progressive=True, file_extension="mp4").order_by("resolution").first()
             for i in range(0, 3):
                 try:
-                    state["tmp_path"] = video.download(output_path="/tmp", filename=storage_id)
+                    tmpname = f"youtube_{time.time()}"
+                    state["tmp_path"] = video.download(output_path=self.tempdir, filename=tmpname)
                     break
 
                 except HTTPException as e:
                     logger.error(f"HTTPException {e}")
                     # will try to download again after delay
                     time.sleep(5)  # TODO: should be configurable
 
@@ -129,69 +134,69 @@
             # For now skip such videos
 
         logger.info(f"download done {storage_id=}")
         state["done"] = True
 
     async def _process_video(self, url, page, context):
         logger.info(f"_process_video {url=}")
-        await page.goto(url)
-        # logger.info(f"loaded {url=}")
-
-        # find channel name, then will search for tag there
-        channel_uri = page.locator("ytd-channel-name a:visible").filter(
-            has_not=page.get_by_role("link", name="ManageEngine", exact=True)
-        )
-        channel_uri = await channel_uri.get_attribute("href")
-        logger.info(f"{channel_uri=}")
-
-        page2 = await context.new_page()
-        tag = await self._get_channel_tag(channel_uri, page2)
-        await page2.close()
-        if tag is None:
-            return
+        if not await self.is_content_processed(url):
+            await page.goto(url)
+            # logger.info(f"loaded {url=}")
 
-        storage_id = await self.download_video(url)
-        if storage_id:
-            yield CrawlerContent(
-                tag_id=str(tag),
-                tag_keepout=tag.is_keepout(),
-                type=DatapoolContentType.Video,
-                storage_id=storage_id,
-                url=url,
+            # find channel name, then will search for tag there
+            channel_uri = page.locator("ytd-channel-name a:visible").filter(
+                has_not=page.get_by_role("link", name="ManageEngine", exact=True)
             )
+            channel_uri = await channel_uri.get_attribute("href")
+            logger.info(f"{channel_uri=}")
 
-    async def download_video(self, url):
-        storage_id = BaseStorage.gen_id(url)
+            page2 = await context.new_page()
+            tag = await self._get_channel_tag(channel_uri, page2)
+            await page2.close()
+            if tag is None:
+                return
+
+            content = await self.download_video(url)
+            if content:
+                yield CrawlerContent(
+                    tag_id=str(tag),
+                    tag_keepout=tag.is_keepout(),
+                    type=DatapoolContentType.Video,
+                    # storage_id=storage_id,
+                    url=url,
+                    content=content,
+                )
+        else:
+            logger.info("already processed")
 
+    async def download_video(self, url):
         # ... .desc()
 
         download_state = {"done": False, "tmp_path": None}
         thread = Thread(
             target=self._download_thread,
-            args=(url, storage_id, download_state),
+            args=(url, download_state),
         )
         thread.start()
-        logger.info(f"started video download thread on {storage_id=}")
+        logger.info(f"started video download thread on {url=}")
         while not download_state["done"]:
             await asyncio.sleep(1)
         thread.join()
-        logger.info(f"finished video download thread on {storage_id=}")
+        logger.info(f"finished video download thread on {url=}")
         tmp_path = download_state["tmp_path"]
 
         if tmp_path:
             raw_video = open(tmp_path, "rb").read()
 
-            await self.ctx.storage.put(storage_id, raw_video)
             # TODO: title and other meta data can be put into separate storage item ( for example storage_id+"_meta" )
             # as json for displaying at openlicense.ai
 
-            logger.info(f"put video into storage {storage_id=}")
             os.remove(tmp_path)
 
-            return storage_id
+            return raw_video
 
     async def _get_channel_tag(self, channel_uri, page):
         # init channel_lock per channel_uri
         async with self.channel_cache_lock_protection:
             if channel_uri not in self.channel_cache_lock:
                 self.channel_cache_lock[channel_uri] = asyncio.Lock()
```

### Comparing `datapools-1.0.57/datapools/worker/worker.py` & `datapools-1.0.58/datapools/worker/worker.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import uuid
 from copy import deepcopy
 from typing import Optional, Set
 
 from ..common.backend_api import BackendAPI
 from ..common.logger import logger
 from ..common.queues import GenericQueue, QueueMessage, QueueMessageType, QueueRole, QueueTopicMessage
-from ..common.session_manager import SessionManager
+from ..common.session_manager import SessionManager, Session
 from ..common.stoppable import Stoppable
 from ..common.storage import FileStorage
 from ..common.types import (
     CrawlerBackTask,
     CrawlerContent,
     CrawlerDemoUser,
     CrawlerHintURLStatus,
@@ -27,28 +27,37 @@
     WorkerSettings,
 )
 from .types import WorkerContext, WorkerTask
 from .plugins.base_plugin import BasePlugin
 from .utils import get_storage_invalidation_topic
 
 
+class WorkerFileStorage(FileStorage):
+    def __init__(self, dstpath, worker_id):
+        super().__init__(os.path.join(dstpath, worker_id))
+
+
 class CrawlerWorker(Stoppable):
     demo_users: dict[str, dict[str, str]]
 
     def __init__(self, cfg: Optional[WorkerSettings] = None):
         super().__init__()
         self.cfg = cfg if cfg is not None else WorkerSettings()
         self.id = uuid.uuid4().hex
         logger.info(f"worker id={self.id}")
 
         self.demo_users = {}
         self.api = BackendAPI(url=self.cfg.BACKEND_API_URL)
 
         self.session_manager = SessionManager(self.cfg.REDIS_HOST, self.cfg.REDIS_PORT)
-        self.storage = FileStorage(self.cfg.STORAGE_PATH)
+
+        # Worker storage must be separated from other workers
+        # so default schema when path is $STORAGE_PATH/$storage_id does not work here.
+        # Using $STORAGE_PATH/$worker_id/$storage_id path
+        self.storage = WorkerFileStorage(self.cfg.STORAGE_PATH, self.id)
 
         self.todo_tasks: Set[asyncio.Task] = set()
 
         self.init_plugins()
         self.todo_queue = GenericQueue(
             role=QueueRole.Receiver,
             url=self.cfg.QUEUE_CONNECTION_URL,
@@ -197,98 +206,73 @@
         except Exception as e:
             logger.error(f"!!!!!!!!Exception in worker_loop() {e}")
             logger.error(traceback.format_exc())
 
     async def _process_todo_message(self, message):
         qm = QueueMessage.decode(message.body)
 
-        if not self.session_manager.has(qm.session_id):
+        session = await self.session_manager.get(qm.session_id)
+        if not session:
             logger.error(f"Session not found {qm.session_id}")
             await self.todo_queue.reject(message, requeue=False)
             return
 
         if qm.type == QueueMessageType.Task:
             done = False
 
             task = WorkerTask(url=qm.data["url"], content_type=qm.data.get("content_type"))
             logger.info(f"got {task=} {qm.session_id=}")
 
             logger.info(f"processing {task.url=}")
 
-            plugin = self._get_url_plugin(task, qm.session_id)
+            plugin = self._get_url_plugin(task, session)
             logger.info(f"suitable {plugin=}")
 
             if plugin is None:
                 await self.todo_queue.reject(message, requeue=False)
                 return
 
             is_stopped = False
             for attempt in range(0, self.cfg.ATTEMPTS_PER_URL):
                 if attempt > 0:
                     logger.info(f"{attempt=}")
 
                 try:
-                    session = self.session_manager.get(qm.session_id)
-                    if session is None:
-                        break
 
-                    if session.is_stopped():
+                    if await session.is_stopped():
                         is_stopped = True
                         logger.info(f"Session is stopped, breaking. {qm.session_id=}")
                         break
 
-                    async for content_or_task in plugin.process(task):
-                        # logger.info( f'{type( content_or_task )=}')
-                        t = type(content_or_task)
+                    async for process_res in plugin.process(task):
+                        # logger.info( f'{type( process_res )=}')
+                        t = type(process_res)
                         # logger.info( f'{(t is CrawlerNop)=}')
 
-                        if session.is_stopped():
+                        if await session.is_stopped():
                             is_stopped = True
                             logger.info(f"Session is stopped, breaking. {qm.session_id=}")
                             break
 
                         if t is CrawlerContent:
-                            session.inc_crawled_content()
-
-                            # notifying producer about new crawled data
-                            await self.producer_queue.push(
-                                QueueMessage(
-                                    qm.session_id,
-                                    QueueMessageType.Task,
-                                    {
-                                        "parent_url": task.url,
-                                        "url": content_or_task.url,
-                                        "storage_id": content_or_task.storage_id,
-                                        "tag_id": content_or_task.tag_id,
-                                        "tag_keepout": content_or_task.tag_keepout,
-                                        "copyright_tag_id": content_or_task.copyright_tag_id,
-                                        "copyright_tag_keepout": content_or_task.copyright_tag_keepout,
-                                        "platform_tag_id": content_or_task.platform_tag_id,
-                                        "platform_tag_keepout": content_or_task.platform_tag_keepout,
-                                        "type": DatapoolContentType(content_or_task.type).value,
-                                        "priority_timestamp": content_or_task.priority_timestamp,
-                                        "worker_id": self.id,
-                                    },
-                                )
-                            )
-
+                            await self._process_crawled_content(process_res, session, plugin, task)
                         elif t is CrawlerBackTask:
-                            await self._add_back_task(qm.session_id, content_or_task)
+                            await self._add_back_task(qm.session_id, process_res)
                         elif t is CrawlerDemoUser:
-                            ct = content_or_task
+                            ct: CrawlerDemoUser = process_res
                             if ct.platform not in self.demo_users:
                                 self.demo_users[ct.platform] = {}
                             if ct.user_name not in self.demo_users[ct.platform]:
                                 logger.info(f"============= {dict(ct)} ===========")
                                 await self.api.add_demo_user(dict(ct))
                                 self.demo_users[ct.platform][ct.user_name] = ct.short_tag_id
                         elif t is CrawlerNop:
                             pass
                         else:
-                            raise Exception(f"unknown {content_or_task=}")
+                            raise Exception(f"unknown {process_res=}")
 
                         is_stopped = await self.is_stopped()
                         if is_stopped:
                             break
 
                     logger.info("plugin.process done")
                     await self._set_task_status(
@@ -330,19 +314,71 @@
             await self.todo_queue.reject(message)
 
     async def _set_task_status(self, session_id, task, status: CrawlerHintURLStatus):
         await self.reports_queue.push(
             QueueMessage(session_id, QueueMessageType.Report, {"task": deepcopy(task), "status": status.value})
         )
 
+    async def _process_crawled_content(
+        self, cc: CrawlerContent, session: Session, plugin: BasePlugin, task: WorkerTask
+    ):
+        if not await session.has_content(cc.url):
+            if not cc.content:
+                logger.info("no content, downloading")
+                cc.content = await plugin.download(cc.url)
+
+            if cc.content:
+                if not cc.tag_id:
+                    # trying to parse author tag
+                    if cc.type == DatapoolContentType.Image:
+                        image_tag = BasePlugin.parse_image_tag(cc.content)
+                        cc.tag_id = str(image_tag) if image_tag is not None else None
+                        cc.tag_keepout = image_tag.is_keepout() if image_tag is not None else False
+                    # TODO: add video/audio parsing here
+
+                if cc.tag_id is None and cc.copyright_tag_id is None and cc.platform_tag_id is None:
+                    logger.info("no tag available")
+                    return
+
+                storage_id = self.storage.gen_id(cc.url)
+                logger.info(f"putting to {storage_id=}")
+                await self.storage.put(storage_id, cc.content)
+
+                await session.add_content(cc.url)
+                await session.inc_crawled_content()
+
+                # notifying producer about new crawled data
+                await self.producer_queue.push(
+                    QueueMessage(
+                        session.id,
+                        QueueMessageType.Task,
+                        {
+                            "parent_url": task.url,
+                            "url": cc.url,
+                            "storage_id": storage_id,
+                            "tag_id": cc.tag_id,
+                            "tag_keepout": cc.tag_keepout,
+                            "copyright_tag_id": cc.copyright_tag_id,
+                            "copyright_tag_keepout": cc.copyright_tag_keepout,
+                            "platform_tag_id": cc.platform_tag_id,
+                            "platform_tag_keepout": cc.platform_tag_keepout,
+                            "type": DatapoolContentType(cc.type).value,
+                            "priority_timestamp": cc.priority_timestamp,
+                            "worker_id": self.id,
+                        },
+                    )
+                )
+            else:
+                logger.info("no content")
+
     async def _add_back_task(self, session_id, task: CrawlerBackTask):
         await self.reports_queue.push(QueueMessage(session_id, QueueMessageType.Task, task.to_dict()))
 
-    def _get_plugin_object(self, cls, session_id) -> BasePlugin:
-        ctx = WorkerContext(session=self.session_manager.get(session_id), storage=self.storage)  # type: ignore
+    def _get_plugin_object(self, cls, session: Session) -> BasePlugin:
+        ctx = WorkerContext(session=session)  # type: ignore
 
         args = [ctx]
         kwargs = {}
         logger.info(f"_get_plugin_object {cls=}")
 
         # convert class name into config plugins key
         # example: GoogleDrivePlugin => google_drive
@@ -355,38 +391,38 @@
         # logger.info(f'{plugin_config=}')
         if plugin_config is not None:
             # plugin config dict keys must match plugin's class __init__ arguments
             kwargs = plugin_config
 
         return cls[1](*args, **kwargs)
 
-    def _get_url_plugin(self, task: WorkerTask, session_id):
+    def _get_url_plugin(self, task: WorkerTask, session: Session):
         for plugin_data in self.plugins:
             cls = plugin_data[1]
             if cls[0] != "DefaultPlugin":
                 if cls[1].is_supported(task.url):
                     if plugin_data[0] is None:
-                        plugin_data[0] = self._get_plugin_object(cls, session_id)
+                        plugin_data[0] = self._get_plugin_object(cls, session)
 
                     if not plugin_data[0].is_busy:  # type: ignore[union-attr]
                         plugin_data[0].is_busy = True  # type: ignore[union-attr]
                         return plugin_data[0]
                     else:
-                        new_obj = self._get_plugin_object(cls, session_id)
+                        new_obj = self._get_plugin_object(cls, session)
                         new_obj.is_busy = True
                         return new_obj
 
         # creating/usingexisting default plugin
         for plugin_data in self.plugins:
             cls = plugin_data[1]
             if cls[0] == "DefaultPlugin":
                 if cls[1].is_supported(task.url):
                     if plugin_data[0] is None:
-                        plugin_data[0] = self._get_plugin_object(cls, session_id)
+                        plugin_data[0] = self._get_plugin_object(cls, session)
 
                     if not plugin_data[0].is_busy:  # type: ignore[union-attr]
                         plugin_data[0].is_busy = True  # type: ignore[union-attr]
                         return plugin_data[0]
                     else:
-                        new_obj = self._get_plugin_object(cls, session_id)
+                        new_obj = self._get_plugin_object(cls, session)
                         new_obj.is_busy = True
                         return new_obj
```

### Comparing `datapools-1.0.57/datapools.egg-info/PKG-INFO` & `datapools-1.0.58/datapools.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datapools
-Version: 1.0.57
+Version: 1.0.58
 Summary: Awesome datapools created by openlicenseai
 Home-page: https://github.com/openlicenseai/datapools/
 Author: openlicenseai
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydantic==2.6.1
 Requires-Dist: pydantic-settings==2.2.1
```

### Comparing `datapools-1.0.57/datapools.egg-info/SOURCES.txt` & `datapools-1.0.58/datapools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datapools-1.0.57/setup.py` & `datapools-1.0.58/setup.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.57/tests/test_base.py` & `datapools-1.0.58/tests/test_base.py`

 * *Files identical despite different names*

