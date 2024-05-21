# Comparing `tmp/devcycle-python-server-sdk-3.5.0.tar.gz` & `tmp/devcycle-python-server-sdk-3.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devcycle-python-server-sdk-3.5.0.tar", last modified: Wed May 15 19:13:42 2024, max compression
+gzip compressed data, was "devcycle-python-server-sdk-3.5.1.tar", last modified: Tue May 21 19:31:10 2024, max compression
```

## Comparing `devcycle-python-server-sdk-3.5.0.tar` & `devcycle-python-server-sdk-3.5.1.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:13:42.541181 devcycle-python-server-sdk-3.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-15 19:13:42.541181 devcycle-python-server-sdk-3.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3751 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:13:42.533181 devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:13:42.537181 devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/api/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/api/backoff.py
--rw-r--r--   0 runner    (1001) docker     (127)     5111 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/api/bucketing_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/api/config_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/api/event_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    16332 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/api/local_bucketing.py
--rw-r--r--   0 runner    (1001) docker     (127)     7352 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/cloud_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/devcycle_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9373 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/local_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:13:42.537181 devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/managers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/managers/config_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     8071 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/managers/event_queue_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:13:42.537181 devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/models/bucketed_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/models/error_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/models/event.py
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/models/feature.py
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/models/platform_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     6266 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/models/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/models/variable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:13:42.537181 devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/open_feature_provider/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/open_feature_provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/open_feature_provider/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/options.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:13:42.537181 devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/protobuf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/protobuf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4684 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/protobuf/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4244 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/protobuf/variableForUserParams_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:13:42.537181 devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/util/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/util/strings.py
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/util/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:13:42.537181 devcycle-python-server-sdk-3.5.0/devcycle_python_server_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-15 19:13:41.000000 devcycle-python-server-sdk-3.5.0/devcycle_python_server_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-05-15 19:13:42.000000 devcycle-python-server-sdk-3.5.0/devcycle_python_server_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 19:13:41.000000 devcycle-python-server-sdk-3.5.0/devcycle_python_server_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-15 19:13:41.000000 devcycle-python-server-sdk-3.5.0/devcycle_python_server_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-15 19:13:41.000000 devcycle-python-server-sdk-3.5.0/devcycle_python_server_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:13:42.541181 devcycle-python-server-sdk-3.5.0/example/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/example/cloud_client_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/example/local_bucketing_client_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/example/openfeature_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-15 19:13:42.541181 devcycle-python-server-sdk-3.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:13:42.541181 devcycle-python-server-sdk-3.5.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:13:42.541181 devcycle-python-server-sdk-3.5.0/test/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/test/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7739 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/test/api/test_bucketing_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4413 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/test/api/test_config_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/test/api/test_event_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    15254 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/test/api/test_local_bucketing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:13:42.541181 devcycle-python-server-sdk-3.5.0/test/fixture/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/test/fixture/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/test/fixture/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:13:42.541181 devcycle-python-server-sdk-3.5.0/test/managers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/test/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5366 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/test/managers/test_config_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    11053 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/test/managers/test_event_queue_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:13:42.541181 devcycle-python-server-sdk-3.5.0/test/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/test/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/test/models/test_bucketed_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6736 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/test/models/test_user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:13:42.541181 devcycle-python-server-sdk-3.5.0/test/openfeature_test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/test/openfeature_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7653 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/test/openfeature_test/test_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     4426 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/test/openfeature_test/test_provider_local_sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)    11442 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/test/test_cloud_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    13022 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/test/test_local_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:13:42.541181 devcycle-python-server-sdk-3.5.0/test/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/test/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/test/util/test_strings.py
--rw-r--r--   0 runner    (1001) docker     (127)     6671 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/test/util/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/test/util/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:31:10.280134 devcycle-python-server-sdk-3.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-21 19:30:56.000000 devcycle-python-server-sdk-3.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-21 19:31:10.280134 devcycle-python-server-sdk-3.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3751 2024-05-21 19:30:56.000000 devcycle-python-server-sdk-3.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:31:10.268134 devcycle-python-server-sdk-3.5.1/devcycle_python_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-21 19:30:56.000000 devcycle-python-server-sdk-3.5.1/devcycle_python_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:31:10.272134 devcycle-python-server-sdk-3.5.1/devcycle_python_sdk/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 19:30:56.000000 devcycle-python-server-sdk-3.5.1/devcycle_python_sdk/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-21 19:30:56.000000 devcycle-python-server-sdk-3.5.1/devcycle_python_sdk/api/backoff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5111 2024-05-21 19:30:56.000000 devcycle-python-server-sdk-3.5.1/devcycle_python_sdk/api/bucketing_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-05-21 19:30:56.000000 devcycle-python-server-sdk-3.5.1/devcycle_python_sdk/api/config_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-05-21 19:30:56.000000 devcycle-python-server-sdk-3.5.1/devcycle_python_sdk/api/event_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16332 2024-05-21 19:30:56.000000 devcycle-python-server-sdk-3.5.1/devcycle_python_sdk/api/local_bucketing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7352 2024-05-21 19:30:56.000000 devcycle-python-server-sdk-3.5.1/devcycle_python_sdk/cloud_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-21 19:30:56.000000 devcycle-python-server-sdk-3.5.1/devcycle_python_sdk/devcycle_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-21 19:30:56.000000 devcycle-python-server-sdk-3.5.1/devcycle_python_sdk/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9373 2024-05-21 19:30:56.000000 devcycle-python-server-sdk-3.5.1/devcycle_python_sdk/local_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:31:10.272134 devcycle-python-server-sdk-3.5.1/devcycle_python_sdk/managers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 19:30:56.000000 devcycle-python-server-sdk-3.5.1/devcycle_python_sdk/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-05-21 19:30:56.000000 devcycle-python-server-sdk-3.5.1/devcycle_python_sdk/managers/config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8071 2024-05-21 19:30:56.000000 devcycle-python-server-sdk-3.5.1/devcycle_python_sdk/managers/event_queue_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:31:10.272134 devcycle-python-server-sdk-3.5.1/devcycle_python_sdk/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 19:30:56.000000 devcycle-python-server-sdk-3.5.1/devcycle_python_sdk/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-05-21 19:30:56.000000 devcycle-python-server-sdk-3.5.1/devcycle_python_sdk/models/bucketed_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-21 19:30:56.000000 devcycle-python-server-sdk-3.5.1/devcycle_python_sdk/models/error_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-05-21 19:30:56.000000 devcycle-python-server-sdk-3.5.1/devcycle_python_sdk/models/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-21 19:30:56.000000 devcycle-python-server-sdk-3.5.1/devcycle_python_sdk/models/feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-21 19:30:56.000000 devcycle-python-server-sdk-3.5.1/devcycle_python_sdk/models/platform_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6266 2024-05-21 19:30:56.000000 devcycle-python-server-sdk-3.5.1/devcycle_python_sdk/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-21 19:30:56.000000 devcycle-python-server-sdk-3.5.1/devcycle_python_sdk/models/variable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:31:10.272134 devcycle-python-server-sdk-3.5.1/devcycle_python_sdk/open_feature_provider/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 19:30:56.000000 devcycle-python-server-sdk-3.5.1/devcycle_python_sdk/open_feature_provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-05-21 19:30:56.000000 devcycle-python-server-sdk-3.5.1/devcycle_python_sdk/open_feature_provider/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-05-21 19:30:56.000000 devcycle-python-server-sdk-3.5.1/devcycle_python_sdk/options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:31:10.272134 devcycle-python-server-sdk-3.5.1/devcycle_python_sdk/protobuf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 19:30:56.000000 devcycle-python-server-sdk-3.5.1/devcycle_python_sdk/protobuf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4684 2024-05-21 19:30:56.000000 devcycle-python-server-sdk-3.5.1/devcycle_python_sdk/protobuf/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4244 2024-05-21 19:30:56.000000 devcycle-python-server-sdk-3.5.1/devcycle_python_sdk/protobuf/variableForUserParams_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:31:10.272134 devcycle-python-server-sdk-3.5.1/devcycle_python_sdk/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 19:30:56.000000 devcycle-python-server-sdk-3.5.1/devcycle_python_sdk/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-21 19:30:56.000000 devcycle-python-server-sdk-3.5.1/devcycle_python_sdk/util/strings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-21 19:30:56.000000 devcycle-python-server-sdk-3.5.1/devcycle_python_sdk/util/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:31:10.272134 devcycle-python-server-sdk-3.5.1/devcycle_python_server_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-21 19:31:10.000000 devcycle-python-server-sdk-3.5.1/devcycle_python_server_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-05-21 19:31:10.000000 devcycle-python-server-sdk-3.5.1/devcycle_python_server_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 19:31:10.000000 devcycle-python-server-sdk-3.5.1/devcycle_python_server_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-21 19:31:10.000000 devcycle-python-server-sdk-3.5.1/devcycle_python_server_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-21 19:31:10.000000 devcycle-python-server-sdk-3.5.1/devcycle_python_server_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:31:10.276134 devcycle-python-server-sdk-3.5.1/example/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 19:30:56.000000 devcycle-python-server-sdk-3.5.1/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-05-21 19:30:56.000000 devcycle-python-server-sdk-3.5.1/example/cloud_client_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-05-21 19:30:56.000000 devcycle-python-server-sdk-3.5.1/example/local_bucketing_client_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-05-21 19:30:56.000000 devcycle-python-server-sdk-3.5.1/example/openfeature_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-21 19:30:56.000000 devcycle-python-server-sdk-3.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-21 19:31:10.280134 devcycle-python-server-sdk-3.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-21 19:30:56.000000 devcycle-python-server-sdk-3.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:31:10.276134 devcycle-python-server-sdk-3.5.1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 19:30:56.000000 devcycle-python-server-sdk-3.5.1/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:31:10.276134 devcycle-python-server-sdk-3.5.1/test/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 19:30:56.000000 devcycle-python-server-sdk-3.5.1/test/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7739 2024-05-21 19:30:56.000000 devcycle-python-server-sdk-3.5.1/test/api/test_bucketing_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4413 2024-05-21 19:30:56.000000 devcycle-python-server-sdk-3.5.1/test/api/test_config_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-05-21 19:30:56.000000 devcycle-python-server-sdk-3.5.1/test/api/test_event_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15254 2024-05-21 19:30:56.000000 devcycle-python-server-sdk-3.5.1/test/api/test_local_bucketing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:31:10.276134 devcycle-python-server-sdk-3.5.1/test/fixture/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 19:30:56.000000 devcycle-python-server-sdk-3.5.1/test/fixture/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-21 19:30:56.000000 devcycle-python-server-sdk-3.5.1/test/fixture/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:31:10.276134 devcycle-python-server-sdk-3.5.1/test/managers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 19:30:56.000000 devcycle-python-server-sdk-3.5.1/test/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5366 2024-05-21 19:30:56.000000 devcycle-python-server-sdk-3.5.1/test/managers/test_config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11053 2024-05-21 19:30:56.000000 devcycle-python-server-sdk-3.5.1/test/managers/test_event_queue_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:31:10.276134 devcycle-python-server-sdk-3.5.1/test/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 19:30:56.000000 devcycle-python-server-sdk-3.5.1/test/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-21 19:30:56.000000 devcycle-python-server-sdk-3.5.1/test/models/test_bucketed_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6736 2024-05-21 19:30:56.000000 devcycle-python-server-sdk-3.5.1/test/models/test_user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:31:10.276134 devcycle-python-server-sdk-3.5.1/test/openfeature_test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 19:30:56.000000 devcycle-python-server-sdk-3.5.1/test/openfeature_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7653 2024-05-21 19:30:56.000000 devcycle-python-server-sdk-3.5.1/test/openfeature_test/test_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4426 2024-05-21 19:30:56.000000 devcycle-python-server-sdk-3.5.1/test/openfeature_test/test_provider_local_sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11442 2024-05-21 19:30:56.000000 devcycle-python-server-sdk-3.5.1/test/test_cloud_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13022 2024-05-21 19:30:56.000000 devcycle-python-server-sdk-3.5.1/test/test_local_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:31:10.276134 devcycle-python-server-sdk-3.5.1/test/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 19:30:56.000000 devcycle-python-server-sdk-3.5.1/test/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-21 19:30:56.000000 devcycle-python-server-sdk-3.5.1/test/util/test_strings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6671 2024-05-21 19:30:56.000000 devcycle-python-server-sdk-3.5.1/test/util/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-21 19:30:56.000000 devcycle-python-server-sdk-3.5.1/test/util/test_version.py
```

### Comparing `devcycle-python-server-sdk-3.5.0/LICENSE` & `devcycle-python-server-sdk-3.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.5.0/README.md` & `devcycle-python-server-sdk-3.5.1/README.md`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/api/bucketing_client.py` & `devcycle-python-server-sdk-3.5.1/devcycle_python_sdk/api/bucketing_client.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/api/config_client.py` & `devcycle-python-server-sdk-3.5.1/devcycle_python_sdk/api/config_client.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/api/event_client.py` & `devcycle-python-server-sdk-3.5.1/devcycle_python_sdk/api/event_client.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/api/local_bucketing.py` & `devcycle-python-server-sdk-3.5.1/devcycle_python_sdk/api/local_bucketing.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/cloud_client.py` & `devcycle-python-server-sdk-3.5.1/devcycle_python_sdk/cloud_client.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/devcycle_client.py` & `devcycle-python-server-sdk-3.5.1/devcycle_python_sdk/devcycle_client.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/exceptions.py` & `devcycle-python-server-sdk-3.5.1/devcycle_python_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/local_client.py` & `devcycle-python-server-sdk-3.5.1/devcycle_python_sdk/local_client.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/managers/config_manager.py` & `devcycle-python-server-sdk-3.5.1/devcycle_python_sdk/managers/config_manager.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/managers/event_queue_manager.py` & `devcycle-python-server-sdk-3.5.1/devcycle_python_sdk/managers/event_queue_manager.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/models/bucketed_config.py` & `devcycle-python-server-sdk-3.5.1/devcycle_python_sdk/models/bucketed_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,17 +56,17 @@
     edge_db: Optional[EdgeDBSettings]
     opt_in: Optional[OptInSettings]
     disable_passthrough_rollouts: Optional[bool]
 
     @classmethod
     def from_json(cls, data: dict) -> "ProjectSettings":
         return cls(
-            edge_db=EdgeDBSettings.from_json(data["edgeDB"])
-            if "edgeDB" in data
-            else None,
+            edge_db=(
+                EdgeDBSettings.from_json(data["edgeDB"]) if "edgeDB" in data else None
+            ),
             opt_in=OptInSettings.from_json(data["optIn"]) if "optIn" in data else None,
             disable_passthrough_rollouts=data.get("disablePassthroughRollouts", False),
         )
 
 
 @dataclass
 class Project:
@@ -77,17 +77,19 @@
 
     @classmethod
     def from_json(cls, data: dict) -> "Project":
         return cls(
             id=data["_id"],
             key=data["key"],
             a0_organization=data["a0_organization"],
-            settings=ProjectSettings.from_json(data["settings"])
-            if "settings" in data
-            else None,
+            settings=(
+                ProjectSettings.from_json(data["settings"])
+                if "settings" in data
+                else None
+            ),
         )
 
 
 @dataclass
 class Environment:
     id: str
     key: str
```

