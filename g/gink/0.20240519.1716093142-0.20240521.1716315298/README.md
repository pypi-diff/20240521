# Comparing `tmp/gink-0.20240519.1716093142.tar.gz` & `tmp/gink-0.20240521.1716315298.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gink-0.20240519.1716093142.tar", last modified: Sun May 19 04:32:25 2024, max compression
+gzip compressed data, was "gink-0.20240521.1716315298.tar", last modified: Tue May 21 18:15:01 2024, max compression
```

## Comparing `gink-0.20240519.1716093142.tar` & `gink-0.20240521.1716315298.tar`

### file list

```diff
@@ -1,101 +1,102 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:32:25.551228 gink-0.20240519.1716093142/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-19 04:32:20.000000 gink-0.20240519.1716093142/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11194 2024-05-19 04:32:25.551228 gink-0.20240519.1716093142/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9857 2024-05-19 04:32:20.000000 gink-0.20240519.1716093142/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:32:25.535228 gink-0.20240519.1716093142/gink/
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-19 04:32:20.000000 gink-0.20240519.1716093142/gink/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5932 2024-05-19 04:32:20.000000 gink-0.20240519.1716093142/gink/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:32:25.539228 gink-0.20240519.1716093142/gink/builders/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 04:32:22.000000 gink-0.20240519.1716093142/gink/builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4350 2024-05-19 04:32:22.000000 gink-0.20240519.1716093142/gink/builders/behavior_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4694 2024-05-19 04:32:22.000000 gink-0.20240519.1716093142/gink/builders/bundle_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-05-19 04:32:22.000000 gink-0.20240519.1716093142/gink/builders/change_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-05-19 04:32:22.000000 gink-0.20240519.1716093142/gink/builders/claim_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-05-19 04:32:22.000000 gink-0.20240519.1716093142/gink/builders/clearance_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-19 04:32:22.000000 gink-0.20240519.1716093142/gink/builders/container_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     8918 2024-05-19 04:32:22.000000 gink-0.20240519.1716093142/gink/builders/entry_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3695 2024-05-19 04:32:22.000000 gink-0.20240519.1716093142/gink/builders/header_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-05-19 04:32:22.000000 gink-0.20240519.1716093142/gink/builders/key_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-05-19 04:32:22.000000 gink-0.20240519.1716093142/gink/builders/log_file_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-05-19 04:32:22.000000 gink-0.20240519.1716093142/gink/builders/movement_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-19 04:32:22.000000 gink-0.20240519.1716093142/gink/builders/muid_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-05-19 04:32:22.000000 gink-0.20240519.1716093142/gink/builders/pair_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    10363 2024-05-19 04:32:22.000000 gink-0.20240519.1716093142/gink/builders/sync_message_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    40439 2024-05-19 04:32:22.000000 gink-0.20240519.1716093142/gink/builders/value_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:32:25.547228 gink-0.20240519.1716093142/gink/impl/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 04:32:20.000000 gink-0.20240519.1716093142/gink/impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11130 2024-05-19 04:32:20.000000 gink-0.20240519.1716093142/gink/impl/abstract_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     4593 2024-05-19 04:32:20.000000 gink-0.20240519.1716093142/gink/impl/addressable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-19 04:32:20.000000 gink-0.20240519.1716093142/gink/impl/attribution.py
--rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-05-19 04:32:20.000000 gink-0.20240519.1716093142/gink/impl/box.py
--rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-05-19 04:32:20.000000 gink-0.20240519.1716093142/gink/impl/braid.py
--rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-05-19 04:32:20.000000 gink-0.20240519.1716093142/gink/impl/builders.py
--rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-05-19 04:32:20.000000 gink-0.20240519.1716093142/gink/impl/bundle_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-05-19 04:32:20.000000 gink-0.20240519.1716093142/gink/impl/bundle_store.py
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-19 04:32:20.000000 gink-0.20240519.1716093142/gink/impl/bundle_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-05-19 04:32:20.000000 gink-0.20240519.1716093142/gink/impl/bundler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-05-19 04:32:20.000000 gink-0.20240519.1716093142/gink/impl/chain_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)    19865 2024-05-19 04:32:20.000000 gink-0.20240519.1716093142/gink/impl/coding.py
--rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-05-19 04:32:20.000000 gink-0.20240519.1716093142/gink/impl/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    13325 2024-05-19 04:32:20.000000 gink-0.20240519.1716093142/gink/impl/container.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    17850 2024-05-19 04:32:20.000000 gink-0.20240519.1716093142/gink/impl/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-19 04:32:20.000000 gink-0.20240519.1716093142/gink/impl/deferred.py
--rw-r--r--   0 runner    (1001) docker     (127)    11594 2024-05-19 04:32:20.000000 gink-0.20240519.1716093142/gink/impl/directory.py
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-19 04:32:20.000000 gink-0.20240519.1716093142/gink/impl/dummy.py
--rw-r--r--   0 runner    (1001) docker     (127)    11834 2024-05-19 04:32:20.000000 gink-0.20240519.1716093142/gink/impl/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-05-19 04:32:20.000000 gink-0.20240519.1716093142/gink/impl/group.py
--rw-r--r--   0 runner    (1001) docker     (127)    11218 2024-05-19 04:32:20.000000 gink-0.20240519.1716093142/gink/impl/key_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-19 04:32:20.000000 gink-0.20240519.1716093142/gink/impl/listener.py
--rw-r--r--   0 runner    (1001) docker     (127)    57325 2024-05-19 04:32:20.000000 gink-0.20240519.1716093142/gink/impl/lmdb_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-05-19 04:32:20.000000 gink-0.20240519.1716093142/gink/impl/lmdb_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-05-19 04:32:20.000000 gink-0.20240519.1716093142/gink/impl/log_backed_store.py
--rw-r--r--   0 runner    (1001) docker     (127)    23274 2024-05-19 04:32:20.000000 gink-0.20240519.1716093142/gink/impl/memory_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-05-19 04:32:20.000000 gink-0.20240519.1716093142/gink/impl/muid.py
--rw-r--r--   0 runner    (1001) docker     (127)     6736 2024-05-19 04:32:20.000000 gink-0.20240519.1716093142/gink/impl/pair_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-05-19 04:32:20.000000 gink-0.20240519.1716093142/gink/impl/pair_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-05-19 04:32:20.000000 gink-0.20240519.1716093142/gink/impl/property.py
--rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-05-19 04:32:20.000000 gink-0.20240519.1716093142/gink/impl/selectable_console.py
--rw-r--r--   0 runner    (1001) docker     (127)    12612 2024-05-19 04:32:20.000000 gink-0.20240519.1716093142/gink/impl/sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-19 04:32:20.000000 gink-0.20240519.1716093142/gink/impl/tuples.py
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-19 04:32:20.000000 gink-0.20240519.1716093142/gink/impl/typedefs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-05-19 04:32:20.000000 gink-0.20240519.1716093142/gink/impl/utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-19 04:32:20.000000 gink-0.20240519.1716093142/gink/impl/watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     7547 2024-05-19 04:32:20.000000 gink-0.20240519.1716093142/gink/impl/websocket_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-19 04:32:20.000000 gink-0.20240519.1716093142/gink/impl/wsgi_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-05-19 04:32:20.000000 gink-0.20240519.1716093142/gink/impl/wsgi_listener.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:32:25.551228 gink-0.20240519.1716093142/gink/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 04:32:20.000000 gink-0.20240519.1716093142/gink/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-19 04:32:20.000000 gink-0.20240519.1716093142/gink/tests/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5022 2024-05-19 04:32:20.000000 gink-0.20240519.1716093142/gink/tests/test_box.py
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-19 04:32:20.000000 gink-0.20240519.1716093142/gink/tests/test_braid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-19 04:32:20.000000 gink-0.20240519.1716093142/gink/tests/test_chain_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-19 04:32:20.000000 gink-0.20240519.1716093142/gink/tests/test_change_set_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-05-19 04:32:20.000000 gink-0.20240519.1716093142/gink/tests/test_code_values.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-19 04:32:20.000000 gink-0.20240519.1716093142/gink/tests/test_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     5029 2024-05-19 04:32:20.000000 gink-0.20240519.1716093142/gink/tests/test_database.py
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-19 04:32:20.000000 gink-0.20240519.1716093142/gink/tests/test_demo.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10116 2024-05-19 04:32:20.000000 gink-0.20240519.1716093142/gink/tests/test_directory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4280 2024-05-19 04:32:20.000000 gink-0.20240519.1716093142/gink/tests/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     7601 2024-05-19 04:32:20.000000 gink-0.20240519.1716093142/gink/tests/test_key_set.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-19 04:32:20.000000 gink-0.20240519.1716093142/gink/tests/test_lmdb_store.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-19 04:32:20.000000 gink-0.20240519.1716093142/gink/tests/test_logbackedstore.py
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-19 04:32:20.000000 gink-0.20240519.1716093142/gink/tests/test_memory_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-19 04:32:20.000000 gink-0.20240519.1716093142/gink/tests/test_muid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-05-19 04:32:20.000000 gink-0.20240519.1716093142/gink/tests/test_names.py
--rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-05-19 04:32:20.000000 gink-0.20240519.1716093142/gink/tests/test_pair_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-05-19 04:32:20.000000 gink-0.20240519.1716093142/gink/tests/test_pair_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-19 04:32:20.000000 gink-0.20240519.1716093142/gink/tests/test_property.py
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-19 04:32:20.000000 gink-0.20240519.1716093142/gink/tests/test_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    10500 2024-05-19 04:32:20.000000 gink-0.20240519.1716093142/gink/tests/test_sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)    14345 2024-05-19 04:32:20.000000 gink-0.20240519.1716093142/gink/tests/test_store.py
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-19 04:32:20.000000 gink-0.20240519.1716093142/gink/tests/test_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-05-19 04:32:20.000000 gink-0.20240519.1716093142/gink/tests/test_websocket_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-05-19 04:32:20.000000 gink-0.20240519.1716093142/gink/tests/test_wsgi_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:32:25.551228 gink-0.20240519.1716093142/gink.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11194 2024-05-19 04:32:25.000000 gink-0.20240519.1716093142/gink.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-19 04:32:25.000000 gink-0.20240519.1716093142/gink.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 04:32:25.000000 gink-0.20240519.1716093142/gink.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-19 04:32:25.000000 gink-0.20240519.1716093142/gink.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-19 04:32:25.000000 gink-0.20240519.1716093142/gink.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 04:32:25.551228 gink-0.20240519.1716093142/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-19 04:32:22.000000 gink-0.20240519.1716093142/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:15:01.871978 gink-0.20240521.1716315298/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11194 2024-05-21 18:15:01.871978 gink-0.20240521.1716315298/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9857 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:15:01.855977 gink-0.20240521.1716315298/gink/
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6055 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:15:01.859978 gink-0.20240521.1716315298/gink/builders/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 18:14:58.000000 gink-0.20240521.1716315298/gink/builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4350 2024-05-21 18:14:58.000000 gink-0.20240521.1716315298/gink/builders/behavior_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4694 2024-05-21 18:14:58.000000 gink-0.20240521.1716315298/gink/builders/bundle_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-05-21 18:14:58.000000 gink-0.20240521.1716315298/gink/builders/change_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-05-21 18:14:58.000000 gink-0.20240521.1716315298/gink/builders/claim_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-05-21 18:14:58.000000 gink-0.20240521.1716315298/gink/builders/clearance_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-21 18:14:58.000000 gink-0.20240521.1716315298/gink/builders/container_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8918 2024-05-21 18:14:58.000000 gink-0.20240521.1716315298/gink/builders/entry_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3695 2024-05-21 18:14:58.000000 gink-0.20240521.1716315298/gink/builders/header_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-05-21 18:14:58.000000 gink-0.20240521.1716315298/gink/builders/key_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-05-21 18:14:58.000000 gink-0.20240521.1716315298/gink/builders/log_file_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-05-21 18:14:58.000000 gink-0.20240521.1716315298/gink/builders/movement_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-21 18:14:58.000000 gink-0.20240521.1716315298/gink/builders/muid_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-05-21 18:14:58.000000 gink-0.20240521.1716315298/gink/builders/pair_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10363 2024-05-21 18:14:58.000000 gink-0.20240521.1716315298/gink/builders/sync_message_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40439 2024-05-21 18:14:58.000000 gink-0.20240521.1716315298/gink/builders/value_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:15:01.867977 gink-0.20240521.1716315298/gink/impl/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11188 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/impl/abstract_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4593 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/impl/addressable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/impl/attribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/impl/box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/impl/braid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/impl/builders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/impl/bundle_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/impl/bundle_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/impl/bundle_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/impl/bundler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/impl/chain_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19865 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/impl/coding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3580 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/impl/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13325 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/impl/container.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14405 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/impl/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/impl/deferred.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11594 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/impl/directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/impl/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11834 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/impl/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/impl/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11218 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/impl/key_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/impl/listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57325 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/impl/lmdb_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/impl/lmdb_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/impl/log_backed_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/impl/looping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23274 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/impl/memory_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/impl/muid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6736 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/impl/pair_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/impl/pair_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/impl/property.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4658 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/impl/selectable_console.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12612 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/impl/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/impl/tuples.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/impl/typedefs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/impl/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/impl/watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7755 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/impl/websocket_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/impl/wsgi_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/impl/wsgi_listener.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:15:01.871978 gink-0.20240521.1716315298/gink/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/tests/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5022 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/tests/test_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/tests/test_braid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/tests/test_chain_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/tests/test_change_set_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/tests/test_code_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/tests/test_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5075 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/tests/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/tests/test_demo.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10116 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/tests/test_directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4280 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/tests/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7601 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/tests/test_key_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/tests/test_lmdb_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/tests/test_logbackedstore.py
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/tests/test_memory_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/tests/test_muid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/tests/test_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/tests/test_pair_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/tests/test_pair_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/tests/test_property.py
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/tests/test_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10500 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/tests/test_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14345 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/tests/test_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/tests/test_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/tests/test_websocket_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/tests/test_wsgi_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:15:01.871978 gink-0.20240521.1716315298/gink.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11194 2024-05-21 18:15:01.000000 gink-0.20240521.1716315298/gink.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-05-21 18:15:01.000000 gink-0.20240521.1716315298/gink.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 18:15:01.000000 gink-0.20240521.1716315298/gink.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-21 18:15:01.000000 gink-0.20240521.1716315298/gink.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-21 18:15:01.000000 gink-0.20240521.1716315298/gink.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 18:15:01.871978 gink-0.20240521.1716315298/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-21 18:14:58.000000 gink-0.20240521.1716315298/setup.py
```

### Comparing `gink-0.20240519.1716093142/LICENSE` & `gink-0.20240521.1716315298/LICENSE`

 * *Files identical despite different names*

### Comparing `gink-0.20240519.1716093142/PKG-INFO` & `gink-0.20240521.1716315298/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gink
-Version: 0.20240519.1716093142
+Version: 0.20240521.1716315298
 Summary: a system for storing data structures in lmdb
 Home-page: https://github.com/x5e/gink
 Author: Darin McGill
 Author-email: gink@darinmcgill.com
 Keywords: gink lmdb crdt history versioned
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `gink-0.20240519.1716093142/README.md` & `gink-0.20240521.1716315298/README.md`

 * *Files identical despite different names*

