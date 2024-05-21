# Comparing `tmp/gp2040ce_binary_tools-0.8.3.tar.gz` & `tmp/gp2040ce_binary_tools-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gp2040ce_binary_tools-0.8.3.tar", last modified: Mon Apr 15 15:22:18 2024, max compression
+gzip compressed data, was "gp2040ce_binary_tools-0.9.0.tar", last modified: Tue May 21 18:11:29 2024, max compression
```

## Comparing `gp2040ce_binary_tools-0.8.3.tar` & `gp2040ce_binary_tools-0.9.0.tar`

### file list

```diff
@@ -1,68 +1,67 @@
-drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-04-15 15:22:18.755234 gp2040ce_binary_tools-0.8.3/
--rw-r--r--   0 bss       (1026) bss       (1000)       12 2023-06-20 20:02:15.000000 gp2040ce_binary_tools-0.8.3/.gitattributes
--rw-r--r--   0 bss       (1026) bss       (1000)     3138 2023-06-20 20:30:00.000000 gp2040ce_binary_tools-0.8.3/.gitignore
-drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-04-15 15:22:18.739234 gp2040ce_binary_tools-0.8.3/.reuse/
--rw-r--r--   0 bss       (1026) bss       (1000)     1123 2024-04-12 12:56:02.000000 gp2040ce_binary_tools-0.8.3/.reuse/dep5
--rw-r--r--   0 bss       (1026) bss       (1000)     6570 2024-04-15 15:16:49.000000 gp2040ce_binary_tools-0.8.3/CHANGELOG.md
--rw-r--r--   0 bss       (1026) bss       (1000)     2726 2024-04-12 12:38:22.000000 gp2040ce_binary_tools-0.8.3/CONTRIBUTING.md
--rw-r--r--   0 bss       (1026) bss       (1000)    34893 2024-04-12 12:38:58.000000 gp2040ce_binary_tools-0.8.3/LICENSE.md
-drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-04-15 15:22:18.739234 gp2040ce_binary_tools-0.8.3/LICENSES/
--rw-r--r--   0 bss       (1026) bss       (1000)    18375 2024-04-12 12:38:22.000000 gp2040ce_binary_tools-0.8.3/LICENSES/CC-BY-SA-4.0.txt
--rw-r--r--   0 bss       (1026) bss       (1000)    34674 2024-04-12 12:38:22.000000 gp2040ce_binary_tools-0.8.3/LICENSES/GPL-3.0-or-later.txt
--rw-r--r--   0 bss       (1026) bss       (1000)     1078 2024-04-12 12:38:22.000000 gp2040ce_binary_tools-0.8.3/LICENSES/MIT.txt
--rw-r--r--   0 bss       (1026) bss       (1000)      428 2024-01-02 21:16:25.000000 gp2040ce_binary_tools-0.8.3/MAINTAINERS.md
--rw-r--r--   0 bss       (1026) bss       (1000)    11186 2024-04-15 15:22:18.755234 gp2040ce_binary_tools-0.8.3/PKG-INFO
--rw-r--r--   0 bss       (1026) bss       (1000)     9343 2024-04-13 01:04:00.000000 gp2040ce_binary_tools-0.8.3/README.md
-drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-04-15 15:22:18.753234 gp2040ce_binary_tools-0.8.3/gp2040ce_binary_tools.egg-info/
--rw-r--r--   0 bss       (1026) bss       (1000)    11186 2024-04-15 15:22:18.000000 gp2040ce_binary_tools-0.8.3/gp2040ce_binary_tools.egg-info/PKG-INFO
--rw-r--r--   0 bss       (1026) bss       (1000)     1744 2024-04-15 15:22:18.000000 gp2040ce_binary_tools-0.8.3/gp2040ce_binary_tools.egg-info/SOURCES.txt
--rw-r--r--   0 bss       (1026) bss       (1000)        1 2024-04-15 15:22:18.000000 gp2040ce_binary_tools-0.8.3/gp2040ce_binary_tools.egg-info/dependency_links.txt
--rw-r--r--   0 bss       (1026) bss       (1000)      347 2024-04-15 15:22:18.000000 gp2040ce_binary_tools-0.8.3/gp2040ce_binary_tools.egg-info/entry_points.txt
--rw-r--r--   0 bss       (1026) bss       (1000)      295 2024-04-15 15:22:18.000000 gp2040ce_binary_tools-0.8.3/gp2040ce_binary_tools.egg-info/requires.txt
--rw-r--r--   0 bss       (1026) bss       (1000)       18 2024-04-15 15:22:18.000000 gp2040ce_binary_tools-0.8.3/gp2040ce_binary_tools.egg-info/top_level.txt
-drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-04-15 15:22:18.740234 gp2040ce_binary_tools-0.8.3/gp2040ce_bintools/
--rw-r--r--   0 bss       (1026) bss       (1000)     2861 2024-03-07 15:08:57.000000 gp2040ce_binary_tools-0.8.3/gp2040ce_bintools/__init__.py
--rw-r--r--   0 bss       (1026) bss       (1000)      411 2024-04-15 15:22:18.000000 gp2040ce_binary_tools-0.8.3/gp2040ce_bintools/_version.py
--rw-r--r--   0 bss       (1026) bss       (1000)    18231 2024-04-15 15:13:16.000000 gp2040ce_binary_tools-0.8.3/gp2040ce_bintools/builder.py
--rw-r--r--   0 bss       (1026) bss       (1000)     1095 2024-04-12 12:38:22.000000 gp2040ce_binary_tools-0.8.3/gp2040ce_bintools/config_tree.css
--rw-r--r--   0 bss       (1026) bss       (1000)    22721 2024-04-13 01:01:20.000000 gp2040ce_binary_tools-0.8.3/gp2040ce_bintools/gui.py
-drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-04-15 15:22:18.740234 gp2040ce_binary_tools-0.8.3/gp2040ce_bintools/proto_snapshot/
--rw-r--r--   0 bss       (1026) bss       (1000)      407 2024-03-07 15:08:57.000000 gp2040ce_binary_tools-0.8.3/gp2040ce_bintools/proto_snapshot/__init__.py
--rw-r--r--   0 bss       (1026) bss       (1000)    23813 2024-04-08 13:57:12.000000 gp2040ce_binary_tools-0.8.3/gp2040ce_bintools/proto_snapshot/config.proto
--rw-r--r--   0 bss       (1026) bss       (1000)    43224 2024-04-08 13:57:12.000000 gp2040ce_binary_tools-0.8.3/gp2040ce_bintools/proto_snapshot/config_pb2.py
--rw-r--r--   0 bss       (1026) bss       (1000)     9696 2024-04-08 13:57:12.000000 gp2040ce_binary_tools-0.8.3/gp2040ce_bintools/proto_snapshot/enums.proto
--rw-r--r--   0 bss       (1026) bss       (1000)    15272 2024-04-08 13:57:12.000000 gp2040ce_binary_tools-0.8.3/gp2040ce_bintools/proto_snapshot/enums_pb2.py
--rw-r--r--   0 bss       (1026) bss       (1000)     7099 2024-04-08 13:35:15.000000 gp2040ce_binary_tools-0.8.3/gp2040ce_bintools/proto_snapshot/nanopb.proto
--rw-r--r--   0 bss       (1026) bss       (1000)     4619 2024-04-08 13:35:48.000000 gp2040ce_binary_tools-0.8.3/gp2040ce_bintools/proto_snapshot/nanopb_pb2.py
--rw-r--r--   0 bss       (1026) bss       (1000)     9212 2024-03-07 15:08:57.000000 gp2040ce_binary_tools-0.8.3/gp2040ce_bintools/rp2040.py
--rw-r--r--   0 bss       (1026) bss       (1000)    17598 2024-04-15 14:05:30.000000 gp2040ce_binary_tools-0.8.3/gp2040ce_bintools/storage.py
--rw-r--r--   0 bss       (1026) bss       (1000)     2871 2024-04-14 04:28:56.000000 gp2040ce_binary_tools-0.8.3/pyproject.toml
-drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-04-15 15:22:18.741234 gp2040ce_binary_tools-0.8.3/requirements/
--rw-r--r--   0 bss       (1026) bss       (1000)     4407 2024-04-12 12:38:22.000000 gp2040ce_binary_tools-0.8.3/requirements/requirements-dev.txt
--rw-r--r--   0 bss       (1026) bss       (1000)      906 2024-04-08 14:07:50.000000 gp2040ce_binary_tools-0.8.3/requirements/requirements.txt
--rw-r--r--   0 bss       (1026) bss       (1000)       38 2024-04-15 15:22:18.755234 gp2040ce_binary_tools-0.8.3/setup.cfg
-drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-04-15 15:22:18.741234 gp2040ce_binary_tools-0.8.3/tests/
--rw-r--r--   0 bss       (1026) bss       (1000)     2029 2024-03-07 15:08:57.000000 gp2040ce_binary_tools-0.8.3/tests/conftest.py
-drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-04-15 15:22:18.743234 gp2040ce_binary_tools-0.8.3/tests/test-files/
-drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-04-15 15:22:18.753234 gp2040ce_binary_tools-0.8.3/tests/test-files/pb2-files/
--rw-r--r--   0 bss       (1026) bss       (1000)    43224 2024-04-08 14:01:25.000000 gp2040ce_binary_tools-0.8.3/tests/test-files/pb2-files/config_pb2.py
--rw-r--r--   0 bss       (1026) bss       (1000)    15272 2024-04-08 14:01:25.000000 gp2040ce_binary_tools-0.8.3/tests/test-files/pb2-files/enums_pb2.py
--rw-r--r--   0 bss       (1026) bss       (1000)     4619 2024-04-08 14:00:25.000000 gp2040ce_binary_tools-0.8.3/tests/test-files/pb2-files/nanopb_pb2.py
-drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-04-15 15:22:18.753234 gp2040ce_binary_tools-0.8.3/tests/test-files/proto-files/
--rw-r--r--   0 bss       (1026) bss       (1000)    23813 2024-04-08 14:01:25.000000 gp2040ce_binary_tools-0.8.3/tests/test-files/proto-files/config.proto
--rw-r--r--   0 bss       (1026) bss       (1000)     9696 2024-04-08 14:01:25.000000 gp2040ce_binary_tools-0.8.3/tests/test-files/proto-files/enums.proto
--rw-r--r--   0 bss       (1026) bss       (1000)     7099 2024-04-08 14:00:09.000000 gp2040ce_binary_tools-0.8.3/tests/test-files/proto-files/nanopb.proto
--rw-r--r--   0 bss       (1026) bss       (1000)     3770 2024-01-03 19:02:39.000000 gp2040ce_binary_tools-0.8.3/tests/test-files/test-binary-source-of-json-config.bin
--rw-r--r--   0 bss       (1026) bss       (1000)     3321 2023-11-06 22:22:53.000000 gp2040ce_binary_tools-0.8.3/tests/test-files/test-config.bin
--rw-r--r--   0 bss       (1026) bss       (1000)    27879 2024-04-08 14:07:47.000000 gp2040ce_binary_tools-0.8.3/tests/test-files/test-config.json
--rw-r--r--   0 bss       (1026) bss       (1000)   816968 2023-11-06 22:20:55.000000 gp2040ce_binary_tools-0.8.3/tests/test-files/test-firmware.bin
--rw-r--r--   0 bss       (1026) bss       (1000)    16384 2023-11-06 22:20:55.000000 gp2040ce_binary_tools-0.8.3/tests/test-files/test-storage-area.bin
--rw-r--r--   0 bss       (1026) bss       (1000)  2097152 2024-01-06 22:53:09.000000 gp2040ce_binary_tools-0.8.3/tests/test-files/test-whole-board-with-board-config.bin
--rw-r--r--   0 bss       (1026) bss       (1000) 16777216 2023-11-06 22:20:55.000000 gp2040ce_binary_tools-0.8.3/tests/test-files/test-whole-board.bin
--rw-r--r--   0 bss       (1026) bss       (1000)    17892 2024-04-15 15:05:25.000000 gp2040ce_binary_tools-0.8.3/tests/test_builder.py
--rw-r--r--   0 bss       (1026) bss       (1000)     3979 2024-04-13 01:01:20.000000 gp2040ce_binary_tools-0.8.3/tests/test_commands.py
--rw-r--r--   0 bss       (1026) bss       (1000)    11360 2024-04-13 01:01:20.000000 gp2040ce_binary_tools-0.8.3/tests/test_gui.py
--rw-r--r--   0 bss       (1026) bss       (1000)     1508 2024-04-08 13:56:04.000000 gp2040ce_binary_tools-0.8.3/tests/test_package.py
--rw-r--r--   0 bss       (1026) bss       (1000)    11088 2024-03-07 15:08:57.000000 gp2040ce_binary_tools-0.8.3/tests/test_rp2040.py
--rw-r--r--   0 bss       (1026) bss       (1000)    12845 2024-04-15 14:24:33.000000 gp2040ce_binary_tools-0.8.3/tests/test_storage.py
--rw-r--r--   0 bss       (1026) bss       (1000)     1707 2024-04-13 01:13:16.000000 gp2040ce_binary_tools-0.8.3/tox.ini
+drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-05-21 18:11:29.434092 gp2040ce_binary_tools-0.9.0/
+-rw-r--r--   0 bss       (1026) bss       (1000)       12 2023-06-20 20:02:15.000000 gp2040ce_binary_tools-0.9.0/.gitattributes
+-rw-r--r--   0 bss       (1026) bss       (1000)     3138 2023-06-20 20:30:00.000000 gp2040ce_binary_tools-0.9.0/.gitignore
+drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-05-21 18:11:29.418092 gp2040ce_binary_tools-0.9.0/.reuse/
+-rw-r--r--   0 bss       (1026) bss       (1000)     1127 2024-04-21 23:51:37.000000 gp2040ce_binary_tools-0.9.0/.reuse/dep5
+-rw-r--r--   0 bss       (1026) bss       (1000)     7002 2024-05-21 18:09:09.000000 gp2040ce_binary_tools-0.9.0/CHANGELOG.md
+-rw-r--r--   0 bss       (1026) bss       (1000)     2726 2024-04-12 12:38:22.000000 gp2040ce_binary_tools-0.9.0/CONTRIBUTING.md
+-rw-r--r--   0 bss       (1026) bss       (1000)    34893 2024-04-12 12:38:58.000000 gp2040ce_binary_tools-0.9.0/LICENSE.md
+drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-05-21 18:11:29.418092 gp2040ce_binary_tools-0.9.0/LICENSES/
+-rw-r--r--   0 bss       (1026) bss       (1000)    34674 2024-04-12 12:38:22.000000 gp2040ce_binary_tools-0.9.0/LICENSES/GPL-3.0-or-later.txt
+-rw-r--r--   0 bss       (1026) bss       (1000)     1078 2024-04-12 12:38:22.000000 gp2040ce_binary_tools-0.9.0/LICENSES/MIT.txt
+-rw-r--r--   0 bss       (1026) bss       (1000)      428 2024-01-02 21:16:25.000000 gp2040ce_binary_tools-0.9.0/MAINTAINERS.md
+-rw-r--r--   0 bss       (1026) bss       (1000)    11186 2024-05-21 18:11:29.434092 gp2040ce_binary_tools-0.9.0/PKG-INFO
+-rw-r--r--   0 bss       (1026) bss       (1000)     9343 2024-04-13 01:04:00.000000 gp2040ce_binary_tools-0.9.0/README.md
+drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-05-21 18:11:29.432092 gp2040ce_binary_tools-0.9.0/gp2040ce_binary_tools.egg-info/
+-rw-r--r--   0 bss       (1026) bss       (1000)    11186 2024-05-21 18:11:29.000000 gp2040ce_binary_tools-0.9.0/gp2040ce_binary_tools.egg-info/PKG-INFO
+-rw-r--r--   0 bss       (1026) bss       (1000)     1718 2024-05-21 18:11:29.000000 gp2040ce_binary_tools-0.9.0/gp2040ce_binary_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 bss       (1026) bss       (1000)        1 2024-05-21 18:11:29.000000 gp2040ce_binary_tools-0.9.0/gp2040ce_binary_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 bss       (1026) bss       (1000)      347 2024-05-21 18:11:29.000000 gp2040ce_binary_tools-0.9.0/gp2040ce_binary_tools.egg-info/entry_points.txt
+-rw-r--r--   0 bss       (1026) bss       (1000)      295 2024-05-21 18:11:29.000000 gp2040ce_binary_tools-0.9.0/gp2040ce_binary_tools.egg-info/requires.txt
+-rw-r--r--   0 bss       (1026) bss       (1000)       18 2024-05-21 18:11:29.000000 gp2040ce_binary_tools-0.9.0/gp2040ce_binary_tools.egg-info/top_level.txt
+drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-05-21 18:11:29.419092 gp2040ce_binary_tools-0.9.0/gp2040ce_bintools/
+-rw-r--r--   0 bss       (1026) bss       (1000)     2922 2024-04-19 13:08:16.000000 gp2040ce_binary_tools-0.9.0/gp2040ce_bintools/__init__.py
+-rw-r--r--   0 bss       (1026) bss       (1000)      411 2024-05-21 18:11:29.000000 gp2040ce_binary_tools-0.9.0/gp2040ce_bintools/_version.py
+-rw-r--r--   0 bss       (1026) bss       (1000)    18475 2024-04-19 12:59:55.000000 gp2040ce_binary_tools-0.9.0/gp2040ce_bintools/builder.py
+-rw-r--r--   0 bss       (1026) bss       (1000)     1095 2024-04-12 12:38:22.000000 gp2040ce_binary_tools-0.9.0/gp2040ce_bintools/config_tree.css
+-rw-r--r--   0 bss       (1026) bss       (1000)    22751 2024-04-19 12:59:55.000000 gp2040ce_binary_tools-0.9.0/gp2040ce_bintools/gui.py
+drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-05-21 18:11:29.420092 gp2040ce_binary_tools-0.9.0/gp2040ce_bintools/proto_snapshot/
+-rw-r--r--   0 bss       (1026) bss       (1000)      407 2024-03-07 15:08:57.000000 gp2040ce_binary_tools-0.9.0/gp2040ce_bintools/proto_snapshot/__init__.py
+-rw-r--r--   0 bss       (1026) bss       (1000)    23813 2024-04-08 13:57:12.000000 gp2040ce_binary_tools-0.9.0/gp2040ce_bintools/proto_snapshot/config.proto
+-rw-r--r--   0 bss       (1026) bss       (1000)    43224 2024-05-21 17:28:46.000000 gp2040ce_binary_tools-0.9.0/gp2040ce_bintools/proto_snapshot/config_pb2.py
+-rw-r--r--   0 bss       (1026) bss       (1000)    10095 2024-05-21 17:28:11.000000 gp2040ce_binary_tools-0.9.0/gp2040ce_bintools/proto_snapshot/enums.proto
+-rw-r--r--   0 bss       (1026) bss       (1000)    15760 2024-05-21 17:28:43.000000 gp2040ce_binary_tools-0.9.0/gp2040ce_bintools/proto_snapshot/enums_pb2.py
+-rw-r--r--   0 bss       (1026) bss       (1000)     7099 2024-04-08 13:35:15.000000 gp2040ce_binary_tools-0.9.0/gp2040ce_bintools/proto_snapshot/nanopb.proto
+-rw-r--r--   0 bss       (1026) bss       (1000)     4619 2024-05-21 17:28:40.000000 gp2040ce_binary_tools-0.9.0/gp2040ce_bintools/proto_snapshot/nanopb_pb2.py
+-rw-r--r--   0 bss       (1026) bss       (1000)     9212 2024-03-07 15:08:57.000000 gp2040ce_binary_tools-0.9.0/gp2040ce_bintools/rp2040.py
+-rw-r--r--   0 bss       (1026) bss       (1000)    17808 2024-04-21 22:44:44.000000 gp2040ce_binary_tools-0.9.0/gp2040ce_bintools/storage.py
+-rw-r--r--   0 bss       (1026) bss       (1000)     2871 2024-04-14 04:28:56.000000 gp2040ce_binary_tools-0.9.0/pyproject.toml
+drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-05-21 18:11:29.420092 gp2040ce_binary_tools-0.9.0/requirements/
+-rw-r--r--   0 bss       (1026) bss       (1000)     4385 2024-05-21 17:17:09.000000 gp2040ce_binary_tools-0.9.0/requirements/requirements-dev.txt
+-rw-r--r--   0 bss       (1026) bss       (1000)      906 2024-05-21 17:16:32.000000 gp2040ce_binary_tools-0.9.0/requirements/requirements.txt
+-rw-r--r--   0 bss       (1026) bss       (1000)       38 2024-05-21 18:11:29.434092 gp2040ce_binary_tools-0.9.0/setup.cfg
+drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-05-21 18:11:29.421092 gp2040ce_binary_tools-0.9.0/tests/
+-rw-r--r--   0 bss       (1026) bss       (1000)     2029 2024-03-07 15:08:57.000000 gp2040ce_binary_tools-0.9.0/tests/conftest.py
+drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-05-21 18:11:29.423092 gp2040ce_binary_tools-0.9.0/tests/test-files/
+drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-05-21 18:11:29.432092 gp2040ce_binary_tools-0.9.0/tests/test-files/pb2-files/
+-rw-r--r--   0 bss       (1026) bss       (1000)    43224 2024-05-21 17:29:42.000000 gp2040ce_binary_tools-0.9.0/tests/test-files/pb2-files/config_pb2.py
+-rw-r--r--   0 bss       (1026) bss       (1000)    15760 2024-05-21 17:29:42.000000 gp2040ce_binary_tools-0.9.0/tests/test-files/pb2-files/enums_pb2.py
+-rw-r--r--   0 bss       (1026) bss       (1000)     4619 2024-05-21 17:29:42.000000 gp2040ce_binary_tools-0.9.0/tests/test-files/pb2-files/nanopb_pb2.py
+drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-05-21 18:11:29.432092 gp2040ce_binary_tools-0.9.0/tests/test-files/proto-files/
+-rw-r--r--   0 bss       (1026) bss       (1000)    23813 2024-04-08 14:01:25.000000 gp2040ce_binary_tools-0.9.0/tests/test-files/proto-files/config.proto
+-rw-r--r--   0 bss       (1026) bss       (1000)    10095 2024-05-21 17:29:05.000000 gp2040ce_binary_tools-0.9.0/tests/test-files/proto-files/enums.proto
+-rw-r--r--   0 bss       (1026) bss       (1000)     7099 2024-04-08 14:00:09.000000 gp2040ce_binary_tools-0.9.0/tests/test-files/proto-files/nanopb.proto
+-rw-r--r--   0 bss       (1026) bss       (1000)     3770 2024-01-03 19:02:39.000000 gp2040ce_binary_tools-0.9.0/tests/test-files/test-binary-source-of-json-config.bin
+-rw-r--r--   0 bss       (1026) bss       (1000)     3321 2023-11-06 22:22:53.000000 gp2040ce_binary_tools-0.9.0/tests/test-files/test-config.bin
+-rw-r--r--   0 bss       (1026) bss       (1000)    27879 2024-04-08 14:07:47.000000 gp2040ce_binary_tools-0.9.0/tests/test-files/test-config.json
+-rw-r--r--   0 bss       (1026) bss       (1000)   816968 2023-11-06 22:20:55.000000 gp2040ce_binary_tools-0.9.0/tests/test-files/test-firmware.bin
+-rw-r--r--   0 bss       (1026) bss       (1000)    16384 2023-11-06 22:20:55.000000 gp2040ce_binary_tools-0.9.0/tests/test-files/test-storage-area.bin
+-rw-r--r--   0 bss       (1026) bss       (1000)  2097152 2024-01-06 22:53:09.000000 gp2040ce_binary_tools-0.9.0/tests/test-files/test-whole-board-with-board-config.bin
+-rw-r--r--   0 bss       (1026) bss       (1000) 16777216 2023-11-06 22:20:55.000000 gp2040ce_binary_tools-0.9.0/tests/test-files/test-whole-board.bin
+-rw-r--r--   0 bss       (1026) bss       (1000)    18468 2024-04-19 12:59:55.000000 gp2040ce_binary_tools-0.9.0/tests/test_builder.py
+-rw-r--r--   0 bss       (1026) bss       (1000)     4045 2024-04-19 13:10:31.000000 gp2040ce_binary_tools-0.9.0/tests/test_commands.py
+-rw-r--r--   0 bss       (1026) bss       (1000)    11360 2024-04-13 01:01:20.000000 gp2040ce_binary_tools-0.9.0/tests/test_gui.py
+-rw-r--r--   0 bss       (1026) bss       (1000)     1508 2024-04-08 13:56:04.000000 gp2040ce_binary_tools-0.9.0/tests/test_package.py
+-rw-r--r--   0 bss       (1026) bss       (1000)    11088 2024-03-07 15:08:57.000000 gp2040ce_binary_tools-0.9.0/tests/test_rp2040.py
+-rw-r--r--   0 bss       (1026) bss       (1000)    13249 2024-04-21 22:44:44.000000 gp2040ce_binary_tools-0.9.0/tests/test_storage.py
+-rw-r--r--   0 bss       (1026) bss       (1000)     1707 2024-04-13 01:13:16.000000 gp2040ce_binary_tools-0.9.0/tox.ini
```

### Comparing `gp2040ce_binary_tools-0.8.3/.gitignore` & `gp2040ce_binary_tools-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.3/.reuse/dep5` & `gp2040ce_binary_tools-0.9.0/.reuse/dep5`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 Files: gp2040ce_bintools/proto_snapshot/*
 Copyright: (c) 2024 OpenStickCommunity (gp2040-ce.info)
 License: MIT
 
 # High level repo docs
 Files: *.md
 Copyright: © 2023 Brian S. Stephan <bss@incorporeal.org>
-License: CC-BY-SA-4.0
+License: GPL-3.0-or-later
 
 # Test data (GP2040-CE-derived)
 Files: tests/test-files/pb2-files/* tests/test-files/proto-files/*
 Copyright: (c) 2024 OpenStickCommunity (gp2040-ce.info)
 License: MIT
 
 # Test data
```

