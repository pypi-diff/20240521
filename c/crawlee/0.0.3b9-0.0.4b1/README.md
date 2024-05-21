# Comparing `tmp/crawlee-0.0.3b9.tar.gz` & `tmp/crawlee-0.0.4b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crawlee-0.0.3b9.tar", max compression
+gzip compressed data, was "crawlee-0.0.4b1.tar", max compression
```

## Comparing `crawlee-0.0.3b9.tar` & `crawlee-0.0.4b1.tar`

### file list

```diff
@@ -1,88 +1,93 @@
--rw-r--r--   0        0        0    11355 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/LICENSE
--rw-r--r--   0        0        0       17 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/README.md
--rw-r--r--   0        0        0     6385 2024-05-09 08:13:08.325150 crawlee-0.0.3b9/pyproject.toml
--rw-r--r--   0        0        0       31 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/__init__.py
--rw-r--r--   0        0        0        0 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/_utils/__init__.py
--rw-r--r--   0        0        0      774 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/_utils/blocked.py
--rw-r--r--   0        0        0     3341 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/_utils/byte_size.py
--rw-r--r--   0        0        0      759 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/_utils/crypto.py
--rw-r--r--   0        0        0     3365 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/_utils/data_processing.py
--rw-r--r--   0        0        0     1950 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/_utils/env_vars.py
--rw-r--r--   0        0        0     4668 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/_utils/file.py
--rw-r--r--   0        0        0     5262 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/_utils/globs.py
--rw-r--r--   0        0        0     2056 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/_utils/lru_cache.py
--rw-r--r--   0        0        0      918 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/_utils/math.py
--rw-r--r--   0        0        0      715 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/_utils/measure_time.py
--rw-r--r--   0        0        0     1585 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/_utils/recurring_task.py
--rw-r--r--   0        0        0     4765 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/_utils/requests.py
--rw-r--r--   0        0        0     2414 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/_utils/system.py
--rw-r--r--   0        0        0     1429 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/_utils/wait.py
--rw-r--r--   0        0        0      142 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/autoscaling/__init__.py
--rw-r--r--   0        0        0    14883 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/autoscaling/autoscaled_pool.py
--rw-r--r--   0        0        0        0 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/autoscaling/py.typed
--rw-r--r--   0        0        0    15793 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/autoscaling/snapshotter.py
--rw-r--r--   0        0        0     9293 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/autoscaling/system_status.py
--rw-r--r--   0        0        0     5140 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/autoscaling/types.py
--rw-r--r--   0        0        0      470 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/base_storage_client/__init__.py
--rw-r--r--   0        0        0     9224 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/base_storage_client/base_dataset_client.py
--rw-r--r--   0        0        0     1904 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/base_storage_client/base_dataset_collection_client.py
--rw-r--r--   0        0        0     3495 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/base_storage_client/base_key_value_store_client.py
--rw-r--r--   0        0        0     2046 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/base_storage_client/base_key_value_store_collection_client.py
--rw-r--r--   0        0        0     5662 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/base_storage_client/base_request_queue_client.py
--rw-r--r--   0        0        0     2013 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/base_storage_client/base_request_queue_collection_client.py
--rw-r--r--   0        0        0     1823 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/base_storage_client/base_storage_client.py
--rw-r--r--   0        0        0        0 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/base_storage_client/py.typed
--rw-r--r--   0        0        0      735 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/base_storage_client/types.py
--rw-r--r--   0        0        0      186 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/basic_crawler/__init__.py
--rw-r--r--   0        0        0    25030 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/basic_crawler/basic_crawler.py
--rw-r--r--   0        0        0     4696 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/basic_crawler/context_pipeline.py
--rw-r--r--   0        0        0     2145 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/basic_crawler/errors.py
--rw-r--r--   0        0        0     2279 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/basic_crawler/router.py
--rw-r--r--   0        0        0     2798 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/basic_crawler/types.py
--rw-r--r--   0        0        0       86 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/beautifulsoup_crawler/__init__.py
--rw-r--r--   0        0        0     5392 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/beautifulsoup_crawler/beautifulsoup_crawler.py
--rw-r--r--   0        0        0      524 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/beautifulsoup_crawler/types.py
--rw-r--r--   0        0        0     1246 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/configuration.py
--rw-r--r--   0        0        0      272 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/enqueue_strategy.py
--rw-r--r--   0        0        0       91 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/events/__init__.py
--rw-r--r--   0        0        0     7211 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/events/event_manager.py
--rw-r--r--   0        0        0     2682 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/events/local_event_manager.py
--rw-r--r--   0        0        0        0 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/events/py.typed
--rw-r--r--   0        0        0     1303 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/events/types.py
--rw-r--r--   0        0        0        0 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/http_clients/__init__.py
--rw-r--r--   0        0        0     1857 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/http_clients/base_http_client.py
--rw-r--r--   0        0        0     4283 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/http_clients/httpx_client.py
--rw-r--r--   0        0        0       38 2024-05-09 08:12:46.929110 crawlee-0.0.3b9/src/crawlee/http_crawler/__init__.py
--rw-r--r--   0        0        0     2834 2024-05-09 08:12:46.929110 crawlee-0.0.3b9/src/crawlee/http_crawler/http_crawler.py
--rw-r--r--   0        0        0      329 2024-05-09 08:12:46.929110 crawlee-0.0.3b9/src/crawlee/http_crawler/types.py
--rw-r--r--   0        0        0     4719 2024-05-09 08:12:46.929110 crawlee-0.0.3b9/src/crawlee/log_config.py
--rw-r--r--   0        0        0       55 2024-05-09 08:12:46.929110 crawlee-0.0.3b9/src/crawlee/memory_storage_client/__init__.py
--rw-r--r--   0        0        0     5471 2024-05-09 08:12:46.929110 crawlee-0.0.3b9/src/crawlee/memory_storage_client/base_resource_client.py
--rw-r--r--   0        0        0     2769 2024-05-09 08:12:46.929110 crawlee-0.0.3b9/src/crawlee/memory_storage_client/base_resource_collection_client.py
--rw-r--r--   0        0        0    17305 2024-05-09 08:12:46.929110 crawlee-0.0.3b9/src/crawlee/memory_storage_client/dataset_client.py
--rw-r--r--   0        0        0     1450 2024-05-09 08:12:46.929110 crawlee-0.0.3b9/src/crawlee/memory_storage_client/dataset_collection_client.py
--rw-r--r--   0        0        0    19187 2024-05-09 08:12:46.929110 crawlee-0.0.3b9/src/crawlee/memory_storage_client/key_value_store_client.py
--rw-r--r--   0        0        0     1534 2024-05-09 08:12:46.929110 crawlee-0.0.3b9/src/crawlee/memory_storage_client/key_value_store_collection_client.py
--rw-r--r--   0        0        0    11318 2024-05-09 08:12:46.929110 crawlee-0.0.3b9/src/crawlee/memory_storage_client/memory_storage_client.py
--rw-r--r--   0        0        0        0 2024-05-09 08:12:46.929110 crawlee-0.0.3b9/src/crawlee/memory_storage_client/py.typed
--rw-r--r--   0        0        0    22665 2024-05-09 08:12:46.929110 crawlee-0.0.3b9/src/crawlee/memory_storage_client/request_queue_client.py
--rw-r--r--   0        0        0     1518 2024-05-09 08:12:46.929110 crawlee-0.0.3b9/src/crawlee/memory_storage_client/request_queue_collection_client.py
--rw-r--r--   0        0        0        0 2024-05-09 08:12:46.929110 crawlee-0.0.3b9/src/crawlee/py.typed
--rw-r--r--   0        0        0     6670 2024-05-09 08:12:46.929110 crawlee-0.0.3b9/src/crawlee/request.py
--rw-r--r--   0        0        0       67 2024-05-09 08:12:46.929110 crawlee-0.0.3b9/src/crawlee/sessions/__init__.py
--rw-r--r--   0        0        0     2430 2024-05-09 08:12:46.929110 crawlee-0.0.3b9/src/crawlee/sessions/models.py
--rw-r--r--   0        0        0        0 2024-05-09 08:12:46.929110 crawlee-0.0.3b9/src/crawlee/sessions/py.typed
--rw-r--r--   0        0        0     8084 2024-05-09 08:12:46.929110 crawlee-0.0.3b9/src/crawlee/sessions/session.py
--rw-r--r--   0        0        0    11695 2024-05-09 08:12:46.929110 crawlee-0.0.3b9/src/crawlee/sessions/session_pool.py
--rw-r--r--   0        0        0     1651 2024-05-09 08:12:46.929110 crawlee-0.0.3b9/src/crawlee/storage_client_manager.py
--rw-r--r--   0        0        0      150 2024-05-09 08:12:46.929110 crawlee-0.0.3b9/src/crawlee/storages/__init__.py
--rw-r--r--   0        0        0     7048 2024-05-09 08:12:46.929110 crawlee-0.0.3b9/src/crawlee/storages/base_storage.py
--rw-r--r--   0        0        0    15692 2024-05-09 08:12:46.929110 crawlee-0.0.3b9/src/crawlee/storages/dataset.py
--rw-r--r--   0        0        0     5004 2024-05-09 08:12:46.929110 crawlee-0.0.3b9/src/crawlee/storages/key_value_store.py
--rw-r--r--   0        0        0     6486 2024-05-09 08:12:46.929110 crawlee-0.0.3b9/src/crawlee/storages/models.py
--rw-r--r--   0        0        0        0 2024-05-09 08:12:46.929110 crawlee-0.0.3b9/src/crawlee/storages/py.typed
--rw-r--r--   0        0        0     2593 2024-05-09 08:12:46.929110 crawlee-0.0.3b9/src/crawlee/storages/request_list.py
--rw-r--r--   0        0        0     2775 2024-05-09 08:12:46.929110 crawlee-0.0.3b9/src/crawlee/storages/request_provider.py
--rw-r--r--   0        0        0    25855 2024-05-09 08:12:46.929110 crawlee-0.0.3b9/src/crawlee/storages/request_queue.py
--rw-r--r--   0        0        0      630 2024-05-09 08:12:46.929110 crawlee-0.0.3b9/src/crawlee/types.py
--rw-r--r--   0        0        0     2083 1970-01-01 00:00:00.000000 crawlee-0.0.3b9/PKG-INFO
+-rw-r--r--   0        0        0    11355 2024-05-21 10:42:40.827903 crawlee-0.0.4b1/LICENSE
+-rw-r--r--   0        0        0    16623 2024-05-21 10:42:40.827903 crawlee-0.0.4b1/README.md
+-rw-r--r--   0        0        0     6603 2024-05-21 10:42:58.843917 crawlee-0.0.4b1/pyproject.toml
+-rw-r--r--   0        0        0       31 2024-05-21 10:42:40.827903 crawlee-0.0.4b1/src/crawlee/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-21 10:42:40.827903 crawlee-0.0.4b1/src/crawlee/_utils/__init__.py
+-rw-r--r--   0        0        0      774 2024-05-21 10:42:40.827903 crawlee-0.0.4b1/src/crawlee/_utils/blocked.py
+-rw-r--r--   0        0        0     3341 2024-05-21 10:42:40.827903 crawlee-0.0.4b1/src/crawlee/_utils/byte_size.py
+-rw-r--r--   0        0        0      759 2024-05-21 10:42:40.827903 crawlee-0.0.4b1/src/crawlee/_utils/crypto.py
+-rw-r--r--   0        0        0     3365 2024-05-21 10:42:40.827903 crawlee-0.0.4b1/src/crawlee/_utils/data_processing.py
+-rw-r--r--   0        0        0     1683 2024-05-21 10:42:40.827903 crawlee-0.0.4b1/src/crawlee/_utils/env_vars.py
+-rw-r--r--   0        0        0     3503 2024-05-21 10:42:40.827903 crawlee-0.0.4b1/src/crawlee/_utils/file.py
+-rw-r--r--   0        0        0     5262 2024-05-21 10:42:40.827903 crawlee-0.0.4b1/src/crawlee/_utils/globs.py
+-rw-r--r--   0        0        0     2056 2024-05-21 10:42:40.827903 crawlee-0.0.4b1/src/crawlee/_utils/lru_cache.py
+-rw-r--r--   0        0        0      918 2024-05-21 10:42:40.827903 crawlee-0.0.4b1/src/crawlee/_utils/math.py
+-rw-r--r--   0        0        0      715 2024-05-21 10:42:40.827903 crawlee-0.0.4b1/src/crawlee/_utils/measure_time.py
+-rw-r--r--   0        0        0      790 2024-05-21 10:42:40.827903 crawlee-0.0.4b1/src/crawlee/_utils/models.py
+-rw-r--r--   0        0        0     1585 2024-05-21 10:42:40.827903 crawlee-0.0.4b1/src/crawlee/_utils/recurring_task.py
+-rw-r--r--   0        0        0     4765 2024-05-21 10:42:40.827903 crawlee-0.0.4b1/src/crawlee/_utils/requests.py
+-rw-r--r--   0        0        0     2414 2024-05-21 10:42:40.827903 crawlee-0.0.4b1/src/crawlee/_utils/system.py
+-rw-r--r--   0        0        0     1429 2024-05-21 10:42:40.827903 crawlee-0.0.4b1/src/crawlee/_utils/wait.py
+-rw-r--r--   0        0        0      142 2024-05-21 10:42:40.827903 crawlee-0.0.4b1/src/crawlee/autoscaling/__init__.py
+-rw-r--r--   0        0        0    14883 2024-05-21 10:42:40.827903 crawlee-0.0.4b1/src/crawlee/autoscaling/autoscaled_pool.py
+-rw-r--r--   0        0        0        0 2024-05-21 10:42:40.827903 crawlee-0.0.4b1/src/crawlee/autoscaling/py.typed
+-rw-r--r--   0        0        0    15793 2024-05-21 10:42:40.827903 crawlee-0.0.4b1/src/crawlee/autoscaling/snapshotter.py
+-rw-r--r--   0        0        0     9293 2024-05-21 10:42:40.827903 crawlee-0.0.4b1/src/crawlee/autoscaling/system_status.py
+-rw-r--r--   0        0        0     5140 2024-05-21 10:42:40.827903 crawlee-0.0.4b1/src/crawlee/autoscaling/types.py
+-rw-r--r--   0        0        0      470 2024-05-21 10:42:40.827903 crawlee-0.0.4b1/src/crawlee/base_storage_client/__init__.py
+-rw-r--r--   0        0        0     9143 2024-05-21 10:42:40.827903 crawlee-0.0.4b1/src/crawlee/base_storage_client/base_dataset_client.py
+-rw-r--r--   0        0        0     1883 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/base_storage_client/base_dataset_collection_client.py
+-rw-r--r--   0        0        0     3486 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/base_storage_client/base_key_value_store_client.py
+-rw-r--r--   0        0        0     2025 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/base_storage_client/base_key_value_store_collection_client.py
+-rw-r--r--   0        0        0     5622 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/base_storage_client/base_request_queue_client.py
+-rw-r--r--   0        0        0     1992 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/base_storage_client/base_request_queue_collection_client.py
+-rw-r--r--   0        0        0     2229 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/base_storage_client/base_storage_client.py
+-rw-r--r--   0        0        0        0 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/base_storage_client/py.typed
+-rw-r--r--   0        0        0      735 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/base_storage_client/types.py
+-rw-r--r--   0        0        0      186 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/basic_crawler/__init__.py
+-rw-r--r--   0        0        0    27235 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/basic_crawler/basic_crawler.py
+-rw-r--r--   0        0        0     4696 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/basic_crawler/context_pipeline.py
+-rw-r--r--   0        0        0     2145 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/basic_crawler/errors.py
+-rw-r--r--   0        0        0     2279 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/basic_crawler/router.py
+-rw-r--r--   0        0        0     2706 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/basic_crawler/types.py
+-rw-r--r--   0        0        0       86 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/beautifulsoup_crawler/__init__.py
+-rw-r--r--   0        0        0     5409 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/beautifulsoup_crawler/beautifulsoup_crawler.py
+-rw-r--r--   0        0        0      524 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/beautifulsoup_crawler/types.py
+-rw-r--r--   0        0        0     1310 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/configuration.py
+-rw-r--r--   0        0        0      146 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/consts.py
+-rw-r--r--   0        0        0      272 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/enqueue_strategy.py
+-rw-r--r--   0        0        0       91 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/events/__init__.py
+-rw-r--r--   0        0        0     7211 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/events/event_manager.py
+-rw-r--r--   0        0        0     2682 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/events/local_event_manager.py
+-rw-r--r--   0        0        0        0 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/events/py.typed
+-rw-r--r--   0        0        0     1303 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/events/types.py
+-rw-r--r--   0        0        0        0 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/http_clients/__init__.py
+-rw-r--r--   0        0        0     1976 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/http_clients/base_http_client.py
+-rw-r--r--   0        0        0     4426 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/http_clients/httpx_client.py
+-rw-r--r--   0        0        0       59 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/http_crawler/__init__.py
+-rw-r--r--   0        0        0     2852 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/http_crawler/http_crawler.py
+-rw-r--r--   0        0        0      329 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/http_crawler/types.py
+-rw-r--r--   0        0        0     4719 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/log_config.py
+-rw-r--r--   0        0        0       55 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/memory_storage_client/__init__.py
+-rw-r--r--   0        0        0    15666 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/memory_storage_client/_creation_management.py
+-rw-r--r--   0        0        0    15684 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/memory_storage_client/dataset_client.py
+-rw-r--r--   0        0        0     2243 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/memory_storage_client/dataset_collection_client.py
+-rw-r--r--   0        0        0    15914 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/memory_storage_client/key_value_store_client.py
+-rw-r--r--   0        0        0     2333 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/memory_storage_client/key_value_store_collection_client.py
+-rw-r--r--   0        0        0    11113 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/memory_storage_client/memory_storage_client.py
+-rw-r--r--   0        0        0        0 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/memory_storage_client/py.typed
+-rw-r--r--   0        0        0    20944 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/memory_storage_client/request_queue_client.py
+-rw-r--r--   0        0        0     2316 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/memory_storage_client/request_queue_collection_client.py
+-rw-r--r--   0        0        0    12997 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/models.py
+-rw-r--r--   0        0        0        0 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/py.typed
+-rw-r--r--   0        0        0       67 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/sessions/__init__.py
+-rw-r--r--   0        0        0     2430 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/sessions/models.py
+-rw-r--r--   0        0        0        0 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/sessions/py.typed
+-rw-r--r--   0        0        0     8084 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/sessions/session.py
+-rw-r--r--   0        0        0    11695 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/sessions/session_pool.py
+-rw-r--r--   0        0        0        0 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/statistics/__init__.py
+-rw-r--r--   0        0        0      980 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/statistics/error_tracker.py
+-rw-r--r--   0        0        0     3646 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/statistics/models.py
+-rw-r--r--   0        0        0    10880 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/statistics/statistics.py
+-rw-r--r--   0        0        0     1520 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/storage_client_manager.py
+-rw-r--r--   0        0        0      150 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/storages/__init__.py
+-rw-r--r--   0        0        0     8804 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/storages/_creation_management.py
+-rw-r--r--   0        0        0     1090 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/storages/base_storage.py
+-rw-r--r--   0        0        0    15956 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/storages/dataset.py
+-rw-r--r--   0        0        0     4994 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/storages/key_value_store.py
+-rw-r--r--   0        0        0        0 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/storages/py.typed
+-rw-r--r--   0        0        0     2841 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/storages/request_list.py
+-rw-r--r--   0        0        0     2755 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/storages/request_provider.py
+-rw-r--r--   0        0        0    25708 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/storages/request_queue.py
+-rw-r--r--   0        0        0      630 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/types.py
+-rw-r--r--   0        0        0    18689 1970-01-01 00:00:00.000000 crawlee-0.0.4b1/PKG-INFO
```

### Comparing `crawlee-0.0.3b9/LICENSE` & `crawlee-0.0.4b1/LICENSE`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b9/pyproject.toml` & `crawlee-0.0.4b1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "crawlee"
-version = "0.0.3b9"
+version = "0.0.4b1"
 description = "Crawlee for Python"
 authors = ["Apify Technologies s.r.o. <support@apify.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{ include = "crawlee", from = "src" }]
 classifiers = [
     "Development Status :: 3 - Alpha",
@@ -191,7 +191,15 @@
 
 [tool.coverage.report]
 exclude_lines = [
     "pragma: no cover",
     "if TYPE_CHECKING:",
     "assert_never()"
 ]
+
+[tool.basedpyright]
+reportPrivateLocalImportUsage = false
+reportUnusedCallResult = false
+reportUnusedVariable = false
+reportCallInDefaultInitializer = false
+reportImplicitStringConcatenation = false
+reportAny = false
```