### Comparing `gink-0.20240519.1716093142/gink/__init__.py` & `gink-0.20240521.1716315298/gink/__init__.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240519.1716093142/gink/__main__.py` & `gink-0.20240521.1716315298/gink/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from argparse import ArgumentParser, Namespace
 from pathlib import Path
 
 from . import *
 from .impl.builders import BundleBuilder
 from .impl.selectable_console import SelectableConsole
 from .impl.utilities import get_identity
+from .impl.looping import loop
 
 parser: ArgumentParser = ArgumentParser(allow_abbrev=False)
 parser.add_argument("db_path", nargs="?", help="path to a database; created if doesn't exist")
 parser.add_argument("--verbosity", "-v", default="INFO", help="the log level to use, e.g. INFO or DEBUG")
 parser.add_argument("--format", default="lmdb", help="storage file format", choices=["lmdb", "binlog"])
 parser.add_argument("--set", help="set key/value in directory (default root) reading value from stdin")
 parser.add_argument("--get", help="get a value in the database (default root) and print to stdout")
@@ -77,55 +78,60 @@
 if args.show_bundles:
     builder = BundleBuilder()
     def show(data: bytes, _: BundleInfo):
         builder.ParseFromString(data)  # type: ignore
         print("=" * 79)
         print(builder)
     store.get_bundles(show)
