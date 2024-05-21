# Comparing `tmp/accelbyte_py_sdk_service_dsartifact-0.5.0.tar.gz` & `tmp/accelbyte_py_sdk_service_dsartifact-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accelbyte_py_sdk_service_dsartifact-0.5.0.tar", last modified: Tue May  7 06:26:45 2024, max compression
+gzip compressed data, was "accelbyte_py_sdk_service_dsartifact-0.6.0.tar", last modified: Tue May 21 03:45:57 2024, max compression
```

## Comparing `accelbyte_py_sdk_service_dsartifact-0.5.0.tar` & `accelbyte_py_sdk_service_dsartifact-0.6.0.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:26:45.227721 accelbyte_py_sdk_service_dsartifact-0.5.0/
--rw-r--r--   0 root         (0) root         (0)     1139 2024-05-07 06:26:45.227721 accelbyte_py_sdk_service_dsartifact-0.5.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      880 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:26:45.223721 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:26:45.223721 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:26:45.223721 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/
--rw-rw-r--   0 root         (0) root         (0)     1957 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:26:45.223721 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/models/
--rw-rw-r--   0 root         (0) root         (0)     1579 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/models/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7055 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/models/log_app_message_declaration.py
--rw-rw-r--   0 root         (0) root         (0)     7962 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/models/models_all_queue_result.py
--rw-rw-r--   0 root         (0) root         (0)     4910 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/models/models_artifact_file_status.py
--rw-rw-r--   0 root         (0) root         (0)     5055 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/models/models_list_all_queue_response.py
--rw-rw-r--   0 root         (0) root         (0)     4872 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/models/models_list_nodes_ip_address.py
--rw-rw-r--   0 root         (0) root         (0)     4982 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/models/models_list_queue_response.py
--rw-rw-r--   0 root         (0) root         (0)     5363 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/models/models_list_terminated_servers_response.py
--rw-rw-r--   0 root         (0) root         (0)     6386 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/models/models_match_result.py
--rw-rw-r--   0 root         (0) root         (0)     5674 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/models/models_notif_payload_server_status_change.py
--rw-rw-r--   0 root         (0) root         (0)     5483 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/models/models_paging_cursor.py
--rw-rw-r--   0 root         (0) root         (0)     8386 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/models/models_queue.py
--rw-rw-r--   0 root         (0) root         (0)     5176 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/models/models_queue_result.py
--rw-rw-r--   0 root         (0) root         (0)     3813 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/models/models_request_match_member.py
--rw-rw-r--   0 root         (0) root         (0)     6031 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/models/models_request_match_party.py
--rw-rw-r--   0 root         (0) root         (0)     4451 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/models/models_request_matching_ally.py
--rw-rw-r--   0 root         (0) root         (0)    17809 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/models/models_server.py
--rw-rw-r--   0 root         (0) root         (0)     4404 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/models/models_status_history.py
--rw-rw-r--   0 root         (0) root         (0)     4439 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/models/response_error.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:26:45.227721 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/
--rw-rw-r--   0 root         (0) root         (0)      440 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:26:45.227721 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/all_terminated_servers/
--rw-rw-r--   0 root         (0) root         (0)      532 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/all_terminated_servers/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    14974 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/all_terminated_servers/list_terminated_servers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:26:45.227721 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/
--rw-rw-r--   0 root         (0) root         (0)      934 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6450 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/delete_active_queue.py
--rw-rw-r--   0 root         (0) root         (0)     7072 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/delete_node_by_id.py
--rw-rw-r--   0 root         (0) root         (0)     7999 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/delete_queue.py
--rw-rw-r--   0 root         (0) root         (0)     6694 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/get_active_queue.py
--rw-rw-r--   0 root         (0) root         (0)    11020 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/list_all_active_queue.py
--rw-rw-r--   0 root         (0) root         (0)    12710 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/list_all_queue.py
--rw-rw-r--   0 root         (0) root         (0)     8998 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/list_nodes_ip_address.py
--rw-rw-r--   0 root         (0) root         (0)     9027 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/list_queue.py
--rw-rw-r--   0 root         (0) root         (0)     7192 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/report_failed_upload.py
--rw-rw-r--   0 root         (0) root         (0)     7225 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/set_active_queue.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:26:45.227721 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/download_server_artifact/
--rw-rw-r--   0 root         (0) root         (0)      591 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/download_server_artifact/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7566 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/download_server_artifact/check_server_artifact.py
--rw-rw-r--   0 root         (0) root         (0)     7364 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/download_server_artifact/download_server_artifacts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:26:45.227721 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/operations/
--rw-rw-r--   0 root         (0) root         (0)      524 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/operations/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4989 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/operations/public_get_messages.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:26:45.227721 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/terminated_servers/
--rw-rw-r--   0 root         (0) root         (0)      552 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/terminated_servers/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    16213 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/terminated_servers/list_terminated_servers_e10383.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:26:45.227721 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/wrappers/
--rw-rw-r--   0 root         (0) root         (0)     2405 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/wrappers/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5983 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/wrappers/_all_terminated_servers.py
--rw-rw-r--   0 root         (0) root         (0)    32309 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/wrappers/_artifact_upload_process_queue.py
--rw-rw-r--   0 root         (0) root         (0)     7686 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/wrappers/_download_server_artifact.py
--rw-rw-r--   0 root         (0) root         (0)     2614 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/wrappers/_operations.py
--rw-rw-r--   0 root         (0) root         (0)     6684 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/wrappers/_terminated_servers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:26:45.227721 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk_service_dsartifact.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1139 2024-05-07 06:26:45.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk_service_dsartifact.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3843 2024-05-07 06:26:45.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk_service_dsartifact.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-07 06:26:45.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk_service_dsartifact.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-07 06:26:45.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk_service_dsartifact.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-05-07 06:26:45.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk_service_dsartifact.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)      366 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-07 06:26:45.227721 accelbyte_py_sdk_service_dsartifact-0.5.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:45:57.652236 accelbyte_py_sdk_service_dsartifact-0.6.0/
+-rw-r--r--   0 root         (0) root         (0)     1139 2024-05-21 03:45:57.652236 accelbyte_py_sdk_service_dsartifact-0.6.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      880 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_dsartifact-0.6.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:45:57.644236 accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:45:57.644236 accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:45:57.648236 accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/
+-rw-rw-r--   0 root         (0) root         (0)     1957 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:45:57.648236 accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/models/
+-rw-rw-r--   0 root         (0) root         (0)     1579 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/models/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7055 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/models/log_app_message_declaration.py
+-rw-rw-r--   0 root         (0) root         (0)     7962 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/models/models_all_queue_result.py
+-rw-rw-r--   0 root         (0) root         (0)     4910 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/models/models_artifact_file_status.py
+-rw-rw-r--   0 root         (0) root         (0)     5055 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/models/models_list_all_queue_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4872 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/models/models_list_nodes_ip_address.py
+-rw-rw-r--   0 root         (0) root         (0)     4982 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/models/models_list_queue_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5363 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/models/models_list_terminated_servers_response.py
+-rw-rw-r--   0 root         (0) root         (0)     6386 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/models/models_match_result.py
+-rw-rw-r--   0 root         (0) root         (0)     5674 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/models/models_notif_payload_server_status_change.py
+-rw-rw-r--   0 root         (0) root         (0)     5483 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/models/models_paging_cursor.py
+-rw-rw-r--   0 root         (0) root         (0)     8386 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/models/models_queue.py
+-rw-rw-r--   0 root         (0) root         (0)     5176 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/models/models_queue_result.py
+-rw-rw-r--   0 root         (0) root         (0)     3813 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/models/models_request_match_member.py
+-rw-rw-r--   0 root         (0) root         (0)     6031 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/models/models_request_match_party.py
+-rw-rw-r--   0 root         (0) root         (0)     4451 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/models/models_request_matching_ally.py
+-rw-rw-r--   0 root         (0) root         (0)    17809 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/models/models_server.py
+-rw-rw-r--   0 root         (0) root         (0)     4404 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/models/models_status_history.py
+-rw-rw-r--   0 root         (0) root         (0)     4439 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/models/response_error.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:45:57.648236 accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/operations/
+-rw-rw-r--   0 root         (0) root         (0)      440 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/operations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:45:57.648236 accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/operations/all_terminated_servers/
+-rw-rw-r--   0 root         (0) root         (0)      532 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/operations/all_terminated_servers/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    14974 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/operations/all_terminated_servers/list_terminated_servers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:45:57.648236 accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/
+-rw-rw-r--   0 root         (0) root         (0)      934 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     6450 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/delete_active_queue.py
+-rw-rw-r--   0 root         (0) root         (0)     7072 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/delete_node_by_id.py
+-rw-rw-r--   0 root         (0) root         (0)     7999 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/delete_queue.py
+-rw-rw-r--   0 root         (0) root         (0)     6694 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/get_active_queue.py
+-rw-rw-r--   0 root         (0) root         (0)    11020 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/list_all_active_queue.py
+-rw-rw-r--   0 root         (0) root         (0)    12710 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/list_all_queue.py
+-rw-rw-r--   0 root         (0) root         (0)     8998 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/list_nodes_ip_address.py
+-rw-rw-r--   0 root         (0) root         (0)     9027 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/list_queue.py
+-rw-rw-r--   0 root         (0) root         (0)     7192 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/report_failed_upload.py
+-rw-rw-r--   0 root         (0) root         (0)     7225 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/set_active_queue.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:45:57.648236 accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/operations/download_server_artifact/
+-rw-rw-r--   0 root         (0) root         (0)      591 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/operations/download_server_artifact/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7566 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/operations/download_server_artifact/check_server_artifact.py
+-rw-rw-r--   0 root         (0) root         (0)     7364 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/operations/download_server_artifact/download_server_artifacts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:45:57.648236 accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/operations/operations/
+-rw-rw-r--   0 root         (0) root         (0)      524 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/operations/operations/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4989 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/operations/operations/public_get_messages.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:45:57.652236 accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/operations/terminated_servers/
+-rw-rw-r--   0 root         (0) root         (0)      552 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/operations/terminated_servers/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    16213 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/operations/terminated_servers/list_terminated_servers_e10383.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:45:57.652236 accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/wrappers/
+-rw-rw-r--   0 root         (0) root         (0)     2405 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/wrappers/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     5983 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/wrappers/_all_terminated_servers.py
+-rw-rw-r--   0 root         (0) root         (0)    32309 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/wrappers/_artifact_upload_process_queue.py
+-rw-rw-r--   0 root         (0) root         (0)     7686 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/wrappers/_download_server_artifact.py
+-rw-rw-r--   0 root         (0) root         (0)     2614 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/wrappers/_operations.py
+-rw-rw-r--   0 root         (0) root         (0)     6684 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/wrappers/_terminated_servers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:45:57.652236 accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk_service_dsartifact.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1139 2024-05-21 03:45:57.000000 accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk_service_dsartifact.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3843 2024-05-21 03:45:57.000000 accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk_service_dsartifact.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 03:45:57.000000 accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk_service_dsartifact.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-21 03:45:57.000000 accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk_service_dsartifact.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-05-21 03:45:57.000000 accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk_service_dsartifact.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)      366 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_dsartifact-0.6.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-21 03:45:57.652236 accelbyte_py_sdk_service_dsartifact-0.6.0/setup.cfg
```

### Comparing `accelbyte_py_sdk_service_dsartifact-0.5.0/PKG-INFO` & `accelbyte_py_sdk_service_dsartifact-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: accelbyte-py-sdk-service-dsartifact
-Version: 0.5.0
+Version: 0.6.0
 Summary: AccelByte Python SDK - AccelByte Gaming Services Ds Artifact Manager
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: accelbyte-py-sdk-core
 
 [//]: # (Code generated. DO NOT EDIT!)
 
 # AccelByte Modular Python SDK - Service Module
 
 This is a service module for the [AccelByte Modular Python SDK](https://github.com/AccelByte/accelbyte-python-modular-sdk) package.
 
 ```text
 AccelByte Gaming Services Ds Artifact Manager
-* Version: 1.11.3
+* Version: 1.11.4
 ```
 
 ## Setup
 
 This SDK requires Python 3.9 to be installed.
 
 ### Install with Pip
```

### Comparing `accelbyte_py_sdk_service_dsartifact-0.5.0/README.md` & `accelbyte_py_sdk_service_dsartifact-0.6.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # AccelByte Modular Python SDK - Service Module
 
 This is a service module for the [AccelByte Modular Python SDK](https://github.com/AccelByte/accelbyte-python-modular-sdk) package.
 
 ```text
 AccelByte Gaming Services Ds Artifact Manager
-* Version: 1.11.3
+* Version: 1.11.4
 ```
 
 ## Setup
 
 This SDK requires Python 3.9 to be installed.
 
 ### Install with Pip
```

### Comparing `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/__init__.py` & `accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: service-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Ds Artifact Manager."""
 
-__version__ = "1.11.3"
+__version__ = "1.11.4"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 # all_terminated_servers
 from .wrappers import list_terminated_servers
```

### Comparing `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/models/__init__.py` & `accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/models/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: model-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Ds Artifact Manager."""
 
-__version__ = "1.11.3"
+__version__ = "1.11.4"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .log_app_message_declaration import LogAppMessageDeclaration
 from .models_all_queue_result import ModelsAllQueueResult
```

### Comparing `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/models/log_app_message_declaration.py` & `accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/models/log_app_message_declaration.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/models/models_all_queue_result.py` & `accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/models/models_all_queue_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/models/models_artifact_file_status.py` & `accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/models/models_artifact_file_status.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/models/models_list_all_queue_response.py` & `accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/models/models_list_all_queue_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/models/models_list_nodes_ip_address.py` & `accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/models/models_list_nodes_ip_address.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/models/models_list_queue_response.py` & `accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/models/models_list_queue_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/models/models_list_terminated_servers_response.py` & `accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/models/models_list_terminated_servers_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/models/models_match_result.py` & `accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/models/models_match_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/models/models_notif_payload_server_status_change.py` & `accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/models/models_notif_payload_server_status_change.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/models/models_paging_cursor.py` & `accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/models/models_paging_cursor.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/models/models_queue.py` & `accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/models/models_queue.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/models/models_queue_result.py` & `accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/models/models_queue_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/models/models_request_match_member.py` & `accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/models/models_request_match_member.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/models/models_request_match_party.py` & `accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/models/models_request_match_party.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/models/models_request_matching_ally.py` & `accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/models/models_request_matching_ally.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/models/models_server.py` & `accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/models/models_server.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/models/models_status_history.py` & `accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/models/models_status_history.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/models/response_error.py` & `accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/models/response_error.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/all_terminated_servers/__init__.py` & `accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/operations/all_terminated_servers/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,14 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Ds Artifact Manager."""
 
-__version__ = "1.11.3"
+__version__ = "1.11.4"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .list_terminated_servers import ListTerminatedServers
```

### Comparing `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/all_terminated_servers/list_terminated_servers.py` & `accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/operations/all_terminated_servers/list_terminated_servers.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/__init__.py` & `accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Ds Artifact Manager."""
 
-__version__ = "1.11.3"
+__version__ = "1.11.4"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .delete_active_queue import DeleteActiveQueue
 from .delete_node_by_id import DeleteNodeByID
```

### Comparing `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/delete_active_queue.py` & `accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/delete_active_queue.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/delete_node_by_id.py` & `accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/delete_node_by_id.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/delete_queue.py` & `accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/delete_queue.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/get_active_queue.py` & `accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/get_active_queue.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/list_all_active_queue.py` & `accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/list_all_active_queue.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/list_all_queue.py` & `accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/list_all_queue.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/list_nodes_ip_address.py` & `accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/list_nodes_ip_address.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/list_queue.py` & `accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/list_queue.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/report_failed_upload.py` & `accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/report_failed_upload.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/set_active_queue.py` & `accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/set_active_queue.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/download_server_artifact/__init__.py` & `accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/operations/download_server_artifact/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Ds Artifact Manager."""
 
-__version__ = "1.11.3"
+__version__ = "1.11.4"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .check_server_artifact import CheckServerArtifact
 from .download_server_artifacts import DownloadServerArtifacts
```

### Comparing `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/download_server_artifact/check_server_artifact.py` & `accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/operations/download_server_artifact/check_server_artifact.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/download_server_artifact/download_server_artifacts.py` & `accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/operations/download_server_artifact/download_server_artifacts.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/operations/__init__.py` & `accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/operations/operations/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,14 +4,14 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Ds Artifact Manager."""
 
-__version__ = "1.11.3"
+__version__ = "1.11.4"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .public_get_messages import PublicGetMessages
```

### Comparing `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/operations/public_get_messages.py` & `accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/operations/operations/public_get_messages.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/terminated_servers/__init__.py` & `accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/operations/terminated_servers/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,14 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Ds Artifact Manager."""
 
-__version__ = "1.11.3"
+__version__ = "1.11.4"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .list_terminated_servers_e10383 import ListTerminatedServersWithNamespace
```

### Comparing `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/terminated_servers/list_terminated_servers_e10383.py` & `accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/operations/terminated_servers/list_terminated_servers_e10383.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/wrappers/__init__.py` & `accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/wrappers/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: wrapper-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Ds Artifact Manager."""
 
-__version__ = "1.11.3"
+__version__ = "1.11.4"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from ._all_terminated_servers import list_terminated_servers
 from ._all_terminated_servers import list_terminated_servers_async
```

### Comparing `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/wrappers/_all_terminated_servers.py` & `accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/wrappers/_all_terminated_servers.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/wrappers/_artifact_upload_process_queue.py` & `accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/wrappers/_artifact_upload_process_queue.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/wrappers/_download_server_artifact.py` & `accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/wrappers/_download_server_artifact.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/wrappers/_operations.py` & `accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/wrappers/_operations.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/wrappers/_terminated_servers.py` & `accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk/api/dsartifact/wrappers/_terminated_servers.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk_service_dsartifact.egg-info/PKG-INFO` & `accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk_service_dsartifact.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: accelbyte-py-sdk-service-dsartifact
-Version: 0.5.0
+Version: 0.6.0
 Summary: AccelByte Python SDK - AccelByte Gaming Services Ds Artifact Manager
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: accelbyte-py-sdk-core
 
 [//]: # (Code generated. DO NOT EDIT!)
 
 # AccelByte Modular Python SDK - Service Module
 
 This is a service module for the [AccelByte Modular Python SDK](https://github.com/AccelByte/accelbyte-python-modular-sdk) package.
 
 ```text
 AccelByte Gaming Services Ds Artifact Manager
-* Version: 1.11.3
+* Version: 1.11.4
 ```
 
 ## Setup
 
 This SDK requires Python 3.9 to be installed.
 
 ### Install with Pip
```

### Comparing `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk_service_dsartifact.egg-info/SOURCES.txt` & `accelbyte_py_sdk_service_dsartifact-0.6.0/accelbyte_py_sdk_service_dsartifact.egg-info/SOURCES.txt`

 * *Files identical despite different names*

