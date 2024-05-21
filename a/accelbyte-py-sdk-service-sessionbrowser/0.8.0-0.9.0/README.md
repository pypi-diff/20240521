# Comparing `tmp/accelbyte-py-sdk-service-sessionbrowser-0.8.0.tar.gz` & `tmp/accelbyte-py-sdk-service-sessionbrowser-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accelbyte-py-sdk-service-sessionbrowser-0.8.0.tar", last modified: Wed Mar 13 06:14:48 2024, max compression
+gzip compressed data, was "accelbyte-py-sdk-service-sessionbrowser-0.9.0.tar", last modified: Tue Mar 26 05:44:57 2024, max compression
```

## Comparing `accelbyte-py-sdk-service-sessionbrowser-0.8.0.tar` & `accelbyte-py-sdk-service-sessionbrowser-0.9.0.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:14:48.488185 accelbyte-py-sdk-service-sessionbrowser-0.8.0/
--rw-r--r--   0 root         (0) root         (0)     1155 2024-03-13 06:14:48.488185 accelbyte-py-sdk-service-sessionbrowser-0.8.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      888 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-sessionbrowser-0.8.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:14:48.484185 accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:14:48.484185 accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:14:48.484185 accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/
--rw-rw-r--   0 root         (0) root         (0)     2341 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:14:48.488185 accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/models/
--rw-rw-r--   0 root         (0) root         (0)     2844 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/models/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5372 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/models/models_active_custom_game_response.py
--rw-rw-r--   0 root         (0) root         (0)     5319 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/models/models_active_matchmaking_game_response.py
--rw-rw-r--   0 root         (0) root         (0)     4548 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/models/models_add_player_request.py
--rw-rw-r--   0 root         (0) root         (0)     3798 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/models/models_add_player_response.py
--rw-rw-r--   0 root         (0) root         (0)    14003 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/models/models_admin_session_response.py
--rw-rw-r--   0 root         (0) root         (0)     5408 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/models/models_count_active_session_response.py
--rw-rw-r--   0 root         (0) root         (0)     7362 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/models/models_create_session_request.py
--rw-rw-r--   0 root         (0) root         (0)    11056 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/models/models_custom_game_response.py
--rw-rw-r--   0 root         (0) root         (0)    13769 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/models/models_game_session.py
--rw-rw-r--   0 root         (0) root         (0)    10821 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/models/models_game_session_setting.py
--rw-rw-r--   0 root         (0) root         (0)    18913 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/models/models_get_session_history_detailed_response_item.py
--rw-rw-r--   0 root         (0) root         (0)    13401 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/models/models_get_session_history_search_response_item_v2.py
--rw-rw-r--   0 root         (0) root         (0)     5529 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/models/models_get_session_history_search_response_v2.py
--rw-rw-r--   0 root         (0) root         (0)     3882 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/models/models_join_game_session_request.py
--rw-rw-r--   0 root         (0) root         (0)     4137 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/models/models_match_attributes.py
--rw-rw-r--   0 root         (0) root         (0)    15432 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/models/models_match_making.py
--rw-rw-r--   0 root         (0) root         (0)     4293 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/models/models_matching_ally.py
--rw-rw-r--   0 root         (0) root         (0)     7026 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/models/models_matching_party.py
--rw-rw-r--   0 root         (0) root         (0)     5444 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/models/models_pagination.py
--rw-rw-r--   0 root         (0) root         (0)     4327 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/models/models_paging_cursor.py
--rw-rw-r--   0 root         (0) root         (0)     4704 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/models/models_party_member.py
--rw-rw-r--   0 root         (0) root         (0)     7449 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/models/models_recent_player_history.py
--rw-rw-r--   0 root         (0) root         (0)     4296 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/models/models_recent_player_query_response.py
--rw-rw-r--   0 root         (0) root         (0)    18558 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/models/models_server.py
--rw-rw-r--   0 root         (0) root         (0)     4192 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/models/models_session_by_user_i_ds_response.py
--rw-rw-r--   0 root         (0) root         (0)     5027 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/models/models_session_player_history.py
--rw-rw-r--   0 root         (0) root         (0)     5007 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/models/models_session_player_joining.py
--rw-rw-r--   0 root         (0) root         (0)     5196 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/models/models_session_query_response.py
--rw-rw-r--   0 root         (0) root         (0)    13882 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/models/models_session_response.py
--rw-rw-r--   0 root         (0) root         (0)     4408 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/models/models_status_history.py
--rw-rw-r--   0 root         (0) root         (0)     3997 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/models/models_update_session_request.py
--rw-rw-r--   0 root         (0) root         (0)     3902 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/models/models_update_settings_request.py
--rw-rw-r--   0 root         (0) root         (0)     4443 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/models/response_error.py
--rw-rw-r--   0 root         (0) root         (0)     6704 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/models/restapi_error_response_v2.py
--rw-rw-r--   0 root         (0) root         (0)     4456 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/models/restapi_error_v1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:14:48.488185 accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/operations/
--rw-rw-r--   0 root         (0) root         (0)      444 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/operations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:14:48.488185 accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/
--rw-rw-r--   0 root         (0) root         (0)     1539 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8271 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/add_player_to_session.py
--rw-rw-r--   0 root         (0) root         (0)     7206 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/admin_delete_session.py
--rw-rw-r--   0 root         (0) root         (0)     6937 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/admin_get_session.py
--rw-rw-r--   0 root         (0) root         (0)    14720 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/admin_query_session.py
--rw-rw-r--   0 root         (0) root         (0)    14569 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/admin_search_sessions_v2.py
--rw-rw-r--   0 root         (0) root         (0)     7783 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/create_session.py
--rw-rw-r--   0 root         (0) root         (0)     7033 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/delete_session.py
--rw-rw-r--   0 root         (0) root         (0)     7151 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/delete_session_local_ds.py
--rw-rw-r--   0 root         (0) root         (0)     9872 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/get_active_custom_game__cd6755.py
--rw-rw-r--   0 root         (0) root         (0)    10799 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/get_active_matchmaking__0b8050.py
--rw-rw-r--   0 root         (0) root         (0)     6812 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/get_recent_player.py
--rw-rw-r--   0 root         (0) root         (0)     6764 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/get_session.py
--rw-rw-r--   0 root         (0) root         (0)     6998 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/get_session_by_user_i_ds.py
--rw-rw-r--   0 root         (0) root         (0)     7836 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/get_session_history_detailed.py
--rw-rw-r--   0 root         (0) root         (0)     7303 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/get_total_active_session.py
--rw-rw-r--   0 root         (0) root         (0)     8610 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/join_session.py
--rw-rw-r--   0 root         (0) root         (0)     7995 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/remove_player_from_session.py
--rw-rw-r--   0 root         (0) root         (0)     8258 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/update_session.py
--rw-rw-r--   0 root         (0) root         (0)     8336 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/update_settings.py
--rw-rw-r--   0 root         (0) root         (0)    14664 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/user_query_session.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:14:48.488185 accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/wrappers/
--rw-rw-r--   0 root         (0) root         (0)     2331 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/wrappers/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    65640 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/wrappers/_session.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:14:48.488185 accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk_service_sessionbrowser.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1155 2024-03-13 06:14:48.000000 accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk_service_sessionbrowser.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4870 2024-03-13 06:14:48.000000 accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk_service_sessionbrowser.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-13 06:14:48.000000 accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk_service_sessionbrowser.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-13 06:14:48.000000 accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk_service_sessionbrowser.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-03-13 06:14:48.000000 accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk_service_sessionbrowser.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)      374 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-sessionbrowser-0.8.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-13 06:14:48.488185 accelbyte-py-sdk-service-sessionbrowser-0.8.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:44:57.695718 accelbyte-py-sdk-service-sessionbrowser-0.9.0/
+-rw-r--r--   0 root         (0) root         (0)     1155 2024-03-26 05:44:57.695718 accelbyte-py-sdk-service-sessionbrowser-0.9.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      888 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-sessionbrowser-0.9.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:44:57.691718 accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:44:57.691718 accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:44:57.691718 accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/
+-rw-rw-r--   0 root         (0) root         (0)     2341 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:44:57.695718 accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/models/
+-rw-rw-r--   0 root         (0) root         (0)     2844 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/models/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     5372 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/models/models_active_custom_game_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5399 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/models/models_active_matchmaking_game_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4548 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/models/models_add_player_request.py
+-rw-rw-r--   0 root         (0) root         (0)     3798 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/models/models_add_player_response.py
+-rw-rw-r--   0 root         (0) root         (0)    14122 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/models/models_admin_session_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5408 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/models/models_count_active_session_response.py
+-rw-rw-r--   0 root         (0) root         (0)     7362 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/models/models_create_session_request.py
+-rw-rw-r--   0 root         (0) root         (0)    11345 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/models/models_custom_game_response.py
+-rw-rw-r--   0 root         (0) root         (0)    14057 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/models/models_game_session.py
+-rw-rw-r--   0 root         (0) root         (0)    10876 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/models/models_game_session_setting.py
+-rw-rw-r--   0 root         (0) root         (0)    19083 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/models/models_get_session_history_detailed_response_item.py
+-rw-rw-r--   0 root         (0) root         (0)    13569 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/models/models_get_session_history_search_response_item_v2.py
+-rw-rw-r--   0 root         (0) root         (0)     5529 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/models/models_get_session_history_search_response_v2.py
+-rw-rw-r--   0 root         (0) root         (0)     3882 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/models/models_join_game_session_request.py
+-rw-rw-r--   0 root         (0) root         (0)     4137 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/models/models_match_attributes.py
+-rw-rw-r--   0 root         (0) root         (0)    15554 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/models/models_match_making.py
+-rw-rw-r--   0 root         (0) root         (0)     4356 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/models/models_matching_ally.py
+-rw-rw-r--   0 root         (0) root         (0)     7212 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/models/models_matching_party.py
+-rw-rw-r--   0 root         (0) root         (0)     5444 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/models/models_pagination.py
+-rw-rw-r--   0 root         (0) root         (0)     4327 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/models/models_paging_cursor.py
+-rw-rw-r--   0 root         (0) root         (0)     4767 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/models/models_party_member.py
+-rw-rw-r--   0 root         (0) root         (0)     7449 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/models/models_recent_player_history.py
+-rw-rw-r--   0 root         (0) root         (0)     4296 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/models/models_recent_player_query_response.py
+-rw-rw-r--   0 root         (0) root         (0)    18731 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/models/models_server.py
+-rw-rw-r--   0 root         (0) root         (0)     4192 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/models/models_session_by_user_i_ds_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5027 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/models/models_session_player_history.py
+-rw-rw-r--   0 root         (0) root         (0)     5007 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/models/models_session_player_joining.py
+-rw-rw-r--   0 root         (0) root         (0)     5196 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/models/models_session_query_response.py
+-rw-rw-r--   0 root         (0) root         (0)    13882 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/models/models_session_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4408 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/models/models_status_history.py
+-rw-rw-r--   0 root         (0) root         (0)     3997 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/models/models_update_session_request.py
+-rw-rw-r--   0 root         (0) root         (0)     3902 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/models/models_update_settings_request.py
+-rw-rw-r--   0 root         (0) root         (0)     4443 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/models/response_error.py
+-rw-rw-r--   0 root         (0) root         (0)     6704 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/models/restapi_error_response_v2.py
+-rw-rw-r--   0 root         (0) root         (0)     4456 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/models/restapi_error_v1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:44:57.695718 accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/operations/
+-rw-rw-r--   0 root         (0) root         (0)      444 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/operations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:44:57.695718 accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/
+-rw-rw-r--   0 root         (0) root         (0)     1539 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8271 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/add_player_to_session.py
+-rw-rw-r--   0 root         (0) root         (0)     7206 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/admin_delete_session.py
+-rw-rw-r--   0 root         (0) root         (0)     6937 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/admin_get_session.py
+-rw-rw-r--   0 root         (0) root         (0)    14720 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/admin_query_session.py
+-rw-rw-r--   0 root         (0) root         (0)    14569 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/admin_search_sessions_v2.py
+-rw-rw-r--   0 root         (0) root         (0)     7783 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/create_session.py
+-rw-rw-r--   0 root         (0) root         (0)     7033 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/delete_session.py
+-rw-rw-r--   0 root         (0) root         (0)     7151 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/delete_session_local_ds.py
+-rw-rw-r--   0 root         (0) root         (0)     9872 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/get_active_custom_game__cd6755.py
+-rw-rw-r--   0 root         (0) root         (0)    10799 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/get_active_matchmaking__0b8050.py
+-rw-rw-r--   0 root         (0) root         (0)     6812 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/get_recent_player.py
+-rw-rw-r--   0 root         (0) root         (0)     6764 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/get_session.py
+-rw-rw-r--   0 root         (0) root         (0)     6998 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/get_session_by_user_i_ds.py
+-rw-rw-r--   0 root         (0) root         (0)     7836 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/get_session_history_detailed.py
+-rw-rw-r--   0 root         (0) root         (0)     7303 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/get_total_active_session.py
+-rw-rw-r--   0 root         (0) root         (0)     8610 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/join_session.py
+-rw-rw-r--   0 root         (0) root         (0)     7995 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/remove_player_from_session.py
+-rw-rw-r--   0 root         (0) root         (0)     8258 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/update_session.py
+-rw-rw-r--   0 root         (0) root         (0)     8336 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/update_settings.py
+-rw-rw-r--   0 root         (0) root         (0)    14664 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/user_query_session.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:44:57.695718 accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/wrappers/
+-rw-rw-r--   0 root         (0) root         (0)     2331 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/wrappers/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    65640 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/wrappers/_session.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:44:57.695718 accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk_service_sessionbrowser.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1155 2024-03-26 05:44:57.000000 accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk_service_sessionbrowser.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4870 2024-03-26 05:44:57.000000 accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk_service_sessionbrowser.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-03-26 05:44:57.000000 accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk_service_sessionbrowser.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 05:44:57.000000 accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk_service_sessionbrowser.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-03-26 05:44:57.000000 accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk_service_sessionbrowser.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)      374 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-sessionbrowser-0.9.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-03-26 05:44:57.695718 accelbyte-py-sdk-service-sessionbrowser-0.9.0/setup.cfg
```

### Comparing `accelbyte-py-sdk-service-sessionbrowser-0.8.0/PKG-INFO` & `accelbyte-py-sdk-service-sessionbrowser-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: accelbyte-py-sdk-service-sessionbrowser
-Version: 0.8.0
+Version: 0.9.0
 Summary: AccelByte Python SDK - AccelByte Gaming Services Session Browser Service
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: accelbyte-py-sdk-core
 
 [//]: # (Code generated. DO NOT EDIT!)
```

### Comparing `accelbyte-py-sdk-service-sessionbrowser-0.8.0/README.md` & `accelbyte-py-sdk-service-sessionbrowser-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/__init__.py` & `accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/__init__.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/models/__init__.py` & `accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/models/__init__.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/models/models_active_custom_game_response.py` & `accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/models/models_active_custom_game_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/models/models_active_matchmaking_game_response.py` & `accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/models/models_active_matchmaking_game_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,21 +33,21 @@
 
 class ModelsActiveMatchmakingGameResponse(Model):
     """Models active matchmaking game response (models.ActiveMatchmakingGameResponse)
 
     Properties:
         pagination: (pagination) REQUIRED ModelsPagingCursor
 
-        sessions: (sessions) REQUIRED List[ModelsGameSession]
+        sessions: (sessions) OPTIONAL List[ModelsGameSession]
     """
 
     # region fields
 
     pagination: ModelsPagingCursor  # REQUIRED
-    sessions: List[ModelsGameSession]  # REQUIRED
+    sessions: List[ModelsGameSession]  # OPTIONAL
 
     # endregion fields
 
     # region with_x methods
 
     def with_pagination(
         self, value: ModelsPagingCursor
@@ -81,19 +81,23 @@
 
     # endregion to methods
 
     # region static methods
 
     @classmethod
     def create(
-        cls, pagination: ModelsPagingCursor, sessions: List[ModelsGameSession], **kwargs
+        cls,
+        pagination: ModelsPagingCursor,
+        sessions: Optional[List[ModelsGameSession]] = None,
+        **kwargs,
     ) -> ModelsActiveMatchmakingGameResponse:
         instance = cls()
         instance.pagination = pagination
-        instance.sessions = sessions
+        if sessions is not None:
+            instance.sessions = sessions
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
     ) -> ModelsActiveMatchmakingGameResponse:
         instance = cls()
@@ -159,11 +163,11 @@
             "sessions": "sessions",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
             "pagination": True,
-            "sessions": True,
+            "sessions": False,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/models/models_add_player_request.py` & `accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/models/models_add_player_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/models/models_add_player_response.py` & `accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/models/models_add_player_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/models/models_admin_session_response.py` & `accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/models/models_session_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,16 +28,16 @@
 from accelbyte_py_sdk.core import Model
 
 from ..models.models_game_session_setting import ModelsGameSessionSetting
 from ..models.models_match_making import ModelsMatchMaking
 from ..models.models_server import ModelsServer
 
 
-class ModelsAdminSessionResponse(Model):
-    """Models admin session response (models.AdminSessionResponse)
+class ModelsSessionResponse(Model):
+    """Models session response (models.SessionResponse)
 
     Properties:
         all_players: (all_players) REQUIRED List[str]
 
         created_at: (created_at) REQUIRED str
 
         game_session_setting: (game_session_setting) REQUIRED ModelsGameSessionSetting
@@ -82,69 +82,69 @@
     user_id: str  # REQUIRED
     username: str  # REQUIRED
 
     # endregion fields
 
     # region with_x methods
 
-    def with_all_players(self, value: List[str]) -> ModelsAdminSessionResponse:
+    def with_all_players(self, value: List[str]) -> ModelsSessionResponse:
         self.all_players = value
         return self
 
-    def with_created_at(self, value: str) -> ModelsAdminSessionResponse:
+    def with_created_at(self, value: str) -> ModelsSessionResponse:
         self.created_at = value
         return self
 
     def with_game_session_setting(
         self, value: ModelsGameSessionSetting
-    ) -> ModelsAdminSessionResponse:
+    ) -> ModelsSessionResponse:
         self.game_session_setting = value
         return self
 
