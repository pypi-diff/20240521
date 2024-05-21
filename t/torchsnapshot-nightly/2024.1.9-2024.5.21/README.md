# Comparing `tmp/torchsnapshot-nightly-2024.1.9.tar.gz` & `tmp/torchsnapshot_nightly-2024.5.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchsnapshot-nightly-2024.1.9.tar", last modified: Tue Jan  9 11:32:49 2024, max compression
+gzip compressed data, was "torchsnapshot_nightly-2024.5.21.tar", last modified: Tue May 21 00:41:24 2024, max compression
```

## Comparing `torchsnapshot-nightly-2024.1.9.tar` & `torchsnapshot_nightly-2024.5.21.tar`

### file list

```diff
@@ -1,87 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 11:32:49.917485 torchsnapshot-nightly-2024.1.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-01-09 11:31:38.000000 torchsnapshot-nightly-2024.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5010 2024-01-09 11:32:49.917485 torchsnapshot-nightly-2024.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-01-09 11:31:38.000000 torchsnapshot-nightly-2024.1.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-01-09 11:31:38.000000 torchsnapshot-nightly-2024.1.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-09 11:32:49.917485 torchsnapshot-nightly-2024.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-01-09 11:31:38.000000 torchsnapshot-nightly-2024.1.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 11:32:49.909484 torchsnapshot-nightly-2024.1.9/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4396 2024-01-09 11:31:38.000000 torchsnapshot-nightly-2024.1.9/tests/test_async_take.py
--rw-r--r--   0 runner    (1001) docker     (127)    13577 2024-01-09 11:31:38.000000 torchsnapshot-nightly-2024.1.9/tests/test_batcher.py
--rw-r--r--   0 runner    (1001) docker     (127)    11615 2024-01-09 11:31:38.000000 torchsnapshot-nightly-2024.1.9/tests/test_chunked_tensor_io_preparer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6774 2024-01-09 11:31:38.000000 torchsnapshot-nightly-2024.1.9/tests/test_ddp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4118 2024-01-09 11:31:38.000000 torchsnapshot-nightly-2024.1.9/tests/test_ddp_infer_replication.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-01-09 11:31:38.000000 torchsnapshot-nightly-2024.1.9/tests/test_ddp_replication_glob.py
--rw-r--r--   0 runner    (1001) docker     (127)     6834 2024-01-09 11:31:38.000000 torchsnapshot-nightly-2024.1.9/tests/test_dist_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     6982 2024-01-09 11:31:38.000000 torchsnapshot-nightly-2024.1.9/tests/test_flatten.py
--rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-01-09 11:31:38.000000 torchsnapshot-nightly-2024.1.9/tests/test_fs_storage_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4147 2024-01-09 11:31:38.000000 torchsnapshot-nightly-2024.1.9/tests/test_gcs_storage_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)    27111 2024-01-09 11:31:38.000000 torchsnapshot-nightly-2024.1.9/tests/test_manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-01-09 11:31:38.000000 torchsnapshot-nightly-2024.1.9/tests/test_memoryview_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     8791 2024-01-09 11:31:38.000000 torchsnapshot-nightly-2024.1.9/tests/test_partitioner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-01-09 11:31:38.000000 torchsnapshot-nightly-2024.1.9/tests/test_pg_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     5764 2024-01-09 11:31:38.000000 torchsnapshot-nightly-2024.1.9/tests/test_read_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     3340 2024-01-09 11:31:38.000000 torchsnapshot-nightly-2024.1.9/tests/test_replication_glob.py
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-01-09 11:31:38.000000 torchsnapshot-nightly-2024.1.9/tests/test_rng_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-01-09 11:31:38.000000 torchsnapshot-nightly-2024.1.9/tests/test_rss_profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3341 2024-01-09 11:31:38.000000 torchsnapshot-nightly-2024.1.9/tests/test_s3_storage_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-01-09 11:31:38.000000 torchsnapshot-nightly-2024.1.9/tests/test_serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)    10052 2024-01-09 11:31:38.000000 torchsnapshot-nightly-2024.1.9/tests/test_sharded_tensor_io_preparer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3455 2024-01-09 11:31:38.000000 torchsnapshot-nightly-2024.1.9/tests/test_sharded_tensor_resharding.py
--rw-r--r--   0 runner    (1001) docker     (127)     6545 2024-01-09 11:31:38.000000 torchsnapshot-nightly-2024.1.9/tests/test_snapshot.py
--rw-r--r--   0 runner    (1001) docker     (127)    13654 2024-01-09 11:31:38.000000 torchsnapshot-nightly-2024.1.9/tests/test_tensor_io_preparer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4971 2024-01-09 11:31:38.000000 torchsnapshot-nightly-2024.1.9/tests/test_test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-01-09 11:31:38.000000 torchsnapshot-nightly-2024.1.9/tests/test_uvm_tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 11:32:49.913484 torchsnapshot-nightly-2024.1.9/torchsnapshot/
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-01-09 11:31:38.000000 torchsnapshot-nightly-2024.1.9/torchsnapshot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17888 2024-01-09 11:31:38.000000 torchsnapshot-nightly-2024.1.9/torchsnapshot/batcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     6143 2024-01-09 11:31:38.000000 torchsnapshot-nightly-2024.1.9/torchsnapshot/dist_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-01-09 11:31:38.000000 torchsnapshot-nightly-2024.1.9/torchsnapshot/dtensor_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-01-09 11:31:38.000000 torchsnapshot-nightly-2024.1.9/torchsnapshot/event.py
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-01-09 11:31:38.000000 torchsnapshot-nightly-2024.1.9/torchsnapshot/event_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7681 2024-01-09 11:31:38.000000 torchsnapshot-nightly-2024.1.9/torchsnapshot/flatten.py
--rw-r--r--   0 runner    (1001) docker     (127)     6490 2024-01-09 11:31:38.000000 torchsnapshot-nightly-2024.1.9/torchsnapshot/io_preparer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 11:32:49.913484 torchsnapshot-nightly-2024.1.9/torchsnapshot/io_preparers/
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-01-09 11:31:38.000000 torchsnapshot-nightly-2024.1.9/torchsnapshot/io_preparers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4339 2024-01-09 11:31:38.000000 torchsnapshot-nightly-2024.1.9/torchsnapshot/io_preparers/chunked_tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)    10398 2024-01-09 11:31:38.000000 torchsnapshot-nightly-2024.1.9/torchsnapshot/io_preparers/dtensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-01-09 11:31:38.000000 torchsnapshot-nightly-2024.1.9/torchsnapshot/io_preparers/object.py
--rw-r--r--   0 runner    (1001) docker     (127)    12198 2024-01-09 11:31:38.000000 torchsnapshot-nightly-2024.1.9/torchsnapshot/io_preparers/sharded_tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)    15266 2024-01-09 11:31:38.000000 torchsnapshot-nightly-2024.1.9/torchsnapshot/io_preparers/tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-01-09 11:31:38.000000 torchsnapshot-nightly-2024.1.9/torchsnapshot/io_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4195 2024-01-09 11:31:38.000000 torchsnapshot-nightly-2024.1.9/torchsnapshot/knobs.py
--rw-r--r--   0 runner    (1001) docker     (127)    15498 2024-01-09 11:31:38.000000 torchsnapshot-nightly-2024.1.9/torchsnapshot/manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)    10417 2024-01-09 11:31:38.000000 torchsnapshot-nightly-2024.1.9/torchsnapshot/manifest_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-01-09 11:31:38.000000 torchsnapshot-nightly-2024.1.9/torchsnapshot/manifest_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-01-09 11:31:38.000000 torchsnapshot-nightly-2024.1.9/torchsnapshot/memoryview_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)    13825 2024-01-09 11:31:38.000000 torchsnapshot-nightly-2024.1.9/torchsnapshot/partitioner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-01-09 11:31:38.000000 torchsnapshot-nightly-2024.1.9/torchsnapshot/pg_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 11:31:38.000000 torchsnapshot-nightly-2024.1.9/torchsnapshot/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-01-09 11:31:38.000000 torchsnapshot-nightly-2024.1.9/torchsnapshot/rng_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-01-09 11:31:38.000000 torchsnapshot-nightly-2024.1.9/torchsnapshot/rss_profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)    16816 2024-01-09 11:31:38.000000 torchsnapshot-nightly-2024.1.9/torchsnapshot/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)    15247 2024-01-09 11:31:38.000000 torchsnapshot-nightly-2024.1.9/torchsnapshot/serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)    36922 2024-01-09 11:31:38.000000 torchsnapshot-nightly-2024.1.9/torchsnapshot/snapshot.py
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-01-09 11:31:38.000000 torchsnapshot-nightly-2024.1.9/torchsnapshot/state_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-01-09 11:31:38.000000 torchsnapshot-nightly-2024.1.9/torchsnapshot/stateful.py
--rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-01-09 11:31:38.000000 torchsnapshot-nightly-2024.1.9/torchsnapshot/storage_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 11:32:49.913484 torchsnapshot-nightly-2024.1.9/torchsnapshot/storage_plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-01-09 11:31:38.000000 torchsnapshot-nightly-2024.1.9/torchsnapshot/storage_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-01-09 11:31:38.000000 torchsnapshot-nightly-2024.1.9/torchsnapshot/storage_plugins/fs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9792 2024-01-09 11:31:38.000000 torchsnapshot-nightly-2024.1.9/torchsnapshot/storage_plugins/gcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-01-09 11:31:38.000000 torchsnapshot-nightly-2024.1.9/torchsnapshot/storage_plugins/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     9648 2024-01-09 11:31:38.000000 torchsnapshot-nightly-2024.1.9/torchsnapshot/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 11:32:49.913484 torchsnapshot-nightly-2024.1.9/torchsnapshot/tricks/
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-01-09 11:31:38.000000 torchsnapshot-nightly-2024.1.9/torchsnapshot/tricks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-01-09 11:31:38.000000 torchsnapshot-nightly-2024.1.9/torchsnapshot/tricks/ddp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-01-09 11:31:38.000000 torchsnapshot-nightly-2024.1.9/torchsnapshot/tricks/deepspeed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-01-09 11:31:38.000000 torchsnapshot-nightly-2024.1.9/torchsnapshot/tricks/fsdp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-01-09 11:31:38.000000 torchsnapshot-nightly-2024.1.9/torchsnapshot/uvm_tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-01-09 11:31:38.000000 torchsnapshot-nightly-2024.1.9/torchsnapshot/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 11:32:49.913484 torchsnapshot-nightly-2024.1.9/torchsnapshot_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5010 2024-01-09 11:32:49.000000 torchsnapshot-nightly-2024.1.9/torchsnapshot_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-01-09 11:32:49.000000 torchsnapshot-nightly-2024.1.9/torchsnapshot_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-09 11:32:49.000000 torchsnapshot-nightly-2024.1.9/torchsnapshot_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-01-09 11:32:49.000000 torchsnapshot-nightly-2024.1.9/torchsnapshot_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-01-09 11:32:49.000000 torchsnapshot-nightly-2024.1.9/torchsnapshot_nightly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-09 11:32:49.000000 torchsnapshot-nightly-2024.1.9/torchsnapshot_nightly.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 00:41:24.027668 torchsnapshot_nightly-2024.5.21/
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-21 00:40:13.000000 torchsnapshot_nightly-2024.5.21/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-05-21 00:41:24.027668 torchsnapshot_nightly-2024.5.21/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-05-21 00:40:13.000000 torchsnapshot_nightly-2024.5.21/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-21 00:40:13.000000 torchsnapshot_nightly-2024.5.21/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 00:41:24.027668 torchsnapshot_nightly-2024.5.21/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-05-21 00:40:13.000000 torchsnapshot_nightly-2024.5.21/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 00:41:24.019668 torchsnapshot_nightly-2024.5.21/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4411 2024-05-21 00:40:13.000000 torchsnapshot_nightly-2024.5.21/tests/test_async_take.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13778 2024-05-21 00:40:13.000000 torchsnapshot_nightly-2024.5.21/tests/test_batcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11630 2024-05-21 00:40:13.000000 torchsnapshot_nightly-2024.5.21/tests/test_chunked_tensor_io_preparer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6789 2024-05-21 00:40:13.000000 torchsnapshot_nightly-2024.5.21/tests/test_ddp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4133 2024-05-21 00:40:13.000000 torchsnapshot_nightly-2024.5.21/tests/test_ddp_infer_replication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-05-21 00:40:13.000000 torchsnapshot_nightly-2024.5.21/tests/test_ddp_replication_glob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6849 2024-05-21 00:40:13.000000 torchsnapshot_nightly-2024.5.21/tests/test_dist_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7005 2024-05-21 00:40:13.000000 torchsnapshot_nightly-2024.5.21/tests/test_flatten.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-05-21 00:40:13.000000 torchsnapshot_nightly-2024.5.21/tests/test_fs_storage_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4162 2024-05-21 00:40:13.000000 torchsnapshot_nightly-2024.5.21/tests/test_gcs_storage_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27126 2024-05-21 00:40:13.000000 torchsnapshot_nightly-2024.5.21/tests/test_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-21 00:40:13.000000 torchsnapshot_nightly-2024.5.21/tests/test_memoryview_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8806 2024-05-21 00:40:13.000000 torchsnapshot_nightly-2024.5.21/tests/test_partitioner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-21 00:40:13.000000 torchsnapshot_nightly-2024.5.21/tests/test_pg_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5779 2024-05-21 00:40:13.000000 torchsnapshot_nightly-2024.5.21/tests/test_read_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3355 2024-05-21 00:40:13.000000 torchsnapshot_nightly-2024.5.21/tests/test_replication_glob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-21 00:40:13.000000 torchsnapshot_nightly-2024.5.21/tests/test_rng_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-21 00:40:13.000000 torchsnapshot_nightly-2024.5.21/tests/test_rss_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-05-21 00:40:13.000000 torchsnapshot_nightly-2024.5.21/tests/test_s3_storage_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-05-21 00:40:13.000000 torchsnapshot_nightly-2024.5.21/tests/test_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10067 2024-05-21 00:40:13.000000 torchsnapshot_nightly-2024.5.21/tests/test_sharded_tensor_io_preparer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-05-21 00:40:13.000000 torchsnapshot_nightly-2024.5.21/tests/test_sharded_tensor_resharding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7905 2024-05-21 00:40:13.000000 torchsnapshot_nightly-2024.5.21/tests/test_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-05-21 00:40:13.000000 torchsnapshot_nightly-2024.5.21/tests/test_state_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13669 2024-05-21 00:40:13.000000 torchsnapshot_nightly-2024.5.21/tests/test_tensor_io_preparer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5075 2024-05-21 00:40:13.000000 torchsnapshot_nightly-2024.5.21/tests/test_test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-21 00:40:13.000000 torchsnapshot_nightly-2024.5.21/tests/test_uvm_tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 00:41:24.023668 torchsnapshot_nightly-2024.5.21/torchsnapshot/
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-21 00:40:13.000000 torchsnapshot_nightly-2024.5.21/torchsnapshot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17905 2024-05-21 00:40:13.000000 torchsnapshot_nightly-2024.5.21/torchsnapshot/batcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6158 2024-05-21 00:40:13.000000 torchsnapshot_nightly-2024.5.21/torchsnapshot/dist_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-21 00:40:13.000000 torchsnapshot_nightly-2024.5.21/torchsnapshot/dtensor_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-21 00:40:13.000000 torchsnapshot_nightly-2024.5.21/torchsnapshot/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-21 00:40:13.000000 torchsnapshot_nightly-2024.5.21/torchsnapshot/event_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7696 2024-05-21 00:40:13.000000 torchsnapshot_nightly-2024.5.21/torchsnapshot/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6346 2024-05-21 00:40:13.000000 torchsnapshot_nightly-2024.5.21/torchsnapshot/io_preparer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 00:41:24.023668 torchsnapshot_nightly-2024.5.21/torchsnapshot/io_preparers/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-21 00:40:13.000000 torchsnapshot_nightly-2024.5.21/torchsnapshot/io_preparers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4354 2024-05-21 00:40:13.000000 torchsnapshot_nightly-2024.5.21/torchsnapshot/io_preparers/chunked_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10746 2024-05-21 00:40:13.000000 torchsnapshot_nightly-2024.5.21/torchsnapshot/io_preparers/dtensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-05-21 00:40:13.000000 torchsnapshot_nightly-2024.5.21/torchsnapshot/io_preparers/object.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12707 2024-05-21 00:40:13.000000 torchsnapshot_nightly-2024.5.21/torchsnapshot/io_preparers/sharded_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15281 2024-05-21 00:40:13.000000 torchsnapshot_nightly-2024.5.21/torchsnapshot/io_preparers/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-05-21 00:40:13.000000 torchsnapshot_nightly-2024.5.21/torchsnapshot/io_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4210 2024-05-21 00:40:13.000000 torchsnapshot_nightly-2024.5.21/torchsnapshot/knobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15513 2024-05-21 00:40:13.000000 torchsnapshot_nightly-2024.5.21/torchsnapshot/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10432 2024-05-21 00:40:13.000000 torchsnapshot_nightly-2024.5.21/torchsnapshot/manifest_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3247 2024-05-21 00:40:13.000000 torchsnapshot_nightly-2024.5.21/torchsnapshot/manifest_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-05-21 00:40:13.000000 torchsnapshot_nightly-2024.5.21/torchsnapshot/memoryview_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13859 2024-05-21 00:40:13.000000 torchsnapshot_nightly-2024.5.21/torchsnapshot/partitioner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-05-21 00:40:13.000000 torchsnapshot_nightly-2024.5.21/torchsnapshot/pg_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 00:40:13.000000 torchsnapshot_nightly-2024.5.21/torchsnapshot/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-21 00:40:13.000000 torchsnapshot_nightly-2024.5.21/torchsnapshot/rng_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-21 00:40:13.000000 torchsnapshot_nightly-2024.5.21/torchsnapshot/rss_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16831 2024-05-21 00:40:13.000000 torchsnapshot_nightly-2024.5.21/torchsnapshot/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15262 2024-05-21 00:40:13.000000 torchsnapshot_nightly-2024.5.21/torchsnapshot/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40127 2024-05-21 00:40:13.000000 torchsnapshot_nightly-2024.5.21/torchsnapshot/snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-21 00:40:13.000000 torchsnapshot_nightly-2024.5.21/torchsnapshot/state_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-21 00:40:13.000000 torchsnapshot_nightly-2024.5.21/torchsnapshot/stateful.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-05-21 00:40:13.000000 torchsnapshot_nightly-2024.5.21/torchsnapshot/storage_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 00:41:24.023668 torchsnapshot_nightly-2024.5.21/torchsnapshot/storage_plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-21 00:40:13.000000 torchsnapshot_nightly-2024.5.21/torchsnapshot/storage_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-05-21 00:40:13.000000 torchsnapshot_nightly-2024.5.21/torchsnapshot/storage_plugins/fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9807 2024-05-21 00:40:13.000000 torchsnapshot_nightly-2024.5.21/torchsnapshot/storage_plugins/gcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-05-21 00:40:13.000000 torchsnapshot_nightly-2024.5.21/torchsnapshot/storage_plugins/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9949 2024-05-21 00:40:13.000000 torchsnapshot_nightly-2024.5.21/torchsnapshot/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 00:41:24.023668 torchsnapshot_nightly-2024.5.21/torchsnapshot/tricks/
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-21 00:40:13.000000 torchsnapshot_nightly-2024.5.21/torchsnapshot/tricks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-05-21 00:40:13.000000 torchsnapshot_nightly-2024.5.21/torchsnapshot/tricks/ddp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-05-21 00:40:13.000000 torchsnapshot_nightly-2024.5.21/torchsnapshot/tricks/deepspeed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-05-21 00:40:13.000000 torchsnapshot_nightly-2024.5.21/torchsnapshot/tricks/fsdp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-21 00:40:13.000000 torchsnapshot_nightly-2024.5.21/torchsnapshot/uvm_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-21 00:40:13.000000 torchsnapshot_nightly-2024.5.21/torchsnapshot/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 00:41:24.027668 torchsnapshot_nightly-2024.5.21/torchsnapshot_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-05-21 00:41:23.000000 torchsnapshot_nightly-2024.5.21/torchsnapshot_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-05-21 00:41:23.000000 torchsnapshot_nightly-2024.5.21/torchsnapshot_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 00:41:23.000000 torchsnapshot_nightly-2024.5.21/torchsnapshot_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-21 00:41:23.000000 torchsnapshot_nightly-2024.5.21/torchsnapshot_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-21 00:41:23.000000 torchsnapshot_nightly-2024.5.21/torchsnapshot_nightly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 00:41:23.000000 torchsnapshot_nightly-2024.5.21/torchsnapshot_nightly.egg-info/zip-safe
```

### Comparing `torchsnapshot-nightly-2024.1.9/LICENSE` & `torchsnapshot_nightly-2024.5.21/LICENSE`

 * *Files identical despite different names*

### Comparing `torchsnapshot-nightly-2024.1.9/PKG-INFO` & `torchsnapshot_nightly-2024.5.21/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchsnapshot-nightly
-Version: 2024.1.9
+Version: 2024.5.21
 Summary: A performant, memory-efficient checkpointing library for PyTorch applications, designed with large, complex distributed workloads in mind.
 Home-page: https://github.com/pytorch/torchsnapshot
 Author: torchsnapshot team
 Author-email: yifu@fb.com
 License: BSD-3
 Keywords: pytorch,snapshot,checkpoint
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -30,15 +30,15 @@
 Requires-Dist: aiobotocore; extra == "dev"
 Requires-Dist: boto3; extra == "dev"
 Requires-Dist: expecttest; extra == "dev"
 Requires-Dist: google-cloud-storage; extra == "dev"
 Requires-Dist: google-resumable-media; extra == "dev"
 Requires-Dist: numpy; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
-Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest==8.1.1; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pytest-timeout; extra == "dev"
 
 # TorchSnapshot (Beta Release)
 
 <p align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: torchsnapshot-nightly Version: 2024.1.9 Summary: A
+Metadata-Version: 2.1 Name: torchsnapshot-nightly Version: 2024.5.21 Summary: A
 performant, memory-efficient checkpointing library for PyTorch applications,
 designed with large, complex distributed workloads in mind. Home-page: https://
 github.com/pytorch/torchsnapshot Author: torchsnapshot team Author-email:
 yifu@fb.com License: BSD-3 Keywords: pytorch,snapshot,checkpoint Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: BSD License Classifier: Programming Language :: Python :: 3
@@ -12,17 +12,17 @@
 PyYAML Requires-Dist: aiofiles Requires-Dist: aiohttp Requires-Dist: importlib-
 metadata Requires-Dist: nest_asyncio Requires-Dist: psutil Requires-Dist:
 pyre_extensions Requires-Dist: torch Requires-Dist: typing-extensions Provides-
 Extra: dev Requires-Dist: aiobotocore; extra == "dev" Requires-Dist: boto3;
 extra == "dev" Requires-Dist: expecttest; extra == "dev" Requires-Dist: google-
 cloud-storage; extra == "dev" Requires-Dist: google-resumable-media; extra ==
 "dev" Requires-Dist: numpy; extra == "dev" Requires-Dist: pre-commit; extra ==