### Comparing `devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/models/event.py` & `devcycle-python-server-sdk-3.5.1/devcycle_python_sdk/models/event.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/models/feature.py` & `devcycle-python-server-sdk-3.5.1/devcycle_python_sdk/models/feature.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/models/platform_data.py` & `devcycle-python-server-sdk-3.5.1/devcycle_python_sdk/models/platform_data.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/models/user.py` & `devcycle-python-server-sdk-3.5.1/devcycle_python_sdk/models/user.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/models/variable.py` & `devcycle-python-server-sdk-3.5.1/devcycle_python_sdk/models/variable.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/open_feature_provider/provider.py` & `devcycle-python-server-sdk-3.5.1/devcycle_python_sdk/open_feature_provider/provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,17 +54,19 @@
                     return FlagResolutionDetails(
                         value=default_value,
                         reason=Reason.DEFAULT,
                     )
                 else:
                     return FlagResolutionDetails(
                         value=variable.value,
-                        reason=Reason.DEFAULT
-                        if variable.isDefaulted
-                        else Reason.TARGETING_MATCH,
+                        reason=(
+                            Reason.DEFAULT
+                            if variable.isDefaulted
+                            else Reason.TARGETING_MATCH
+                        ),
                     )
             except ValueError as e:
                 # occurs if the key or default value is None
                 raise InvalidContextError(str(e))
         else:
             return FlagResolutionDetails(
                 value=default_value,
```

### Comparing `devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/options.py` & `devcycle-python-server-sdk-3.5.1/devcycle_python_sdk/options.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/protobuf/utils.py` & `devcycle-python-server-sdk-3.5.1/devcycle_python_sdk/protobuf/utils.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/protobuf/variableForUserParams_pb2.py` & `devcycle-python-server-sdk-3.5.1/devcycle_python_sdk/protobuf/variableForUserParams_pb2.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.5.0/devcycle_python_server_sdk.egg-info/SOURCES.txt` & `devcycle-python-server-sdk-3.5.1/devcycle_python_server_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.5.0/example/cloud_client_example.py` & `devcycle-python-server-sdk-3.5.1/example/cloud_client_example.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.5.0/example/local_bucketing_client_example.py` & `devcycle-python-server-sdk-3.5.1/example/local_bucketing_client_example.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.5.0/example/openfeature_example.py` & `devcycle-python-server-sdk-3.5.1/example/openfeature_example.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.5.0/pyproject.toml` & `devcycle-python-server-sdk-3.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.5.0/setup.py` & `devcycle-python-server-sdk-3.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.5.0/test/api/test_bucketing_client.py` & `devcycle-python-server-sdk-3.5.1/test/api/test_bucketing_client.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.5.0/test/api/test_config_client.py` & `devcycle-python-server-sdk-3.5.1/test/api/test_config_client.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.5.0/test/api/test_event_client.py` & `devcycle-python-server-sdk-3.5.1/test/api/test_event_client.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.5.0/test/api/test_local_bucketing.py` & `devcycle-python-server-sdk-3.5.1/test/api/test_local_bucketing.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.5.0/test/fixture/data.py` & `devcycle-python-server-sdk-3.5.1/test/fixture/data.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.5.0/test/managers/test_config_manager.py` & `devcycle-python-server-sdk-3.5.1/test/managers/test_config_manager.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.5.0/test/managers/test_event_queue_manager.py` & `devcycle-python-server-sdk-3.5.1/test/managers/test_event_queue_manager.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.5.0/test/models/test_bucketed_config.py` & `devcycle-python-server-sdk-3.5.1/test/models/test_bucketed_config.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.5.0/test/models/test_user.py` & `devcycle-python-server-sdk-3.5.1/test/models/test_user.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.5.0/test/openfeature_test/test_provider.py` & `devcycle-python-server-sdk-3.5.1/test/openfeature_test/test_provider.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.5.0/test/openfeature_test/test_provider_local_sdk.py` & `devcycle-python-server-sdk-3.5.1/test/openfeature_test/test_provider_local_sdk.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.5.0/test/test_cloud_client.py` & `devcycle-python-server-sdk-3.5.1/test/test_cloud_client.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.5.0/test/test_local_client.py` & `devcycle-python-server-sdk-3.5.1/test/test_local_client.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.5.0/test/util/test_strings.py` & `devcycle-python-server-sdk-3.5.1/test/util/test_strings.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.5.0/test/util/test_utils.py` & `devcycle-python-server-sdk-3.5.1/test/util/test_utils.py`

 * *Files identical despite different names*