### Comparing `crawlee-0.0.3b9/src/crawlee/_utils/blocked.py` & `crawlee-0.0.4b1/src/crawlee/_utils/blocked.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b9/src/crawlee/_utils/byte_size.py` & `crawlee-0.0.4b1/src/crawlee/_utils/byte_size.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b9/src/crawlee/_utils/crypto.py` & `crawlee-0.0.4b1/src/crawlee/_utils/crypto.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b9/src/crawlee/_utils/data_processing.py` & `crawlee-0.0.4b1/src/crawlee/_utils/data_processing.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b9/src/crawlee/_utils/file.py` & `crawlee-0.0.4b1/src/crawlee/_utils/file.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 from __future__ import annotations
 
 import asyncio
 import contextlib
 import io
 import json
 import mimetypes
-import os
 import re
 from enum import Enum
 from typing import Any
 
-import aiofiles
 import aioshutil
 from aiofiles import ospath
-from aiofiles.os import makedirs, remove, rename
+from aiofiles.os import remove, rename
 
 
 class ContentType(Enum):
     JSON = r'^application/json'
     TEXT = r'^text/'
     XML = r'^application/.*xml$'
 
@@ -104,33 +102,7 @@
     Args:
         obj: The object to serialize.
 
     Returns:
         A string containing the JSON representation of the input object.
     """
     return await asyncio.to_thread(json.dumps, obj, ensure_ascii=False, indent=2, default=str)
-
-
-async def persist_metadata_if_enabled(*, data: dict, entity_directory: str, write_metadata: bool) -> None:
-    """Updates or writes metadata to a specified directory.
-
-    The function writes a given metadata dictionary to a JSON file within a specified directory.
-    The writing process is skipped if `write_metadata` is False. Before writing, it ensures that
-    the target directory exists, creating it if necessary.
-
-    Args:
-        data: A dictionary containing metadata to be written.
-        entity_directory: The directory path where the metadata file should be stored.
-        write_metadata: A boolean flag indicating whether the metadata should be written to file.
-    """
-    # Skip metadata write; ensure directory exists first
-    if not write_metadata:
-        return
-
-    # Ensure the directory for the entity exists
-    await makedirs(entity_directory, exist_ok=True)
-
-    # Write the metadata to the file
-    file_path = os.path.join(entity_directory, '__metadata__.json')
-    async with aiofiles.open(file_path, mode='wb') as f:
-        s = await json_dumps(data)
-        await f.write(s.encode('utf-8'))
```

### Comparing `crawlee-0.0.3b9/src/crawlee/_utils/globs.py` & `crawlee-0.0.4b1/src/crawlee/_utils/globs.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b9/src/crawlee/_utils/lru_cache.py` & `crawlee-0.0.4b1/src/crawlee/_utils/lru_cache.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b9/src/crawlee/_utils/math.py` & `crawlee-0.0.4b1/src/crawlee/_utils/math.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b9/src/crawlee/_utils/measure_time.py` & `crawlee-0.0.4b1/src/crawlee/_utils/measure_time.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b9/src/crawlee/_utils/recurring_task.py` & `crawlee-0.0.4b1/src/crawlee/_utils/recurring_task.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b9/src/crawlee/_utils/requests.py` & `crawlee-0.0.4b1/src/crawlee/_utils/requests.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b9/src/crawlee/_utils/system.py` & `crawlee-0.0.4b1/src/crawlee/_utils/system.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b9/src/crawlee/_utils/wait.py` & `crawlee-0.0.4b1/src/crawlee/_utils/wait.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b9/src/crawlee/autoscaling/autoscaled_pool.py` & `crawlee-0.0.4b1/src/crawlee/autoscaling/autoscaled_pool.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b9/src/crawlee/autoscaling/snapshotter.py` & `crawlee-0.0.4b1/src/crawlee/autoscaling/snapshotter.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b9/src/crawlee/autoscaling/system_status.py` & `crawlee-0.0.4b1/src/crawlee/autoscaling/system_status.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b9/src/crawlee/autoscaling/types.py` & `crawlee-0.0.4b1/src/crawlee/autoscaling/types.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b9/src/crawlee/base_storage_client/base_dataset_client.py` & `crawlee-0.0.4b1/src/crawlee/base_storage_client/base_dataset_client.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from typing import TYPE_CHECKING, AsyncIterator
 
 if TYPE_CHECKING:
-    from crawlee.storages.models import DatasetItemsListPage, DatasetMetadata
+    from crawlee.models import DatasetItemsListPage, DatasetMetadata
     from crawlee.types import JSONSerializable
 
 
 class BaseDatasetClient(ABC):
     """Abstract base class for dataset resource clients.
 
     These clients are specific to the type of resource they manage and operate under a designated storage
@@ -124,24 +124,24 @@
     @abstractmethod
     async def get_items_as_bytes(
         self,
         *,
         item_format: str = 'json',
         offset: int | None = None,
         limit: int | None = None,
-        desc: bool | None = None,
-        clean: bool | None = None,
-        bom: bool | None = None,
+        desc: bool = False,
+        clean: bool = False,
+        bom: bool = False,
         delimiter: str | None = None,
         fields: list[str] | None = None,
         omit: list[str] | None = None,
         unwind: str | None = None,
-        skip_empty: bool | None = None,
-        skip_header_row: bool | None = None,
-        skip_hidden: bool | None = None,
+        skip_empty: bool = False,
+        skip_header_row: bool = False,
+        skip_hidden: bool = False,
         xml_root: str | None = None,
         xml_row: str | None = None,
         flatten: list[str] | None = None,
     ) -> bytes:
         """Retrieves dataset items as bytes.
 
         Args:
@@ -169,24 +169,24 @@
     @abstractmethod
     async def stream_items(
         self,
         *,
         item_format: str = 'json',
         offset: int | None = None,
         limit: int | None = None,
-        desc: bool | None = None,
-        clean: bool | None = None,
-        bom: bool | None = None,
+        desc: bool = False,
+        clean: bool = False,
+        bom: bool = False,
         delimiter: str | None = None,
         fields: list[str] | None = None,
         omit: list[str] | None = None,
         unwind: str | None = None,
-        skip_empty: bool | None = None,
-        skip_header_row: bool | None = None,
-        skip_hidden: bool | None = None,
+        skip_empty: bool = False,
+        skip_header_row: bool = False,
+        skip_hidden: bool = False,
         xml_root: str | None = None,
         xml_row: str | None = None,
     ) -> AsyncIterator[dict]:
         """Retrieves dataset items as a streaming response.
 
         Args:
             item_format: Output format, options include json, jsonl, csv, html, xlsx, xml, rss; default is json.
```

### Comparing `crawlee-0.0.3b9/src/crawlee/base_storage_client/base_dataset_collection_client.py` & `crawlee-0.0.4b1/src/crawlee/base_storage_client/base_dataset_collection_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
-    from crawlee.storages.models import DatasetListPage, DatasetMetadata
+    from crawlee.models import DatasetListPage, DatasetMetadata
 
 
 class BaseDatasetCollectionClient(ABC):
     """Abstract base class for dataset collection clients.
 
     This collection client handles operations that involve multiple instances of a given resource type.
     """
@@ -36,18 +36,18 @@
             Metadata object containing the information of the retrieved or created dataset.
         """
 
     @abstractmethod
     async def list(
         self,
         *,
-        unnamed: bool | None = None,
+        unnamed: bool = False,
         limit: int | None = None,
         offset: int | None = None,
-        desc: bool | None = None,
+        desc: bool = False,
     ) -> DatasetListPage:
         """List the available datasets.
 
         Args:
             unnamed: Whether to list only the unnamed datasets.
             limit: Maximum number of datasets to return.
             offset: Number of datasets to skip from the beginning of the list.
```

### Comparing `crawlee-0.0.3b9/src/crawlee/base_storage_client/base_key_value_store_client.py` & `crawlee-0.0.4b1/src/crawlee/base_storage_client/base_key_value_store_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from typing import TYPE_CHECKING, Any, AsyncIterator
 
 if TYPE_CHECKING:
-    from crawlee.storages.models import KeyValueStoreListKeysPage, KeyValueStoreMetadata, KeyValueStoreRecord
+    from crawlee.models import KeyValueStoreListKeysPage, KeyValueStoreMetadata, KeyValueStoreRecord
 
 
 class BaseKeyValueStoreClient(ABC):
     """Abstract base class for key-value store resource clients.
 
     These clients are specific to the type of resource they manage and operate under a designated storage
     client, like a memory storage client.
```

### Comparing `crawlee-0.0.3b9/src/crawlee/base_storage_client/base_key_value_store_collection_client.py` & `crawlee-0.0.4b1/src/crawlee/base_storage_client/base_key_value_store_collection_client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
-    from crawlee.storages.models import KeyValueStoreListPage, KeyValueStoreMetadata
+    from crawlee.models import KeyValueStoreListPage, KeyValueStoreMetadata
 
 
 class BaseKeyValueStoreCollectionClient(ABC):
     """Abstract base class for key-value store collection clients.
 
     This collection client handles operations that involve multiple instances of a given resource type.
     """
@@ -36,18 +36,18 @@
             Metadata object containing the information of the retrieved or created key-value store.
         """
 
     @abstractmethod
     async def list(
         self,
         *,
-        unnamed: bool | None = None,
+        unnamed: bool = False,
         limit: int | None = None,
         offset: int | None = None,
-        desc: bool | None = None,
+        desc: bool = False,
     ) -> KeyValueStoreListPage:
         """List the available key-value stores.
 
         Args:
             unnamed: Whether to list only the unnamed key-value stores.
             limit: Maximum number of key-value stores to return.
             offset: Number of key-value stores to skip from the beginning of the list.
```

### Comparing `crawlee-0.0.3b9/src/crawlee/base_storage_client/base_request_queue_client.py` & `crawlee-0.0.4b1/src/crawlee/base_storage_client/base_request_queue_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
-    from crawlee.request import Request
-    from crawlee.storages.models import RequestQueueHead, RequestQueueMetadata, RequestQueueOperationInfo
+    from crawlee.models import Request, RequestQueueHead, RequestQueueMetadata, RequestQueueOperationInfo
 
 
 class BaseRequestQueueClient(ABC):
     """Abstract base class for request queue resource clients.
 
     These clients are specific to the type of resource they manage and operate under a designated storage
     client, like a memory storage client.
```

### Comparing `crawlee-0.0.3b9/src/crawlee/base_storage_client/base_request_queue_collection_client.py` & `crawlee-0.0.4b1/src/crawlee/base_storage_client/base_request_queue_collection_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
-    from crawlee.storages.models import RequestQueueListPage, RequestQueueMetadata
+    from crawlee.models import RequestQueueListPage, RequestQueueMetadata
 
 
 class BaseRequestQueueCollectionClient(ABC):
     """Abstract base class for request queue collection clients.
 
     This collection client handles operations that involve multiple instances of a given resource type.
     """
@@ -36,18 +36,18 @@
             Metadata object containing the information of the retrieved or created request queue.
         """
 
     @abstractmethod
     async def list(
         self,
         *,
-        unnamed: bool | None = None,
+        unnamed: bool = False,
         limit: int | None = None,
         offset: int | None = None,
-        desc: bool | None = None,
+        desc: bool = False,
     ) -> RequestQueueListPage:
         """List the available request queues.
 
         Args:
             unnamed: Whether to list only the unnamed request queues.
             limit: Maximum number of request queues to return.
             offset: Number of request queues to skip from the beginning of the list.