-    store.close()
+    database.close()
     exit(0)
 
 if args.set:
     value = stdin.read().rstrip()
     container = root
     key = args.set
     container.set(key, value, comment=args.comment)
+    database.close()
     exit(0)
 
 if args.get:
     container = root
     result = container.get(args.get, as_of=args.as_of)
     print(result)
+    database.close()
     exit(0)
 
 if args.blame:
     if args.blame is True:
         root.show_blame(as_of=args.as_of)
     else:
         old_directory = root
         path_components = args.get.split("/")
         for component in path_components:
             old_directory = old_directory.get(component, as_of=args.as_of)
             assert isinstance(old_directory, Directory)
         old_directory.show_blame()
+    database.close()
     exit(0)
 
 if args.mkdir:
     path_components = args.mkdir.split("/")
     old_directory = root
     for component in path_components[:-1]:
         if not component: continue
         old_directory = old_directory.get(component, as_of=args.as_of)
         assert isinstance(old_directory, Directory)
     new_directory = Directory.create(database=database)
     old_directory.set(path_components[-1], new_directory, comment=args.comment)
+    database.close()
     exit(0)
 
 if args.log:
     database.show_log(args.log, include_starts=args.starts)
+    database.close()
     exit(0)
 
 if args.listen_on:
     ip_addr = "*"
     port = "8080"
     if args.listen_on is True:
         pass
@@ -147,11 +153,8 @@
 elif args.line_mode:
     interactive = False
 else:
     interactive = stdin.isatty()
 
 console = SelectableConsole(locals(), interactive=interactive, heartbeat_to=args.heartbeat_to)
 
-try:
-    database.run(console=console)
-except EOFError:
-    pass
+loop(console, database, context_manager=console)
```

### Comparing `gink-0.20240519.1716093142/gink/builders/behavior_pb2.py` & `gink-0.20240521.1716315298/gink/builders/behavior_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240519.1716093142/gink/builders/bundle_pb2.py` & `gink-0.20240521.1716315298/gink/builders/bundle_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240519.1716093142/gink/builders/change_pb2.py` & `gink-0.20240521.1716315298/gink/builders/change_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240519.1716093142/gink/builders/claim_pb2.py` & `gink-0.20240521.1716315298/gink/builders/claim_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240519.1716093142/gink/builders/clearance_pb2.py` & `gink-0.20240521.1716315298/gink/builders/clearance_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240519.1716093142/gink/builders/container_pb2.py` & `gink-0.20240521.1716315298/gink/builders/container_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240519.1716093142/gink/builders/entry_pb2.py` & `gink-0.20240521.1716315298/gink/builders/entry_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240519.1716093142/gink/builders/header_pb2.py` & `gink-0.20240521.1716315298/gink/builders/header_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240519.1716093142/gink/builders/key_pb2.py` & `gink-0.20240521.1716315298/gink/builders/key_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240519.1716093142/gink/builders/log_file_pb2.py` & `gink-0.20240521.1716315298/gink/builders/log_file_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240519.1716093142/gink/builders/movement_pb2.py` & `gink-0.20240521.1716315298/gink/builders/movement_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240519.1716093142/gink/builders/muid_pb2.py` & `gink-0.20240521.1716315298/gink/builders/muid_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240519.1716093142/gink/builders/pair_pb2.py` & `gink-0.20240521.1716315298/gink/builders/pair_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240519.1716093142/gink/builders/sync_message_pb2.py` & `gink-0.20240521.1716315298/gink/builders/sync_message_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240519.1716093142/gink/builders/value_pb2.py` & `gink-0.20240521.1716315298/gink/builders/value_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240519.1716093142/gink/impl/abstract_store.py` & `gink-0.20240521.1716315298/gink/impl/abstract_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,25 +25,25 @@
 
         Stores both the bundles received and the contents of those
         bundles unpacked so that you can examine entries, container definitions, etc.
 
         Warning! Since data stores are viewed as part of the internal implementation,
         this interface may change at any time without warning on a minor version change.
     """
+    on_ready: Callable  # needs to by dynamically assigned
 
     def __enter__(self):
         pass
 
     def __exit__(self, *_):
         self.close()
 
     @abstractmethod
     def _get_file_path(self) -> Optional[Path]:
         """ Return the underlying file name, or None if the store isn't file backed.