-    def with_game_version(self, value: str) -> ModelsAdminSessionResponse:
+    def with_game_version(self, value: str) -> ModelsSessionResponse:
         self.game_version = value
         return self
 
-    def with_joinable(self, value: bool) -> ModelsAdminSessionResponse:
+    def with_joinable(self, value: bool) -> ModelsSessionResponse:
         self.joinable = value
         return self
 
-    def with_match(self, value: ModelsMatchMaking) -> ModelsAdminSessionResponse:
+    def with_match(self, value: ModelsMatchMaking) -> ModelsSessionResponse:
         self.match = value
         return self
 
-    def with_namespace(self, value: str) -> ModelsAdminSessionResponse:
+    def with_namespace(self, value: str) -> ModelsSessionResponse:
         self.namespace = value
         return self
 
-    def with_players(self, value: List[str]) -> ModelsAdminSessionResponse:
+    def with_players(self, value: List[str]) -> ModelsSessionResponse:
         self.players = value
         return self
 
-    def with_server(self, value: ModelsServer) -> ModelsAdminSessionResponse:
+    def with_server(self, value: ModelsServer) -> ModelsSessionResponse:
         self.server = value
         return self
 
-    def with_session_id(self, value: str) -> ModelsAdminSessionResponse:
+    def with_session_id(self, value: str) -> ModelsSessionResponse:
         self.session_id = value
         return self
 
-    def with_session_type(self, value: str) -> ModelsAdminSessionResponse:
+    def with_session_type(self, value: str) -> ModelsSessionResponse:
         self.session_type = value
         return self
 
-    def with_spectators(self, value: List[str]) -> ModelsAdminSessionResponse:
+    def with_spectators(self, value: List[str]) -> ModelsSessionResponse:
         self.spectators = value
         return self
 
-    def with_user_id(self, value: str) -> ModelsAdminSessionResponse:
+    def with_user_id(self, value: str) -> ModelsSessionResponse:
         self.user_id = value
         return self
 
-    def with_username(self, value: str) -> ModelsAdminSessionResponse:
+    def with_username(self, value: str) -> ModelsSessionResponse:
         self.username = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
@@ -228,15 +228,15 @@
         server: ModelsServer,
         session_id: str,
         session_type: str,
         spectators: List[str],
         user_id: str,
         username: str,
         **kwargs,
-    ) -> ModelsAdminSessionResponse:
+    ) -> ModelsSessionResponse:
         instance = cls()
         instance.all_players = all_players
         instance.created_at = created_at
         instance.game_session_setting = game_session_setting
         instance.game_version = game_version
         instance.joinable = joinable
         instance.match = match
@@ -249,15 +249,15 @@
         instance.user_id = user_id
         instance.username = username
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> ModelsAdminSessionResponse:
+    ) -> ModelsSessionResponse:
         instance = cls()
         if not dict_:
             return instance
         if "all_players" in dict_ and dict_["all_players"] is not None:
             instance.all_players = [str(i0) for i0 in dict_["all_players"]]
         elif include_empty:
             instance.all_players = []
@@ -323,38 +323,38 @@
         elif include_empty:
             instance.username = ""
         return instance
 
     @classmethod
     def create_many_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> Dict[str, ModelsAdminSessionResponse]:
+    ) -> Dict[str, ModelsSessionResponse]:
         return (
             {k: cls.create_from_dict(v, include_empty=include_empty) for k, v in dict_}
             if dict_
             else {}
         )
 
     @classmethod
     def create_many_from_list(
         cls, list_: list, include_empty: bool = False
-    ) -> List[ModelsAdminSessionResponse]:
+    ) -> List[ModelsSessionResponse]:
         return (
             [cls.create_from_dict(i, include_empty=include_empty) for i in list_]
             if list_
             else []
         )
 
     @classmethod
     def create_from_any(
         cls, any_: any, include_empty: bool = False, many: bool = False
     ) -> Union[
-        ModelsAdminSessionResponse,
-        List[ModelsAdminSessionResponse],
-        Dict[Any, ModelsAdminSessionResponse],
+        ModelsSessionResponse,
+        List[ModelsSessionResponse],
+        Dict[Any, ModelsSessionResponse],
     ]:
         if many:
             if isinstance(any_, dict):
                 return cls.create_many_from_dict(any_, include_empty=include_empty)
             elif isinstance(any_, list):
                 return cls.create_many_from_list(any_, include_empty=include_empty)
             else:
```

### Comparing `accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/models/models_count_active_session_response.py` & `accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/models/models_count_active_session_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/models/models_create_session_request.py` & `accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/models/models_create_session_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/models/models_custom_game_response.py` & `accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/models/models_custom_game_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,226 +31,231 @@
 from ..models.models_server import ModelsServer
 
 
 class ModelsCustomGameResponse(Model):
     """Models custom game response (models.CustomGameResponse)
 
     Properties:
-        all_players: (all_players) REQUIRED List[str]
-
         created_at: (created_at) REQUIRED str
 
-        game_session_setting: (game_session_setting) REQUIRED ModelsGameSessionSetting
-
         joinable: (joinable) REQUIRED bool
 
         namespace: (namespace) REQUIRED str
 
-        players: (players) REQUIRED List[str]
-
-        server: (server) REQUIRED ModelsServer
-
         session_id: (session_id) REQUIRED str
 
         session_type: (session_type) REQUIRED str
 
-        spectators: (spectators) REQUIRED List[str]
+        all_players: (all_players) OPTIONAL List[str]
+
+        game_session_setting: (game_session_setting) OPTIONAL ModelsGameSessionSetting
+
+        players: (players) OPTIONAL List[str]
+
+        server: (server) OPTIONAL ModelsServer
+
+        spectators: (spectators) OPTIONAL List[str]
     """
 
     # region fields
 
-    all_players: List[str]  # REQUIRED
     created_at: str  # REQUIRED
-    game_session_setting: ModelsGameSessionSetting  # REQUIRED
     joinable: bool  # REQUIRED
     namespace: str  # REQUIRED
-    players: List[str]  # REQUIRED
-    server: ModelsServer  # REQUIRED
     session_id: str  # REQUIRED
     session_type: str  # REQUIRED
-    spectators: List[str]  # REQUIRED
+    all_players: List[str]  # OPTIONAL
+    game_session_setting: ModelsGameSessionSetting  # OPTIONAL
+    players: List[str]  # OPTIONAL
+    server: ModelsServer  # OPTIONAL
+    spectators: List[str]  # OPTIONAL
 
     # endregion fields
 
     # region with_x methods
 
-    def with_all_players(self, value: List[str]) -> ModelsCustomGameResponse:
-        self.all_players = value
-        return self
-
     def with_created_at(self, value: str) -> ModelsCustomGameResponse:
         self.created_at = value
         return self
 
-    def with_game_session_setting(
-        self, value: ModelsGameSessionSetting
-    ) -> ModelsCustomGameResponse:
-        self.game_session_setting = value
-        return self
-
     def with_joinable(self, value: bool) -> ModelsCustomGameResponse:
         self.joinable = value
         return self
 
     def with_namespace(self, value: str) -> ModelsCustomGameResponse:
         self.namespace = value
         return self
 
-    def with_players(self, value: List[str]) -> ModelsCustomGameResponse:
-        self.players = value
-        return self
-
-    def with_server(self, value: ModelsServer) -> ModelsCustomGameResponse:
-        self.server = value
-        return self
-
     def with_session_id(self, value: str) -> ModelsCustomGameResponse:
         self.session_id = value
         return self
 
     def with_session_type(self, value: str) -> ModelsCustomGameResponse:
         self.session_type = value
         return self
 
+    def with_all_players(self, value: List[str]) -> ModelsCustomGameResponse:
+        self.all_players = value
+        return self
+
+    def with_game_session_setting(
+        self, value: ModelsGameSessionSetting
+    ) -> ModelsCustomGameResponse:
+        self.game_session_setting = value
+        return self
+
+    def with_players(self, value: List[str]) -> ModelsCustomGameResponse:
+        self.players = value
+        return self
+
+    def with_server(self, value: ModelsServer) -> ModelsCustomGameResponse:
+        self.server = value
+        return self
+
     def with_spectators(self, value: List[str]) -> ModelsCustomGameResponse:
         self.spectators = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
-        if hasattr(self, "all_players"):
-            result["all_players"] = [str(i0) for i0 in self.all_players]
-        elif include_empty:
-            result["all_players"] = []
         if hasattr(self, "created_at"):
             result["created_at"] = str(self.created_at)
         elif include_empty:
             result["created_at"] = ""
-        if hasattr(self, "game_session_setting"):
-            result["game_session_setting"] = self.game_session_setting.to_dict(
-                include_empty=include_empty
-            )
-        elif include_empty:
-            result["game_session_setting"] = ModelsGameSessionSetting()
         if hasattr(self, "joinable"):
             result["joinable"] = bool(self.joinable)
         elif include_empty:
             result["joinable"] = False
         if hasattr(self, "namespace"):
             result["namespace"] = str(self.namespace)
         elif include_empty:
             result["namespace"] = ""
-        if hasattr(self, "players"):
-            result["players"] = [str(i0) for i0 in self.players]
-        elif include_empty:
-            result["players"] = []
-        if hasattr(self, "server"):
-            result["server"] = self.server.to_dict(include_empty=include_empty)
-        elif include_empty:
-            result["server"] = ModelsServer()
         if hasattr(self, "session_id"):
             result["session_id"] = str(self.session_id)
         elif include_empty:
             result["session_id"] = ""
         if hasattr(self, "session_type"):
             result["session_type"] = str(self.session_type)
         elif include_empty:
             result["session_type"] = ""
+        if hasattr(self, "all_players"):
+            result["all_players"] = [str(i0) for i0 in self.all_players]
+        elif include_empty:
+            result["all_players"] = []
+        if hasattr(self, "game_session_setting"):
+            result["game_session_setting"] = self.game_session_setting.to_dict(
+                include_empty=include_empty
+            )
+        elif include_empty:
+            result["game_session_setting"] = ModelsGameSessionSetting()
+        if hasattr(self, "players"):
+            result["players"] = [str(i0) for i0 in self.players]
+        elif include_empty:
+            result["players"] = []
+        if hasattr(self, "server"):
+            result["server"] = self.server.to_dict(include_empty=include_empty)
+        elif include_empty:
+            result["server"] = ModelsServer()
         if hasattr(self, "spectators"):
             result["spectators"] = [str(i0) for i0 in self.spectators]
         elif include_empty:
             result["spectators"] = []
         return result
 
     # endregion to methods
 
     # region static methods
 
     @classmethod
     def create(
         cls,
-        all_players: List[str],
         created_at: str,
-        game_session_setting: ModelsGameSessionSetting,
         joinable: bool,
         namespace: str,
-        players: List[str],
-        server: ModelsServer,
         session_id: str,
         session_type: str,
-        spectators: List[str],
+        all_players: Optional[List[str]] = None,
+        game_session_setting: Optional[ModelsGameSessionSetting] = None,
+        players: Optional[List[str]] = None,
+        server: Optional[ModelsServer] = None,
+        spectators: Optional[List[str]] = None,
         **kwargs,
     ) -> ModelsCustomGameResponse:
         instance = cls()
-        instance.all_players = all_players
         instance.created_at = created_at
-        instance.game_session_setting = game_session_setting
         instance.joinable = joinable
         instance.namespace = namespace
-        instance.players = players
-        instance.server = server
         instance.session_id = session_id
         instance.session_type = session_type
-        instance.spectators = spectators
+        if all_players is not None:
+            instance.all_players = all_players
+        if game_session_setting is not None:
+            instance.game_session_setting = game_session_setting
+        if players is not None:
+            instance.players = players
+        if server is not None:
+            instance.server = server
+        if spectators is not None:
+            instance.spectators = spectators
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
     ) -> ModelsCustomGameResponse:
         instance = cls()
         if not dict_:
             return instance
-        if "all_players" in dict_ and dict_["all_players"] is not None:
-            instance.all_players = [str(i0) for i0 in dict_["all_players"]]
-        elif include_empty:
-            instance.all_players = []
         if "created_at" in dict_ and dict_["created_at"] is not None:
             instance.created_at = str(dict_["created_at"])
         elif include_empty:
             instance.created_at = ""
+        if "joinable" in dict_ and dict_["joinable"] is not None:
+            instance.joinable = bool(dict_["joinable"])
+        elif include_empty:
+            instance.joinable = False
+        if "namespace" in dict_ and dict_["namespace"] is not None:
+            instance.namespace = str(dict_["namespace"])
+        elif include_empty:
+            instance.namespace = ""
+        if "session_id" in dict_ and dict_["session_id"] is not None:
+            instance.session_id = str(dict_["session_id"])
+        elif include_empty:
+            instance.session_id = ""
+        if "session_type" in dict_ and dict_["session_type"] is not None:
+            instance.session_type = str(dict_["session_type"])
+        elif include_empty:
+            instance.session_type = ""
+        if "all_players" in dict_ and dict_["all_players"] is not None:
+            instance.all_players = [str(i0) for i0 in dict_["all_players"]]
+        elif include_empty:
+            instance.all_players = []
         if (
             "game_session_setting" in dict_
             and dict_["game_session_setting"] is not None
         ):
             instance.game_session_setting = ModelsGameSessionSetting.create_from_dict(
                 dict_["game_session_setting"], include_empty=include_empty
             )
         elif include_empty:
             instance.game_session_setting = ModelsGameSessionSetting()