```

### Comparing `crawlee-0.0.3b9/src/crawlee/base_storage_client/base_storage_client.py` & `crawlee-0.0.4b1/src/crawlee/base_storage_client/base_storage_client.py`

 * *Files 17% similar despite different names*

```diff
@@ -40,7 +40,16 @@
     @abstractmethod
     def request_queue(self, id: str) -> BaseRequestQueueClient:
         """Gets a subclient for a specific request queue by its ID."""
 
     @abstractmethod
     def request_queues(self) -> BaseRequestQueueCollectionClient:
         """Gets a subclient for request queue collection operations."""
+
+    @abstractmethod
+    async def purge_on_start(self) -> None:
+        """Performs a purge of the default storages.
+
+        This method ensures that the purge is executed only once during the lifetime of the instance.
+        It is primarily used to clean up residual data from previous runs to maintain a clean state.
+        If the storage client does not support purging, leave it empty.
+        """
```

### Comparing `crawlee-0.0.3b9/src/crawlee/base_storage_client/types.py` & `crawlee-0.0.4b1/src/crawlee/base_storage_client/types.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b9/src/crawlee/basic_crawler/basic_crawler.py` & `crawlee-0.0.4b1/src/crawlee/basic_crawler/basic_crawler.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from __future__ import annotations
 
 import tempfile
 from contextlib import AsyncExitStack
 from datetime import timedelta
 from functools import partial
 from logging import getLogger
-from typing import TYPE_CHECKING, AsyncGenerator, Awaitable, Callable, Generic, Sequence, Union, cast
+from typing import TYPE_CHECKING, Any, AsyncGenerator, Awaitable, Callable, Generic, Sequence, Union, cast
 
 import httpx
 from tldextract import TLDExtract
 from typing_extensions import NotRequired, TypedDict, TypeVar, assert_never
 
 from crawlee import Glob
 from crawlee._utils.wait import wait_for
@@ -26,31 +26,32 @@
     RequestHandlerError,
     SessionError,
     UserDefinedErrorHandlerError,
 )
 from crawlee.basic_crawler.router import Router
 from crawlee.basic_crawler.types import (
     BasicCrawlingContext,
-    FinalStatistics,
     RequestHandlerRunResult,
     SendRequestFunction,
 )
 from crawlee.configuration import Configuration
 from crawlee.enqueue_strategy import EnqueueStrategy
 from crawlee.events.local_event_manager import LocalEventManager
 from crawlee.http_clients.httpx_client import HttpxClient
-from crawlee.request import BaseRequestData, Request, RequestState
+from crawlee.models import BaseRequestData, Request, RequestState
 from crawlee.sessions import SessionPool
+from crawlee.statistics.statistics import Statistics
 from crawlee.storages.request_queue import RequestQueue
 
 if TYPE_CHECKING:
     import re
 
     from crawlee.http_clients.base_http_client import BaseHttpClient, HttpResponse
     from crawlee.sessions.session import Session
+    from crawlee.statistics.models import FinalStatistics, StatisticsState
     from crawlee.storages.request_provider import RequestProvider
 
 TCrawlingContext = TypeVar('TCrawlingContext', bound=BasicCrawlingContext, default=BasicCrawlingContext)
 ErrorHandler = Callable[[TCrawlingContext, Exception], Awaitable[Union[Request, None]]]
 FailedRequestHandler = Callable[[TCrawlingContext, Exception], Awaitable[None]]
 
 logger = getLogger(__name__)
@@ -66,14 +67,15 @@
     max_request_retries: NotRequired[int]
     max_session_rotations: NotRequired[int]
     configuration: NotRequired[Configuration]
     request_handler_timeout: NotRequired[timedelta]
     session_pool: NotRequired[SessionPool]
     use_session_pool: NotRequired[bool]
     retry_on_blocked: NotRequired[bool]
+    statistics: NotRequired[Statistics[StatisticsState]]
     _context_pipeline: NotRequired[ContextPipeline[TCrawlingContext]]
 
 
 class BasicCrawler(Generic[TCrawlingContext]):
     """Provides a simple framework for parallel crawling of web pages.
 
     The URLs to crawl are fed either from a static list of URLs or from a dynamic queue of URLs enabling recursive
@@ -94,14 +96,15 @@
         max_request_retries: int = 3,
         max_session_rotations: int = 10,
         configuration: Configuration | None = None,
         request_handler_timeout: timedelta = timedelta(minutes=1),
         session_pool: SessionPool | None = None,
         use_session_pool: bool = True,
         retry_on_blocked: bool = True,
+        statistics: Statistics | None = None,
         _context_pipeline: ContextPipeline[TCrawlingContext] | None = None,
     ) -> None:
         """Initialize the BasicCrawler.
 
         Args:
             request_provider: Provides requests to be processed
             request_handler: A callable to which request handling is delegated
@@ -110,16 +113,17 @@
             max_request_retries: Maximum amount of attempts at processing a request
             max_session_rotations: Maximum number of session rotations per request.
                 The crawler will automatically rotate the session in case of a proxy error or if it gets blocked by
                 the website.
             configuration: Crawler configuration
             request_handler_timeout: How long is a single request handler allowed to run
             use_session_pool: Enables using the session pool for crawling
-            session_pool: A preconfigured SessionPool instance if you wish to use non-default configuration
+            session_pool: A preconfigured `SessionPool` instance if you wish to use non-default configuration
             retry_on_blocked: If set to True, the crawler will try to automatically bypass any detected bot protection
+            statistics: A preconfigured `Statistics` instance if you wish to use non-default configuration
             _context_pipeline: Allows extending the request lifecycle and modifying the crawling context.
                 This parameter is meant to be used by child classes, not when BasicCrawler is instantiated directly.
         """
         self._router: Router[TCrawlingContext] | None = None
 
         if isinstance(cast(Router, request_handler), Router):
             self._router = cast(Router[TCrawlingContext], request_handler)
@@ -157,18 +161,26 @@
             is_finished_function=self.__is_finished_function,
             is_task_ready_function=self.__is_task_ready_function,
             run_task_function=self.__run_task_function,
             concurrency_settings=concurrency_settings,
         )
 
         self._use_session_pool = use_session_pool
-        self._session_pool: SessionPool = session_pool or SessionPool()
+        self._session_pool = session_pool or SessionPool()
 
         self._retry_on_blocked = retry_on_blocked
 
+        self._statistics = statistics or Statistics(
+            event_manager=self._event_manager,
+            log_message=f'{logger.name} request statistics',
+        )
+
+        self._running = False
+        self._has_finished_before = False
+
     @property
     def router(self) -> Router[TCrawlingContext]:
         """The router used to handle each individual crawling request."""
         if self._router is None:
             self._router = Router[TCrawlingContext]()
 
         return self._router
@@ -176,14 +188,19 @@
     @router.setter
     def router(self, router: Router[TCrawlingContext]) -> None:
         if self._router is not None:
             raise RuntimeError('A router is already set')
 
         self._router = router
 
+    @property
+    def statistics(self) -> Statistics[StatisticsState]:
+        """Statistics about the current (or last) crawler run."""
+        return self._statistics
+
     async def _get_session(self) -> Session | None:
         """If session pool is being used, try to take a session from it."""
         if not self._use_session_pool:
             return None
 
         return await wait_for(
             self._session_pool.get_session,
@@ -231,27 +248,51 @@
             batch_size=batch_size,
             wait_for_all_requests_to_be_added=wait_for_all_requests_to_be_added,
             wait_time_between_batches=wait_time_between_batches,
         )
 
     async def run(self, requests: list[str | BaseRequestData] | None = None) -> FinalStatistics:
         """Run the crawler until all requests are processed."""
+        if self._running:
+            raise RuntimeError(
+                'This crawler instance is already running, you can add more requests to it via `crawler.add_requests()`'
+            )
+
+        self._running = True
+
+        if self._has_finished_before:
+            await self._statistics.reset()
+
+            if self._use_session_pool:
+                await self._session_pool.reset_store()
+
         if requests is not None:
             await self.add_requests(requests)
 
         async with AsyncExitStack() as exit_stack:
             await exit_stack.enter_async_context(self._event_manager)
             await exit_stack.enter_async_context(self._snapshotter)
+            await exit_stack.enter_async_context(self._statistics)
 
             if self._use_session_pool:
                 await exit_stack.enter_async_context(self._session_pool)
 
             await self._pool.run()
 
-        return FinalStatistics()
+        if self._statistics.error_tracker.total > 0:
+            logger.info(
+                'Error analysis:'
+                f' total_errors={self._statistics.error_tracker.total}'
+                f' unique_errors={self._statistics.error_tracker.unique_error_count}'
+            )
+
+        self._running = False
+        self._has_finished_before = True
+
+        return self._statistics.calculate()
 
     def _should_retry_request(self, crawling_context: BasicCrawlingContext, error: Exception) -> bool:
         if crawling_context.request.no_retry:
             return False
 
         if isinstance(error, SessionError):
             return ((crawling_context.request.session_rotation_count or 0) + 1) < self._max_session_rotations
@@ -294,21 +335,21 @@
 
         if strategy == EnqueueStrategy.SAME_ORIGIN:
             return target_url.host == origin_url.host and target_url.scheme == origin_url.scheme
 
         if strategy == EnqueueStrategy.ALL:
             return True
 
-        assert_never()
+        assert_never(strategy)
 
     def _check_url_patterns(
         self,
         target_url: httpx.URL,
-        include: Sequence[re.Pattern | Glob] | None,
-        exclude: Sequence[re.Pattern | Glob] | None,
+        include: Sequence[re.Pattern[Any] | Glob] | None,
+        exclude: Sequence[re.Pattern[Any] | Glob] | None,
     ) -> bool:
         """Check if a URL matches configured include/exclude patterns."""
         # If the URL matches any `exclude` pattern, reject it
         for pattern in exclude or ():
             if isinstance(pattern, Glob):
                 pattern = pattern.regexp  # noqa: PLW2901
 
@@ -328,18 +369,19 @@
                 return True
 
         # The URL does not match any `include` pattern - reject it
         return False
 
     async def _handle_request_error(self, crawling_context: TCrawlingContext, error: Exception) -> None:
         request_provider = await self.get_request_provider()
+        request = crawling_context.request
 
         if self._should_retry_request(crawling_context, error):
-            request = crawling_context.request
             request.retry_count += 1
+            self._statistics.error_tracker.add(error)
 
             if self._error_handler:
                 try:
                     new_request = await self._error_handler(crawling_context, error)
                 except Exception as e:
                     raise UserDefinedErrorHandlerError('Exception thrown in user-defined request error handler') from e
                 else:
@@ -353,17 +395,19 @@
                 timeout=self._internal_timeout,
                 timeout_message='Marking request as handled timed out after '
                 f'{self._internal_timeout.total_seconds()} seconds',
                 logger=logger,
                 max_retries=3,
             )
             await self._handle_failed_request(crawling_context, error)
+            self._statistics.record_request_processing_failure(request.id or request.unique_key)
 
     async def _handle_failed_request(self, crawling_context: TCrawlingContext, error: Exception) -> None:
         logger.exception('Request failed and reached maximum retries', exc_info=error)
+        self._statistics.error_tracker.add(error)
 
         if self._failed_request_handler:
             try:
                 await self._failed_request_handler(crawling_context, error)
             except Exception as e:
                 raise UserDefinedErrorHandlerError('Exception thrown in user-defined failed request handler') from e
 
@@ -437,14 +481,17 @@
         crawling_context = BasicCrawlingContext(
             request=request,
             session=session,
             send_request=self._prepare_send_request_function(session),
             add_requests=result.add_requests,
         )
 
+        statistics_id = request.id or request.unique_key
+        self._statistics.record_request_processing_start(statistics_id)
+
         try:
             request.state = RequestState.REQUEST_HANDLER
 
             await wait_for(
                 lambda: self.__run_request_handler(crawling_context),
                 timeout=self._request_handler_timeout,
                 timeout_message='Request handler timed out after '
@@ -463,14 +510,16 @@
                 max_retries=3,
             )
 
             request.state = RequestState.DONE
 
             if crawling_context.session:
                 crawling_context.session.mark_good()
+
+            self._statistics.record_request_processing_finish(statistics_id)
         except RequestHandlerError as primary_error:
             primary_error = cast(
                 RequestHandlerError[TCrawlingContext], primary_error
             )  # valid thanks to ContextPipeline
 
             try:
                 request.state = RequestState.ERROR_HANDLER
@@ -510,25 +559,29 @@
                 crawling_context.session.retire()
 
                 if crawling_context.request.session_rotation_count is None:
                     crawling_context.request.session_rotation_count = 0
                 crawling_context.request.session_rotation_count += 1
 
                 await request_provider.reclaim_request(request)
+                self._statistics.error_tracker_retry.add(session_error)
             else:
                 logger.exception('Request failed and reached maximum retries', exc_info=session_error)
 
                 await wait_for(
                     lambda: request_provider.mark_request_as_handled(crawling_context.request),
                     timeout=self._internal_timeout,
                     timeout_message='Marking request as handled timed out after '
                     f'{self._internal_timeout.total_seconds()} seconds',
                     logger=logger,
                     max_retries=3,
                 )
+
+                self._statistics.record_request_processing_failure(statistics_id)
+                self._statistics.error_tracker.add(session_error)
         except ContextPipelineInterruptedError as interruped_error:
             logger.debug('The context pipeline was interrupted', exc_info=interruped_error)
 
             await wait_for(
                 lambda: request_provider.mark_request_as_handled(crawling_context.request),
                 timeout=self._internal_timeout,
                 timeout_message='Marking request as handled timed out after '
```

### Comparing `crawlee-0.0.3b9/src/crawlee/basic_crawler/context_pipeline.py` & `crawlee-0.0.4b1/src/crawlee/basic_crawler/context_pipeline.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b9/src/crawlee/basic_crawler/errors.py` & `crawlee-0.0.4b1/src/crawlee/basic_crawler/errors.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b9/src/crawlee/basic_crawler/router.py` & `crawlee-0.0.4b1/src/crawlee/basic_crawler/router.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b9/src/crawlee/basic_crawler/types.py` & `crawlee-0.0.4b1/src/crawlee/basic_crawler/types.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from typing_extensions import NotRequired, TypedDict, Unpack
 
 if TYPE_CHECKING:
     from crawlee import Glob
     from crawlee.enqueue_strategy import EnqueueStrategy
     from crawlee.http_clients.base_http_client import HttpResponse
-    from crawlee.request import BaseRequestData, Request
+    from crawlee.models import BaseRequestData, Request
     from crawlee.sessions.session import Session
 
 
 class AddRequestsFunctionKwargs(TypedDict):
     """Keyword arguments type for AddRequestsFunction."""
 
     limit: NotRequired[int]
@@ -64,19 +64,14 @@
 
     request: Request
     session: Session | None
     send_request: SendRequestFunction
     add_requests: AddRequestsFunction
 
 
-@dataclass(frozen=True)
-class FinalStatistics:
-    """Statistics about a crawler run."""
-
-
 class AddRequestsFunctionCall(AddRequestsFunctionKwargs):
     """Record of a call to `add_requests`."""
 
     requests: Sequence[str | BaseRequestData]
 
 
 @dataclass()
```

### Comparing `crawlee-0.0.3b9/src/crawlee/beautifulsoup_crawler/beautifulsoup_crawler.py` & `crawlee-0.0.4b1/src/crawlee/beautifulsoup_crawler/beautifulsoup_crawler.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from crawlee.basic_crawler.basic_crawler import BasicCrawler, BasicCrawlerOptions
 from crawlee.basic_crawler.context_pipeline import ContextPipeline
 from crawlee.basic_crawler.errors import SessionError
 from crawlee.beautifulsoup_crawler.types import BeautifulSoupCrawlingContext
 from crawlee.enqueue_strategy import EnqueueStrategy
 from crawlee.http_clients.httpx_client import HttpxClient
 from crawlee.http_crawler.types import HttpCrawlingContext
-from crawlee.request import BaseRequestData
+from crawlee.models import BaseRequestData
 
 if TYPE_CHECKING:
     from crawlee.basic_crawler.types import AddRequestsFunctionKwargs, BasicCrawlingContext
 
 
 class BeautifulSoupCrawler(BasicCrawler[BeautifulSoupCrawlingContext]):
     """A crawler that fetches the request URL using `httpx` and parses the result with `BeautifulSoup`."""
@@ -58,15 +58,15 @@
                 ignore_http_error_status_codes=ignore_http_error_status_codes,
             ),
         )
 
         super().__init__(**kwargs)
 
     async def _make_http_request(self, context: BasicCrawlingContext) -> AsyncGenerator[HttpCrawlingContext, None]:
-        result = await self._http_client.crawl(context.request, context.session)
+        result = await self._http_client.crawl(context.request, context.session, self._statistics)
 
         yield HttpCrawlingContext(
             request=context.request,
             session=context.session,
             send_request=context.send_request,
             add_requests=context.add_requests,
             http_response=result.http_response,
```

### Comparing `crawlee-0.0.3b9/src/crawlee/beautifulsoup_crawler/types.py` & `crawlee-0.0.4b1/src/crawlee/beautifulsoup_crawler/types.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b9/src/crawlee/configuration.py` & `crawlee-0.0.4b1/src/crawlee/configuration.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,28 +2,30 @@
 
 from __future__ import annotations
 
 from datetime import timedelta
 from typing import Annotated
 
 from pydantic import Field
-from pydantic_settings import BaseSettings
+from pydantic_settings import BaseSettings, SettingsConfigDict
 
 
 class Configuration(BaseSettings):
     """Configuration of the Crawler.
 
     Args:
         internal_timeout: timeout for internal operations such as marking a request as processed
         verbose_log: allows verbose logging