### Comparing `gp2040ce_binary_tools-0.8.3/CHANGELOG.md` & `gp2040ce_binary_tools-0.9.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,26 @@
 # CHANGELOG
 
 Included is a summary of changes to the project. For full details, especially on behind-the-scenes code changes and
 development tools, see the commit history.
 
+## v0.9.0
+
+### Features
+
+* The TUI editor can read and save configs as JSON files, which should create another avenue for making configs
+  available and editable for humans.
+
+### Miscellaneous
+
+* The `--version` flag outputs a bit of information about the program and Python version.
+* The config protobuf snapshot has been updated for (what should be) GP2040-CE v0.7.9.
+* Requirements version bumps.
+* REUSE specification errata.
+
 ## v0.8.3
 
 ### Improvements
 
 * `summarize-gp2040ce` can now understand the segmented UF2 files written in v0.8.1.
 * `concatenate` has an added `--backup` flag, which will move an existing output file aside before writing the new
   output.
```

### Comparing `gp2040ce_binary_tools-0.8.3/CONTRIBUTING.md` & `gp2040ce_binary_tools-0.9.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.3/LICENSE.md` & `gp2040ce_binary_tools-0.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.3/LICENSES/GPL-3.0-or-later.txt` & `gp2040ce_binary_tools-0.9.0/LICENSES/GPL-3.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.3/LICENSES/MIT.txt` & `gp2040ce_binary_tools-0.9.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.3/PKG-INFO` & `gp2040ce_binary_tools-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gp2040ce-binary-tools
-Version: 0.8.3
+Version: 0.9.0
 Summary: Tools for working with GP2040-CE firmware and storage binaries.
 Author-email: "Brian S. Stephan" <bss@incorporeal.org>
 License: GPL-3.0-or-later
 Project-URL: Homepage, https://github.com/OpenStickCommunity/gp2040ce-binary-tools
 Project-URL: Changelog, https://github.com/OpenStickCommunity/gp2040ce-binary-tools/blob/main/CHANGELOG.md
 Project-URL: Bug Tracker, https://github.com/OpenStickCommunity/gp2040ce-binary-tools/issues
 Classifier: Environment :: Console
```

### Comparing `gp2040ce_binary_tools-0.8.3/README.md` & `gp2040ce_binary_tools-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.3/gp2040ce_binary_tools.egg-info/PKG-INFO` & `gp2040ce_binary_tools-0.9.0/gp2040ce_binary_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gp2040ce-binary-tools
-Version: 0.8.3
+Version: 0.9.0
 Summary: Tools for working with GP2040-CE firmware and storage binaries.
 Author-email: "Brian S. Stephan" <bss@incorporeal.org>
 License: GPL-3.0-or-later
 Project-URL: Homepage, https://github.com/OpenStickCommunity/gp2040ce-binary-tools
 Project-URL: Changelog, https://github.com/OpenStickCommunity/gp2040ce-binary-tools/blob/main/CHANGELOG.md
 Project-URL: Bug Tracker, https://github.com/OpenStickCommunity/gp2040ce-binary-tools/issues
 Classifier: Environment :: Console
```

### Comparing `gp2040ce_binary_tools-0.8.3/gp2040ce_binary_tools.egg-info/SOURCES.txt` & `gp2040ce_binary_tools-0.9.0/gp2040ce_binary_tools.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 CONTRIBUTING.md
 LICENSE.md
 MAINTAINERS.md
 README.md
 pyproject.toml
 tox.ini
 .reuse/dep5
-LICENSES/CC-BY-SA-4.0.txt
 LICENSES/GPL-3.0-or-later.txt
 LICENSES/MIT.txt
 gp2040ce_binary_tools.egg-info/PKG-INFO
 gp2040ce_binary_tools.egg-info/SOURCES.txt
 gp2040ce_binary_tools.egg-info/dependency_links.txt
 gp2040ce_binary_tools.egg-info/entry_points.txt
 gp2040ce_binary_tools.egg-info/requires.txt
```

### Comparing `gp2040ce_binary_tools-0.8.3/gp2040ce_bintools/__init__.py` & `gp2040ce_binary_tools-0.9.0/gp2040ce_bintools/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,16 @@
 handler.setFormatter(formatter)
 root.addHandler(handler)
 
 logger = logging.getLogger(__name__)
 
 # parse flags that are common to many tools (e.g. adding paths for finding .proto files)
 core_parser = argparse.ArgumentParser(add_help=False)