-        if "joinable" in dict_ and dict_["joinable"] is not None:
-            instance.joinable = bool(dict_["joinable"])
-        elif include_empty:
-            instance.joinable = False
-        if "namespace" in dict_ and dict_["namespace"] is not None:
-            instance.namespace = str(dict_["namespace"])
-        elif include_empty:
-            instance.namespace = ""
         if "players" in dict_ and dict_["players"] is not None:
             instance.players = [str(i0) for i0 in dict_["players"]]
         elif include_empty:
             instance.players = []
         if "server" in dict_ and dict_["server"] is not None:
             instance.server = ModelsServer.create_from_dict(
                 dict_["server"], include_empty=include_empty
             )
         elif include_empty:
             instance.server = ModelsServer()
-        if "session_id" in dict_ and dict_["session_id"] is not None:
-            instance.session_id = str(dict_["session_id"])
-        elif include_empty:
-            instance.session_id = ""
-        if "session_type" in dict_ and dict_["session_type"] is not None:
-            instance.session_type = str(dict_["session_type"])
-        elif include_empty:
-            instance.session_type = ""
         if "spectators" in dict_ and dict_["spectators"] is not None:
             instance.spectators = [str(i0) for i0 in dict_["spectators"]]
         elif include_empty:
             instance.spectators = []
         return instance
 
     @classmethod
@@ -290,35 +295,35 @@
                 raise ValueError()
         else:
             return cls.create_from_dict(any_, include_empty=include_empty)
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
-            "all_players": "all_players",
             "created_at": "created_at",
-            "game_session_setting": "game_session_setting",
             "joinable": "joinable",
             "namespace": "namespace",
-            "players": "players",
-            "server": "server",
             "session_id": "session_id",
             "session_type": "session_type",
+            "all_players": "all_players",
+            "game_session_setting": "game_session_setting",
+            "players": "players",
+            "server": "server",
             "spectators": "spectators",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
-            "all_players": True,
             "created_at": True,
-            "game_session_setting": True,
             "joinable": True,
             "namespace": True,
-            "players": True,
-            "server": True,
             "session_id": True,
             "session_type": True,
-            "spectators": True,
+            "all_players": False,
+            "game_session_setting": False,
+            "players": False,
+            "server": False,
+            "spectators": False,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/models/models_game_session.py` & `accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/models/models_game_session.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,300 +32,305 @@
 from ..models.models_server import ModelsServer
 
 
 class ModelsGameSession(Model):
     """Models game session (models.GameSession)
 
     Properties:
-        all_players: (all_players) REQUIRED List[str]
-
         created_at: (created_at) REQUIRED str
 
-        game_session_setting: (game_session_setting) REQUIRED ModelsGameSessionSetting
-
         game_version: (game_version) REQUIRED str
 
         joinable: (joinable) REQUIRED bool
 
-        match: (match) REQUIRED ModelsMatchMaking
-
         namespace: (namespace) REQUIRED str
 
-        players: (players) REQUIRED List[str]
-
         server: (server) REQUIRED ModelsServer
 
         session_id: (session_id) REQUIRED str
 
         session_type: (session_type) REQUIRED str
 
-        spectators: (spectators) REQUIRED List[str]
-
         user_id: (user_id) REQUIRED str
 
         username: (username) REQUIRED str
+
+        all_players: (all_players) OPTIONAL List[str]
+
+        game_session_setting: (game_session_setting) OPTIONAL ModelsGameSessionSetting
+
+        match: (match) OPTIONAL ModelsMatchMaking
+
+        players: (players) OPTIONAL List[str]
+
+        spectators: (spectators) OPTIONAL List[str]
     """
 
     # region fields
 
-    all_players: List[str]  # REQUIRED
     created_at: str  # REQUIRED
-    game_session_setting: ModelsGameSessionSetting  # REQUIRED
     game_version: str  # REQUIRED
     joinable: bool  # REQUIRED
-    match: ModelsMatchMaking  # REQUIRED
     namespace: str  # REQUIRED
-    players: List[str]  # REQUIRED
     server: ModelsServer  # REQUIRED
     session_id: str  # REQUIRED
     session_type: str  # REQUIRED
-    spectators: List[str]  # REQUIRED
     user_id: str  # REQUIRED
     username: str  # REQUIRED
+    all_players: List[str]  # OPTIONAL
+    game_session_setting: ModelsGameSessionSetting  # OPTIONAL
+    match: ModelsMatchMaking  # OPTIONAL
+    players: List[str]  # OPTIONAL
+    spectators: List[str]  # OPTIONAL
 
     # endregion fields
 
     # region with_x methods
 
-    def with_all_players(self, value: List[str]) -> ModelsGameSession:
-        self.all_players = value
-        return self
-
     def with_created_at(self, value: str) -> ModelsGameSession:
         self.created_at = value
         return self
 
-    def with_game_session_setting(
-        self, value: ModelsGameSessionSetting
-    ) -> ModelsGameSession:
-        self.game_session_setting = value
-        return self
-
     def with_game_version(self, value: str) -> ModelsGameSession:
         self.game_version = value
         return self
 
     def with_joinable(self, value: bool) -> ModelsGameSession:
         self.joinable = value
         return self
 
-    def with_match(self, value: ModelsMatchMaking) -> ModelsGameSession:
-        self.match = value
-        return self
-
     def with_namespace(self, value: str) -> ModelsGameSession:
         self.namespace = value
         return self
 
-    def with_players(self, value: List[str]) -> ModelsGameSession:
-        self.players = value
-        return self
-
     def with_server(self, value: ModelsServer) -> ModelsGameSession:
         self.server = value
         return self
 
     def with_session_id(self, value: str) -> ModelsGameSession:
         self.session_id = value
         return self
 
     def with_session_type(self, value: str) -> ModelsGameSession:
         self.session_type = value
         return self
 
-    def with_spectators(self, value: List[str]) -> ModelsGameSession:
-        self.spectators = value
-        return self
-
     def with_user_id(self, value: str) -> ModelsGameSession:
         self.user_id = value
         return self
 
     def with_username(self, value: str) -> ModelsGameSession:
         self.username = value
         return self
 
+    def with_all_players(self, value: List[str]) -> ModelsGameSession:
+        self.all_players = value
+        return self
+
+    def with_game_session_setting(
+        self, value: ModelsGameSessionSetting
+    ) -> ModelsGameSession:
+        self.game_session_setting = value
+        return self
+
+    def with_match(self, value: ModelsMatchMaking) -> ModelsGameSession:
+        self.match = value
+        return self
+
+    def with_players(self, value: List[str]) -> ModelsGameSession:
+        self.players = value
+        return self
+
+    def with_spectators(self, value: List[str]) -> ModelsGameSession:
+        self.spectators = value
+        return self
+
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
-        if hasattr(self, "all_players"):
-            result["all_players"] = [str(i0) for i0 in self.all_players]
-        elif include_empty:
-            result["all_players"] = []
         if hasattr(self, "created_at"):
             result["created_at"] = str(self.created_at)
         elif include_empty:
             result["created_at"] = ""
-        if hasattr(self, "game_session_setting"):
-            result["game_session_setting"] = self.game_session_setting.to_dict(
-                include_empty=include_empty
-            )
-        elif include_empty:
-            result["game_session_setting"] = ModelsGameSessionSetting()
         if hasattr(self, "game_version"):
             result["game_version"] = str(self.game_version)
         elif include_empty:
             result["game_version"] = ""
         if hasattr(self, "joinable"):
             result["joinable"] = bool(self.joinable)
         elif include_empty:
             result["joinable"] = False
-        if hasattr(self, "match"):
-            result["match"] = self.match.to_dict(include_empty=include_empty)
-        elif include_empty:
-            result["match"] = ModelsMatchMaking()
         if hasattr(self, "namespace"):
             result["namespace"] = str(self.namespace)
         elif include_empty:
             result["namespace"] = ""
-        if hasattr(self, "players"):
-            result["players"] = [str(i0) for i0 in self.players]
-        elif include_empty:
-            result["players"] = []
         if hasattr(self, "server"):
             result["server"] = self.server.to_dict(include_empty=include_empty)
         elif include_empty:
             result["server"] = ModelsServer()
         if hasattr(self, "session_id"):
             result["session_id"] = str(self.session_id)
         elif include_empty:
             result["session_id"] = ""
         if hasattr(self, "session_type"):
             result["session_type"] = str(self.session_type)
         elif include_empty:
             result["session_type"] = ""
-        if hasattr(self, "spectators"):
-            result["spectators"] = [str(i0) for i0 in self.spectators]
-        elif include_empty:
-            result["spectators"] = []
         if hasattr(self, "user_id"):
             result["user_id"] = str(self.user_id)
         elif include_empty:
             result["user_id"] = ""
         if hasattr(self, "username"):
             result["username"] = str(self.username)
         elif include_empty:
             result["username"] = ""
+        if hasattr(self, "all_players"):
+            result["all_players"] = [str(i0) for i0 in self.all_players]
+        elif include_empty:
+            result["all_players"] = []
+        if hasattr(self, "game_session_setting"):
+            result["game_session_setting"] = self.game_session_setting.to_dict(
+                include_empty=include_empty
+            )
+        elif include_empty:
+            result["game_session_setting"] = ModelsGameSessionSetting()
+        if hasattr(self, "match"):
+            result["match"] = self.match.to_dict(include_empty=include_empty)
+        elif include_empty:
+            result["match"] = ModelsMatchMaking()
+        if hasattr(self, "players"):
+            result["players"] = [str(i0) for i0 in self.players]
+        elif include_empty:
+            result["players"] = []
+        if hasattr(self, "spectators"):
+            result["spectators"] = [str(i0) for i0 in self.spectators]
+        elif include_empty:
+            result["spectators"] = []
         return result
 
     # endregion to methods
 
     # region static methods
 
     @classmethod
     def create(
         cls,
-        all_players: List[str],
         created_at: str,
-        game_session_setting: ModelsGameSessionSetting,
         game_version: str,
         joinable: bool,
-        match: ModelsMatchMaking,
         namespace: str,
-        players: List[str],
         server: ModelsServer,
         session_id: str,
         session_type: str,
-        spectators: List[str],
         user_id: str,
         username: str,
+        all_players: Optional[List[str]] = None,
+        game_session_setting: Optional[ModelsGameSessionSetting] = None,
+        match: Optional[ModelsMatchMaking] = None,
+        players: Optional[List[str]] = None,
+        spectators: Optional[List[str]] = None,
         **kwargs,
     ) -> ModelsGameSession:
         instance = cls()
-        instance.all_players = all_players
         instance.created_at = created_at
-        instance.game_session_setting = game_session_setting
         instance.game_version = game_version
         instance.joinable = joinable
-        instance.match = match
         instance.namespace = namespace
-        instance.players = players
         instance.server = server
         instance.session_id = session_id
         instance.session_type = session_type
-        instance.spectators = spectators
         instance.user_id = user_id
         instance.username = username
+        if all_players is not None:
+            instance.all_players = all_players
+        if game_session_setting is not None:
+            instance.game_session_setting = game_session_setting
+        if match is not None:
+            instance.match = match
+        if players is not None:
+            instance.players = players
+        if spectators is not None:
+            instance.spectators = spectators
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
     ) -> ModelsGameSession:
         instance = cls()
         if not dict_:
             return instance
-        if "all_players" in dict_ and dict_["all_players"] is not None:
-            instance.all_players = [str(i0) for i0 in dict_["all_players"]]
-        elif include_empty:
-            instance.all_players = []
         if "created_at" in dict_ and dict_["created_at"] is not None:
             instance.created_at = str(dict_["created_at"])
         elif include_empty:
             instance.created_at = ""
-        if (
-            "game_session_setting" in dict_
-            and dict_["game_session_setting"] is not None
-        ):
-            instance.game_session_setting = ModelsGameSessionSetting.create_from_dict(
-                dict_["game_session_setting"], include_empty=include_empty
-            )
-        elif include_empty:
-            instance.game_session_setting = ModelsGameSessionSetting()
         if "game_version" in dict_ and dict_["game_version"] is not None:
             instance.game_version = str(dict_["game_version"])
         elif include_empty:
             instance.game_version = ""
         if "joinable" in dict_ and dict_["joinable"] is not None:
             instance.joinable = bool(dict_["joinable"])
         elif include_empty:
             instance.joinable = False
-        if "match" in dict_ and dict_["match"] is not None:
-            instance.match = ModelsMatchMaking.create_from_dict(
-                dict_["match"], include_empty=include_empty
-            )
-        elif include_empty:
-            instance.match = ModelsMatchMaking()
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
         elif include_empty:
             instance.namespace = ""
-        if "players" in dict_ and dict_["players"] is not None:
-            instance.players = [str(i0) for i0 in dict_["players"]]
-        elif include_empty:
-            instance.players = []
         if "server" in dict_ and dict_["server"] is not None:
             instance.server = ModelsServer.create_from_dict(
                 dict_["server"], include_empty=include_empty
             )
         elif include_empty:
             instance.server = ModelsServer()
         if "session_id" in dict_ and dict_["session_id"] is not None:
             instance.session_id = str(dict_["session_id"])
         elif include_empty:
             instance.session_id = ""
         if "session_type" in dict_ and dict_["session_type"] is not None:
             instance.session_type = str(dict_["session_type"])
         elif include_empty:
             instance.session_type = ""
-        if "spectators" in dict_ and dict_["spectators"] is not None:
-            instance.spectators = [str(i0) for i0 in dict_["spectators"]]
-        elif include_empty:
-            instance.spectators = []
         if "user_id" in dict_ and dict_["user_id"] is not None:
             instance.user_id = str(dict_["user_id"])
         elif include_empty:
             instance.user_id = ""
         if "username" in dict_ and dict_["username"] is not None:
             instance.username = str(dict_["username"])
         elif include_empty:
             instance.username = ""