-        default_dataset_id: The default dataset ID.
-        default_key_value_store_id: The default key-value store ID.
-        default_request_queue_id: The default request queue ID.
+        default_storage_id: The default storage ID.
         purge_on_start: Whether to purge the storage on start.
     """
 
+    model_config = SettingsConfigDict(populate_by_name=True)
+
     internal_timeout: Annotated[timedelta | None, Field(alias='crawlee_internal_timeout')] = None
     verbose_log: Annotated[bool, Field(alias='crawlee_verbose_log')] = False
-    default_dataset_id: Annotated[str, Field(alias='crawlee_default_dataset_id')] = 'default'
-    default_key_value_store_id: Annotated[str, Field(alias='crawlee_default_key_value_store_id')] = 'default'
-    default_request_queue_id: Annotated[str, Field(alias='crawlee_default_request_queue_id')] = 'default'
-    purge_on_start: Annotated[bool, Field(alias='crawlee_purge_on_start')] = False
+    default_storage_id: Annotated[str, Field(alias='crawlee_default_storage_id')] = 'default'
+    purge_on_start: Annotated[bool, Field(alias='crawlee_purge_on_start')] = True
+    write_metadata: Annotated[bool, Field(alias='crawlee_write_metadata')] = True
+    persist_storage: Annotated[bool, Field(alias='crawlee_persist_storage')] = True
+    local_storage_dir: Annotated[str, Field(alias='crawlee_local_storage_dir')] = './storage'
+    in_cloud: Annotated[bool, Field(alias='crawlee_in_cloud')] = False
```

### Comparing `crawlee-0.0.3b9/src/crawlee/events/event_manager.py` & `crawlee-0.0.4b1/src/crawlee/events/event_manager.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b9/src/crawlee/events/local_event_manager.py` & `crawlee-0.0.4b1/src/crawlee/events/local_event_manager.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b9/src/crawlee/events/types.py` & `crawlee-0.0.4b1/src/crawlee/events/types.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b9/src/crawlee/http_clients/base_http_client.py` & `crawlee-0.0.4b1/src/crawlee/http_clients/base_http_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from typing import TYPE_CHECKING, Iterable, Protocol
 
 if TYPE_CHECKING:
     from httpx import Headers  # Type from `httpx` is used here because it is lightweight and convenient
 
-    from crawlee.request import Request
+    from crawlee.models import Request
     from crawlee.sessions.session import Session
+    from crawlee.statistics.statistics import Statistics
 
 
 class HttpResponse(Protocol):
     """Response to an HTTP call."""
 
     def read(self) -> bytes:
         """Read the content of the response body."""
@@ -44,15 +45,20 @@
         ignore_http_error_status_codes: Iterable[int] = (),
     ) -> None:
         self._persist_cookies_per_session = persist_cookies_per_session
         self._additional_http_error_status_codes = set(additional_http_error_status_codes)
         self._ignore_http_error_status_codes = set(ignore_http_error_status_codes)
 
     @abstractmethod
-    async def crawl(self, request: Request, session: Session | None) -> HttpCrawlingResult:
+    async def crawl(
+        self,
+        request: Request,
+        session: Session | None,
+        statistics: Statistics,
+    ) -> HttpCrawlingResult:
         """Perform a crawl of an URL."""
 
     @abstractmethod
     async def send_request(
         self, url: str, *, method: str, headers: Headers | dict[str, str], session: Session | None = None
     ) -> HttpResponse:
         """Perform an HTTP request."""
```

### Comparing `crawlee-0.0.3b9/src/crawlee/http_clients/httpx_client.py` & `crawlee-0.0.4b1/src/crawlee/http_clients/httpx_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 
 from crawlee._utils.blocked import ROTATE_PROXY_ERRORS
 from crawlee.basic_crawler.errors import ProxyError
 from crawlee.http_clients.base_http_client import BaseHttpClient, HttpCrawlingResult, HttpResponse
 from crawlee.sessions.session import Session
 
 if TYPE_CHECKING:
-    from crawlee.request import Request
+    from crawlee.models import Request
+    from crawlee.statistics.statistics import Statistics
 
 
 class HttpTransport(httpx.AsyncHTTPTransport):
     """A modified HTTP transport adapter that stores response cookies in a `Session` instead of the httpx client."""
 
     @override
     async def handle_async_request(
@@ -60,15 +61,15 @@
             persist_cookies_per_session=persist_cookies_per_session,
             additional_http_error_status_codes=additional_http_error_status_codes,
             ignore_http_error_status_codes=ignore_http_error_status_codes,
         )
         self._client = httpx.AsyncClient(transport=HttpTransport())
 
     @override
-    async def crawl(self, request: Request, session: Session | None) -> HttpCrawlingResult:
+    async def crawl(self, request: Request, session: Session | None, statistics: Statistics) -> HttpCrawlingResult:
         http_request = self._client.build_request(
             method=request.method,
             url=request.url,
             headers=request.headers,
             cookies=session.cookies if session else None,
             extensions={'crawlee_session': session if self._persist_cookies_per_session else None},
         )
@@ -77,14 +78,16 @@
             response = await self._client.send(http_request, follow_redirects=True)
         except httpx.TransportError as e:
             if _is_proxy_error(e):
                 raise ProxyError from e
 
             raise
 
+        statistics.register_status_code(response.status_code)
+
         exclude_error = response.status_code in self._ignore_http_error_status_codes
         include_error = response.status_code in self._additional_http_error_status_codes
 
         if include_error or (response.is_server_error and not exclude_error):
             if include_error:
                 raise httpx.HTTPStatusError(
                     f'Status code {response.status_code} (user-configured to be an error) returned',
```

### Comparing `crawlee-0.0.3b9/src/crawlee/http_crawler/http_crawler.py` & `crawlee-0.0.4b1/src/crawlee/http_crawler/http_crawler.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         )
 
         super().__init__(**kwargs)
 
     async def _make_http_request(
         self, crawling_context: BasicCrawlingContext
     ) -> AsyncGenerator[HttpCrawlingContext, None]:
-        result = await self._http_client.crawl(crawling_context.request, crawling_context.session)
+        result = await self._http_client.crawl(crawling_context.request, crawling_context.session, self._statistics)
 
         yield HttpCrawlingContext(
             request=crawling_context.request,
             session=crawling_context.session,
             send_request=crawling_context.send_request,
             add_requests=crawling_context.add_requests,
             http_response=result.http_response,
```

### Comparing `crawlee-0.0.3b9/src/crawlee/log_config.py` & `crawlee-0.0.4b1/src/crawlee/log_config.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b9/src/crawlee/memory_storage_client/base_resource_collection_client.py` & `crawlee-0.0.4b1/src/crawlee/memory_storage_client/request_queue_collection_client.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,81 +1,71 @@
 from __future__ import annotations
 
-from abc import ABC, abstractmethod
-from typing import TYPE_CHECKING, Generic, TypeVar
+from typing import TYPE_CHECKING
 
-from crawlee._utils.file import persist_metadata_if_enabled
-from crawlee.memory_storage_client.base_resource_client import BaseResourceClient
+from typing_extensions import override
 
-if TYPE_CHECKING:
-    from crawlee.memory_storage_client import MemoryStorageClient
-    from crawlee.storages.models import BaseStorageMetadata
+from crawlee.base_storage_client import BaseRequestQueueCollectionClient
+from crawlee.memory_storage_client._creation_management import get_or_create_inner
+from crawlee.memory_storage_client.request_queue_client import RequestQueueClient
+from crawlee.models import RequestQueueListPage, RequestQueueMetadata
 
-ResourceClientType = TypeVar('ResourceClientType', bound=BaseResourceClient, contravariant=True)  # noqa: PLC0105
+if TYPE_CHECKING:
+    from crawlee.memory_storage_client.memory_storage_client import MemoryStorageClient
 
 
-class BaseResourceCollectionClient(ABC, Generic[ResourceClientType]):
-    """Base class for resource collection clients."""
+class RequestQueueCollectionClient(BaseRequestQueueCollectionClient):
+    """Subclient for manipulating request queues."""
 
     def __init__(
         self,
         *,
         base_storage_directory: str,
         memory_storage_client: MemoryStorageClient,
     ) -> None:
         self._base_storage_directory = base_storage_directory
         self._memory_storage_client = memory_storage_client
 
     @property
-    @abstractmethod
-    def _client_class(self) -> type[ResourceClientType]:
-        """Get the class of the resource clients."""
-
-    @abstractmethod
-    def _get_storage_client_cache(self) -> list[ResourceClientType]:
-        """Get the storage client cache."""
+    def _storage_client_cache(self) -> list[RequestQueueClient]:
+        return self._memory_storage_client.request_queues_handled
 
+    @override
     async def get_or_create(
         self,
         *,
         name: str | None = None,
-        schema: dict | None = None,  # noqa: ARG002
+        schema: dict | None = None,
         id: str | None = None,
-    ) -> BaseStorageMetadata:
-        """Retrieve a named storage, or create a new one when it doesn't exist.
-
-        Args:
-            name: The name of the storage to retrieve or create.
-            schema: The schema of the storage
-            id: ID of the storage to retrieve or create
-
-        Returns:
-            The retrieved or newly-created storage.
-        """
-        resource_client_class = self._client_class
-        storage_client_cache = self._get_storage_client_cache()
-
-        if name or id:
-            found = resource_client_class.find_or_create_client_by_id_or_name(
-                memory_storage_client=self._memory_storage_client,
-                name=name,
-                id=id,
-            )
-            if found:
-                return found.resource_info
+    ) -> RequestQueueMetadata:
+        if name is None and id is None:
+            id = self._memory_storage_client.default_storage_id
 
-        new_resource = resource_client_class(
-            id=id,
-            name=name,
-            base_storage_directory=self._base_storage_directory,
+        resource_client = await get_or_create_inner(
             memory_storage_client=self._memory_storage_client,
+            base_storage_directory=self._base_storage_directory,
+            storage_client_cache=self._storage_client_cache,
+            resource_client_class=RequestQueueClient,
+            name=name,
+            id=id,
         )
-        storage_client_cache.append(new_resource)
+        return resource_client.resource_info
 
-        # Write to the disk
-        await persist_metadata_if_enabled(
-            data=new_resource.resource_info.model_dump(),
-            entity_directory=new_resource.resource_directory,  # type: ignore
-            write_metadata=self._memory_storage_client.write_metadata,
+    @override
+    async def list(
+        self,
+        *,
+        unnamed: bool = False,
+        limit: int | None = None,
+        offset: int | None = None,
+        desc: bool = False,
+    ) -> RequestQueueListPage:
+        items = [storage.resource_info for storage in self._storage_client_cache]
+
+        return RequestQueueListPage(
+            total=len(items),
+            count=len(items),
+            offset=0,
+            limit=len(items),
+            desc=False,
+            items=sorted(items, key=lambda item: item.created_at),
         )
-
-        return new_resource.resource_info
```

### Comparing `crawlee-0.0.3b9/src/crawlee/memory_storage_client/dataset_client.py` & `crawlee-0.0.4b1/src/crawlee/memory_storage_client/dataset_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,28 +10,28 @@
 import aiofiles
 import aioshutil
 from aiofiles.os import makedirs
 from typing_extensions import override
 
 from crawlee._utils.crypto import crypto_random_object_id
 from crawlee._utils.data_processing import raise_on_duplicate_storage, raise_on_non_existing_storage
-from crawlee._utils.file import force_rename, json_dumps, persist_metadata_if_enabled
+from crawlee._utils.file import force_rename, json_dumps
 from crawlee.base_storage_client import BaseDatasetClient
-from crawlee.memory_storage_client.base_resource_client import BaseResourceClient as BaseMemoryResourceClient
-from crawlee.storages.models import DatasetItemsListPage, DatasetMetadata
+from crawlee.consts import DATASET_LABEL
+from crawlee.models import DatasetItemsListPage, DatasetMetadata
 from crawlee.types import StorageTypes
 
 if TYPE_CHECKING:
     from crawlee.memory_storage_client import MemoryStorageClient
     from crawlee.types import JSONSerializable
 
 logger = getLogger(__name__)
 
 
-class DatasetClient(BaseDatasetClient, BaseMemoryResourceClient):
+class DatasetClient(BaseDatasetClient):
     """Subclient for manipulating a single dataset."""
 
     _LIST_ITEMS_LIMIT = 999_999_999_999
     """This is what API returns in the x-apify-pagination-limit header when no limit query parameter is used."""
 
     _LOCAL_ENTRY_NAME_DIGITS = 9
     """Number of characters of the dataset item file names, e.g.: 000000019.json - 9 digits."""
@@ -52,108 +52,63 @@
         self._memory_storage_client = memory_storage_client
         self.id = id or crypto_random_object_id()
         self.name = name
         self._created_at = created_at or datetime.now(timezone.utc)
         self._accessed_at = accessed_at or datetime.now(timezone.utc)
         self._modified_at = modified_at or datetime.now(timezone.utc)
 
-        self.resource_directory = os.path.join(self._base_storage_directory, self.name or self.id)
         self.dataset_entries: dict[str, dict] = {}
         self.file_operation_lock = asyncio.Lock()
         self.item_count = item_count
 
     @property
-    @override
     def resource_info(self) -> DatasetMetadata:
         """Get the resource info for the dataset client."""
         return DatasetMetadata(
-            id=str(self.id),
-            name=str(self.name),
+            id=self.id,
+            name=self.name,
             accessed_at=self._accessed_at,
             created_at=self._created_at,
             modified_at=self._modified_at,
             item_count=self.item_count,
         )
 
-    @classmethod
-    @override
-    def _get_storages_dir(cls, memory_storage_client: MemoryStorageClient) -> str:
-        return memory_storage_client.datasets_directory
-
-    @classmethod
-    @override
-    def _get_storage_client_cache(
-        cls,
-        memory_storage_client: MemoryStorageClient,
-    ) -> list[DatasetClient]:
-        return memory_storage_client.datasets_handled
+    @property
+    def resource_directory(self) -> str:
+        """Get the resource directory for the client."""
+        return os.path.join(self._base_storage_directory, self.name or self.id)
 
     @classmethod
-    @override
-    def _create_from_directory(
+    def find_or_create_client_by_id_or_name(
         cls,
-        storage_directory: str,
         memory_storage_client: MemoryStorageClient,
         id: str | None = None,
         name: str | None = None,
-    ) -> DatasetClient:
-        item_count = 0
-        created_at = datetime.now(timezone.utc)
-        accessed_at = datetime.now(timezone.utc)
-        modified_at = datetime.now(timezone.utc)
-
-        # Load metadata if it exists
-        metadata_filepath = os.path.join(storage_directory, '__metadata__.json')
-
-        if os.path.exists(metadata_filepath):
-            with open(metadata_filepath, encoding='utf-8') as f:
-                json_content = json.load(f)
-                resource_info = DatasetMetadata(**json_content)
-
-            id = resource_info.id
-            name = resource_info.name
-            item_count = resource_info.item_count
-            created_at = resource_info.created_at
-            accessed_at = resource_info.accessed_at
-            modified_at = resource_info.modified_at
-
-        # Load dataset entries
-        entries: dict[str, dict] = {}
-        has_seen_metadata_file = False
-
-        for entry in os.scandir(storage_directory):
-            if entry.is_file():
-                if entry.name == '__metadata__.json':
-                    has_seen_metadata_file = True
-                    continue
-
-                with open(os.path.join(storage_directory, entry.name), encoding='utf-8') as f:
-                    entry_content = json.load(f)
-
-                entry_name = entry.name.split('.')[0]
-                entries[entry_name] = entry_content
-
-                if not has_seen_metadata_file:
-                    item_count += 1
-
-        # Create new dataset client
-        new_client = DatasetClient(
-            base_storage_directory=memory_storage_client.datasets_directory,
+    ) -> DatasetClient | None:
+        """Restore existing or create a new dataset client based on the given ID or name.
+
+        Args:
+            memory_storage_client: The memory storage client used to store and retrieve dataset client.
+            id: The unique identifier for the dataset client.
+            name: The name of the dataset client.
+
+        Returns:
+            The found or created dataset client, or None if no client could be found or created.
+        """
+        from crawlee.memory_storage_client._creation_management import find_or_create_client_by_id_or_name_inner
+
+        return find_or_create_client_by_id_or_name_inner(
+            resource_label=DATASET_LABEL,
+            storage_client_cache=memory_storage_client.datasets_handled,
+            storages_dir=memory_storage_client.datasets_directory,
             memory_storage_client=memory_storage_client,
             id=id,
             name=name,
-            created_at=created_at,
-            accessed_at=accessed_at,
-            modified_at=modified_at,
-            item_count=item_count,
         )
 
-        new_client.dataset_entries.update(entries)
-        return new_client
-
     @override
     async def get(self) -> DatasetMetadata | None:
         found = self.find_or_create_client_by_id_or_name(
             memory_storage_client=self._memory_storage_client,
             id=self.id,
             name=self.name,
         )
@@ -191,21 +146,16 @@
                 ),
                 None,
             )
 
             if existing_dataset_by_name is not None:
                 raise_on_duplicate_storage(StorageTypes.DATASET, 'name', name)
 
-            existing_dataset_by_id.name = name
-
             previous_dir = existing_dataset_by_id.resource_directory
-
-            existing_dataset_by_id.resource_directory = os.path.join(
-                self._memory_storage_client.datasets_directory, name
-            )
+            existing_dataset_by_id.name = name
 
             await force_rename(previous_dir, existing_dataset_by_id.resource_directory)
 
             # Update timestamps
             await existing_dataset_by_id.update_timestamps(has_been_modified=True)
 
         return existing_dataset_by_id.resource_info
@@ -319,47 +269,47 @@
     @override
     async def get_items_as_bytes(
         self,
         *,
         item_format: str = 'json',
         offset: int | None = None,
         limit: int | None = None,
-        desc: bool | None = None,
-        clean: bool | None = None,
-        bom: bool | None = None,
+        desc: bool = False,
+        clean: bool = False,
+        bom: bool = False,
         delimiter: str | None = None,
         fields: list[str] | None = None,
         omit: list[str] | None = None,
         unwind: str | None = None,
-        skip_empty: bool | None = None,
-        skip_header_row: bool | None = None,
-        skip_hidden: bool | None = None,
+        skip_empty: bool = False,
+        skip_header_row: bool = False,
+        skip_hidden: bool = False,
         xml_root: str | None = None,
         xml_row: str | None = None,
         flatten: list[str] | None = None,
     ) -> bytes:
         raise NotImplementedError('This method is not supported in memory storage.')
 
     @override
     async def stream_items(
         self,
         *,
         item_format: str = 'json',
         offset: int | None = None,
         limit: int | None = None,
-        desc: bool | None = None,
-        clean: bool | None = None,
-        bom: bool | None = None,
+        desc: bool = False,
+        clean: bool = False,
+        bom: bool = False,
         delimiter: str | None = None,
         fields: list[str] | None = None,
         omit: list[str] | None = None,
         unwind: str | None = None,
-        skip_empty: bool | None = None,
-        skip_header_row: bool | None = None,
-        skip_hidden: bool | None = None,
+        skip_empty: bool = False,
+        skip_header_row: bool = False,
+        skip_hidden: bool = False,
         xml_root: str | None = None,
         xml_row: str | None = None,
     ) -> AsyncIterator:
         raise NotImplementedError('This method is not supported in memory storage.')
 
     @override
     async def push_items(
@@ -428,14 +378,16 @@
             file_path = os.path.join(entity_directory, f'{idx}.json')
             async with aiofiles.open(file_path, mode='wb') as f:
                 s = await json_dumps(item)
                 await f.write(s.encode('utf-8'))
 
     async def update_timestamps(self, *, has_been_modified: bool) -> None:
         """Update the timestamps of the dataset."""
+        from crawlee.memory_storage_client._creation_management import persist_metadata_if_enabled
+
         self._accessed_at = datetime.now(timezone.utc)
 
         if has_been_modified:
             self._modified_at = datetime.now(timezone.utc)
 
         await persist_metadata_if_enabled(
             data=self.resource_info.model_dump(),
```

### Comparing `crawlee-0.0.3b9/src/crawlee/memory_storage_client/dataset_collection_client.py` & `crawlee-0.0.4b1/src/crawlee/memory_storage_client/dataset_collection_client.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,45 +1,69 @@
 from __future__ import annotations
 
+from typing import TYPE_CHECKING
+
 from typing_extensions import override
 
 from crawlee.base_storage_client import BaseDatasetCollectionClient
-from crawlee.memory_storage_client.base_resource_collection_client import (
-    BaseResourceCollectionClient as BaseMemoryResourceCollectionClient,
-)
+from crawlee.memory_storage_client._creation_management import get_or_create_inner
 from crawlee.memory_storage_client.dataset_client import DatasetClient
-from crawlee.storages.models import DatasetListPage
+from crawlee.models import DatasetListPage, DatasetMetadata
+
+if TYPE_CHECKING:
+    from crawlee.memory_storage_client.memory_storage_client import MemoryStorageClient
 
 
-class DatasetCollectionClient(  # type: ignore
-    BaseMemoryResourceCollectionClient,
-    BaseDatasetCollectionClient,
-):
+class DatasetCollectionClient(BaseDatasetCollectionClient):
     """Subclient for manipulating datasets."""
 
+    def __init__(
+        self,
+        *,
+        base_storage_directory: str,
+        memory_storage_client: MemoryStorageClient,
+    ) -> None:
+        self._base_storage_directory = base_storage_directory
+        self._memory_storage_client = memory_storage_client
+
     @property
-    @override
-    def _client_class(self) -> type[DatasetClient]:
-        return DatasetClient
+    def _storage_client_cache(self) -> list[DatasetClient]:
+        return self._memory_storage_client.datasets_handled
 
     @override
-    def _get_storage_client_cache(self) -> list[DatasetClient]:
-        return self._memory_storage_client.datasets_handled
+    async def get_or_create(
+        self,
+        *,
+        name: str | None = None,
+        schema: dict | None = None,
+        id: str | None = None,
+    ) -> DatasetMetadata:
+        if name is None and id is None:
+            id = self._memory_storage_client.default_storage_id
+
+        resource_client = await get_or_create_inner(
+            memory_storage_client=self._memory_storage_client,
+            base_storage_directory=self._base_storage_directory,
+            storage_client_cache=self._storage_client_cache,
+            resource_client_class=DatasetClient,
+            name=name,
+            id=id,
+        )
+        return resource_client.resource_info
 
     @override
     async def list(
         self,
         *,
-        unnamed: bool | None = None,
+        unnamed: bool = False,
         limit: int | None = None,
         offset: int | None = None,
-        desc: bool | None = None,
+        desc: bool = False,
     ) -> DatasetListPage:
-        storage_client_cache = self._get_storage_client_cache()
-        items = [storage.resource_info for storage in storage_client_cache]
+        items = [storage.resource_info for storage in self._storage_client_cache]
 
         return DatasetListPage(
             total=len(items),
             count=len(items),
             offset=0,
             limit=len(items),
             desc=False,
```

### Comparing `crawlee-0.0.3b9/src/crawlee/memory_storage_client/key_value_store_client.py` & `crawlee-0.0.4b1/src/crawlee/memory_storage_client/key_value_store_client.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,52 +1,46 @@
 from __future__ import annotations
 
 import asyncio
 import io
-import json
-import mimetypes
 import os
-import pathlib
 from datetime import datetime, timezone
 from logging import getLogger
 from typing import TYPE_CHECKING, Any, AsyncIterator
 
 import aiofiles
 import aioshutil
 from aiofiles.os import makedirs
 from typing_extensions import override
 
 from crawlee._utils.crypto import crypto_random_object_id
 from crawlee._utils.data_processing import maybe_parse_body, raise_on_duplicate_storage, raise_on_non_existing_storage
-from crawlee._utils.file import (
-    determine_file_extension,
-    force_remove,
-    force_rename,
-    is_file_or_bytes,
-    json_dumps,
+from crawlee._utils.file import determine_file_extension, force_remove, force_rename, is_file_or_bytes, json_dumps
+from crawlee.base_storage_client import BaseKeyValueStoreClient
+from crawlee.consts import KEY_VALUE_STORE_LABEL
+from crawlee.memory_storage_client._creation_management import (
+    find_or_create_client_by_id_or_name_inner,
     persist_metadata_if_enabled,
 )
-from crawlee.base_storage_client import BaseKeyValueStoreClient
-from crawlee.memory_storage_client.base_resource_client import BaseResourceClient as MemoryBaseResourceClient
-from crawlee.storages.models import (
+from crawlee.models import (
     KeyValueStoreKeyInfo,
     KeyValueStoreListKeysPage,
     KeyValueStoreMetadata,
     KeyValueStoreRecord,
     KeyValueStoreRecordMetadata,
 )
 from crawlee.types import StorageTypes
 
 if TYPE_CHECKING:
     from crawlee.memory_storage_client import MemoryStorageClient
 
 logger = getLogger(__name__)
 
 
-class KeyValueStoreClient(BaseKeyValueStoreClient, MemoryBaseResourceClient):
+class KeyValueStoreClient(BaseKeyValueStoreClient):
     """Subclient for manipulating a single key-value store."""
 
     def __init__(
         self,
         *,
         base_storage_directory: str,
         memory_storage_client: MemoryStorageClient,
@@ -61,137 +55,60 @@
 
         self._base_storage_directory = base_storage_directory
         self._memory_storage_client = memory_storage_client
         self._created_at = created_at or datetime.now(timezone.utc)
         self._accessed_at = accessed_at or datetime.now(timezone.utc)
         self._modified_at = modified_at or datetime.now(timezone.utc)
 
-        self.resource_directory = os.path.join(base_storage_directory, self.name or self.id)
         self.records: dict[str, KeyValueStoreRecord] = {}
         self.file_operation_lock = asyncio.Lock()
 
     @property
-    @override
     def resource_info(self) -> KeyValueStoreMetadata:
         """Get the resource info for the key-value store client."""
         return KeyValueStoreMetadata(
-            id=str(self.id),
-            name=str(self.name),
+            id=self.id,
+            name=self.name,
             accessed_at=self._accessed_at,
             created_at=self._created_at,
             modified_at=self._modified_at,
             user_id='1',
         )
 
-    @classmethod
-    @override
-    def _get_storages_dir(cls, memory_storage_client: MemoryStorageClient) -> str:
-        return memory_storage_client.key_value_stores_directory
-
-    @classmethod
-    @override
-    def _get_storage_client_cache(cls, memory_storage_client: MemoryStorageClient) -> list[KeyValueStoreClient]:
-        return memory_storage_client.key_value_stores_handled
+    @property
+    def resource_directory(self) -> str:
+        """Get the resource directory for the client."""
+        return os.path.join(self._base_storage_directory, self.name or self.id)
 
     @classmethod
-    @override
-    def _create_from_directory(
+    def find_or_create_client_by_id_or_name(
         cls,
-        storage_directory: str,
         memory_storage_client: MemoryStorageClient,
         id: str | None = None,
         name: str | None = None,
-    ) -> KeyValueStoreClient:
-        created_at = datetime.now(timezone.utc)
-        accessed_at = datetime.now(timezone.utc)
-        modified_at = datetime.now(timezone.utc)
-
-        # Load metadata if it exists
-        metadata_filepath = os.path.join(storage_directory, '__metadata__.json')
-
-        if os.path.exists(metadata_filepath):
-            with open(metadata_filepath, encoding='utf-8') as f:
-                json_content = json.load(f)
-                resource_info = KeyValueStoreMetadata(**json_content)
-
-            id = resource_info.id
-            name = resource_info.name
-            created_at = resource_info.created_at
-            accessed_at = resource_info.accessed_at
-            modified_at = resource_info.modified_at
-
-        # Create new KVS client
-        new_client = KeyValueStoreClient(
-            base_storage_directory=memory_storage_client.key_value_stores_directory,
+    ) -> KeyValueStoreClient | None:
+        """Restore existing or create a new key-value store client based on the given ID or name.
+
+        Args:
+            memory_storage_client: The memory storage client used to store and retrieve key-value store client.
+            id: The unique identifier for the key-value store client.
+            name: The name of the key-value store client.
+
+        Returns:
+            The found or created key-value store client, or None if no client could be found or created.
+        """
+        return find_or_create_client_by_id_or_name_inner(
+            resource_label=KEY_VALUE_STORE_LABEL,
+            storage_client_cache=memory_storage_client.key_value_stores_handled,
+            storages_dir=memory_storage_client.key_value_stores_directory,
             memory_storage_client=memory_storage_client,
             id=id,
             name=name,
-            accessed_at=accessed_at,
-            created_at=created_at,
-            modified_at=modified_at,
         )
 
-        # Scan the KVS folder, check each entry in there and parse it as a store record
-        for entry in os.scandir(storage_directory):
-            if not entry.is_file():
-                continue
-
-            # Ignore metadata files on their own
-            if entry.name.endswith('__metadata__.json'):
-                continue
-
-            # Try checking if this file has a metadata file associated with it
-            record_metadata = None
-            record_metadata_filepath = os.path.join(storage_directory, f'{entry.name}.__metadata__.json')
-
-            if os.path.exists(record_metadata_filepath):
-                with open(record_metadata_filepath, encoding='utf-8') as metadata_file:
-                    try:
-                        json_content = json.load(metadata_file)
-                        record_metadata = KeyValueStoreRecordMetadata(**json_content)
-
-                    except Exception:
-                        logger.warning(
-                            f'Metadata of key-value store entry "{entry.name}" for store {name or id} could '
-                            'not be parsed. The metadata file will be ignored.',
-                            exc_info=True,
-                        )
-
-            if not record_metadata:
-                content_type, _ = mimetypes.guess_type(entry.name)
-                if content_type is None:
-                    content_type = 'application/octet-stream'
-
-                record_metadata = KeyValueStoreRecordMetadata(
-                    key=pathlib.Path(entry.name).stem,
-                    content_type=content_type,
-                )
-
-            with open(os.path.join(storage_directory, entry.name), 'rb') as f:
-                file_content = f.read()
-
-            try:
-                maybe_parse_body(file_content, record_metadata.content_type)
-            except Exception:
-                record_metadata.content_type = 'application/octet-stream'
-                logger.warning(
-                    f'Key-value store entry "{record_metadata.key}" for store {name or id} could not be parsed.'
-                    'The entry will be assumed as binary.',
-                    exc_info=True,
-                )
-
-            new_client.records[record_metadata.key] = KeyValueStoreRecord(
-                key=record_metadata.key,
-                content_type=record_metadata.content_type,
-                filename=entry.name,
-                value=file_content,
-            )
-
-        return new_client
-
     @override
     async def get(self) -> KeyValueStoreMetadata | None:
         found = self.find_or_create_client_by_id_or_name(
             memory_storage_client=self._memory_storage_client,
             id=self.id,
             name=self.name,
         )
@@ -229,22 +146,16 @@
                 ),
                 None,
             )
 
             if existing_store_by_name is not None:
                 raise_on_duplicate_storage(StorageTypes.KEY_VALUE_STORE, 'name', name)
 
-            existing_store_by_id.name = name
-
             previous_dir = existing_store_by_id.resource_directory
-
-            existing_store_by_id.resource_directory = os.path.join(
-                self._memory_storage_client.key_value_stores_directory,
-                name,
-            )
+            existing_store_by_id.name = name
 
             await force_rename(previous_dir, existing_store_by_id.resource_directory)
 
             # Update timestamps
             await existing_store_by_id.update_timestamps(has_been_modified=True)
 
         return existing_store_by_id.resource_info
```

### Comparing `crawlee-0.0.3b9/src/crawlee/memory_storage_client/memory_storage_client.py` & `crawlee-0.0.4b1/src/crawlee/memory_storage_client/memory_storage_client.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 from __future__ import annotations
 
 import asyncio
 import contextlib
 import os
+from logging import getLogger
 from pathlib import Path
 
 import aioshutil
 from aiofiles import ospath
 from aiofiles.os import rename, scandir
 from typing_extensions import override
 
-from crawlee._utils.data_processing import maybe_parse_bool
-from crawlee._utils.env_vars import CrawleeEnvVars
 from crawlee.base_storage_client import BaseStorageClient
+from crawlee.configuration import Configuration
+from crawlee.memory_storage_client.dataset_client import DatasetClient
+from crawlee.memory_storage_client.dataset_collection_client import DatasetCollectionClient
+from crawlee.memory_storage_client.key_value_store_client import KeyValueStoreClient
+from crawlee.memory_storage_client.key_value_store_collection_client import KeyValueStoreCollectionClient
+from crawlee.memory_storage_client.request_queue_client import RequestQueueClient
+from crawlee.memory_storage_client.request_queue_collection_client import RequestQueueCollectionClient
 
-from .dataset_client import DatasetClient
-from .dataset_collection_client import DatasetCollectionClient
-from .key_value_store_client import KeyValueStoreClient
-from .key_value_store_collection_client import KeyValueStoreCollectionClient
-from .request_queue_client import RequestQueueClient
-from .request_queue_collection_client import RequestQueueCollectionClient
+logger = getLogger(__name__)
 
 
 class MemoryStorageClient(BaseStorageClient):
     """Represents an in-memory storage client for managing datasets, key-value stores, and request queues.
 
     It emulates in-memory storage similar to the Apify platform, supporting both in-memory and local file system-based
     persistence.