-
         """
 
     def is_selectable(self) -> bool:
         return self._get_watcher() is not None
 
     def _get_watcher(self) -> Optional[Watcher]:
         if not Watcher.supported():
```

### Comparing `gink-0.20240519.1716093142/gink/impl/addressable.py` & `gink-0.20240521.1716315298/gink/impl/addressable.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240519.1716093142/gink/impl/attribution.py` & `gink-0.20240521.1716315298/gink/impl/attribution.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240519.1716093142/gink/impl/box.py` & `gink-0.20240521.1716315298/gink/impl/box.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240519.1716093142/gink/impl/braid.py` & `gink-0.20240521.1716315298/gink/impl/braid.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240519.1716093142/gink/impl/builders.py` & `gink-0.20240521.1716315298/gink/impl/builders.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240519.1716093142/gink/impl/bundle_info.py` & `gink-0.20240521.1716315298/gink/impl/bundle_info.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240519.1716093142/gink/impl/bundle_store.py` & `gink-0.20240521.1716315298/gink/impl/bundle_store.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240519.1716093142/gink/impl/bundle_wrapper.py` & `gink-0.20240521.1716315298/gink/impl/bundle_wrapper.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240519.1716093142/gink/impl/bundler.py` & `gink-0.20240521.1716315298/gink/impl/bundler.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240519.1716093142/gink/impl/chain_tracker.py` & `gink-0.20240521.1716315298/gink/impl/chain_tracker.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240519.1716093142/gink/impl/coding.py` & `gink-0.20240521.1716315298/gink/impl/coding.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240519.1716093142/gink/impl/connection.py` & `gink-0.20240521.1716315298/gink/impl/connection.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """ Contains the Peer class that manages a connection to another gink instance. """
-from typing import Iterable, Optional, Union
+from typing import Iterable, Optional, Union, Callable
 from socket import (
     socket as Socket,
     AF_INET,
     SOCK_STREAM,
 )
 from logging import getLogger
 from abc import ABC, abstractmethod
@@ -16,31 +16,33 @@
 
 class Connection(ABC):
     """ Manages a connection to another gink database.
 
         Eventually there will be two subclasses: one to manage websocket connections,
         and another subclass to manage raw socket connections.
     """
-
+    on_ready: Callable
     def __init__(
             self,
             host: Optional[str] = None,
             port: Optional[int] = None,
-            socket: Optional[Socket] = None
+            socket: Optional[Socket] = None,
+            greeting: Optional[SyncMessage] = None,
     ):
         if socket is None:
             assert host is not None and port is not None
             socket = Socket(AF_INET, SOCK_STREAM)
             socket.connect((host, port))
         self._socket = socket
         self._host = host
         self._port = port
         self._logger = getLogger(self.__class__.__name__)
         self._closed = False
         self._tracker: Optional[ChainTracker] = None
+        self._greeting = greeting
 
     def fileno(self):
         """ Return the file descriptor of the underlying socket.
         """
         return self._socket.fileno()
 
     def is_closed(self) -> bool:
```

### Comparing `gink-0.20240519.1716093142/gink/impl/container.py` & `gink-0.20240521.1716315298/gink/impl/container.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240519.1716093142/gink/impl/database.py` & `gink-0.20240521.1716315298/gink/impl/database.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 #!/usr/bin/env python3
 """ contains the Database class """
 
 # standard python modules
-from typing import Optional, Set, Union, Iterable, Dict, List, Callable
-from datetime import datetime, date, timedelta
+from typing import Optional, Set, Union, Iterable, List, Callable
 from threading import Lock
-from select import select
 from sys import stdout
 from logging import getLogger
 from re import fullmatch, IGNORECASE
-from contextlib import nullcontext
+from socket import socketpair
 
 # builders
-from .builders import SyncMessage, ContainerBuilder
+from .builders import ContainerBuilder
 
 # gink modules
 from .abstract_store import AbstractStore
 from .bundler import Bundler
 from .bundle_info import BundleInfo
 from .typedefs import Medallion, MuTimestamp, GenericTimestamp, EPOCH
 from .tuples import Chain
@@ -24,60 +22,60 @@
 from .websocket_connection import WebsocketConnection
 from .listener import Listener
 from .muid import Muid
 from .chain_tracker import ChainTracker
 from .attribution import Attribution
 from .lmdb_store import LmdbStore
 from .memory_store import MemoryStore
-from .selectable_console import SelectableConsole
 from .bundle_wrapper import BundleWrapper
-from .wsgi_listener import WsgiListener
-from .wsgi_connection import WsgiConnection
-from .utilities import generate_timestamp, experimental, get_identity, generate_medallion
-
+from .utilities import (
+    generate_timestamp,
+    experimental,
+    get_identity,
+    generate_medallion,
+    resolve_timestamp,
+)
+from .looping import Selectable, Finished
 
 class Database:
     """ A class that mediates user interaction with a datastore and peers. """
     _chain: Optional[Chain]
     _lock: Lock
     _last_time: Optional[MuTimestamp]
     _store: AbstractStore
     _connections: Set[Connection]
-    _wsgi_connections: Set[WsgiConnection]
     _listeners: Set[Listener]
     _sent_but_not_acked: Set[BundleInfo]
     _last_link: Optional[BundleInfo]
     _container_types: dict = {}
 
-    def __init__(self,
-                 store: Union[AbstractStore, str, None] = None,
-                 identity = get_identity(),
-                 web_server = None,
-                 web_server_addr: tuple = ('localhost', 8081)):
+    def __init__(self, store: Union[AbstractStore, str, None] = None, identity = get_identity()):
         setattr(Database, "_last", self)
         if isinstance(store, str):
             store = LmdbStore(store)
         if isinstance(store, type(None)):
             store = MemoryStore()
         assert isinstance(store, AbstractStore)
         self._store = store
         self._last_link = None
         self._lock = Lock()
         self._last_time = None
         self._connections = set()
-        self._wsgi_connections = set()
         self._listeners = set()
         self._identity = identity
         self._logger = getLogger(self.__class__.__name__)
-        self._wsgi_listener: Optional[WsgiListener] = None
-        # Web server would be a Flask app or other WSGI compatible app
-        if web_server:
-            self._wsgi_listener = WsgiListener(app=web_server, address=web_server_addr)
         self._sent_but_not_acked = set()
         self._callbacks: List[Callable[[BundleInfo], None]] = list()
+        (self._socket_left, self._socket_rite) = socketpair()
+        self._indication_sent = False
+        if self._store.is_selectable():
+            self._indicate_selectables_changed()
+
+    def fileno(self) -> int:
+        return self._socket_rite.fileno()
 
     @experimental
     def add_callback(self, callback: Callable[[BundleInfo], None]):
         self._callbacks.append(callback)
 
     @staticmethod
     def get_last():
@@ -91,20 +89,22 @@
         behavior = getattr(container_cls, "BEHAVIOR")
         cls._container_types[behavior] = container_cls
 
     def get_store(self) -> AbstractStore:
         """ returns the store managed by this database """
         return self._store
 
+    @experimental
     def get_chain(self) -> Optional[Chain]:
         """ gets the chain this database is appending to (or None if it hasn't started writing yet) """
         if self._last_link is not None:
             return self._last_link.get_chain()
         return None
 
+    @experimental
     def get_now(self):
         return generate_timestamp()
 
     def resolve_timestamp(self, timestamp: GenericTimestamp = None) -> MuTimestamp:
         """ translates an abstract time into a real timestamp
 
             date and datetime behave as you might expect (turned into unix time)
@@ -112,46 +112,21 @@
             integers and floats that look like timestamps or microsecond timestamps are
             treated as such.
 
             small integers are treated as "right before the <index> bundle"
         """
         if timestamp is None:
             return generate_timestamp()
-        if isinstance(timestamp, str):
-            if fullmatch(r"-?\d+", timestamp):
-                timestamp = int(timestamp)
-            else:
-                timestamp = datetime.fromisoformat(timestamp)
-        if isinstance(timestamp, Muid):
-            muid_timestamp = timestamp.timestamp
-            if not isinstance(muid_timestamp, MuTimestamp):
-                raise ValueError("muid doesn't have a resolved timestamp")
-            return muid_timestamp
-        if isinstance(timestamp, timedelta):
-            return generate_timestamp() + int(timestamp.total_seconds() * 1e6)
-        if isinstance(timestamp, date):
-            timestamp = datetime(timestamp.year, timestamp.month, timestamp.day)
-        if isinstance(timestamp, datetime):
-            timestamp = timestamp.timestamp()
-        if isinstance(timestamp, (int, float)):
-            if 1671697316392367 < timestamp < 2147483648000000:
-                # appears to be a microsecond timestamp
-                return int(timestamp)
-            if 1671697630 < timestamp < 2147483648:
-                # appears to be seconds since epoch
-                return int(timestamp * 1e6)
         if isinstance(timestamp, int) and -1e6 < timestamp < 1e6:
             bundle_info = self._store.get_one(BundleInfo, int(timestamp))
             if bundle_info is None:
                 raise ValueError("don't have that many bundles")
             assert isinstance(bundle_info, BundleInfo)
             return bundle_info.timestamp
-        if isinstance(timestamp, float) and 1e6 > timestamp > -1e6:
-            return generate_timestamp() + int(1e6 * timestamp)
-        raise ValueError(f"don't know how to resolve {timestamp} into a timestamp")
+        return resolve_timestamp(timestamp)
 
     def _acquire_appendable_chain(self) -> BundleInfo:
         """ Either starts a chain or finds one to reuse, then returns the last link in it.
         """
         reused = self._store.maybe_reuse_chain(self._identity)
         if reused:
             return reused
@@ -188,114 +163,95 @@
         """ Sends a bundle either created locally or received from a peer to other peers.
         """
         for peer in self._connections:
             peer.send_bundle(bundle_wrapper)
         for callback in self._callbacks:
             callback(bundle_wrapper.get_info())
 
-    def _on_peer_ready(self, peer: Connection):
+    def _on_connection_ready(self, connection: Connection) -> None:
         with self._lock:
-            for thing in peer.receive_objects():
-                if isinstance(thing, BundleWrapper):  # some data
-                    self._store.apply_bundle(thing, self._on_bundle)
-                elif isinstance(thing, ChainTracker):  # greeting message
-                    self._store.get_bundles(peer.send_bundle, peer_has=thing)
-                elif isinstance(thing, BundleInfo):  # an ack:
-                    self._sent_but_not_acked.discard(thing)
-                else:
-                    raise AssertionError("unexpected object")
+            try:
+                for thing in connection.receive_objects():
+                    if isinstance(thing, BundleWrapper):  # some data
+                        self._store.apply_bundle(thing, self._on_bundle)
+                    elif isinstance(thing, ChainTracker):  # greeting message
+                        self._store.get_bundles(connection.send_bundle, peer_has=thing)
+                    elif isinstance(thing, BundleInfo):  # an ack:
+                        self._sent_but_not_acked.discard(thing)
+                    else:
+                        raise AssertionError("unexpected object")
+            except Finished:
+                self._connections.remove(connection)
+                raise
+
+    def _on_listener_ready(self, listener: Listener) -> Iterable[Selectable]:
+        sync_message = self._store.get_chain_tracker().to_greeting_message()
+        connection: Connection = listener.accept(sync_message)
+        connection.on_ready = lambda: self._on_connection_ready(connection)
+        self._connections.add(connection)
+        self._logger.info("accepted incoming connection from %s", connection)
+        return [connection]
 
     def start_listening(self, ip_addr="", port: Union[str, int] = "8080"):
         """ Listen for incoming connections on the given port.
 
             Note that you'll still need to call "run" to actually accept those connections.
         """
         port = int(port)
         self._logger.info("starting to listen on %r:%r", ip_addr, port)
-        self._listeners.add(Listener(WebsocketConnection, ip_addr=ip_addr, port=port))
+        listener = Listener(WebsocketConnection, ip_addr=ip_addr, port=port)
+        listener.on_ready = lambda: self._on_listener_ready(listener)
+        self._listeners.add(listener)
+        self._indicate_selectables_changed()
 
     def connect_to(self, target: str):
         """ initiate a connection to another gink instance """
         self._logger.info("initating connection to %s", target)
         match = fullmatch(r"(ws+://)?([a-z0-9.-]+)(?::(\d+))?(?:/+(.*))?$", target, IGNORECASE)
         assert match, f"can't connect to: {target}"
         prefix, host, port, path = match.groups()
         if prefix and prefix != "ws://":
             raise NotImplementedError("only vanilla websockets currently supported")
         port = port or "8080"
         path = path or "/"
         greeting = self._store.get_chain_tracker().to_greeting_message()
         connection = WebsocketConnection(host=host, port=int(port), path=path, greeting=greeting)
+        connection.on_ready = lambda: self._on_connection_ready(connection)
         self._connections.add(connection)
         self._logger.debug("connection added")
+        self._indicate_selectables_changed()
 
-    def run(self,
-            until: GenericTimestamp = None,
-            console: Optional[SelectableConsole]=None,
-            connect_to: Optional[list[str]]=None):
-        """ Waits for activity on ports then exchanges data with peers.
-            Optionally connects to other database instances.
-        """
-        if connect_to:
-            for target in connect_to:
-                self.connect_to(target)
-        self._logger.debug("starting run loop until %r", until)
-        if until is not None:
-            until = self.resolve_timestamp(until)
-        context_manager = console or nullcontext()
-        with context_manager:
-            while (until is None or generate_timestamp() < until):
-                # eventually will want to support epoll on platforms where its supported
-                readers: List[Union[Listener, WsgiListener, Connection, WsgiConnection, SelectableConsole, AbstractStore]] = []
-                if self._store.is_selectable():
-                        readers.append(self._store)
-                for listener in self._listeners:
-                    readers.append(listener)
-                for connection in list(self._connections):
-                    if connection.is_closed():
-                        self._connections.remove(connection)
-                    else:
-                        readers.append(connection)
-                if self._wsgi_listener:
-                    readers.append(self._wsgi_listener)
-                for conn in list(self._wsgi_connections):
-                    readers.append(conn)
-                if isinstance(console, SelectableConsole):
-                    readers.append(console)
-                    console.refresh()
-                ready_readers, _, _ = select(readers, [], [], 0.1)
-                for ready_reader in ready_readers:
-                    if isinstance(ready_reader, Connection):
-                        self._on_peer_ready(ready_reader)
-                        if ready_reader.is_closed():
-                            self._connections.remove(ready_reader)
-                            readers.remove(ready_reader)
-                    elif isinstance(ready_reader, WsgiListener) and self._wsgi_listener:
-                        conn = self._wsgi_listener.accept()
-                        if conn:
-                            self._wsgi_connections.add(conn)
-                            readers.append(conn)
-                    elif isinstance(ready_reader, WsgiConnection) and self._wsgi_listener:
-                        request_data = ready_reader.receive_data()
-                        result = self._wsgi_listener.process_request(request_data)
-                        if result != False:
-                            self._wsgi_listener.finish_response(result, ready_reader)
-                        ready_reader.close()
-                        self._wsgi_connections.remove(ready_reader)
-                        readers.remove(ready_reader)
-                    elif isinstance(ready_reader, Listener):
-                        sync_message = self._store.get_chain_tracker().to_greeting_message()
-                        new_connection: Connection = ready_reader.accept(sync_message)
-                        self._connections.add(new_connection)
-                        readers.append(new_connection)
-                        self._logger.info("accepted incoming connection from %s", new_connection)
-                    elif isinstance(ready_reader, SelectableConsole):
-                        ready_reader.call_when_ready()
-                    elif isinstance(ready_reader, AbstractStore):
-                        ready_reader.refresh(self._on_bundle)
+    def _on_store_ready(self):
+        self._store.refresh(self._on_bundle)
+
+    def on_ready(self) -> Iterable[Selectable]:
+        if self._indication_sent:
+            self._socket_rite.recv(1)
+            self._indication_sent = False
+        if self._store.is_selectable():
+            self._store.on_ready = self._on_store_ready
+            yield self._store
+        for listener in self._listeners:
+            yield listener
+        for connection in self._connections:
+            yield connection
+
+    def _indicate_selectables_changed(self):
+        if not self._indication_sent:
+            self._socket_left.send(b'0x01')
+            self._indication_sent = True
+
+    def close(self):
+        for connection in self._connections:
+            connection.close()
+        for listener in self._listeners:
+            listener.close()
+        self._store.close()
+        self._socket_left.close()
+        self._socket_rite.close()
 
     def reset(self, to_time: GenericTimestamp = EPOCH, *, bundler=None, comment=None):
         """ Resets the database to a specific point in time.
 
             Note that it literally just "re"-sets everything in one big
             bundle to the values that existed at that time, so you can always
             go and look at the state of the database beforehand.
```

### Comparing `gink-0.20240519.1716093142/gink/impl/deferred.py` & `gink-0.20240521.1716315298/gink/impl/deferred.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240519.1716093142/gink/impl/directory.py` & `gink-0.20240521.1716315298/gink/impl/directory.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240519.1716093142/gink/impl/graph.py` & `gink-0.20240521.1716315298/gink/impl/graph.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240519.1716093142/gink/impl/group.py` & `gink-0.20240521.1716315298/gink/impl/group.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240519.1716093142/gink/impl/key_set.py` & `gink-0.20240521.1716315298/gink/impl/key_set.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240519.1716093142/gink/impl/listener.py` & `gink-0.20240521.1716315298/gink/impl/listener.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """ contains the Listener class that listens on a port for incomming connections """
+from typing import Callable, Type
 from socket import (
     socket as Socket,
     AF_INET,
     SOCK_STREAM,
     SOL_SOCKET,
     SO_REUSEADDR,
 )
@@ -12,27 +13,32 @@
 from .connection import Connection
 from .websocket_connection import WebsocketConnection
 
 
 class Listener:
     """ Listens on a port for incoming connections. """
 
-    def __init__(self, connection_class=WebsocketConnection, ip_addr: str = "", port: int = 8080):
-        self.connection_class = connection_class
-        self.socket = Socket(AF_INET, SOCK_STREAM)
-        self.socket.setsockopt(SOL_SOCKET, SO_REUSEADDR, 1)
-        self.socket.bind((ip_addr, int(port)))
-        self.socket.listen(128)
+    on_ready: Callable  # needs to by dynamically assigned
+
+    def __init__(self, connection_class: Type[Connection]=WebsocketConnection, ip_addr: str = "", port: int = 8080):
+        self._connection_class = connection_class
+        self._socket = Socket(AF_INET, SOCK_STREAM)
+        self._socket.setsockopt(SOL_SOCKET, SO_REUSEADDR, 1)
+        self._socket.bind((ip_addr, int(port)))
+        self._socket.listen(128)
 
     def fileno(self):
         """ Gives the file descriptor for use in socket.select and similar. """
-        return self.socket.fileno()
+        return self._socket.fileno()
+
+    def close(self):
+        self._socket.close()
 
     def accept(self, greeting: SyncMessage) -> Connection:
         """ Method to call when the underlying socket is "ready". """
-        (new_socket, addr) = self.socket.accept()
-        peer: Connection = self.connection_class(
+        (new_socket, addr) = self._socket.accept()
+        peer: Connection = self._connection_class(
             socket=new_socket,
             host=addr[0],
             port=addr[1],
             greeting=greeting)
         return peer
```

### Comparing `gink-0.20240519.1716093142/gink/impl/lmdb_store.py` & `gink-0.20240521.1716315298/gink/impl/lmdb_store.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240519.1716093142/gink/impl/lmdb_utilities.py` & `gink-0.20240521.1716315298/gink/impl/lmdb_utilities.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240519.1716093142/gink/impl/log_backed_store.py` & `gink-0.20240521.1716315298/gink/impl/log_backed_store.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240519.1716093142/gink/impl/memory_store.py` & `gink-0.20240521.1716315298/gink/impl/memory_store.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240519.1716093142/gink/impl/muid.py` & `gink-0.20240521.1716315298/gink/impl/muid.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240519.1716093142/gink/impl/pair_map.py` & `gink-0.20240521.1716315298/gink/impl/pair_map.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240519.1716093142/gink/impl/pair_set.py` & `gink-0.20240521.1716315298/gink/impl/pair_set.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240519.1716093142/gink/impl/property.py` & `gink-0.20240521.1716315298/gink/impl/property.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240519.1716093142/gink/impl/selectable_console.py` & `gink-0.20240521.1716315298/gink/impl/selectable_console.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
             tcsetattr(self._input.fileno(), TCSADRAIN, self._settings)
             self._settings = None
 
     def _bytes_available(self) -> int:
         ioctl(self.fileno(), FIONREAD, self._c_int)  # type: ignore
         return self._c_int.value
 
-    def call_when_ready(self):
+    def on_ready(self):
         try:
             if self._interactive:
                 for _ in range(self._bytes_available()):
                   self.on_character(self._input.read(1))
             else:
                 self.on_line(input())
         except KeyboardInterrupt:
@@ -64,15 +64,15 @@
             pass
 
     def on_line(self, line):
         result = self.runsource(line)
         if result is True:
             self._logger.warning("multi-line input not yet implemented")
 
-    def refresh(self):
+    def on_timeout(self):
         if self._interactive:
             data = self._prompt + "".join(self._buffer)
             self._output.write("\r" + data + " ")
             self._output.write("\r" + data)
             self._output.flush()
             if self._heartbeat_to:
                 print(str(DateTime.now().time()), file=self._heartbeat_to)
```

### Comparing `gink-0.20240519.1716093142/gink/impl/sequence.py` & `gink-0.20240521.1716315298/gink/impl/sequence.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240519.1716093142/gink/impl/tuples.py` & `gink-0.20240521.1716315298/gink/impl/tuples.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240519.1716093142/gink/impl/typedefs.py` & `gink-0.20240521.1716315298/gink/impl/typedefs.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240519.1716093142/gink/impl/watcher.py` & `gink-0.20240521.1716315298/gink/impl/watcher.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240519.1716093142/gink/impl/websocket_connection.py` & `gink-0.20240521.1716315298/gink/impl/websocket_connection.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """ Contains the WsPeer class to manage a connection to a websocket (gink) peer. """
 
 # batteries included python imports
-from typing import Iterable, Optional
+from typing import Iterable, Optional, Callable
 from socket import (
     socket as Socket,
     SHUT_WR, SHUT_RDWR
 )
 from select import select
 from os import environ
 
@@ -25,38 +25,40 @@
 )
 
 # builders
 from .builders import SyncMessage
 
 # gink modules
 from .connection import Connection
+from .looping import Finished
 
 
 class WebsocketConnection(Connection):
     """ Manages the connection to one peer via a websocket.
 
         Set is_client to indicate that the provided socket is a client connection.
         If there's no socket provided then one will be established, and is_client is implied.
     """
     PROTOCOL = "gink"
-
+    on_ready: Callable
     def __init__(
             self,
             host: Optional[str] = None,
             port: Optional[int] = None,
             socket: Optional[Socket] = None,
             force_to_be_client: bool = False,
             path: Optional[str] = None,
             greeting: Optional[SyncMessage] = None
     ):
-        Connection.__init__(self, socket=socket, host=host, port=port)
+        Connection.__init__(self, socket=socket, host=host, port=port, greeting=greeting)
         if socket is None:
             force_to_be_client = True
         connection_type = ConnectionType.CLIENT if force_to_be_client else ConnectionType.SERVER
         self._ws = WSConnection(connection_type=connection_type)
+        self._ws_closed = False
         self._buffered: bytes = b""
         self._ready = False
         self.auth_token = environ.get("GINK_AUTH_TOKEN")
         if force_to_be_client:
             subprotocols = [self.PROTOCOL]
 
             if self.auth_token:
@@ -65,25 +67,26 @@
 
             host = host or "localhost"
             path = path or "/"
             request = Request(host=host, target=path, subprotocols=subprotocols)
             self._socket.send(self._ws.send(request))
         self._logger.debug("finished setup")
         self._socket.settimeout(0.2)
-        self._greeting = greeting
+
 
     def __repr__(self):
         return f"{self.__class__.__name__}(host={self._host!r})"
 
     def receive(self) -> Iterable[SyncMessage]:
         if self._closed:
-            return
+            raise Finished()
         data = self._socket.recv(4096 * 4096)
         if not data:
-            self._closed = True
+            self._ws_closed = True
+            raise Finished()
         self._ws.receive_data(data)
         for event in self._ws.events():
             if isinstance(event, Request):
                 if self.auth_token:
                     # Ensures any capitalization of 'Token' and any number of spaces works
                     key = self.auth_token.lower().split("token ")[1].lstrip()
                     token = None
@@ -105,22 +108,20 @@
                     self._logger.debug("got a Request, sending an AcceptConnection")
                     self._socket.send(self._ws.send(AcceptConnection("gink")))
                     self._logger.info("Server connection established!")
                     self._send_greeting()
                     self._ready = True
             elif isinstance(event, CloseConnection):
                 self._logger.info("got close msg, code=%d, reason=%s", event.code, event.reason)
-                self._closed = True
                 try:
                     self._socket.send(self._ws.send(event.response()))
-                    self._socket.shutdown(SHUT_RDWR)
                 except BrokenPipeError:
                     self._logger.warning("could not send websocket close ack")
-                self._socket.close()
-                return
+                self._ws_closed = True
+                raise Finished()
             elif isinstance(event, TextMessage):
                 self._logger.info('Text message received: %r', event.data)
             elif isinstance(event, BytesMessage):
                 received = bytes(event.data) if isinstance(event.data, bytearray) else event.data
                 assert isinstance(received, bytes)
                 self._logger.debug('We got %d bytes!', len(received))
                 if event.message_finished:
@@ -153,29 +154,35 @@
 
     def send(self, sync_message: SyncMessage) -> int:
         assert not self._closed
         data = self._ws.send(BytesMessage(sync_message.SerializeToString()))
         return self._socket.send(data)
 
     def close(self, reason=None):
-        self._closed = True
+        if self._closed:
+            return
         code = 1000
         if reason is not None:
             raise NotImplementedError()
         try:
-            self._socket.send(self._ws.send(CloseConnection(code=code)))
-            self._socket.shutdown(SHUT_WR)
+            if not self._ws_closed:
+                self._socket.send(self._ws.send(CloseConnection(code=code)))
+                self._socket.shutdown(SHUT_WR)
+                self._ws_closed = True
+            """
             self._logger.debug("Sent connection close message, waiting for close ack.")
             while True:
                 ready = select([self._socket], [], [], 0.2)
                 if not ready[0]:
                     self._logger.warning("timed out waiting for peer to ack my close message")
                     break
                 data = self._socket.recv(2 ** 30)
                 self._ws.receive_data(data)
                 for event in self._ws.events():
                     if isinstance(event, CloseConnection):
                         self._logger.debug("Received close connnection ack.")
                         break
                     self._logger.warning("got something unexpected waiting for close: %s", event)
+            """
         finally:
             self._socket.close()
+            self._closed = True
```

### Comparing `gink-0.20240519.1716093142/gink/tests/test_box.py` & `gink-0.20240521.1716315298/gink/tests/test_box.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240519.1716093142/gink/tests/test_braid.py` & `gink-0.20240521.1716315298/gink/tests/test_braid.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240519.1716093142/gink/tests/test_chain_tracker.py` & `gink-0.20240521.1716315298/gink/tests/test_chain_tracker.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240519.1716093142/gink/tests/test_change_set_info.py` & `gink-0.20240521.1716315298/gink/tests/test_change_set_info.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240519.1716093142/gink/tests/test_code_values.py` & `gink-0.20240521.1716315298/gink/tests/test_code_values.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240519.1716093142/gink/tests/test_container.py` & `gink-0.20240521.1716315298/gink/tests/test_container.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240519.1716093142/gink/tests/test_database.py` & `gink-0.20240521.1716315298/gink/tests/test_database.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from ..impl.lmdb_store import LmdbStore
 from ..impl.bundler import Bundler
 from ..impl.bundle_info import BundleInfo
 from ..impl.directory import Directory
 from ..impl.sequence import Sequence
 from ..impl.key_set import KeySet
 from ..impl.log_backed_store import LogBackedStore
+from ..impl.looping import loop
 
 
 def test_database():
     """ tests that the last() thing works """
     store = MemoryStore()
     database = Database(store=store)
     last = Database.get_last()
@@ -119,19 +120,19 @@
 
         db1a = Database(store1a)
         db1b = Database(store1b)
 
         root1a = Directory(arche=True, database=db1a)
         root1b = Directory(arche=True, database=db1b)
 
-        db1b.run(0.01)
+        loop(db1b, until=.01)
         bundle_infos = list()
         db1b.add_callback(lambda bi: bundle_infos.append(bi))
         root1a.set("foo", "bar", comment="abc")
-        db1b.run(0.01)
+        loop(db1b, until=.01)
         assert bundle_infos and bundle_infos[-1].comment == "abc"
         found = root1b.get("foo")
         assert found == "bar", found
 
 
 def test_dump():
     """
```

### Comparing `gink-0.20240519.1716093142/gink/tests/test_demo.py` & `gink-0.20240521.1716315298/gink/tests/test_demo.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240519.1716093142/gink/tests/test_directory.py` & `gink-0.20240521.1716315298/gink/tests/test_directory.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240519.1716093142/gink/tests/test_graph.py` & `gink-0.20240521.1716315298/gink/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240519.1716093142/gink/tests/test_key_set.py` & `gink-0.20240521.1716315298/gink/tests/test_key_set.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240519.1716093142/gink/tests/test_lmdb_store.py` & `gink-0.20240521.1716315298/gink/tests/test_lmdb_store.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240519.1716093142/gink/tests/test_logbackedstore.py` & `gink-0.20240521.1716315298/gink/tests/test_logbackedstore.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240519.1716093142/gink/tests/test_muid.py` & `gink-0.20240521.1716315298/gink/tests/test_muid.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240519.1716093142/gink/tests/test_names.py` & `gink-0.20240521.1716315298/gink/tests/test_names.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240519.1716093142/gink/tests/test_pair_map.py` & `gink-0.20240521.1716315298/gink/tests/test_pair_map.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240519.1716093142/gink/tests/test_pair_set.py` & `gink-0.20240521.1716315298/gink/tests/test_pair_set.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240519.1716093142/gink/tests/test_property.py` & `gink-0.20240521.1716315298/gink/tests/test_property.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240519.1716093142/gink/tests/test_role.py` & `gink-0.20240521.1716315298/gink/tests/test_role.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240519.1716093142/gink/tests/test_sequence.py` & `gink-0.20240521.1716315298/gink/tests/test_sequence.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240519.1716093142/gink/tests/test_store.py` & `gink-0.20240521.1716315298/gink/tests/test_store.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240519.1716093142/gink/tests/test_websocket_connection.py` & `gink-0.20240521.1716315298/gink/tests/test_websocket_connection.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import os
 
 # builders
 from ..impl.builders import SyncMessage
 from google.protobuf.text_format import Parse  # type: ignore
 
-from ..impl.websocket_connection import WebsocketConnection
+from ..impl.websocket_connection import WebsocketConnection, Finished
 
 logging.basicConfig(level=logging.DEBUG)
 
 
 def test_chit_chat():
     """ ensures that I can send and receive data via a websocket connection """
     server_socket, client_socket = socketpair()
@@ -48,16 +48,19 @@
 
     for message in [sync_message]:
         client.send(message)
         for incoming in server.receive():
             assert incoming == message, incoming
 
     client.close()
-    for _ in server.receive():
-        raise Exception("not expected")
+    try:
+        for _ in server.receive():
+            raise Exception("not expected")
+    except Finished:
+        server.close()
 
     assert client.is_closed() and server.is_closed()
 
 def test_auth():
     """ tests authentication """
     server_socket, client_socket = socketpair()
```

### Comparing `gink-0.20240519.1716093142/gink.egg-info/PKG-INFO` & `gink-0.20240521.1716315298/gink.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gink
-Version: 0.20240519.1716093142
+Version: 0.20240521.1716315298
 Summary: a system for storing data structures in lmdb
 Home-page: https://github.com/x5e/gink
 Author: Darin McGill
 Author-email: gink@darinmcgill.com
 Keywords: gink lmdb crdt history versioned
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `gink-0.20240519.1716093142/gink.egg-info/SOURCES.txt` & `gink-0.20240521.1716315298/gink.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 gink/impl/graph.py
 gink/impl/group.py
 gink/impl/key_set.py
 gink/impl/listener.py
 gink/impl/lmdb_store.py
 gink/impl/lmdb_utilities.py
 gink/impl/log_backed_store.py
+gink/impl/looping.py
 gink/impl/memory_store.py
 gink/impl/muid.py
 gink/impl/pair_map.py
 gink/impl/pair_set.py
 gink/impl/property.py
 gink/impl/selectable_console.py
 gink/impl/sequence.py
```

### Comparing `gink-0.20240519.1716093142/setup.py` & `gink-0.20240521.1716315298/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 
 setup(
     name='gink',
-    version='0.20240519.1716093142',
+    version='0.20240521.1716315298',
     description='a system for storing data structures in lmdb',
     url='https://github.com/x5e/gink',
     author='Darin McGill',
     author_email="gink@darinmcgill.com",
     classifiers=[
         'Development Status :: 4 - Beta',
         "Intended Audience :: Developers",
```