+        if "all_players" in dict_ and dict_["all_players"] is not None:
+            instance.all_players = [str(i0) for i0 in dict_["all_players"]]
+        elif include_empty:
+            instance.all_players = []
+        if (
+            "game_session_setting" in dict_
+            and dict_["game_session_setting"] is not None
+        ):
+            instance.game_session_setting = ModelsGameSessionSetting.create_from_dict(
+                dict_["game_session_setting"], include_empty=include_empty
+            )
+        elif include_empty:
+            instance.game_session_setting = ModelsGameSessionSetting()
+        if "match" in dict_ and dict_["match"] is not None:
+            instance.match = ModelsMatchMaking.create_from_dict(
+                dict_["match"], include_empty=include_empty
+            )
+        elif include_empty:
+            instance.match = ModelsMatchMaking()
+        if "players" in dict_ and dict_["players"] is not None:
+            instance.players = [str(i0) for i0 in dict_["players"]]
+        elif include_empty:
+            instance.players = []
+        if "spectators" in dict_ and dict_["spectators"] is not None:
+            instance.spectators = [str(i0) for i0 in dict_["spectators"]]
+        elif include_empty:
+            instance.spectators = []
         return instance
 
     @classmethod
     def create_many_from_dict(
         cls, dict_: dict, include_empty: bool = False
     ) -> Dict[str, ModelsGameSession]:
         return (
@@ -359,43 +364,43 @@
                 raise ValueError()
         else:
             return cls.create_from_dict(any_, include_empty=include_empty)
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
-            "all_players": "all_players",
             "created_at": "created_at",
-            "game_session_setting": "game_session_setting",
             "game_version": "game_version",
             "joinable": "joinable",
-            "match": "match",
             "namespace": "namespace",
-            "players": "players",
             "server": "server",
             "session_id": "session_id",
             "session_type": "session_type",
-            "spectators": "spectators",
             "user_id": "user_id",
             "username": "username",
+            "all_players": "all_players",
+            "game_session_setting": "game_session_setting",
+            "match": "match",
+            "players": "players",
+            "spectators": "spectators",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
-            "all_players": True,
             "created_at": True,
-            "game_session_setting": True,
             "game_version": True,
             "joinable": True,
-            "match": True,
             "namespace": True,
-            "players": True,
             "server": True,
             "session_id": True,
             "session_type": True,
-            "spectators": True,
             "user_id": True,
             "username": True,
+            "all_players": False,
+            "game_session_setting": False,
+            "match": False,
+            "players": False,
+            "spectators": False,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/models/models_game_session_setting.py` & `accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/models/models_game_session_setting.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,29 +46,29 @@
 
         mode: (mode) REQUIRED str
 
         num_bot: (num_bot) REQUIRED int
 
         password: (password) REQUIRED str
 
-        settings: (settings) REQUIRED Dict[str, Any]
+        settings: (settings) OPTIONAL Dict[str, Any]
     """
 
     # region fields
 
     allow_join_in_progress: bool  # REQUIRED
     current_internal_player: int  # REQUIRED
     current_player: int  # REQUIRED
     map_name: str  # REQUIRED
     max_internal_player: int  # REQUIRED
     max_player: int  # REQUIRED
     mode: str  # REQUIRED
     num_bot: int  # REQUIRED
     password: str  # REQUIRED
-    settings: Dict[str, Any]  # REQUIRED
+    settings: Dict[str, Any]  # OPTIONAL
 
     # endregion fields
 
     # region with_x methods
 
     def with_allow_join_in_progress(self, value: bool) -> ModelsGameSessionSetting:
         self.allow_join_in_progress = value
@@ -170,28 +170,29 @@
         current_player: int,
         map_name: str,
         max_internal_player: int,
         max_player: int,
         mode: str,
         num_bot: int,
         password: str,
-        settings: Dict[str, Any],
+        settings: Optional[Dict[str, Any]] = None,
         **kwargs,
     ) -> ModelsGameSessionSetting:
         instance = cls()
         instance.allow_join_in_progress = allow_join_in_progress
         instance.current_internal_player = current_internal_player
         instance.current_player = current_player
         instance.map_name = map_name
         instance.max_internal_player = max_internal_player
         instance.max_player = max_player
         instance.mode = mode
         instance.num_bot = num_bot
         instance.password = password
-        instance.settings = settings
+        if settings is not None:
+            instance.settings = settings
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
     ) -> ModelsGameSessionSetting:
         instance = cls()
@@ -306,11 +307,11 @@
             "current_player": True,
             "map_name": True,
             "max_internal_player": True,
             "max_player": True,
             "mode": True,
             "num_bot": True,
             "password": True,
-            "settings": True,
+            "settings": False,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/models/models_get_session_history_detailed_response_item.py` & `accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/models/models_get_session_history_detailed_response_item.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,61 +48,61 @@
 
         game_mode: (game_mode) REQUIRED str
 
         id_: (_id) REQUIRED str
 
         joinable: (joinable) REQUIRED bool
 
-        joining: (joining) REQUIRED List[ModelsSessionPlayerJoining]
-
         match_id: (match_id) REQUIRED str
 
-        matching_allies: (matching_allies) REQUIRED List[ModelsMatchingAlly]
-
         namespace: (namespace) REQUIRED str
 
-        players: (players) REQUIRED List[ModelsSessionPlayerHistory]
-
         region: (region) REQUIRED str
 
         removed_reason: (removed_reason) REQUIRED str
 
         server_name: (server_name) REQUIRED str
 
         session_type: (session_type) REQUIRED str
 
         status: (status) REQUIRED str
 
         user_id: (user_id) REQUIRED str
 
+        joining: (joining) OPTIONAL List[ModelsSessionPlayerJoining]
+
+        matching_allies: (matching_allies) OPTIONAL List[ModelsMatchingAlly]
+
         party_id: (party_id) OPTIONAL str
+
+        players: (players) OPTIONAL List[ModelsSessionPlayerHistory]
     """
 
     # region fields
 
     channel: str  # REQUIRED
     client_version: str  # REQUIRED
     created_at: str  # REQUIRED
     event_description: str  # REQUIRED
     event_name: str  # REQUIRED
     game_mode: str  # REQUIRED
     id_: str  # REQUIRED
     joinable: bool  # REQUIRED
-    joining: List[ModelsSessionPlayerJoining]  # REQUIRED
     match_id: str  # REQUIRED
-    matching_allies: List[ModelsMatchingAlly]  # REQUIRED
     namespace: str  # REQUIRED
-    players: List[ModelsSessionPlayerHistory]  # REQUIRED
     region: str  # REQUIRED
     removed_reason: str  # REQUIRED
     server_name: str  # REQUIRED
     session_type: str  # REQUIRED
     status: str  # REQUIRED
     user_id: str  # REQUIRED
+    joining: List[ModelsSessionPlayerJoining]  # OPTIONAL
+    matching_allies: List[ModelsMatchingAlly]  # OPTIONAL
     party_id: str  # OPTIONAL
+    players: List[ModelsSessionPlayerHistory]  # OPTIONAL
 
     # endregion fields
 
     # region with_x methods
 
     def with_channel(self, value: str) -> ModelsGetSessionHistoryDetailedResponseItem:
         self.channel = value
@@ -140,40 +140,22 @@
         self.id_ = value
         return self
 
     def with_joinable(self, value: bool) -> ModelsGetSessionHistoryDetailedResponseItem:
         self.joinable = value
         return self
 
-    def with_joining(
-        self, value: List[ModelsSessionPlayerJoining]
-    ) -> ModelsGetSessionHistoryDetailedResponseItem:
-        self.joining = value
-        return self
-
     def with_match_id(self, value: str) -> ModelsGetSessionHistoryDetailedResponseItem:
         self.match_id = value
         return self
 
-    def with_matching_allies(
-        self, value: List[ModelsMatchingAlly]
-    ) -> ModelsGetSessionHistoryDetailedResponseItem:
-        self.matching_allies = value
-        return self
-
     def with_namespace(self, value: str) -> ModelsGetSessionHistoryDetailedResponseItem:
         self.namespace = value
         return self
 
-    def with_players(
-        self, value: List[ModelsSessionPlayerHistory]
-    ) -> ModelsGetSessionHistoryDetailedResponseItem:
-        self.players = value
-        return self
-
     def with_region(self, value: str) -> ModelsGetSessionHistoryDetailedResponseItem:
         self.region = value
         return self
 
     def with_removed_reason(
         self, value: str
     ) -> ModelsGetSessionHistoryDetailedResponseItem:
@@ -196,18 +178,36 @@
         self.status = value
         return self
 
     def with_user_id(self, value: str) -> ModelsGetSessionHistoryDetailedResponseItem:
         self.user_id = value
         return self
 
+    def with_joining(
+        self, value: List[ModelsSessionPlayerJoining]
+    ) -> ModelsGetSessionHistoryDetailedResponseItem:
+        self.joining = value
+        return self
+
+    def with_matching_allies(
+        self, value: List[ModelsMatchingAlly]
+    ) -> ModelsGetSessionHistoryDetailedResponseItem:
+        self.matching_allies = value
+        return self
+
     def with_party_id(self, value: str) -> ModelsGetSessionHistoryDetailedResponseItem:
         self.party_id = value
         return self
 
+    def with_players(
+        self, value: List[ModelsSessionPlayerHistory]
+    ) -> ModelsGetSessionHistoryDetailedResponseItem:
+        self.players = value
+        return self
+
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
         if hasattr(self, "channel"):
@@ -238,40 +238,22 @@
             result["_id"] = str(self.id_)
         elif include_empty:
             result["_id"] = ""
         if hasattr(self, "joinable"):
             result["joinable"] = bool(self.joinable)
         elif include_empty:
             result["joinable"] = False
-        if hasattr(self, "joining"):
-            result["joining"] = [
-                i0.to_dict(include_empty=include_empty) for i0 in self.joining
-            ]
-        elif include_empty:
-            result["joining"] = []
         if hasattr(self, "match_id"):
             result["match_id"] = str(self.match_id)
         elif include_empty:
             result["match_id"] = ""
-        if hasattr(self, "matching_allies"):
-            result["matching_allies"] = [
-                i0.to_dict(include_empty=include_empty) for i0 in self.matching_allies
-            ]
-        elif include_empty:
-            result["matching_allies"] = []
         if hasattr(self, "namespace"):
             result["namespace"] = str(self.namespace)
         elif include_empty:
             result["namespace"] = ""
-        if hasattr(self, "players"):
-            result["players"] = [
-                i0.to_dict(include_empty=include_empty) for i0 in self.players
-            ]
-        elif include_empty:
-            result["players"] = []
         if hasattr(self, "region"):
             result["region"] = str(self.region)
         elif include_empty:
             result["region"] = ""
         if hasattr(self, "removed_reason"):
             result["removed_reason"] = str(self.removed_reason)
         elif include_empty:
@@ -288,18 +270,36 @@
             result["status"] = str(self.status)
         elif include_empty:
             result["status"] = ""
         if hasattr(self, "user_id"):
             result["user_id"] = str(self.user_id)
         elif include_empty:
             result["user_id"] = ""
+        if hasattr(self, "joining"):
+            result["joining"] = [
+                i0.to_dict(include_empty=include_empty) for i0 in self.joining
+            ]
+        elif include_empty:
+            result["joining"] = []
+        if hasattr(self, "matching_allies"):
+            result["matching_allies"] = [
+                i0.to_dict(include_empty=include_empty) for i0 in self.matching_allies
+            ]
+        elif include_empty:
+            result["matching_allies"] = []
         if hasattr(self, "party_id"):
             result["party_id"] = str(self.party_id)
         elif include_empty:
             result["party_id"] = ""
+        if hasattr(self, "players"):
+            result["players"] = [
+                i0.to_dict(include_empty=include_empty) for i0 in self.players
+            ]
+        elif include_empty:
+            result["players"] = []
         return result
 
     # endregion to methods
 
     # region static methods
 
     @classmethod
@@ -309,50 +309,53 @@
         client_version: str,
         created_at: str,
         event_description: str,
         event_name: str,
         game_mode: str,
         id_: str,
         joinable: bool,
-        joining: List[ModelsSessionPlayerJoining],
         match_id: str,
-        matching_allies: List[ModelsMatchingAlly],
         namespace: str,
-        players: List[ModelsSessionPlayerHistory],
         region: str,
         removed_reason: str,
         server_name: str,
         session_type: str,
         status: str,
         user_id: str,
+        joining: Optional[List[ModelsSessionPlayerJoining]] = None,
+        matching_allies: Optional[List[ModelsMatchingAlly]] = None,
         party_id: Optional[str] = None,
+        players: Optional[List[ModelsSessionPlayerHistory]] = None,
         **kwargs,
     ) -> ModelsGetSessionHistoryDetailedResponseItem:
         instance = cls()
         instance.channel = channel
         instance.client_version = client_version
         instance.created_at = created_at
         instance.event_description = event_description
         instance.event_name = event_name
         instance.game_mode = game_mode
         instance.id_ = id_
         instance.joinable = joinable
-        instance.joining = joining
         instance.match_id = match_id
-        instance.matching_allies = matching_allies
         instance.namespace = namespace
-        instance.players = players
         instance.region = region
         instance.removed_reason = removed_reason
         instance.server_name = server_name
         instance.session_type = session_type
         instance.status = status
         instance.user_id = user_id
+        if joining is not None:
+            instance.joining = joining
+        if matching_allies is not None:
+            instance.matching_allies = matching_allies
         if party_id is not None:
             instance.party_id = party_id
+        if players is not None:
+            instance.players = players
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
     ) -> ModelsGetSessionHistoryDetailedResponseItem:
         instance = cls()
@@ -386,47 +389,22 @@
             instance.id_ = str(dict_["_id"])
         elif include_empty:
             instance.id_ = ""
         if "joinable" in dict_ and dict_["joinable"] is not None:
             instance.joinable = bool(dict_["joinable"])
         elif include_empty:
             instance.joinable = False
-        if "joining" in dict_ and dict_["joining"] is not None:
-            instance.joining = [
-                ModelsSessionPlayerJoining.create_from_dict(
-                    i0, include_empty=include_empty
-                )
-                for i0 in dict_["joining"]
-            ]
-        elif include_empty:
-            instance.joining = []
         if "match_id" in dict_ and dict_["match_id"] is not None:
             instance.match_id = str(dict_["match_id"])
         elif include_empty:
             instance.match_id = ""
-        if "matching_allies" in dict_ and dict_["matching_allies"] is not None:
-            instance.matching_allies = [
-                ModelsMatchingAlly.create_from_dict(i0, include_empty=include_empty)
-                for i0 in dict_["matching_allies"]
-            ]
-        elif include_empty:
-            instance.matching_allies = []
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
         elif include_empty:
             instance.namespace = ""
-        if "players" in dict_ and dict_["players"] is not None:
-            instance.players = [
-                ModelsSessionPlayerHistory.create_from_dict(
-                    i0, include_empty=include_empty
-                )
-                for i0 in dict_["players"]
-            ]
-        elif include_empty:
-            instance.players = []
         if "region" in dict_ and dict_["region"] is not None:
             instance.region = str(dict_["region"])
         elif include_empty:
             instance.region = ""
         if "removed_reason" in dict_ and dict_["removed_reason"] is not None:
             instance.removed_reason = str(dict_["removed_reason"])
         elif include_empty:
@@ -443,18 +421,43 @@
             instance.status = str(dict_["status"])
         elif include_empty:
             instance.status = ""
         if "user_id" in dict_ and dict_["user_id"] is not None:
             instance.user_id = str(dict_["user_id"])
         elif include_empty:
             instance.user_id = ""
+        if "joining" in dict_ and dict_["joining"] is not None:
+            instance.joining = [
+                ModelsSessionPlayerJoining.create_from_dict(
+                    i0, include_empty=include_empty
+                )
+                for i0 in dict_["joining"]
+            ]
+        elif include_empty:
+            instance.joining = []
+        if "matching_allies" in dict_ and dict_["matching_allies"] is not None:
+            instance.matching_allies = [
+                ModelsMatchingAlly.create_from_dict(i0, include_empty=include_empty)
+                for i0 in dict_["matching_allies"]
+            ]
+        elif include_empty:
+            instance.matching_allies = []
         if "party_id" in dict_ and dict_["party_id"] is not None:
             instance.party_id = str(dict_["party_id"])
         elif include_empty:
             instance.party_id = ""