@@ -34,61 +35,63 @@
 
     _MIGRATING_KEY_VALUE_STORE_DIR_NAME = '__CRAWLEE_MIGRATING_KEY_VALUE_STORE'
     """Name of the directory used to temporarily store files during the migration of the default key-value store."""
 
     _TEMPORARY_DIR_NAME = '__CRAWLEE_TEMPORARY'
     """Name of the directory used to temporarily store files during purges."""
 
-    def __init__(
-        self,
-        *,
-        local_data_directory: str | None = None,
-        write_metadata: bool | None = None,
-        persist_storage: bool | None = None,
-    ) -> None:
+    def __init__(self, configuration: Configuration | None = None) -> None:
         """Create a new instance.
 
         Args:
-            local_data_directory: Path to the local directory where data will be persisted. If None, defaults to
-                CrawleeEnvVars.LOCAL_STORAGE_DIR or './storage'.
-
-            write_metadata: Flag indicating whether to write metadata for the storages. Defaults based on DEBUG
-                environment variable.
-
-            persist_storage: Flag indicating whether to persist the storage data locally. Defaults based on
-                CrawleeEnvVars.PERSIST_STORAGE.
+            configuration: Configuration object to use. If None, a default Configuration object will be created.
         """
-        self._local_data_directory = local_data_directory or os.getenv(CrawleeEnvVars.LOCAL_STORAGE_DIR) or './storage'
-        self.write_metadata = write_metadata if write_metadata is not None else '*' in os.getenv('DEBUG', '')
-        self.persist_storage = (
-            persist_storage
-            if persist_storage is not None
-            else maybe_parse_bool(os.getenv(CrawleeEnvVars.PERSIST_STORAGE, 'true'))
-        )
+        self._configuration = configuration or Configuration()
 