-"dev" Requires-Dist: pytest; extra == "dev" Requires-Dist: pytest-asyncio;
-extra == "dev" Requires-Dist: pytest-cov; extra == "dev" Requires-Dist: pytest-
-timeout; extra == "dev" # TorchSnapshot (Beta Release)
+"dev" Requires-Dist: pytest==8.1.1; extra == "dev" Requires-Dist: pytest-
+asyncio; extra == "dev" Requires-Dist: pytest-cov; extra == "dev" Requires-
+Dist: pytest-timeout; extra == "dev" # TorchSnapshot (Beta Release)
 _[_b_u_i_l_d_ _s_t_a_t_u_s_]_[_p_y_p_i_ _v_e_r_s_i_o_n_]_[_c_o_n_d_a_ _v_e_r_s_i_o_n_]_[_p_y_p_i_ _n_i_g_h_t_l_y_ _v_e_r_s_i_o_n_]_[_c_o_d_e_c_o_v_]_[_b_s_d
                                    _l_i_c_e_n_s_e_]
 A performant, memory-efficient checkpointing library for PyTorch applications,
 designed with large, complex distributed workloads in mind. ## Install Requires
 Python >= 3.8 and PyTorch >= 2.0.0 From pip: ```bash # Stable pip install
 torchsnapshot # Or, using conda conda install -c conda-forge torchsnapshot #
 Nightly pip install --pre torchsnapshot-nightly ``` From source: ```bash git
```

### Comparing `torchsnapshot-nightly-2024.1.9/README.md` & `torchsnapshot_nightly-2024.5.21/README.md`

 * *Files identical despite different names*

### Comparing `torchsnapshot-nightly-2024.1.9/setup.py` & `torchsnapshot_nightly-2024.5.21/setup.py`

 * *Files identical despite different names*

### Comparing `torchsnapshot-nightly-2024.1.9/tests/test_async_take.py` & `torchsnapshot_nightly-2024.5.21/tests/test_async_take.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 import asyncio
 import os
 import tempfile
 import unittest
 from unittest.mock import patch
 
 import torch
```

### Comparing `torchsnapshot-nightly-2024.1.9/tests/test_batcher.py` & `torchsnapshot_nightly-2024.5.21/tests/test_batcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 # pyre-ignore-all-errors[21, 56]: ignore pytest undefine import and invalid decoration
 import copy
 import random
 import sys
 
 import uuid
 from typing import cast, Generator, List, Optional, Tuple