+        if "players" in dict_ and dict_["players"] is not None:
+            instance.players = [
+                ModelsSessionPlayerHistory.create_from_dict(
+                    i0, include_empty=include_empty
+                )
+                for i0 in dict_["players"]
+            ]
+        elif include_empty:
+            instance.players = []
         return instance
 
     @classmethod
     def create_many_from_dict(
         cls, dict_: dict, include_empty: bool = False
     ) -> Dict[str, ModelsGetSessionHistoryDetailedResponseItem]:
         return (
@@ -498,47 +501,47 @@
             "client_version": "client_version",
             "created_at": "created_at",
             "event_description": "event_description",
             "event_name": "event_name",
             "game_mode": "game_mode",
             "_id": "id_",
             "joinable": "joinable",
-            "joining": "joining",
             "match_id": "match_id",
-            "matching_allies": "matching_allies",
             "namespace": "namespace",
-            "players": "players",
             "region": "region",
             "removed_reason": "removed_reason",
             "server_name": "server_name",
             "session_type": "session_type",
             "status": "status",
             "user_id": "user_id",
+            "joining": "joining",
+            "matching_allies": "matching_allies",
             "party_id": "party_id",
+            "players": "players",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
             "channel": True,
             "client_version": True,
             "created_at": True,
             "event_description": True,
             "event_name": True,
             "game_mode": True,
             "_id": True,
             "joinable": True,
-            "joining": True,
             "match_id": True,
-            "matching_allies": True,
             "namespace": True,
-            "players": True,
             "region": True,
             "removed_reason": True,
             "server_name": True,
             "session_type": True,
             "status": True,
             "user_id": True,
+            "joining": False,
+            "matching_allies": False,
             "party_id": False,
+            "players": False,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/models/models_get_session_history_search_response_item_v2.py` & `accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/models/models_get_session_history_search_response_item_v2.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,48 +39,48 @@
 
         game_mode: (game_mode) REQUIRED str
 
         id_: (_id) REQUIRED str
 
         joinable: (joinable) REQUIRED bool
 
-        joining: (joining) REQUIRED List[ModelsSessionPlayerJoining]
-
         match_id: (match_id) REQUIRED str
 
         namespace: (namespace) REQUIRED str
 
-        players: (players) REQUIRED List[ModelsSessionPlayerHistory]
-
         removed_reason: (removed_reason) REQUIRED str
 
         session_type: (session_type) REQUIRED str
 
         status: (status) REQUIRED str
 
-        sub_game_mode: (sub_game_mode) REQUIRED List[str]
-
         user_id: (user_id) REQUIRED str
+
+        joining: (joining) OPTIONAL List[ModelsSessionPlayerJoining]
+
+        players: (players) OPTIONAL List[ModelsSessionPlayerHistory]
+
+        sub_game_mode: (sub_game_mode) OPTIONAL List[str]
     """
 
     # region fields
 
     created_at: str  # REQUIRED
     game_mode: str  # REQUIRED
     id_: str  # REQUIRED
     joinable: bool  # REQUIRED
-    joining: List[ModelsSessionPlayerJoining]  # REQUIRED
     match_id: str  # REQUIRED
     namespace: str  # REQUIRED
-    players: List[ModelsSessionPlayerHistory]  # REQUIRED
     removed_reason: str  # REQUIRED
     session_type: str  # REQUIRED
     status: str  # REQUIRED
-    sub_game_mode: List[str]  # REQUIRED
     user_id: str  # REQUIRED
+    joining: List[ModelsSessionPlayerJoining]  # OPTIONAL
+    players: List[ModelsSessionPlayerHistory]  # OPTIONAL
+    sub_game_mode: List[str]  # OPTIONAL
 
     # endregion fields
 
     # region with_x methods
 
     def with_created_at(
         self, value: str
@@ -96,34 +96,22 @@
         self.id_ = value
         return self
 
     def with_joinable(self, value: bool) -> ModelsGetSessionHistorySearchResponseItemV2:
         self.joinable = value
         return self
 
-    def with_joining(
-        self, value: List[ModelsSessionPlayerJoining]
-    ) -> ModelsGetSessionHistorySearchResponseItemV2:
-        self.joining = value
-        return self
-
     def with_match_id(self, value: str) -> ModelsGetSessionHistorySearchResponseItemV2:
         self.match_id = value
         return self
 
     def with_namespace(self, value: str) -> ModelsGetSessionHistorySearchResponseItemV2:
         self.namespace = value
         return self
 
-    def with_players(
-        self, value: List[ModelsSessionPlayerHistory]
-    ) -> ModelsGetSessionHistorySearchResponseItemV2:
-        self.players = value
-        return self
-
     def with_removed_reason(
         self, value: str
     ) -> ModelsGetSessionHistorySearchResponseItemV2:
         self.removed_reason = value
         return self
 
     def with_session_type(
@@ -132,24 +120,36 @@
         self.session_type = value
         return self
 
     def with_status(self, value: str) -> ModelsGetSessionHistorySearchResponseItemV2:
         self.status = value
         return self
 
+    def with_user_id(self, value: str) -> ModelsGetSessionHistorySearchResponseItemV2:
+        self.user_id = value
+        return self
+
+    def with_joining(
+        self, value: List[ModelsSessionPlayerJoining]
+    ) -> ModelsGetSessionHistorySearchResponseItemV2:
+        self.joining = value
+        return self
+
+    def with_players(
+        self, value: List[ModelsSessionPlayerHistory]
+    ) -> ModelsGetSessionHistorySearchResponseItemV2:
+        self.players = value
+        return self
+
     def with_sub_game_mode(
         self, value: List[str]
     ) -> ModelsGetSessionHistorySearchResponseItemV2:
         self.sub_game_mode = value
         return self
 
-    def with_user_id(self, value: str) -> ModelsGetSessionHistorySearchResponseItemV2:
-        self.user_id = value
-        return self
-
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
         if hasattr(self, "created_at"):
@@ -164,92 +164,95 @@
             result["_id"] = str(self.id_)
         elif include_empty:
             result["_id"] = ""
         if hasattr(self, "joinable"):
             result["joinable"] = bool(self.joinable)
         elif include_empty:
             result["joinable"] = False
-        if hasattr(self, "joining"):
-            result["joining"] = [
-                i0.to_dict(include_empty=include_empty) for i0 in self.joining
-            ]
-        elif include_empty:
-            result["joining"] = []
         if hasattr(self, "match_id"):
             result["match_id"] = str(self.match_id)
         elif include_empty:
             result["match_id"] = ""
         if hasattr(self, "namespace"):
             result["namespace"] = str(self.namespace)
         elif include_empty:
             result["namespace"] = ""
-        if hasattr(self, "players"):
-            result["players"] = [
-                i0.to_dict(include_empty=include_empty) for i0 in self.players
-            ]
-        elif include_empty:
-            result["players"] = []
         if hasattr(self, "removed_reason"):
             result["removed_reason"] = str(self.removed_reason)
         elif include_empty:
             result["removed_reason"] = ""
         if hasattr(self, "session_type"):
             result["session_type"] = str(self.session_type)
         elif include_empty:
             result["session_type"] = ""
         if hasattr(self, "status"):
             result["status"] = str(self.status)
         elif include_empty:
             result["status"] = ""
-        if hasattr(self, "sub_game_mode"):
-            result["sub_game_mode"] = [str(i0) for i0 in self.sub_game_mode]
-        elif include_empty:
-            result["sub_game_mode"] = []
         if hasattr(self, "user_id"):
             result["user_id"] = str(self.user_id)
         elif include_empty:
             result["user_id"] = ""
+        if hasattr(self, "joining"):
+            result["joining"] = [
+                i0.to_dict(include_empty=include_empty) for i0 in self.joining
+            ]
+        elif include_empty:
+            result["joining"] = []
+        if hasattr(self, "players"):
+            result["players"] = [
+                i0.to_dict(include_empty=include_empty) for i0 in self.players
+            ]
+        elif include_empty:
+            result["players"] = []
+        if hasattr(self, "sub_game_mode"):
+            result["sub_game_mode"] = [str(i0) for i0 in self.sub_game_mode]
+        elif include_empty:
+            result["sub_game_mode"] = []
         return result
 
     # endregion to methods
 
     # region static methods
 
     @classmethod
     def create(
         cls,
         created_at: str,
         game_mode: str,
         id_: str,
         joinable: bool,
-        joining: List[ModelsSessionPlayerJoining],
         match_id: str,
         namespace: str,
-        players: List[ModelsSessionPlayerHistory],
         removed_reason: str,
         session_type: str,
         status: str,
-        sub_game_mode: List[str],
         user_id: str,
+        joining: Optional[List[ModelsSessionPlayerJoining]] = None,
+        players: Optional[List[ModelsSessionPlayerHistory]] = None,
+        sub_game_mode: Optional[List[str]] = None,
         **kwargs,
     ) -> ModelsGetSessionHistorySearchResponseItemV2:
         instance = cls()
         instance.created_at = created_at
         instance.game_mode = game_mode
         instance.id_ = id_
         instance.joinable = joinable
-        instance.joining = joining
         instance.match_id = match_id
         instance.namespace = namespace
-        instance.players = players
         instance.removed_reason = removed_reason
         instance.session_type = session_type
         instance.status = status
-        instance.sub_game_mode = sub_game_mode
         instance.user_id = user_id
+        if joining is not None:
+            instance.joining = joining
+        if players is not None:
+            instance.players = players
+        if sub_game_mode is not None:
+            instance.sub_game_mode = sub_game_mode
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
     ) -> ModelsGetSessionHistorySearchResponseItemV2:
         instance = cls()
@@ -267,60 +270,60 @@
             instance.id_ = str(dict_["_id"])
         elif include_empty:
             instance.id_ = ""
         if "joinable" in dict_ and dict_["joinable"] is not None:
             instance.joinable = bool(dict_["joinable"])
         elif include_empty:
             instance.joinable = False
-        if "joining" in dict_ and dict_["joining"] is not None:
-            instance.joining = [
-                ModelsSessionPlayerJoining.create_from_dict(
-                    i0, include_empty=include_empty
-                )
-                for i0 in dict_["joining"]
-            ]
-        elif include_empty:
-            instance.joining = []
         if "match_id" in dict_ and dict_["match_id"] is not None:
             instance.match_id = str(dict_["match_id"])
         elif include_empty:
             instance.match_id = ""
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
         elif include_empty:
             instance.namespace = ""
-        if "players" in dict_ and dict_["players"] is not None:
-            instance.players = [
-                ModelsSessionPlayerHistory.create_from_dict(
-                    i0, include_empty=include_empty
-                )
-                for i0 in dict_["players"]
-            ]
-        elif include_empty:
-            instance.players = []
         if "removed_reason" in dict_ and dict_["removed_reason"] is not None:
             instance.removed_reason = str(dict_["removed_reason"])
         elif include_empty:
             instance.removed_reason = ""
         if "session_type" in dict_ and dict_["session_type"] is not None:
             instance.session_type = str(dict_["session_type"])
         elif include_empty:
             instance.session_type = ""
         if "status" in dict_ and dict_["status"] is not None:
             instance.status = str(dict_["status"])
         elif include_empty:
             instance.status = ""
-        if "sub_game_mode" in dict_ and dict_["sub_game_mode"] is not None:
-            instance.sub_game_mode = [str(i0) for i0 in dict_["sub_game_mode"]]
-        elif include_empty:
-            instance.sub_game_mode = []
         if "user_id" in dict_ and dict_["user_id"] is not None:
             instance.user_id = str(dict_["user_id"])
         elif include_empty:
             instance.user_id = ""
+        if "joining" in dict_ and dict_["joining"] is not None:
+            instance.joining = [
+                ModelsSessionPlayerJoining.create_from_dict(
+                    i0, include_empty=include_empty
+                )
+                for i0 in dict_["joining"]
+            ]
+        elif include_empty:
+            instance.joining = []
+        if "players" in dict_ and dict_["players"] is not None:
+            instance.players = [
+                ModelsSessionPlayerHistory.create_from_dict(
+                    i0, include_empty=include_empty
+                )
+                for i0 in dict_["players"]
+            ]
+        elif include_empty:
+            instance.players = []
+        if "sub_game_mode" in dict_ and dict_["sub_game_mode"] is not None:
+            instance.sub_game_mode = [str(i0) for i0 in dict_["sub_game_mode"]]
+        elif include_empty:
+            instance.sub_game_mode = []
         return instance
 
     @classmethod
     def create_many_from_dict(
         cls, dict_: dict, include_empty: bool = False
     ) -> Dict[str, ModelsGetSessionHistorySearchResponseItemV2]:
         return (
@@ -360,37 +363,37 @@
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
             "created_at": "created_at",
             "game_mode": "game_mode",
             "_id": "id_",
             "joinable": "joinable",
-            "joining": "joining",
             "match_id": "match_id",
             "namespace": "namespace",
-            "players": "players",
             "removed_reason": "removed_reason",
             "session_type": "session_type",
             "status": "status",
-            "sub_game_mode": "sub_game_mode",
             "user_id": "user_id",
+            "joining": "joining",
+            "players": "players",
+            "sub_game_mode": "sub_game_mode",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
             "created_at": True,
             "game_mode": True,
             "_id": True,
             "joinable": True,
-            "joining": True,
             "match_id": True,
             "namespace": True,
-            "players": True,
             "removed_reason": True,
             "session_type": True,
             "status": True,
-            "sub_game_mode": True,
             "user_id": True,
+            "joining": False,
+            "players": False,
+            "sub_game_mode": False,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/models/models_get_session_history_search_response_v2.py` & `accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/models/models_get_session_history_search_response_v2.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/models/models_join_game_session_request.py` & `accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/models/models_join_game_session_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/models/models_match_attributes.py` & `accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/models/models_match_attributes.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/models/models_match_making.py` & `accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/models/models_match_making.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,54 +44,54 @@
 
         event: (event) REQUIRED str
 
         game_mode: (game_mode) REQUIRED str
 
         match_id: (match_id) REQUIRED str
 
-        matching_allies: (matching_allies) REQUIRED List[ModelsMatchingAlly]
-
         namespace: (namespace) REQUIRED str
 
         party_attributes: (party_attributes) REQUIRED Dict[str, Any]
 
         queued_at: (queued_at) REQUIRED int
 
         region: (region) REQUIRED str
 
         server_name: (server_name) REQUIRED str
 
         status: (status) REQUIRED str
 
-        sub_game_mode: (sub_game_mode) REQUIRED List[str]
-
         joinable: (joinable) OPTIONAL bool
 
+        matching_allies: (matching_allies) OPTIONAL List[ModelsMatchingAlly]
+
         party_id: (party_id) OPTIONAL str
+
+        sub_game_mode: (sub_game_mode) OPTIONAL List[str]
     """
 
     # region fields
 
     channel: str  # REQUIRED
     client_version: str  # REQUIRED
     created_at: str  # REQUIRED
     deployment: str  # REQUIRED
     event: str  # REQUIRED
     game_mode: str  # REQUIRED
     match_id: str  # REQUIRED
-    matching_allies: List[ModelsMatchingAlly]  # REQUIRED
     namespace: str  # REQUIRED
     party_attributes: Dict[str, Any]  # REQUIRED
     queued_at: int  # REQUIRED
     region: str  # REQUIRED
     server_name: str  # REQUIRED
     status: str  # REQUIRED
-    sub_game_mode: List[str]  # REQUIRED
     joinable: bool  # OPTIONAL
+    matching_allies: List[ModelsMatchingAlly]  # OPTIONAL
     party_id: str  # OPTIONAL
+    sub_game_mode: List[str]  # OPTIONAL
 
     # endregion fields
 
     # region with_x methods
 
     def with_channel(self, value: str) -> ModelsMatchMaking:
         self.channel = value
@@ -117,20 +117,14 @@
         self.game_mode = value
         return self
 
     def with_match_id(self, value: str) -> ModelsMatchMaking:
         self.match_id = value
         return self
 
-    def with_matching_allies(
-        self, value: List[ModelsMatchingAlly]
-    ) -> ModelsMatchMaking:
-        self.matching_allies = value
-        return self
-
     def with_namespace(self, value: str) -> ModelsMatchMaking:
         self.namespace = value
         return self
 
     def with_party_attributes(self, value: Dict[str, Any]) -> ModelsMatchMaking:
         self.party_attributes = value
         return self
@@ -147,26 +141,32 @@
         self.server_name = value
         return self
 
     def with_status(self, value: str) -> ModelsMatchMaking:
         self.status = value
         return self
 
-    def with_sub_game_mode(self, value: List[str]) -> ModelsMatchMaking:
-        self.sub_game_mode = value
-        return self
-
     def with_joinable(self, value: bool) -> ModelsMatchMaking:
         self.joinable = value
         return self
 
+    def with_matching_allies(
+        self, value: List[ModelsMatchingAlly]
+    ) -> ModelsMatchMaking:
+        self.matching_allies = value
+        return self
+
     def with_party_id(self, value: str) -> ModelsMatchMaking:
         self.party_id = value
         return self
 
+    def with_sub_game_mode(self, value: List[str]) -> ModelsMatchMaking:
+        self.sub_game_mode = value
+        return self
+
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
         if hasattr(self, "channel"):
@@ -193,20 +193,14 @@
             result["game_mode"] = str(self.game_mode)
         elif include_empty:
             result["game_mode"] = ""
         if hasattr(self, "match_id"):
             result["match_id"] = str(self.match_id)
         elif include_empty:
             result["match_id"] = ""
-        if hasattr(self, "matching_allies"):
-            result["matching_allies"] = [
-                i0.to_dict(include_empty=include_empty) for i0 in self.matching_allies
-            ]
-        elif include_empty:
-            result["matching_allies"] = []
         if hasattr(self, "namespace"):
             result["namespace"] = str(self.namespace)
         elif include_empty:
             result["namespace"] = ""
         if hasattr(self, "party_attributes"):
             result["party_attributes"] = {
                 str(k0): v0 for k0, v0 in self.party_attributes.items()
@@ -225,26 +219,32 @@
             result["server_name"] = str(self.server_name)
         elif include_empty:
             result["server_name"] = ""
         if hasattr(self, "status"):
             result["status"] = str(self.status)
         elif include_empty:
             result["status"] = ""
-        if hasattr(self, "sub_game_mode"):
-            result["sub_game_mode"] = [str(i0) for i0 in self.sub_game_mode]
-        elif include_empty:
-            result["sub_game_mode"] = []
         if hasattr(self, "joinable"):
             result["joinable"] = bool(self.joinable)
         elif include_empty:
             result["joinable"] = False
+        if hasattr(self, "matching_allies"):
+            result["matching_allies"] = [
+                i0.to_dict(include_empty=include_empty) for i0 in self.matching_allies
+            ]
+        elif include_empty:
+            result["matching_allies"] = []
         if hasattr(self, "party_id"):
             result["party_id"] = str(self.party_id)
         elif include_empty:
             result["party_id"] = ""
+        if hasattr(self, "sub_game_mode"):
+            result["sub_game_mode"] = [str(i0) for i0 in self.sub_game_mode]
+        elif include_empty:
+            result["sub_game_mode"] = []
         return result
 
     # endregion to methods
 
     # region static methods
 
     @classmethod
@@ -253,46 +253,48 @@
         channel: str,
         client_version: str,
         created_at: str,
         deployment: str,
         event: str,
         game_mode: str,
         match_id: str,
-        matching_allies: List[ModelsMatchingAlly],
         namespace: str,
         party_attributes: Dict[str, Any],
         queued_at: int,
         region: str,
         server_name: str,
         status: str,
-        sub_game_mode: List[str],
         joinable: Optional[bool] = None,
+        matching_allies: Optional[List[ModelsMatchingAlly]] = None,
         party_id: Optional[str] = None,
+        sub_game_mode: Optional[List[str]] = None,
         **kwargs,
     ) -> ModelsMatchMaking:
         instance = cls()
         instance.channel = channel
         instance.client_version = client_version
         instance.created_at = created_at
         instance.deployment = deployment
         instance.event = event
         instance.game_mode = game_mode
         instance.match_id = match_id
-        instance.matching_allies = matching_allies
         instance.namespace = namespace
         instance.party_attributes = party_attributes
         instance.queued_at = queued_at
         instance.region = region
         instance.server_name = server_name
         instance.status = status
-        instance.sub_game_mode = sub_game_mode
         if joinable is not None:
             instance.joinable = joinable
+        if matching_allies is not None:
+            instance.matching_allies = matching_allies
         if party_id is not None:
             instance.party_id = party_id
+        if sub_game_mode is not None:
+            instance.sub_game_mode = sub_game_mode
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
     ) -> ModelsMatchMaking:
         instance = cls()