-        self._purged_on_start = False  # Indicates whether a purge was already performed on this instance.
         self.datasets_handled: list[DatasetClient] = []
         self.key_value_stores_handled: list[KeyValueStoreClient] = []
         self.request_queues_handled: list[RequestQueueClient] = []
+
+        self._purged_on_start = False  # Indicates whether a purge was already performed on this instance.
         self._purge_lock = asyncio.Lock()
 
     @property
+    def default_storage_id(self) -> str:
+        """The ID of the default storage."""
+        return self._configuration.default_storage_id
+
+    @property
+    def write_metadata(self) -> bool:
+        """Whether to write metadata to the storage."""
+        return self._configuration.write_metadata
+
+    @property
+    def persist_storage(self) -> bool:
+        """Whether to persist the storage."""
+        return self._configuration.persist_storage
+
+    @property
+    def storage_dir(self) -> str:
+        """Path to the storage directory."""
+        return self._configuration.local_storage_dir
+
+    @property
     def datasets_directory(self) -> str:
         """Path to the directory containing datasets."""
-        return os.path.join(self._local_data_directory, 'datasets')
+        return os.path.join(self.storage_dir, 'datasets')
 
     @property
     def key_value_stores_directory(self) -> str:
         """Path to the directory containing key-value stores."""
-        return os.path.join(self._local_data_directory, 'key_value_stores')
+        return os.path.join(self.storage_dir, 'key_value_stores')
 
     @property
     def request_queues_directory(self) -> str:
         """Path to the directory containing request queues."""