@@ -159,16 +161,18 @@
 
     placements = [Replicate()]
 
     srcs = []
     dsts = []
     for idx in range(NUM_TENSORS):
         mesh = (
+            # pyre-fixme[6]: For 2nd argument expected `Union[_SupportsArray[typing.A...
             DeviceMesh("cuda", mesh=[0])
             if use_gpu and idx % 2 == 0
+            # pyre-fixme[6]: For 2nd argument expected `Union[_SupportsArray[typing.A...
             else DeviceMesh("cpu", mesh=[0])
         )
         srcs.append(
             distribute_tensor(
                 tensor=torch.rand(*TENSOR_SHAPE),
                 device_mesh=mesh,
                 placements=placements,
@@ -381,17 +385,17 @@
 
     # Prepare read requests for the dst tensors
     read_reqs = []
     for entry, obj_out in zip(entries, dst_tensors + [None] * NUM_TENSORS):
         rrs, _ = prepare_read(
             entry=entry,
             obj_out=obj_out,
-            buffer_size_limit_bytes=read_chunk_size_bytes
-            if enable_chunked_read
-            else None,
+            buffer_size_limit_bytes=(
+                read_chunk_size_bytes if enable_chunked_read else None
+            ),
         )
         read_reqs.extend(rrs)
 
     # Read should work regardless of whether write was batched or not
     if enable_batched_read:
         batched_read_reqs = batch_read_requests(read_reqs=read_reqs)
         assert len(batched_read_reqs) < len(read_reqs)
```

### Comparing `torchsnapshot-nightly-2024.1.9/tests/test_chunked_tensor_io_preparer.py` & `torchsnapshot_nightly-2024.5.21/tests/test_chunked_tensor_io_preparer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
+
+# pyre-strict
 import asyncio
 import tempfile
 import unittest
 from typing import List, Tuple
 
 import torch
 import torchsnapshot
```

### Comparing `torchsnapshot-nightly-2024.1.9/tests/test_ddp.py` & `torchsnapshot_nightly-2024.5.21/tests/test_ddp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 from functools import reduce
 from operator import mul
 from pathlib import Path
 from typing import Generator, List
 
 import pytest
```

### Comparing `torchsnapshot-nightly-2024.1.9/tests/test_ddp_infer_replication.py` & `torchsnapshot_nightly-2024.5.21/tests/test_ddp_infer_replication.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 import unittest
 from typing import Dict, List
 
 import torch
 import torch.distributed as dist
 import torch.distributed.launcher as pet
 from torch.nn.parallel import DistributedDataParallel as DDP
```

### Comparing `torchsnapshot-nightly-2024.1.9/tests/test_ddp_replication_glob.py` & `torchsnapshot_nightly-2024.5.21/tests/test_ddp_replication_glob.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 from pathlib import Path
 from typing import List, Optional
 
 import pytest
 
 import torch
 import torch.distributed as dist
```

### Comparing `torchsnapshot-nightly-2024.1.9/tests/test_dist_store.py` & `torchsnapshot_nightly-2024.5.21/tests/test_dist_store.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 import unittest
 from datetime import timedelta
 
 import torch.distributed as dist
 
 import torch.distributed.launcher as pet
 from torchsnapshot.dist_store import create_store, get_or_create_store, LinearBarrier
```

### Comparing `torchsnapshot-nightly-2024.1.9/tests/test_flatten.py` & `torchsnapshot_nightly-2024.5.21/tests/test_flatten.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 # pyre-ignore-all-errors[2, 3]: allow `Any` in function signatures
 import os
 from collections import OrderedDict
 from typing import Any, Dict
 
 import pytest
 
@@ -172,17 +174,17 @@
     "x%2Fy/%25a%2Fb": 10,
 }
 
 
 def test_simple_flatten_with_prefix() -> None:
     manifest, flattened = flatten(obj=_OBJ, prefix="my/prefix")
     expected_manifest = {
-        os.path.join(_encode("my/prefix"), path)
-        if path
-        else _encode("my/prefix"): entry
+        (
+            os.path.join(_encode("my/prefix"), path) if path else _encode("my/prefix")
+        ): entry
         for path, entry in _EXPECTED_MANIFEST.items()
     }
     expected_flattened = {
         os.path.join(_encode("my/prefix"), path): entry
         for path, entry in _EXPECTED_FLATTENED.items()
     }
     assert manifest == expected_manifest
```

### Comparing `torchsnapshot-nightly-2024.1.9/tests/test_fs_storage_plugin.py` & `torchsnapshot_nightly-2024.5.21/tests/test_fs_storage_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 # pyre-ignore-all-errors[56]
 
 import io
 
 import logging
 import random
 from pathlib import Path
```

### Comparing `torchsnapshot-nightly-2024.1.9/tests/test_gcs_storage_plugin.py` & `torchsnapshot_nightly-2024.5.21/tests/test_gcs_storage_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 # pyre-ignore-all-errors[56]
 
 import io
 import logging
 import os
 import random
 import tempfile
```

### Comparing `torchsnapshot-nightly-2024.1.9/tests/test_manifest.py` & `torchsnapshot_nightly-2024.5.21/tests/test_manifest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 from dataclasses import asdict
 from typing import Dict, Generator
 from unittest.mock import patch
 
 import pytest
 
 import yaml
```

### Comparing `torchsnapshot-nightly-2024.1.9/tests/test_memoryview_stream.py` & `torchsnapshot_nightly-2024.5.21/tests/test_memoryview_stream.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 import io
 import unittest
 
 import torch
 from torchsnapshot.memoryview_stream import MemoryviewStream
```

### Comparing `torchsnapshot-nightly-2024.1.9/tests/test_partitioner.py` & `torchsnapshot_nightly-2024.5.21/tests/test_partitioner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 from collections import defaultdict
 from pathlib import Path
 from typing import List, Tuple
 
 import pytest
 import torch
 import torch.distributed as dist
```

### Comparing `torchsnapshot-nightly-2024.1.9/tests/test_pg_wrapper.py` & `torchsnapshot_nightly-2024.5.21/tests/test_pg_wrapper.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 # pyre-ignore-all-errors[56]
 
 import os
 import unittest
 
 import torch
```

### Comparing `torchsnapshot-nightly-2024.1.9/tests/test_read_object.py` & `torchsnapshot_nightly-2024.5.21/tests/test_read_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 import tempfile
 import unittest
 
 import torch
 import torch.distributed as dist
 import torch.distributed.launcher as pet
 import torchsnapshot
```

### Comparing `torchsnapshot-nightly-2024.1.9/tests/test_replication_glob.py` & `torchsnapshot_nightly-2024.5.21/tests/test_replication_glob.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 from pathlib import Path
 from typing import Any, Dict, List
 
 import pytest
 
 import torch
 import torch.distributed as dist
```

### Comparing `torchsnapshot-nightly-2024.1.9/tests/test_rng_state.py` & `torchsnapshot_nightly-2024.5.21/tests/test_rng_state.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 import tempfile
 import unittest
 from typing import Any, Dict
 
 import torch
 import torchsnapshot
```

### Comparing `torchsnapshot-nightly-2024.1.9/tests/test_rss_profiler.py` & `torchsnapshot_nightly-2024.5.21/tests/test_rss_profiler.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 import time
 import unittest
 
 import torch
 from torchsnapshot.rss_profiler import measure_rss_deltas
```

### Comparing `torchsnapshot-nightly-2024.1.9/tests/test_s3_storage_plugin.py` & `torchsnapshot_nightly-2024.5.21/tests/test_s3_storage_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 # pyre-ignore-all-errors[56]
 
 import io
 import logging
 import os
 import random
 import uuid
```

### Comparing `torchsnapshot-nightly-2024.1.9/tests/test_serialization.py` & `torchsnapshot_nightly-2024.5.21/tests/test_serialization.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 
 from typing import Tuple
 
 import pytest
 
 import torch
```

### Comparing `torchsnapshot-nightly-2024.1.9/tests/test_sharded_tensor_io_preparer.py` & `torchsnapshot_nightly-2024.5.21/tests/test_sharded_tensor_io_preparer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 import copy
 import unittest
 from typing import Generator, List, Set, Tuple
 
 import pytest
 
 import torch
```

### Comparing `torchsnapshot-nightly-2024.1.9/tests/test_sharded_tensor_resharding.py` & `torchsnapshot_nightly-2024.5.21/tests/test_sharded_tensor_resharding.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 # pyre-ignore-all-errors[21, 56]: ignore pytest undefine import and invalid decoration
 import itertools
 import uuid
 from typing import cast, Generator, List
 
 import pytest
 import torch
```

### Comparing `torchsnapshot-nightly-2024.1.9/tests/test_snapshot.py` & `torchsnapshot_nightly-2024.5.21/tests/test_snapshot.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 import copy
 from pathlib import Path
 from typing import Any, Dict, List
+from unittest.mock import MagicMock
 
 import pytest
 
 import torch
 from torchsnapshot import Snapshot, StateDict
 from torchsnapshot.manifest import PrimitiveEntry
 from torchsnapshot.test_utils import check_state_dict_eq
@@ -72,14 +75,35 @@
 
     snapshot = Snapshot.take(str(tmp_path), {"foo": foo})
     snapshot.restore({"foo": bar})
     assert check_state_dict_eq(foo.state_dict(), bar.state_dict())
 
 
 @pytest.mark.usefixtures("toggle_batching")
+def test_strict_false(tmp_path: Path) -> None:
+    foo = torch.nn.Sequential(
+        torch.nn.Linear(128, 64),
+        torch.nn.Linear(64, 32),
+        torch.nn.Linear(32, 16),
+    )
+    bar = torch.nn.Sequential(
+        torch.nn.Linear(128, 64),
+        torch.nn.Linear(64, 32),
+        torch.nn.Linear(32, 16),
+        torch.nn.Linear(16, 8),
+    )
+    assert not check_state_dict_eq(foo.state_dict(), bar.state_dict())
+
+    expected_dict = foo.state_dict()
+    snapshot = Snapshot.take(str(tmp_path), {"foo": foo})
+    snapshot.restore({"foo": bar}, strict=False)
+    assert check_state_dict_eq(foo.state_dict(), expected_dict)
+
+
+@pytest.mark.usefixtures("toggle_batching")
 def test_adagrad(tmp_path: Path) -> None:
     model = torch.nn.Sequential(
         torch.nn.Linear(128, 64),
         torch.nn.Linear(64, 32),
         torch.nn.Linear(32, 16),
     )
     optim = torch.optim.Adagrad(model.parameters(), lr=0.01)
@@ -199,7 +223,25 @@
         src.objs.append(torch.rand(64, 64))
     src.objs.append([torch.rand(64, 64) for _ in range(10)])
 
     assert not check_state_dict_eq(src.state_dict(), dst.state_dict())
     snapshot = Snapshot.take(app_state={"state": src}, path=str(tmp_path))
     snapshot.restore(app_state={"state": dst})
     assert check_state_dict_eq(src.state_dict(), dst.state_dict())
+
+
+@pytest.mark.usefixtures("toggle_batching")
+def test_snapshot_metadata_error(tmp_path: Path) -> None:
+    mock_storage_plugin = MagicMock()
+    mock_event_loop = MagicMock()
+    mock_storage_plugin.sync_read.side_effect = Exception(
+        "Mock error reading from storage"
+    )
+    with pytest.raises(
+        expected_exception=RuntimeError,
+        match=(
+            "Failed to read .snapshot_metadata. "
+            "Ensure path to snapshot is correct, "
+            "otherwise snapshot is likely incomplete or corrupted."
+        ),
+    ):
+        Snapshot._read_snapshot_metadata(mock_storage_plugin, mock_event_loop)
```

### Comparing `torchsnapshot-nightly-2024.1.9/tests/test_tensor_io_preparer.py` & `torchsnapshot_nightly-2024.5.21/tests/test_tensor_io_preparer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
+
+# pyre-strict
 import asyncio
 import functools
 import itertools
 import tempfile
 
 import unittest
 from typing import Callable, cast, List
```

### Comparing `torchsnapshot-nightly-2024.1.9/tests/test_test_utils.py` & `torchsnapshot_nightly-2024.5.21/tests/test_test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 import unittest
 
 import torch
 import torch.distributed as dist
 import torch.distributed.launcher as pet
 from torch.distributed._shard.metadata import ShardMetadata
 from torch.distributed._shard.sharded_tensor import (
@@ -117,14 +119,15 @@
     @staticmethod
     def _create_dtensor() -> DTensor:
         dim_0: int = 128
         dim_1: int = 16
 
         local_tensor = torch.rand((dim_0, dim_1))
 
+        # pyre-fixme[6]: For 2nd argument expected `Union[_SupportsArray[typing.Any],...
         mesh = DeviceMesh("cpu", mesh=[[0, 1], [2, 3]])
         placements = [Replicate(), Shard(0)]
         dtensor = distribute_tensor(
             tensor=local_tensor, device_mesh=mesh, placements=placements
         )
 
         return dtensor
```

### Comparing `torchsnapshot-nightly-2024.1.9/tests/test_uvm_tensor.py` & `torchsnapshot_nightly-2024.5.21/tests/test_uvm_tensor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 # pyre-ignore-all-errors[56]
 
 import pytest
 import torch
 from torchsnapshot.uvm_tensor import (
     _UVM_TENSOR_AVAILABLE,
     is_uvm_tensor,
```

### Comparing `torchsnapshot-nightly-2024.1.9/torchsnapshot/__init__.py` & `torchsnapshot_nightly-2024.5.21/torchsnapshot/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 "A lightweight library for adding fault tolerance to large-scale PyTorch distributed training workloads"
 
 from .rng_state import RNGState
 from .snapshot import Snapshot
 from .state_dict import StateDict
 from .stateful import Stateful
 from .version import __version__
```

### Comparing `torchsnapshot-nightly-2024.1.9/torchsnapshot/batcher.py` & `torchsnapshot_nightly-2024.5.21/torchsnapshot/batcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 import asyncio
 import os
 import uuid
 from collections import defaultdict
 from concurrent.futures import Executor
 from enum import Enum
 from typing import cast, Dict, Iterator, List, Optional, Tuple
@@ -131,17 +133,17 @@
                     "GPUBatchedBufferStager only supports batchable entries "
                     f"(got {buffer_stager.entry})."
                 )
             if not buffer_stager.tensor.is_cuda:
                 raise AssertionError(
                     "GPUBatchedBufferStager only supports GPU tensors."
                 )
-        self.byte_range_to_buffer_stager: Dict[
-            Tuple[int, int], TensorBufferStager
-        ] = cast(Dict[Tuple[int, int], TensorBufferStager], byte_range_to_buffer_stager)
+        self.byte_range_to_buffer_stager: Dict[Tuple[int, int], TensorBufferStager] = (
+            cast(Dict[Tuple[int, int], TensorBufferStager], byte_range_to_buffer_stager)
+        )
 
     async def stage_buffer(self, executor: Optional[Executor] = None) -> BufferType:
         try:
             # pyre-fixme[16]: Module `cuda` has no attribute `ByteTensor`.
             gpu_buf = torch.cuda.ByteTensor(self.slab_sz_bytes)
         except torch.cuda.OutOfMemoryError:
             gpu_buf = None
```

### Comparing `torchsnapshot-nightly-2024.1.9/torchsnapshot/dist_store.py` & `torchsnapshot_nightly-2024.5.21/torchsnapshot/dist_store.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 from datetime import timedelta
 from typing import Dict, Optional
 
 import torch.distributed as dist
 from torch.distributed.elastic.utils.distributed import get_socket_with_port
 
 from .pg_wrapper import PGWrapper
```

### Comparing `torchsnapshot-nightly-2024.1.9/torchsnapshot/dtensor_utils.py` & `torchsnapshot_nightly-2024.5.21/torchsnapshot/dtensor_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 from typing import Dict, Iterator, List, Set
 
 import torch
 from torch.distributed._shard.sharded_tensor import ShardedTensor
 from torch.distributed._tensor import DTensor, Replicate, Shard
```

### Comparing `torchsnapshot-nightly-2024.1.9/torchsnapshot/event.py` & `torchsnapshot_nightly-2024.5.21/torchsnapshot/event.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 from dataclasses import dataclass, field
 from typing import Dict, Union
 
 EventMetadataValue = Union[str, int, float, bool, None]
 
 
 @dataclass
```

### Comparing `torchsnapshot-nightly-2024.1.9/torchsnapshot/event_handlers.py` & `torchsnapshot_nightly-2024.5.21/torchsnapshot/event_handlers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 #!/usr/bin/env python3
 
+# pyre-strict
+
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
 import logging
@@ -16,16 +18,15 @@
 from .event import Event
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 @runtime_checkable
 class EventHandler(Protocol):
-    def handle_event(self, event: Event) -> None:
-        ...
+    def handle_event(self, event: Event) -> None: ...
 
 
 _log_handlers: List[EventHandler] = []
 
 
 @lru_cache(maxsize=None)
 def get_event_handlers() -> List[EventHandler]:
```

### Comparing `torchsnapshot-nightly-2024.1.9/torchsnapshot/flatten.py` & `torchsnapshot_nightly-2024.5.21/torchsnapshot/flatten.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 # pyre-ignore-all-errors[2, 3]: allow `Any` in function signatures
 
 import itertools
 from collections import defaultdict, OrderedDict
 from typing import Any, Dict, Tuple, Union
 from urllib.parse import unquote
```

### Comparing `torchsnapshot-nightly-2024.1.9/torchsnapshot/io_preparer.py` & `torchsnapshot_nightly-2024.5.21/torchsnapshot/io_preparer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 # pyre-ignore-all-errors[2, 3]: Allow `Any` in type annotations
 
 import logging
 import os
 from typing import Any, Callable, List, Optional, Tuple
 
 import torch
@@ -157,18 +159,14 @@
         entry: The entry describing the object.
         obj: The object to load.
 
     Returns:
         A list of class::`ReadReq` for loading the object.
     """
     if isinstance(entry, ShardedTensorEntry):
-        if obj_out is None:
-            raise RuntimeError(
-                "Reading a ShardedTensor without a runtime object is not supported."
-            )
         return ShardedTensorIOPreparer.prepare_read(entry, obj_out)
     elif isinstance(entry, ChunkedTensorEntry):
         return ChunkedTensorIOPreparer.prepare_read(
             entry, obj_out, buffer_size_limit_bytes=buffer_size_limit_bytes
         )
     elif isinstance(entry, DTensorEntry):
         return DTensorIOPreparer.prepare_read(entry, obj_out)
```

### Comparing `torchsnapshot-nightly-2024.1.9/torchsnapshot/io_preparers/chunked_tensor.py` & `torchsnapshot_nightly-2024.5.21/torchsnapshot/io_preparers/chunked_tensor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 import logging
 import math
 from dataclasses import dataclass
 from typing import Callable, List, Optional, Tuple, Union
 
 import torch
```

### Comparing `torchsnapshot-nightly-2024.1.9/torchsnapshot/io_preparers/dtensor.py` & `torchsnapshot_nightly-2024.5.21/torchsnapshot/io_preparers/dtensor.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 import itertools
 import logging
 from collections import defaultdict
 
 from typing import Callable, List, Optional, Sequence, Tuple
 
 import torch
@@ -24,15 +26,28 @@
 from torch.distributed._tensor import (
     DeviceMesh,
     DTensor,
     Placement,
     Replicate,
     Shard as ShardPlacement,
 )
-from torch.distributed._tensor._utils import compute_local_shape_and_global_offset
+
+try:
+    from torch.distributed._tensor._utils import compute_local_shape_and_global_offset
+
+except ImportError:
+
+    def compute_local_shape_and_global_offset(
+        global_shape: ShapeType, mesh: DeviceMesh, placements: Sequence[Placement]
+    ) -> Tuple[Tuple[int, ...], Tuple[int, ...]]:
+        raise RuntimeError(
+            "Please use the latest nightly pytorch release to use this feature."
+        )
+
+
 from torchsnapshot.io_preparers.sharded_tensor import (
     _OverlappingRegion,
     ShardedTensorBufferConsumer,
     ShardedTensorIOPreparer,
 )
 
 from torchsnapshot.io_preparers.tensor import TensorIOPreparer
```

### Comparing `torchsnapshot-nightly-2024.1.9/torchsnapshot/io_preparers/object.py` & `torchsnapshot_nightly-2024.5.21/torchsnapshot/io_preparers/object.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 # pyre-ignore-all-errors[2]: Allow `Any` in type annotations
 
 import io
 import logging
 import sys
 from concurrent.futures import Executor
 from typing import Any, Generic, List, Optional, Tuple, TypeVar
@@ -81,12 +83,13 @@
 class ObjectBufferConsumer(BufferConsumer, Generic[T]):
     def __init__(self, fut: Future[T]) -> None:
         self.fut = fut
 
     async def consume_buffer(
         self, buf: bytes, executor: Optional[Executor] = None
     ) -> None:
-        obj: T = torch.load(io.BytesIO(buf))
+        map_location = None if torch.cuda.is_available() else torch.device("cpu")
+        obj: T = torch.load(io.BytesIO(buf), map_location=map_location)
         self.fut.obj = obj
 
     def get_consuming_cost_bytes(self) -> int:
         return sys.getsizeof(self.fut.obj)
```

### Comparing `torchsnapshot-nightly-2024.1.9/torchsnapshot/io_preparers/sharded_tensor.py` & `torchsnapshot_nightly-2024.5.21/torchsnapshot/io_preparers/sharded_tensor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 import asyncio
 import copy
 import itertools
 import logging
 import math
 from collections import defaultdict
 from concurrent.futures import Executor
 from dataclasses import dataclass
 from functools import reduce
 from operator import mul
-from typing import Callable, List, Optional, Tuple
+from typing import Callable, List, Optional, Tuple, Union
 
 import torch
 from torch.distributed._shard.sharded_tensor import (
     Shard as ShardedTensorShard,
     ShardedTensor,
     ShardMetadata,
 )
@@ -33,15 +35,15 @@
     TensorBufferConsumer,
     TensorIOPreparer,
 )
 
 from torchsnapshot.io_types import BufferConsumer, Future, ReadReq, WriteReq
 from torchsnapshot.knobs import get_max_shard_size_bytes
 from torchsnapshot.manifest import Shard, ShardedTensorEntry, TensorEntry
-from torchsnapshot.serialization import Serializer
+from torchsnapshot.serialization import Serializer, string_to_dtype
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 class ShardedTensorIOPreparer:
     @staticmethod
     def subdivide_shard(
@@ -193,18 +195,19 @@
             )
 
     @classmethod
     def prepare_read(
         cls,
         entry: ShardedTensorEntry,
         obj_out: Optional[ShardedTensor] = None,
-    ) -> Tuple[List[ReadReq], Future[ShardedTensor]]:
+    ) -> Tuple[List[ReadReq], Future[Union[ShardedTensor, torch.Tensor]]]:
+        # Note: in case obj_out is None, a Future[Tensor] will be returned
         if obj_out is None:
-            raise RuntimeError(
-                "Reading a ShardedTensor without a runtime object is not supported."
+            obj_out = ShardedTensorIOPreparer.empty_tensor_from_sharded_tensor_entry(
+                entry
             )
 
         global_shape = cls._get_global_shape(entry=entry)
         cls._validate_shape(global_shape=global_shape, obj_out=obj_out)
 
         if type(obj_out) == ShardedTensor:
             local_shards = obj_out.local_shards()
@@ -263,14 +266,25 @@
                         entry=shard.tensor,
                     ),
                     byte_range=shard.tensor.byte_range_tuple,
                 )
             )
         return read_reqs, Future(obj=obj_out)
 
+    @staticmethod
+    def empty_tensor_from_sharded_tensor_entry(
+        entry: ShardedTensorEntry,
+    ) -> torch.Tensor:
+        # construct tensor for to fill in-place
+        # by reading shard metadata
+        shape = entry.get_tensor_shape()
+        dtype = entry.shards[0].tensor.dtype
+        tensor = torch.empty(shape, dtype=string_to_dtype(dtype))
+        return tensor
+
 
 @dataclass
 class _OverlappingRegion:
     dst_tensor: torch.Tensor
     overlap_region: List[
         Tuple[int, int, int, int]
     ]  # (dim, src_offset, dst_offset, length)
```

### Comparing `torchsnapshot-nightly-2024.1.9/torchsnapshot/io_preparers/tensor.py` & `torchsnapshot_nightly-2024.5.21/torchsnapshot/io_preparers/tensor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 # pyre-ignore-all-errors[2]: Allow `Any` in type annotations
 
 import asyncio
 import logging
 import math
 from concurrent.futures import Executor
 from functools import reduce
```

### Comparing `torchsnapshot-nightly-2024.1.9/torchsnapshot/io_types.py` & `torchsnapshot_nightly-2024.5.21/torchsnapshot/io_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 import abc
 import asyncio
 import io
 from concurrent.futures import Executor
 from dataclasses import dataclass, field
 from typing import Generic, Optional, Tuple, TypeVar, Union
```

### Comparing `torchsnapshot-nightly-2024.1.9/torchsnapshot/knobs.py` & `torchsnapshot_nightly-2024.5.21/torchsnapshot/knobs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 # pyre-ignore-all-errors[2]: Allow `Any` in type annotations
 import os
 from contextlib import contextmanager
 from typing import Any, Generator
 
 # This file contains various non-user facing constants used throughout the
 # project, and utilities for overriding the constants for testing and debugging
```

### Comparing `torchsnapshot-nightly-2024.1.9/torchsnapshot/manifest.py` & `torchsnapshot_nightly-2024.5.21/torchsnapshot/manifest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 # pyre-ignore-all-errors[2]: Allow `Any` in type annotations
 
 import base64
 import json
 import logging
 import struct
 from dataclasses import asdict, dataclass
```

### Comparing `torchsnapshot-nightly-2024.1.9/torchsnapshot/manifest_ops.py` & `torchsnapshot_nightly-2024.5.21/torchsnapshot/manifest_ops.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 
 import copy
 from collections import defaultdict
 from typing import Dict, List, Tuple
 
 from torchsnapshot.dtensor_utils import _ReplicatedShards
```

### Comparing `torchsnapshot-nightly-2024.1.9/torchsnapshot/manifest_utils.py` & `torchsnapshot_nightly-2024.5.21/torchsnapshot/manifest_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 import itertools
 from typing import List, Set
 
 import numpy as np
 
 from torchsnapshot.manifest import (
     DictEntry,
```

### Comparing `torchsnapshot-nightly-2024.1.9/torchsnapshot/memoryview_stream.py` & `torchsnapshot_nightly-2024.5.21/torchsnapshot/memoryview_stream.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 import io
 from typing import Optional
 
 
 # pyre-fixme[13]: Attribute `write` is never initialized.
 class MemoryviewStream(io.IOBase):
     def __init__(self, mv: memoryview) -> None:
```

### Comparing `torchsnapshot-nightly-2024.1.9/torchsnapshot/partitioner.py` & `torchsnapshot_nightly-2024.5.21/torchsnapshot/partitioner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 import copy
 import os
 from collections import defaultdict
 
 from dataclasses import dataclass
 from typing import cast, Dict, List, Tuple
 
@@ -333,15 +335,15 @@
         for logical_path in list(entries.keys()):
             entry = entries[logical_path]
             if not is_fully_replicated_entry(entry):
                 continue
             if logical_path in replicated_entries:
                 if replicated_entries[logical_path] != entry:
                     raise ValueError(
-                        f"Paths for replicated entry do not match: replicated entries={replicated_entries[logical_path]} vs. entry={entry}"
+                        f"Paths for replicated entry for {logical_path} do not match: replicated entries={replicated_entries[logical_path]} vs. entry={entry}"
                     )
             else:
                 replicated_entries[logical_path] = entry
             del entries[logical_path]
 
     # Add the replicated entries to the manifests
     for rank, entries in enumerate(rank_to_entries):
```

### Comparing `torchsnapshot-nightly-2024.1.9/torchsnapshot/pg_wrapper.py` & `torchsnapshot_nightly-2024.5.21/torchsnapshot/pg_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 # pyre-ignore-all-errors[2]
 
 from typing import Any, List, Optional
 
 import torch.distributed as dist
```

### Comparing `torchsnapshot-nightly-2024.1.9/torchsnapshot/rng_state.py` & `torchsnapshot_nightly-2024.5.21/torchsnapshot/rng_state.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 from typing import Dict
 
 import torch
 
 
 class RNGState:
     """
```

### Comparing `torchsnapshot-nightly-2024.1.9/torchsnapshot/rss_profiler.py` & `torchsnapshot_nightly-2024.5.21/torchsnapshot/rss_profiler.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 
 import time
 from contextlib import contextmanager
 from datetime import timedelta
 from threading import Event, Thread
 from typing import Generator, List
```

### Comparing `torchsnapshot-nightly-2024.1.9/torchsnapshot/scheduler.py` & `torchsnapshot_nightly-2024.5.21/torchsnapshot/scheduler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 #!/usr/bin/env python3
 
+# pyre-strict
+
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
 import asyncio
```

### Comparing `torchsnapshot-nightly-2024.1.9/torchsnapshot/serialization.py` & `torchsnapshot_nightly-2024.5.21/torchsnapshot/serialization.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 import functools
 import io
 import logging
 import operator
 import struct
 import warnings
 from enum import Enum
```

### Comparing `torchsnapshot-nightly-2024.1.9/torchsnapshot/snapshot.py` & `torchsnapshot_nightly-2024.5.21/torchsnapshot/snapshot.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 import asyncio
 
 import copy
 import fnmatch
 import functools
 import itertools
 import logging
 import os
 import random
 import sys
 import traceback
+from asyncio import AbstractEventLoop
 
 from collections import defaultdict
 from datetime import timedelta
 from threading import Thread
-from typing import Any, Callable, cast, Dict, List, Optional, Set, Tuple, TypeVar
+from typing import Any, Callable, cast, Dict, List, Optional, Set, Tuple, TypeVar, Union
 
 import torch
 import torch.distributed as dist
 from torch.distributed._shard.sharded_tensor import ShardedTensor
 from torch.distributed._tensor import DTensor
 from torch.nn.parallel import DistributedDataParallel as DDP
 from torchsnapshot.dtensor_utils import is_sharded
-from torchsnapshot.manifest import ShardedTensorEntry
-from torchsnapshot.serialization import string_to_dtype
 
 from .batcher import batch_read_requests, batch_write_requests
 
 from .dist_store import get_or_create_store, LinearBarrier
 
 from .event import Event
 from .event_handlers import log_event
@@ -168,16 +169,20 @@
         torch._C._log_api_usage_once("torchsnapshot.Snapshot.take")
         cls._validate_app_state(app_state)
 
         event_loop = asyncio.new_event_loop()
         pg_wrapper = PGWrapper(pg=pg)
 
         unique_id = _generate_random_int64()
+        rank = pg_wrapper.get_rank()
         log_event(
-            Event(name="take", metadata={"action": "start", "unique_id": unique_id})
+            Event(
+                name="take",
+                metadata={"action": "start", "unique_id": unique_id, "rank": rank},
+            )
         )
 
         path, coalesced_replicated = cls._coalesce_path_and_replicated(
             path=path,
             pg_wrapper=pg_wrapper,
             app_state=app_state,
             replicated=replicated or [],
@@ -210,15 +215,20 @@
         event_loop.close()
         snapshot = cls(path=path, pg=pg, storage_options=storage_options)
         snapshot._metadata = metadata
 
         log_event(
             Event(
                 name="take",
-                metadata={"action": "end", "unique_id": unique_id, "is_success": True},
+                metadata={
+                    "action": "end",
+                    "unique_id": unique_id,
+                    "is_success": True,
+                    "rank": rank,
+                },
             )
         )
         return snapshot
 
     @classmethod
     def async_take(
         cls,
@@ -253,17 +263,19 @@
         torch._C._log_api_usage_once("torchsnapshot.Snapshot.async_take")
         cls._validate_app_state(app_state)
 
         event_loop = asyncio.new_event_loop()
         pg_wrapper = PGWrapper(pg=pg)
 
         unique_id = _generate_random_int64()
+        rank = pg_wrapper.get_rank()
         log_event(
             Event(
-                name="async_take", metadata={"action": "start", "unique_id": unique_id}
+                name="async_take",
+                metadata={"action": "start", "unique_id": unique_id, "rank": rank},
             )
         )
 
         path, coalesced_replicated = cls._coalesce_path_and_replicated(
             path=path,
             pg_wrapper=pg_wrapper,
             app_state=app_state,
@@ -283,15 +295,19 @@
             is_async_snapshot=True,
             _custom_tensor_prepare_func=_custom_tensor_prepare_func,
         )
 
         log_event(
             Event(
                 name="async_take",
-                metadata={"action": "end_collection", "unique_id": unique_id},
+                metadata={
+                    "action": "end_collection",
+                    "unique_id": unique_id,
+                    "rank": rank,
+                },
             )
         )
 
         # PendingSnapshot is responsible for closing `storage` and `event_loop`
         return PendingSnapshot(
             path=path,
             pending_io_work=pending_io_work,
@@ -299,33 +315,41 @@
             metadata=metadata,
             storage=storage,
             event_loop=event_loop,
             storage_options=storage_options,
             unique_id=unique_id,
         )
 
-    def restore(self, app_state: AppState) -> None:
+    def restore(self, app_state: AppState, strict: bool = True) -> None:
         """
         Restores the application state from the snapshot.
 
         Args:
             app_state (Dict[str, Stateful]): The application state to restore.
                 ``app_state`` needs to be either identical to or a subset of the
                 ``app_state`` used for :func:`Snapshot.take` when the snapshot was
                 taken.
+            strict (bool, optional): If ``True``, raises an error if the expected
+                state_dict keys in the snapshot do not match the actual keys in
+                the :class:`torch.nn.Module`. This only applies to :class:`torch.nn.Module`
+                and not other objects being restored in ``app_state``.
         """
         torch._C._log_api_usage_once("torchsnapshot.Snapshot.restore")
         self._validate_app_state(app_state)
 
         event_loop = asyncio.new_event_loop()
         pg_wrapper = PGWrapper(self.pg)
 
         unique_id = _generate_random_int64()
+        rank = pg_wrapper.get_rank()
         log_event(
-            Event(name="restore", metadata={"action": "start", "unique_id": unique_id})
+            Event(
+                name="restore",
+                metadata={"action": "start", "unique_id": unique_id, "rank": rank},
+            )
         )
 
         storage = url_to_storage_plugin_in_event_loop(
             url_path=self.path,
             event_loop=event_loop,
             storage_options=self._storage_options,
         )
@@ -336,37 +360,44 @@
         global_keys = self._gather_keys(
             keys=list(app_state.keys()), pg_wrapper=pg_wrapper
         )
         for key in global_keys:
             self._load_stateful(
                 stateful_key=key,
                 stateful=app_state.get(key),
+                strict=strict,
                 storage=storage,
                 pg=pg_wrapper,
                 event_loop=event_loop,
             )
             pg_wrapper.barrier()
 
         # Restore the RNG state last to avoid potential side effects.
         if rng_state_item is not None:
             key, stateful = rng_state_item
             self._load_stateful(
                 stateful_key=key,
                 stateful=stateful,
+                strict=strict,
                 storage=storage,
                 pg=pg_wrapper,
                 event_loop=event_loop,
             )
         storage.sync_close(event_loop=event_loop)
         event_loop.close()
 
         log_event(
             Event(
                 name="restore",
-                metadata={"action": "end", "unique_id": unique_id, "is_success": True},
+                metadata={
+                    "action": "end",
+                    "unique_id": unique_id,
+                    "is_success": True,
+                    "rank": rank,
+                },
             )
         )
 
     def read_object(
         self,
         path: str,
         obj_out: Optional[T] = None,
@@ -434,21 +465,14 @@
             url_path=self.path,
             event_loop=event_loop,
             storage_options=self._storage_options,
         )
         entry = merged_sd_entries.get(unranked_path) or manifest[unranked_path]
         if isinstance(entry, PrimitiveEntry):
             return cast(T, entry.get_value())
-        elif obj_out is None and isinstance(entry, ShardedTensorEntry):
-            # construct tensor for `obj_out` to fill in-place
-            # by reading shard metadata
-            shape = entry.get_tensor_shape()
-            dtype = entry.shards[0].tensor.dtype
-            tensor = torch.empty(shape, dtype=string_to_dtype(dtype))
-            obj_out = tensor
 
         read_reqs, fut = prepare_read(
             entry=entry,
             obj_out=obj_out,
             # TODO: find a suitable buffer_size_limit_bytes to enable chunked
             # read even when memory_budget_bytes is not specified, as chunked
             # tensor read allows for pipelining HtoD copy and storage I/O when
@@ -563,19 +587,19 @@
         for logical_path, obj in flattened.items():
             entry, wrs = prepare_write(
                 obj=obj,
                 logical_path=logical_path,
                 rank=pg_wrapper.get_rank(),
                 replicated=logical_path in replicated_paths,
                 is_async_snapshot=is_async_snapshot,
-                _tensor_prepare_func=functools.partial(
-                    _custom_tensor_prepare_func, logical_path
-                )
-                if _custom_tensor_prepare_func is not None
-                else None,
+                _tensor_prepare_func=(
+                    functools.partial(_custom_tensor_prepare_func, logical_path)
+                    if _custom_tensor_prepare_func is not None
+                    else None
+                ),
             )
             # Primitive entries don't have write requests
             # and don't need to be partitioned
             if isinstance(entry, PrimitiveEntry):
                 primitive_entries[logical_path] = entry
             else:
                 object_entries[logical_path] = entry
@@ -654,18 +678,58 @@
         for key, value in app_state.items():
             if not isinstance(value, Stateful):
                 value_type = type(value)
                 raise TypeError(
                     f"Expected Stateful in app_state for key {key}, got {value_type}."
                 )
 
+    # pyre-fixme: inflate returns Dict[Any,Any]
+    # Missing return annotation [3]: Return type must be specified as type that does not contain `Any`
+    def get_state_dict_for_key(self, key: str) -> Dict[Any, Any]:
+        """
+        Gets the state dict for a selected key in the snapshot.
+        This is useful in case you want to get the state dict without loading it to the stateful.
+
+        Args:
+            key (str): The key to get the state dict for. Assumes the key was stored as a topline
+                key in the snapshot.
+
+        Returns:
+            The state dict associated with the key.
+
+        Below is a usage example
+
+        .. code-block:: python
+
+            snapshot = Snapshot.take(path=..., app_state={"stateful_key": module})
+            module_state_dict = snapshot.get_state_dict_for_key("stateful_key")
+        """
+        event_loop = asyncio.new_event_loop()
+        pg = PGWrapper(self.pg)
+
+        manifest, _ = get_manifest_for_rank(metadata=self.metadata, rank=pg.get_rank())
+
+        # filter out irrelevant entries from the manifest
+        manifest = {k: v for k, v in manifest.items() if k.split("/")[0] == key}
+
+        storage = url_to_storage_plugin_in_event_loop(
+            url_path=self.path,
+            event_loop=event_loop,
+            storage_options=self._storage_options,
+        )
+
+        return self._get_state_dict_for_manifest(
+            key, manifest, {}, pg, storage, event_loop
+        )
+
     def _load_stateful(  # noqa
         self,
         stateful_key: str,
         stateful: Optional[Stateful],
+        strict: bool,
         storage: StoragePlugin,
         pg: PGWrapper,
         event_loop: asyncio.AbstractEventLoop,
     ) -> None:
         if stateful is None:
             return
 
@@ -696,14 +760,35 @@
 
         handle_sharded_tensor_elasticity(
             manifest=manifest,
             merged_sd_entries=merged_sd_entries,
             tensor_requests=list(flattened.keys()),
         )
 
+        # Build the originally saved state dict and use it to restore the stateful
+        state_dict = self._get_state_dict_for_manifest(
+            stateful_key, manifest, flattened, pg, storage, event_loop
+        )
+
+        if isinstance(stateful, torch.nn.Module):
+            stateful.load_state_dict(state_dict, strict=strict)
+        else:
+            stateful.load_state_dict(state_dict)
+
+    @staticmethod
+    # pyre-fixme: inflate returns Dict[Any,Any]
+    # Missing return annotation [3]: Return type must be specified as type that does not contain `Any`
+    def _get_state_dict_for_manifest(
+        stateful_key: str,
+        manifest: Manifest,
+        flattened: Dict[str, Union[torch.Tensor, ShardedTensor, DTensor]],
+        pg: PGWrapper,
+        storage: StoragePlugin,
+        event_loop: AbstractEventLoop,
+    ) -> Dict[Any, Any]:
         container_entries = {}
         read_reqs: List[ReadReq] = []
         futs = {}
         for logical_path, entry in manifest.items():
             if is_container_entry(entry):
                 container_entries[logical_path] = entry
                 continue
@@ -728,20 +813,19 @@
             storage=storage,
             memory_budget_bytes=memory_budget_bytes,
             rank=pg.get_rank(),
             event_loop=event_loop,
         )
 
         # Build the originally saved state dict and use it to restore the stateful
-        state_dict = inflate(
+        return inflate(
             manifest=container_entries,
             flattened={k: fut.obj for k, fut in futs.items()},
             prefix=stateful_key,
         )
-        stateful.load_state_dict(state_dict)
 
     @staticmethod
     def _write_snapshot_metadata(
         snapshot_metadata: SnapshotMetadata,
         storage: StoragePlugin,
         event_loop: asyncio.AbstractEventLoop,
     ) -> None:
@@ -752,15 +836,22 @@
         storage.sync_write(write_io=write_io, event_loop=event_loop)
 
     @staticmethod
     def _read_snapshot_metadata(
         storage: StoragePlugin, event_loop: asyncio.AbstractEventLoop
     ) -> SnapshotMetadata:
         read_io = ReadIO(path=SNAPSHOT_METADATA_FNAME)
-        storage.sync_read(read_io=read_io, event_loop=event_loop)
+        try:
+            storage.sync_read(read_io=read_io, event_loop=event_loop)
+        except Exception as e:
+            raise RuntimeError(
+                f"Failed to read {SNAPSHOT_METADATA_FNAME}. "
+                "Ensure path to snapshot is correct, "
+                "otherwise snapshot is likely incomplete or corrupted."
+            ) from e
         yaml_str = read_io.buf.getvalue().decode("utf-8")
         return SnapshotMetadata.from_yaml(yaml_str)
 
     @classmethod
     def _coalesce_path_and_replicated(
         cls,
         path: str,
@@ -871,15 +962,15 @@
         self,
         path: str,
         pending_io_work: PendingIOWork,
         pg_wrapper: PGWrapper,
         metadata: SnapshotMetadata,
         storage: StoragePlugin,
         event_loop: asyncio.AbstractEventLoop,
-        unique_id: int,
+        unique_id: Optional[int],
         storage_options: Optional[Dict[str, Any]] = None,
     ) -> None:
         self.path = path
         self.pg: Optional[dist.ProcessGroup] = pg_wrapper.pg
         # pyre-ignore
         self.exc_info: Optional[Any] = None
         self._done = False
@@ -949,14 +1040,15 @@
         log_event(
             Event(
                 name="async_take",
                 metadata={
                     "action": "end",
                     "unique_id": self._unique_id,
                     "is_success": succeeded,
+                    "rank": rank,
                 },
             )
         )
 
     def wait(self) -> Snapshot:
         self.thread.join()
         if self.exc_info is not None:
```

### Comparing `torchsnapshot-nightly-2024.1.9/torchsnapshot/state_dict.py` & `torchsnapshot_nightly-2024.5.21/torchsnapshot/state_dict.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 from collections import UserDict
 from typing import Any, Dict
 
 
 # pyre-fixme[24]: Python <3.9 doesn't support typing on UserDict
 class StateDict(UserDict):
     """
```

### Comparing `torchsnapshot-nightly-2024.1.9/torchsnapshot/stateful.py` & `torchsnapshot_nightly-2024.5.21/torchsnapshot/stateful.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 from typing import Any, Dict, TypeVar
 
 from typing_extensions import Protocol, runtime_checkable
 
 
 @runtime_checkable
 class Stateful(Protocol):
-    def state_dict(self) -> Dict[str, Any]:
-        ...
+    def state_dict(self) -> Dict[str, Any]: ...
 
-    def load_state_dict(self, state_dict: Dict[str, Any]) -> None:
-        ...
+    def load_state_dict(self, state_dict: Dict[str, Any]) -> None: ...
 
 
 T = TypeVar("T", bound=Stateful)
 AppState = Dict[str, T]
```

### Comparing `torchsnapshot-nightly-2024.1.9/torchsnapshot/storage_plugin.py` & `torchsnapshot_nightly-2024.5.21/torchsnapshot/storage_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 import asyncio
 from typing import Any, Dict, Optional
 
 from importlib_metadata import entry_points
 
 from .io_types import StoragePlugin
 from .storage_plugins.fs import FSStoragePlugin
```

### Comparing `torchsnapshot-nightly-2024.1.9/torchsnapshot/storage_plugins/fs.py` & `torchsnapshot_nightly-2024.5.21/torchsnapshot/storage_plugins/fs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 import io
 import os
 import pathlib
 from typing import Any, Dict, Optional, Set
 
 import aiofiles
 import aiofiles.os
```

### Comparing `torchsnapshot-nightly-2024.1.9/torchsnapshot/storage_plugins/gcs.py` & `torchsnapshot_nightly-2024.5.21/torchsnapshot/storage_plugins/gcs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 # pyre-ignore-all-errors[2]: Allow `Any` in type annotations
 # pyre-ignore-all-errors[21]: Undefined import
 
 import asyncio
 import functools
 import io
 import logging
```

### Comparing `torchsnapshot-nightly-2024.1.9/torchsnapshot/storage_plugins/s3.py` & `torchsnapshot_nightly-2024.5.21/torchsnapshot/storage_plugins/s3.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 import io
 import os
 from typing import Any, Dict, Optional
 
 from torchsnapshot.io_types import ReadIO, StoragePlugin, WriteIO
 from torchsnapshot.memoryview_stream import MemoryviewStream
```

### Comparing `torchsnapshot-nightly-2024.1.9/torchsnapshot/test_utils.py` & `torchsnapshot_nightly-2024.5.21/torchsnapshot/test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 # pyre-ignore-all-errors[2]: Allow `Any` in type annotations
 
 import asyncio
 import functools
 import unittest
 import uuid
 from contextlib import contextmanager
@@ -311,14 +313,18 @@
     dtype: torch.dtype,
     shape: List[int],
     logical_path: str,
     rank: int,
     replicated: bool,
 ) -> Tuple[DTensor, Entry, List[WriteReq]]:
     # WORLD_SIZE needs to be at least 4
+    # pyre-fixme[6]: For 2nd argument expected `Union[_SupportsArray[typing.Any],
+    #  _NestedSequence[Union[bool, bytes, complex, float, int, str]],
+    #  _NestedSequence[_SupportsArray[typing.Any]], bool, bytes, complex, float, int,
+    #  str, Tensor]` but got `List[List[int]]`.
     mesh = DeviceMesh("cuda", mesh=[[0, 1], [2, 3]])
     placements = [Replicate(), Shard(0)]
     local_tensor = rand_tensor(shape, dtype=dtype)
     dtensor = distribute_tensor(
         tensor=local_tensor, device_mesh=mesh, placements=placements
     )
```

### Comparing `torchsnapshot-nightly-2024.1.9/torchsnapshot/tricks/ddp.py` & `torchsnapshot_nightly-2024.5.21/torchsnapshot/tricks/ddp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 from typing import Any, Dict
 
 import torch
 
 DDP_STATE_DICT_PREFIX: str = "module."
```

### Comparing `torchsnapshot-nightly-2024.1.9/torchsnapshot/tricks/deepspeed.py` & `torchsnapshot_nightly-2024.5.21/torchsnapshot/tricks/deepspeed.py`

 * *Files identical despite different names*

### Comparing `torchsnapshot-nightly-2024.1.9/torchsnapshot/tricks/fsdp.py` & `torchsnapshot_nightly-2024.5.21/torchsnapshot/tricks/fsdp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 from typing import Any, Dict
 
 import torch
 from torch.distributed.fsdp import FullyShardedDataParallel as FSDP
 
 
 class FSDPOptimizerAdapter:
```

### Comparing `torchsnapshot-nightly-2024.1.9/torchsnapshot/uvm_tensor.py` & `torchsnapshot_nightly-2024.5.21/torchsnapshot/uvm_tensor.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
+
+# pyre-strict
 from typing import List
 
 import torch
 
 _UVM_TENSOR_AVAILABLE = False
 
 try:
```

### Comparing `torchsnapshot-nightly-2024.1.9/torchsnapshot/version.py` & `torchsnapshot_nightly-2024.5.21/torchsnapshot/version.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-strict
+
 # Follows PEP-0440 version scheme guidelines
 # https://www.python.org/dev/peps/pep-0440/#version-scheme
 #
 # Examples:
 # 0.1.0.devN # Developmental release
 # 0.1.0aN  # Alpha release
 # 0.1.0bN  # Beta release
```

### Comparing `torchsnapshot-nightly-2024.1.9/torchsnapshot_nightly.egg-info/PKG-INFO` & `torchsnapshot_nightly-2024.5.21/torchsnapshot_nightly.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchsnapshot-nightly
-Version: 2024.1.9
+Version: 2024.5.21
 Summary: A performant, memory-efficient checkpointing library for PyTorch applications, designed with large, complex distributed workloads in mind.
 Home-page: https://github.com/pytorch/torchsnapshot
 Author: torchsnapshot team
 Author-email: yifu@fb.com
 License: BSD-3
 Keywords: pytorch,snapshot,checkpoint
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -30,15 +30,15 @@
 Requires-Dist: aiobotocore; extra == "dev"
 Requires-Dist: boto3; extra == "dev"
 Requires-Dist: expecttest; extra == "dev"
 Requires-Dist: google-cloud-storage; extra == "dev"
 Requires-Dist: google-resumable-media; extra == "dev"
 Requires-Dist: numpy; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
-Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest==8.1.1; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pytest-timeout; extra == "dev"
 
 # TorchSnapshot (Beta Release)
 
 <p align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: torchsnapshot-nightly Version: 2024.1.9 Summary: A
+Metadata-Version: 2.1 Name: torchsnapshot-nightly Version: 2024.5.21 Summary: A
 performant, memory-efficient checkpointing library for PyTorch applications,
 designed with large, complex distributed workloads in mind. Home-page: https://
 github.com/pytorch/torchsnapshot Author: torchsnapshot team Author-email:
 yifu@fb.com License: BSD-3 Keywords: pytorch,snapshot,checkpoint Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: BSD License Classifier: Programming Language :: Python :: 3
@@ -12,17 +12,17 @@
 PyYAML Requires-Dist: aiofiles Requires-Dist: aiohttp Requires-Dist: importlib-
 metadata Requires-Dist: nest_asyncio Requires-Dist: psutil Requires-Dist:
 pyre_extensions Requires-Dist: torch Requires-Dist: typing-extensions Provides-
 Extra: dev Requires-Dist: aiobotocore; extra == "dev" Requires-Dist: boto3;
 extra == "dev" Requires-Dist: expecttest; extra == "dev" Requires-Dist: google-
 cloud-storage; extra == "dev" Requires-Dist: google-resumable-media; extra ==
 "dev" Requires-Dist: numpy; extra == "dev" Requires-Dist: pre-commit; extra ==
-"dev" Requires-Dist: pytest; extra == "dev" Requires-Dist: pytest-asyncio;
-extra == "dev" Requires-Dist: pytest-cov; extra == "dev" Requires-Dist: pytest-
-timeout; extra == "dev" # TorchSnapshot (Beta Release)
+"dev" Requires-Dist: pytest==8.1.1; extra == "dev" Requires-Dist: pytest-
+asyncio; extra == "dev" Requires-Dist: pytest-cov; extra == "dev" Requires-
+Dist: pytest-timeout; extra == "dev" # TorchSnapshot (Beta Release)
 _[_b_u_i_l_d_ _s_t_a_t_u_s_]_[_p_y_p_i_ _v_e_r_s_i_o_n_]_[_c_o_n_d_a_ _v_e_r_s_i_o_n_]_[_p_y_p_i_ _n_i_g_h_t_l_y_ _v_e_r_s_i_o_n_]_[_c_o_d_e_c_o_v_]_[_b_s_d
                                    _l_i_c_e_n_s_e_]
 A performant, memory-efficient checkpointing library for PyTorch applications,
 designed with large, complex distributed workloads in mind. ## Install Requires
 Python >= 3.8 and PyTorch >= 2.0.0 From pip: ```bash # Stable pip install
 torchsnapshot # Or, using conda conda install -c conda-forge torchsnapshot #
 Nightly pip install --pre torchsnapshot-nightly ``` From source: ```bash git
```

### Comparing `torchsnapshot-nightly-2024.1.9/torchsnapshot_nightly.egg-info/SOURCES.txt` & `torchsnapshot_nightly-2024.5.21/torchsnapshot_nightly.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 tests/test_rng_state.py
 tests/test_rss_profiler.py
 tests/test_s3_storage_plugin.py
 tests/test_serialization.py
 tests/test_sharded_tensor_io_preparer.py
 tests/test_sharded_tensor_resharding.py
 tests/test_snapshot.py
+tests/test_state_dict.py
 tests/test_tensor_io_preparer.py
 tests/test_test_utils.py
 tests/test_uvm_tensor.py
 torchsnapshot/__init__.py
 torchsnapshot/batcher.py
 torchsnapshot/dist_store.py
 torchsnapshot/dtensor_utils.py
```