@@ -322,21 +324,14 @@
             instance.game_mode = str(dict_["game_mode"])
         elif include_empty:
             instance.game_mode = ""
         if "match_id" in dict_ and dict_["match_id"] is not None:
             instance.match_id = str(dict_["match_id"])
         elif include_empty:
             instance.match_id = ""
-        if "matching_allies" in dict_ and dict_["matching_allies"] is not None:
-            instance.matching_allies = [
-                ModelsMatchingAlly.create_from_dict(i0, include_empty=include_empty)
-                for i0 in dict_["matching_allies"]
-            ]
-        elif include_empty:
-            instance.matching_allies = []
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
         elif include_empty:
             instance.namespace = ""
         if "party_attributes" in dict_ and dict_["party_attributes"] is not None:
             instance.party_attributes = {
                 str(k0): v0 for k0, v0 in dict_["party_attributes"].items()
@@ -355,26 +350,33 @@
             instance.server_name = str(dict_["server_name"])
         elif include_empty:
             instance.server_name = ""
         if "status" in dict_ and dict_["status"] is not None:
             instance.status = str(dict_["status"])
         elif include_empty:
             instance.status = ""
-        if "sub_game_mode" in dict_ and dict_["sub_game_mode"] is not None:
-            instance.sub_game_mode = [str(i0) for i0 in dict_["sub_game_mode"]]
-        elif include_empty:
-            instance.sub_game_mode = []
         if "joinable" in dict_ and dict_["joinable"] is not None:
             instance.joinable = bool(dict_["joinable"])
         elif include_empty:
             instance.joinable = False
+        if "matching_allies" in dict_ and dict_["matching_allies"] is not None:
+            instance.matching_allies = [
+                ModelsMatchingAlly.create_from_dict(i0, include_empty=include_empty)
+                for i0 in dict_["matching_allies"]
+            ]
+        elif include_empty:
+            instance.matching_allies = []
         if "party_id" in dict_ and dict_["party_id"] is not None:
             instance.party_id = str(dict_["party_id"])
         elif include_empty:
             instance.party_id = ""
+        if "sub_game_mode" in dict_ and dict_["sub_game_mode"] is not None:
+            instance.sub_game_mode = [str(i0) for i0 in dict_["sub_game_mode"]]
+        elif include_empty:
+            instance.sub_game_mode = []
         return instance
 
     @classmethod
     def create_many_from_dict(
         cls, dict_: dict, include_empty: bool = False
     ) -> Dict[str, ModelsMatchMaking]:
         return (
@@ -415,42 +417,42 @@
             "channel": "channel",
             "client_version": "client_version",
             "created_at": "created_at",
             "deployment": "deployment",
             "event": "event",
             "game_mode": "game_mode",
             "match_id": "match_id",
-            "matching_allies": "matching_allies",
             "namespace": "namespace",
             "party_attributes": "party_attributes",
             "queued_at": "queued_at",
             "region": "region",
             "server_name": "server_name",
             "status": "status",
-            "sub_game_mode": "sub_game_mode",
             "joinable": "joinable",
+            "matching_allies": "matching_allies",
             "party_id": "party_id",
+            "sub_game_mode": "sub_game_mode",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
             "channel": True,
             "client_version": True,
             "created_at": True,
             "deployment": True,
             "event": True,
             "game_mode": True,
             "match_id": True,
-            "matching_allies": True,
             "namespace": True,
             "party_attributes": True,
             "queued_at": True,
             "region": True,
             "server_name": True,
             "status": True,
-            "sub_game_mode": True,
             "joinable": False,
+            "matching_allies": False,
             "party_id": False,
+            "sub_game_mode": False,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/models/models_matching_ally.py` & `accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/models/models_matching_ally.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,20 +30,20 @@
 from ..models.models_matching_party import ModelsMatchingParty
 
 
 class ModelsMatchingAlly(Model):
     """Models matching ally (models.MatchingAlly)
 
     Properties:
-        matching_parties: (matching_parties) REQUIRED List[ModelsMatchingParty]
+        matching_parties: (matching_parties) OPTIONAL List[ModelsMatchingParty]
     """
 
     # region fields
 
-    matching_parties: List[ModelsMatchingParty]  # REQUIRED
+    matching_parties: List[ModelsMatchingParty]  # OPTIONAL
 
     # endregion fields
 
     # region with_x methods
 
     def with_matching_parties(
         self, value: List[ModelsMatchingParty]
@@ -67,18 +67,19 @@
 
     # endregion to methods
 
     # region static methods
 
     @classmethod
     def create(
-        cls, matching_parties: List[ModelsMatchingParty], **kwargs
+        cls, matching_parties: Optional[List[ModelsMatchingParty]] = None, **kwargs
     ) -> ModelsMatchingAlly:
         instance = cls()
-        instance.matching_parties = matching_parties
+        if matching_parties is not None:
+            instance.matching_parties = matching_parties
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
     ) -> ModelsMatchingAlly:
         instance = cls()
@@ -134,11 +135,11 @@
         return {
             "matching_parties": "matching_parties",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
-            "matching_parties": True,
+            "matching_parties": False,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/models/models_matching_party.py` & `accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/models/models_matching_party.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,74 +31,74 @@
 from ..models.models_party_member import ModelsPartyMember
 
 
 class ModelsMatchingParty(Model):
     """Models matching party (models.MatchingParty)
 
     Properties:
-        match_attributes: (match_attributes) REQUIRED ModelsMatchAttributes
+        party_id: (party_id) REQUIRED str
 
-        party_attributes: (party_attributes) REQUIRED Dict[str, Any]
+        match_attributes: (match_attributes) OPTIONAL ModelsMatchAttributes
 
-        party_id: (party_id) REQUIRED str
+        party_attributes: (party_attributes) OPTIONAL Dict[str, Any]
 
-        party_members: (party_members) REQUIRED List[ModelsPartyMember]
+        party_members: (party_members) OPTIONAL List[ModelsPartyMember]
     """
 
     # region fields
 
-    match_attributes: ModelsMatchAttributes  # REQUIRED
-    party_attributes: Dict[str, Any]  # REQUIRED
     party_id: str  # REQUIRED
-    party_members: List[ModelsPartyMember]  # REQUIRED
+    match_attributes: ModelsMatchAttributes  # OPTIONAL
+    party_attributes: Dict[str, Any]  # OPTIONAL
+    party_members: List[ModelsPartyMember]  # OPTIONAL
 
     # endregion fields
 
     # region with_x methods
 
+    def with_party_id(self, value: str) -> ModelsMatchingParty:
+        self.party_id = value
+        return self
+
     def with_match_attributes(
         self, value: ModelsMatchAttributes
     ) -> ModelsMatchingParty:
         self.match_attributes = value
         return self
 
     def with_party_attributes(self, value: Dict[str, Any]) -> ModelsMatchingParty:
         self.party_attributes = value
         return self
 
-    def with_party_id(self, value: str) -> ModelsMatchingParty:
-        self.party_id = value
-        return self
-
     def with_party_members(self, value: List[ModelsPartyMember]) -> ModelsMatchingParty:
         self.party_members = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
+        if hasattr(self, "party_id"):
+            result["party_id"] = str(self.party_id)
+        elif include_empty:
+            result["party_id"] = ""
         if hasattr(self, "match_attributes"):
             result["match_attributes"] = self.match_attributes.to_dict(
                 include_empty=include_empty
             )
         elif include_empty:
             result["match_attributes"] = ModelsMatchAttributes()
         if hasattr(self, "party_attributes"):
             result["party_attributes"] = {
                 str(k0): v0 for k0, v0 in self.party_attributes.items()
             }
         elif include_empty:
             result["party_attributes"] = {}
-        if hasattr(self, "party_id"):
-            result["party_id"] = str(self.party_id)
-        elif include_empty:
-            result["party_id"] = ""
         if hasattr(self, "party_members"):
             result["party_members"] = [
                 i0.to_dict(include_empty=include_empty) for i0 in self.party_members
             ]
         elif include_empty:
             result["party_members"] = []
         return result
@@ -106,50 +106,53 @@
     # endregion to methods
 
     # region static methods
 
     @classmethod
     def create(
         cls,
-        match_attributes: ModelsMatchAttributes,
-        party_attributes: Dict[str, Any],
         party_id: str,
-        party_members: List[ModelsPartyMember],
+        match_attributes: Optional[ModelsMatchAttributes] = None,
+        party_attributes: Optional[Dict[str, Any]] = None,
+        party_members: Optional[List[ModelsPartyMember]] = None,
         **kwargs,
     ) -> ModelsMatchingParty:
         instance = cls()
-        instance.match_attributes = match_attributes
-        instance.party_attributes = party_attributes
         instance.party_id = party_id
-        instance.party_members = party_members
+        if match_attributes is not None:
+            instance.match_attributes = match_attributes
+        if party_attributes is not None:
+            instance.party_attributes = party_attributes
+        if party_members is not None:
+            instance.party_members = party_members
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
     ) -> ModelsMatchingParty:
         instance = cls()
         if not dict_:
             return instance
+        if "party_id" in dict_ and dict_["party_id"] is not None:
+            instance.party_id = str(dict_["party_id"])
+        elif include_empty:
+            instance.party_id = ""
         if "match_attributes" in dict_ and dict_["match_attributes"] is not None:
             instance.match_attributes = ModelsMatchAttributes.create_from_dict(
                 dict_["match_attributes"], include_empty=include_empty
             )
         elif include_empty:
             instance.match_attributes = ModelsMatchAttributes()
         if "party_attributes" in dict_ and dict_["party_attributes"] is not None:
             instance.party_attributes = {
                 str(k0): v0 for k0, v0 in dict_["party_attributes"].items()
             }
         elif include_empty:
             instance.party_attributes = {}
-        if "party_id" in dict_ and dict_["party_id"] is not None:
-            instance.party_id = str(dict_["party_id"])
-        elif include_empty:
-            instance.party_id = ""
         if "party_members" in dict_ and dict_["party_members"] is not None:
             instance.party_members = [
                 ModelsPartyMember.create_from_dict(i0, include_empty=include_empty)
                 for i0 in dict_["party_members"]
             ]
         elif include_empty:
             instance.party_members = []
@@ -190,23 +193,23 @@
                 raise ValueError()
         else:
             return cls.create_from_dict(any_, include_empty=include_empty)
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
+            "party_id": "party_id",
             "match_attributes": "match_attributes",
             "party_attributes": "party_attributes",
-            "party_id": "party_id",
             "party_members": "party_members",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
-            "match_attributes": True,
-            "party_attributes": True,
             "party_id": True,
-            "party_members": True,
+            "match_attributes": False,
+            "party_attributes": False,
+            "party_members": False,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/models/models_pagination.py` & `accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/models/models_pagination.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/models/models_paging_cursor.py` & `accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/models/models_paging_cursor.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/models/models_party_member.py` & `accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/models/models_party_member.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,84 +28,85 @@
 from accelbyte_py_sdk.core import Model
 
 
 class ModelsPartyMember(Model):
     """Models party member (models.PartyMember)
 
     Properties:
-        extra_attributes: (extra_attributes) REQUIRED Dict[str, Any]
-
         user_id: (user_id) REQUIRED str
+
+        extra_attributes: (extra_attributes) OPTIONAL Dict[str, Any]
     """
 
     # region fields
 
-    extra_attributes: Dict[str, Any]  # REQUIRED
     user_id: str  # REQUIRED
+    extra_attributes: Dict[str, Any]  # OPTIONAL
 
     # endregion fields
 
     # region with_x methods
 
-    def with_extra_attributes(self, value: Dict[str, Any]) -> ModelsPartyMember:
-        self.extra_attributes = value
-        return self
-
     def with_user_id(self, value: str) -> ModelsPartyMember:
         self.user_id = value
         return self
 
+    def with_extra_attributes(self, value: Dict[str, Any]) -> ModelsPartyMember:
+        self.extra_attributes = value
+        return self
+
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
+        if hasattr(self, "user_id"):
+            result["user_id"] = str(self.user_id)
+        elif include_empty:
+            result["user_id"] = ""
         if hasattr(self, "extra_attributes"):
             result["extra_attributes"] = {
                 str(k0): v0 for k0, v0 in self.extra_attributes.items()
             }
         elif include_empty:
             result["extra_attributes"] = {}
-        if hasattr(self, "user_id"):
-            result["user_id"] = str(self.user_id)
-        elif include_empty:
-            result["user_id"] = ""
         return result
 
     # endregion to methods
 
     # region static methods
 
     @classmethod
     def create(
-        cls, extra_attributes: Dict[str, Any], user_id: str, **kwargs
+        cls, user_id: str, extra_attributes: Optional[Dict[str, Any]] = None, **kwargs
     ) -> ModelsPartyMember:
         instance = cls()
-        instance.extra_attributes = extra_attributes
         instance.user_id = user_id
+        if extra_attributes is not None:
+            instance.extra_attributes = extra_attributes
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
     ) -> ModelsPartyMember:
         instance = cls()
         if not dict_:
             return instance
+        if "user_id" in dict_ and dict_["user_id"] is not None:
+            instance.user_id = str(dict_["user_id"])
+        elif include_empty:
+            instance.user_id = ""
         if "extra_attributes" in dict_ and dict_["extra_attributes"] is not None:
             instance.extra_attributes = {
                 str(k0): v0 for k0, v0 in dict_["extra_attributes"].items()
             }
         elif include_empty:
             instance.extra_attributes = {}
-        if "user_id" in dict_ and dict_["user_id"] is not None:
-            instance.user_id = str(dict_["user_id"])
-        elif include_empty:
-            instance.user_id = ""
         return instance
 
     @classmethod
     def create_many_from_dict(
         cls, dict_: dict, include_empty: bool = False
     ) -> Dict[str, ModelsPartyMember]:
         return (
@@ -139,19 +140,19 @@
                 raise ValueError()
         else:
             return cls.create_from_dict(any_, include_empty=include_empty)
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
-            "extra_attributes": "extra_attributes",
             "user_id": "user_id",
+            "extra_attributes": "extra_attributes",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
-            "extra_attributes": True,
             "user_id": True,
+            "extra_attributes": False,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/models/models_recent_player_history.py` & `accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/models/models_recent_player_history.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/models/models_recent_player_query_response.py` & `accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/models/models_recent_player_query_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/models/models_server.py` & `accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/models/models_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,16 +32,14 @@
 
 class ModelsServer(Model):
     """Models server (models.Server)
 
     Properties:
         allocation_id: (allocation_id) REQUIRED str
 
-        alternate_ips: (alternate_ips) REQUIRED List[str]
-
         cpu_limit: (cpu_limit) REQUIRED int
 
         cpu_request: (cpu_request) REQUIRED str
 
         deployment: (deployment) REQUIRED str
 
         game_version: (game_version) REQUIRED str
@@ -62,64 +60,62 @@
 
         params: (params) REQUIRED str
 
         pod_name: (pod_name) REQUIRED str
 
         port: (port) REQUIRED int
 
-        ports: (ports) REQUIRED Dict[str, int]
-
         provider: (provider) REQUIRED str
 
         region: (region) REQUIRED str
 
         session_id: (session_id) REQUIRED str
 
         status: (status) REQUIRED str
 
-        status_history: (status_history) REQUIRED List[ModelsStatusHistory]
+        alternate_ips: (alternate_ips) OPTIONAL List[str]
+
+        ports: (ports) OPTIONAL Dict[str, int]
+
+        status_history: (status_history) OPTIONAL List[ModelsStatusHistory]
     """
 
     # region fields
 
     allocation_id: str  # REQUIRED
-    alternate_ips: List[str]  # REQUIRED
     cpu_limit: int  # REQUIRED
     cpu_request: str  # REQUIRED
     deployment: str  # REQUIRED
     game_version: str  # REQUIRED
     image_version: str  # REQUIRED
     ip: str  # REQUIRED
     is_override_game_version: bool  # REQUIRED
     last_update: str  # REQUIRED
     mem_limit: int  # REQUIRED
     mem_request: str  # REQUIRED
     namespace: str  # REQUIRED
     params: str  # REQUIRED
     pod_name: str  # REQUIRED
     port: int  # REQUIRED
-    ports: Dict[str, int]  # REQUIRED
     provider: str  # REQUIRED
     region: str  # REQUIRED
     session_id: str  # REQUIRED
     status: str  # REQUIRED
-    status_history: List[ModelsStatusHistory]  # REQUIRED
+    alternate_ips: List[str]  # OPTIONAL
+    ports: Dict[str, int]  # OPTIONAL
+    status_history: List[ModelsStatusHistory]  # OPTIONAL
 
     # endregion fields
 
     # region with_x methods
 
     def with_allocation_id(self, value: str) -> ModelsServer:
         self.allocation_id = value
         return self
 
-    def with_alternate_ips(self, value: List[str]) -> ModelsServer:
-        self.alternate_ips = value
-        return self
-
     def with_cpu_limit(self, value: int) -> ModelsServer:
         self.cpu_limit = value
         return self
 
     def with_cpu_request(self, value: str) -> ModelsServer:
         self.cpu_request = value
         return self
@@ -168,18 +164,14 @@
         self.pod_name = value
         return self
 
     def with_port(self, value: int) -> ModelsServer:
         self.port = value
         return self
 
-    def with_ports(self, value: Dict[str, int]) -> ModelsServer:
-        self.ports = value
-        return self
-
     def with_provider(self, value: str) -> ModelsServer:
         self.provider = value
         return self
 
     def with_region(self, value: str) -> ModelsServer:
         self.region = value
         return self
@@ -188,32 +180,36 @@
         self.session_id = value
         return self
 
     def with_status(self, value: str) -> ModelsServer:
         self.status = value
         return self
 
+    def with_alternate_ips(self, value: List[str]) -> ModelsServer:
+        self.alternate_ips = value
+        return self
+
+    def with_ports(self, value: Dict[str, int]) -> ModelsServer:
+        self.ports = value
+        return self
+
     def with_status_history(self, value: List[ModelsStatusHistory]) -> ModelsServer:
         self.status_history = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
         if hasattr(self, "allocation_id"):
             result["allocation_id"] = str(self.allocation_id)
         elif include_empty:
             result["allocation_id"] = ""
-        if hasattr(self, "alternate_ips"):
-            result["alternate_ips"] = [str(i0) for i0 in self.alternate_ips]
-        elif include_empty:
-            result["alternate_ips"] = []
         if hasattr(self, "cpu_limit"):
             result["cpu_limit"] = int(self.cpu_limit)
         elif include_empty:
             result["cpu_limit"] = 0
         if hasattr(self, "cpu_request"):
             result["cpu_request"] = str(self.cpu_request)
         elif include_empty:
@@ -262,18 +258,14 @@
             result["pod_name"] = str(self.pod_name)
         elif include_empty:
             result["pod_name"] = ""
         if hasattr(self, "port"):
             result["port"] = int(self.port)
         elif include_empty:
             result["port"] = 0
-        if hasattr(self, "ports"):
-            result["ports"] = {str(k0): int(v0) for k0, v0 in self.ports.items()}
-        elif include_empty:
-            result["ports"] = {}
         if hasattr(self, "provider"):
             result["provider"] = str(self.provider)
         elif include_empty:
             result["provider"] = ""
         if hasattr(self, "region"):
             result["region"] = str(self.region)
         elif include_empty:
@@ -282,14 +274,22 @@
             result["session_id"] = str(self.session_id)
         elif include_empty:
             result["session_id"] = ""
         if hasattr(self, "status"):
             result["status"] = str(self.status)
         elif include_empty:
             result["status"] = ""
+        if hasattr(self, "alternate_ips"):
+            result["alternate_ips"] = [str(i0) for i0 in self.alternate_ips]
+        elif include_empty:
+            result["alternate_ips"] = []
+        if hasattr(self, "ports"):
+            result["ports"] = {str(k0): int(v0) for k0, v0 in self.ports.items()}
+        elif include_empty:
+            result["ports"] = {}
         if hasattr(self, "status_history"):
             result["status_history"] = [
                 i0.to_dict(include_empty=include_empty) for i0 in self.status_history
             ]
         elif include_empty:
             result["status_history"] = []
         return result
@@ -298,75 +298,74 @@
 
     # region static methods
 
     @classmethod
     def create(
         cls,
         allocation_id: str,
-        alternate_ips: List[str],
         cpu_limit: int,
         cpu_request: str,
         deployment: str,
         game_version: str,
         image_version: str,
         ip: str,
         is_override_game_version: bool,
         last_update: str,
         mem_limit: int,
         mem_request: str,
         namespace: str,
         params: str,
         pod_name: str,
         port: int,
-        ports: Dict[str, int],
         provider: str,
         region: str,
         session_id: str,
         status: str,
-        status_history: List[ModelsStatusHistory],
+        alternate_ips: Optional[List[str]] = None,
+        ports: Optional[Dict[str, int]] = None,
+        status_history: Optional[List[ModelsStatusHistory]] = None,
         **kwargs,
     ) -> ModelsServer:
         instance = cls()
         instance.allocation_id = allocation_id
-        instance.alternate_ips = alternate_ips
         instance.cpu_limit = cpu_limit
         instance.cpu_request = cpu_request
         instance.deployment = deployment
         instance.game_version = game_version
         instance.image_version = image_version
         instance.ip = ip
         instance.is_override_game_version = is_override_game_version
         instance.last_update = last_update
         instance.mem_limit = mem_limit
         instance.mem_request = mem_request
         instance.namespace = namespace
         instance.params = params
         instance.pod_name = pod_name
         instance.port = port
-        instance.ports = ports
         instance.provider = provider
         instance.region = region
         instance.session_id = session_id
         instance.status = status
-        instance.status_history = status_history
+        if alternate_ips is not None:
+            instance.alternate_ips = alternate_ips
+        if ports is not None:
+            instance.ports = ports
+        if status_history is not None:
+            instance.status_history = status_history
         return instance
 
     @classmethod
     def create_from_dict(cls, dict_: dict, include_empty: bool = False) -> ModelsServer:
         instance = cls()
         if not dict_:
             return instance
         if "allocation_id" in dict_ and dict_["allocation_id"] is not None:
             instance.allocation_id = str(dict_["allocation_id"])
         elif include_empty:
             instance.allocation_id = ""
-        if "alternate_ips" in dict_ and dict_["alternate_ips"] is not None:
-            instance.alternate_ips = [str(i0) for i0 in dict_["alternate_ips"]]
-        elif include_empty:
-            instance.alternate_ips = []
         if "cpu_limit" in dict_ and dict_["cpu_limit"] is not None:
             instance.cpu_limit = int(dict_["cpu_limit"])
         elif include_empty:
             instance.cpu_limit = 0
         if "cpu_request" in dict_ and dict_["cpu_request"] is not None:
             instance.cpu_request = str(dict_["cpu_request"])
         elif include_empty:
@@ -418,18 +417,14 @@
             instance.pod_name = str(dict_["pod_name"])
         elif include_empty:
             instance.pod_name = ""
         if "port" in dict_ and dict_["port"] is not None:
             instance.port = int(dict_["port"])
         elif include_empty:
             instance.port = 0
-        if "ports" in dict_ and dict_["ports"] is not None:
-            instance.ports = {str(k0): int(v0) for k0, v0 in dict_["ports"].items()}
-        elif include_empty:
-            instance.ports = {}
         if "provider" in dict_ and dict_["provider"] is not None:
             instance.provider = str(dict_["provider"])
         elif include_empty:
             instance.provider = ""
         if "region" in dict_ and dict_["region"] is not None:
             instance.region = str(dict_["region"])
         elif include_empty:
@@ -438,14 +433,22 @@
             instance.session_id = str(dict_["session_id"])
         elif include_empty:
             instance.session_id = ""
         if "status" in dict_ and dict_["status"] is not None:
             instance.status = str(dict_["status"])
         elif include_empty:
             instance.status = ""
+        if "alternate_ips" in dict_ and dict_["alternate_ips"] is not None:
+            instance.alternate_ips = [str(i0) for i0 in dict_["alternate_ips"]]
+        elif include_empty:
+            instance.alternate_ips = []
+        if "ports" in dict_ and dict_["ports"] is not None:
+            instance.ports = {str(k0): int(v0) for k0, v0 in dict_["ports"].items()}
+        elif include_empty:
+            instance.ports = {}
         if "status_history" in dict_ and dict_["status_history"] is not None:
             instance.status_history = [
                 ModelsStatusHistory.create_from_dict(i0, include_empty=include_empty)
                 for i0 in dict_["status_history"]
             ]
         elif include_empty:
             instance.status_history = []
@@ -485,58 +488,58 @@
         else:
             return cls.create_from_dict(any_, include_empty=include_empty)
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
             "allocation_id": "allocation_id",
-            "alternate_ips": "alternate_ips",
             "cpu_limit": "cpu_limit",
             "cpu_request": "cpu_request",
             "deployment": "deployment",
             "game_version": "game_version",
             "image_version": "image_version",
             "ip": "ip",
             "is_override_game_version": "is_override_game_version",
             "last_update": "last_update",
             "mem_limit": "mem_limit",
             "mem_request": "mem_request",
             "namespace": "namespace",
             "params": "params",
             "pod_name": "pod_name",
             "port": "port",
-            "ports": "ports",
             "provider": "provider",
             "region": "region",
             "session_id": "session_id",
             "status": "status",
+            "alternate_ips": "alternate_ips",
+            "ports": "ports",
             "status_history": "status_history",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
             "allocation_id": True,
-            "alternate_ips": True,
             "cpu_limit": True,
             "cpu_request": True,
             "deployment": True,
             "game_version": True,
             "image_version": True,
             "ip": True,
             "is_override_game_version": True,
             "last_update": True,
             "mem_limit": True,
             "mem_request": True,
             "namespace": True,
             "params": True,
             "pod_name": True,
             "port": True,
-            "ports": True,
             "provider": True,
             "region": True,
             "session_id": True,
             "status": True,
-            "status_history": True,
+            "alternate_ips": False,
+            "ports": False,
+            "status_history": False,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/models/models_session_by_user_i_ds_response.py` & `accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/models/models_session_by_user_i_ds_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/models/models_session_player_history.py` & `accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/models/models_session_player_history.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/models/models_session_player_joining.py` & `accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/models/models_session_player_joining.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/models/models_session_query_response.py` & `accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/models/models_session_query_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/models/models_session_response.py` & `accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/models/models_admin_session_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,30 +28,26 @@
 from accelbyte_py_sdk.core import Model
 
 from ..models.models_game_session_setting import ModelsGameSessionSetting
 from ..models.models_match_making import ModelsMatchMaking
 from ..models.models_server import ModelsServer
 
 
-class ModelsSessionResponse(Model):
-    """Models session response (models.SessionResponse)
+class ModelsAdminSessionResponse(Model):
+    """Models admin session response (models.AdminSessionResponse)
 
     Properties:
         all_players: (all_players) REQUIRED List[str]
 
         created_at: (created_at) REQUIRED str
 
-        game_session_setting: (game_session_setting) REQUIRED ModelsGameSessionSetting
-
         game_version: (game_version) REQUIRED str
 
         joinable: (joinable) REQUIRED bool
 
-        match: (match) REQUIRED ModelsMatchMaking
-
         namespace: (namespace) REQUIRED str
 
         players: (players) REQUIRED List[str]
 
         server: (server) REQUIRED ModelsServer
 
         session_id: (session_id) REQUIRED str
@@ -59,127 +55,121 @@
         session_type: (session_type) REQUIRED str
 
         spectators: (spectators) REQUIRED List[str]
 
         user_id: (user_id) REQUIRED str
 
         username: (username) REQUIRED str
+
+        game_session_setting: (game_session_setting) OPTIONAL ModelsGameSessionSetting
+
+        match: (match) OPTIONAL ModelsMatchMaking
     """
 
     # region fields
 
     all_players: List[str]  # REQUIRED
     created_at: str  # REQUIRED
-    game_session_setting: ModelsGameSessionSetting  # REQUIRED
     game_version: str  # REQUIRED
     joinable: bool  # REQUIRED
-    match: ModelsMatchMaking  # REQUIRED
     namespace: str  # REQUIRED
     players: List[str]  # REQUIRED
     server: ModelsServer  # REQUIRED
     session_id: str  # REQUIRED
     session_type: str  # REQUIRED
     spectators: List[str]  # REQUIRED
     user_id: str  # REQUIRED
     username: str  # REQUIRED
+    game_session_setting: ModelsGameSessionSetting  # OPTIONAL
+    match: ModelsMatchMaking  # OPTIONAL
 
     # endregion fields
 
     # region with_x methods
 
-    def with_all_players(self, value: List[str]) -> ModelsSessionResponse:
+    def with_all_players(self, value: List[str]) -> ModelsAdminSessionResponse:
         self.all_players = value
         return self
 
-    def with_created_at(self, value: str) -> ModelsSessionResponse:
+    def with_created_at(self, value: str) -> ModelsAdminSessionResponse:
         self.created_at = value
         return self
 
-    def with_game_session_setting(
-        self, value: ModelsGameSessionSetting
-    ) -> ModelsSessionResponse:
-        self.game_session_setting = value
-        return self
-
-    def with_game_version(self, value: str) -> ModelsSessionResponse:
+    def with_game_version(self, value: str) -> ModelsAdminSessionResponse:
         self.game_version = value
         return self
 
-    def with_joinable(self, value: bool) -> ModelsSessionResponse:
+    def with_joinable(self, value: bool) -> ModelsAdminSessionResponse:
         self.joinable = value
         return self
 
-    def with_match(self, value: ModelsMatchMaking) -> ModelsSessionResponse:
-        self.match = value
-        return self
-
-    def with_namespace(self, value: str) -> ModelsSessionResponse:
+    def with_namespace(self, value: str) -> ModelsAdminSessionResponse:
         self.namespace = value
         return self
 
-    def with_players(self, value: List[str]) -> ModelsSessionResponse:
+    def with_players(self, value: List[str]) -> ModelsAdminSessionResponse:
         self.players = value
         return self
 
-    def with_server(self, value: ModelsServer) -> ModelsSessionResponse:
+    def with_server(self, value: ModelsServer) -> ModelsAdminSessionResponse:
         self.server = value
         return self
 
-    def with_session_id(self, value: str) -> ModelsSessionResponse:
+    def with_session_id(self, value: str) -> ModelsAdminSessionResponse:
         self.session_id = value
         return self
 
-    def with_session_type(self, value: str) -> ModelsSessionResponse:
+    def with_session_type(self, value: str) -> ModelsAdminSessionResponse:
         self.session_type = value
         return self
 
-    def with_spectators(self, value: List[str]) -> ModelsSessionResponse:
+    def with_spectators(self, value: List[str]) -> ModelsAdminSessionResponse:
         self.spectators = value
         return self
 
-    def with_user_id(self, value: str) -> ModelsSessionResponse:
+    def with_user_id(self, value: str) -> ModelsAdminSessionResponse:
         self.user_id = value
         return self
 
-    def with_username(self, value: str) -> ModelsSessionResponse:
+    def with_username(self, value: str) -> ModelsAdminSessionResponse:
         self.username = value
         return self
 
+    def with_game_session_setting(
+        self, value: ModelsGameSessionSetting
+    ) -> ModelsAdminSessionResponse:
+        self.game_session_setting = value
+        return self
+
+    def with_match(self, value: ModelsMatchMaking) -> ModelsAdminSessionResponse:
+        self.match = value
+        return self
+
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
         if hasattr(self, "all_players"):
             result["all_players"] = [str(i0) for i0 in self.all_players]
         elif include_empty:
             result["all_players"] = []
         if hasattr(self, "created_at"):
             result["created_at"] = str(self.created_at)
         elif include_empty:
             result["created_at"] = ""
-        if hasattr(self, "game_session_setting"):
-            result["game_session_setting"] = self.game_session_setting.to_dict(
-                include_empty=include_empty
-            )
-        elif include_empty:
-            result["game_session_setting"] = ModelsGameSessionSetting()
         if hasattr(self, "game_version"):
             result["game_version"] = str(self.game_version)
         elif include_empty:
             result["game_version"] = ""
         if hasattr(self, "joinable"):
             result["joinable"] = bool(self.joinable)
         elif include_empty:
             result["joinable"] = False
-        if hasattr(self, "match"):
-            result["match"] = self.match.to_dict(include_empty=include_empty)
-        elif include_empty:
-            result["match"] = ModelsMatchMaking()
         if hasattr(self, "namespace"):
             result["namespace"] = str(self.namespace)
         elif include_empty:
             result["namespace"] = ""
         if hasattr(self, "players"):
             result["players"] = [str(i0) for i0 in self.players]
         elif include_empty:
@@ -204,94 +194,91 @@
             result["user_id"] = str(self.user_id)
         elif include_empty:
             result["user_id"] = ""
         if hasattr(self, "username"):
             result["username"] = str(self.username)
         elif include_empty:
             result["username"] = ""
+        if hasattr(self, "game_session_setting"):
+            result["game_session_setting"] = self.game_session_setting.to_dict(
+                include_empty=include_empty
+            )
+        elif include_empty:
+            result["game_session_setting"] = ModelsGameSessionSetting()
+        if hasattr(self, "match"):
+            result["match"] = self.match.to_dict(include_empty=include_empty)
+        elif include_empty:
+            result["match"] = ModelsMatchMaking()
         return result
 
     # endregion to methods
 
     # region static methods
 
     @classmethod
     def create(
         cls,
         all_players: List[str],
         created_at: str,
-        game_session_setting: ModelsGameSessionSetting,
         game_version: str,
         joinable: bool,
-        match: ModelsMatchMaking,
         namespace: str,
         players: List[str],
         server: ModelsServer,
         session_id: str,
         session_type: str,
         spectators: List[str],
         user_id: str,
         username: str,
+        game_session_setting: Optional[ModelsGameSessionSetting] = None,
+        match: Optional[ModelsMatchMaking] = None,
         **kwargs,
-    ) -> ModelsSessionResponse:
+    ) -> ModelsAdminSessionResponse:
         instance = cls()
         instance.all_players = all_players
         instance.created_at = created_at
-        instance.game_session_setting = game_session_setting
         instance.game_version = game_version
         instance.joinable = joinable
-        instance.match = match
         instance.namespace = namespace
         instance.players = players
         instance.server = server
         instance.session_id = session_id
         instance.session_type = session_type
         instance.spectators = spectators
         instance.user_id = user_id
         instance.username = username
+        if game_session_setting is not None:
+            instance.game_session_setting = game_session_setting
+        if match is not None:
+            instance.match = match
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> ModelsSessionResponse:
+    ) -> ModelsAdminSessionResponse:
         instance = cls()
         if not dict_:
             return instance
         if "all_players" in dict_ and dict_["all_players"] is not None:
             instance.all_players = [str(i0) for i0 in dict_["all_players"]]
         elif include_empty:
             instance.all_players = []
         if "created_at" in dict_ and dict_["created_at"] is not None:
             instance.created_at = str(dict_["created_at"])
         elif include_empty:
             instance.created_at = ""
-        if (
-            "game_session_setting" in dict_
-            and dict_["game_session_setting"] is not None
-        ):
-            instance.game_session_setting = ModelsGameSessionSetting.create_from_dict(
-                dict_["game_session_setting"], include_empty=include_empty
-            )
-        elif include_empty:
-            instance.game_session_setting = ModelsGameSessionSetting()
         if "game_version" in dict_ and dict_["game_version"] is not None:
             instance.game_version = str(dict_["game_version"])
         elif include_empty:
             instance.game_version = ""
         if "joinable" in dict_ and dict_["joinable"] is not None:
             instance.joinable = bool(dict_["joinable"])
         elif include_empty:
             instance.joinable = False
-        if "match" in dict_ and dict_["match"] is not None:
-            instance.match = ModelsMatchMaking.create_from_dict(
-                dict_["match"], include_empty=include_empty
-            )
-        elif include_empty:
-            instance.match = ModelsMatchMaking()
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
         elif include_empty:
             instance.namespace = ""
         if "players" in dict_ and dict_["players"] is not None:
             instance.players = [str(i0) for i0 in dict_["players"]]
         elif include_empty:
@@ -318,43 +305,58 @@
             instance.user_id = str(dict_["user_id"])
         elif include_empty:
             instance.user_id = ""
         if "username" in dict_ and dict_["username"] is not None:
             instance.username = str(dict_["username"])
         elif include_empty:
             instance.username = ""
+        if (
+            "game_session_setting" in dict_
+            and dict_["game_session_setting"] is not None
+        ):
+            instance.game_session_setting = ModelsGameSessionSetting.create_from_dict(
+                dict_["game_session_setting"], include_empty=include_empty
+            )
+        elif include_empty:
+            instance.game_session_setting = ModelsGameSessionSetting()
+        if "match" in dict_ and dict_["match"] is not None:
+            instance.match = ModelsMatchMaking.create_from_dict(
+                dict_["match"], include_empty=include_empty
+            )
+        elif include_empty:
+            instance.match = ModelsMatchMaking()
         return instance
 
     @classmethod
     def create_many_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> Dict[str, ModelsSessionResponse]:
+    ) -> Dict[str, ModelsAdminSessionResponse]:
         return (
             {k: cls.create_from_dict(v, include_empty=include_empty) for k, v in dict_}
             if dict_
             else {}
         )
 
     @classmethod
     def create_many_from_list(
         cls, list_: list, include_empty: bool = False
-    ) -> List[ModelsSessionResponse]:
+    ) -> List[ModelsAdminSessionResponse]:
         return (
             [cls.create_from_dict(i, include_empty=include_empty) for i in list_]
             if list_
             else []
         )
 
     @classmethod
     def create_from_any(
         cls, any_: any, include_empty: bool = False, many: bool = False
     ) -> Union[
-        ModelsSessionResponse,
-        List[ModelsSessionResponse],
-        Dict[Any, ModelsSessionResponse],
+        ModelsAdminSessionResponse,
+        List[ModelsAdminSessionResponse],
+        Dict[Any, ModelsAdminSessionResponse],
     ]:
         if many:
             if isinstance(any_, dict):
                 return cls.create_many_from_dict(any_, include_empty=include_empty)
             elif isinstance(any_, list):
                 return cls.create_many_from_list(any_, include_empty=include_empty)
             else:
@@ -363,41 +365,41 @@
             return cls.create_from_dict(any_, include_empty=include_empty)
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
             "all_players": "all_players",
             "created_at": "created_at",
-            "game_session_setting": "game_session_setting",
             "game_version": "game_version",
             "joinable": "joinable",
-            "match": "match",
             "namespace": "namespace",
             "players": "players",
             "server": "server",
             "session_id": "session_id",
             "session_type": "session_type",
             "spectators": "spectators",
             "user_id": "user_id",
             "username": "username",
+            "game_session_setting": "game_session_setting",
+            "match": "match",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
             "all_players": True,
             "created_at": True,
-            "game_session_setting": True,
             "game_version": True,
             "joinable": True,
-            "match": True,
             "namespace": True,
             "players": True,
             "server": True,
             "session_id": True,
             "session_type": True,
             "spectators": True,
             "user_id": True,
             "username": True,
+            "game_session_setting": False,
+            "match": False,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/models/models_status_history.py` & `accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/models/models_status_history.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/models/models_update_session_request.py` & `accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/models/models_update_session_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/models/models_update_settings_request.py` & `accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/models/models_update_settings_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/models/response_error.py` & `accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/models/response_error.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/models/restapi_error_response_v2.py` & `accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/models/restapi_error_response_v2.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/models/restapi_error_v1.py` & `accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/models/restapi_error_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/__init__.py` & `accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/__init__.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/add_player_to_session.py` & `accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/add_player_to_session.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/admin_delete_session.py` & `accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/admin_delete_session.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/admin_get_session.py` & `accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/admin_get_session.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/admin_query_session.py` & `accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/admin_query_session.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/admin_search_sessions_v2.py` & `accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/admin_search_sessions_v2.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/create_session.py` & `accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/create_session.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/delete_session.py` & `accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/delete_session.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/delete_session_local_ds.py` & `accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/delete_session_local_ds.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/get_active_custom_game__cd6755.py` & `accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/get_active_custom_game__cd6755.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/get_active_matchmaking__0b8050.py` & `accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/get_active_matchmaking__0b8050.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/get_recent_player.py` & `accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/get_recent_player.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/get_session.py` & `accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/get_session.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/get_session_by_user_i_ds.py` & `accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/get_session_by_user_i_ds.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/get_session_history_detailed.py` & `accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/get_session_history_detailed.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/get_total_active_session.py` & `accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/get_total_active_session.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/join_session.py` & `accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/join_session.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/remove_player_from_session.py` & `accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/remove_player_from_session.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/update_session.py` & `accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/update_session.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/update_settings.py` & `accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/update_settings.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/user_query_session.py` & `accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/operations/session/user_query_session.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/wrappers/__init__.py` & `accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/wrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk/api/sessionbrowser/wrappers/_session.py` & `accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk/api/sessionbrowser/wrappers/_session.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk_service_sessionbrowser.egg-info/PKG-INFO` & `accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk_service_sessionbrowser.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: accelbyte-py-sdk-service-sessionbrowser
-Version: 0.8.0
+Version: 0.9.0
 Summary: AccelByte Python SDK - AccelByte Gaming Services Session Browser Service
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: accelbyte-py-sdk-core
 
 [//]: # (Code generated. DO NOT EDIT!)
```

### Comparing `accelbyte-py-sdk-service-sessionbrowser-0.8.0/accelbyte_py_sdk_service_sessionbrowser.egg-info/SOURCES.txt` & `accelbyte-py-sdk-service-sessionbrowser-0.9.0/accelbyte_py_sdk_service_sessionbrowser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