-        return os.path.join(self._local_data_directory, 'request_queues')
+        return os.path.join(self.storage_dir, 'request_queues')
 
     @override
     def dataset(self, id: str) -> DatasetClient:
         return DatasetClient(
             base_storage_directory=self.datasets_directory,
             memory_storage_client=self,
             id=id,
@@ -127,34 +130,31 @@
     @override
     def request_queues(self) -> RequestQueueCollectionClient:
         return RequestQueueCollectionClient(
             base_storage_directory=self.request_queues_directory,
             memory_storage_client=self,
         )
 
+    @override
     async def purge_on_start(self) -> None:
-        """Performs a purge of the default storage directories.
-
-        This method ensures that the purge is executed only once during the lifetime of the instance.
-        It is primarily used to clean up residual data from previous runs to maintain a clean state.
-        """
         # Optimistic, non-blocking check
         if self._purged_on_start is True:
+            logger.debug('Storage was already purged on start.')
             return
 
         async with self._purge_lock:
             # Another check under the lock just to be sure
             if self._purged_on_start is True:
                 # Mypy doesn't understand that the _purged_on_start can change while we're getting the async lock
                 return  # type: ignore[unreachable]
 
-            await self._purge_inner()
+            await self._purge_default_storages()
             self._purged_on_start = True
 
-    async def _purge_inner(self) -> None:
+    async def _purge_default_storages(self) -> None:
         """Cleans up the storage directories, preparing the environment for a new run.
 
         It aims to remove residues from previous executions to avoid data contamination between runs.
 
         It specifically targets:
          - The local directory containing the default dataset.
          - All records from the default key-value store in the local directory, except for the 'INPUT' key.
@@ -164,29 +164,31 @@
         if await ospath.exists(self.key_value_stores_directory):
             key_value_store_folders = await scandir(self.key_value_stores_directory)
             for key_value_store_folder in key_value_store_folders:
                 if key_value_store_folder.name.startswith(
                     self._TEMPORARY_DIR_NAME
                 ) or key_value_store_folder.name.startswith('__OLD'):
                     await self._batch_remove_files(key_value_store_folder.path)
-                elif key_value_store_folder.name == 'default':
+                elif key_value_store_folder.name == self.default_storage_id:
                     await self._handle_default_key_value_store(key_value_store_folder.path)
 
         # Datasets
         if await ospath.exists(self.datasets_directory):
             dataset_folders = await scandir(self.datasets_directory)
             for dataset_folder in dataset_folders:
-                if dataset_folder.name == 'default' or dataset_folder.name.startswith(self._TEMPORARY_DIR_NAME):
+                if dataset_folder.name == self.default_storage_id or dataset_folder.name.startswith(
+                    self._TEMPORARY_DIR_NAME
+                ):
                     await self._batch_remove_files(dataset_folder.path)
 
         # Request queues
         if await ospath.exists(self.request_queues_directory):
             request_queue_folders = await scandir(self.request_queues_directory)
             for request_queue_folder in request_queue_folders:
-                if request_queue_folder.name == 'default' or request_queue_folder.name.startswith(
+                if request_queue_folder.name == self.default_storage_id or request_queue_folder.name.startswith(
                     self._TEMPORARY_DIR_NAME
                 ):
                     await self._batch_remove_files(request_queue_folder.path)
 
     async def _handle_default_key_value_store(self, folder: str) -> None:
         """Manages the cleanup of the default key-value store.
```

### Comparing `crawlee-0.0.3b9/src/crawlee/memory_storage_client/request_queue_client.py` & `crawlee-0.0.4b1/src/crawlee/memory_storage_client/request_queue_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,27 +15,30 @@
 
 from crawlee._utils.crypto import crypto_random_object_id
 from crawlee._utils.data_processing import (
     filter_out_none_values_recursively,
     raise_on_duplicate_storage,
     raise_on_non_existing_storage,
 )
-from crawlee._utils.file import force_remove, force_rename, json_dumps, persist_metadata_if_enabled
+from crawlee._utils.file import force_remove, force_rename, json_dumps
 from crawlee._utils.requests import unique_key_to_request_id
 from crawlee.base_storage_client import BaseRequestQueueClient
-from crawlee.memory_storage_client.base_resource_client import BaseResourceClient
-from crawlee.request import Request
-from crawlee.storages.models import RequestQueueHead, RequestQueueMetadata, RequestQueueOperationInfo
+from crawlee.consts import REQUEST_QUEUE_LABEL
+from crawlee.memory_storage_client._creation_management import (
+    find_or_create_client_by_id_or_name_inner,
+    persist_metadata_if_enabled,
+)
+from crawlee.models import Request, RequestQueueHead, RequestQueueMetadata, RequestQueueOperationInfo
 from crawlee.types import StorageTypes
 
 if TYPE_CHECKING:
     from crawlee.memory_storage_client import MemoryStorageClient
 
 
-class RequestQueueClient(BaseRequestQueueClient, BaseResourceClient):
+class RequestQueueClient(BaseRequestQueueClient):
     """Subclient for manipulating a single request queue."""
 
     def __init__(
         self,
         *,
         base_storage_directory: str,
         memory_storage_client: MemoryStorageClient,
@@ -53,113 +56,67 @@
         self.name = name
         self._created_at = created_at or datetime.now(timezone.utc)
         self._accessed_at = accessed_at or datetime.now(timezone.utc)
         self._modified_at = modified_at or datetime.now(timezone.utc)
         self.handled_request_count = handled_request_count
         self.pending_request_count = pending_request_count
 
-        self.resource_directory = os.path.join(base_storage_directory, name or self.id)
         self.requests = ValueSortedDict(lambda request: request.order_no or -float('inf'))
         self.file_operation_lock = asyncio.Lock()
         self._last_used_timestamp = Decimal(0.0)
 
     @property
-    @override
     def resource_info(self) -> RequestQueueMetadata:
         """Get the resource info for the request queue client."""
         return RequestQueueMetadata(
-            id=str(self.id),
-            name=str(self.name),
+            id=self.id,
+            name=self.name,
             accessed_at=self._accessed_at,
             created_at=self._created_at,
             modified_at=self._modified_at,
             had_multiple_clients=False,
             handled_request_count=self.handled_request_count,
             pending_request_count=self.pending_request_count,
             stats={},
             total_request_count=len(self.requests),
             user_id='1',
             resource_directory=self.resource_directory,
         )
 
-    @classmethod
-    @override
-    def _get_storages_dir(cls, memory_storage_client: MemoryStorageClient) -> str:
-        return memory_storage_client.request_queues_directory
-
-    @classmethod
-    @override
-    def _get_storage_client_cache(cls, memory_storage_client: MemoryStorageClient) -> list[RequestQueueClient]:
-        return memory_storage_client.request_queues_handled
+    @property
+    def resource_directory(self) -> str:
+        """Get the resource directory for the client."""
+        return os.path.join(self._base_storage_directory, self.name or self.id)
 
     @classmethod
-    @override
-    def _create_from_directory(
+    def find_or_create_client_by_id_or_name(
         cls,
-        storage_directory: str,
         memory_storage_client: MemoryStorageClient,
         id: str | None = None,
         name: str | None = None,
-    ) -> RequestQueueClient:
-        created_at = datetime.now(timezone.utc)
-        accessed_at = datetime.now(timezone.utc)
-        modified_at = datetime.now(timezone.utc)
-        handled_request_count = 0
-        pending_request_count = 0
-
-        # Load metadata if it exists
-        metadata_filepath = os.path.join(storage_directory, '__metadata__.json')
-
-        if os.path.exists(metadata_filepath):
-            with open(metadata_filepath, encoding='utf-8') as f:
-                json_content = json.load(f)
-                resource_info = RequestQueueMetadata(**json_content)
-
-            id = resource_info.id
-            name = resource_info.name
-            created_at = resource_info.created_at
-            accessed_at = resource_info.accessed_at
-            modified_at = resource_info.modified_at
-            handled_request_count = resource_info.handled_request_count
-            pending_request_count = resource_info.pending_request_count
-
-        # Load request entries
-        entries: dict[str, Request] = {}
-
-        for entry in os.scandir(storage_directory):
-            if entry.is_file():
-                if entry.name == '__metadata__.json':
-                    continue
-
-                with open(os.path.join(storage_directory, entry.name), encoding='utf-8') as f:
-                    content = json.load(f)
-
-                request = Request(**content)
-                order_no = request.order_no
-                if order_no:
-                    request.order_no = Decimal(order_no)
-
-                entries[request.id] = request
-
-        # Create new RQ client
-        new_client = RequestQueueClient(
-            base_storage_directory=memory_storage_client.request_queues_directory,
+    ) -> RequestQueueClient | None:
+        """Restore existing or create a new key-value store client based on the given ID or name.
+
+        Args:
+            memory_storage_client: The memory storage client used to store and retrieve key-value store client.
+            id: The unique identifier for the key-value store client.
+            name: The name of the key-value store client.
+
+        Returns:
+            The found or created key-value store client, or None if no client could be found or created.
+        """
+        return find_or_create_client_by_id_or_name_inner(
+            resource_label=REQUEST_QUEUE_LABEL,
+            storage_client_cache=memory_storage_client.request_queues_handled,
+            storages_dir=memory_storage_client.request_queues_directory,
             memory_storage_client=memory_storage_client,
             id=id,
             name=name,
-            accessed_at=accessed_at,
-            created_at=created_at,
-            modified_at=modified_at,
-            handled_request_count=handled_request_count,
-            pending_request_count=pending_request_count,
         )
 
-        new_client.requests.update(entries)
-        return new_client
-
     @override
     async def get(self) -> RequestQueueMetadata | None:
         found = self.find_or_create_client_by_id_or_name(
             memory_storage_client=self._memory_storage_client,
             id=self.id,
             name=self.name,
         )
@@ -197,20 +154,16 @@
                 ),
                 None,
             )
 
             if existing_queue_by_name is not None:
                 raise_on_duplicate_storage(StorageTypes.REQUEST_QUEUE, 'name', name)
 
-            existing_queue_by_id.name = name
             previous_dir = existing_queue_by_id.resource_directory
-            existing_queue_by_id.resource_directory = os.path.join(
-                self._memory_storage_client.request_queues_directory,
-                name,
-            )
+            existing_queue_by_id.name = name
 
             await force_rename(previous_dir, existing_queue_by_id.resource_directory)
 
             # Update timestamps
             await existing_queue_by_id.update_timestamps(has_been_modified=True)
 
             return existing_queue_by_id.resource_info
@@ -278,15 +231,15 @@
         raise NotImplementedError('This method is not supported in memory storage.')
 
     @override
     async def add_request(
         self,
         request: Request,
         *,
-        forefront: bool | None = None,
+        forefront: bool = False,
     ) -> RequestQueueOperationInfo:
         existing_queue_by_id = self.find_or_create_client_by_id_or_name(
             memory_storage_client=self._memory_storage_client,
             id=self.id,
             name=self.name,
         )
 
@@ -348,15 +301,15 @@
             return self._json_to_request(request.json_ if request is not None else None)
 
     @override
     async def update_request(
         self,
         request: Request,
         *,
-        forefront: bool | None = None,
+        forefront: bool = False,
     ) -> RequestQueueOperationInfo:
         existing_queue_by_id = self.find_or_create_client_by_id_or_name(
             memory_storage_client=self._memory_storage_client,
             id=self.id,
             name=self.name,
         )
```

### Comparing `crawlee-0.0.3b9/src/crawlee/sessions/models.py` & `crawlee-0.0.4b1/src/crawlee/sessions/models.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b9/src/crawlee/sessions/session.py` & `crawlee-0.0.4b1/src/crawlee/sessions/session.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b9/src/crawlee/sessions/session_pool.py` & `crawlee-0.0.4b1/src/crawlee/sessions/session_pool.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b9/src/crawlee/storage_client_manager.py` & `crawlee-0.0.4b1/src/crawlee/storage_client_manager.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,54 +1,50 @@
 from __future__ import annotations
 
-from typing import Any
+from typing import TYPE_CHECKING
 
 from crawlee.memory_storage_client import MemoryStorageClient
 
+if TYPE_CHECKING:
+    from crawlee.base_storage_client import BaseStorageClient
+
 
 class StorageClientManager:
     """A class for managing storage clients."""
 
-    persist_storage: bool | None = None
-    is_at_home: bool | None = None
-
-    local_client: MemoryStorageClient | None = None
-    cloud_client: None = None
-
-    _default_instance: StorageClientManager | None = None
+    _local_client: BaseStorageClient = MemoryStorageClient()
+    _cloud_client: BaseStorageClient | None = None
 
     @classmethod
-    def get_storage_client(cls) -> MemoryStorageClient:
-        """Get the current storage client instance.
+    def get_storage_client(cls, *, in_cloud: bool = False) -> BaseStorageClient:
+        """Get the storage client instance for the current environment.
+
+        Args:
+            in_cloud: Whether the code is running in the cloud environment.
 
         Returns:
             The current storage client instance.
         """
-        default_instance = cls._get_default_instance()
-        if not default_instance.local_client:
-            default_instance.local_client = MemoryStorageClient(
-                persist_storage=default_instance.persist_storage,
-                write_metadata=True,
-            )
-
-        if default_instance.is_at_home:
-            if default_instance.cloud_client is None:
-                raise RuntimeError('Cloud client is expected but not set in the environment.')
-            return default_instance.cloud_client  # type: ignore
+        if in_cloud:
+            if cls._cloud_client is None:
+                raise RuntimeError('Running in cloud environment, but cloud client was not provided.')
+            return cls._cloud_client
 
-        return default_instance.local_client
+        return cls._local_client
 
     @classmethod
-    def set_cloud_client(cls, client: Any) -> None:
-        """Set the storage client.
+    def set_cloud_client(cls, cloud_client: BaseStorageClient) -> None:
+        """Set the cloud storage client instance.
 
         Args:
-            client: The instance of a storage client.
+            cloud_client: The cloud storage client instance.
         """
-        cls._get_default_instance().cloud_client = client
+        cls._cloud_client = cloud_client
 
     @classmethod
-    def _get_default_instance(cls) -> StorageClientManager:
-        if cls._default_instance is None:
-            cls._default_instance = cls()
+    def set_local_client(cls, local_client: BaseStorageClient) -> None:
+        """Set the local storage client instance.
 
-        return cls._default_instance
+        Args:
+            local_client: The local storage client instance.
+        """
+        cls._local_client = local_client
```

### Comparing `crawlee-0.0.3b9/src/crawlee/storages/dataset.py` & `crawlee-0.0.4b1/src/crawlee/storages/dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,22 +4,23 @@
 import io
 from typing import TYPE_CHECKING, AsyncIterator
 
 from typing_extensions import override
 
 from crawlee._utils.byte_size import ByteSize
 from crawlee._utils.file import json_dumps
+from crawlee.consts import DATASET_LABEL
+from crawlee.models import DatasetMetadata
 from crawlee.storages.base_storage import BaseStorage
 from crawlee.storages.key_value_store import KeyValueStore
-from crawlee.storages.models import DatasetMetadata
 
 if TYPE_CHECKING:
-    from crawlee.base_storage_client import BaseDatasetClient, BaseDatasetCollectionClient, BaseStorageClient
+    from crawlee.base_storage_client import BaseStorageClient
     from crawlee.configuration import Configuration
-    from crawlee.storages.models import DatasetItemsListPage
+    from crawlee.models import DatasetItemsListPage
     from crawlee.types import JSONSerializable
 
 
 class Dataset(BaseStorage):
     """Represents an append-only structured storage, ideal for tabular data akin to database tables.
 
     Represents a structured data store similar to a table, where each object (row) has consistent attributes (columns).
@@ -34,14 +35,17 @@
     dataset for the current crawler run is used. Opening a non-existent dataset by `id` raises an error, while
     by `name`, it is created.
 
     Usage:
         dataset = await Dataset.open(id='my_dataset_id')
     """
 
+    LABEL = DATASET_LABEL
+    """Human readable label of the storage."""
+
     _MAX_PAYLOAD_SIZE = ByteSize.from_mb(9)
     """Maximum size for a single payload."""
 
     _SAFETY_BUFFER_PERCENT = 0.01 / 100  # 0.01%
     """Percentage buffer to reduce payload limit slightly for safety."""
 
     _EFFECTIVE_LIMIT_SIZE = _MAX_PAYLOAD_SIZE - (_MAX_PAYLOAD_SIZE * _SAFETY_BUFFER_PERCENT)
@@ -50,36 +54,56 @@
     def __init__(
         self,
         id: str,
         name: str | None,
         configuration: Configuration,
         client: BaseStorageClient,
     ) -> None:
-        super().__init__(id=id, name=name, client=client, configuration=configuration)
-        self._dataset_client = client.dataset(self.id)
+        self._id = id
+        self._name = name
+        self._configuration = configuration
+
+        # Get resource clients from storage client
+        self._resource_client = client.dataset(self._id)
+        self._resource_collection_client = client.datasets()
 
-    @classmethod
     @override
-    def _get_human_friendly_label(cls) -> str:
-        return 'Dataset'
+    @property
+    def id(self) -> str:
+        return self._id
 
-    @classmethod
     @override
-    def _get_default_id(cls, configuration: Configuration) -> str:
-        return configuration.default_dataset_id
+    @property
+    def name(self) -> str | None:
+        return self._name
 
-    @classmethod
     @override
-    def _get_single_storage_client(cls, id: str, client: BaseStorageClient) -> BaseDatasetClient:
-        return client.dataset(id)
-
     @classmethod
+    async def open(
+        cls,
+        *,
+        id: str | None = None,
+        name: str | None = None,
+        configuration: Configuration | None = None,
+    ) -> Dataset:
+        from crawlee.storages._creation_management import open_storage
+
+        return await open_storage(
+            storage_class=cls,
+            id=id,
+            name=name,
+            configuration=configuration,
+        )
+
     @override
-    def _get_storage_collection_client(cls, client: BaseStorageClient) -> BaseDatasetCollectionClient:
-        return client.datasets()
+    async def drop(self) -> None:
+        from crawlee.storages._creation_management import remove_storage_from_cache
+
+        await self._resource_client.delete()
+        remove_storage_from_cache(storage_class_label=self.LABEL, id=self._id, name=self._name)
 
     async def push_data(self, data: JSONSerializable) -> None:
         """Store an object or an array of objects to the dataset.
 
         The size of the data is limited by the receiving API and therefore `push_data()` will only
         allow objects whose JSON representation is smaller than 9MB. When an array is passed,
         none of the included objects may be larger than 9MB, but the array itself may be of any size.
@@ -87,22 +111,22 @@
         Args:
             data: A JSON serializable data structure to be stored in the dataset.
                 The JSON representation of each item must be smaller than 9MB.
         """
         # Handle singular items
         if not isinstance(data, list):
             payload = await self._check_and_serialize(data)
-            return await self._dataset_client.push_items(payload)
+            return await self._resource_client.push_items(payload)
 
         # Handle lists
         payloads_generator = (await self._check_and_serialize(item, index) for index, item in enumerate(data))
 
         # Invoke client in series to preserve the order of data
         async for chunk in self._chunk_by_size(payloads_generator):
-            await self._dataset_client.push_items(chunk)
+            await self._resource_client.push_items(chunk)
 
         return None
 
     async def get_data(
         self,
         *,
         offset: int | None = None,
@@ -136,15 +160,15 @@
             view: Specifies the dataset view to be used.
 
         Returns:
             List page containing filtered and paginated dataset items.
         """
         # TODO: Improve error handling here
         # https://github.com/apify/apify-sdk-python/issues/140
-        return await self._dataset_client.list_items(
+        return await self._resource_client.list_items(
             offset=offset,
             limit=limit,
             desc=desc,
             clean=clean,
             fields=fields,
             omit=omit,
             unwind=unwind,
@@ -214,15 +238,15 @@
 
     async def get_info(self) -> DatasetMetadata | None:
         """Get an object containing general information about the dataset.
 
         Returns:
             Object returned by calling the GET dataset API endpoint.
         """
-        metadata = await self._dataset_client.get()
+        metadata = await self._resource_client.get()
         if isinstance(metadata, DatasetMetadata):
             return metadata
         return None
 
     async def iterate_items(
         self,
         *,
@@ -252,32 +276,27 @@
             unwind: Field name to unwind items by.
             skip_empty: Omits empty items if True.
             skip_hidden: Excludes fields starting with '#' if True.
 
         Yields:
             Each item from the dataset as a dictionary.
         """
-        async for item in self._dataset_client.iterate_items(  # type: ignore
+        async for item in self._resource_client.iterate_items(  # type: ignore
             offset=offset,
             limit=limit,
             clean=clean,
             desc=desc,
             fields=fields,
             omit=omit,
             unwind=unwind,
             skip_empty=skip_empty,
             skip_hidden=skip_hidden,
         ):
             yield item
 
-    async def drop(self) -> None:
-        """Remove the dataset either from the Apify cloud storage or from the local directory."""
-        await self._dataset_client.delete()
-        self._remove_from_cache()
-
     async def _export_to(
         self,
         key: str,
         *,
         to_key_value_store_id: str | None = None,
         to_key_value_store_name: str | None = None,
         content_type: str | None = None,
@@ -296,15 +315,15 @@
             content_type: Either 'text/csv' or 'application/json'. Defaults to JSON.
         """
         key_value_store = await KeyValueStore.open(id=to_key_value_store_id, name=to_key_value_store_name)
         items: list[dict] = []
         limit = 1000
         offset = 0
         while True:
-            list_items = await self._dataset_client.list_items(limit=limit, offset=offset)
+            list_items = await self._resource_client.list_items(limit=limit, offset=offset)
             items.extend(list_items.items)
             if list_items.total <= offset + list_items.count:
                 break
             offset += list_items.count
 
         if len(items) == 0:
             raise ValueError('Cannot export an empty dataset')
```

### Comparing `crawlee-0.0.3b9/src/crawlee/storages/key_value_store.py` & `crawlee-0.0.4b1/src/crawlee/storages/key_value_store.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, AsyncIterator, TypeVar, overload
 
 from typing_extensions import override
 
+from crawlee.consts import KEY_VALUE_STORE_LABEL
+from crawlee.models import KeyValueStoreKeyInfo
 from crawlee.storages.base_storage import BaseStorage
-from crawlee.storages.models import KeyValueStoreKeyInfo
 
 if TYPE_CHECKING:
-    from crawlee.base_storage_client import (
-        BaseKeyValueStoreClient,
-        BaseKeyValueStoreCollectionClient,
-        BaseStorageClient,
-    )
+    from crawlee.base_storage_client import BaseStorageClient
     from crawlee.configuration import Configuration
 
 T = TypeVar('T')
 
 
 class KeyValueStore(BaseStorage):
     """Represents a key-value based storage for reading data records or files.
@@ -35,99 +32,117 @@
     `config`. If neither is provided, the default store for the crawler run is used. Opening a non-existent store by
     `id` raises an error, while a non-existent store by `name` is created.
 
     Usage:
         kvs = await KeyValueStore.open(id='my_kvs_id')
     """
 
+    LABEL = KEY_VALUE_STORE_LABEL
+    """Human readable label of the storage."""
+
     def __init__(
         self,
         id: str,
         name: str | None,
         configuration: Configuration,
         client: BaseStorageClient,
     ) -> None:
-        super().__init__(id=id, name=name, client=client, configuration=configuration)
-        self._key_value_store_client = client.key_value_store(self.id)
+        self._id = id
+        self._name = name
+        self._configuration = configuration
+
+        # Get resource clients from storage client
+        self._resource_client = client.key_value_store(self._id)
+        self._resource_collection_client = client.key_value_stores()
 
-    @classmethod
     @override
-    def _get_human_friendly_label(cls) -> str:
-        return 'Key-value store'
+    @property
+    def id(self) -> str:
+        return self._id
 
-    @classmethod
     @override
-    def _get_default_id(cls, configuration: Configuration) -> str:
-        return configuration.default_key_value_store_id
+    @property
+    def name(self) -> str | None:
+        return self._name
 
-    @classmethod
     @override
-    def _get_single_storage_client(cls, id: str, client: BaseStorageClient) -> BaseKeyValueStoreClient:
-        return client.key_value_store(id)
-
     @classmethod
+    async def open(
+        cls,
+        *,
+        id: str | None = None,
+        name: str | None = None,
+        configuration: Configuration | None = None,
+    ) -> KeyValueStore:
+        from crawlee.storages._creation_management import open_storage
+
+        return await open_storage(
+            storage_class=cls,
+            id=id,
+            name=name,
+            configuration=configuration,
+        )
+
     @override
-    def _get_storage_collection_client(cls, client: BaseStorageClient) -> BaseKeyValueStoreCollectionClient:
-        return client.key_value_stores()
+    async def drop(self) -> None:
+        from crawlee.storages._creation_management import remove_storage_from_cache
+
+        await self._resource_client.delete()
+        remove_storage_from_cache(storage_class_label=self.LABEL, id=self._id, name=self._name)
 
     @overload
     async def get_value(self, key: str) -> Any: ...
 
     @overload
     async def get_value(self, key: str, default_value: T) -> T: ...
 
     @overload
     async def get_value(self, key: str, default_value: T | None = None) -> T | None: ...
 
     async def get_value(self, key: str, default_value: T | None = None) -> T | None:
-        """Get a value from the key-value store.
+        """Get a value from the KVS.
 
         Args:
             key: Key of the record to retrieve.
             default_value: Default value returned in case the record does not exist.
 
         Returns:
-            Any: The value associated with the given key. `default_value` is used in case the record does not exist.
+            The value associated with the given key. `default_value` is used in case the record does not exist.
         """
-        record = await self._key_value_store_client.get_record(key)
+        record = await self._resource_client.get_record(key)
         return record.value if record else default_value
 
     async def iterate_keys(self, exclusive_start_key: str | None = None) -> AsyncIterator[KeyValueStoreKeyInfo]:
-        """Iterate over the keys in the key-value store.
+        """Iterate over the existing keys in the KVS.
 
         Args:
-            exclusive_start_key: All keys up to this one (including) are skipped from the result.
+            exclusive_start_key: Key to start the iteration from.
 
         Yields:
-            Information about a key-value store record.
+            Information about the key.
         """
         while True:
-            list_keys = await self._key_value_store_client.list_keys(exclusive_start_key=exclusive_start_key)
+            list_keys = await self._resource_client.list_keys(exclusive_start_key=exclusive_start_key)
             for item in list_keys.items:
                 yield KeyValueStoreKeyInfo(key=item.key, size=item.size)
 
             if not list_keys.is_truncated:
                 break
             exclusive_start_key = list_keys.next_exclusive_start_key
 
     async def set_value(
         self,
         key: str,
         value: Any,
         content_type: str | None = None,
     ) -> None:
-        """Set or delete a value in the key-value store.
+        """Set a value in the KVS.
 
         Args:
-            key: The key under which the value should be saved.
-            value: The value to save. If the value is `None`, the corresponding key-value pair will be deleted.
-            content_type: The content type of the saved value.
+            key: Key of the record to set.
+            value: Value to set. If `None`, the record is deleted.
+            content_type: Content type of the record.
         """
         if value is None:
-            return await self._key_value_store_client.delete_record(key)
+            return await self._resource_client.delete_record(key)
 
-        return await self._key_value_store_client.set_record(key, value, content_type)
-
-    async def drop(self) -> None:
-        """Remove the key-value store either from the Apify cloud storage or from the local directory."""
-        await self._key_value_store_client.delete()
-        self._remove_from_cache()
+        return await self._resource_client.set_record(key, value, content_type)
```

### Comparing `crawlee-0.0.3b9/src/crawlee/storages/request_list.py` & `crawlee-0.0.4b1/src/crawlee/storages/request_list.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from __future__ import annotations
 
 from collections import deque
 from datetime import timedelta
+from typing import Sequence
 
 from typing_extensions import override
 
-from crawlee.request import BaseRequestData, Request
+from crawlee.models import BaseRequestData, Request
 from crawlee.storages.request_provider import RequestProvider
 
 
 class RequestList(RequestProvider):
     """Represents a (potentially very large) list of URLs to crawl."""
 
     def __init__(self, sources: list[str | Request] | None = None, name: str | None = None) -> None:
@@ -72,16 +73,24 @@
     @override
     async def get_handled_count(self) -> int:
         return self._handled_count
 
     @override
     async def add_requests_batched(
         self,
-        requests: list[BaseRequestData | Request],
+        requests: Sequence[BaseRequestData | Request | str],
         *,
         batch_size: int = 1000,
         wait_for_all_requests_to_be_added: bool = False,
         wait_time_between_batches: timedelta = timedelta(seconds=1),
     ) -> None:
-        self._sources.extend(
-            request if isinstance(request, Request) else Request.from_base_request_data(request) for request in requests
-        )
+        batch = []
+
+        for request in requests:
+            if isinstance(request, Request):
+                batch.append(request)
+            elif isinstance(request, BaseRequestData):
+                batch.append(Request.from_base_request_data(request))
+            else:
+                batch.append(Request.from_url(request))
+
+        self._sources.extend(batch)
```

### Comparing `crawlee-0.0.3b9/src/crawlee/storages/request_provider.py` & `crawlee-0.0.4b1/src/crawlee/storages/request_provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from datetime import timedelta
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Sequence
 
 if TYPE_CHECKING:
-    from crawlee.request import BaseRequestData, Request
-    from crawlee.storages.models import RequestQueueOperationInfo
+    from crawlee.models import BaseRequestData, Request, RequestQueueOperationInfo
 
 
 class RequestProvider(ABC):
     """Provides access to a queue of crawling requests."""
 
     @property
     @abstractmethod
@@ -51,15 +50,15 @@
     @abstractmethod
     async def get_handled_count(self) -> int:
         """Returns the number of handled requests."""
 
     @abstractmethod
     async def add_requests_batched(
         self,
-        requests: list[BaseRequestData | Request],
+        requests: Sequence[BaseRequestData | Request | str],
         *,
         batch_size: int = 1000,
         wait_for_all_requests_to_be_added: bool = False,
         wait_time_between_batches: timedelta = timedelta(seconds=1),
     ) -> None:
         """Adds requests to the queue in batches.
```

### Comparing `crawlee-0.0.3b9/src/crawlee/storages/request_queue.py` & `crawlee-0.0.4b1/src/crawlee/storages/request_queue.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 from __future__ import annotations
 
 import asyncio
 from collections import OrderedDict
 from datetime import datetime, timedelta, timezone
 from logging import getLogger
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Sequence
 from typing import OrderedDict as OrderedDictType
 
 from typing_extensions import override
 
 from crawlee._utils.crypto import crypto_random_object_id
 from crawlee._utils.lru_cache import LRUCache
 from crawlee._utils.requests import unique_key_to_request_id
-from crawlee.request import Request
+from crawlee.consts import REQUEST_QUEUE_LABEL
+from crawlee.models import BaseRequestData, Request, RequestQueueHeadState, RequestQueueOperationInfo
 from crawlee.storages.base_storage import BaseStorage
-from crawlee.storages.models import RequestQueueHeadState, RequestQueueOperationInfo
 from crawlee.storages.request_provider import RequestProvider
 
 if TYPE_CHECKING:
-    from crawlee.base_storage_client import BaseRequestQueueClient, BaseRequestQueueCollectionClient, BaseStorageClient
+    from crawlee.base_storage_client import BaseStorageClient
     from crawlee.configuration import Configuration
-    from crawlee.request import BaseRequestData
-    from crawlee.storages.models import BaseStorageMetadata
+    from crawlee.models import BaseStorageMetadata
 
 logger = getLogger(__name__)
 
 
 class RequestQueue(BaseStorage, RequestProvider):
     """Represents a queue storage for HTTP requests to crawl.
 
@@ -42,14 +41,17 @@
     unnamed queues expiring after 7 days unless specified otherwise. Supports mutable operations—URLs can be added
     and deleted.
 
     Usage:
         rq = await RequestQueue.open(id='my_rq_id')
     """
 
+    LABEL = REQUEST_QUEUE_LABEL
+    """Human readable label of the storage."""
+
     _API_PROCESSED_REQUESTS_DELAY = timedelta(seconds=10)
     """Delay threshold to assume consistency of queue head operations after queue modifications."""
 
     _MAX_CACHED_REQUESTS = 1_000_000
     """Maximum number of requests that can be cached."""
 
     _MAX_HEAD_LIMIT = 1000
@@ -73,71 +75,72 @@
     def __init__(
         self,
         id: str,
         name: str | None,
         configuration: Configuration,
         client: BaseStorageClient,
     ) -> None:
-        super().__init__(id=id, name=name, client=client, configuration=configuration)
+        self._id = id
+        self._name = name
+        self._configuration = configuration
+
+        # Get resource clients from storage client
+        self._resource_client = client.request_queue(self._id)
+        self._resource_collection_client = client.request_queues()
 
+        # Other internal attributes
         self._client_key = crypto_random_object_id()
         self._internal_timeout_seconds = 5 * 60
         self._assumed_total_count = 0
         self._assumed_handled_count = 0
-        self._request_queue_client = client.request_queue(self.id)
         self._queue_head_dict: OrderedDictType[str, str] = OrderedDict()
         self._query_queue_head_task: asyncio.Task | None = None
         self._in_progress: set[str] = set()
         self._last_activity = datetime.now(timezone.utc)
         self._recently_handled: LRUCache[bool] = LRUCache(max_length=self._RECENTLY_HANDLED_CACHE_SIZE)
         self._requests_cache: LRUCache[dict] = LRUCache(max_length=self._MAX_CACHED_REQUESTS)
 
-    @classmethod
     @override
+    @property
+    def id(self) -> str:
+        return self._id
+
+    @override
+    @property
+    def name(self) -> str | None:
+        return self._name
+
+    @override
+    @classmethod
     async def open(
         cls,
         *,
         id: str | None = None,
         name: str | None = None,
         configuration: Configuration | None = None,
     ) -> RequestQueue:
-        rq = await super().open(id=id, name=name, configuration=configuration)
-        await rq.ensure_head_is_non_empty()
-        return rq
+        from crawlee.storages._creation_management import open_storage
 
-    @classmethod
-    @override
-    def _get_human_friendly_label(cls) -> str:
-        return 'Request queue'
-
-    @classmethod
-    @override
-    def _get_default_id(cls, configuration: Configuration) -> str:
-        return configuration.default_request_queue_id
+        return await open_storage(
+            storage_class=cls,
+            id=id,
+            name=name,
+            configuration=configuration,
+        )
 
-    @classmethod
     @override
-    def _get_single_storage_client(
-        cls,
-        id: str,
-        client: BaseStorageClient,
-    ) -> BaseRequestQueueClient:
-        return client.request_queue(id)
+    async def drop(self) -> None:
+        from crawlee.storages._creation_management import remove_storage_from_cache
 
-    @classmethod
-    @override
-    def _get_storage_collection_client(
-        cls,
-        client: BaseStorageClient,
-    ) -> BaseRequestQueueCollectionClient:
-        return client.request_queues()
+        await self._resource_client.delete()
+        remove_storage_from_cache(storage_class_label=self.LABEL, id=self._id, name=self._name)
 
     async def add_request(
         self,
-        request: Request,
+        request: Request | BaseRequestData | str,
         *,
         forefront: bool = False,
     ) -> RequestQueueOperationInfo:
         """Adds a request to the `RequestQueue` while managing deduplication and positioning within the queue.
 
         The deduplication of requests relies on the `uniqueKey` field within the request dictionary. If `uniqueKey`
         exists, it remains unchanged; if it does not, it is generated based on the request's `url`, `method`,
@@ -163,14 +166,19 @@
 
         Returns: A dictionary containing information about the operation, including:
             - `requestId` The ID of the request.
             - `uniqueKey` The unique key associated with the request.
             - `wasAlreadyPresent` (bool): Indicates whether the request was already in the queue.
             - `wasAlreadyHandled` (bool): Indicates whether the request was already processed.
         """
+        if isinstance(request, BaseRequestData):
+            request = Request.from_base_request_data(request)
+        elif isinstance(request, str):
+            request = Request.from_url(request)
+
         self._last_activity = datetime.now(timezone.utc)
 
         cache_key = unique_key_to_request_id(request.unique_key)
         cached_info = self._requests_cache.get(cache_key)
 
         if cached_info:
             request.id = cached_info['id']
@@ -179,15 +187,15 @@
             return RequestQueueOperationInfo(
                 request_id=request.id,
                 request_unique_key=request.unique_key,
                 was_already_present=True,
                 was_already_handled=cached_info['wasAlreadyHandled'],
             )
 
-        queue_operation_info = await self._request_queue_client.add_request(request, forefront=forefront)
+        queue_operation_info = await self._resource_client.add_request(request, forefront=forefront)
         queue_operation_info.request_unique_key = request.unique_key
 
         self._cache_request(cache_key, queue_operation_info)
 
         request_id, was_already_present = queue_operation_info.request_id, queue_operation_info.was_already_present
         is_handled = request.handled_at is not None
 
@@ -201,36 +209,33 @@
             self._maybe_add_request_to_queue_head(request_id, forefront=forefront)
 
         return queue_operation_info
 
     @override
     async def add_requests_batched(
         self,
-        requests: list[BaseRequestData | Request],
+        requests: Sequence[BaseRequestData | Request | str],
         *,
         batch_size: int = 1000,
         wait_for_all_requests_to_be_added: bool = False,
         wait_time_between_batches: timedelta = timedelta(seconds=1),
     ) -> None:
         for request in requests:
-            if isinstance(request, Request):
-                await self.add_request(request)
-            else:
-                await self.add_request(Request.from_base_request_data(request))
+            await self.add_request(request)
 
     async def get_request(self, request_id: str) -> Request | None:
         """Retrieve a request from the queue.
 
         Args:
             request_id: ID of the request to retrieve.
 
         Returns:
             The retrieved request, or `None`, if it does not exist.
         """
-        return await self._request_queue_client.get_request(request_id)
+        return await self._resource_client.get_request(request_id)
 
     async def fetch_next_request(self) -> Request | None:
         """Return the next request in the queue to be processed.
 
         Once you successfully finish processing of the request, you need to call `RequestQueue.mark_request_as_handled`
         to mark the request as handled in the queue. If there was some error in processing the request, call
         `RequestQueue.reclaim_request` instead, so that the queue will give the request to some other consumer
@@ -323,15 +328,15 @@
         if request.id not in self._in_progress:
             logger.debug(f'Cannot mark request (ID: {request.id}) as handled, because it is not in progress!')
             return None
 
         if request.handled_at is None:
             request.handled_at = datetime.now(timezone.utc)
 
-        queue_operation_info = await self._request_queue_client.update_request(request)
+        queue_operation_info = await self._resource_client.update_request(request)
         queue_operation_info.request_unique_key = request.unique_key
 
         self._in_progress.remove(request.id)
         self._recently_handled[request.id] = True
 
         if not queue_operation_info.was_already_handled:
             self._assumed_handled_count += 1
@@ -361,15 +366,15 @@
         if request.id not in self._in_progress:
             logger.debug(f'Cannot reclaim request (ID: {request.id}), because it is not in progress!')
             return None
 
         # TODO: If request hasn't been changed since the last getRequest(), we don't need to call updateRequest()
         # and thus improve performance.
         # https://github.com/apify/apify-sdk-python/issues/143
-        queue_operation_info = await self._request_queue_client.update_request(request, forefront=forefront)
+        queue_operation_info = await self._resource_client.update_request(request, forefront=forefront)
         queue_operation_info.request_unique_key = request.unique_key
         self._cache_request(unique_key_to_request_id(request.unique_key), queue_operation_info)
 
         # Wait a little to increase a chance that the next call to fetchNextRequest() will return the request with
         # updated data. This is to compensate for the limitation of DynamoDB, where writes might not be immediately
         # visible to subsequent reads.
         def callback() -> None:
@@ -413,26 +418,21 @@
 
         if len(self._queue_head_dict) > 0 or self._in_progress_count() > 0:
             return False
 
         is_head_consistent = await self.ensure_head_is_non_empty(ensure_consistency=True)
         return is_head_consistent and len(self._queue_head_dict) == 0 and self._in_progress_count() == 0
 
-    async def drop(self) -> None:
-        """Remove the request queue either from the Apify cloud storage or from the local directory."""
-        await self._request_queue_client.delete()
-        self._remove_from_cache()
-
     async def get_info(self) -> BaseStorageMetadata | None:
         """Get an object containing general information about the request queue.
 
         Returns:
             Object returned by calling the GET request queue API endpoint.
         """
-        return await self._request_queue_client.get()
+        return await self._resource_client.get()
 
     @override
     async def get_handled_count(self) -> int:
         return self._assumed_handled_count
 
     @override
     async def get_total_count(self) -> int:
@@ -535,15 +535,15 @@
             'uniqueKey': operation_info.request_unique_key,
             'wasAlreadyHandled': operation_info.was_already_handled,
         }
 
     async def _queue_query_head(self, limit: int) -> RequestQueueHeadState:
         query_started_at = datetime.now(timezone.utc)
 
-        list_head = await self._request_queue_client.list_head(limit=limit)
+        list_head = await self._resource_client.list_head(limit=limit)
         list_head_items: list[Request] = list_head.items
 
         for request in list_head_items:
             # Queue head index might be behind the main table, so ensure we don't recycle requests
             if (
                 not request.id
                 or not request.unique_key
```

### Comparing `crawlee-0.0.3b9/src/crawlee/types.py` & `crawlee-0.0.4b1/src/crawlee/types.py`

 * *Files identical despite different names*