-core_parser.add_argument('-v', '--version', action='version', version=f"%(prog)s {__version__}",
+core_parser.add_argument('-v', '--version', action='version',
+                         version=f"gp2040ce-binary-tools {__version__} (Python {sys.version})",
                          help="show version information and exit")
 core_parser.add_argument('-d', '--debug', action='store_true', help="enable debug logging")
 core_parser.add_argument('-P', '--proto-files-path', type=pathlib.Path, default=list(), action='append',
                          help="path to .proto files to read, including dependencies; you will likely need "
                               "to supply this twice, once for GP2040-CE's .proto files and once for nanopb's")
 args, _ = core_parser.parse_known_args()
 for path in args.proto_files_path:
```

### Comparing `gp2040ce_binary_tools-0.8.3/gp2040ce_bintools/builder.py` & `gp2040ce_binary_tools-0.9.0/gp2040ce_bintools/builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import argparse
 import copy
 import logging
 import os
 import re
 from typing import Optional
 
+from google.protobuf.json_format import MessageToJson
 from google.protobuf.message import Message
 
 import gp2040ce_bintools.storage as storage
 from gp2040ce_bintools import core_parser
 from gp2040ce_bintools.rp2040 import get_bootsel_endpoints, read, write
 
 logger = logging.getLogger(__name__)
@@ -244,23 +245,27 @@
         config_binary = storage.serialize_config_with_footer(config)
         with open(filename, 'rb') as file:
             existing_binary = file.read()
         binary = replace_config_in_binary(bytearray(existing_binary), config_binary)
         with open(filename, 'wb') as file:
             file.write(binary)
     else:
-        binary = storage.serialize_config_with_footer(config)
-        with open(filename, 'wb') as file:
-            if filename[-4:] == '.uf2':
-                # we must pad to storage start in order for the UF2 write addresses to make sense
-                file.write(storage.convert_binary_to_uf2([
-                    (storage.USER_CONFIG_BINARY_LOCATION, storage.pad_config_to_storage_size(binary)),
-                ]))
-            else:
-                file.write(binary)
+        if filename[-5:] == '.json':
+            with open(filename, 'w') as file:
+                file.write(f'{MessageToJson(config)}\n')
+        else:
+            binary = storage.serialize_config_with_footer(config)
+            with open(filename, 'wb') as file:
+                if filename[-4:] == '.uf2':
+                    # we must pad to storage start in order for the UF2 write addresses to make sense
+                    file.write(storage.convert_binary_to_uf2([
+                        (storage.USER_CONFIG_BINARY_LOCATION, storage.pad_config_to_storage_size(binary)),
+                    ]))
+                else:
+                    file.write(binary)
 
 
 def write_new_config_to_usb(config: Message, endpoint_out: object, endpoint_in: object):
     """Serialize the provided config to a device over USB, in the proper location for a GP2040-CE board.
 
     Args:
         config: the Protobuf configuration to write to a RP2040 board in BOOTSEL mode
```

### Comparing `gp2040ce_binary_tools-0.8.3/gp2040ce_bintools/config_tree.css` & `gp2040ce_binary_tools-0.9.0/gp2040ce_bintools/config_tree.css`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.3/gp2040ce_bintools/gui.py` & `gp2040ce_binary_tools-0.9.0/gp2040ce_bintools/gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,15 +130,16 @@
         self.config = config
         super().__init__(*args, **kwargs)
 
     def compose(self) -> ComposeResult:
         """Build the pop-up window prompting for the new filename to save the configuration as."""
         self.filename_field = Input(value=None, id='field-input', validators=[Length(minimum=1)])
         yield Grid(
-            Container(Label("Filename (.uf2 or .bin) to write to:", id='field-name'), id='field-name-container'),
+            Container(Label("Filename (.uf2, .bin, or .json) to write to:", id='field-name'),
+                      id='field-name-container'),
             Container(self.filename_field, id='input-field-container'),
             Container(Pretty('', id='input-errors', classes='hidden'), id='error-container'),
             Horizontal(Container(Button("Cancel", id='cancel-button'), id='cancel-button-container'),
                        Container(Button("Confirm", id='confirm-button'), id='confirm-button-container'),
                        id='button-container'),
             id='save-as-dialog',
         )
```

### Comparing `gp2040ce_binary_tools-0.8.3/gp2040ce_bintools/proto_snapshot/config.proto` & `gp2040ce_binary_tools-0.9.0/gp2040ce_bintools/proto_snapshot/config.proto`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.3/gp2040ce_bintools/proto_snapshot/config_pb2.py` & `gp2040ce_binary_tools-0.9.0/gp2040ce_bintools/proto_snapshot/config_pb2.py`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.3/gp2040ce_bintools/proto_snapshot/enums.proto` & `gp2040ce_binary_tools-0.9.0/gp2040ce_bintools/proto_snapshot/enums.proto`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,19 @@
     BUTTON_LAYOUT_TAIKO_A = 21;
     BUTTON_LAYOUT_BM_TURNTABLE_A = 22;
     BUTTON_LAYOUT_BM_5KEY_A = 23;
     BUTTON_LAYOUT_BM_7KEY_A = 24;
     BUTTON_LAYOUT_GITADORA_FRET_A = 25;
     BUTTON_LAYOUT_GITADORA_STRUM_A = 26;
     BUTTON_LAYOUT_BOARD_DEFINED_A = 27;
+    BUTTON_LAYOUT_BANDHERO_FRET_A = 28;
+    BUTTON_LAYOUT_BANDHERO_STRUM_A = 29;
+    BUTTON_LAYOUT_6GAWD_A = 30;
+    BUTTON_LAYOUT_6GAWD_ALLBUTTON_A = 31;
+    BUTTON_LAYOUT_6GAWD_ALLBUTTONPLUS_A = 32;
 }
 
 enum ButtonLayoutRight
 {
     option (nanopb_enumopt).long_names = false;
 
     BUTTON_LAYOUT_ARCADE = 0;
@@ -68,14 +73,19 @@
     BUTTON_LAYOUT_TAIKO_B = 25;
     BUTTON_LAYOUT_BM_TURNTABLE_B = 26;
     BUTTON_LAYOUT_BM_5KEY_B = 27;
     BUTTON_LAYOUT_BM_7KEY_B = 28;
     BUTTON_LAYOUT_GITADORA_FRET_B = 29;
     BUTTON_LAYOUT_GITADORA_STRUM_B = 30;
     BUTTON_LAYOUT_BOARD_DEFINED_B = 31;
+    BUTTON_LAYOUT_BANDHERO_FRET_B = 32;
+    BUTTON_LAYOUT_BANDHERO_STRUM_B = 33;
+    BUTTON_LAYOUT_6GAWD_B = 34;
+    BUTTON_LAYOUT_6GAWD_ALLBUTTON_B = 35;
+    BUTTON_LAYOUT_6GAWD_ALLBUTTONPLUS_B = 36;
 }
 
 enum SplashMode
 {
     option (nanopb_enumopt).long_names = false;
 
     SPLASH_MODE_STATIC = 0;
@@ -338,15 +348,15 @@
 
 enum GPShape_Type
 {
     option (nanopb_enumopt).long_names = false;
     
     GP_SHAPE_ELLIPSE = 0;
     GP_SHAPE_SQUARE = 1;
-    GP_SHAPE_DIAMOND = 2;
+    GP_SHAPE_LINE = 2;
     GP_SHAPE_POLYGON = 3;
     GP_SHAPE_ARC = 4;
 };
 
 enum RotaryEncoderPinMode
 {
     option (nanopb_enumopt).long_names = false;
```

### Comparing `gp2040ce_binary_tools-0.8.3/gp2040ce_bintools/proto_snapshot/enums_pb2.py` & `gp2040ce_binary_tools-0.9.0/gp2040ce_bintools/proto_snapshot/enums_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 _sym_db = _symbol_database.Default()
 
 
 import nanopb_pb2 as nanopb__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0b\x65nums.proto\x1a\x0cnanopb.proto*\x8d\x07\n\x0c\x42uttonLayout\x12\x17\n\x13\x42UTTON_LAYOUT_STICK\x10\x00\x12\x1b\n\x17\x42UTTON_LAYOUT_STICKLESS\x10\x01\x12 \n\x1c\x42UTTON_LAYOUT_BUTTONS_ANGLED\x10\x02\x12\x1f\n\x1b\x42UTTON_LAYOUT_BUTTONS_BASIC\x10\x03\x12!\n\x1d\x42UTTON_LAYOUT_KEYBOARD_ANGLED\x10\x04\x12\x1b\n\x17\x42UTTON_LAYOUT_KEYBOARDA\x10\x05\x12\x1b\n\x17\x42UTTON_LAYOUT_DANCEPADA\x10\x06\x12\x1c\n\x18\x42UTTON_LAYOUT_TWINSTICKA\x10\x07\x12\x18\n\x14\x42UTTON_LAYOUT_BLANKA\x10\x08\x12\x16\n\x12\x42UTTON_LAYOUT_VLXA\x10\t\x12\"\n\x1e\x42UTTON_LAYOUT_FIGHTBOARD_STICK\x10\n\x12%\n!BUTTON_LAYOUT_FIGHTBOARD_MIRRORED\x10\x0b\x12\x19\n\x15\x42UTTON_LAYOUT_CUSTOMA\x10\x0c\x12 \n\x1c\x42UTTON_LAYOUT_OPENCORE0WASDA\x10\r\x12\x1e\n\x1a\x42UTTON_LAYOUT_STICKLESS_13\x10\x0e\x12\x1e\n\x1a\x42UTTON_LAYOUT_STICKLESS_16\x10\x0f\x12\x1e\n\x1a\x42UTTON_LAYOUT_STICKLESS_14\x10\x10\x12#\n\x1f\x42UTTON_LAYOUT_DANCEPAD_DDR_LEFT\x10\x11\x12#\n\x1f\x42UTTON_LAYOUT_DANCEPAD_DDR_SOLO\x10\x12\x12#\n\x1f\x42UTTON_LAYOUT_DANCEPAD_PIU_LEFT\x10\x13\x12\x18\n\x14\x42UTTON_LAYOUT_POPN_A\x10\x14\x12\x19\n\x15\x42UTTON_LAYOUT_TAIKO_A\x10\x15\x12 \n\x1c\x42UTTON_LAYOUT_BM_TURNTABLE_A\x10\x16\x12\x1b\n\x17\x42UTTON_LAYOUT_BM_5KEY_A\x10\x17\x12\x1b\n\x17\x42UTTON_LAYOUT_BM_7KEY_A\x10\x18\x12!\n\x1d\x42UTTON_LAYOUT_GITADORA_FRET_A\x10\x19\x12\"\n\x1e\x42UTTON_LAYOUT_GITADORA_STRUM_A\x10\x1a\x12!\n\x1d\x42UTTON_LAYOUT_BOARD_DEFINED_A\x10\x1b\x1a\x05\x92?\x02 \x00*\xec\x07\n\x11\x42uttonLayoutRight\x12\x18\n\x14\x42UTTON_LAYOUT_ARCADE\x10\x00\x12\x1c\n\x18\x42UTTON_LAYOUT_STICKLESSB\x10\x01\x12!\n\x1d\x42UTTON_LAYOUT_BUTTONS_ANGLEDB\x10\x02\x12\x18\n\x14\x42UTTON_LAYOUT_VEWLIX\x10\x03\x12\x19\n\x15\x42UTTON_LAYOUT_VEWLIX7\x10\x04\x12\x18\n\x14\x42UTTON_LAYOUT_CAPCOM\x10\x05\x12\x19\n\x15\x42UTTON_LAYOUT_CAPCOM6\x10\x06\x12\x18\n\x14\x42UTTON_LAYOUT_SEGA2P\x10\x07\x12\x17\n\x13\x42UTTON_LAYOUT_NOIR8\x10\x08\x12\x1b\n\x17\x42UTTON_LAYOUT_KEYBOARDB\x10\t\x12\x1b\n\x17\x42UTTON_LAYOUT_DANCEPADB\x10\n\x12\x1c\n\x18\x42UTTON_LAYOUT_TWINSTICKB\x10\x0b\x12\x18\n\x14\x42UTTON_LAYOUT_BLANKB\x10\x0c\x12\x16\n\x12\x42UTTON_LAYOUT_VLXB\x10\r\x12\x1c\n\x18\x42UTTON_LAYOUT_FIGHTBOARD\x10\x0e\x12+\n\'BUTTON_LAYOUT_FIGHTBOARD_STICK_MIRRORED\x10\x0f\x12\x19\n\x15\x42UTTON_LAYOUT_CUSTOMB\x10\x10\x12\x1c\n\x18\x42UTTON_LAYOUT_KEYBOARD8B\x10\x11\x12 \n\x1c\x42UTTON_LAYOUT_OPENCORE0WASDB\x10\x12\x12\x1f\n\x1b\x42UTTON_LAYOUT_STICKLESS_13B\x10\x13\x12\x1f\n\x1b\x42UTTON_LAYOUT_STICKLESS_16B\x10\x14\x12\x1f\n\x1b\x42UTTON_LAYOUT_STICKLESS_14B\x10\x15\x12$\n BUTTON_LAYOUT_DANCEPAD_DDR_RIGHT\x10\x16\x12$\n BUTTON_LAYOUT_DANCEPAD_PIU_RIGHT\x10\x17\x12\x18\n\x14\x42UTTON_LAYOUT_POPN_B\x10\x18\x12\x19\n\x15\x42UTTON_LAYOUT_TAIKO_B\x10\x19\x12 \n\x1c\x42UTTON_LAYOUT_BM_TURNTABLE_B\x10\x1a\x12\x1b\n\x17\x42UTTON_LAYOUT_BM_5KEY_B\x10\x1b\x12\x1b\n\x17\x42UTTON_LAYOUT_BM_7KEY_B\x10\x1c\x12!\n\x1d\x42UTTON_LAYOUT_GITADORA_FRET_B\x10\x1d\x12\"\n\x1e\x42UTTON_LAYOUT_GITADORA_STRUM_B\x10\x1e\x12!\n\x1d\x42UTTON_LAYOUT_BOARD_DEFINED_B\x10\x1f\x1a\x05\x92?\x02 \x00*y\n\nSplashMode\x12\x16\n\x12SPLASH_MODE_STATIC\x10\x00\x12\x17\n\x13SPLASH_MODE_CLOSEIN\x10\x01\x12\x1d\n\x19SPLASH_MODE_CLOSEINCUSTOM\x10\x02\x12\x14\n\x10SPLASH_MODE_NONE\x10\x03\x1a\x05\x92?\x02 \x00*\xa0\x01\n\x0cSplashChoice\x12\x16\n\x12SPLASH_CHOICE_MAIN\x10\x00\x12\x13\n\x0fSPLASH_CHOICE_X\x10\x01\x12\x13\n\x0fSPLASH_CHOICE_Y\x10\x02\x12\x13\n\x0fSPLASH_CHOICE_Z\x10\x03\x12\x18\n\x14SPLASH_CHOICE_CUSTOM\x10\x04\x12\x18\n\x14SPLASH_CHOICE_LEGACY\x10\x05\x1a\x05\x92?\x02 \x00*\x99\x01\n\x0eOnBoardLedMode\x12\x19\n\x15ON_BOARD_LED_MODE_OFF\x10\x00\x12$\n ON_BOARD_LED_MODE_MODE_INDICATOR\x10\x01\x12 \n\x1cON_BOARD_LED_MODE_INPUT_TEST\x10\x02\x12\x1d\n\x19ON_BOARD_LED_MODE_PS_AUTH\x10\x03\x1a\x05\x92?\x02 \x00*\xec\x02\n\tInputMode\x12\x15\n\x11INPUT_MODE_XINPUT\x10\x00\x12\x15\n\x11INPUT_MODE_SWITCH\x10\x01\x12\x12\n\x0eINPUT_MODE_HID\x10\x02\x12\x17\n\x13INPUT_MODE_KEYBOARD\x10\x03\x12\x12\n\x0eINPUT_MODE_PS4\x10\x04\x12\x14\n\x10INPUT_MODE_XBONE\x10\x05\x12\x15\n\x11INPUT_MODE_MDMINI\x10\x06\x12\x15\n\x11INPUT_MODE_NEOGEO\x10\x07\x12\x16\n\x12INPUT_MODE_PCEMINI\x10\x08\x12\x14\n\x10INPUT_MODE_EGRET\x10\t\x12\x14\n\x10INPUT_MODE_ASTRO\x10\n\x12\x18\n\x14INPUT_MODE_PSCLASSIC\x10\x0b\x12\x1b\n\x17INPUT_MODE_XBOXORIGINAL\x10\x0c\x12\x12\n\x0eINPUT_MODE_PS5\x10\r\x12\x16\n\x11INPUT_MODE_CONFIG\x10\xff\x01\x1a\x05\x92?\x02 \x00*\x94\x01\n\x11InputModeAuthType\x12\x1d\n\x19INPUT_MODE_AUTH_TYPE_NONE\x10\x00\x12\x1d\n\x19INPUT_MODE_AUTH_TYPE_KEYS\x10\x01\x12\x1c\n\x18INPUT_MODE_AUTH_TYPE_USB\x10\x02\x12\x1c\n\x18INPUT_MODE_AUTH_TYPE_I2C\x10\x03\x1a\x05\x92?\x02 \x00*_\n\x08\x44padMode\x12\x15\n\x11\x44PAD_MODE_DIGITAL\x10\x00\x12\x19\n\x15\x44PAD_MODE_LEFT_ANALOG\x10\x01\x12\x1a\n\x16\x44PAD_MODE_RIGHT_ANALOG\x10\x02\x1a\x05\x92?\x02 \x00*O\n\nInvertMode\x12\x0f\n\x0bINVERT_NONE\x10\x00\x12\x0c\n\x08INVERT_X\x10\x01\x12\x0c\n\x08INVERT_Y\x10\x02\x12\r\n\tINVERT_XY\x10\x03\x1a\x05\x92?\x02 \x00*\xa2\x01\n\x08SOCDMode\x12\x19\n\x15SOCD_MODE_UP_PRIORITY\x10\x00\x12\x15\n\x11SOCD_MODE_NEUTRAL\x10\x01\x12#\n\x1fSOCD_MODE_SECOND_INPUT_PRIORITY\x10\x02\x12\"\n\x1eSOCD_MODE_FIRST_INPUT_PRIORITY\x10\x03\x12\x14\n\x10SOCD_MODE_BYPASS\x10\x04\x1a\x05\x92?\x02 \x00*\x88\x08\n\nGpioAction\x12\x11\n\x04NONE\x10\xf6\xff\xff\xff\xff\xff\xff\xff\xff\x01\x12\x15\n\x08RESERVED\x10\xfb\xff\xff\xff\xff\xff\xff\xff\xff\x01\x12\x15\n\x11\x41SSIGNED_TO_ADDON\x10\x00\x12\x13\n\x0f\x42UTTON_PRESS_UP\x10\x01\x12\x15\n\x11\x42UTTON_PRESS_DOWN\x10\x02\x12\x15\n\x11\x42UTTON_PRESS_LEFT\x10\x03\x12\x16\n\x12\x42UTTON_PRESS_RIGHT\x10\x04\x12\x13\n\x0f\x42UTTON_PRESS_B1\x10\x05\x12\x13\n\x0f\x42UTTON_PRESS_B2\x10\x06\x12\x13\n\x0f\x42UTTON_PRESS_B3\x10\x07\x12\x13\n\x0f\x42UTTON_PRESS_B4\x10\x08\x12\x13\n\x0f\x42UTTON_PRESS_L1\x10\t\x12\x13\n\x0f\x42UTTON_PRESS_R1\x10\n\x12\x13\n\x0f\x42UTTON_PRESS_L2\x10\x0b\x12\x13\n\x0f\x42UTTON_PRESS_R2\x10\x0c\x12\x13\n\x0f\x42UTTON_PRESS_S1\x10\r\x12\x13\n\x0f\x42UTTON_PRESS_S2\x10\x0e\x12\x13\n\x0f\x42UTTON_PRESS_A1\x10\x0f\x12\x13\n\x0f\x42UTTON_PRESS_A2\x10\x10\x12\x13\n\x0f\x42UTTON_PRESS_L3\x10\x11\x12\x13\n\x0f\x42UTTON_PRESS_R3\x10\x12\x12\x13\n\x0f\x42UTTON_PRESS_FN\x10\x13\x12\x17\n\x13\x42UTTON_PRESS_DDI_UP\x10\x14\x12\x19\n\x15\x42UTTON_PRESS_DDI_DOWN\x10\x15\x12\x19\n\x15\x42UTTON_PRESS_DDI_LEFT\x10\x16\x12\x1a\n\x16\x42UTTON_PRESS_DDI_RIGHT\x10\x17\x12\x16\n\x12SUSTAIN_DP_MODE_DP\x10\x18\x12\x16\n\x12SUSTAIN_DP_MODE_LS\x10\x19\x12\x16\n\x12SUSTAIN_DP_MODE_RS\x10\x1a\x12\x1d\n\x19SUSTAIN_SOCD_MODE_UP_PRIO\x10\x1b\x12\x1d\n\x19SUSTAIN_SOCD_MODE_NEUTRAL\x10\x1c\x12 \n\x1cSUSTAIN_SOCD_MODE_SECOND_WIN\x10\x1d\x12\x1f\n\x1bSUSTAIN_SOCD_MODE_FIRST_WIN\x10\x1e\x12\x1c\n\x18SUSTAIN_SOCD_MODE_BYPASS\x10\x1f\x12\x16\n\x12\x42UTTON_PRESS_TURBO\x10 \x12\x16\n\x12\x42UTTON_PRESS_MACRO\x10!\x12\x18\n\x14\x42UTTON_PRESS_MACRO_1\x10\"\x12\x18\n\x14\x42UTTON_PRESS_MACRO_2\x10#\x12\x18\n\x14\x42UTTON_PRESS_MACRO_3\x10$\x12\x18\n\x14\x42UTTON_PRESS_MACRO_4\x10%\x12\x18\n\x14\x42UTTON_PRESS_MACRO_5\x10&\x12\x18\n\x14\x42UTTON_PRESS_MACRO_6\x10\'\x1a\x05\x92?\x02 \x00*\x80\x07\n\rGamepadHotkey\x12\x0f\n\x0bHOTKEY_NONE\x10\x00\x12\x17\n\x13HOTKEY_DPAD_DIGITAL\x10\x01\x12\x1b\n\x17HOTKEY_DPAD_LEFT_ANALOG\x10\x02\x12\x1c\n\x18HOTKEY_DPAD_RIGHT_ANALOG\x10\x03\x12\x16\n\x12HOTKEY_HOME_BUTTON\x10\x04\x12\x19\n\x15HOTKEY_CAPTURE_BUTTON\x10\x05\x12\x1b\n\x17HOTKEY_SOCD_UP_PRIORITY\x10\x06\x12\x17\n\x13HOTKEY_SOCD_NEUTRAL\x10\x07\x12\x1a\n\x16HOTKEY_SOCD_LAST_INPUT\x10\x08\x12\x18\n\x14HOTKEY_INVERT_X_AXIS\x10\t\x12\x18\n\x14HOTKEY_INVERT_Y_AXIS\x10\n\x12\x1b\n\x17HOTKEY_SOCD_FIRST_INPUT\x10\x0b\x12\x16\n\x12HOTKEY_SOCD_BYPASS\x10\x0c\x12\x1c\n\x18HOTKEY_TOGGLE_4_WAY_MODE\x10\r\x12 \n\x1cHOTKEY_TOGGLE_DDI_4_WAY_MODE\x10\x0e\x12\x19\n\x15HOTKEY_LOAD_PROFILE_1\x10\x0f\x12\x19\n\x15HOTKEY_LOAD_PROFILE_2\x10\x10\x12\x19\n\x15HOTKEY_LOAD_PROFILE_3\x10\x11\x12\x19\n\x15HOTKEY_LOAD_PROFILE_4\x10\x12\x12\x14\n\x10HOTKEY_L3_BUTTON\x10\x13\x12\x14\n\x10HOTKEY_R3_BUTTON\x10\x14\x12\x1a\n\x16HOTKEY_TOUCHPAD_BUTTON\x10\x15\x12\x19\n\x15HOTKEY_REBOOT_DEFAULT\x10\x16\x12\x14\n\x10HOTKEY_B1_BUTTON\x10\x17\x12\x14\n\x10HOTKEY_B2_BUTTON\x10\x18\x12\x14\n\x10HOTKEY_B3_BUTTON\x10\x19\x12\x14\n\x10HOTKEY_B4_BUTTON\x10\x1a\x12\x14\n\x10HOTKEY_L1_BUTTON\x10\x1b\x12\x14\n\x10HOTKEY_R1_BUTTON\x10\x1c\x12\x14\n\x10HOTKEY_L2_BUTTON\x10\x1d\x12\x14\n\x10HOTKEY_R2_BUTTON\x10\x1e\x12\x14\n\x10HOTKEY_S1_BUTTON\x10\x1f\x12\x14\n\x10HOTKEY_S2_BUTTON\x10 \x12\x14\n\x10HOTKEY_A1_BUTTON\x10!\x12\x14\n\x10HOTKEY_A2_BUTTON\x10\"\x1a\x05\x92?\x02 \x00*c\n\x0fLEDFormat_Proto\x12\x12\n\x0eLED_FORMAT_GRB\x10\x00\x12\x12\n\x0eLED_FORMAT_RGB\x10\x01\x12\x13\n\x0fLED_FORMAT_GRBW\x10\x02\x12\x13\n\x0fLED_FORMAT_RGBW\x10\x03*\\\n\x0cShmupMixMode\x12!\n\x1dSHMUP_MIX_MODE_TURBO_PRIORITY\x10\x00\x12\"\n\x1eSHMUP_MIX_MODE_CHARGE_PRIORITY\x10\x01\x1a\x05\x92?\x02 \x00*T\n\x08PLEDType\x12\x1b\n\x0ePLED_TYPE_NONE\x10\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\x12\x11\n\rPLED_TYPE_PWM\x10\x00\x12\x11\n\rPLED_TYPE_RGB\x10\x01\x1a\x05\x92?\x02 \x00*\xa3\x01\n\x0f\x46orcedSetupMode\x12\x19\n\x15\x46ORCED_SETUP_MODE_OFF\x10\x00\x12&\n\"FORCED_SETUP_MODE_LOCK_MODE_SWITCH\x10\x01\x12%\n!FORCED_SETUP_MODE_LOCK_WEB_CONFIG\x10\x02\x12\x1f\n\x1b\x46ORCED_SETUP_MODE_LOCK_BOTH\x10\x03\x1a\x05\x92?\x02 \x00*g\n\x1e\x44ualDirectionalCombinationMode\x12\x0e\n\nMIXED_MODE\x10\x00\x12\x10\n\x0cGAMEPAD_MODE\x10\x01\x12\r\n\tDUAL_MODE\x10\x02\x12\r\n\tNONE_MODE\x10\x03\x1a\x05\x92?\x02 \x00*C\n\x11PS4ControllerType\x12\x12\n\x0ePS4_CONTROLLER\x10\x00\x12\x13\n\x0fPS4_ARCADESTICK\x10\x07\x1a\x05\x92?\x02 \x00*C\n\tMacroType\x12\x0c\n\x08ON_PRESS\x10\x01\x12\x12\n\x0eON_HOLD_REPEAT\x10\x02\x12\r\n\tON_TOGGLE\x10\x03\x1a\x05\x92?\x02 \x00*\xea\x01\n\tGPElement\x12\x15\n\x11GP_ELEMENT_WIDGET\x10\x00\x12\x15\n\x11GP_ELEMENT_SCREEN\x10\x01\x12\x19\n\x15GP_ELEMENT_BTN_BUTTON\x10\x02\x12\x19\n\x15GP_ELEMENT_DIR_BUTTON\x10\x03\x12\x19\n\x15GP_ELEMENT_PIN_BUTTON\x10\x04\x12\x14\n\x10GP_ELEMENT_LEVER\x10\x05\x12\x14\n\x10GP_ELEMENT_LABEL\x10\x06\x12\x15\n\x11GP_ELEMENT_SPRITE\x10\x07\x12\x14\n\x10GP_ELEMENT_SHAPE\x10\x08\x1a\x05\x92?\x02 \x00*~\n\x0cGPShape_Type\x12\x14\n\x10GP_SHAPE_ELLIPSE\x10\x00\x12\x13\n\x0fGP_SHAPE_SQUARE\x10\x01\x12\x14\n\x10GP_SHAPE_DIAMOND\x10\x02\x12\x14\n\x10GP_SHAPE_POLYGON\x10\x03\x12\x10\n\x0cGP_SHAPE_ARC\x10\x04\x1a\x05\x92?\x02 \x00*\xa7\x02\n\x14RotaryEncoderPinMode\x12\x15\n\x11\x45NCODER_MODE_NONE\x10\x00\x12\x1e\n\x1a\x45NCODER_MODE_LEFT_ANALOG_X\x10\x01\x12\x1e\n\x1a\x45NCODER_MODE_LEFT_ANALOG_Y\x10\x02\x12\x1f\n\x1b\x45NCODER_MODE_RIGHT_ANALOG_X\x10\x03\x12\x1f\n\x1b\x45NCODER_MODE_RIGHT_ANALOG_Y\x10\x04\x12\x1d\n\x19\x45NCODER_MODE_LEFT_TRIGGER\x10\x05\x12\x1e\n\x1a\x45NCODER_MODE_RIGHT_TRIGGER\x10\x06\x12\x17\n\x13\x45NCODER_MODE_DPAD_X\x10\x07\x12\x17\n\x13\x45NCODER_MODE_DPAD_Y\x10\x08\x1a\x05\x92?\x02 \x00')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0b\x65nums.proto\x1a\x0cnanopb.proto*\xbd\x08\n\x0c\x42uttonLayout\x12\x17\n\x13\x42UTTON_LAYOUT_STICK\x10\x00\x12\x1b\n\x17\x42UTTON_LAYOUT_STICKLESS\x10\x01\x12 \n\x1c\x42UTTON_LAYOUT_BUTTONS_ANGLED\x10\x02\x12\x1f\n\x1b\x42UTTON_LAYOUT_BUTTONS_BASIC\x10\x03\x12!\n\x1d\x42UTTON_LAYOUT_KEYBOARD_ANGLED\x10\x04\x12\x1b\n\x17\x42UTTON_LAYOUT_KEYBOARDA\x10\x05\x12\x1b\n\x17\x42UTTON_LAYOUT_DANCEPADA\x10\x06\x12\x1c\n\x18\x42UTTON_LAYOUT_TWINSTICKA\x10\x07\x12\x18\n\x14\x42UTTON_LAYOUT_BLANKA\x10\x08\x12\x16\n\x12\x42UTTON_LAYOUT_VLXA\x10\t\x12\"\n\x1e\x42UTTON_LAYOUT_FIGHTBOARD_STICK\x10\n\x12%\n!BUTTON_LAYOUT_FIGHTBOARD_MIRRORED\x10\x0b\x12\x19\n\x15\x42UTTON_LAYOUT_CUSTOMA\x10\x0c\x12 \n\x1c\x42UTTON_LAYOUT_OPENCORE0WASDA\x10\r\x12\x1e\n\x1a\x42UTTON_LAYOUT_STICKLESS_13\x10\x0e\x12\x1e\n\x1a\x42UTTON_LAYOUT_STICKLESS_16\x10\x0f\x12\x1e\n\x1a\x42UTTON_LAYOUT_STICKLESS_14\x10\x10\x12#\n\x1f\x42UTTON_LAYOUT_DANCEPAD_DDR_LEFT\x10\x11\x12#\n\x1f\x42UTTON_LAYOUT_DANCEPAD_DDR_SOLO\x10\x12\x12#\n\x1f\x42UTTON_LAYOUT_DANCEPAD_PIU_LEFT\x10\x13\x12\x18\n\x14\x42UTTON_LAYOUT_POPN_A\x10\x14\x12\x19\n\x15\x42UTTON_LAYOUT_TAIKO_A\x10\x15\x12 \n\x1c\x42UTTON_LAYOUT_BM_TURNTABLE_A\x10\x16\x12\x1b\n\x17\x42UTTON_LAYOUT_BM_5KEY_A\x10\x17\x12\x1b\n\x17\x42UTTON_LAYOUT_BM_7KEY_A\x10\x18\x12!\n\x1d\x42UTTON_LAYOUT_GITADORA_FRET_A\x10\x19\x12\"\n\x1e\x42UTTON_LAYOUT_GITADORA_STRUM_A\x10\x1a\x12!\n\x1d\x42UTTON_LAYOUT_BOARD_DEFINED_A\x10\x1b\x12!\n\x1d\x42UTTON_LAYOUT_BANDHERO_FRET_A\x10\x1c\x12\"\n\x1e\x42UTTON_LAYOUT_BANDHERO_STRUM_A\x10\x1d\x12\x19\n\x15\x42UTTON_LAYOUT_6GAWD_A\x10\x1e\x12#\n\x1f\x42UTTON_LAYOUT_6GAWD_ALLBUTTON_A\x10\x1f\x12\'\n#BUTTON_LAYOUT_6GAWD_ALLBUTTONPLUS_A\x10 \x1a\x05\x92?\x02 \x00*\x9c\t\n\x11\x42uttonLayoutRight\x12\x18\n\x14\x42UTTON_LAYOUT_ARCADE\x10\x00\x12\x1c\n\x18\x42UTTON_LAYOUT_STICKLESSB\x10\x01\x12!\n\x1d\x42UTTON_LAYOUT_BUTTONS_ANGLEDB\x10\x02\x12\x18\n\x14\x42UTTON_LAYOUT_VEWLIX\x10\x03\x12\x19\n\x15\x42UTTON_LAYOUT_VEWLIX7\x10\x04\x12\x18\n\x14\x42UTTON_LAYOUT_CAPCOM\x10\x05\x12\x19\n\x15\x42UTTON_LAYOUT_CAPCOM6\x10\x06\x12\x18\n\x14\x42UTTON_LAYOUT_SEGA2P\x10\x07\x12\x17\n\x13\x42UTTON_LAYOUT_NOIR8\x10\x08\x12\x1b\n\x17\x42UTTON_LAYOUT_KEYBOARDB\x10\t\x12\x1b\n\x17\x42UTTON_LAYOUT_DANCEPADB\x10\n\x12\x1c\n\x18\x42UTTON_LAYOUT_TWINSTICKB\x10\x0b\x12\x18\n\x14\x42UTTON_LAYOUT_BLANKB\x10\x0c\x12\x16\n\x12\x42UTTON_LAYOUT_VLXB\x10\r\x12\x1c\n\x18\x42UTTON_LAYOUT_FIGHTBOARD\x10\x0e\x12+\n\'BUTTON_LAYOUT_FIGHTBOARD_STICK_MIRRORED\x10\x0f\x12\x19\n\x15\x42UTTON_LAYOUT_CUSTOMB\x10\x10\x12\x1c\n\x18\x42UTTON_LAYOUT_KEYBOARD8B\x10\x11\x12 \n\x1c\x42UTTON_LAYOUT_OPENCORE0WASDB\x10\x12\x12\x1f\n\x1b\x42UTTON_LAYOUT_STICKLESS_13B\x10\x13\x12\x1f\n\x1b\x42UTTON_LAYOUT_STICKLESS_16B\x10\x14\x12\x1f\n\x1b\x42UTTON_LAYOUT_STICKLESS_14B\x10\x15\x12$\n BUTTON_LAYOUT_DANCEPAD_DDR_RIGHT\x10\x16\x12$\n BUTTON_LAYOUT_DANCEPAD_PIU_RIGHT\x10\x17\x12\x18\n\x14\x42UTTON_LAYOUT_POPN_B\x10\x18\x12\x19\n\x15\x42UTTON_LAYOUT_TAIKO_B\x10\x19\x12 \n\x1c\x42UTTON_LAYOUT_BM_TURNTABLE_B\x10\x1a\x12\x1b\n\x17\x42UTTON_LAYOUT_BM_5KEY_B\x10\x1b\x12\x1b\n\x17\x42UTTON_LAYOUT_BM_7KEY_B\x10\x1c\x12!\n\x1d\x42UTTON_LAYOUT_GITADORA_FRET_B\x10\x1d\x12\"\n\x1e\x42UTTON_LAYOUT_GITADORA_STRUM_B\x10\x1e\x12!\n\x1d\x42UTTON_LAYOUT_BOARD_DEFINED_B\x10\x1f\x12!\n\x1d\x42UTTON_LAYOUT_BANDHERO_FRET_B\x10 \x12\"\n\x1e\x42UTTON_LAYOUT_BANDHERO_STRUM_B\x10!\x12\x19\n\x15\x42UTTON_LAYOUT_6GAWD_B\x10\"\x12#\n\x1f\x42UTTON_LAYOUT_6GAWD_ALLBUTTON_B\x10#\x12\'\n#BUTTON_LAYOUT_6GAWD_ALLBUTTONPLUS_B\x10$\x1a\x05\x92?\x02 \x00*y\n\nSplashMode\x12\x16\n\x12SPLASH_MODE_STATIC\x10\x00\x12\x17\n\x13SPLASH_MODE_CLOSEIN\x10\x01\x12\x1d\n\x19SPLASH_MODE_CLOSEINCUSTOM\x10\x02\x12\x14\n\x10SPLASH_MODE_NONE\x10\x03\x1a\x05\x92?\x02 \x00*\xa0\x01\n\x0cSplashChoice\x12\x16\n\x12SPLASH_CHOICE_MAIN\x10\x00\x12\x13\n\x0fSPLASH_CHOICE_X\x10\x01\x12\x13\n\x0fSPLASH_CHOICE_Y\x10\x02\x12\x13\n\x0fSPLASH_CHOICE_Z\x10\x03\x12\x18\n\x14SPLASH_CHOICE_CUSTOM\x10\x04\x12\x18\n\x14SPLASH_CHOICE_LEGACY\x10\x05\x1a\x05\x92?\x02 \x00*\x99\x01\n\x0eOnBoardLedMode\x12\x19\n\x15ON_BOARD_LED_MODE_OFF\x10\x00\x12$\n ON_BOARD_LED_MODE_MODE_INDICATOR\x10\x01\x12 \n\x1cON_BOARD_LED_MODE_INPUT_TEST\x10\x02\x12\x1d\n\x19ON_BOARD_LED_MODE_PS_AUTH\x10\x03\x1a\x05\x92?\x02 \x00*\xec\x02\n\tInputMode\x12\x15\n\x11INPUT_MODE_XINPUT\x10\x00\x12\x15\n\x11INPUT_MODE_SWITCH\x10\x01\x12\x12\n\x0eINPUT_MODE_HID\x10\x02\x12\x17\n\x13INPUT_MODE_KEYBOARD\x10\x03\x12\x12\n\x0eINPUT_MODE_PS4\x10\x04\x12\x14\n\x10INPUT_MODE_XBONE\x10\x05\x12\x15\n\x11INPUT_MODE_MDMINI\x10\x06\x12\x15\n\x11INPUT_MODE_NEOGEO\x10\x07\x12\x16\n\x12INPUT_MODE_PCEMINI\x10\x08\x12\x14\n\x10INPUT_MODE_EGRET\x10\t\x12\x14\n\x10INPUT_MODE_ASTRO\x10\n\x12\x18\n\x14INPUT_MODE_PSCLASSIC\x10\x0b\x12\x1b\n\x17INPUT_MODE_XBOXORIGINAL\x10\x0c\x12\x12\n\x0eINPUT_MODE_PS5\x10\r\x12\x16\n\x11INPUT_MODE_CONFIG\x10\xff\x01\x1a\x05\x92?\x02 \x00*\x94\x01\n\x11InputModeAuthType\x12\x1d\n\x19INPUT_MODE_AUTH_TYPE_NONE\x10\x00\x12\x1d\n\x19INPUT_MODE_AUTH_TYPE_KEYS\x10\x01\x12\x1c\n\x18INPUT_MODE_AUTH_TYPE_USB\x10\x02\x12\x1c\n\x18INPUT_MODE_AUTH_TYPE_I2C\x10\x03\x1a\x05\x92?\x02 \x00*_\n\x08\x44padMode\x12\x15\n\x11\x44PAD_MODE_DIGITAL\x10\x00\x12\x19\n\x15\x44PAD_MODE_LEFT_ANALOG\x10\x01\x12\x1a\n\x16\x44PAD_MODE_RIGHT_ANALOG\x10\x02\x1a\x05\x92?\x02 \x00*O\n\nInvertMode\x12\x0f\n\x0bINVERT_NONE\x10\x00\x12\x0c\n\x08INVERT_X\x10\x01\x12\x0c\n\x08INVERT_Y\x10\x02\x12\r\n\tINVERT_XY\x10\x03\x1a\x05\x92?\x02 \x00*\xa2\x01\n\x08SOCDMode\x12\x19\n\x15SOCD_MODE_UP_PRIORITY\x10\x00\x12\x15\n\x11SOCD_MODE_NEUTRAL\x10\x01\x12#\n\x1fSOCD_MODE_SECOND_INPUT_PRIORITY\x10\x02\x12\"\n\x1eSOCD_MODE_FIRST_INPUT_PRIORITY\x10\x03\x12\x14\n\x10SOCD_MODE_BYPASS\x10\x04\x1a\x05\x92?\x02 \x00*\x88\x08\n\nGpioAction\x12\x11\n\x04NONE\x10\xf6\xff\xff\xff\xff\xff\xff\xff\xff\x01\x12\x15\n\x08RESERVED\x10\xfb\xff\xff\xff\xff\xff\xff\xff\xff\x01\x12\x15\n\x11\x41SSIGNED_TO_ADDON\x10\x00\x12\x13\n\x0f\x42UTTON_PRESS_UP\x10\x01\x12\x15\n\x11\x42UTTON_PRESS_DOWN\x10\x02\x12\x15\n\x11\x42UTTON_PRESS_LEFT\x10\x03\x12\x16\n\x12\x42UTTON_PRESS_RIGHT\x10\x04\x12\x13\n\x0f\x42UTTON_PRESS_B1\x10\x05\x12\x13\n\x0f\x42UTTON_PRESS_B2\x10\x06\x12\x13\n\x0f\x42UTTON_PRESS_B3\x10\x07\x12\x13\n\x0f\x42UTTON_PRESS_B4\x10\x08\x12\x13\n\x0f\x42UTTON_PRESS_L1\x10\t\x12\x13\n\x0f\x42UTTON_PRESS_R1\x10\n\x12\x13\n\x0f\x42UTTON_PRESS_L2\x10\x0b\x12\x13\n\x0f\x42UTTON_PRESS_R2\x10\x0c\x12\x13\n\x0f\x42UTTON_PRESS_S1\x10\r\x12\x13\n\x0f\x42UTTON_PRESS_S2\x10\x0e\x12\x13\n\x0f\x42UTTON_PRESS_A1\x10\x0f\x12\x13\n\x0f\x42UTTON_PRESS_A2\x10\x10\x12\x13\n\x0f\x42UTTON_PRESS_L3\x10\x11\x12\x13\n\x0f\x42UTTON_PRESS_R3\x10\x12\x12\x13\n\x0f\x42UTTON_PRESS_FN\x10\x13\x12\x17\n\x13\x42UTTON_PRESS_DDI_UP\x10\x14\x12\x19\n\x15\x42UTTON_PRESS_DDI_DOWN\x10\x15\x12\x19\n\x15\x42UTTON_PRESS_DDI_LEFT\x10\x16\x12\x1a\n\x16\x42UTTON_PRESS_DDI_RIGHT\x10\x17\x12\x16\n\x12SUSTAIN_DP_MODE_DP\x10\x18\x12\x16\n\x12SUSTAIN_DP_MODE_LS\x10\x19\x12\x16\n\x12SUSTAIN_DP_MODE_RS\x10\x1a\x12\x1d\n\x19SUSTAIN_SOCD_MODE_UP_PRIO\x10\x1b\x12\x1d\n\x19SUSTAIN_SOCD_MODE_NEUTRAL\x10\x1c\x12 \n\x1cSUSTAIN_SOCD_MODE_SECOND_WIN\x10\x1d\x12\x1f\n\x1bSUSTAIN_SOCD_MODE_FIRST_WIN\x10\x1e\x12\x1c\n\x18SUSTAIN_SOCD_MODE_BYPASS\x10\x1f\x12\x16\n\x12\x42UTTON_PRESS_TURBO\x10 \x12\x16\n\x12\x42UTTON_PRESS_MACRO\x10!\x12\x18\n\x14\x42UTTON_PRESS_MACRO_1\x10\"\x12\x18\n\x14\x42UTTON_PRESS_MACRO_2\x10#\x12\x18\n\x14\x42UTTON_PRESS_MACRO_3\x10$\x12\x18\n\x14\x42UTTON_PRESS_MACRO_4\x10%\x12\x18\n\x14\x42UTTON_PRESS_MACRO_5\x10&\x12\x18\n\x14\x42UTTON_PRESS_MACRO_6\x10\'\x1a\x05\x92?\x02 \x00*\x80\x07\n\rGamepadHotkey\x12\x0f\n\x0bHOTKEY_NONE\x10\x00\x12\x17\n\x13HOTKEY_DPAD_DIGITAL\x10\x01\x12\x1b\n\x17HOTKEY_DPAD_LEFT_ANALOG\x10\x02\x12\x1c\n\x18HOTKEY_DPAD_RIGHT_ANALOG\x10\x03\x12\x16\n\x12HOTKEY_HOME_BUTTON\x10\x04\x12\x19\n\x15HOTKEY_CAPTURE_BUTTON\x10\x05\x12\x1b\n\x17HOTKEY_SOCD_UP_PRIORITY\x10\x06\x12\x17\n\x13HOTKEY_SOCD_NEUTRAL\x10\x07\x12\x1a\n\x16HOTKEY_SOCD_LAST_INPUT\x10\x08\x12\x18\n\x14HOTKEY_INVERT_X_AXIS\x10\t\x12\x18\n\x14HOTKEY_INVERT_Y_AXIS\x10\n\x12\x1b\n\x17HOTKEY_SOCD_FIRST_INPUT\x10\x0b\x12\x16\n\x12HOTKEY_SOCD_BYPASS\x10\x0c\x12\x1c\n\x18HOTKEY_TOGGLE_4_WAY_MODE\x10\r\x12 \n\x1cHOTKEY_TOGGLE_DDI_4_WAY_MODE\x10\x0e\x12\x19\n\x15HOTKEY_LOAD_PROFILE_1\x10\x0f\x12\x19\n\x15HOTKEY_LOAD_PROFILE_2\x10\x10\x12\x19\n\x15HOTKEY_LOAD_PROFILE_3\x10\x11\x12\x19\n\x15HOTKEY_LOAD_PROFILE_4\x10\x12\x12\x14\n\x10HOTKEY_L3_BUTTON\x10\x13\x12\x14\n\x10HOTKEY_R3_BUTTON\x10\x14\x12\x1a\n\x16HOTKEY_TOUCHPAD_BUTTON\x10\x15\x12\x19\n\x15HOTKEY_REBOOT_DEFAULT\x10\x16\x12\x14\n\x10HOTKEY_B1_BUTTON\x10\x17\x12\x14\n\x10HOTKEY_B2_BUTTON\x10\x18\x12\x14\n\x10HOTKEY_B3_BUTTON\x10\x19\x12\x14\n\x10HOTKEY_B4_BUTTON\x10\x1a\x12\x14\n\x10HOTKEY_L1_BUTTON\x10\x1b\x12\x14\n\x10HOTKEY_R1_BUTTON\x10\x1c\x12\x14\n\x10HOTKEY_L2_BUTTON\x10\x1d\x12\x14\n\x10HOTKEY_R2_BUTTON\x10\x1e\x12\x14\n\x10HOTKEY_S1_BUTTON\x10\x1f\x12\x14\n\x10HOTKEY_S2_BUTTON\x10 \x12\x14\n\x10HOTKEY_A1_BUTTON\x10!\x12\x14\n\x10HOTKEY_A2_BUTTON\x10\"\x1a\x05\x92?\x02 \x00*c\n\x0fLEDFormat_Proto\x12\x12\n\x0eLED_FORMAT_GRB\x10\x00\x12\x12\n\x0eLED_FORMAT_RGB\x10\x01\x12\x13\n\x0fLED_FORMAT_GRBW\x10\x02\x12\x13\n\x0fLED_FORMAT_RGBW\x10\x03*\\\n\x0cShmupMixMode\x12!\n\x1dSHMUP_MIX_MODE_TURBO_PRIORITY\x10\x00\x12\"\n\x1eSHMUP_MIX_MODE_CHARGE_PRIORITY\x10\x01\x1a\x05\x92?\x02 \x00*T\n\x08PLEDType\x12\x1b\n\x0ePLED_TYPE_NONE\x10\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\x12\x11\n\rPLED_TYPE_PWM\x10\x00\x12\x11\n\rPLED_TYPE_RGB\x10\x01\x1a\x05\x92?\x02 \x00*\xa3\x01\n\x0f\x46orcedSetupMode\x12\x19\n\x15\x46ORCED_SETUP_MODE_OFF\x10\x00\x12&\n\"FORCED_SETUP_MODE_LOCK_MODE_SWITCH\x10\x01\x12%\n!FORCED_SETUP_MODE_LOCK_WEB_CONFIG\x10\x02\x12\x1f\n\x1b\x46ORCED_SETUP_MODE_LOCK_BOTH\x10\x03\x1a\x05\x92?\x02 \x00*g\n\x1e\x44ualDirectionalCombinationMode\x12\x0e\n\nMIXED_MODE\x10\x00\x12\x10\n\x0cGAMEPAD_MODE\x10\x01\x12\r\n\tDUAL_MODE\x10\x02\x12\r\n\tNONE_MODE\x10\x03\x1a\x05\x92?\x02 \x00*C\n\x11PS4ControllerType\x12\x12\n\x0ePS4_CONTROLLER\x10\x00\x12\x13\n\x0fPS4_ARCADESTICK\x10\x07\x1a\x05\x92?\x02 \x00*C\n\tMacroType\x12\x0c\n\x08ON_PRESS\x10\x01\x12\x12\n\x0eON_HOLD_REPEAT\x10\x02\x12\r\n\tON_TOGGLE\x10\x03\x1a\x05\x92?\x02 \x00*\xea\x01\n\tGPElement\x12\x15\n\x11GP_ELEMENT_WIDGET\x10\x00\x12\x15\n\x11GP_ELEMENT_SCREEN\x10\x01\x12\x19\n\x15GP_ELEMENT_BTN_BUTTON\x10\x02\x12\x19\n\x15GP_ELEMENT_DIR_BUTTON\x10\x03\x12\x19\n\x15GP_ELEMENT_PIN_BUTTON\x10\x04\x12\x14\n\x10GP_ELEMENT_LEVER\x10\x05\x12\x14\n\x10GP_ELEMENT_LABEL\x10\x06\x12\x15\n\x11GP_ELEMENT_SPRITE\x10\x07\x12\x14\n\x10GP_ELEMENT_SHAPE\x10\x08\x1a\x05\x92?\x02 \x00*{\n\x0cGPShape_Type\x12\x14\n\x10GP_SHAPE_ELLIPSE\x10\x00\x12\x13\n\x0fGP_SHAPE_SQUARE\x10\x01\x12\x11\n\rGP_SHAPE_LINE\x10\x02\x12\x14\n\x10GP_SHAPE_POLYGON\x10\x03\x12\x10\n\x0cGP_SHAPE_ARC\x10\x04\x1a\x05\x92?\x02 \x00*\xa7\x02\n\x14RotaryEncoderPinMode\x12\x15\n\x11\x45NCODER_MODE_NONE\x10\x00\x12\x1e\n\x1a\x45NCODER_MODE_LEFT_ANALOG_X\x10\x01\x12\x1e\n\x1a\x45NCODER_MODE_LEFT_ANALOG_Y\x10\x02\x12\x1f\n\x1b\x45NCODER_MODE_RIGHT_ANALOG_X\x10\x03\x12\x1f\n\x1b\x45NCODER_MODE_RIGHT_ANALOG_Y\x10\x04\x12\x1d\n\x19\x45NCODER_MODE_LEFT_TRIGGER\x10\x05\x12\x1e\n\x1a\x45NCODER_MODE_RIGHT_TRIGGER\x10\x06\x12\x17\n\x13\x45NCODER_MODE_DPAD_X\x10\x07\x12\x17\n\x13\x45NCODER_MODE_DPAD_Y\x10\x08\x1a\x05\x92?\x02 \x00')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'enums_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   _BUTTONLAYOUT._options = None
@@ -60,51 +60,51 @@
   _GPELEMENT._options = None
   _GPELEMENT._serialized_options = b'\222?\002 \000'
   _GPSHAPE_TYPE._options = None
   _GPSHAPE_TYPE._serialized_options = b'\222?\002 \000'
   _ROTARYENCODERPINMODE._options = None
   _ROTARYENCODERPINMODE._serialized_options = b'\222?\002 \000'
   _BUTTONLAYOUT._serialized_start=30
-  _BUTTONLAYOUT._serialized_end=939
-  _BUTTONLAYOUTRIGHT._serialized_start=942
-  _BUTTONLAYOUTRIGHT._serialized_end=1946
-  _SPLASHMODE._serialized_start=1948
-  _SPLASHMODE._serialized_end=2069
-  _SPLASHCHOICE._serialized_start=2072
-  _SPLASHCHOICE._serialized_end=2232
-  _ONBOARDLEDMODE._serialized_start=2235
-  _ONBOARDLEDMODE._serialized_end=2388
-  _INPUTMODE._serialized_start=2391
-  _INPUTMODE._serialized_end=2755
-  _INPUTMODEAUTHTYPE._serialized_start=2758
-  _INPUTMODEAUTHTYPE._serialized_end=2906
-  _DPADMODE._serialized_start=2908
-  _DPADMODE._serialized_end=3003
-  _INVERTMODE._serialized_start=3005
-  _INVERTMODE._serialized_end=3084
-  _SOCDMODE._serialized_start=3087
-  _SOCDMODE._serialized_end=3249
-  _GPIOACTION._serialized_start=3252
-  _GPIOACTION._serialized_end=4284
-  _GAMEPADHOTKEY._serialized_start=4287
-  _GAMEPADHOTKEY._serialized_end=5183
-  _LEDFORMAT_PROTO._serialized_start=5185
-  _LEDFORMAT_PROTO._serialized_end=5284
-  _SHMUPMIXMODE._serialized_start=5286
-  _SHMUPMIXMODE._serialized_end=5378
-  _PLEDTYPE._serialized_start=5380
-  _PLEDTYPE._serialized_end=5464
-  _FORCEDSETUPMODE._serialized_start=5467
-  _FORCEDSETUPMODE._serialized_end=5630
-  _DUALDIRECTIONALCOMBINATIONMODE._serialized_start=5632
-  _DUALDIRECTIONALCOMBINATIONMODE._serialized_end=5735
-  _PS4CONTROLLERTYPE._serialized_start=5737
-  _PS4CONTROLLERTYPE._serialized_end=5804
-  _MACROTYPE._serialized_start=5806
-  _MACROTYPE._serialized_end=5873
-  _GPELEMENT._serialized_start=5876
-  _GPELEMENT._serialized_end=6110
-  _GPSHAPE_TYPE._serialized_start=6112
-  _GPSHAPE_TYPE._serialized_end=6238
-  _ROTARYENCODERPINMODE._serialized_start=6241
-  _ROTARYENCODERPINMODE._serialized_end=6536
+  _BUTTONLAYOUT._serialized_end=1115
+  _BUTTONLAYOUTRIGHT._serialized_start=1118
+  _BUTTONLAYOUTRIGHT._serialized_end=2298
+  _SPLASHMODE._serialized_start=2300
+  _SPLASHMODE._serialized_end=2421
+  _SPLASHCHOICE._serialized_start=2424
+  _SPLASHCHOICE._serialized_end=2584
+  _ONBOARDLEDMODE._serialized_start=2587
+  _ONBOARDLEDMODE._serialized_end=2740
+  _INPUTMODE._serialized_start=2743
+  _INPUTMODE._serialized_end=3107
+  _INPUTMODEAUTHTYPE._serialized_start=3110
+  _INPUTMODEAUTHTYPE._serialized_end=3258
+  _DPADMODE._serialized_start=3260
+  _DPADMODE._serialized_end=3355
+  _INVERTMODE._serialized_start=3357
+  _INVERTMODE._serialized_end=3436
+  _SOCDMODE._serialized_start=3439
+  _SOCDMODE._serialized_end=3601
+  _GPIOACTION._serialized_start=3604
+  _GPIOACTION._serialized_end=4636
+  _GAMEPADHOTKEY._serialized_start=4639
+  _GAMEPADHOTKEY._serialized_end=5535
+  _LEDFORMAT_PROTO._serialized_start=5537
+  _LEDFORMAT_PROTO._serialized_end=5636
+  _SHMUPMIXMODE._serialized_start=5638
+  _SHMUPMIXMODE._serialized_end=5730
+  _PLEDTYPE._serialized_start=5732
+  _PLEDTYPE._serialized_end=5816
+  _FORCEDSETUPMODE._serialized_start=5819
+  _FORCEDSETUPMODE._serialized_end=5982
+  _DUALDIRECTIONALCOMBINATIONMODE._serialized_start=5984
+  _DUALDIRECTIONALCOMBINATIONMODE._serialized_end=6087
+  _PS4CONTROLLERTYPE._serialized_start=6089
+  _PS4CONTROLLERTYPE._serialized_end=6156
+  _MACROTYPE._serialized_start=6158
+  _MACROTYPE._serialized_end=6225
+  _GPELEMENT._serialized_start=6228
+  _GPELEMENT._serialized_end=6462
+  _GPSHAPE_TYPE._serialized_start=6464
+  _GPSHAPE_TYPE._serialized_end=6587
+  _ROTARYENCODERPINMODE._serialized_start=6590
+  _ROTARYENCODERPINMODE._serialized_end=6885
 # @@protoc_insertion_point(module_scope)
```

### Comparing `gp2040ce_binary_tools-0.8.3/gp2040ce_bintools/proto_snapshot/nanopb.proto` & `gp2040ce_binary_tools-0.9.0/gp2040ce_bintools/proto_snapshot/nanopb.proto`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.3/gp2040ce_bintools/proto_snapshot/nanopb_pb2.py` & `gp2040ce_binary_tools-0.9.0/gp2040ce_bintools/proto_snapshot/nanopb_pb2.py`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.3/gp2040ce_bintools/rp2040.py` & `gp2040ce_binary_tools-0.9.0/gp2040ce_bintools/rp2040.py`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.3/gp2040ce_bintools/storage.py` & `gp2040ce_binary_tools-0.9.0/gp2040ce_bintools/storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -237,29 +237,32 @@
         whole_board: optional, if true, attempt to find the storage section from its normal location on a board
         allow_no_file: if true, attempting to open a nonexistent file returns an empty config, else it errors
         board_config: if true, the board config is provided instead of the user config
     Returns:
         the parsed configuration
     """
     try:
-        content = get_binary_from_file(filename)
+        if filename[-5:] == '.json':
+            with open(filename) as file_:
+                return get_config_from_json(file_.read())
+        else:
+            content = get_binary_from_file(filename)
+            if whole_board:
+                if board_config:
+                    return get_config(get_board_storage_section(content))
+                else:
+                    return get_config(get_user_storage_section(content))
+            else:
+                return get_config(content)
     except FileNotFoundError:
         if not allow_no_file:
             raise
         config_pb2 = get_config_pb2()
         return config_pb2.Config()
 
-    if whole_board:
-        if board_config:
-            return get_config(get_board_storage_section(content))
-        else:
-            return get_config(get_user_storage_section(content))
-    else:
-        return get_config(content)
-
 
 def get_config_from_usb(address: int) -> tuple[Message, object, object]:
     """Read a config section from a USB device and provide the protobuf Message.
 
     Args:
         address: location of the flash to start reading from
     Returns:
```

### Comparing `gp2040ce_binary_tools-0.8.3/pyproject.toml` & `gp2040ce_binary_tools-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.3/requirements/requirements-dev.txt` & `gp2040ce_binary_tools-0.9.0/requirements/requirements-dev.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #
-# This file is autogenerated by pip-compile with Python 3.11
+# This file is autogenerated by pip-compile with Python 3.12
 # by the following command:
 #
 #    pip-compile --extra=dev --output-file=requirements/requirements-dev.txt
 #
-aiohttp==3.9.3
+aiohttp==3.9.5
     # via textual-dev
 aiosignal==1.3.1
     # via aiohttp
 attrs==23.2.0
     # via aiohttp
 bandit==1.7.8
     # via gp2040ce-binary-tools (pyproject.toml)
@@ -29,36 +29,36 @@
     #   tox
 click==8.1.7
     # via
     #   pip-tools
     #   textual-dev
 colorama==0.4.6
     # via tox
-coverage[toml]==7.4.4
+coverage[toml]==7.5.1
     # via pytest-cov
 decorator==5.1.1
     # via gp2040ce-binary-tools (pyproject.toml)
 distlib==0.3.8
     # via virtualenv
-filelock==3.13.3
+filelock==3.14.0
     # via
     #   tox
     #   virtualenv
 flake8==7.0.0
     # via
     #   flake8-builtins
     #   flake8-docstrings
     #   flake8-executable
     #   flake8-isort
     #   flake8-mutable
     #   flake8-pyproject
     #   gp2040ce-binary-tools (pyproject.toml)
 flake8-blind-except==0.2.1
     # via gp2040ce-binary-tools (pyproject.toml)
-flake8-builtins==2.4.0
+flake8-builtins==2.5.0
     # via gp2040ce-binary-tools (pyproject.toml)
 flake8-docstrings==1.7.0
     # via gp2040ce-binary-tools (pyproject.toml)
 flake8-executable==2.1.3
     # via gp2040ce-binary-tools (pyproject.toml)
 flake8-fixme==1.1.1
     # via gp2040ce-binary-tools (pyproject.toml)
@@ -70,94 +70,94 @@
     # via gp2040ce-binary-tools (pyproject.toml)
 flake8-pyproject==1.2.3
     # via gp2040ce-binary-tools (pyproject.toml)
 frozenlist==1.4.1
     # via
     #   aiohttp
     #   aiosignal
-grpcio==1.62.1
+grpcio==1.64.0
     # via grpcio-tools
-grpcio-tools==1.62.1
+grpcio-tools==1.64.0
     # via gp2040ce-binary-tools (pyproject.toml)
-idna==3.6
+idna==3.7
     # via yarl
 iniconfig==2.0.0
     # via pytest
 isort==5.13.2
     # via flake8-isort
-jinja2==3.1.3
+jinja2==3.1.4
     # via reuse
 license-expression==30.3.0
     # via reuse
 linkify-it-py==2.0.3
     # via markdown-it-py
 markdown-it-py[linkify,plugins]==3.0.0
     # via
     #   mdit-py-plugins
     #   rich
     #   textual
 markupsafe==2.1.5
     # via jinja2
 mccabe==0.7.0
     # via flake8
-mdit-py-plugins==0.4.0
+mdit-py-plugins==0.4.1
     # via markdown-it-py
 mdurl==0.1.2
     # via markdown-it-py
 msgpack==1.0.8
     # via textual-dev
 multidict==6.0.5
     # via
     #   aiohttp
     #   yarl
-mypy==1.9.0
+mypy==1.10.0
     # via gp2040ce-binary-tools (pyproject.toml)
 mypy-extensions==1.0.0
     # via mypy
 packaging==24.0
     # via
     #   build
     #   pyproject-api
     #   pytest
     #   setuptools-scm
     #   tox
 pbr==6.0.0
     # via stevedore
 pip-tools==7.4.1
     # via gp2040ce-binary-tools (pyproject.toml)
-platformdirs==4.2.0
+platformdirs==4.2.2
     # via
     #   tox
     #   virtualenv
-pluggy==1.4.0
+pluggy==1.5.0
     # via
     #   pytest
     #   tox
-protobuf==4.25.3
+protobuf==5.26.1
     # via grpcio-tools
 pycodestyle==2.11.1
     # via flake8
 pydocstyle==6.3.0
     # via flake8-docstrings
 pyflakes==3.2.0
     # via flake8
-pygments==2.17.2
+pygments==2.18.0
     # via rich
 pyproject-api==1.6.1
     # via tox
-pyproject-hooks==1.0.0
+pyproject-hooks==1.1.0
     # via
     #   build
     #   pip-tools
-pytest==8.1.1
+pytest==8.2.1
     # via
     #   gp2040ce-binary-tools (pyproject.toml)
     #   pytest-asyncio
     #   pytest-cov
-pytest-asyncio==0.23.6
+pytest-asyncio==0.23.7
     # via gp2040ce-binary-tools (pyproject.toml)
 pytest-cov==5.0.0
     # via gp2040ce-binary-tools (pyproject.toml)
 python-debian==0.1.49
     # via reuse
 pyusb==1.2.1
     # via gp2040ce-binary-tools (pyproject.toml)
@@ -165,37 +165,36 @@
     # via bandit
 reuse==3.0.2
     # via gp2040ce-binary-tools (pyproject.toml)
 rich==13.7.1
     # via
     #   bandit
     #   textual
-setuptools-scm==8.0.4
+setuptools-scm==8.1.0
     # via gp2040ce-binary-tools (pyproject.toml)
 snowballstemmer==2.2.0
     # via pydocstyle
 stevedore==5.2.0
     # via bandit
-textual==0.56.2
+textual==0.62.0
     # via
     #   gp2040ce-binary-tools (pyproject.toml)
     #   textual-dev
 textual-dev==1.5.1
     # via gp2040ce-binary-tools (pyproject.toml)
-tox==4.14.2
+tox==4.15.0
     # via gp2040ce-binary-tools (pyproject.toml)
 typing-extensions==4.11.0
     # via
     #   mypy
-    #   setuptools-scm
     #   textual
     #   textual-dev
 uc-micro-py==1.0.3
     # via linkify-it-py
-virtualenv==20.25.1
+virtualenv==20.26.2
     # via tox
 wheel==0.43.0
     # via pip-tools
 yarl==1.9.4
     # via aiohttp
 
 # The following packages are considered to be unsafe in a requirements file:
```

### Comparing `gp2040ce_binary_tools-0.8.3/requirements/requirements.txt` & `gp2040ce_binary_tools-0.9.0/requirements/requirements.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 #
-# This file is autogenerated by pip-compile with Python 3.11
+# This file is autogenerated by pip-compile with Python 3.12
 # by the following command:
 #
 #    pip-compile --output-file=requirements/requirements.txt
 #
-grpcio==1.62.1
+grpcio==1.64.0
     # via grpcio-tools
-grpcio-tools==1.62.1
+grpcio-tools==1.64.0
     # via gp2040ce-binary-tools (pyproject.toml)
 linkify-it-py==2.0.3
     # via markdown-it-py
 markdown-it-py[linkify,plugins]==3.0.0
     # via
     #   mdit-py-plugins
     #   rich
     #   textual
-mdit-py-plugins==0.4.0
+mdit-py-plugins==0.4.1
     # via markdown-it-py
 mdurl==0.1.2
     # via markdown-it-py
-protobuf==4.25.3
+protobuf==5.26.1
     # via grpcio-tools
-pygments==2.17.2
+pygments==2.18.0
     # via rich
 pyusb==1.2.1
     # via gp2040ce-binary-tools (pyproject.toml)
 rich==13.7.1
     # via textual
-textual==0.56.2
+textual==0.62.0
     # via gp2040ce-binary-tools (pyproject.toml)
 typing-extensions==4.11.0
     # via textual
 uc-micro-py==1.0.3
     # via linkify-it-py
 
 # The following packages are considered to be unsafe in a requirements file:
```

### Comparing `gp2040ce_binary_tools-0.8.3/tests/conftest.py` & `gp2040ce_binary_tools-0.9.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.3/tests/test-files/pb2-files/config_pb2.py` & `gp2040ce_binary_tools-0.9.0/tests/test-files/pb2-files/config_pb2.py`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.3/tests/test-files/pb2-files/enums_pb2.py` & `gp2040ce_binary_tools-0.9.0/tests/test-files/pb2-files/enums_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 _sym_db = _symbol_database.Default()
 
 
 import nanopb_pb2 as nanopb__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0b\x65nums.proto\x1a\x0cnanopb.proto*\x8d\x07\n\x0c\x42uttonLayout\x12\x17\n\x13\x42UTTON_LAYOUT_STICK\x10\x00\x12\x1b\n\x17\x42UTTON_LAYOUT_STICKLESS\x10\x01\x12 \n\x1c\x42UTTON_LAYOUT_BUTTONS_ANGLED\x10\x02\x12\x1f\n\x1b\x42UTTON_LAYOUT_BUTTONS_BASIC\x10\x03\x12!\n\x1d\x42UTTON_LAYOUT_KEYBOARD_ANGLED\x10\x04\x12\x1b\n\x17\x42UTTON_LAYOUT_KEYBOARDA\x10\x05\x12\x1b\n\x17\x42UTTON_LAYOUT_DANCEPADA\x10\x06\x12\x1c\n\x18\x42UTTON_LAYOUT_TWINSTICKA\x10\x07\x12\x18\n\x14\x42UTTON_LAYOUT_BLANKA\x10\x08\x12\x16\n\x12\x42UTTON_LAYOUT_VLXA\x10\t\x12\"\n\x1e\x42UTTON_LAYOUT_FIGHTBOARD_STICK\x10\n\x12%\n!BUTTON_LAYOUT_FIGHTBOARD_MIRRORED\x10\x0b\x12\x19\n\x15\x42UTTON_LAYOUT_CUSTOMA\x10\x0c\x12 \n\x1c\x42UTTON_LAYOUT_OPENCORE0WASDA\x10\r\x12\x1e\n\x1a\x42UTTON_LAYOUT_STICKLESS_13\x10\x0e\x12\x1e\n\x1a\x42UTTON_LAYOUT_STICKLESS_16\x10\x0f\x12\x1e\n\x1a\x42UTTON_LAYOUT_STICKLESS_14\x10\x10\x12#\n\x1f\x42UTTON_LAYOUT_DANCEPAD_DDR_LEFT\x10\x11\x12#\n\x1f\x42UTTON_LAYOUT_DANCEPAD_DDR_SOLO\x10\x12\x12#\n\x1f\x42UTTON_LAYOUT_DANCEPAD_PIU_LEFT\x10\x13\x12\x18\n\x14\x42UTTON_LAYOUT_POPN_A\x10\x14\x12\x19\n\x15\x42UTTON_LAYOUT_TAIKO_A\x10\x15\x12 \n\x1c\x42UTTON_LAYOUT_BM_TURNTABLE_A\x10\x16\x12\x1b\n\x17\x42UTTON_LAYOUT_BM_5KEY_A\x10\x17\x12\x1b\n\x17\x42UTTON_LAYOUT_BM_7KEY_A\x10\x18\x12!\n\x1d\x42UTTON_LAYOUT_GITADORA_FRET_A\x10\x19\x12\"\n\x1e\x42UTTON_LAYOUT_GITADORA_STRUM_A\x10\x1a\x12!\n\x1d\x42UTTON_LAYOUT_BOARD_DEFINED_A\x10\x1b\x1a\x05\x92?\x02 \x00*\xec\x07\n\x11\x42uttonLayoutRight\x12\x18\n\x14\x42UTTON_LAYOUT_ARCADE\x10\x00\x12\x1c\n\x18\x42UTTON_LAYOUT_STICKLESSB\x10\x01\x12!\n\x1d\x42UTTON_LAYOUT_BUTTONS_ANGLEDB\x10\x02\x12\x18\n\x14\x42UTTON_LAYOUT_VEWLIX\x10\x03\x12\x19\n\x15\x42UTTON_LAYOUT_VEWLIX7\x10\x04\x12\x18\n\x14\x42UTTON_LAYOUT_CAPCOM\x10\x05\x12\x19\n\x15\x42UTTON_LAYOUT_CAPCOM6\x10\x06\x12\x18\n\x14\x42UTTON_LAYOUT_SEGA2P\x10\x07\x12\x17\n\x13\x42UTTON_LAYOUT_NOIR8\x10\x08\x12\x1b\n\x17\x42UTTON_LAYOUT_KEYBOARDB\x10\t\x12\x1b\n\x17\x42UTTON_LAYOUT_DANCEPADB\x10\n\x12\x1c\n\x18\x42UTTON_LAYOUT_TWINSTICKB\x10\x0b\x12\x18\n\x14\x42UTTON_LAYOUT_BLANKB\x10\x0c\x12\x16\n\x12\x42UTTON_LAYOUT_VLXB\x10\r\x12\x1c\n\x18\x42UTTON_LAYOUT_FIGHTBOARD\x10\x0e\x12+\n\'BUTTON_LAYOUT_FIGHTBOARD_STICK_MIRRORED\x10\x0f\x12\x19\n\x15\x42UTTON_LAYOUT_CUSTOMB\x10\x10\x12\x1c\n\x18\x42UTTON_LAYOUT_KEYBOARD8B\x10\x11\x12 \n\x1c\x42UTTON_LAYOUT_OPENCORE0WASDB\x10\x12\x12\x1f\n\x1b\x42UTTON_LAYOUT_STICKLESS_13B\x10\x13\x12\x1f\n\x1b\x42UTTON_LAYOUT_STICKLESS_16B\x10\x14\x12\x1f\n\x1b\x42UTTON_LAYOUT_STICKLESS_14B\x10\x15\x12$\n BUTTON_LAYOUT_DANCEPAD_DDR_RIGHT\x10\x16\x12$\n BUTTON_LAYOUT_DANCEPAD_PIU_RIGHT\x10\x17\x12\x18\n\x14\x42UTTON_LAYOUT_POPN_B\x10\x18\x12\x19\n\x15\x42UTTON_LAYOUT_TAIKO_B\x10\x19\x12 \n\x1c\x42UTTON_LAYOUT_BM_TURNTABLE_B\x10\x1a\x12\x1b\n\x17\x42UTTON_LAYOUT_BM_5KEY_B\x10\x1b\x12\x1b\n\x17\x42UTTON_LAYOUT_BM_7KEY_B\x10\x1c\x12!\n\x1d\x42UTTON_LAYOUT_GITADORA_FRET_B\x10\x1d\x12\"\n\x1e\x42UTTON_LAYOUT_GITADORA_STRUM_B\x10\x1e\x12!\n\x1d\x42UTTON_LAYOUT_BOARD_DEFINED_B\x10\x1f\x1a\x05\x92?\x02 \x00*y\n\nSplashMode\x12\x16\n\x12SPLASH_MODE_STATIC\x10\x00\x12\x17\n\x13SPLASH_MODE_CLOSEIN\x10\x01\x12\x1d\n\x19SPLASH_MODE_CLOSEINCUSTOM\x10\x02\x12\x14\n\x10SPLASH_MODE_NONE\x10\x03\x1a\x05\x92?\x02 \x00*\xa0\x01\n\x0cSplashChoice\x12\x16\n\x12SPLASH_CHOICE_MAIN\x10\x00\x12\x13\n\x0fSPLASH_CHOICE_X\x10\x01\x12\x13\n\x0fSPLASH_CHOICE_Y\x10\x02\x12\x13\n\x0fSPLASH_CHOICE_Z\x10\x03\x12\x18\n\x14SPLASH_CHOICE_CUSTOM\x10\x04\x12\x18\n\x14SPLASH_CHOICE_LEGACY\x10\x05\x1a\x05\x92?\x02 \x00*\x99\x01\n\x0eOnBoardLedMode\x12\x19\n\x15ON_BOARD_LED_MODE_OFF\x10\x00\x12$\n ON_BOARD_LED_MODE_MODE_INDICATOR\x10\x01\x12 \n\x1cON_BOARD_LED_MODE_INPUT_TEST\x10\x02\x12\x1d\n\x19ON_BOARD_LED_MODE_PS_AUTH\x10\x03\x1a\x05\x92?\x02 \x00*\xec\x02\n\tInputMode\x12\x15\n\x11INPUT_MODE_XINPUT\x10\x00\x12\x15\n\x11INPUT_MODE_SWITCH\x10\x01\x12\x12\n\x0eINPUT_MODE_HID\x10\x02\x12\x17\n\x13INPUT_MODE_KEYBOARD\x10\x03\x12\x12\n\x0eINPUT_MODE_PS4\x10\x04\x12\x14\n\x10INPUT_MODE_XBONE\x10\x05\x12\x15\n\x11INPUT_MODE_MDMINI\x10\x06\x12\x15\n\x11INPUT_MODE_NEOGEO\x10\x07\x12\x16\n\x12INPUT_MODE_PCEMINI\x10\x08\x12\x14\n\x10INPUT_MODE_EGRET\x10\t\x12\x14\n\x10INPUT_MODE_ASTRO\x10\n\x12\x18\n\x14INPUT_MODE_PSCLASSIC\x10\x0b\x12\x1b\n\x17INPUT_MODE_XBOXORIGINAL\x10\x0c\x12\x12\n\x0eINPUT_MODE_PS5\x10\r\x12\x16\n\x11INPUT_MODE_CONFIG\x10\xff\x01\x1a\x05\x92?\x02 \x00*\x94\x01\n\x11InputModeAuthType\x12\x1d\n\x19INPUT_MODE_AUTH_TYPE_NONE\x10\x00\x12\x1d\n\x19INPUT_MODE_AUTH_TYPE_KEYS\x10\x01\x12\x1c\n\x18INPUT_MODE_AUTH_TYPE_USB\x10\x02\x12\x1c\n\x18INPUT_MODE_AUTH_TYPE_I2C\x10\x03\x1a\x05\x92?\x02 \x00*_\n\x08\x44padMode\x12\x15\n\x11\x44PAD_MODE_DIGITAL\x10\x00\x12\x19\n\x15\x44PAD_MODE_LEFT_ANALOG\x10\x01\x12\x1a\n\x16\x44PAD_MODE_RIGHT_ANALOG\x10\x02\x1a\x05\x92?\x02 \x00*O\n\nInvertMode\x12\x0f\n\x0bINVERT_NONE\x10\x00\x12\x0c\n\x08INVERT_X\x10\x01\x12\x0c\n\x08INVERT_Y\x10\x02\x12\r\n\tINVERT_XY\x10\x03\x1a\x05\x92?\x02 \x00*\xa2\x01\n\x08SOCDMode\x12\x19\n\x15SOCD_MODE_UP_PRIORITY\x10\x00\x12\x15\n\x11SOCD_MODE_NEUTRAL\x10\x01\x12#\n\x1fSOCD_MODE_SECOND_INPUT_PRIORITY\x10\x02\x12\"\n\x1eSOCD_MODE_FIRST_INPUT_PRIORITY\x10\x03\x12\x14\n\x10SOCD_MODE_BYPASS\x10\x04\x1a\x05\x92?\x02 \x00*\x88\x08\n\nGpioAction\x12\x11\n\x04NONE\x10\xf6\xff\xff\xff\xff\xff\xff\xff\xff\x01\x12\x15\n\x08RESERVED\x10\xfb\xff\xff\xff\xff\xff\xff\xff\xff\x01\x12\x15\n\x11\x41SSIGNED_TO_ADDON\x10\x00\x12\x13\n\x0f\x42UTTON_PRESS_UP\x10\x01\x12\x15\n\x11\x42UTTON_PRESS_DOWN\x10\x02\x12\x15\n\x11\x42UTTON_PRESS_LEFT\x10\x03\x12\x16\n\x12\x42UTTON_PRESS_RIGHT\x10\x04\x12\x13\n\x0f\x42UTTON_PRESS_B1\x10\x05\x12\x13\n\x0f\x42UTTON_PRESS_B2\x10\x06\x12\x13\n\x0f\x42UTTON_PRESS_B3\x10\x07\x12\x13\n\x0f\x42UTTON_PRESS_B4\x10\x08\x12\x13\n\x0f\x42UTTON_PRESS_L1\x10\t\x12\x13\n\x0f\x42UTTON_PRESS_R1\x10\n\x12\x13\n\x0f\x42UTTON_PRESS_L2\x10\x0b\x12\x13\n\x0f\x42UTTON_PRESS_R2\x10\x0c\x12\x13\n\x0f\x42UTTON_PRESS_S1\x10\r\x12\x13\n\x0f\x42UTTON_PRESS_S2\x10\x0e\x12\x13\n\x0f\x42UTTON_PRESS_A1\x10\x0f\x12\x13\n\x0f\x42UTTON_PRESS_A2\x10\x10\x12\x13\n\x0f\x42UTTON_PRESS_L3\x10\x11\x12\x13\n\x0f\x42UTTON_PRESS_R3\x10\x12\x12\x13\n\x0f\x42UTTON_PRESS_FN\x10\x13\x12\x17\n\x13\x42UTTON_PRESS_DDI_UP\x10\x14\x12\x19\n\x15\x42UTTON_PRESS_DDI_DOWN\x10\x15\x12\x19\n\x15\x42UTTON_PRESS_DDI_LEFT\x10\x16\x12\x1a\n\x16\x42UTTON_PRESS_DDI_RIGHT\x10\x17\x12\x16\n\x12SUSTAIN_DP_MODE_DP\x10\x18\x12\x16\n\x12SUSTAIN_DP_MODE_LS\x10\x19\x12\x16\n\x12SUSTAIN_DP_MODE_RS\x10\x1a\x12\x1d\n\x19SUSTAIN_SOCD_MODE_UP_PRIO\x10\x1b\x12\x1d\n\x19SUSTAIN_SOCD_MODE_NEUTRAL\x10\x1c\x12 \n\x1cSUSTAIN_SOCD_MODE_SECOND_WIN\x10\x1d\x12\x1f\n\x1bSUSTAIN_SOCD_MODE_FIRST_WIN\x10\x1e\x12\x1c\n\x18SUSTAIN_SOCD_MODE_BYPASS\x10\x1f\x12\x16\n\x12\x42UTTON_PRESS_TURBO\x10 \x12\x16\n\x12\x42UTTON_PRESS_MACRO\x10!\x12\x18\n\x14\x42UTTON_PRESS_MACRO_1\x10\"\x12\x18\n\x14\x42UTTON_PRESS_MACRO_2\x10#\x12\x18\n\x14\x42UTTON_PRESS_MACRO_3\x10$\x12\x18\n\x14\x42UTTON_PRESS_MACRO_4\x10%\x12\x18\n\x14\x42UTTON_PRESS_MACRO_5\x10&\x12\x18\n\x14\x42UTTON_PRESS_MACRO_6\x10\'\x1a\x05\x92?\x02 \x00*\x80\x07\n\rGamepadHotkey\x12\x0f\n\x0bHOTKEY_NONE\x10\x00\x12\x17\n\x13HOTKEY_DPAD_DIGITAL\x10\x01\x12\x1b\n\x17HOTKEY_DPAD_LEFT_ANALOG\x10\x02\x12\x1c\n\x18HOTKEY_DPAD_RIGHT_ANALOG\x10\x03\x12\x16\n\x12HOTKEY_HOME_BUTTON\x10\x04\x12\x19\n\x15HOTKEY_CAPTURE_BUTTON\x10\x05\x12\x1b\n\x17HOTKEY_SOCD_UP_PRIORITY\x10\x06\x12\x17\n\x13HOTKEY_SOCD_NEUTRAL\x10\x07\x12\x1a\n\x16HOTKEY_SOCD_LAST_INPUT\x10\x08\x12\x18\n\x14HOTKEY_INVERT_X_AXIS\x10\t\x12\x18\n\x14HOTKEY_INVERT_Y_AXIS\x10\n\x12\x1b\n\x17HOTKEY_SOCD_FIRST_INPUT\x10\x0b\x12\x16\n\x12HOTKEY_SOCD_BYPASS\x10\x0c\x12\x1c\n\x18HOTKEY_TOGGLE_4_WAY_MODE\x10\r\x12 \n\x1cHOTKEY_TOGGLE_DDI_4_WAY_MODE\x10\x0e\x12\x19\n\x15HOTKEY_LOAD_PROFILE_1\x10\x0f\x12\x19\n\x15HOTKEY_LOAD_PROFILE_2\x10\x10\x12\x19\n\x15HOTKEY_LOAD_PROFILE_3\x10\x11\x12\x19\n\x15HOTKEY_LOAD_PROFILE_4\x10\x12\x12\x14\n\x10HOTKEY_L3_BUTTON\x10\x13\x12\x14\n\x10HOTKEY_R3_BUTTON\x10\x14\x12\x1a\n\x16HOTKEY_TOUCHPAD_BUTTON\x10\x15\x12\x19\n\x15HOTKEY_REBOOT_DEFAULT\x10\x16\x12\x14\n\x10HOTKEY_B1_BUTTON\x10\x17\x12\x14\n\x10HOTKEY_B2_BUTTON\x10\x18\x12\x14\n\x10HOTKEY_B3_BUTTON\x10\x19\x12\x14\n\x10HOTKEY_B4_BUTTON\x10\x1a\x12\x14\n\x10HOTKEY_L1_BUTTON\x10\x1b\x12\x14\n\x10HOTKEY_R1_BUTTON\x10\x1c\x12\x14\n\x10HOTKEY_L2_BUTTON\x10\x1d\x12\x14\n\x10HOTKEY_R2_BUTTON\x10\x1e\x12\x14\n\x10HOTKEY_S1_BUTTON\x10\x1f\x12\x14\n\x10HOTKEY_S2_BUTTON\x10 \x12\x14\n\x10HOTKEY_A1_BUTTON\x10!\x12\x14\n\x10HOTKEY_A2_BUTTON\x10\"\x1a\x05\x92?\x02 \x00*c\n\x0fLEDFormat_Proto\x12\x12\n\x0eLED_FORMAT_GRB\x10\x00\x12\x12\n\x0eLED_FORMAT_RGB\x10\x01\x12\x13\n\x0fLED_FORMAT_GRBW\x10\x02\x12\x13\n\x0fLED_FORMAT_RGBW\x10\x03*\\\n\x0cShmupMixMode\x12!\n\x1dSHMUP_MIX_MODE_TURBO_PRIORITY\x10\x00\x12\"\n\x1eSHMUP_MIX_MODE_CHARGE_PRIORITY\x10\x01\x1a\x05\x92?\x02 \x00*T\n\x08PLEDType\x12\x1b\n\x0ePLED_TYPE_NONE\x10\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\x12\x11\n\rPLED_TYPE_PWM\x10\x00\x12\x11\n\rPLED_TYPE_RGB\x10\x01\x1a\x05\x92?\x02 \x00*\xa3\x01\n\x0f\x46orcedSetupMode\x12\x19\n\x15\x46ORCED_SETUP_MODE_OFF\x10\x00\x12&\n\"FORCED_SETUP_MODE_LOCK_MODE_SWITCH\x10\x01\x12%\n!FORCED_SETUP_MODE_LOCK_WEB_CONFIG\x10\x02\x12\x1f\n\x1b\x46ORCED_SETUP_MODE_LOCK_BOTH\x10\x03\x1a\x05\x92?\x02 \x00*g\n\x1e\x44ualDirectionalCombinationMode\x12\x0e\n\nMIXED_MODE\x10\x00\x12\x10\n\x0cGAMEPAD_MODE\x10\x01\x12\r\n\tDUAL_MODE\x10\x02\x12\r\n\tNONE_MODE\x10\x03\x1a\x05\x92?\x02 \x00*C\n\x11PS4ControllerType\x12\x12\n\x0ePS4_CONTROLLER\x10\x00\x12\x13\n\x0fPS4_ARCADESTICK\x10\x07\x1a\x05\x92?\x02 \x00*C\n\tMacroType\x12\x0c\n\x08ON_PRESS\x10\x01\x12\x12\n\x0eON_HOLD_REPEAT\x10\x02\x12\r\n\tON_TOGGLE\x10\x03\x1a\x05\x92?\x02 \x00*\xea\x01\n\tGPElement\x12\x15\n\x11GP_ELEMENT_WIDGET\x10\x00\x12\x15\n\x11GP_ELEMENT_SCREEN\x10\x01\x12\x19\n\x15GP_ELEMENT_BTN_BUTTON\x10\x02\x12\x19\n\x15GP_ELEMENT_DIR_BUTTON\x10\x03\x12\x19\n\x15GP_ELEMENT_PIN_BUTTON\x10\x04\x12\x14\n\x10GP_ELEMENT_LEVER\x10\x05\x12\x14\n\x10GP_ELEMENT_LABEL\x10\x06\x12\x15\n\x11GP_ELEMENT_SPRITE\x10\x07\x12\x14\n\x10GP_ELEMENT_SHAPE\x10\x08\x1a\x05\x92?\x02 \x00*~\n\x0cGPShape_Type\x12\x14\n\x10GP_SHAPE_ELLIPSE\x10\x00\x12\x13\n\x0fGP_SHAPE_SQUARE\x10\x01\x12\x14\n\x10GP_SHAPE_DIAMOND\x10\x02\x12\x14\n\x10GP_SHAPE_POLYGON\x10\x03\x12\x10\n\x0cGP_SHAPE_ARC\x10\x04\x1a\x05\x92?\x02 \x00*\xa7\x02\n\x14RotaryEncoderPinMode\x12\x15\n\x11\x45NCODER_MODE_NONE\x10\x00\x12\x1e\n\x1a\x45NCODER_MODE_LEFT_ANALOG_X\x10\x01\x12\x1e\n\x1a\x45NCODER_MODE_LEFT_ANALOG_Y\x10\x02\x12\x1f\n\x1b\x45NCODER_MODE_RIGHT_ANALOG_X\x10\x03\x12\x1f\n\x1b\x45NCODER_MODE_RIGHT_ANALOG_Y\x10\x04\x12\x1d\n\x19\x45NCODER_MODE_LEFT_TRIGGER\x10\x05\x12\x1e\n\x1a\x45NCODER_MODE_RIGHT_TRIGGER\x10\x06\x12\x17\n\x13\x45NCODER_MODE_DPAD_X\x10\x07\x12\x17\n\x13\x45NCODER_MODE_DPAD_Y\x10\x08\x1a\x05\x92?\x02 \x00')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0b\x65nums.proto\x1a\x0cnanopb.proto*\xbd\x08\n\x0c\x42uttonLayout\x12\x17\n\x13\x42UTTON_LAYOUT_STICK\x10\x00\x12\x1b\n\x17\x42UTTON_LAYOUT_STICKLESS\x10\x01\x12 \n\x1c\x42UTTON_LAYOUT_BUTTONS_ANGLED\x10\x02\x12\x1f\n\x1b\x42UTTON_LAYOUT_BUTTONS_BASIC\x10\x03\x12!\n\x1d\x42UTTON_LAYOUT_KEYBOARD_ANGLED\x10\x04\x12\x1b\n\x17\x42UTTON_LAYOUT_KEYBOARDA\x10\x05\x12\x1b\n\x17\x42UTTON_LAYOUT_DANCEPADA\x10\x06\x12\x1c\n\x18\x42UTTON_LAYOUT_TWINSTICKA\x10\x07\x12\x18\n\x14\x42UTTON_LAYOUT_BLANKA\x10\x08\x12\x16\n\x12\x42UTTON_LAYOUT_VLXA\x10\t\x12\"\n\x1e\x42UTTON_LAYOUT_FIGHTBOARD_STICK\x10\n\x12%\n!BUTTON_LAYOUT_FIGHTBOARD_MIRRORED\x10\x0b\x12\x19\n\x15\x42UTTON_LAYOUT_CUSTOMA\x10\x0c\x12 \n\x1c\x42UTTON_LAYOUT_OPENCORE0WASDA\x10\r\x12\x1e\n\x1a\x42UTTON_LAYOUT_STICKLESS_13\x10\x0e\x12\x1e\n\x1a\x42UTTON_LAYOUT_STICKLESS_16\x10\x0f\x12\x1e\n\x1a\x42UTTON_LAYOUT_STICKLESS_14\x10\x10\x12#\n\x1f\x42UTTON_LAYOUT_DANCEPAD_DDR_LEFT\x10\x11\x12#\n\x1f\x42UTTON_LAYOUT_DANCEPAD_DDR_SOLO\x10\x12\x12#\n\x1f\x42UTTON_LAYOUT_DANCEPAD_PIU_LEFT\x10\x13\x12\x18\n\x14\x42UTTON_LAYOUT_POPN_A\x10\x14\x12\x19\n\x15\x42UTTON_LAYOUT_TAIKO_A\x10\x15\x12 \n\x1c\x42UTTON_LAYOUT_BM_TURNTABLE_A\x10\x16\x12\x1b\n\x17\x42UTTON_LAYOUT_BM_5KEY_A\x10\x17\x12\x1b\n\x17\x42UTTON_LAYOUT_BM_7KEY_A\x10\x18\x12!\n\x1d\x42UTTON_LAYOUT_GITADORA_FRET_A\x10\x19\x12\"\n\x1e\x42UTTON_LAYOUT_GITADORA_STRUM_A\x10\x1a\x12!\n\x1d\x42UTTON_LAYOUT_BOARD_DEFINED_A\x10\x1b\x12!\n\x1d\x42UTTON_LAYOUT_BANDHERO_FRET_A\x10\x1c\x12\"\n\x1e\x42UTTON_LAYOUT_BANDHERO_STRUM_A\x10\x1d\x12\x19\n\x15\x42UTTON_LAYOUT_6GAWD_A\x10\x1e\x12#\n\x1f\x42UTTON_LAYOUT_6GAWD_ALLBUTTON_A\x10\x1f\x12\'\n#BUTTON_LAYOUT_6GAWD_ALLBUTTONPLUS_A\x10 \x1a\x05\x92?\x02 \x00*\x9c\t\n\x11\x42uttonLayoutRight\x12\x18\n\x14\x42UTTON_LAYOUT_ARCADE\x10\x00\x12\x1c\n\x18\x42UTTON_LAYOUT_STICKLESSB\x10\x01\x12!\n\x1d\x42UTTON_LAYOUT_BUTTONS_ANGLEDB\x10\x02\x12\x18\n\x14\x42UTTON_LAYOUT_VEWLIX\x10\x03\x12\x19\n\x15\x42UTTON_LAYOUT_VEWLIX7\x10\x04\x12\x18\n\x14\x42UTTON_LAYOUT_CAPCOM\x10\x05\x12\x19\n\x15\x42UTTON_LAYOUT_CAPCOM6\x10\x06\x12\x18\n\x14\x42UTTON_LAYOUT_SEGA2P\x10\x07\x12\x17\n\x13\x42UTTON_LAYOUT_NOIR8\x10\x08\x12\x1b\n\x17\x42UTTON_LAYOUT_KEYBOARDB\x10\t\x12\x1b\n\x17\x42UTTON_LAYOUT_DANCEPADB\x10\n\x12\x1c\n\x18\x42UTTON_LAYOUT_TWINSTICKB\x10\x0b\x12\x18\n\x14\x42UTTON_LAYOUT_BLANKB\x10\x0c\x12\x16\n\x12\x42UTTON_LAYOUT_VLXB\x10\r\x12\x1c\n\x18\x42UTTON_LAYOUT_FIGHTBOARD\x10\x0e\x12+\n\'BUTTON_LAYOUT_FIGHTBOARD_STICK_MIRRORED\x10\x0f\x12\x19\n\x15\x42UTTON_LAYOUT_CUSTOMB\x10\x10\x12\x1c\n\x18\x42UTTON_LAYOUT_KEYBOARD8B\x10\x11\x12 \n\x1c\x42UTTON_LAYOUT_OPENCORE0WASDB\x10\x12\x12\x1f\n\x1b\x42UTTON_LAYOUT_STICKLESS_13B\x10\x13\x12\x1f\n\x1b\x42UTTON_LAYOUT_STICKLESS_16B\x10\x14\x12\x1f\n\x1b\x42UTTON_LAYOUT_STICKLESS_14B\x10\x15\x12$\n BUTTON_LAYOUT_DANCEPAD_DDR_RIGHT\x10\x16\x12$\n BUTTON_LAYOUT_DANCEPAD_PIU_RIGHT\x10\x17\x12\x18\n\x14\x42UTTON_LAYOUT_POPN_B\x10\x18\x12\x19\n\x15\x42UTTON_LAYOUT_TAIKO_B\x10\x19\x12 \n\x1c\x42UTTON_LAYOUT_BM_TURNTABLE_B\x10\x1a\x12\x1b\n\x17\x42UTTON_LAYOUT_BM_5KEY_B\x10\x1b\x12\x1b\n\x17\x42UTTON_LAYOUT_BM_7KEY_B\x10\x1c\x12!\n\x1d\x42UTTON_LAYOUT_GITADORA_FRET_B\x10\x1d\x12\"\n\x1e\x42UTTON_LAYOUT_GITADORA_STRUM_B\x10\x1e\x12!\n\x1d\x42UTTON_LAYOUT_BOARD_DEFINED_B\x10\x1f\x12!\n\x1d\x42UTTON_LAYOUT_BANDHERO_FRET_B\x10 \x12\"\n\x1e\x42UTTON_LAYOUT_BANDHERO_STRUM_B\x10!\x12\x19\n\x15\x42UTTON_LAYOUT_6GAWD_B\x10\"\x12#\n\x1f\x42UTTON_LAYOUT_6GAWD_ALLBUTTON_B\x10#\x12\'\n#BUTTON_LAYOUT_6GAWD_ALLBUTTONPLUS_B\x10$\x1a\x05\x92?\x02 \x00*y\n\nSplashMode\x12\x16\n\x12SPLASH_MODE_STATIC\x10\x00\x12\x17\n\x13SPLASH_MODE_CLOSEIN\x10\x01\x12\x1d\n\x19SPLASH_MODE_CLOSEINCUSTOM\x10\x02\x12\x14\n\x10SPLASH_MODE_NONE\x10\x03\x1a\x05\x92?\x02 \x00*\xa0\x01\n\x0cSplashChoice\x12\x16\n\x12SPLASH_CHOICE_MAIN\x10\x00\x12\x13\n\x0fSPLASH_CHOICE_X\x10\x01\x12\x13\n\x0fSPLASH_CHOICE_Y\x10\x02\x12\x13\n\x0fSPLASH_CHOICE_Z\x10\x03\x12\x18\n\x14SPLASH_CHOICE_CUSTOM\x10\x04\x12\x18\n\x14SPLASH_CHOICE_LEGACY\x10\x05\x1a\x05\x92?\x02 \x00*\x99\x01\n\x0eOnBoardLedMode\x12\x19\n\x15ON_BOARD_LED_MODE_OFF\x10\x00\x12$\n ON_BOARD_LED_MODE_MODE_INDICATOR\x10\x01\x12 \n\x1cON_BOARD_LED_MODE_INPUT_TEST\x10\x02\x12\x1d\n\x19ON_BOARD_LED_MODE_PS_AUTH\x10\x03\x1a\x05\x92?\x02 \x00*\xec\x02\n\tInputMode\x12\x15\n\x11INPUT_MODE_XINPUT\x10\x00\x12\x15\n\x11INPUT_MODE_SWITCH\x10\x01\x12\x12\n\x0eINPUT_MODE_HID\x10\x02\x12\x17\n\x13INPUT_MODE_KEYBOARD\x10\x03\x12\x12\n\x0eINPUT_MODE_PS4\x10\x04\x12\x14\n\x10INPUT_MODE_XBONE\x10\x05\x12\x15\n\x11INPUT_MODE_MDMINI\x10\x06\x12\x15\n\x11INPUT_MODE_NEOGEO\x10\x07\x12\x16\n\x12INPUT_MODE_PCEMINI\x10\x08\x12\x14\n\x10INPUT_MODE_EGRET\x10\t\x12\x14\n\x10INPUT_MODE_ASTRO\x10\n\x12\x18\n\x14INPUT_MODE_PSCLASSIC\x10\x0b\x12\x1b\n\x17INPUT_MODE_XBOXORIGINAL\x10\x0c\x12\x12\n\x0eINPUT_MODE_PS5\x10\r\x12\x16\n\x11INPUT_MODE_CONFIG\x10\xff\x01\x1a\x05\x92?\x02 \x00*\x94\x01\n\x11InputModeAuthType\x12\x1d\n\x19INPUT_MODE_AUTH_TYPE_NONE\x10\x00\x12\x1d\n\x19INPUT_MODE_AUTH_TYPE_KEYS\x10\x01\x12\x1c\n\x18INPUT_MODE_AUTH_TYPE_USB\x10\x02\x12\x1c\n\x18INPUT_MODE_AUTH_TYPE_I2C\x10\x03\x1a\x05\x92?\x02 \x00*_\n\x08\x44padMode\x12\x15\n\x11\x44PAD_MODE_DIGITAL\x10\x00\x12\x19\n\x15\x44PAD_MODE_LEFT_ANALOG\x10\x01\x12\x1a\n\x16\x44PAD_MODE_RIGHT_ANALOG\x10\x02\x1a\x05\x92?\x02 \x00*O\n\nInvertMode\x12\x0f\n\x0bINVERT_NONE\x10\x00\x12\x0c\n\x08INVERT_X\x10\x01\x12\x0c\n\x08INVERT_Y\x10\x02\x12\r\n\tINVERT_XY\x10\x03\x1a\x05\x92?\x02 \x00*\xa2\x01\n\x08SOCDMode\x12\x19\n\x15SOCD_MODE_UP_PRIORITY\x10\x00\x12\x15\n\x11SOCD_MODE_NEUTRAL\x10\x01\x12#\n\x1fSOCD_MODE_SECOND_INPUT_PRIORITY\x10\x02\x12\"\n\x1eSOCD_MODE_FIRST_INPUT_PRIORITY\x10\x03\x12\x14\n\x10SOCD_MODE_BYPASS\x10\x04\x1a\x05\x92?\x02 \x00*\x88\x08\n\nGpioAction\x12\x11\n\x04NONE\x10\xf6\xff\xff\xff\xff\xff\xff\xff\xff\x01\x12\x15\n\x08RESERVED\x10\xfb\xff\xff\xff\xff\xff\xff\xff\xff\x01\x12\x15\n\x11\x41SSIGNED_TO_ADDON\x10\x00\x12\x13\n\x0f\x42UTTON_PRESS_UP\x10\x01\x12\x15\n\x11\x42UTTON_PRESS_DOWN\x10\x02\x12\x15\n\x11\x42UTTON_PRESS_LEFT\x10\x03\x12\x16\n\x12\x42UTTON_PRESS_RIGHT\x10\x04\x12\x13\n\x0f\x42UTTON_PRESS_B1\x10\x05\x12\x13\n\x0f\x42UTTON_PRESS_B2\x10\x06\x12\x13\n\x0f\x42UTTON_PRESS_B3\x10\x07\x12\x13\n\x0f\x42UTTON_PRESS_B4\x10\x08\x12\x13\n\x0f\x42UTTON_PRESS_L1\x10\t\x12\x13\n\x0f\x42UTTON_PRESS_R1\x10\n\x12\x13\n\x0f\x42UTTON_PRESS_L2\x10\x0b\x12\x13\n\x0f\x42UTTON_PRESS_R2\x10\x0c\x12\x13\n\x0f\x42UTTON_PRESS_S1\x10\r\x12\x13\n\x0f\x42UTTON_PRESS_S2\x10\x0e\x12\x13\n\x0f\x42UTTON_PRESS_A1\x10\x0f\x12\x13\n\x0f\x42UTTON_PRESS_A2\x10\x10\x12\x13\n\x0f\x42UTTON_PRESS_L3\x10\x11\x12\x13\n\x0f\x42UTTON_PRESS_R3\x10\x12\x12\x13\n\x0f\x42UTTON_PRESS_FN\x10\x13\x12\x17\n\x13\x42UTTON_PRESS_DDI_UP\x10\x14\x12\x19\n\x15\x42UTTON_PRESS_DDI_DOWN\x10\x15\x12\x19\n\x15\x42UTTON_PRESS_DDI_LEFT\x10\x16\x12\x1a\n\x16\x42UTTON_PRESS_DDI_RIGHT\x10\x17\x12\x16\n\x12SUSTAIN_DP_MODE_DP\x10\x18\x12\x16\n\x12SUSTAIN_DP_MODE_LS\x10\x19\x12\x16\n\x12SUSTAIN_DP_MODE_RS\x10\x1a\x12\x1d\n\x19SUSTAIN_SOCD_MODE_UP_PRIO\x10\x1b\x12\x1d\n\x19SUSTAIN_SOCD_MODE_NEUTRAL\x10\x1c\x12 \n\x1cSUSTAIN_SOCD_MODE_SECOND_WIN\x10\x1d\x12\x1f\n\x1bSUSTAIN_SOCD_MODE_FIRST_WIN\x10\x1e\x12\x1c\n\x18SUSTAIN_SOCD_MODE_BYPASS\x10\x1f\x12\x16\n\x12\x42UTTON_PRESS_TURBO\x10 \x12\x16\n\x12\x42UTTON_PRESS_MACRO\x10!\x12\x18\n\x14\x42UTTON_PRESS_MACRO_1\x10\"\x12\x18\n\x14\x42UTTON_PRESS_MACRO_2\x10#\x12\x18\n\x14\x42UTTON_PRESS_MACRO_3\x10$\x12\x18\n\x14\x42UTTON_PRESS_MACRO_4\x10%\x12\x18\n\x14\x42UTTON_PRESS_MACRO_5\x10&\x12\x18\n\x14\x42UTTON_PRESS_MACRO_6\x10\'\x1a\x05\x92?\x02 \x00*\x80\x07\n\rGamepadHotkey\x12\x0f\n\x0bHOTKEY_NONE\x10\x00\x12\x17\n\x13HOTKEY_DPAD_DIGITAL\x10\x01\x12\x1b\n\x17HOTKEY_DPAD_LEFT_ANALOG\x10\x02\x12\x1c\n\x18HOTKEY_DPAD_RIGHT_ANALOG\x10\x03\x12\x16\n\x12HOTKEY_HOME_BUTTON\x10\x04\x12\x19\n\x15HOTKEY_CAPTURE_BUTTON\x10\x05\x12\x1b\n\x17HOTKEY_SOCD_UP_PRIORITY\x10\x06\x12\x17\n\x13HOTKEY_SOCD_NEUTRAL\x10\x07\x12\x1a\n\x16HOTKEY_SOCD_LAST_INPUT\x10\x08\x12\x18\n\x14HOTKEY_INVERT_X_AXIS\x10\t\x12\x18\n\x14HOTKEY_INVERT_Y_AXIS\x10\n\x12\x1b\n\x17HOTKEY_SOCD_FIRST_INPUT\x10\x0b\x12\x16\n\x12HOTKEY_SOCD_BYPASS\x10\x0c\x12\x1c\n\x18HOTKEY_TOGGLE_4_WAY_MODE\x10\r\x12 \n\x1cHOTKEY_TOGGLE_DDI_4_WAY_MODE\x10\x0e\x12\x19\n\x15HOTKEY_LOAD_PROFILE_1\x10\x0f\x12\x19\n\x15HOTKEY_LOAD_PROFILE_2\x10\x10\x12\x19\n\x15HOTKEY_LOAD_PROFILE_3\x10\x11\x12\x19\n\x15HOTKEY_LOAD_PROFILE_4\x10\x12\x12\x14\n\x10HOTKEY_L3_BUTTON\x10\x13\x12\x14\n\x10HOTKEY_R3_BUTTON\x10\x14\x12\x1a\n\x16HOTKEY_TOUCHPAD_BUTTON\x10\x15\x12\x19\n\x15HOTKEY_REBOOT_DEFAULT\x10\x16\x12\x14\n\x10HOTKEY_B1_BUTTON\x10\x17\x12\x14\n\x10HOTKEY_B2_BUTTON\x10\x18\x12\x14\n\x10HOTKEY_B3_BUTTON\x10\x19\x12\x14\n\x10HOTKEY_B4_BUTTON\x10\x1a\x12\x14\n\x10HOTKEY_L1_BUTTON\x10\x1b\x12\x14\n\x10HOTKEY_R1_BUTTON\x10\x1c\x12\x14\n\x10HOTKEY_L2_BUTTON\x10\x1d\x12\x14\n\x10HOTKEY_R2_BUTTON\x10\x1e\x12\x14\n\x10HOTKEY_S1_BUTTON\x10\x1f\x12\x14\n\x10HOTKEY_S2_BUTTON\x10 \x12\x14\n\x10HOTKEY_A1_BUTTON\x10!\x12\x14\n\x10HOTKEY_A2_BUTTON\x10\"\x1a\x05\x92?\x02 \x00*c\n\x0fLEDFormat_Proto\x12\x12\n\x0eLED_FORMAT_GRB\x10\x00\x12\x12\n\x0eLED_FORMAT_RGB\x10\x01\x12\x13\n\x0fLED_FORMAT_GRBW\x10\x02\x12\x13\n\x0fLED_FORMAT_RGBW\x10\x03*\\\n\x0cShmupMixMode\x12!\n\x1dSHMUP_MIX_MODE_TURBO_PRIORITY\x10\x00\x12\"\n\x1eSHMUP_MIX_MODE_CHARGE_PRIORITY\x10\x01\x1a\x05\x92?\x02 \x00*T\n\x08PLEDType\x12\x1b\n\x0ePLED_TYPE_NONE\x10\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\x12\x11\n\rPLED_TYPE_PWM\x10\x00\x12\x11\n\rPLED_TYPE_RGB\x10\x01\x1a\x05\x92?\x02 \x00*\xa3\x01\n\x0f\x46orcedSetupMode\x12\x19\n\x15\x46ORCED_SETUP_MODE_OFF\x10\x00\x12&\n\"FORCED_SETUP_MODE_LOCK_MODE_SWITCH\x10\x01\x12%\n!FORCED_SETUP_MODE_LOCK_WEB_CONFIG\x10\x02\x12\x1f\n\x1b\x46ORCED_SETUP_MODE_LOCK_BOTH\x10\x03\x1a\x05\x92?\x02 \x00*g\n\x1e\x44ualDirectionalCombinationMode\x12\x0e\n\nMIXED_MODE\x10\x00\x12\x10\n\x0cGAMEPAD_MODE\x10\x01\x12\r\n\tDUAL_MODE\x10\x02\x12\r\n\tNONE_MODE\x10\x03\x1a\x05\x92?\x02 \x00*C\n\x11PS4ControllerType\x12\x12\n\x0ePS4_CONTROLLER\x10\x00\x12\x13\n\x0fPS4_ARCADESTICK\x10\x07\x1a\x05\x92?\x02 \x00*C\n\tMacroType\x12\x0c\n\x08ON_PRESS\x10\x01\x12\x12\n\x0eON_HOLD_REPEAT\x10\x02\x12\r\n\tON_TOGGLE\x10\x03\x1a\x05\x92?\x02 \x00*\xea\x01\n\tGPElement\x12\x15\n\x11GP_ELEMENT_WIDGET\x10\x00\x12\x15\n\x11GP_ELEMENT_SCREEN\x10\x01\x12\x19\n\x15GP_ELEMENT_BTN_BUTTON\x10\x02\x12\x19\n\x15GP_ELEMENT_DIR_BUTTON\x10\x03\x12\x19\n\x15GP_ELEMENT_PIN_BUTTON\x10\x04\x12\x14\n\x10GP_ELEMENT_LEVER\x10\x05\x12\x14\n\x10GP_ELEMENT_LABEL\x10\x06\x12\x15\n\x11GP_ELEMENT_SPRITE\x10\x07\x12\x14\n\x10GP_ELEMENT_SHAPE\x10\x08\x1a\x05\x92?\x02 \x00*{\n\x0cGPShape_Type\x12\x14\n\x10GP_SHAPE_ELLIPSE\x10\x00\x12\x13\n\x0fGP_SHAPE_SQUARE\x10\x01\x12\x11\n\rGP_SHAPE_LINE\x10\x02\x12\x14\n\x10GP_SHAPE_POLYGON\x10\x03\x12\x10\n\x0cGP_SHAPE_ARC\x10\x04\x1a\x05\x92?\x02 \x00*\xa7\x02\n\x14RotaryEncoderPinMode\x12\x15\n\x11\x45NCODER_MODE_NONE\x10\x00\x12\x1e\n\x1a\x45NCODER_MODE_LEFT_ANALOG_X\x10\x01\x12\x1e\n\x1a\x45NCODER_MODE_LEFT_ANALOG_Y\x10\x02\x12\x1f\n\x1b\x45NCODER_MODE_RIGHT_ANALOG_X\x10\x03\x12\x1f\n\x1b\x45NCODER_MODE_RIGHT_ANALOG_Y\x10\x04\x12\x1d\n\x19\x45NCODER_MODE_LEFT_TRIGGER\x10\x05\x12\x1e\n\x1a\x45NCODER_MODE_RIGHT_TRIGGER\x10\x06\x12\x17\n\x13\x45NCODER_MODE_DPAD_X\x10\x07\x12\x17\n\x13\x45NCODER_MODE_DPAD_Y\x10\x08\x1a\x05\x92?\x02 \x00')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'enums_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   _BUTTONLAYOUT._options = None
@@ -60,51 +60,51 @@
   _GPELEMENT._options = None
   _GPELEMENT._serialized_options = b'\222?\002 \000'
   _GPSHAPE_TYPE._options = None
   _GPSHAPE_TYPE._serialized_options = b'\222?\002 \000'
   _ROTARYENCODERPINMODE._options = None
   _ROTARYENCODERPINMODE._serialized_options = b'\222?\002 \000'
   _BUTTONLAYOUT._serialized_start=30
-  _BUTTONLAYOUT._serialized_end=939
-  _BUTTONLAYOUTRIGHT._serialized_start=942
-  _BUTTONLAYOUTRIGHT._serialized_end=1946
-  _SPLASHMODE._serialized_start=1948
-  _SPLASHMODE._serialized_end=2069
-  _SPLASHCHOICE._serialized_start=2072
-  _SPLASHCHOICE._serialized_end=2232
-  _ONBOARDLEDMODE._serialized_start=2235
-  _ONBOARDLEDMODE._serialized_end=2388
-  _INPUTMODE._serialized_start=2391
-  _INPUTMODE._serialized_end=2755
-  _INPUTMODEAUTHTYPE._serialized_start=2758
-  _INPUTMODEAUTHTYPE._serialized_end=2906
-  _DPADMODE._serialized_start=2908
-  _DPADMODE._serialized_end=3003
-  _INVERTMODE._serialized_start=3005
-  _INVERTMODE._serialized_end=3084
-  _SOCDMODE._serialized_start=3087
-  _SOCDMODE._serialized_end=3249
-  _GPIOACTION._serialized_start=3252
-  _GPIOACTION._serialized_end=4284
-  _GAMEPADHOTKEY._serialized_start=4287
-  _GAMEPADHOTKEY._serialized_end=5183
-  _LEDFORMAT_PROTO._serialized_start=5185
-  _LEDFORMAT_PROTO._serialized_end=5284
-  _SHMUPMIXMODE._serialized_start=5286
-  _SHMUPMIXMODE._serialized_end=5378
-  _PLEDTYPE._serialized_start=5380
-  _PLEDTYPE._serialized_end=5464
-  _FORCEDSETUPMODE._serialized_start=5467
-  _FORCEDSETUPMODE._serialized_end=5630
-  _DUALDIRECTIONALCOMBINATIONMODE._serialized_start=5632
-  _DUALDIRECTIONALCOMBINATIONMODE._serialized_end=5735
-  _PS4CONTROLLERTYPE._serialized_start=5737
-  _PS4CONTROLLERTYPE._serialized_end=5804
-  _MACROTYPE._serialized_start=5806
-  _MACROTYPE._serialized_end=5873
-  _GPELEMENT._serialized_start=5876
-  _GPELEMENT._serialized_end=6110
-  _GPSHAPE_TYPE._serialized_start=6112
-  _GPSHAPE_TYPE._serialized_end=6238
-  _ROTARYENCODERPINMODE._serialized_start=6241
-  _ROTARYENCODERPINMODE._serialized_end=6536
+  _BUTTONLAYOUT._serialized_end=1115
+  _BUTTONLAYOUTRIGHT._serialized_start=1118
+  _BUTTONLAYOUTRIGHT._serialized_end=2298
+  _SPLASHMODE._serialized_start=2300
+  _SPLASHMODE._serialized_end=2421
+  _SPLASHCHOICE._serialized_start=2424
+  _SPLASHCHOICE._serialized_end=2584
+  _ONBOARDLEDMODE._serialized_start=2587
+  _ONBOARDLEDMODE._serialized_end=2740
+  _INPUTMODE._serialized_start=2743
+  _INPUTMODE._serialized_end=3107
+  _INPUTMODEAUTHTYPE._serialized_start=3110
+  _INPUTMODEAUTHTYPE._serialized_end=3258
+  _DPADMODE._serialized_start=3260
+  _DPADMODE._serialized_end=3355
+  _INVERTMODE._serialized_start=3357
+  _INVERTMODE._serialized_end=3436
+  _SOCDMODE._serialized_start=3439
+  _SOCDMODE._serialized_end=3601
+  _GPIOACTION._serialized_start=3604
+  _GPIOACTION._serialized_end=4636
+  _GAMEPADHOTKEY._serialized_start=4639
+  _GAMEPADHOTKEY._serialized_end=5535
+  _LEDFORMAT_PROTO._serialized_start=5537
+  _LEDFORMAT_PROTO._serialized_end=5636
+  _SHMUPMIXMODE._serialized_start=5638
+  _SHMUPMIXMODE._serialized_end=5730
+  _PLEDTYPE._serialized_start=5732
+  _PLEDTYPE._serialized_end=5816
+  _FORCEDSETUPMODE._serialized_start=5819
+  _FORCEDSETUPMODE._serialized_end=5982
+  _DUALDIRECTIONALCOMBINATIONMODE._serialized_start=5984
+  _DUALDIRECTIONALCOMBINATIONMODE._serialized_end=6087
+  _PS4CONTROLLERTYPE._serialized_start=6089
+  _PS4CONTROLLERTYPE._serialized_end=6156
+  _MACROTYPE._serialized_start=6158
+  _MACROTYPE._serialized_end=6225
+  _GPELEMENT._serialized_start=6228
+  _GPELEMENT._serialized_end=6462
+  _GPSHAPE_TYPE._serialized_start=6464
+  _GPSHAPE_TYPE._serialized_end=6587
+  _ROTARYENCODERPINMODE._serialized_start=6590
+  _ROTARYENCODERPINMODE._serialized_end=6885
 # @@protoc_insertion_point(module_scope)
```

### Comparing `gp2040ce_binary_tools-0.8.3/tests/test-files/pb2-files/nanopb_pb2.py` & `gp2040ce_binary_tools-0.9.0/tests/test-files/pb2-files/nanopb_pb2.py`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.3/tests/test-files/proto-files/config.proto` & `gp2040ce_binary_tools-0.9.0/tests/test-files/proto-files/config.proto`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.3/tests/test-files/proto-files/enums.proto` & `gp2040ce_binary_tools-0.9.0/tests/test-files/proto-files/enums.proto`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,19 @@
     BUTTON_LAYOUT_TAIKO_A = 21;
     BUTTON_LAYOUT_BM_TURNTABLE_A = 22;
     BUTTON_LAYOUT_BM_5KEY_A = 23;
     BUTTON_LAYOUT_BM_7KEY_A = 24;
     BUTTON_LAYOUT_GITADORA_FRET_A = 25;
     BUTTON_LAYOUT_GITADORA_STRUM_A = 26;
     BUTTON_LAYOUT_BOARD_DEFINED_A = 27;
+    BUTTON_LAYOUT_BANDHERO_FRET_A = 28;
+    BUTTON_LAYOUT_BANDHERO_STRUM_A = 29;
+    BUTTON_LAYOUT_6GAWD_A = 30;
+    BUTTON_LAYOUT_6GAWD_ALLBUTTON_A = 31;
+    BUTTON_LAYOUT_6GAWD_ALLBUTTONPLUS_A = 32;
 }
 
 enum ButtonLayoutRight
 {
     option (nanopb_enumopt).long_names = false;
 
     BUTTON_LAYOUT_ARCADE = 0;
@@ -68,14 +73,19 @@
     BUTTON_LAYOUT_TAIKO_B = 25;
     BUTTON_LAYOUT_BM_TURNTABLE_B = 26;
     BUTTON_LAYOUT_BM_5KEY_B = 27;
     BUTTON_LAYOUT_BM_7KEY_B = 28;
     BUTTON_LAYOUT_GITADORA_FRET_B = 29;
     BUTTON_LAYOUT_GITADORA_STRUM_B = 30;
     BUTTON_LAYOUT_BOARD_DEFINED_B = 31;
+    BUTTON_LAYOUT_BANDHERO_FRET_B = 32;
+    BUTTON_LAYOUT_BANDHERO_STRUM_B = 33;
+    BUTTON_LAYOUT_6GAWD_B = 34;
+    BUTTON_LAYOUT_6GAWD_ALLBUTTON_B = 35;
+    BUTTON_LAYOUT_6GAWD_ALLBUTTONPLUS_B = 36;
 }
 
 enum SplashMode
 {
     option (nanopb_enumopt).long_names = false;
 
     SPLASH_MODE_STATIC = 0;
@@ -338,15 +348,15 @@
 
 enum GPShape_Type
 {
     option (nanopb_enumopt).long_names = false;
     
     GP_SHAPE_ELLIPSE = 0;
     GP_SHAPE_SQUARE = 1;
-    GP_SHAPE_DIAMOND = 2;
+    GP_SHAPE_LINE = 2;
     GP_SHAPE_POLYGON = 3;
     GP_SHAPE_ARC = 4;
 };
 
 enum RotaryEncoderPinMode
 {
     option (nanopb_enumopt).long_names = false;
```

### Comparing `gp2040ce_binary_tools-0.8.3/tests/test-files/proto-files/nanopb.proto` & `gp2040ce_binary_tools-0.9.0/tests/test-files/proto-files/nanopb.proto`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.3/tests/test-files/test-binary-source-of-json-config.bin` & `gp2040ce_binary_tools-0.9.0/tests/test-files/test-binary-source-of-json-config.bin`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.3/tests/test-files/test-config.bin` & `gp2040ce_binary_tools-0.9.0/tests/test-files/test-config.bin`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.3/tests/test-files/test-config.json` & `gp2040ce_binary_tools-0.9.0/tests/test-files/test-config.json`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.3/tests/test-files/test-firmware.bin` & `gp2040ce_binary_tools-0.9.0/tests/test-files/test-firmware.bin`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.3/tests/test-files/test-storage-area.bin` & `gp2040ce_binary_tools-0.9.0/tests/test-files/test-storage-area.bin`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.3/tests/test-files/test-whole-board-with-board-config.bin` & `gp2040ce_binary_tools-0.9.0/tests/test-files/test-whole-board-with-board-config.bin`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.3/tests/test-files/test-whole-board.bin` & `gp2040ce_binary_tools-0.9.0/tests/test-files/test-whole-board.bin`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.3/tests/test_builder.py` & `gp2040ce_binary_tools-0.9.0/tests/test_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 """Tests for the image builder module.
 
 SPDX-FileCopyrightText: © 2023 Brian S. Stephan <bss@incorporeal.org>
 SPDX-License-Identifier: GPL-3.0-or-later
 """
+import logging
 import math
 import os
 import sys
 import unittest.mock as mock
 
 import pytest
 from decorator import decorator
 
 import gp2040ce_bintools.builder as builder
 from gp2040ce_bintools import get_config_pb2
 from gp2040ce_bintools.storage import (STORAGE_SIZE, get_board_storage_section, get_config, get_config_footer,
-                                       get_user_storage_section, serialize_config_with_footer)
+                                       get_config_from_json, get_user_storage_section, serialize_config_with_footer)
 
 HERE = os.path.dirname(os.path.abspath(__file__))
 
+logger = logging.getLogger(__name__)
+
 
 @decorator
 def with_pb2s(test, *args, **kwargs):
     """Wrap a test with precompiled pb2 files on the path."""
     proto_path = os.path.join(HERE, 'test-files', 'pb2-files')
     sys.path.append(proto_path)
 
@@ -348,14 +351,29 @@
         config_dump = file.read()
     # the current implementation of UF2 writing does it in 256 blocks, so each 256 byte block of
     # binary is 512 bytes in the UF2
     assert len(config_dump) == STORAGE_SIZE * 2
 
 
 @with_pb2s
+def test_write_new_config_to_config_json(config_binary, tmp_path):
+    """Test that the config can be written to a file."""
+    tmp_file = os.path.join(tmp_path, 'config.json')
+    config = get_config(config_binary)
+    builder.write_new_config_to_filename(config, tmp_file)
+
+    # read new file
+    with open(tmp_file, 'r') as file:
+        config_dump = file.read()
+    logger.debug(config_dump)
+    config = get_config_from_json(config_dump)
+    assert config.boardVersion == 'v0.7.5'
+
+
+@with_pb2s
 def test_write_new_config_to_usb(config_binary):
     """Test that the config can be written to USB at the proper alignment."""
     config = get_config(config_binary)
     serialized = serialize_config_with_footer(config)
     end_out, end_in = mock.MagicMock(), mock.MagicMock()
     with mock.patch('gp2040ce_bintools.builder.write') as mock_write:
         builder.write_new_config_to_usb(config, end_out, end_in)
```

### Comparing `gp2040ce_binary_tools-0.8.3/tests/test_commands.py` & `gp2040ce_binary_tools-0.9.0/tests/test_commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,16 @@
     sys.path.pop()
     del sys.modules['config_pb2']
 
 
 def test_version_flag():
     """Test that tools report the version."""
     result = run(['visualize-config', '-v'], capture_output=True, encoding='utf8')
-    assert __version__ in result.stdout
+    assert f'gp2040ce-binary-tools {__version__}' in result.stdout
+    assert 'Python 3' in result.stdout
 
 
 def test_help_flag():
     """Test that tools report the usage information."""
     result = run(['visualize-config', '-h'], capture_output=True, encoding='utf8')
     assert 'usage: visualize-config' in result.stdout
     assert 'Read the configuration section from a dump of a GP2040-CE board' in result.stdout
```

### Comparing `gp2040ce_binary_tools-0.8.3/tests/test_gui.py` & `gp2040ce_binary_tools-0.9.0/tests/test_gui.py`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.3/tests/test_package.py` & `gp2040ce_binary_tools-0.9.0/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.3/tests/test_rp2040.py` & `gp2040ce_binary_tools-0.9.0/tests/test_rp2040.py`

 * *Files identical despite different names*

### Comparing `gp2040ce_binary_tools-0.8.3/tests/test_storage.py` & `gp2040ce_binary_tools-0.9.0/tests/test_storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,14 +96,23 @@
     filename = os.path.join(HERE, 'test-files', 'test-whole-board-with-board-config.bin')
     config = storage.get_config_from_file(filename, whole_board=True, board_config=True)
     assert config.boardVersion == 'v0.7.6-15-g71f4512'
     assert config.addonOptions.bootselButtonOptions.enabled is False
 
 
 @with_pb2s
+def test_get_board_config_from_json_file():
+    """Test that we can open a JSON file and parse the config."""
+    filename = os.path.join(HERE, 'test-files', 'test-config.json')
+    config = storage.get_config_from_file(filename, whole_board=True, board_config=True)
+    assert config.boardVersion == 'v0.7.6-15-g71f4512'
+    assert config.addonOptions.bootselButtonOptions.enabled is False
+
+
+@with_pb2s
 def test_get_config_from_file_file_not_fonud_ok():
     """If we allow opening a file that doesn't exist (e.g. for the editor), check we get an empty config."""
     filename = os.path.join(HERE, 'test-files', 'nope.bin')
     config = storage.get_config_from_file(filename, allow_no_file=True)
     assert config.boardVersion == ''
```

### Comparing `gp2040ce_binary_tools-0.8.3/tox.ini` & `gp2040ce_binary_tools-0.9.0/tox.ini`

 * *Files identical despite different names*

