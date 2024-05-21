# Comparing `tmp/accelbyte-py-sdk-service-leaderboard-0.8.0.tar.gz` & `tmp/accelbyte-py-sdk-service-leaderboard-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accelbyte-py-sdk-service-leaderboard-0.8.0.tar", last modified: Wed Mar 13 06:12:41 2024, max compression
+gzip compressed data, was "accelbyte-py-sdk-service-leaderboard-0.9.0.tar", last modified: Tue Mar 26 05:42:53 2024, max compression
```

## Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0.tar` & `accelbyte-py-sdk-service-leaderboard-0.9.0.tar`

### file list

```diff
@@ -1,155 +1,155 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:12:41.042680 accelbyte-py-sdk-service-leaderboard-0.8.0/
--rw-r--r--   0 root         (0) root         (0)     1141 2024-03-13 06:12:41.042680 accelbyte-py-sdk-service-leaderboard-0.8.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      881 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:12:41.030680 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:12:41.030680 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:12:41.030680 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/
--rw-rw-r--   0 root         (0) root         (0)     8443 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:12:41.034680 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/
--rw-rw-r--   0 root         (0) root         (0)     4146 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5268 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/models_archive_leaderboard_req.py
--rw-rw-r--   0 root         (0) root         (0)     4768 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/models_archive_leaderboard_signed_url_response.py
--rw-rw-r--   0 root         (0) root         (0)     3881 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/models_bulk_user_i_ds_request.py
--rw-rw-r--   0 root         (0) root         (0)     4308 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/models_bulk_user_ranking_response_v3.py
--rw-rw-r--   0 root         (0) root         (0)     3770 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/models_daily_config.py
--rw-rw-r--   0 root         (0) root         (0)     4760 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/models_delete_bulk_leaderboard_failed_resp.py
--rw-rw-r--   0 root         (0) root         (0)     4165 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/models_delete_bulk_leaderboards_req.py
--rw-rw-r--   0 root         (0) root         (0)     4438 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/models_delete_bulk_leaderboards_resp.py
--rw-rw-r--   0 root         (0) root         (0)     5406 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/models_get_all_leaderboard_configs_public_resp.py
--rw-rw-r--   0 root         (0) root         (0)     5465 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/models_get_all_leaderboard_configs_public_resp_v3.py
--rw-rw-r--   0 root         (0) root         (0)     5281 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/models_get_all_leaderboard_configs_resp.py
--rw-rw-r--   0 root         (0) root         (0)     5349 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/models_get_all_leaderboard_configs_resp_v3.py
--rw-rw-r--   0 root         (0) root         (0)     5228 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/models_get_all_user_leaderboards_resp.py
--rw-rw-r--   0 root         (0) root         (0)     5301 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/models_get_all_user_leaderboards_resp_v3.py
--rw-rw-r--   0 root         (0) root         (0)     4729 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/models_get_hidden_user_response.py
--rw-rw-r--   0 root         (0) root         (0)     6040 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/models_get_leaderboard_config_public_resp.py
--rw-rw-r--   0 root         (0) root         (0)     7550 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/models_get_leaderboard_config_public_resp_v3.py
--rw-rw-r--   0 root         (0) root         (0)    13069 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/models_get_leaderboard_config_resp.py
--rw-rw-r--   0 root         (0) root         (0)    11837 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/models_get_leaderboard_config_resp_v3.py
--rw-rw-r--   0 root         (0) root         (0)     5060 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/models_get_leaderboard_ranking_resp.py
--rw-rw-r--   0 root         (0) root         (0)     5281 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/models_get_user_visibility_response.py
--rw-rw-r--   0 root         (0) root         (0)    10788 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/models_leaderboard_config_req.py
--rw-rw-r--   0 root         (0) root         (0)     8963 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/models_leaderboard_config_req_v3.py
--rw-rw-r--   0 root         (0) root         (0)     4466 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/models_monthly_config.py
--rw-rw-r--   0 root         (0) root         (0)     5440 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/models_pagination.py
--rw-rw-r--   0 root         (0) root         (0)     5483 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/models_pagination_v3.py
--rw-rw-r--   0 root         (0) root         (0)     3952 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/models_set_user_visibility_request.py
--rw-rw-r--   0 root         (0) root         (0)    10120 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/models_update_leaderboard_config_req.py
--rw-rw-r--   0 root         (0) root         (0)     7574 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/models_update_leaderboard_config_req_v3.py
--rw-rw-r--   0 root         (0) root         (0)     4631 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/models_update_user_point_admin_v1_request.py
--rw-rw-r--   0 root         (0) root         (0)     4569 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/models_update_user_point_admin_v1_response.py
--rw-rw-r--   0 root         (0) root         (0)     6937 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/models_user_cycle_ranking_response_detail.py
--rw-rw-r--   0 root         (0) root         (0)    10373 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/models_user_leaderboard_ranking.py
--rw-rw-r--   0 root         (0) root         (0)     7842 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/models_user_leaderboard_ranking_v3.py
--rw-rw-r--   0 root         (0) root         (0)     5926 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/models_user_point.py
--rw-rw-r--   0 root         (0) root         (0)     8699 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/models_user_ranking_response.py
--rw-rw-r--   0 root         (0) root         (0)     6143 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/models_user_ranking_response_detail.py
--rw-rw-r--   0 root         (0) root         (0)     6234 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/models_user_ranking_response_detail_v3.py
--rw-rw-r--   0 root         (0) root         (0)     6173 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/models_user_ranking_response_v3.py
--rw-rw-r--   0 root         (0) root         (0)     4434 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/models_weekly_config.py
--rw-rw-r--   0 root         (0) root         (0)     4581 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/response_error_response.py
--rw-rw-r--   0 root         (0) root         (0)     5249 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/v2_entry.py
--rw-rw-r--   0 root         (0) root         (0)     5280 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/v2_get_all_leaderboard_configs_public_resp.py
--rw-rw-r--   0 root         (0) root         (0)     5984 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/v2_get_leaderboard_config_public_resp.py
--rw-rw-r--   0 root         (0) root         (0)     5026 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/v2_get_public_leaderboard_ranking_response.py
--rw-rw-r--   0 root         (0) root         (0)     5370 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/v2_pagination.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:12:41.034680 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/
--rw-rw-r--   0 root         (0) root         (0)      440 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:12:41.034680 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/anonymization/
--rw-rw-r--   0 root         (0) root         (0)      554 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/anonymization/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7155 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/anonymization/admin_anonymize_user_le_6fbe1f.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:12:41.034680 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration/
--rw-rw-r--   0 root         (0) root         (0)     1282 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     9165 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration/create_leaderboard_conf_663810.py
--rw-rw-r--   0 root         (0) root         (0)     9226 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration/create_leaderboard_conf_8287f9.py
--rw-rw-r--   0 root         (0) root         (0)     8173 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration/delete_bulk_leaderboard_94414e.py
--rw-rw-r--   0 root         (0) root         (0)     7886 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration/delete_leaderboard_conf_e6fbfe.py
--rw-rw-r--   0 root         (0) root         (0)    10346 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration/get_leaderboard_configu_3c85d9.py
--rw-rw-r--   0 root         (0) root         (0)     8542 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration/get_leaderboard_configu_d8a38d.py
--rw-rw-r--   0 root         (0) root         (0)     8063 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration/get_leaderboard_configu_dfbf1e.py
--rw-rw-r--   0 root         (0) root         (0)    10436 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration/get_leaderboard_configu_e27832.py
--rw-rw-r--   0 root         (0) root         (0)     8068 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration/hard_delete_leaderboard_e07e01.py
--rw-rw-r--   0 root         (0) root         (0)    10479 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration/update_leaderboard_conf_ca626e.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:12:41.034680 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration_v3/
--rw-rw-r--   0 root         (0) root         (0)     1198 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration_v3/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     9362 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration_v3/create_leaderboard_conf_2ad364.py
--rw-rw-r--   0 root         (0) root         (0)     8173 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration_v3/delete_bulk_leaderboard_f7002d.py
--rw-rw-r--   0 root         (0) root         (0)     7914 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration_v3/delete_leaderboard_conf_8f143c.py
--rw-rw-r--   0 root         (0) root         (0)     8162 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration_v3/get_leaderboard_configu_290af8.py
--rw-rw-r--   0 root         (0) root         (0)     8075 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration_v3/get_leaderboard_configu_33150a.py
--rw-rw-r--   0 root         (0) root         (0)     9432 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration_v3/get_leaderboard_configu_9b2b53.py
--rw-rw-r--   0 root         (0) root         (0)     9523 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration_v3/get_leaderboard_configu_b16dd3.py
--rw-rw-r--   0 root         (0) root         (0)     8096 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration_v3/hard_delete_leaderboard_c58ff0.py
--rw-rw-r--   0 root         (0) root         (0)    10833 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration_v3/update_leaderboard_conf_1b8e6b.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:12:41.038680 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/
--rw-rw-r--   0 root         (0) root         (0)     2150 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     9397 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/admin_get_archived_lead_191726.py
--rw-rw-r--   0 root         (0) root         (0)     8219 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/create_archived_leaderb_5492e4.py
--rw-rw-r--   0 root         (0) root         (0)     8618 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/delete_user_ranking_admin_v1.py
--rw-rw-r--   0 root         (0) root         (0)     7822 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/delete_user_ranking_by__ed6de1.py
--rw-rw-r--   0 root         (0) root         (0)     8627 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/delete_user_ranking_public_v1.py
--rw-rw-r--   0 root         (0) root         (0)     8403 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/delete_user_rankings_admin_v1.py
--rw-rw-r--   0 root         (0) root         (0)     9488 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/get_all_time_leaderboar_358b23.py
--rw-rw-r--   0 root         (0) root         (0)     9850 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/get_all_time_leaderboar_9cbcdd.py
--rw-rw-r--   0 root         (0) root         (0)     9982 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/get_all_time_leaderboar_d0fb4b.py
--rw-rw-r--   0 root         (0) root         (0)    10368 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/get_archived_leaderboar_c023ea.py
--rw-rw-r--   0 root         (0) root         (0)    11093 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/get_current_month_leade_26486d.py
--rw-rw-r--   0 root         (0) root         (0)    10584 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/get_current_month_leade_4373db.py
--rw-rw-r--   0 root         (0) root         (0)    10599 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/get_current_season_lead_51d992.py
--rw-rw-r--   0 root         (0) root         (0)    11108 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/get_current_season_lead_a79ffc.py
--rw-rw-r--   0 root         (0) root         (0)    10569 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/get_current_week_leader_07d571.py
--rw-rw-r--   0 root         (0) root         (0)    11078 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/get_current_week_leader_bdd5ce.py
--rw-rw-r--   0 root         (0) root         (0)    10970 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/get_today_leaderboard_r_2eefd7.py
--rw-rw-r--   0 root         (0) root         (0)    10461 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/get_today_leaderboard_r_51cbb5.py
--rw-rw-r--   0 root         (0) root         (0)     9819 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/get_user_ranking_admin_v1.py
--rw-rw-r--   0 root         (0) root         (0)     9829 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/get_user_ranking_public_v1.py
--rw-rw-r--   0 root         (0) root         (0)    10192 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/update_user_point_admin_v1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:12:41.038680 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data_v3/
--rw-rw-r--   0 root         (0) root         (0)     1223 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data_v3/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     9316 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data_v3/bulk_get_users_ranking__e7e5b3.py
--rw-rw-r--   0 root         (0) root         (0)     8620 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data_v3/delete_user_ranking_admin_v3.py
--rw-rw-r--   0 root         (0) root         (0)     7860 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data_v3/delete_user_ranking_by__c762e5.py
--rw-rw-r--   0 root         (0) root         (0)     8405 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data_v3/delete_user_rankings_admin_v3.py
--rw-rw-r--   0 root         (0) root         (0)     9988 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data_v3/get_all_time_leaderboar_489ddb.py
--rw-rw-r--   0 root         (0) root         (0)     9480 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data_v3/get_all_time_leaderboar_5b0d52.py
--rw-rw-r--   0 root         (0) root         (0)    10333 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data_v3/get_current_cycle_leade_2c20ce.py
--rw-rw-r--   0 root         (0) root         (0)    10840 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data_v3/get_current_cycle_leade_f8a4d7.py
--rw-rw-r--   0 root         (0) root         (0)     8516 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data_v3/get_user_ranking_admin_v3.py
--rw-rw-r--   0 root         (0) root         (0)     8525 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data_v3/get_user_ranking_public_v3.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:12:41.038680 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/user_data/
--rw-rw-r--   0 root         (0) root         (0)      551 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/user_data/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    10024 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/user_data/get_user_leaderboard_ra_d2aae2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:12:41.038680 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/user_data_v3/
--rw-rw-r--   0 root         (0) root         (0)      551 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/user_data_v3/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     9003 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/user_data_v3/get_user_leaderboard_ra_e5b21a.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:12:41.038680 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/user_visibility/
--rw-rw-r--   0 root         (0) root         (0)      742 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/user_visibility/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     9412 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/user_visibility/get_hidden_users_v2.py
--rw-rw-r--   0 root         (0) root         (0)     8558 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/user_visibility/get_user_visibility_status_v2.py
--rw-rw-r--   0 root         (0) root         (0)    10089 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/user_visibility/set_user_leaderboard_vi_7b0546.py
--rw-rw-r--   0 root         (0) root         (0)     8899 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/user_visibility/set_user_visibility_status_v2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:12:41.038680 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/user_visibility_v3/
--rw-rw-r--   0 root         (0) root         (0)      723 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/user_visibility_v3/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     9362 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/user_visibility_v3/get_hidden_users_v3.py
--rw-rw-r--   0 root         (0) root         (0)     8574 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/user_visibility_v3/get_user_visibility_status_v3.py
--rw-rw-r--   0 root         (0) root         (0)    10043 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/user_visibility_v3/set_user_leaderboard_vi_da19f8.py
--rw-rw-r--   0 root         (0) root         (0)     8921 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/user_visibility_v3/set_user_visibility_v3.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:12:41.042680 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/wrappers/
--rw-rw-r--   0 root         (0) root         (0)     9867 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/wrappers/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4072 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/wrappers/_anonymization.py
--rw-rw-r--   0 root         (0) root         (0)    42098 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/wrappers/_leaderboard_configuration.py
--rw-rw-r--   0 root         (0) root         (0)    37127 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/wrappers/_leaderboard_configuration_v3.py
--rw-rw-r--   0 root         (0) root         (0)    83583 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/wrappers/_leaderboard_data.py
--rw-rw-r--   0 root         (0) root         (0)    37871 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/wrappers/_leaderboard_data_v3.py
--rw-rw-r--   0 root         (0) root         (0)     4731 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/wrappers/_user_data.py
--rw-rw-r--   0 root         (0) root         (0)     4436 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/wrappers/_user_data_v3.py
--rw-rw-r--   0 root         (0) root         (0)    15670 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/wrappers/_user_visibility.py
--rw-rw-r--   0 root         (0) root         (0)    15624 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/wrappers/_user_visibility_v3.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:12:41.042680 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk_service_leaderboard.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1141 2024-03-13 06:12:41.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk_service_leaderboard.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11285 2024-03-13 06:12:41.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk_service_leaderboard.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-13 06:12:41.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk_service_leaderboard.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-13 06:12:41.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk_service_leaderboard.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-03-13 06:12:41.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk_service_leaderboard.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)      367 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-leaderboard-0.8.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-13 06:12:41.042680 accelbyte-py-sdk-service-leaderboard-0.8.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:42:53.178462 accelbyte-py-sdk-service-leaderboard-0.9.0/
+-rw-r--r--   0 root         (0) root         (0)     1141 2024-03-26 05:42:53.178462 accelbyte-py-sdk-service-leaderboard-0.9.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      881 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:42:53.162462 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:42:53.162462 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:42:53.166462 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/
+-rw-rw-r--   0 root         (0) root         (0)     8443 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:42:53.170462 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/
+-rw-rw-r--   0 root         (0) root         (0)     4146 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     5268 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/models_archive_leaderboard_req.py
+-rw-rw-r--   0 root         (0) root         (0)     4768 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/models_archive_leaderboard_signed_url_response.py
+-rw-rw-r--   0 root         (0) root         (0)     3881 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/models_bulk_user_i_ds_request.py
+-rw-rw-r--   0 root         (0) root         (0)     4308 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/models_bulk_user_ranking_response_v3.py
+-rw-rw-r--   0 root         (0) root         (0)     3770 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/models_daily_config.py
+-rw-rw-r--   0 root         (0) root         (0)     4760 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/models_delete_bulk_leaderboard_failed_resp.py
+-rw-rw-r--   0 root         (0) root         (0)     4165 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/models_delete_bulk_leaderboards_req.py
+-rw-rw-r--   0 root         (0) root         (0)     4438 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/models_delete_bulk_leaderboards_resp.py
+-rw-rw-r--   0 root         (0) root         (0)     5406 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/models_get_all_leaderboard_configs_public_resp.py
+-rw-rw-r--   0 root         (0) root         (0)     5465 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/models_get_all_leaderboard_configs_public_resp_v3.py
+-rw-rw-r--   0 root         (0) root         (0)     5281 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/models_get_all_leaderboard_configs_resp.py
+-rw-rw-r--   0 root         (0) root         (0)     5349 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/models_get_all_leaderboard_configs_resp_v3.py
+-rw-rw-r--   0 root         (0) root         (0)     5228 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/models_get_all_user_leaderboards_resp.py
+-rw-rw-r--   0 root         (0) root         (0)     5301 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/models_get_all_user_leaderboards_resp_v3.py
+-rw-rw-r--   0 root         (0) root         (0)     4729 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/models_get_hidden_user_response.py
+-rw-rw-r--   0 root         (0) root         (0)     6040 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/models_get_leaderboard_config_public_resp.py
+-rw-rw-r--   0 root         (0) root         (0)     7550 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/models_get_leaderboard_config_public_resp_v3.py
+-rw-rw-r--   0 root         (0) root         (0)    13069 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/models_get_leaderboard_config_resp.py
+-rw-rw-r--   0 root         (0) root         (0)    11837 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/models_get_leaderboard_config_resp_v3.py
+-rw-rw-r--   0 root         (0) root         (0)     5060 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/models_get_leaderboard_ranking_resp.py
+-rw-rw-r--   0 root         (0) root         (0)     5281 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/models_get_user_visibility_response.py
+-rw-rw-r--   0 root         (0) root         (0)    10788 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/models_leaderboard_config_req.py
+-rw-rw-r--   0 root         (0) root         (0)     8963 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/models_leaderboard_config_req_v3.py
+-rw-rw-r--   0 root         (0) root         (0)     4466 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/models_monthly_config.py
+-rw-rw-r--   0 root         (0) root         (0)     5440 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/models_pagination.py
+-rw-rw-r--   0 root         (0) root         (0)     5483 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/models_pagination_v3.py
+-rw-rw-r--   0 root         (0) root         (0)     3952 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/models_set_user_visibility_request.py
+-rw-rw-r--   0 root         (0) root         (0)    10120 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/models_update_leaderboard_config_req.py
+-rw-rw-r--   0 root         (0) root         (0)     7574 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/models_update_leaderboard_config_req_v3.py
+-rw-rw-r--   0 root         (0) root         (0)     4631 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/models_update_user_point_admin_v1_request.py
+-rw-rw-r--   0 root         (0) root         (0)     4569 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/models_update_user_point_admin_v1_response.py
+-rw-rw-r--   0 root         (0) root         (0)     6937 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/models_user_cycle_ranking_response_detail.py
+-rw-rw-r--   0 root         (0) root         (0)    10373 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/models_user_leaderboard_ranking.py
+-rw-rw-r--   0 root         (0) root         (0)     7842 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/models_user_leaderboard_ranking_v3.py
+-rw-rw-r--   0 root         (0) root         (0)     5926 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/models_user_point.py
+-rw-rw-r--   0 root         (0) root         (0)     8699 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/models_user_ranking_response.py
+-rw-rw-r--   0 root         (0) root         (0)     6143 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/models_user_ranking_response_detail.py
+-rw-rw-r--   0 root         (0) root         (0)     6234 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/models_user_ranking_response_detail_v3.py
+-rw-rw-r--   0 root         (0) root         (0)     6173 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/models_user_ranking_response_v3.py
+-rw-rw-r--   0 root         (0) root         (0)     4434 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/models_weekly_config.py
+-rw-rw-r--   0 root         (0) root         (0)     4581 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/response_error_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5249 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/v2_entry.py
+-rw-rw-r--   0 root         (0) root         (0)     5280 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/v2_get_all_leaderboard_configs_public_resp.py
+-rw-rw-r--   0 root         (0) root         (0)     5984 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/v2_get_leaderboard_config_public_resp.py
+-rw-rw-r--   0 root         (0) root         (0)     5026 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/v2_get_public_leaderboard_ranking_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5370 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/v2_pagination.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:42:53.170462 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/
+-rw-rw-r--   0 root         (0) root         (0)      440 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:42:53.170462 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/anonymization/
+-rw-rw-r--   0 root         (0) root         (0)      554 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/anonymization/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7155 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/anonymization/admin_anonymize_user_le_6fbe1f.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:42:53.170462 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration/
+-rw-rw-r--   0 root         (0) root         (0)     1282 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     9165 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration/create_leaderboard_conf_663810.py
+-rw-rw-r--   0 root         (0) root         (0)     9226 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration/create_leaderboard_conf_8287f9.py
+-rw-rw-r--   0 root         (0) root         (0)     8173 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration/delete_bulk_leaderboard_94414e.py
+-rw-rw-r--   0 root         (0) root         (0)     7886 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration/delete_leaderboard_conf_e6fbfe.py
+-rw-rw-r--   0 root         (0) root         (0)    10346 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration/get_leaderboard_configu_3c85d9.py
+-rw-rw-r--   0 root         (0) root         (0)     8542 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration/get_leaderboard_configu_d8a38d.py
+-rw-rw-r--   0 root         (0) root         (0)     8063 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration/get_leaderboard_configu_dfbf1e.py
+-rw-rw-r--   0 root         (0) root         (0)    10436 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration/get_leaderboard_configu_e27832.py
+-rw-rw-r--   0 root         (0) root         (0)     8195 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration/hard_delete_leaderboard_e07e01.py
+-rw-rw-r--   0 root         (0) root         (0)    10479 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration/update_leaderboard_conf_ca626e.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:42:53.170462 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration_v3/
+-rw-rw-r--   0 root         (0) root         (0)     1198 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration_v3/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     9362 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration_v3/create_leaderboard_conf_2ad364.py
+-rw-rw-r--   0 root         (0) root         (0)     8173 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration_v3/delete_bulk_leaderboard_f7002d.py
+-rw-rw-r--   0 root         (0) root         (0)     7914 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration_v3/delete_leaderboard_conf_8f143c.py
+-rw-rw-r--   0 root         (0) root         (0)     8162 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration_v3/get_leaderboard_configu_290af8.py
+-rw-rw-r--   0 root         (0) root         (0)     8075 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration_v3/get_leaderboard_configu_33150a.py
+-rw-rw-r--   0 root         (0) root         (0)     9432 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration_v3/get_leaderboard_configu_9b2b53.py
+-rw-rw-r--   0 root         (0) root         (0)     9523 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration_v3/get_leaderboard_configu_b16dd3.py
+-rw-rw-r--   0 root         (0) root         (0)     8223 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration_v3/hard_delete_leaderboard_c58ff0.py
+-rw-rw-r--   0 root         (0) root         (0)    10833 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration_v3/update_leaderboard_conf_1b8e6b.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:42:53.174462 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/
+-rw-rw-r--   0 root         (0) root         (0)     2150 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     9397 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/admin_get_archived_lead_191726.py
+-rw-rw-r--   0 root         (0) root         (0)     8219 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/create_archived_leaderb_5492e4.py
+-rw-rw-r--   0 root         (0) root         (0)     8618 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/delete_user_ranking_admin_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     7822 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/delete_user_ranking_by__ed6de1.py
+-rw-rw-r--   0 root         (0) root         (0)     8627 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/delete_user_ranking_public_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     8403 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/delete_user_rankings_admin_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     9488 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/get_all_time_leaderboar_358b23.py
+-rw-rw-r--   0 root         (0) root         (0)     9850 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/get_all_time_leaderboar_9cbcdd.py
+-rw-rw-r--   0 root         (0) root         (0)     9982 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/get_all_time_leaderboar_d0fb4b.py
+-rw-rw-r--   0 root         (0) root         (0)    10368 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/get_archived_leaderboar_c023ea.py
+-rw-rw-r--   0 root         (0) root         (0)    11093 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/get_current_month_leade_26486d.py
+-rw-rw-r--   0 root         (0) root         (0)    10584 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/get_current_month_leade_4373db.py
+-rw-rw-r--   0 root         (0) root         (0)    10599 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/get_current_season_lead_51d992.py
+-rw-rw-r--   0 root         (0) root         (0)    11108 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/get_current_season_lead_a79ffc.py
+-rw-rw-r--   0 root         (0) root         (0)    10569 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/get_current_week_leader_07d571.py
+-rw-rw-r--   0 root         (0) root         (0)    11078 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/get_current_week_leader_bdd5ce.py
+-rw-rw-r--   0 root         (0) root         (0)    10970 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/get_today_leaderboard_r_2eefd7.py
+-rw-rw-r--   0 root         (0) root         (0)    10461 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/get_today_leaderboard_r_51cbb5.py
+-rw-rw-r--   0 root         (0) root         (0)     9819 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/get_user_ranking_admin_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     9829 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/get_user_ranking_public_v1.py
+-rw-rw-r--   0 root         (0) root         (0)    10192 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/update_user_point_admin_v1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:42:53.174462 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data_v3/
+-rw-rw-r--   0 root         (0) root         (0)     1223 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data_v3/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     9316 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data_v3/bulk_get_users_ranking__e7e5b3.py
+-rw-rw-r--   0 root         (0) root         (0)     8620 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data_v3/delete_user_ranking_admin_v3.py
+-rw-rw-r--   0 root         (0) root         (0)     7860 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data_v3/delete_user_ranking_by__c762e5.py
+-rw-rw-r--   0 root         (0) root         (0)     8405 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data_v3/delete_user_rankings_admin_v3.py
+-rw-rw-r--   0 root         (0) root         (0)     9988 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data_v3/get_all_time_leaderboar_489ddb.py
+-rw-rw-r--   0 root         (0) root         (0)     9480 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data_v3/get_all_time_leaderboar_5b0d52.py
+-rw-rw-r--   0 root         (0) root         (0)    10333 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data_v3/get_current_cycle_leade_2c20ce.py
+-rw-rw-r--   0 root         (0) root         (0)    10840 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data_v3/get_current_cycle_leade_f8a4d7.py
+-rw-rw-r--   0 root         (0) root         (0)     8516 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data_v3/get_user_ranking_admin_v3.py
+-rw-rw-r--   0 root         (0) root         (0)     8525 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data_v3/get_user_ranking_public_v3.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:42:53.174462 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/user_data/
+-rw-rw-r--   0 root         (0) root         (0)      551 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/user_data/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    10024 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/user_data/get_user_leaderboard_ra_d2aae2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:42:53.174462 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/user_data_v3/
+-rw-rw-r--   0 root         (0) root         (0)      551 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/user_data_v3/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     9003 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/user_data_v3/get_user_leaderboard_ra_e5b21a.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:42:53.174462 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/user_visibility/
+-rw-rw-r--   0 root         (0) root         (0)      742 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/user_visibility/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     9412 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/user_visibility/get_hidden_users_v2.py
+-rw-rw-r--   0 root         (0) root         (0)     8558 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/user_visibility/get_user_visibility_status_v2.py
+-rw-rw-r--   0 root         (0) root         (0)    10089 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/user_visibility/set_user_leaderboard_vi_7b0546.py
+-rw-rw-r--   0 root         (0) root         (0)     8899 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/user_visibility/set_user_visibility_status_v2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:42:53.174462 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/user_visibility_v3/
+-rw-rw-r--   0 root         (0) root         (0)      723 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/user_visibility_v3/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     9362 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/user_visibility_v3/get_hidden_users_v3.py
+-rw-rw-r--   0 root         (0) root         (0)     8574 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/user_visibility_v3/get_user_visibility_status_v3.py
+-rw-rw-r--   0 root         (0) root         (0)    10043 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/user_visibility_v3/set_user_leaderboard_vi_da19f8.py
+-rw-rw-r--   0 root         (0) root         (0)     8921 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/user_visibility_v3/set_user_visibility_v3.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:42:53.178462 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/wrappers/
+-rw-rw-r--   0 root         (0) root         (0)     9867 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/wrappers/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4072 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/wrappers/_anonymization.py
+-rw-rw-r--   0 root         (0) root         (0)    42414 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/wrappers/_leaderboard_configuration.py
+-rw-rw-r--   0 root         (0) root         (0)    37443 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/wrappers/_leaderboard_configuration_v3.py
+-rw-rw-r--   0 root         (0) root         (0)    83583 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/wrappers/_leaderboard_data.py
+-rw-rw-r--   0 root         (0) root         (0)    37871 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/wrappers/_leaderboard_data_v3.py
+-rw-rw-r--   0 root         (0) root         (0)     4731 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/wrappers/_user_data.py
+-rw-rw-r--   0 root         (0) root         (0)     4436 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/wrappers/_user_data_v3.py
+-rw-rw-r--   0 root         (0) root         (0)    15670 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/wrappers/_user_visibility.py
+-rw-rw-r--   0 root         (0) root         (0)    15624 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/wrappers/_user_visibility_v3.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:42:53.178462 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk_service_leaderboard.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1141 2024-03-26 05:42:53.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk_service_leaderboard.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11285 2024-03-26 05:42:53.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk_service_leaderboard.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-03-26 05:42:53.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk_service_leaderboard.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 05:42:53.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk_service_leaderboard.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-03-26 05:42:53.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk_service_leaderboard.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)      367 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-leaderboard-0.9.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-03-26 05:42:53.178462 accelbyte-py-sdk-service-leaderboard-0.9.0/setup.cfg
```

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/PKG-INFO` & `accelbyte-py-sdk-service-leaderboard-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: accelbyte-py-sdk-service-leaderboard
-Version: 0.8.0
+Version: 0.9.0
 Summary: AccelByte Python SDK - AccelByte Gaming Services Leaderboard Service
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: accelbyte-py-sdk-core
 
 [//]: # (Code generated. DO NOT EDIT!)
 
 # AccelByte Modular Python SDK - Service Module
 
 This is a service module for the [AccelByte Modular Python SDK](https://github.com/AccelByte/accelbyte-python-modular-sdk) package.
 
 ```text
 AccelByte Gaming Services Leaderboard Service
-* Version: 2.28.0
+* Version: 2.29.0
 ```
 
 ## Setup
 
 This SDK requires Python 3.9 to be installed.
 
 ### Install with Pip
```

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/README.md` & `accelbyte-py-sdk-service-leaderboard-0.9.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # AccelByte Modular Python SDK - Service Module
 
 This is a service module for the [AccelByte Modular Python SDK](https://github.com/AccelByte/accelbyte-python-modular-sdk) package.
 
 ```text
 AccelByte Gaming Services Leaderboard Service
-* Version: 2.28.0
+* Version: 2.29.0
 ```
 
 ## Setup
 
 This SDK requires Python 3.9 to be installed.
 
 ### Install with Pip
```

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/__init__.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: service-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Leaderboard Service."""
 
-__version__ = "2.28.0"
+__version__ = "2.29.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 # anonymization
 from .wrappers import admin_anonymize_user_leaderboard_admin_v1
```

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/__init__.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: model-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Leaderboard Service."""
 
-__version__ = "2.28.0"
+__version__ = "2.29.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .models_archive_leaderboard_req import ModelsArchiveLeaderboardReq
 from .models_archive_leaderboard_signed_url_response import (
```

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/models_archive_leaderboard_req.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/models_archive_leaderboard_req.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/models_archive_leaderboard_signed_url_response.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/models_archive_leaderboard_signed_url_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/models_bulk_user_i_ds_request.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/models_bulk_user_i_ds_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/models_bulk_user_ranking_response_v3.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/models_bulk_user_ranking_response_v3.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/models_daily_config.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/models_daily_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/models_delete_bulk_leaderboard_failed_resp.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/models_delete_bulk_leaderboard_failed_resp.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/models_delete_bulk_leaderboards_req.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/models_delete_bulk_leaderboards_req.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/models_delete_bulk_leaderboards_resp.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/models_delete_bulk_leaderboards_resp.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/models_get_all_leaderboard_configs_public_resp.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/models_get_all_leaderboard_configs_public_resp.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/models_get_all_leaderboard_configs_public_resp_v3.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/models_get_all_leaderboard_configs_public_resp_v3.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/models_get_all_leaderboard_configs_resp.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/models_get_all_leaderboard_configs_resp.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/models_get_all_leaderboard_configs_resp_v3.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/models_get_all_leaderboard_configs_resp_v3.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/models_get_all_user_leaderboards_resp.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/models_get_all_user_leaderboards_resp.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/models_get_all_user_leaderboards_resp_v3.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/models_get_all_user_leaderboards_resp_v3.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/models_get_hidden_user_response.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/models_get_hidden_user_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/models_get_leaderboard_config_public_resp.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/models_get_leaderboard_config_public_resp.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/models_get_leaderboard_config_public_resp_v3.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/models_get_leaderboard_config_public_resp_v3.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/models_get_leaderboard_config_resp.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/models_get_leaderboard_config_resp.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/models_get_leaderboard_config_resp_v3.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/models_get_leaderboard_config_resp_v3.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/models_get_leaderboard_ranking_resp.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/models_get_leaderboard_ranking_resp.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/models_get_user_visibility_response.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/models_get_user_visibility_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/models_leaderboard_config_req.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/models_leaderboard_config_req.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/models_leaderboard_config_req_v3.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/models_leaderboard_config_req_v3.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/models_monthly_config.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/models_monthly_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/models_pagination.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/models_pagination.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/models_pagination_v3.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/models_pagination_v3.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/models_set_user_visibility_request.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/models_set_user_visibility_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/models_update_leaderboard_config_req.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/models_update_leaderboard_config_req.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/models_update_leaderboard_config_req_v3.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/models_update_leaderboard_config_req_v3.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/models_update_user_point_admin_v1_request.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/models_update_user_point_admin_v1_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/models_update_user_point_admin_v1_response.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/models_update_user_point_admin_v1_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/models_user_cycle_ranking_response_detail.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/models_user_cycle_ranking_response_detail.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/models_user_leaderboard_ranking.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/models_user_leaderboard_ranking.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/models_user_leaderboard_ranking_v3.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/models_user_leaderboard_ranking_v3.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/models_user_point.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/models_user_point.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/models_user_ranking_response.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/models_user_ranking_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/models_user_ranking_response_detail.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/models_user_ranking_response_detail.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/models_user_ranking_response_detail_v3.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/models_user_ranking_response_detail_v3.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/models_user_ranking_response_v3.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/models_user_ranking_response_v3.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/models_weekly_config.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/models_weekly_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/response_error_response.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/response_error_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/v2_entry.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/v2_entry.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/v2_get_all_leaderboard_configs_public_resp.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/v2_get_all_leaderboard_configs_public_resp.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/v2_get_leaderboard_config_public_resp.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/v2_get_leaderboard_config_public_resp.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/v2_get_public_leaderboard_ranking_response.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/v2_get_public_leaderboard_ranking_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/models/v2_pagination.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/models/v2_pagination.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/anonymization/__init__.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/anonymization/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,14 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Leaderboard Service."""
 
-__version__ = "2.28.0"
+__version__ = "2.29.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .admin_anonymize_user_le_6fbe1f import AdminAnonymizeUserLeaderboardAdminV1
```

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/anonymization/admin_anonymize_user_le_6fbe1f.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/anonymization/admin_anonymize_user_le_6fbe1f.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration/__init__.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Leaderboard Service."""
 
-__version__ = "2.28.0"
+__version__ = "2.29.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .create_leaderboard_conf_663810 import CreateLeaderboardConfigurationAdminV1
 from .create_leaderboard_conf_8287f9 import CreateLeaderboardConfigurationPublicV1
```

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration/create_leaderboard_conf_663810.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration/create_leaderboard_conf_663810.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration/create_leaderboard_conf_8287f9.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration/create_leaderboard_conf_8287f9.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration/delete_bulk_leaderboard_94414e.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration/delete_bulk_leaderboard_94414e.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration/delete_leaderboard_conf_e6fbfe.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration/delete_leaderboard_conf_e6fbfe.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration/get_leaderboard_configu_3c85d9.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration/get_leaderboard_configu_3c85d9.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration/get_leaderboard_configu_d8a38d.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration/get_leaderboard_configu_d8a38d.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration/get_leaderboard_configu_dfbf1e.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration/get_leaderboard_configu_dfbf1e.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration/get_leaderboard_configu_e27832.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration/get_leaderboard_configu_e27832.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration/hard_delete_leaderboard_e07e01.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration_v3/delete_leaderboard_conf_8f143c.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,63 +28,55 @@
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
 from ...models import ResponseErrorResponse
 
 
-class HardDeleteLeaderboardAdminV1(Operation):
-    """hard delete leaderboard config and data by leaderboard code (hardDeleteLeaderboardAdminV1)
+class DeleteLeaderboardConfigurationAdminV3(Operation):
+    """delete leaderboard by leaderboardCode (deleteLeaderboardConfigurationAdminV3)
 
-    [Test Facility Only]
-
-
-
-
-    This endpoint will delete leaderboard configuration and its data
-
-
-
-
-    Note: this endpoint only works on development environment, you might want to use archive endpoint instead hard delete.
+    This endpoint delete a leaderboard configuration
 
     Properties:
-        url: /leaderboard/v1/admin/namespaces/{namespace}/leaderboards/{leaderboardCode}/hard
+        url: /leaderboard/v3/admin/namespaces/{namespace}/leaderboards/{leaderboardCode}
 
         method: DELETE
 
-        tags: ["LeaderboardConfiguration"]
+        tags: ["LeaderboardConfigurationV3"]
 
         consumes: []
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
         leaderboard_code: (leaderboardCode) REQUIRED str in path
 
         namespace: (namespace) REQUIRED str in path
 
     Responses:
-        204: No Content - (Leaderboard deleted)
+        204: No Content - (Leaderboard successfully deleted)
 
         400: Bad Request - ResponseErrorResponse (20002: validation error)
 
         401: Unauthorized - ResponseErrorResponse (20001: unauthorized access)
 
-        403: Forbidden - ResponseErrorResponse (20013: insufficient permissions | 71241: forbidden environment)
+        403: Forbidden - ResponseErrorResponse (20013: insufficient permissions)
 
         404: Not Found - ResponseErrorResponse (71130: leaderboard config not found)
 
         500: Internal Server Error - ResponseErrorResponse (20000: internal server error)
     """
 
     # region fields
 
-    _url: str = "/leaderboard/v1/admin/namespaces/{namespace}/leaderboards/{leaderboardCode}/hard"
+    _url: str = (
+        "/leaderboard/v3/admin/namespaces/{namespace}/leaderboards/{leaderboardCode}"
+    )
     _method: str = "DELETE"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
     leaderboard_code: str  # REQUIRED in [path]
@@ -143,19 +135,21 @@
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_leaderboard_code(self, value: str) -> HardDeleteLeaderboardAdminV1:
+    def with_leaderboard_code(
+        self, value: str
+    ) -> DeleteLeaderboardConfigurationAdminV3:
         self.leaderboard_code = value
         return self
 
-    def with_namespace(self, value: str) -> HardDeleteLeaderboardAdminV1:
+    def with_namespace(self, value: str) -> DeleteLeaderboardConfigurationAdminV3:
         self.namespace = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
@@ -177,21 +171,21 @@
 
     # noinspection PyMethodMayBeStatic
     def parse_response(
         self, code: int, content_type: str, content: Any
     ) -> Tuple[None, Union[None, HttpResponse, ResponseErrorResponse]]:
         """Parse the given response.
 
-        204: No Content - (Leaderboard deleted)
+        204: No Content - (Leaderboard successfully deleted)
 
         400: Bad Request - ResponseErrorResponse (20002: validation error)
 
         401: Unauthorized - ResponseErrorResponse (20001: unauthorized access)
 
-        403: Forbidden - ResponseErrorResponse (20013: insufficient permissions | 71241: forbidden environment)
+        403: Forbidden - ResponseErrorResponse (20013: insufficient permissions)
 
         404: Not Found - ResponseErrorResponse (71130: leaderboard config not found)
 
         500: Internal Server Error - ResponseErrorResponse (20000: internal server error)
 
         ---: HttpResponse (Undocumented Response)
 
@@ -226,26 +220,26 @@
     # endregion response methods
 
     # region static methods
 
     @classmethod
     def create(
         cls, leaderboard_code: str, namespace: str, **kwargs
-    ) -> HardDeleteLeaderboardAdminV1:
+    ) -> DeleteLeaderboardConfigurationAdminV3:
         instance = cls()
         instance.leaderboard_code = leaderboard_code
         instance.namespace = namespace
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> HardDeleteLeaderboardAdminV1:
+    ) -> DeleteLeaderboardConfigurationAdminV3:
         instance = cls()
         if "leaderboardCode" in dict_ and dict_["leaderboardCode"] is not None:
             instance.leaderboard_code = str(dict_["leaderboardCode"])
         elif include_empty:
             instance.leaderboard_code = ""
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
```

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration/update_leaderboard_conf_ca626e.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration/update_leaderboard_conf_ca626e.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration_v3/__init__.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration_v3/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Leaderboard Service."""
 
-__version__ = "2.28.0"
+__version__ = "2.29.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .create_leaderboard_conf_2ad364 import CreateLeaderboardConfigurationAdminV3
 from .delete_bulk_leaderboard_f7002d import DeleteBulkLeaderboardConfigurationAdminV3
```

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration_v3/create_leaderboard_conf_2ad364.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration_v3/create_leaderboard_conf_2ad364.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration_v3/delete_bulk_leaderboard_f7002d.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration_v3/delete_bulk_leaderboard_f7002d.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration_v3/delete_leaderboard_conf_8f143c.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration_v3/get_leaderboard_configu_33150a.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,41 +25,42 @@
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
+from ...models import ModelsGetLeaderboardConfigRespV3
 from ...models import ResponseErrorResponse
 
 
-class DeleteLeaderboardConfigurationAdminV3(Operation):
-    """delete leaderboard by leaderboardCode (deleteLeaderboardConfigurationAdminV3)
+class GetLeaderboardConfigurationAdminV3(Operation):
+    """get leaderboard by leaderboardCode (getLeaderboardConfigurationAdminV3)
 
-    This endpoint delete a leaderboard configuration
+    This endpoint returns a leaderboard configuration
 
     Properties:
         url: /leaderboard/v3/admin/namespaces/{namespace}/leaderboards/{leaderboardCode}
 
-        method: DELETE
+        method: GET
 
         tags: ["LeaderboardConfigurationV3"]
 
         consumes: []
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
         leaderboard_code: (leaderboardCode) REQUIRED str in path
 
         namespace: (namespace) REQUIRED str in path
 
     Responses:
-        204: No Content - (Leaderboard successfully deleted)
+        200: OK - ModelsGetLeaderboardConfigRespV3 (Leaderboard retrieved)
 
         400: Bad Request - ResponseErrorResponse (20002: validation error)
 
         401: Unauthorized - ResponseErrorResponse (20001: unauthorized access)
 
         403: Forbidden - ResponseErrorResponse (20013: insufficient permissions)
 
@@ -69,15 +70,15 @@
     """
 
     # region fields
 
     _url: str = (
         "/leaderboard/v3/admin/namespaces/{namespace}/leaderboards/{leaderboardCode}"
     )
-    _method: str = "DELETE"
+    _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
     leaderboard_code: str  # REQUIRED in [path]
     namespace: str  # REQUIRED in [path]
@@ -135,21 +136,19 @@
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_leaderboard_code(
-        self, value: str
-    ) -> DeleteLeaderboardConfigurationAdminV3:
+    def with_leaderboard_code(self, value: str) -> GetLeaderboardConfigurationAdminV3:
         self.leaderboard_code = value
         return self
 
-    def with_namespace(self, value: str) -> DeleteLeaderboardConfigurationAdminV3:
+    def with_namespace(self, value: str) -> GetLeaderboardConfigurationAdminV3:
         self.namespace = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
@@ -168,18 +167,21 @@
     # endregion to methods
 
     # region response methods
 
     # noinspection PyMethodMayBeStatic
     def parse_response(
         self, code: int, content_type: str, content: Any
-    ) -> Tuple[None, Union[None, HttpResponse, ResponseErrorResponse]]:
+    ) -> Tuple[
+        Union[None, ModelsGetLeaderboardConfigRespV3],
+        Union[None, HttpResponse, ResponseErrorResponse],
+    ]:
         """Parse the given response.
 
-        204: No Content - (Leaderboard successfully deleted)
+        200: OK - ModelsGetLeaderboardConfigRespV3 (Leaderboard retrieved)
 
         400: Bad Request - ResponseErrorResponse (20002: validation error)
 
         401: Unauthorized - ResponseErrorResponse (20001: unauthorized access)
 
         403: Forbidden - ResponseErrorResponse (20013: insufficient permissions)
 
@@ -196,16 +198,16 @@
         pre_processed_response, error = self.pre_process_response(
             code=code, content_type=content_type, content=content
         )
         if error is not None:
             return None, None if error.is_no_content() else error
         code, content_type, content = pre_processed_response
 
-        if code == 204:
-            return None, None
+        if code == 200:
+            return ModelsGetLeaderboardConfigRespV3.create_from_dict(content), None
         if code == 400:
             return None, ResponseErrorResponse.create_from_dict(content)
         if code == 401:
             return None, ResponseErrorResponse.create_from_dict(content)
         if code == 403:
             return None, ResponseErrorResponse.create_from_dict(content)
         if code == 404:
@@ -220,26 +222,26 @@
     # endregion response methods
 
     # region static methods
 
     @classmethod
     def create(
         cls, leaderboard_code: str, namespace: str, **kwargs
-    ) -> DeleteLeaderboardConfigurationAdminV3:
+    ) -> GetLeaderboardConfigurationAdminV3:
         instance = cls()
         instance.leaderboard_code = leaderboard_code
         instance.namespace = namespace
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> DeleteLeaderboardConfigurationAdminV3:
+    ) -> GetLeaderboardConfigurationAdminV3:
         instance = cls()
         if "leaderboardCode" in dict_ and dict_["leaderboardCode"] is not None:
             instance.leaderboard_code = str(dict_["leaderboardCode"])
         elif include_empty:
             instance.leaderboard_code = ""
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
```

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration_v3/get_leaderboard_configu_290af8.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration_v3/get_leaderboard_configu_290af8.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration_v3/get_leaderboard_configu_33150a.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration_v3/hard_delete_leaderboard_c58ff0.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,60 +25,75 @@
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
-from ...models import ModelsGetLeaderboardConfigRespV3
 from ...models import ResponseErrorResponse
 
 
-class GetLeaderboardConfigurationAdminV3(Operation):
-    """get leaderboard by leaderboardCode (getLeaderboardConfigurationAdminV3)
+class HardDeleteLeaderboardAdminV3(Operation):
+    """hard delete leaderboard config and data by leaderboard code (hardDeleteLeaderboardAdminV3)
 
-    This endpoint returns a leaderboard configuration
+    [Test Facility Only]
+
+
+
+
+    Required permission 'ADMIN:NAMESPACE:{namespace}:LEADERBOARD:HARDDELETE [DELETE]'
+
+
+
+
+    This endpoint will delete leaderboard configuration and its data
+
+
+
+
+    Note: this endpoint only works on development environment, you might want to use archive endpoint instead hard delete.
+
+    Required Permission(s):
+        - ADMIN:NAMESPACE:{namespace}:LEADERBOARD:HARDDELETE [DELETE]
 
     Properties:
-        url: /leaderboard/v3/admin/namespaces/{namespace}/leaderboards/{leaderboardCode}
+        url: /leaderboard/v3/admin/namespaces/{namespace}/leaderboards/{leaderboardCode}/hard
 
-        method: GET
+        method: DELETE
 
         tags: ["LeaderboardConfigurationV3"]
 
         consumes: []
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
         leaderboard_code: (leaderboardCode) REQUIRED str in path
 
         namespace: (namespace) REQUIRED str in path
 
     Responses:
-        200: OK - ModelsGetLeaderboardConfigRespV3 (Leaderboard retrieved)
+        204: No Content - (Leaderboard successfully deleted)
 
         400: Bad Request - ResponseErrorResponse (20002: validation error)
 
         401: Unauthorized - ResponseErrorResponse (20001: unauthorized access)
 
         403: Forbidden - ResponseErrorResponse (20013: insufficient permissions)
 
         404: Not Found - ResponseErrorResponse (71130: leaderboard config not found)
 
         500: Internal Server Error - ResponseErrorResponse (20000: internal server error)
     """
 
     # region fields
 
-    _url: str = (
-        "/leaderboard/v3/admin/namespaces/{namespace}/leaderboards/{leaderboardCode}"
-    )
-    _method: str = "GET"
+    _url: str = "/leaderboard/v3/admin/namespaces/{namespace}/leaderboards/{leaderboardCode}/hard"
+    _method: str = "DELETE"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
     leaderboard_code: str  # REQUIRED in [path]
     namespace: str  # REQUIRED in [path]
@@ -136,19 +151,19 @@
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_leaderboard_code(self, value: str) -> GetLeaderboardConfigurationAdminV3:
+    def with_leaderboard_code(self, value: str) -> HardDeleteLeaderboardAdminV3:
         self.leaderboard_code = value
         return self
 
-    def with_namespace(self, value: str) -> GetLeaderboardConfigurationAdminV3:
+    def with_namespace(self, value: str) -> HardDeleteLeaderboardAdminV3:
         self.namespace = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
@@ -167,21 +182,18 @@
     # endregion to methods
 
     # region response methods
 
     # noinspection PyMethodMayBeStatic
     def parse_response(
         self, code: int, content_type: str, content: Any
-    ) -> Tuple[
-        Union[None, ModelsGetLeaderboardConfigRespV3],
-        Union[None, HttpResponse, ResponseErrorResponse],
-    ]:
+    ) -> Tuple[None, Union[None, HttpResponse, ResponseErrorResponse]]:
         """Parse the given response.
 
-        200: OK - ModelsGetLeaderboardConfigRespV3 (Leaderboard retrieved)
+        204: No Content - (Leaderboard successfully deleted)
 
         400: Bad Request - ResponseErrorResponse (20002: validation error)
 
         401: Unauthorized - ResponseErrorResponse (20001: unauthorized access)
 
         403: Forbidden - ResponseErrorResponse (20013: insufficient permissions)
 
@@ -198,16 +210,16 @@
         pre_processed_response, error = self.pre_process_response(
             code=code, content_type=content_type, content=content
         )
         if error is not None:
             return None, None if error.is_no_content() else error
         code, content_type, content = pre_processed_response
 
-        if code == 200:
-            return ModelsGetLeaderboardConfigRespV3.create_from_dict(content), None
+        if code == 204:
+            return None, None
         if code == 400:
             return None, ResponseErrorResponse.create_from_dict(content)
         if code == 401:
             return None, ResponseErrorResponse.create_from_dict(content)
         if code == 403:
             return None, ResponseErrorResponse.create_from_dict(content)
         if code == 404:
@@ -222,26 +234,26 @@
     # endregion response methods
 
     # region static methods
 
     @classmethod
     def create(
         cls, leaderboard_code: str, namespace: str, **kwargs
-    ) -> GetLeaderboardConfigurationAdminV3:
+    ) -> HardDeleteLeaderboardAdminV3:
         instance = cls()
         instance.leaderboard_code = leaderboard_code
         instance.namespace = namespace
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> GetLeaderboardConfigurationAdminV3:
+    ) -> HardDeleteLeaderboardAdminV3:
         instance = cls()
         if "leaderboardCode" in dict_ and dict_["leaderboardCode"] is not None:
             instance.leaderboard_code = str(dict_["leaderboardCode"])
         elif include_empty:
             instance.leaderboard_code = ""
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
```

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration_v3/get_leaderboard_configu_9b2b53.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration_v3/get_leaderboard_configu_9b2b53.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration_v3/get_leaderboard_configu_b16dd3.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration_v3/get_leaderboard_configu_b16dd3.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration_v3/hard_delete_leaderboard_c58ff0.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration/hard_delete_leaderboard_e07e01.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,63 +28,71 @@
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
 from ...models import ResponseErrorResponse
 
 
-class HardDeleteLeaderboardAdminV3(Operation):
-    """hard delete leaderboard config and data by leaderboard code (hardDeleteLeaderboardAdminV3)
+class HardDeleteLeaderboardAdminV1(Operation):
+    """hard delete leaderboard config and data by leaderboard code (hardDeleteLeaderboardAdminV1)
 
     [Test Facility Only]
 
 
 
 
+    Required permission 'ADMIN:NAMESPACE:{namespace}:LEADERBOARD:HARDDELETE [DELETE]'
+
+
+
+
     This endpoint will delete leaderboard configuration and its data
 
 
 
 
     Note: this endpoint only works on development environment, you might want to use archive endpoint instead hard delete.
 
+    Required Permission(s):
+        - ADMIN:NAMESPACE:{namespace}:LEADERBOARD:HARDDELETE [DELETE]
+
     Properties:
-        url: /leaderboard/v3/admin/namespaces/{namespace}/leaderboards/{leaderboardCode}/hard
+        url: /leaderboard/v1/admin/namespaces/{namespace}/leaderboards/{leaderboardCode}/hard
 
         method: DELETE
 
-        tags: ["LeaderboardConfigurationV3"]
+        tags: ["LeaderboardConfiguration"]
 
         consumes: []
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
         leaderboard_code: (leaderboardCode) REQUIRED str in path
 
         namespace: (namespace) REQUIRED str in path
 
     Responses:
-        204: No Content - (Leaderboard successfully deleted)
+        204: No Content - (Leaderboard deleted)
 
         400: Bad Request - ResponseErrorResponse (20002: validation error)
 
         401: Unauthorized - ResponseErrorResponse (20001: unauthorized access)
 
-        403: Forbidden - ResponseErrorResponse (20013: insufficient permissions | 71241: forbidden environment)
+        403: Forbidden - ResponseErrorResponse (20013: insufficient permissions)
 
         404: Not Found - ResponseErrorResponse (71130: leaderboard config not found)
 
         500: Internal Server Error - ResponseErrorResponse (20000: internal server error)
     """
 
     # region fields
 
-    _url: str = "/leaderboard/v3/admin/namespaces/{namespace}/leaderboards/{leaderboardCode}/hard"
+    _url: str = "/leaderboard/v1/admin/namespaces/{namespace}/leaderboards/{leaderboardCode}/hard"
     _method: str = "DELETE"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
     leaderboard_code: str  # REQUIRED in [path]
@@ -143,19 +151,19 @@
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_leaderboard_code(self, value: str) -> HardDeleteLeaderboardAdminV3:
+    def with_leaderboard_code(self, value: str) -> HardDeleteLeaderboardAdminV1:
         self.leaderboard_code = value
         return self
 
-    def with_namespace(self, value: str) -> HardDeleteLeaderboardAdminV3:
+    def with_namespace(self, value: str) -> HardDeleteLeaderboardAdminV1:
         self.namespace = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
@@ -177,21 +185,21 @@
 
     # noinspection PyMethodMayBeStatic
     def parse_response(
         self, code: int, content_type: str, content: Any
     ) -> Tuple[None, Union[None, HttpResponse, ResponseErrorResponse]]:
         """Parse the given response.
 
-        204: No Content - (Leaderboard successfully deleted)
+        204: No Content - (Leaderboard deleted)
 
         400: Bad Request - ResponseErrorResponse (20002: validation error)
 
         401: Unauthorized - ResponseErrorResponse (20001: unauthorized access)
 
-        403: Forbidden - ResponseErrorResponse (20013: insufficient permissions | 71241: forbidden environment)
+        403: Forbidden - ResponseErrorResponse (20013: insufficient permissions)
 
         404: Not Found - ResponseErrorResponse (71130: leaderboard config not found)
 
         500: Internal Server Error - ResponseErrorResponse (20000: internal server error)
 
         ---: HttpResponse (Undocumented Response)
 
@@ -226,26 +234,26 @@
     # endregion response methods
 
     # region static methods
 
     @classmethod
     def create(
         cls, leaderboard_code: str, namespace: str, **kwargs
-    ) -> HardDeleteLeaderboardAdminV3:
+    ) -> HardDeleteLeaderboardAdminV1:
         instance = cls()
         instance.leaderboard_code = leaderboard_code
         instance.namespace = namespace
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> HardDeleteLeaderboardAdminV3:
+    ) -> HardDeleteLeaderboardAdminV1:
         instance = cls()
         if "leaderboardCode" in dict_ and dict_["leaderboardCode"] is not None:
             instance.leaderboard_code = str(dict_["leaderboardCode"])
         elif include_empty:
             instance.leaderboard_code = ""
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
```

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration_v3/update_leaderboard_conf_1b8e6b.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_configuration_v3/update_leaderboard_conf_1b8e6b.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/__init__.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Leaderboard Service."""
 
-__version__ = "2.28.0"
+__version__ = "2.29.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .admin_get_archived_lead_191726 import (
     AdminGetArchivedLeaderboardRankingDataV1Handler,
```

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/admin_get_archived_lead_191726.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/admin_get_archived_lead_191726.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/create_archived_leaderb_5492e4.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/create_archived_leaderb_5492e4.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/delete_user_ranking_admin_v1.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/delete_user_ranking_admin_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/delete_user_ranking_by__ed6de1.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/delete_user_ranking_by__ed6de1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/delete_user_ranking_public_v1.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/delete_user_ranking_public_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/delete_user_rankings_admin_v1.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/delete_user_rankings_admin_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/get_all_time_leaderboar_358b23.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/get_all_time_leaderboar_358b23.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/get_all_time_leaderboar_9cbcdd.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/get_all_time_leaderboar_9cbcdd.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/get_all_time_leaderboar_d0fb4b.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/get_all_time_leaderboar_d0fb4b.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/get_archived_leaderboar_c023ea.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/get_archived_leaderboar_c023ea.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/get_current_month_leade_26486d.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/get_current_month_leade_26486d.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/get_current_month_leade_4373db.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/get_current_month_leade_4373db.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/get_current_season_lead_51d992.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/get_current_season_lead_51d992.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/get_current_season_lead_a79ffc.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/get_current_season_lead_a79ffc.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/get_current_week_leader_07d571.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/get_current_week_leader_07d571.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/get_current_week_leader_bdd5ce.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/get_current_week_leader_bdd5ce.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/get_today_leaderboard_r_2eefd7.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/get_today_leaderboard_r_2eefd7.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/get_today_leaderboard_r_51cbb5.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/get_today_leaderboard_r_51cbb5.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/get_user_ranking_admin_v1.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/get_user_ranking_admin_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/get_user_ranking_public_v1.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/get_user_ranking_public_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/update_user_point_admin_v1.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data/update_user_point_admin_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data_v3/__init__.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data_v3/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Leaderboard Service."""
 
-__version__ = "2.28.0"
+__version__ = "2.29.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .bulk_get_users_ranking__e7e5b3 import BulkGetUsersRankingPublicV3
 from .delete_user_ranking_admin_v3 import DeleteUserRankingAdminV3
```

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data_v3/bulk_get_users_ranking__e7e5b3.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data_v3/bulk_get_users_ranking__e7e5b3.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data_v3/delete_user_ranking_admin_v3.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data_v3/delete_user_ranking_admin_v3.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data_v3/delete_user_ranking_by__c762e5.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data_v3/delete_user_ranking_by__c762e5.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data_v3/delete_user_rankings_admin_v3.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data_v3/delete_user_rankings_admin_v3.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data_v3/get_all_time_leaderboar_489ddb.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data_v3/get_all_time_leaderboar_489ddb.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data_v3/get_all_time_leaderboar_5b0d52.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data_v3/get_all_time_leaderboar_5b0d52.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data_v3/get_current_cycle_leade_2c20ce.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data_v3/get_current_cycle_leade_2c20ce.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data_v3/get_current_cycle_leade_f8a4d7.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data_v3/get_current_cycle_leade_f8a4d7.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data_v3/get_user_ranking_admin_v3.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data_v3/get_user_ranking_admin_v3.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data_v3/get_user_ranking_public_v3.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/leaderboard_data_v3/get_user_ranking_public_v3.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/user_data/__init__.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/user_data/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,14 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Leaderboard Service."""
 
-__version__ = "2.28.0"
+__version__ = "2.29.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .get_user_leaderboard_ra_d2aae2 import GetUserLeaderboardRankingsAdminV1
```

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/user_data/get_user_leaderboard_ra_d2aae2.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/user_data/get_user_leaderboard_ra_d2aae2.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/user_data_v3/__init__.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/user_data_v3/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,14 +4,14 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Leaderboard Service."""
 
-__version__ = "2.28.0"
+__version__ = "2.29.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .get_user_leaderboard_ra_e5b21a import GetUserLeaderboardRankingsAdminV3
```

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/user_data_v3/get_user_leaderboard_ra_e5b21a.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/user_data_v3/get_user_leaderboard_ra_e5b21a.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/user_visibility/__init__.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/user_visibility/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Leaderboard Service."""
 
-__version__ = "2.28.0"
+__version__ = "2.29.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .get_hidden_users_v2 import GetHiddenUsersV2
 from .get_user_visibility_status_v2 import GetUserVisibilityStatusV2
```

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/user_visibility/get_hidden_users_v2.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/user_visibility/get_hidden_users_v2.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/user_visibility/get_user_visibility_status_v2.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/user_visibility/get_user_visibility_status_v2.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/user_visibility/set_user_leaderboard_vi_7b0546.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/user_visibility/set_user_leaderboard_vi_7b0546.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/user_visibility/set_user_visibility_status_v2.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/user_visibility/set_user_visibility_status_v2.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/user_visibility_v3/__init__.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/user_visibility_v3/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Leaderboard Service."""
 
-__version__ = "2.28.0"
+__version__ = "2.29.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .get_hidden_users_v3 import GetHiddenUsersV3
 from .get_user_visibility_status_v3 import GetUserVisibilityStatusV3
```

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/user_visibility_v3/get_hidden_users_v3.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/user_visibility_v3/get_hidden_users_v3.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/user_visibility_v3/get_user_visibility_status_v3.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/user_visibility_v3/get_user_visibility_status_v3.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/user_visibility_v3/set_user_leaderboard_vi_da19f8.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/user_visibility_v3/set_user_leaderboard_vi_da19f8.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/operations/user_visibility_v3/set_user_visibility_v3.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/operations/user_visibility_v3/set_user_visibility_v3.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/wrappers/__init__.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/wrappers/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: wrapper-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Leaderboard Service."""
 
-__version__ = "2.28.0"
+__version__ = "2.29.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from ._anonymization import admin_anonymize_user_leaderboard_admin_v1
 from ._anonymization import admin_anonymize_user_leaderboard_admin_v1_async
```

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/wrappers/_anonymization.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/wrappers/_anonymization.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/wrappers/_leaderboard_configuration.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/wrappers/_leaderboard_configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1077,21 +1077,29 @@
     """hard delete leaderboard config and data by leaderboard code (hardDeleteLeaderboardAdminV1)
 
     [Test Facility Only]
 
 
 
 
+    Required permission 'ADMIN:NAMESPACE:{namespace}:LEADERBOARD:HARDDELETE [DELETE]'
+
+
+
+
     This endpoint will delete leaderboard configuration and its data
 
 
 
 
     Note: this endpoint only works on development environment, you might want to use archive endpoint instead hard delete.
 
+    Required Permission(s):
+        - ADMIN:NAMESPACE:{namespace}:LEADERBOARD:HARDDELETE [DELETE]
+
     Properties:
         url: /leaderboard/v1/admin/namespaces/{namespace}/leaderboards/{leaderboardCode}/hard
 
         method: DELETE
 
         tags: ["LeaderboardConfiguration"]
 
@@ -1108,15 +1116,15 @@
     Responses:
         204: No Content - (Leaderboard deleted)
 
         400: Bad Request - ResponseErrorResponse (20002: validation error)
 
         401: Unauthorized - ResponseErrorResponse (20001: unauthorized access)
 
-        403: Forbidden - ResponseErrorResponse (20013: insufficient permissions | 71241: forbidden environment)
+        403: Forbidden - ResponseErrorResponse (20013: insufficient permissions)
 
         404: Not Found - ResponseErrorResponse (71130: leaderboard config not found)
 
         500: Internal Server Error - ResponseErrorResponse (20000: internal server error)
     """
     if namespace is None:
         namespace, error = get_services_namespace()
@@ -1139,21 +1147,29 @@
     """hard delete leaderboard config and data by leaderboard code (hardDeleteLeaderboardAdminV1)
 
     [Test Facility Only]
 
 
 
 
+    Required permission 'ADMIN:NAMESPACE:{namespace}:LEADERBOARD:HARDDELETE [DELETE]'
+
+
+
+
     This endpoint will delete leaderboard configuration and its data
 
 
 
 
     Note: this endpoint only works on development environment, you might want to use archive endpoint instead hard delete.
 
+    Required Permission(s):
+        - ADMIN:NAMESPACE:{namespace}:LEADERBOARD:HARDDELETE [DELETE]
+
     Properties:
         url: /leaderboard/v1/admin/namespaces/{namespace}/leaderboards/{leaderboardCode}/hard
 
         method: DELETE
 
         tags: ["LeaderboardConfiguration"]
 
@@ -1170,15 +1186,15 @@
     Responses:
         204: No Content - (Leaderboard deleted)
 
         400: Bad Request - ResponseErrorResponse (20002: validation error)
 
         401: Unauthorized - ResponseErrorResponse (20001: unauthorized access)
 
-        403: Forbidden - ResponseErrorResponse (20013: insufficient permissions | 71241: forbidden environment)
+        403: Forbidden - ResponseErrorResponse (20013: insufficient permissions)
 
         404: Not Found - ResponseErrorResponse (71130: leaderboard config not found)
 
         500: Internal Server Error - ResponseErrorResponse (20000: internal server error)
     """
     if namespace is None:
         namespace, error = get_services_namespace()
```

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/wrappers/_leaderboard_configuration_v3.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/wrappers/_leaderboard_configuration_v3.py`

 * *Files 2% similar despite different names*

```diff
@@ -888,21 +888,29 @@
     """hard delete leaderboard config and data by leaderboard code (hardDeleteLeaderboardAdminV3)
 
     [Test Facility Only]
 
 
 
 
+    Required permission 'ADMIN:NAMESPACE:{namespace}:LEADERBOARD:HARDDELETE [DELETE]'
+
+
+
+
     This endpoint will delete leaderboard configuration and its data
 
 
 
 
     Note: this endpoint only works on development environment, you might want to use archive endpoint instead hard delete.
 
+    Required Permission(s):
+        - ADMIN:NAMESPACE:{namespace}:LEADERBOARD:HARDDELETE [DELETE]
+
     Properties:
         url: /leaderboard/v3/admin/namespaces/{namespace}/leaderboards/{leaderboardCode}/hard
 
         method: DELETE
 
         tags: ["LeaderboardConfigurationV3"]
 
@@ -919,15 +927,15 @@
     Responses:
         204: No Content - (Leaderboard successfully deleted)
 
         400: Bad Request - ResponseErrorResponse (20002: validation error)
 
         401: Unauthorized - ResponseErrorResponse (20001: unauthorized access)
 
-        403: Forbidden - ResponseErrorResponse (20013: insufficient permissions | 71241: forbidden environment)
+        403: Forbidden - ResponseErrorResponse (20013: insufficient permissions)
 
         404: Not Found - ResponseErrorResponse (71130: leaderboard config not found)
 
         500: Internal Server Error - ResponseErrorResponse (20000: internal server error)
     """
     if namespace is None:
         namespace, error = get_services_namespace()
@@ -950,21 +958,29 @@
     """hard delete leaderboard config and data by leaderboard code (hardDeleteLeaderboardAdminV3)
 
     [Test Facility Only]
 
 
 
 
+    Required permission 'ADMIN:NAMESPACE:{namespace}:LEADERBOARD:HARDDELETE [DELETE]'
+
+
+
+
     This endpoint will delete leaderboard configuration and its data
 
 
 
 
     Note: this endpoint only works on development environment, you might want to use archive endpoint instead hard delete.
 
+    Required Permission(s):
+        - ADMIN:NAMESPACE:{namespace}:LEADERBOARD:HARDDELETE [DELETE]
+
     Properties:
         url: /leaderboard/v3/admin/namespaces/{namespace}/leaderboards/{leaderboardCode}/hard
 
         method: DELETE
 
         tags: ["LeaderboardConfigurationV3"]
 
@@ -981,15 +997,15 @@
     Responses:
         204: No Content - (Leaderboard successfully deleted)
 
         400: Bad Request - ResponseErrorResponse (20002: validation error)
 
         401: Unauthorized - ResponseErrorResponse (20001: unauthorized access)
 
-        403: Forbidden - ResponseErrorResponse (20013: insufficient permissions | 71241: forbidden environment)
+        403: Forbidden - ResponseErrorResponse (20013: insufficient permissions)
 
         404: Not Found - ResponseErrorResponse (71130: leaderboard config not found)
 
         500: Internal Server Error - ResponseErrorResponse (20000: internal server error)
     """
     if namespace is None:
         namespace, error = get_services_namespace()
```

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/wrappers/_leaderboard_data.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/wrappers/_leaderboard_data.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/wrappers/_leaderboard_data_v3.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/wrappers/_leaderboard_data_v3.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/wrappers/_user_data.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/wrappers/_user_data.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/wrappers/_user_data_v3.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/wrappers/_user_data_v3.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/wrappers/_user_visibility.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/wrappers/_user_visibility.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk/api/leaderboard/wrappers/_user_visibility_v3.py` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk/api/leaderboard/wrappers/_user_visibility_v3.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk_service_leaderboard.egg-info/PKG-INFO` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk_service_leaderboard.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: accelbyte-py-sdk-service-leaderboard
-Version: 0.8.0
+Version: 0.9.0
 Summary: AccelByte Python SDK - AccelByte Gaming Services Leaderboard Service
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: accelbyte-py-sdk-core
 
 [//]: # (Code generated. DO NOT EDIT!)
 
 # AccelByte Modular Python SDK - Service Module
 
 This is a service module for the [AccelByte Modular Python SDK](https://github.com/AccelByte/accelbyte-python-modular-sdk) package.
 
 ```text
 AccelByte Gaming Services Leaderboard Service
-* Version: 2.28.0
+* Version: 2.29.0
 ```
 
 ## Setup
 
 This SDK requires Python 3.9 to be installed.
 
 ### Install with Pip
```

### Comparing `accelbyte-py-sdk-service-leaderboard-0.8.0/accelbyte_py_sdk_service_leaderboard.egg-info/SOURCES.txt` & `accelbyte-py-sdk-service-leaderboard-0.9.0/accelbyte_py_sdk_service_leaderboard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

