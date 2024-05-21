# Comparing `tmp/accelbyte-py-sdk-service-session-0.8.0.tar.gz` & `tmp/accelbyte-py-sdk-service-session-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accelbyte-py-sdk-service-session-0.8.0.tar", last modified: Tue Feb 27 05:42:02 2024, max compression
+gzip compressed data, was "accelbyte-py-sdk-service-session-0.9.0.tar", last modified: Wed Mar 13 06:14:35 2024, max compression
```

## Comparing `accelbyte-py-sdk-service-session-0.8.0.tar` & `accelbyte-py-sdk-service-session-0.9.0.tar`

### file list

```diff
@@ -1,199 +1,200 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:42:02.679661 accelbyte-py-sdk-service-session-0.8.0/
--rw-r--r--   0 root         (0) root         (0)     1126 2024-02-27 05:42:02.679661 accelbyte-py-sdk-service-session-0.8.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      874 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:42:02.663661 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:42:02.663661 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:42:02.663661 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/
--rw-rw-r--   0 root         (0) root         (0)     8940 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:42:02.671661 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/
--rw-rw-r--   0 root         (0) root         (0)     5331 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6303 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_append_team_game_session_request.py
--rw-rw-r--   0 root         (0) root         (0)     4019 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_config_alert_request_create.py
--rw-rw-r--   0 root         (0) root         (0)     6061 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_config_alert_response.py
--rw-rw-r--   0 root         (0) root         (0)    29623 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_configuration_template_response.py
--rw-rw-r--   0 root         (0) root         (0)     5426 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_configuration_templates_response.py
--rw-rw-r--   0 root         (0) root         (0)    27225 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_create_configuration_template_request.py
--rw-rw-r--   0 root         (0) root         (0)    21065 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_create_game_session_request.py
--rw-rw-r--   0 root         (0) root         (0)    10943 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_create_party_request.py
--rw-rw-r--   0 root         (0) root         (0)     3928 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_delete_bulk_game_session_request.py
--rw-rw-r--   0 root         (0) root         (0)     5407 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_delete_bulk_game_sessions_api_response.py
--rw-rw-r--   0 root         (0) root         (0)     7039 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_ds_information_response.py
--rw-rw-r--   0 root         (0) root         (0)     4473 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_environment_variable_list_response.py
--rw-rw-r--   0 root         (0) root         (0)     6320 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_environment_variable_response.py
--rw-rw-r--   0 root         (0) root         (0)     5276 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_game_session_query_response.py
--rw-rw-r--   0 root         (0) root         (0)    18971 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_game_session_response.py
--rw-rw-r--   0 root         (0) root         (0)     8991 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_global_configuration_response.py
--rw-rw-r--   0 root         (0) root         (0)     3772 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_join_by_code_request.py
--rw-rw-r--   0 root         (0) root         (0)     5484 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_kick_response.py
--rw-rw-r--   0 root         (0) root         (0)     5178 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_native_session_paging_response.py
--rw-rw-r--   0 root         (0) root         (0)     5492 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_pagination.py
--rw-rw-r--   0 root         (0) root         (0)     5196 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_party_query_response.py
--rw-rw-r--   0 root         (0) root         (0)    14495 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_party_session_response.py
--rw-rw-r--   0 root         (0) root         (0)     7499 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_player_attributes_request_body.py
--rw-rw-r--   0 root         (0) root         (0)     8118 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_player_attributes_response_body.py
--rw-rw-r--   0 root         (0) root         (0)     5532 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_player_platform.py
--rw-rw-r--   0 root         (0) root         (0)     4070 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_players_current_platform_request.py
--rw-rw-r--   0 root         (0) root         (0)     4361 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_players_current_platform_response.py
--rw-rw-r--   0 root         (0) root         (0)     3896 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_promote_leader_request.py
--rw-rw-r--   0 root         (0) root         (0)    26389 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_public_configuration.py
--rw-rw-r--   0 root         (0) root         (0)     8321 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_put_global_configuration_request.py
--rw-rw-r--   0 root         (0) root         (0)     4294 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_put_platform_credentials_request.py
--rw-rw-r--   0 root         (0) root         (0)     5201 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_request_member.py
--rw-rw-r--   0 root         (0) root         (0)     4505 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_response_delete_bulk_game_sessions.py
--rw-rw-r--   0 root         (0) root         (0)     3755 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_server_secret.py
--rw-rw-r--   0 root         (0) root         (0)     4576 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_session_invite_request.py
--rw-rw-r--   0 root         (0) root         (0)     4039 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_session_invite_response.py
--rw-rw-r--   0 root         (0) root         (0)     3804 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_set_ds_ready_request.py
--rw-rw-r--   0 root         (0) root         (0)    27225 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_update_configuration_template_request.py
--rw-rw-r--   0 root         (0) root         (0)     4230 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_update_game_session_backfill_request.py
--rw-rw-r--   0 root         (0) root         (0)     4745 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_update_game_session_member_status_response.py
--rw-rw-r--   0 root         (0) root         (0)    17963 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_update_game_session_request.py
--rw-rw-r--   0 root         (0) root         (0)     9018 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_update_party_request.py
--rw-rw-r--   0 root         (0) root         (0)     7187 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_user_response.py
--rw-rw-r--   0 root         (0) root         (0)     9420 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/model_native_session.py
--rw-rw-r--   0 root         (0) root         (0)     5309 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/model_native_session_member.py
--rw-rw-r--   0 root         (0) root         (0)     4736 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/models_default_dsmc_config.py
--rw-rw-r--   0 root         (0) root         (0)     6783 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/models_dsm_config_record.py
--rw-rw-r--   0 root         (0) root         (0)    17324 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/models_game_server.py
--rw-rw-r--   0 root         (0) root         (0)     8672 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/models_member_active_session.py
--rw-rw-r--   0 root         (0) root         (0)    12456 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/models_native_session_setting.py
--rw-rw-r--   0 root         (0) root         (0)     4452 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/models_party_members.py
--rw-rw-r--   0 root         (0) root         (0)     4831 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/models_platform_credentials.py
--rw-rw-r--   0 root         (0) root         (0)     4422 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/models_port_configuration_ams.py
--rw-rw-r--   0 root         (0) root         (0)     5251 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/models_psn_app_server_credentials.py
--rw-rw-r--   0 root         (0) root         (0)     4229 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/models_recent_player_query_response.py
--rw-rw-r--   0 root         (0) root         (0)     3957 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/models_request_reconcile_max_active_session.py
--rw-rw-r--   0 root         (0) root         (0)     4795 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/models_team.py
--rw-rw-r--   0 root         (0) root         (0)     6264 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/models_user_info_response.py
--rw-rw-r--   0 root         (0) root         (0)     4346 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/models_user_platform_info.py
--rw-rw-r--   0 root         (0) root         (0)     6528 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/response_error.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:42:02.671661 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/
--rw-rw-r--   0 root         (0) root         (0)      437 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:42:02.671661 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/certificate/
--rw-rw-r--   0 root         (0) root         (0)      545 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/certificate/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    10139 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/certificate/handle_upload_xbox_pfx__ac7973.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:42:02.671661 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/configuration_template/
--rw-rw-r--   0 root         (0) root         (0)     1302 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/configuration_template/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    12136 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/configuration_template/admin_create_configurat_34b9c2.py
--rw-rw-r--   0 root         (0) root         (0)     8203 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/configuration_template/admin_create_configurat_f62fb0.py
--rw-rw-r--   0 root         (0) root         (0)     6308 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/configuration_template/admin_delete_configurat_0f97ac.py
--rw-rw-r--   0 root         (0) root         (0)     7031 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/configuration_template/admin_delete_configurat_f38a32.py
--rw-rw-r--   0 root         (0) root         (0)    10707 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/configuration_template/admin_get_all_configura_f8d91f.py
--rw-rw-r--   0 root         (0) root         (0)     6673 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/configuration_template/admin_get_configuration_6c66b1.py
--rw-rw-r--   0 root         (0) root         (0)     7490 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/configuration_template/admin_get_configuration_b1005a.py
--rw-rw-r--   0 root         (0) root         (0)     6591 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/configuration_template/admin_get_dsmc_configuration.py
--rw-rw-r--   0 root         (0) root         (0)     6605 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/configuration_template/admin_sync_dsmc_configuration.py
--rw-rw-r--   0 root         (0) root         (0)     7992 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/configuration_template/admin_update_configurat_5d9582.py
--rw-rw-r--   0 root         (0) root         (0)    12547 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/configuration_template/admin_update_configurat_b6ef34.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:42:02.671661 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/dsmc_default_configuration/
--rw-rw-r--   0 root         (0) root         (0)      547 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/dsmc_default_configuration/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5667 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/dsmc_default_configuration/admin_get_dsmc_configur_e05bc8.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:42:02.671661 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/environment_variable/
--rw-rw-r--   0 root         (0) root         (0)      544 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/environment_variable/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5153 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/environment_variable/admin_list_environment__aed044.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:42:02.675661 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/game_session/
--rw-rw-r--   0 root         (0) root         (0)     1974 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/game_session/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7821 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/game_session/admin_delete_bulk_game__144132.py
--rw-rw-r--   0 root         (0) root         (0)     8147 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/game_session/admin_query_game_sessio_9fd853.py
--rw-rw-r--   0 root         (0) root         (0)    21249 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/game_session/admin_query_game_sessions.py
--rw-rw-r--   0 root         (0) root         (0)     8317 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/game_session/admin_set_ds_ready.py
--rw-rw-r--   0 root         (0) root         (0)     9394 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/game_session/admin_update_game_sessi_718745.py
--rw-rw-r--   0 root         (0) root         (0)     8558 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/game_session/append_team_game_session.py
--rw-rw-r--   0 root         (0) root         (0)     9328 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/game_session/create_game_session.py
--rw-rw-r--   0 root         (0) root         (0)     6829 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/game_session/delete_game_session.py
--rw-rw-r--   0 root         (0) root         (0)     7505 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/game_session/game_session_generate_code.py
--rw-rw-r--   0 root         (0) root         (0)     7924 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/game_session/get_game_session.py
--rw-rw-r--   0 root         (0) root         (0)     7826 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/game_session/get_game_session_by_pod_name.py
--rw-rw-r--   0 root         (0) root         (0)     7746 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/game_session/get_session_server_secret.py
--rw-rw-r--   0 root         (0) root         (0)     7380 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/game_session/join_game_session.py
--rw-rw-r--   0 root         (0) root         (0)     7207 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/game_session/leave_game_session.py
--rw-rw-r--   0 root         (0) root         (0)     8710 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/game_session/patch_update_game_session.py
--rw-rw-r--   0 root         (0) root         (0)     8678 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/game_session/public_game_session_invite.py
--rw-rw-r--   0 root         (0) root         (0)     7325 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/game_session/public_game_session_reject.py
--rw-rw-r--   0 root         (0) root         (0)     9405 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/game_session/public_promote_game_ses_482ff3.py
--rw-rw-r--   0 root         (0) root         (0)     8137 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/game_session/public_query_game_sessi_875927.py
--rw-rw-r--   0 root         (0) root         (0)     9308 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/game_session/public_query_my_game_sessions.py
--rw-rw-r--   0 root         (0) root         (0)     7367 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/game_session/public_revoke_game_sess_c2a52e.py
--rw-rw-r--   0 root         (0) root         (0)     7816 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/game_session/public_session_join_code.py
--rw-rw-r--   0 root         (0) root         (0)     9004 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/game_session/update_game_session.py
--rw-rw-r--   0 root         (0) root         (0)     8760 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/game_session/update_game_session_bac_df8b84.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:42:02.675661 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/global_configuration/
--rw-rw-r--   0 root         (0) root         (0)      693 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/global_configuration/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4887 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/global_configuration/admin_delete_global_con_ede905.py
--rw-rw-r--   0 root         (0) root         (0)     5092 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/global_configuration/admin_list_global_confi_b0d245.py
--rw-rw-r--   0 root         (0) root         (0)     6378 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/global_configuration/admin_update_global_con_006df0.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:42:02.675661 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/max_active/
--rw-rw-r--   0 root         (0) root         (0)      617 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/max_active/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7729 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/max_active/admin_get_member_active_3765c4.py
--rw-rw-r--   0 root         (0) root         (0)     8121 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/max_active/admin_reconcile_max_act_4f7653.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:42:02.675661 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/native_session/
--rw-rw-r--   0 root         (0) root         (0)      539 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/native_session/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8497 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/native_session/admin_get_list_native_session.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:42:02.675661 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/operations/
--rw-rw-r--   0 root         (0) root         (0)      581 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/operations/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4178 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/operations/get_healthcheck_info.py
--rw-rw-r--   0 root         (0) root         (0)     4205 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/operations/get_healthcheck_info_v1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:42:02.675661 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/party/
--rw-rw-r--   0 root         (0) root         (0)     1279 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/party/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    16206 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/party/admin_query_parties.py
--rw-rw-r--   0 root         (0) root         (0)     8176 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/party/public_create_party.py
--rw-rw-r--   0 root         (0) root         (0)     7395 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/party/public_generate_party_code.py
--rw-rw-r--   0 root         (0) root         (0)     6920 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/party/public_get_party.py
--rw-rw-r--   0 root         (0) root         (0)     8698 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/party/public_party_invite.py
--rw-rw-r--   0 root         (0) root         (0)     7426 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/party/public_party_join.py
--rw-rw-r--   0 root         (0) root         (0)     7804 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/party/public_party_join_code.py
--rw-rw-r--   0 root         (0) root         (0)     8118 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/party/public_party_kick.py
--rw-rw-r--   0 root         (0) root         (0)     6783 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/party/public_party_leave.py
--rw-rw-r--   0 root         (0) root         (0)     7210 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/party/public_party_reject.py
--rw-rw-r--   0 root         (0) root         (0)     8901 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/party/public_patch_update_party.py
--rw-rw-r--   0 root         (0) root         (0)     8673 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/party/public_promote_party_leader.py
--rw-rw-r--   0 root         (0) root         (0)     8796 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/party/public_query_my_parties.py
--rw-rw-r--   0 root         (0) root         (0)     7182 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/party/public_revoke_party_code.py
--rw-rw-r--   0 root         (0) root         (0)     9045 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/party/public_update_party.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:42:02.675661 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/platform_credential/
--rw-rw-r--   0 root         (0) root         (0)      692 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/platform_credential/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6524 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/platform_credential/admin_delete_platform_c_b8f2c5.py
--rw-rw-r--   0 root         (0) root         (0)     6999 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/platform_credential/admin_get_platform_credentials.py
--rw-rw-r--   0 root         (0) root         (0)     8278 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/platform_credential/admin_update_platform_c_5be87f.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:42:02.675661 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/player/
--rw-rw-r--   0 root         (0) root         (0)      898 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/player/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7909 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/player/admin_get_player_attributes.py
--rw-rw-r--   0 root         (0) root         (0)     8188 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/player/admin_query_player_attributes.py
--rw-rw-r--   0 root         (0) root         (0)     6236 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/player/public_delete_player_at_57835b.py
--rw-rw-r--   0 root         (0) root         (0)     7870 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/player/public_get_bulk_player__da8481.py
--rw-rw-r--   0 root         (0) root         (0)     7120 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/player/public_get_player_attributes.py
--rw-rw-r--   0 root         (0) root         (0)     8239 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/player/public_store_player_attributes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:42:02.675661 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/recent_player/
--rw-rw-r--   0 root         (0) root         (0)      530 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/recent_player/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8170 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/recent_player/public_get_recent_player.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:42:02.679661 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/session_storage/
--rw-rw-r--   0 root         (0) root         (0)      840 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/session_storage/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7127 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/session_storage/admin_delete_user_sessi_e92b87.py
--rw-rw-r--   0 root         (0) root         (0)     7137 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/session_storage/admin_read_session_storage.py
--rw-rw-r--   0 root         (0) root         (0)     7941 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/session_storage/admin_read_user_session_f101bc.py
--rw-rw-r--   0 root         (0) root         (0)     8604 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/session_storage/public_update_insert_se_4c0538.py
--rw-rw-r--   0 root         (0) root         (0)     9330 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/session_storage/public_update_insert_se_f96597.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:42:02.679661 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/wrappers/
--rw-rw-r--   0 root         (0) root         (0)     9545 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/wrappers/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4831 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/wrappers/_certificate.py
--rw-rw-r--   0 root         (0) root         (0)    49610 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/wrappers/_configuration_template.py
--rw-rw-r--   0 root         (0) root         (0)     3372 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/wrappers/_dsmc_default_configuration.py
--rw-rw-r--   0 root         (0) root         (0)     3002 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/wrappers/_environment_variable.py
--rw-rw-r--   0 root         (0) root         (0)    88517 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/wrappers/_game_session.py
--rw-rw-r--   0 root         (0) root         (0)     6979 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/wrappers/_global_configuration.py
--rw-rw-r--   0 root         (0) root         (0)     6942 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/wrappers/_max_active.py
--rw-rw-r--   0 root         (0) root         (0)     4068 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/wrappers/_native_session.py
--rw-rw-r--   0 root         (0) root         (0)     3381 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/wrappers/_operations.py
--rw-rw-r--   0 root         (0) root         (0)    50175 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/wrappers/_party.py
--rw-rw-r--   0 root         (0) root         (0)    11084 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/wrappers/_platform_credential.py
--rw-rw-r--   0 root         (0) root         (0)    22954 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/wrappers/_player.py
--rw-rw-r--   0 root         (0) root         (0)     4142 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/wrappers/_recent_player.py
--rw-rw-r--   0 root         (0) root         (0)    16855 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/wrappers/_session_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:42:02.679661 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk_service_session.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1126 2024-02-27 05:42:02.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk_service_session.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12985 2024-02-27 05:42:02.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk_service_session.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-27 05:42:02.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk_service_session.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       22 2024-02-27 05:42:02.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk_service_session.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-02-27 05:42:02.000000 accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk_service_session.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)      359 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-session-0.8.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-27 05:42:02.679661 accelbyte-py-sdk-service-session-0.8.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:14:35.812431 accelbyte-py-sdk-service-session-0.9.0/
+-rw-r--r--   0 root         (0) root         (0)     1125 2024-03-13 06:14:35.812431 accelbyte-py-sdk-service-session-0.9.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      873 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:14:35.796431 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:14:35.796431 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:14:35.796431 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/
+-rw-rw-r--   0 root         (0) root         (0)     9037 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:14:35.800431 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/
+-rw-rw-r--   0 root         (0) root         (0)     5330 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     6303 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_append_team_game_session_request.py
+-rw-rw-r--   0 root         (0) root         (0)     4019 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_config_alert_request_create.py
+-rw-rw-r--   0 root         (0) root         (0)     6061 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_config_alert_response.py
+-rw-rw-r--   0 root         (0) root         (0)    29623 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_configuration_template_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5426 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_configuration_templates_response.py
+-rw-rw-r--   0 root         (0) root         (0)    27225 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_create_configuration_template_request.py
+-rw-rw-r--   0 root         (0) root         (0)    21065 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_create_game_session_request.py
+-rw-rw-r--   0 root         (0) root         (0)    10943 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_create_party_request.py
+-rw-rw-r--   0 root         (0) root         (0)     3928 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_delete_bulk_game_session_request.py
+-rw-rw-r--   0 root         (0) root         (0)     5407 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_delete_bulk_game_sessions_api_response.py
+-rw-rw-r--   0 root         (0) root         (0)     7039 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_ds_information_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4473 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_environment_variable_list_response.py
+-rw-rw-r--   0 root         (0) root         (0)     6320 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_environment_variable_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5276 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_game_session_query_response.py
+-rw-rw-r--   0 root         (0) root         (0)    18971 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_game_session_response.py
+-rw-rw-r--   0 root         (0) root         (0)     8991 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_global_configuration_response.py
+-rw-rw-r--   0 root         (0) root         (0)     3772 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_join_by_code_request.py
+-rw-rw-r--   0 root         (0) root         (0)     5484 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_kick_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5178 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_native_session_paging_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5492 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_pagination.py
+-rw-rw-r--   0 root         (0) root         (0)     5196 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_party_query_response.py
+-rw-rw-r--   0 root         (0) root         (0)    14495 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_party_session_response.py
+-rw-rw-r--   0 root         (0) root         (0)     7499 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_player_attributes_request_body.py
+-rw-rw-r--   0 root         (0) root         (0)     8118 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_player_attributes_response_body.py
+-rw-rw-r--   0 root         (0) root         (0)     5532 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_player_platform.py
+-rw-rw-r--   0 root         (0) root         (0)     4070 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_players_current_platform_request.py
+-rw-rw-r--   0 root         (0) root         (0)     4361 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_players_current_platform_response.py
+-rw-rw-r--   0 root         (0) root         (0)     3896 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_promote_leader_request.py
+-rw-rw-r--   0 root         (0) root         (0)    26389 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_public_configuration.py
+-rw-rw-r--   0 root         (0) root         (0)     8321 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_put_global_configuration_request.py
+-rw-rw-r--   0 root         (0) root         (0)     4294 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_put_platform_credentials_request.py
+-rw-rw-r--   0 root         (0) root         (0)     5201 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_request_member.py
+-rw-rw-r--   0 root         (0) root         (0)     4505 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_response_delete_bulk_game_sessions.py
+-rw-rw-r--   0 root         (0) root         (0)     3755 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_server_secret.py
+-rw-rw-r--   0 root         (0) root         (0)     4576 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_session_invite_request.py
+-rw-rw-r--   0 root         (0) root         (0)     4039 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_session_invite_response.py
+-rw-rw-r--   0 root         (0) root         (0)     3804 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_set_ds_ready_request.py
+-rw-rw-r--   0 root         (0) root         (0)    27225 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_update_configuration_template_request.py
+-rw-rw-r--   0 root         (0) root         (0)     4230 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_update_game_session_backfill_request.py
+-rw-rw-r--   0 root         (0) root         (0)     4745 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_update_game_session_member_status_response.py
+-rw-rw-r--   0 root         (0) root         (0)    17963 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_update_game_session_request.py
+-rw-rw-r--   0 root         (0) root         (0)     9018 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_update_party_request.py
+-rw-rw-r--   0 root         (0) root         (0)     7187 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_user_response.py
+-rw-rw-r--   0 root         (0) root         (0)     9420 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/model_native_session.py
+-rw-rw-r--   0 root         (0) root         (0)     5309 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/model_native_session_member.py
+-rw-rw-r--   0 root         (0) root         (0)     4736 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/models_default_dsmc_config.py
+-rw-rw-r--   0 root         (0) root         (0)     6783 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/models_dsm_config_record.py
+-rw-rw-r--   0 root         (0) root         (0)    17324 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/models_game_server.py
+-rw-rw-r--   0 root         (0) root         (0)     8672 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/models_member_active_session.py
+-rw-rw-r--   0 root         (0) root         (0)    12456 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/models_native_session_setting.py
+-rw-rw-r--   0 root         (0) root         (0)     4452 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/models_party_members.py
+-rw-rw-r--   0 root         (0) root         (0)     4831 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/models_platform_credentials.py
+-rw-rw-r--   0 root         (0) root         (0)     4422 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/models_port_configuration_ams.py
+-rw-rw-r--   0 root         (0) root         (0)     5251 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/models_psn_app_server_credentials.py
+-rw-rw-r--   0 root         (0) root         (0)     4229 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/models_recent_player_query_response.py
+-rw-rw-r--   0 root         (0) root         (0)     3957 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/models_request_reconcile_max_active_session.py
+-rw-rw-r--   0 root         (0) root         (0)     4795 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/models_team.py
+-rw-rw-r--   0 root         (0) root         (0)     6264 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/models_user_info_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4346 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/models_user_platform_info.py
+-rw-rw-r--   0 root         (0) root         (0)     6528 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/response_error.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:14:35.800431 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/
+-rw-rw-r--   0 root         (0) root         (0)      436 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:14:35.800431 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/certificate/
+-rw-rw-r--   0 root         (0) root         (0)      544 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/certificate/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    10139 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/certificate/handle_upload_xbox_pfx__ac7973.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:14:35.804431 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/configuration_template/
+-rw-rw-r--   0 root         (0) root         (0)     1301 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/configuration_template/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    12136 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/configuration_template/admin_create_configurat_34b9c2.py
+-rw-rw-r--   0 root         (0) root         (0)     8203 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/configuration_template/admin_create_configurat_f62fb0.py
+-rw-rw-r--   0 root         (0) root         (0)     6308 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/configuration_template/admin_delete_configurat_0f97ac.py
+-rw-rw-r--   0 root         (0) root         (0)     7031 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/configuration_template/admin_delete_configurat_f38a32.py
+-rw-rw-r--   0 root         (0) root         (0)    10707 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/configuration_template/admin_get_all_configura_f8d91f.py
+-rw-rw-r--   0 root         (0) root         (0)     6673 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/configuration_template/admin_get_configuration_6c66b1.py
+-rw-rw-r--   0 root         (0) root         (0)     7490 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/configuration_template/admin_get_configuration_b1005a.py
+-rw-rw-r--   0 root         (0) root         (0)     6591 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/configuration_template/admin_get_dsmc_configuration.py
+-rw-rw-r--   0 root         (0) root         (0)     6605 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/configuration_template/admin_sync_dsmc_configuration.py
+-rw-rw-r--   0 root         (0) root         (0)     7992 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/configuration_template/admin_update_configurat_5d9582.py
+-rw-rw-r--   0 root         (0) root         (0)    12547 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/configuration_template/admin_update_configurat_b6ef34.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:14:35.804431 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/dsmc_default_configuration/
+-rw-rw-r--   0 root         (0) root         (0)      546 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/dsmc_default_configuration/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     5667 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/dsmc_default_configuration/admin_get_dsmc_configur_e05bc8.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:14:35.804431 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/environment_variable/
+-rw-rw-r--   0 root         (0) root         (0)      543 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/environment_variable/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     5153 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/environment_variable/admin_list_environment__aed044.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:14:35.804431 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/game_session/
+-rw-rw-r--   0 root         (0) root         (0)     1973 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/game_session/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7821 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/game_session/admin_delete_bulk_game__144132.py
+-rw-rw-r--   0 root         (0) root         (0)     8147 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/game_session/admin_query_game_sessio_9fd853.py
+-rw-rw-r--   0 root         (0) root         (0)    21249 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/game_session/admin_query_game_sessions.py
+-rw-rw-r--   0 root         (0) root         (0)     8317 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/game_session/admin_set_ds_ready.py
+-rw-rw-r--   0 root         (0) root         (0)     9394 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/game_session/admin_update_game_sessi_718745.py
+-rw-rw-r--   0 root         (0) root         (0)     8558 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/game_session/append_team_game_session.py
+-rw-rw-r--   0 root         (0) root         (0)     9328 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/game_session/create_game_session.py
+-rw-rw-r--   0 root         (0) root         (0)     6829 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/game_session/delete_game_session.py
+-rw-rw-r--   0 root         (0) root         (0)     7505 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/game_session/game_session_generate_code.py
+-rw-rw-r--   0 root         (0) root         (0)     7924 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/game_session/get_game_session.py
+-rw-rw-r--   0 root         (0) root         (0)     7826 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/game_session/get_game_session_by_pod_name.py
+-rw-rw-r--   0 root         (0) root         (0)     7746 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/game_session/get_session_server_secret.py
+-rw-rw-r--   0 root         (0) root         (0)     7380 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/game_session/join_game_session.py
+-rw-rw-r--   0 root         (0) root         (0)     7207 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/game_session/leave_game_session.py
+-rw-rw-r--   0 root         (0) root         (0)     8710 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/game_session/patch_update_game_session.py
+-rw-rw-r--   0 root         (0) root         (0)     8678 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/game_session/public_game_session_invite.py
+-rw-rw-r--   0 root         (0) root         (0)     7325 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/game_session/public_game_session_reject.py
+-rw-rw-r--   0 root         (0) root         (0)     9405 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/game_session/public_promote_game_ses_482ff3.py
+-rw-rw-r--   0 root         (0) root         (0)     8137 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/game_session/public_query_game_sessi_875927.py
+-rw-rw-r--   0 root         (0) root         (0)     9308 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/game_session/public_query_my_game_sessions.py
+-rw-rw-r--   0 root         (0) root         (0)     7367 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/game_session/public_revoke_game_sess_c2a52e.py
+-rw-rw-r--   0 root         (0) root         (0)     7816 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/game_session/public_session_join_code.py
+-rw-rw-r--   0 root         (0) root         (0)     9004 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/game_session/update_game_session.py
+-rw-rw-r--   0 root         (0) root         (0)     8760 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/game_session/update_game_session_bac_df8b84.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:14:35.804431 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/global_configuration/
+-rw-rw-r--   0 root         (0) root         (0)      692 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/global_configuration/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4887 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/global_configuration/admin_delete_global_con_ede905.py
+-rw-rw-r--   0 root         (0) root         (0)     5092 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/global_configuration/admin_list_global_confi_b0d245.py
+-rw-rw-r--   0 root         (0) root         (0)     6378 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/global_configuration/admin_update_global_con_006df0.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:14:35.808431 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/max_active/
+-rw-rw-r--   0 root         (0) root         (0)      616 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/max_active/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7729 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/max_active/admin_get_member_active_3765c4.py
+-rw-rw-r--   0 root         (0) root         (0)     8121 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/max_active/admin_reconcile_max_act_4f7653.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:14:35.808431 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/native_session/
+-rw-rw-r--   0 root         (0) root         (0)      538 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/native_session/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8497 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/native_session/admin_get_list_native_session.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:14:35.808431 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/operations/
+-rw-rw-r--   0 root         (0) root         (0)      580 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/operations/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4178 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/operations/get_healthcheck_info.py
+-rw-rw-r--   0 root         (0) root         (0)     4205 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/operations/get_healthcheck_info_v1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:14:35.808431 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/party/
+-rw-rw-r--   0 root         (0) root         (0)     1278 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/party/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    16206 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/party/admin_query_parties.py
+-rw-rw-r--   0 root         (0) root         (0)     8176 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/party/public_create_party.py
+-rw-rw-r--   0 root         (0) root         (0)     7395 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/party/public_generate_party_code.py
+-rw-rw-r--   0 root         (0) root         (0)     6920 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/party/public_get_party.py
+-rw-rw-r--   0 root         (0) root         (0)     8698 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/party/public_party_invite.py
+-rw-rw-r--   0 root         (0) root         (0)     7426 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/party/public_party_join.py
+-rw-rw-r--   0 root         (0) root         (0)     7804 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/party/public_party_join_code.py
+-rw-rw-r--   0 root         (0) root         (0)     8118 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/party/public_party_kick.py
+-rw-rw-r--   0 root         (0) root         (0)     6783 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/party/public_party_leave.py
+-rw-rw-r--   0 root         (0) root         (0)     7210 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/party/public_party_reject.py
+-rw-rw-r--   0 root         (0) root         (0)     8901 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/party/public_patch_update_party.py
+-rw-rw-r--   0 root         (0) root         (0)     8673 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/party/public_promote_party_leader.py
+-rw-rw-r--   0 root         (0) root         (0)     8796 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/party/public_query_my_parties.py
+-rw-rw-r--   0 root         (0) root         (0)     7182 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/party/public_revoke_party_code.py
+-rw-rw-r--   0 root         (0) root         (0)     9045 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/party/public_update_party.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:14:35.808431 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/platform_credential/
+-rw-rw-r--   0 root         (0) root         (0)      691 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/platform_credential/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     6524 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/platform_credential/admin_delete_platform_c_b8f2c5.py
+-rw-rw-r--   0 root         (0) root         (0)     6999 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/platform_credential/admin_get_platform_credentials.py
+-rw-rw-r--   0 root         (0) root         (0)     8278 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/platform_credential/admin_update_platform_c_5be87f.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:14:35.808431 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/player/
+-rw-rw-r--   0 root         (0) root         (0)      897 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/player/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7909 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/player/admin_get_player_attributes.py
+-rw-rw-r--   0 root         (0) root         (0)     8188 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/player/admin_query_player_attributes.py
+-rw-rw-r--   0 root         (0) root         (0)     6236 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/player/public_delete_player_at_57835b.py
+-rw-rw-r--   0 root         (0) root         (0)     7870 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/player/public_get_bulk_player__da8481.py
+-rw-rw-r--   0 root         (0) root         (0)     7120 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/player/public_get_player_attributes.py
+-rw-rw-r--   0 root         (0) root         (0)     8239 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/player/public_store_player_attributes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:14:35.808431 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/recent_player/
+-rw-rw-r--   0 root         (0) root         (0)      587 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/recent_player/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8161 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/recent_player/admin_get_recent_player.py
+-rw-rw-r--   0 root         (0) root         (0)     7347 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/recent_player/public_get_recent_player.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:14:35.808431 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/session_storage/
+-rw-rw-r--   0 root         (0) root         (0)      839 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/session_storage/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7127 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/session_storage/admin_delete_user_sessi_e92b87.py
+-rw-rw-r--   0 root         (0) root         (0)     7137 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/session_storage/admin_read_session_storage.py
+-rw-rw-r--   0 root         (0) root         (0)     7941 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/session_storage/admin_read_user_session_f101bc.py
+-rw-rw-r--   0 root         (0) root         (0)     8604 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/session_storage/public_update_insert_se_4c0538.py
+-rw-rw-r--   0 root         (0) root         (0)     9330 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/session_storage/public_update_insert_se_f96597.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:14:35.812431 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/wrappers/
+-rw-rw-r--   0 root         (0) root         (0)     9654 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/wrappers/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4831 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/wrappers/_certificate.py
+-rw-rw-r--   0 root         (0) root         (0)    49610 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/wrappers/_configuration_template.py
+-rw-rw-r--   0 root         (0) root         (0)     3372 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/wrappers/_dsmc_default_configuration.py
+-rw-rw-r--   0 root         (0) root         (0)     3002 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/wrappers/_environment_variable.py
+-rw-rw-r--   0 root         (0) root         (0)    88517 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/wrappers/_game_session.py
+-rw-rw-r--   0 root         (0) root         (0)     6979 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/wrappers/_global_configuration.py
+-rw-rw-r--   0 root         (0) root         (0)     6942 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/wrappers/_max_active.py
+-rw-rw-r--   0 root         (0) root         (0)     4068 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/wrappers/_native_session.py
+-rw-rw-r--   0 root         (0) root         (0)     3381 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/wrappers/_operations.py
+-rw-rw-r--   0 root         (0) root         (0)    50175 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/wrappers/_party.py
+-rw-rw-r--   0 root         (0) root         (0)    11084 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/wrappers/_platform_credential.py
+-rw-rw-r--   0 root         (0) root         (0)    22954 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/wrappers/_player.py
+-rw-rw-r--   0 root         (0) root         (0)     6858 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/wrappers/_recent_player.py
+-rw-rw-r--   0 root         (0) root         (0)    16855 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/wrappers/_session_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:14:35.812431 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk_service_session.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1125 2024-03-13 06:14:35.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk_service_session.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    13066 2024-03-13 06:14:35.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk_service_session.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-03-13 06:14:35.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk_service_session.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-03-13 06:14:35.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk_service_session.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-03-13 06:14:35.000000 accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk_service_session.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)      359 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-session-0.9.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-03-13 06:14:35.812431 accelbyte-py-sdk-service-session-0.9.0/setup.cfg
```

### Comparing `accelbyte-py-sdk-service-session-0.8.0/PKG-INFO` & `accelbyte-py-sdk-service-session-0.9.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: accelbyte-py-sdk-service-session
-Version: 0.8.0
+Version: 0.9.0
 Summary: AccelByte Python SDK - AccelByte Gaming Services Session Service
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: accelbyte-py-sdk-core
 
 [//]: # (Code generated. DO NOT EDIT!)
 
 # AccelByte Modular Python SDK - Service Module
 
 This is a service module for the [AccelByte Modular Python SDK](https://github.com/AccelByte/accelbyte-python-modular-sdk) package.
 
 ```text
 AccelByte Gaming Services Session Service
-* Version: 3.13.14
+* Version: 3.14.0
 ```
 
 ## Setup
 
 This SDK requires Python 3.9 to be installed.
 
 ### Install with Pip
```

### Comparing `accelbyte-py-sdk-service-session-0.8.0/README.md` & `accelbyte-py-sdk-service-session-0.9.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # AccelByte Modular Python SDK - Service Module
 
 This is a service module for the [AccelByte Modular Python SDK](https://github.com/AccelByte/accelbyte-python-modular-sdk) package.
 
 ```text
 AccelByte Gaming Services Session Service
-* Version: 3.13.14
+* Version: 3.14.0
 ```
 
 ## Setup
 
 This SDK requires Python 3.9 to be installed.
 
 ### Install with Pip
```

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/__init__.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: service-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Session Service."""
 
-__version__ = "3.13.14"
+__version__ = "3.14.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 # certificate
 from .wrappers import handle_upload_xbox_pfx_certificate
@@ -175,14 +175,16 @@
 from .wrappers import public_get_bulk_player_current_platform_async
 from .wrappers import public_get_player_attributes
 from .wrappers import public_get_player_attributes_async
 from .wrappers import public_store_player_attributes
 from .wrappers import public_store_player_attributes_async
 
 # recent_player
+from .wrappers import admin_get_recent_player
+from .wrappers import admin_get_recent_player_async
 from .wrappers import public_get_recent_player
 from .wrappers import public_get_recent_player_async
 
 # session_storage
 from .wrappers import admin_delete_user_session_storage
 from .wrappers import admin_delete_user_session_storage_async
 from .wrappers import admin_read_session_storage
```

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/__init__.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: model-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Session Service."""
 
-__version__ = "3.13.14"
+__version__ = "3.14.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .apimodels_append_team_game_session_request import (
     ApimodelsAppendTeamGameSessionRequest,
```

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_append_team_game_session_request.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_append_team_game_session_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_config_alert_request_create.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_config_alert_request_create.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_config_alert_response.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_config_alert_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_configuration_template_response.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_configuration_template_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_configuration_templates_response.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_configuration_templates_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_create_configuration_template_request.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_create_configuration_template_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_create_game_session_request.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_create_game_session_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_create_party_request.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_create_party_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_delete_bulk_game_session_request.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_delete_bulk_game_session_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_delete_bulk_game_sessions_api_response.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_delete_bulk_game_sessions_api_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_ds_information_response.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_ds_information_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_environment_variable_list_response.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_environment_variable_list_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_environment_variable_response.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_environment_variable_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_game_session_query_response.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_game_session_query_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_game_session_response.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_game_session_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_global_configuration_response.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_global_configuration_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_join_by_code_request.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_join_by_code_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_kick_response.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_kick_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_native_session_paging_response.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_native_session_paging_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_pagination.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_pagination.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_party_query_response.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_party_query_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_party_session_response.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_party_session_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_player_attributes_request_body.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_player_attributes_request_body.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_player_attributes_response_body.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_player_attributes_response_body.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_player_platform.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_player_platform.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_players_current_platform_request.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_players_current_platform_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_players_current_platform_response.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_players_current_platform_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_promote_leader_request.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_promote_leader_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_public_configuration.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_public_configuration.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_put_global_configuration_request.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_put_global_configuration_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_put_platform_credentials_request.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_put_platform_credentials_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_request_member.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_request_member.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_response_delete_bulk_game_sessions.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_response_delete_bulk_game_sessions.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_server_secret.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_server_secret.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_session_invite_request.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_session_invite_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_session_invite_response.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_session_invite_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_set_ds_ready_request.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_set_ds_ready_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_update_configuration_template_request.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_update_configuration_template_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_update_game_session_backfill_request.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_update_game_session_backfill_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_update_game_session_member_status_response.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_update_game_session_member_status_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_update_game_session_request.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_update_game_session_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_update_party_request.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_update_party_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/apimodels_user_response.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/apimodels_user_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/model_native_session.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/model_native_session.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/model_native_session_member.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/model_native_session_member.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/models_default_dsmc_config.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/models_default_dsmc_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/models_dsm_config_record.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/models_dsm_config_record.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/models_game_server.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/models_game_server.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/models_member_active_session.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/models_member_active_session.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/models_native_session_setting.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/models_native_session_setting.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/models_party_members.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/models_party_members.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/models_platform_credentials.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/models_platform_credentials.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/models_port_configuration_ams.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/models_port_configuration_ams.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/models_psn_app_server_credentials.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/models_psn_app_server_credentials.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/models_recent_player_query_response.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/models_recent_player_query_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/models_request_reconcile_max_active_session.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/models_request_reconcile_max_active_session.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/models_team.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/models_team.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/models_user_info_response.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/models_user_info_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/models_user_platform_info.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/models_user_platform_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/models/response_error.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/models/response_error.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/certificate/__init__.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/certificate/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,14 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Session Service."""
 
-__version__ = "3.13.14"
+__version__ = "3.14.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .handle_upload_xbox_pfx__ac7973 import HandleUploadXboxPFXCertificate
```

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/certificate/handle_upload_xbox_pfx__ac7973.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/certificate/handle_upload_xbox_pfx__ac7973.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/configuration_template/__init__.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/configuration_template/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Session Service."""
 
-__version__ = "3.13.14"
+__version__ = "3.14.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .admin_create_configurat_f62fb0 import AdminCreateConfigurationAlertV1
 from .admin_create_configurat_34b9c2 import AdminCreateConfigurationTemplateV1
```

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/configuration_template/admin_create_configurat_34b9c2.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/configuration_template/admin_create_configurat_34b9c2.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/configuration_template/admin_create_configurat_f62fb0.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/configuration_template/admin_create_configurat_f62fb0.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/configuration_template/admin_delete_configurat_0f97ac.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/configuration_template/admin_delete_configurat_0f97ac.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/configuration_template/admin_delete_configurat_f38a32.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/configuration_template/admin_delete_configurat_f38a32.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/configuration_template/admin_get_all_configura_f8d91f.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/configuration_template/admin_get_all_configura_f8d91f.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/configuration_template/admin_get_configuration_6c66b1.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/configuration_template/admin_get_configuration_6c66b1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/configuration_template/admin_get_configuration_b1005a.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/configuration_template/admin_get_configuration_b1005a.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/configuration_template/admin_get_dsmc_configuration.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/configuration_template/admin_get_dsmc_configuration.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/configuration_template/admin_sync_dsmc_configuration.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/configuration_template/admin_sync_dsmc_configuration.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/configuration_template/admin_update_configurat_5d9582.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/configuration_template/admin_update_configurat_5d9582.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/configuration_template/admin_update_configurat_b6ef34.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/configuration_template/admin_update_configurat_b6ef34.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/dsmc_default_configuration/admin_get_dsmc_configur_e05bc8.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/dsmc_default_configuration/admin_get_dsmc_configur_e05bc8.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/environment_variable/__init__.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/environment_variable/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,14 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Session Service."""
 
-__version__ = "3.13.14"
+__version__ = "3.14.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .admin_list_environment__aed044 import AdminListEnvironmentVariables
```

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/environment_variable/admin_list_environment__aed044.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/environment_variable/admin_list_environment__aed044.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/game_session/__init__.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/game_session/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Session Service."""
 
-__version__ = "3.13.14"
+__version__ = "3.14.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .admin_delete_bulk_game__144132 import AdminDeleteBulkGameSessions
 from .admin_query_game_sessions import AdminQueryGameSessions
```

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/game_session/admin_delete_bulk_game__144132.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/game_session/admin_delete_bulk_game__144132.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/game_session/admin_query_game_sessio_9fd853.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/game_session/admin_query_game_sessio_9fd853.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/game_session/admin_query_game_sessions.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/game_session/admin_query_game_sessions.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/game_session/admin_set_ds_ready.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/game_session/admin_set_ds_ready.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/game_session/admin_update_game_sessi_718745.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/game_session/admin_update_game_sessi_718745.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/game_session/append_team_game_session.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/game_session/append_team_game_session.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/game_session/create_game_session.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/game_session/create_game_session.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/game_session/delete_game_session.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/game_session/delete_game_session.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/game_session/game_session_generate_code.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/game_session/game_session_generate_code.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/game_session/get_game_session.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/game_session/get_game_session.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/game_session/get_game_session_by_pod_name.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/game_session/get_game_session_by_pod_name.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/game_session/get_session_server_secret.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/game_session/get_session_server_secret.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/game_session/join_game_session.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/game_session/join_game_session.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/game_session/leave_game_session.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/game_session/leave_game_session.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/game_session/patch_update_game_session.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/game_session/patch_update_game_session.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/game_session/public_game_session_invite.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/game_session/public_game_session_invite.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/game_session/public_game_session_reject.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/game_session/public_game_session_reject.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/game_session/public_promote_game_ses_482ff3.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/game_session/public_promote_game_ses_482ff3.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/game_session/public_query_game_sessi_875927.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/game_session/public_query_game_sessi_875927.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/game_session/public_query_my_game_sessions.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/game_session/public_query_my_game_sessions.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/game_session/public_revoke_game_sess_c2a52e.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/game_session/public_revoke_game_sess_c2a52e.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/game_session/public_session_join_code.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/game_session/public_session_join_code.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/game_session/update_game_session.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/game_session/update_game_session.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/game_session/update_game_session_bac_df8b84.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/game_session/update_game_session_bac_df8b84.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/global_configuration/__init__.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/global_configuration/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Session Service."""
 
-__version__ = "3.13.14"
+__version__ = "3.14.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .admin_delete_global_con_ede905 import AdminDeleteGlobalConfiguration
 from .admin_list_global_confi_b0d245 import AdminListGlobalConfiguration
```

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/global_configuration/admin_delete_global_con_ede905.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/global_configuration/admin_delete_global_con_ede905.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/global_configuration/admin_list_global_confi_b0d245.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/global_configuration/admin_list_global_confi_b0d245.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/global_configuration/admin_update_global_con_006df0.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/global_configuration/admin_update_global_con_006df0.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/max_active/__init__.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/max_active/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Session Service."""
 
-__version__ = "3.13.14"
+__version__ = "3.14.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .admin_get_member_active_3765c4 import AdminGetMemberActiveSession
 from .admin_reconcile_max_act_4f7653 import AdminReconcileMaxActiveSession
```

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/max_active/admin_get_member_active_3765c4.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/max_active/admin_get_member_active_3765c4.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/max_active/admin_reconcile_max_act_4f7653.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/max_active/admin_reconcile_max_act_4f7653.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/native_session/__init__.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/native_session/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,14 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Session Service."""
 
-__version__ = "3.13.14"
+__version__ = "3.14.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .admin_get_list_native_session import AdminGetListNativeSession
```

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/native_session/admin_get_list_native_session.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/native_session/admin_get_list_native_session.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/operations/__init__.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/operations/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Session Service."""
 
-__version__ = "3.13.14"
+__version__ = "3.14.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .get_healthcheck_info import GetHealthcheckInfo
 from .get_healthcheck_info_v1 import GetHealthcheckInfoV1
```

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/operations/get_healthcheck_info.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/operations/get_healthcheck_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/operations/get_healthcheck_info_v1.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/operations/get_healthcheck_info_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/party/__init__.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/party/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Session Service."""
 
-__version__ = "3.13.14"
+__version__ = "3.14.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .admin_query_parties import AdminQueryParties
 from .public_create_party import PublicCreateParty
```

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/party/admin_query_parties.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/party/admin_query_parties.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/party/public_create_party.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/party/public_create_party.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/party/public_generate_party_code.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/party/public_generate_party_code.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/party/public_get_party.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/party/public_get_party.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/party/public_party_invite.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/party/public_party_invite.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/party/public_party_join.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/party/public_party_join.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/party/public_party_join_code.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/party/public_party_join_code.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/party/public_party_kick.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/party/public_party_kick.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/party/public_party_leave.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/party/public_party_leave.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/party/public_party_reject.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/party/public_party_reject.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/party/public_patch_update_party.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/party/public_patch_update_party.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/party/public_promote_party_leader.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/party/public_promote_party_leader.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/party/public_query_my_parties.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/party/public_query_my_parties.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/party/public_revoke_party_code.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/party/public_revoke_party_code.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/party/public_update_party.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/party/public_update_party.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/platform_credential/__init__.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/platform_credential/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Session Service."""
 
-__version__ = "3.13.14"
+__version__ = "3.14.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .admin_delete_platform_c_b8f2c5 import AdminDeletePlatformCredentials
 from .admin_get_platform_credentials import AdminGetPlatformCredentials
```

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/platform_credential/admin_delete_platform_c_b8f2c5.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/platform_credential/admin_delete_platform_c_b8f2c5.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/platform_credential/admin_get_platform_credentials.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/platform_credential/admin_get_platform_credentials.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/platform_credential/admin_update_platform_c_5be87f.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/platform_credential/admin_update_platform_c_5be87f.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/player/__init__.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/player/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Session Service."""
 
-__version__ = "3.13.14"
+__version__ = "3.14.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .admin_get_player_attributes import AdminGetPlayerAttributes
 from .admin_query_player_attributes import AdminQueryPlayerAttributes
```

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/player/admin_get_player_attributes.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/player/admin_get_player_attributes.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/player/admin_query_player_attributes.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/player/admin_query_player_attributes.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/player/public_delete_player_at_57835b.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/player/public_delete_player_at_57835b.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/player/public_get_bulk_player__da8481.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/player/public_get_bulk_player__da8481.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/player/public_get_player_attributes.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/player/public_get_player_attributes.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/player/public_store_player_attributes.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/player/public_store_player_attributes.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/recent_player/__init__.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/recent_player/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Session Service."""
 
-__version__ = "3.13.14"
+__version__ = "3.14.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
+from .admin_get_recent_player import AdminGetRecentPlayer
 from .public_get_recent_player import PublicGetRecentPlayer
```

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/recent_player/public_get_recent_player.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/recent_player/admin_get_recent_player.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,21 +29,21 @@
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
 from ...models import ModelsRecentPlayerQueryResponse
 from ...models import ResponseError
 
 
-class PublicGetRecentPlayer(Operation):
-    """Query recent player with given user id. (publicGetRecentPlayer)
+class AdminGetRecentPlayer(Operation):
+    """Query recent player with given user id. (adminGetRecentPlayer)
 
     Query recent player with given user id.
 
     Properties:
-        url: /session/v1/public/namespaces/{namespace}/recent-player
+        url: /session/v1/admin/namespaces/{namespace}/recent-player
 
         method: GET
 
         tags: ["Recent Player"]
 
         consumes: ["application/json"]
 
@@ -67,15 +67,15 @@
         404: Not Found - ResponseError (Not Found)
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
-    _url: str = "/session/v1/public/namespaces/{namespace}/recent-player"
+    _url: str = "/session/v1/admin/namespaces/{namespace}/recent-player"
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
     namespace: str  # REQUIRED in [path]
@@ -142,23 +142,23 @@
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_namespace(self, value: str) -> PublicGetRecentPlayer:
+    def with_namespace(self, value: str) -> AdminGetRecentPlayer:
         self.namespace = value
         return self
 
-    def with_limit(self, value: int) -> PublicGetRecentPlayer:
+    def with_limit(self, value: int) -> AdminGetRecentPlayer:
         self.limit = value
         return self
 
-    def with_user_id(self, value: str) -> PublicGetRecentPlayer:
+    def with_user_id(self, value: str) -> AdminGetRecentPlayer:
         self.user_id = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
@@ -236,29 +236,29 @@
     @classmethod
     def create(
         cls,
         namespace: str,
         limit: Optional[int] = None,
         user_id: Optional[str] = None,
         **kwargs,
-    ) -> PublicGetRecentPlayer:
+    ) -> AdminGetRecentPlayer:
         instance = cls()
         instance.namespace = namespace
         if limit is not None:
             instance.limit = limit
         if user_id is not None:
             instance.user_id = user_id
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> PublicGetRecentPlayer:
+    ) -> AdminGetRecentPlayer:
         instance = cls()
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
         elif include_empty:
             instance.namespace = ""
         if "limit" in dict_ and dict_["limit"] is not None:
             instance.limit = int(dict_["limit"])
```

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/session_storage/__init__.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/session_storage/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Session Service."""
 
-__version__ = "3.13.14"
+__version__ = "3.14.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .admin_delete_user_sessi_e92b87 import AdminDeleteUserSessionStorage
 from .admin_read_session_storage import AdminReadSessionStorage
```

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/session_storage/admin_delete_user_sessi_e92b87.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/session_storage/admin_delete_user_sessi_e92b87.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/session_storage/admin_read_session_storage.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/session_storage/admin_read_session_storage.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/session_storage/admin_read_user_session_f101bc.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/session_storage/admin_read_user_session_f101bc.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/session_storage/public_update_insert_se_4c0538.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/session_storage/public_update_insert_se_4c0538.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/operations/session_storage/public_update_insert_se_f96597.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/operations/session_storage/public_update_insert_se_f96597.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/wrappers/__init__.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/wrappers/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: wrapper-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Session Service."""
 
-__version__ = "3.13.14"
+__version__ = "3.14.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from ._certificate import handle_upload_xbox_pfx_certificate
 from ._certificate import handle_upload_xbox_pfx_certificate_async
@@ -162,14 +162,16 @@
 from ._player import public_get_bulk_player_current_platform
 from ._player import public_get_bulk_player_current_platform_async
 from ._player import public_get_player_attributes
 from ._player import public_get_player_attributes_async
 from ._player import public_store_player_attributes
 from ._player import public_store_player_attributes_async
 
+from ._recent_player import admin_get_recent_player
+from ._recent_player import admin_get_recent_player_async
 from ._recent_player import public_get_recent_player
 from ._recent_player import public_get_recent_player_async
 
 from ._session_storage import admin_delete_user_session_storage
 from ._session_storage import admin_delete_user_session_storage_async
 from ._session_storage import admin_read_session_storage
 from ._session_storage import admin_read_session_storage_async
```

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/wrappers/_certificate.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/wrappers/_certificate.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/wrappers/_configuration_template.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/wrappers/_configuration_template.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/wrappers/_dsmc_default_configuration.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/wrappers/_dsmc_default_configuration.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/wrappers/_environment_variable.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/wrappers/_environment_variable.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/wrappers/_game_session.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/wrappers/_game_session.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/wrappers/_global_configuration.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/wrappers/_global_configuration.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/wrappers/_max_active.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/wrappers/_max_active.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/wrappers/_native_session.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/wrappers/_native_session.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/wrappers/_operations.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/wrappers/_operations.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/wrappers/_party.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/wrappers/_party.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/wrappers/_platform_credential.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/wrappers/_platform_credential.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/wrappers/_player.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/wrappers/_player.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/wrappers/_recent_player.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/wrappers/_recent_player.py`

 * *Files 25% similar despite different names*

```diff
@@ -28,21 +28,131 @@
 from accelbyte_py_sdk.core import run_request
 from accelbyte_py_sdk.core import run_request_async
 from accelbyte_py_sdk.core import same_doc_as
 
 from ..models import ModelsRecentPlayerQueryResponse
 from ..models import ResponseError
 
+from ..operations.recent_player import AdminGetRecentPlayer
 from ..operations.recent_player import PublicGetRecentPlayer
 
 
+@same_doc_as(AdminGetRecentPlayer)
+def admin_get_recent_player(
+    limit: Optional[int] = None,
+    user_id: Optional[str] = None,
+    namespace: Optional[str] = None,
+    x_additional_headers: Optional[Dict[str, str]] = None,
+    **kwargs
+):
+    """Query recent player with given user id. (adminGetRecentPlayer)
+
+    Query recent player with given user id.
+
+    Properties:
+        url: /session/v1/admin/namespaces/{namespace}/recent-player
+
+        method: GET
+
+        tags: ["Recent Player"]
+
+        consumes: ["application/json"]
+
+        produces: ["application/json"]
+
+        securities: [BEARER_AUTH]
+
+        namespace: (namespace) REQUIRED str in path
+
+        limit: (limit) OPTIONAL int in query
+
+        user_id: (userId) OPTIONAL str in query
+
+    Responses:
+        200: OK - ModelsRecentPlayerQueryResponse (OK)
+
+        400: Bad Request - ResponseError (Bad Request)
+
+        401: Unauthorized - ResponseError (Unauthorized)
+
+        404: Not Found - ResponseError (Not Found)
+
+        500: Internal Server Error - ResponseError (Internal Server Error)
+    """
+    if namespace is None:
+        namespace, error = get_services_namespace()
+        if error:
+            return None, error
+    request = AdminGetRecentPlayer.create(
+        limit=limit,
+        user_id=user_id,
+        namespace=namespace,
+    )
+    return run_request(request, additional_headers=x_additional_headers, **kwargs)
+
+
+@same_doc_as(AdminGetRecentPlayer)
+async def admin_get_recent_player_async(
+    limit: Optional[int] = None,
+    user_id: Optional[str] = None,
+    namespace: Optional[str] = None,
+    x_additional_headers: Optional[Dict[str, str]] = None,
+    **kwargs
+):
+    """Query recent player with given user id. (adminGetRecentPlayer)
+
+    Query recent player with given user id.
+
+    Properties:
+        url: /session/v1/admin/namespaces/{namespace}/recent-player
+
+        method: GET
+
+        tags: ["Recent Player"]
+
+        consumes: ["application/json"]
+
+        produces: ["application/json"]
+
+        securities: [BEARER_AUTH]
+
+        namespace: (namespace) REQUIRED str in path
+
+        limit: (limit) OPTIONAL int in query
+
+        user_id: (userId) OPTIONAL str in query
+
+    Responses:
+        200: OK - ModelsRecentPlayerQueryResponse (OK)
+
+        400: Bad Request - ResponseError (Bad Request)
+
+        401: Unauthorized - ResponseError (Unauthorized)
+
+        404: Not Found - ResponseError (Not Found)
+
+        500: Internal Server Error - ResponseError (Internal Server Error)
+    """
+    if namespace is None:
+        namespace, error = get_services_namespace()
+        if error:
+            return None, error
+    request = AdminGetRecentPlayer.create(
+        limit=limit,
+        user_id=user_id,
+        namespace=namespace,
+    )
+    return await run_request_async(
+        request, additional_headers=x_additional_headers, **kwargs
+    )
+
+
 @same_doc_as(PublicGetRecentPlayer)
 def public_get_recent_player(
     limit: Optional[int] = None,
-    user_id: Optional[str] = None,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Query recent player with given user id. (publicGetRecentPlayer)
 
     Query recent player with given user id.
@@ -60,16 +170,14 @@
 
         securities: [BEARER_AUTH]
 
         namespace: (namespace) REQUIRED str in path
 
         limit: (limit) OPTIONAL int in query
 
-        user_id: (userId) OPTIONAL str in query
-
     Responses:
         200: OK - ModelsRecentPlayerQueryResponse (OK)
 
         400: Bad Request - ResponseError (Bad Request)
 
         401: Unauthorized - ResponseError (Unauthorized)
 
@@ -79,24 +187,22 @@
     """
     if namespace is None:
         namespace, error = get_services_namespace()
         if error:
             return None, error
     request = PublicGetRecentPlayer.create(
         limit=limit,
-        user_id=user_id,
         namespace=namespace,
     )
     return run_request(request, additional_headers=x_additional_headers, **kwargs)
 
 
 @same_doc_as(PublicGetRecentPlayer)
 async def public_get_recent_player_async(
     limit: Optional[int] = None,
-    user_id: Optional[str] = None,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Query recent player with given user id. (publicGetRecentPlayer)
 
     Query recent player with given user id.
@@ -114,16 +220,14 @@
 
         securities: [BEARER_AUTH]
 
         namespace: (namespace) REQUIRED str in path
 
         limit: (limit) OPTIONAL int in query
 
-        user_id: (userId) OPTIONAL str in query
-
     Responses:
         200: OK - ModelsRecentPlayerQueryResponse (OK)
 
         400: Bad Request - ResponseError (Bad Request)
 
         401: Unauthorized - ResponseError (Unauthorized)
 
@@ -133,13 +237,12 @@
     """
     if namespace is None:
         namespace, error = get_services_namespace()
         if error:
             return None, error
     request = PublicGetRecentPlayer.create(
         limit=limit,
-        user_id=user_id,
         namespace=namespace,
     )
     return await run_request_async(
         request, additional_headers=x_additional_headers, **kwargs
     )
```

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk/api/session/wrappers/_session_storage.py` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk/api/session/wrappers/_session_storage.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk_service_session.egg-info/PKG-INFO` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk_service_session.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: accelbyte-py-sdk-service-session
-Version: 0.8.0
+Version: 0.9.0
 Summary: AccelByte Python SDK - AccelByte Gaming Services Session Service
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: accelbyte-py-sdk-core
 
 [//]: # (Code generated. DO NOT EDIT!)
 
 # AccelByte Modular Python SDK - Service Module
 
 This is a service module for the [AccelByte Modular Python SDK](https://github.com/AccelByte/accelbyte-python-modular-sdk) package.
 
 ```text
 AccelByte Gaming Services Session Service
-* Version: 3.13.14
+* Version: 3.14.0
 ```
 
 ## Setup
 
 This SDK requires Python 3.9 to be installed.
 
 ### Install with Pip
```

### Comparing `accelbyte-py-sdk-service-session-0.8.0/accelbyte_py_sdk_service_session.egg-info/SOURCES.txt` & `accelbyte-py-sdk-service-session-0.9.0/accelbyte_py_sdk_service_session.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -142,14 +142,15 @@
 accelbyte_py_sdk/api/session/operations/player/admin_get_player_attributes.py
 accelbyte_py_sdk/api/session/operations/player/admin_query_player_attributes.py
 accelbyte_py_sdk/api/session/operations/player/public_delete_player_at_57835b.py
 accelbyte_py_sdk/api/session/operations/player/public_get_bulk_player__da8481.py
 accelbyte_py_sdk/api/session/operations/player/public_get_player_attributes.py
 accelbyte_py_sdk/api/session/operations/player/public_store_player_attributes.py
 accelbyte_py_sdk/api/session/operations/recent_player/__init__.py
+accelbyte_py_sdk/api/session/operations/recent_player/admin_get_recent_player.py
 accelbyte_py_sdk/api/session/operations/recent_player/public_get_recent_player.py
 accelbyte_py_sdk/api/session/operations/session_storage/__init__.py
 accelbyte_py_sdk/api/session/operations/session_storage/admin_delete_user_sessi_e92b87.py
 accelbyte_py_sdk/api/session/operations/session_storage/admin_read_session_storage.py
 accelbyte_py_sdk/api/session/operations/session_storage/admin_read_user_session_f101bc.py
 accelbyte_py_sdk/api/session/operations/session_storage/public_update_insert_se_4c0538.py
 accelbyte_py_sdk/api/session/operations/session_storage/public_update_insert_se_f96597.py
```

