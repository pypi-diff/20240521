# Comparing `tmp/accelbyte_py_sdk_service_ams-0.8.0.tar.gz` & `tmp/accelbyte_py_sdk_service_ams-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accelbyte_py_sdk_service_ams-0.8.0.tar", last modified: Tue May  7 06:25:47 2024, max compression
+gzip compressed data, was "accelbyte_py_sdk_service_ams-0.9.0.tar", last modified: Tue May 21 03:44:59 2024, max compression
```

## Comparing `accelbyte_py_sdk_service_ams-0.8.0.tar` & `accelbyte_py_sdk_service_ams-0.9.0.tar`

### file list

```diff
@@ -1,151 +1,151 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:25:47.721259 accelbyte_py_sdk_service_ams-0.8.0/
--rw-r--r--   0 root         (0) root         (0)     1065 2024-05-07 06:25:47.721259 accelbyte_py_sdk_service_ams-0.8.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      843 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:25:47.709260 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:25:47.709260 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:25:47.709260 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/
--rw-rw-r--   0 root         (0) root         (0)     4248 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:25:47.713260 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/
--rw-rw-r--   0 root         (0) root         (0)     4009 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3712 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_account_create_request.py
--rw-rw-r--   0 root         (0) root         (0)     5933 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_account_create_response.py
--rw-rw-r--   0 root         (0) root         (0)     7626 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_account_limits.py
--rw-rw-r--   0 root         (0) root         (0)     3710 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_account_link_request.py
--rw-rw-r--   0 root         (0) root         (0)     5905 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_account_link_response.py
--rw-rw-r--   0 root         (0) root         (0)     3777 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_account_link_token_response.py
--rw-rw-r--   0 root         (0) root         (0)     5831 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_account_response.py
--rw-rw-r--   0 root         (0) root         (0)     3872 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_ams_regions_response.py
--rw-rw-r--   0 root         (0) root         (0)     4756 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_artifact_list_response.py
--rw-rw-r--   0 root         (0) root         (0)    10866 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_artifact_response.py
--rw-rw-r--   0 root         (0) root         (0)     4484 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_artifact_sampling_rule.py
--rw-rw-r--   0 root         (0) root         (0)     5109 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_artifact_type_sampling_rules.py
--rw-rw-r--   0 root         (0) root         (0)     3681 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_artifact_url_response.py
--rw-rw-r--   0 root         (0) root         (0)     5325 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_artifact_usage_response.py
--rw-rw-r--   0 root         (0) root         (0)     4810 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_available_instance_types_response.py
--rw-rw-r--   0 root         (0) root         (0)     5643 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_development_server_configuration_create_request.py
--rw-rw-r--   0 root         (0) root         (0)     3992 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_development_server_configuration_create_response.py
--rw-rw-r--   0 root         (0) root         (0)     5603 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_development_server_configuration_get_response.py
--rw-rw-r--   0 root         (0) root         (0)     5300 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_development_server_configuration_list_response.py
--rw-rw-r--   0 root         (0) root         (0)     7606 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_ds_history_event.py
--rw-rw-r--   0 root         (0) root         (0)     4833 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_ds_history_list.py
--rw-rw-r--   0 root         (0) root         (0)     5335 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_ds_host_configuration.py
--rw-rw-r--   0 root         (0) root         (0)     5170 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_fleet_artifacts_sample_rules.py
--rw-rw-r--   0 root         (0) root         (0)     5243 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_fleet_claim_by_keys_req.py
--rw-rw-r--   0 root         (0) root         (0)     4317 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_fleet_claim_req.py
--rw-rw-r--   0 root         (0) root         (0)     5630 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_fleet_claim_response.py
--rw-rw-r--   0 root         (0) root         (0)     3672 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_fleet_create_response.py
--rw-rw-r--   0 root         (0) root         (0)    10552 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_fleet_get_response.py
--rw-rw-r--   0 root         (0) root         (0)     8648 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_fleet_list_item_response.py
--rw-rw-r--   0 root         (0) root         (0)     4174 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_fleet_list_response.py
--rw-rw-r--   0 root         (0) root         (0)    10632 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_fleet_parameters.py
--rw-rw-r--   0 root         (0) root         (0)     7934 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_fleet_regional_server_counts.py
--rw-rw-r--   0 root         (0) root         (0)     6137 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_fleet_server_connection_info_response.py
--rw-rw-r--   0 root         (0) root         (0)     7978 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_fleet_server_history_event_response.py
--rw-rw-r--   0 root         (0) root         (0)     4354 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_fleet_server_history_response.py
--rw-rw-r--   0 root         (0) root         (0)    13441 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_fleet_server_info_response.py
--rw-rw-r--   0 root         (0) root         (0)     5362 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_fleet_servers_response.py
--rw-rw-r--   0 root         (0) root         (0)     6671 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_image_deployment_profile.py
--rw-rw-r--   0 root         (0) root         (0)    10824 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_image_details.py
--rw-rw-r--   0 root         (0) root         (0)     3917 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_image_list.py
--rw-rw-r--   0 root         (0) root         (0)    10462 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_image_list_item.py
--rw-rw-r--   0 root         (0) root         (0)     5849 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_image_update.py
--rw-rw-r--   0 root         (0) root         (0)     7271 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_instance_type_description_response.py
--rw-rw-r--   0 root         (0) root         (0)     8240 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_paging_info.py
--rw-rw-r--   0 root         (0) root         (0)     4323 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_port_configuration.py
--rw-rw-r--   0 root         (0) root         (0)     4066 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_qo_s_endpoint_response.py
--rw-rw-r--   0 root         (0) root         (0)     6600 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_qo_s_server.py
--rw-rw-r--   0 root         (0) root         (0)     5104 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_referencing_fleet.py
--rw-rw-r--   0 root         (0) root         (0)     5941 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_region_config.py
--rw-rw-r--   0 root         (0) root         (0)     4775 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_time.py
--rw-rw-r--   0 root         (0) root         (0)     5513 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_timeout.py
--rw-rw-r--   0 root         (0) root         (0)     3741 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_update_server_request.py
--rw-rw-r--   0 root         (0) root         (0)     5191 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/response_error_response.py
--rw-rw-r--   0 root         (0) root         (0)     7999 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/time_location.py
--rw-rw-r--   0 root         (0) root         (0)     4688 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/time_zone.py
--rw-rw-r--   0 root         (0) root         (0)     5338 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/time_zone_trans.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:25:47.713260 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/
--rw-rw-r--   0 root         (0) root         (0)      410 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:25:47.713260 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/account/
--rw-rw-r--   0 root         (0) root         (0)      715 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/account/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6823 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/account/account_get.py
--rw-rw-r--   0 root         (0) root         (0)     7829 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/account/admin_account_create.py
--rw-rw-r--   0 root         (0) root         (0)     6898 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/account/admin_account_get.py
--rw-rw-r--   0 root         (0) root         (0)     7188 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/account/admin_account_link_token_get.py
--rw-rw-r--   0 root         (0) root         (0)     8043 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/account/admin_account_link_token_post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:25:47.717259 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/ams_info/
--rw-rw-r--   0 root         (0) root         (0)      583 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/ams_info/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6623 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/ams_info/info_regions.py
--rw-rw-r--   0 root         (0) root         (0)     6790 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/ams_info/info_supported_instances.py
--rw-rw-r--   0 root         (0) root         (0)     4453 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/ams_info/upload_url_get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:25:47.717259 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/ams_qo_s/
--rw-rw-r--   0 root         (0) root         (0)      537 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/ams_qo_s/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8566 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/ams_qo_s/qo_s_regions_get.py
--rw-rw-r--   0 root         (0) root         (0)     8934 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/ams_qo_s/qo_s_regions_update.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:25:47.717259 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/artifacts/
--rw-rw-r--   0 root         (0) root         (0)      767 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/artifacts/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7939 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/artifacts/artifact_delete.py
--rw-rw-r--   0 root         (0) root         (0)    16985 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/artifacts/artifact_get.py
--rw-rw-r--   0 root         (0) root         (0)     8071 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/artifacts/artifact_get_url.py
--rw-rw-r--   0 root         (0) root         (0)     6724 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/artifacts/artifact_usage_get.py
--rw-rw-r--   0 root         (0) root         (0)     8204 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/artifacts/fleet_artifact_sampling_739743.py
--rw-rw-r--   0 root         (0) root         (0)     9258 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/artifacts/fleet_artifact_sampling_a22d2b.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:25:47.717259 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/auth/
--rw-rw-r--   0 root         (0) root         (0)      477 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/auth/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5321 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/auth/auth_check.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:25:47.717259 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/development/
--rw-rw-r--   0 root         (0) root         (0)      762 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/development/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8497 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/development/development_server_conf_2194f5.py
--rw-rw-r--   0 root         (0) root         (0)     8782 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/development/development_server_conf_282185.py
--rw-rw-r--   0 root         (0) root         (0)     8819 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/development/development_server_conf_7b687b.py
--rw-rw-r--   0 root         (0) root         (0)     8882 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/development/development_server_conf_a8e4dd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:25:47.717259 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/fleet_commander/
--rw-rw-r--   0 root         (0) root         (0)      568 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/fleet_commander/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4429 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/fleet_commander/basic_health_check.py
--rw-rw-r--   0 root         (0) root         (0)     4383 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/fleet_commander/func1.py
--rw-rw-r--   0 root         (0) root         (0)     4445 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/fleet_commander/portal_health_check.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:25:47.717259 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/fleets/
--rw-rw-r--   0 root         (0) root         (0)      759 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/fleets/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8942 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/fleets/fleet_claim_by_id.py
--rw-rw-r--   0 root         (0) root         (0)     8296 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/fleets/fleet_claim_by_keys.py
--rw-rw-r--   0 root         (0) root         (0)     7948 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/fleets/fleet_create.py
--rw-rw-r--   0 root         (0) root         (0)     7685 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/fleets/fleet_delete.py
--rw-rw-r--   0 root         (0) root         (0)     7806 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/fleets/fleet_get.py
--rw-rw-r--   0 root         (0) root         (0)     6104 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/fleets/fleet_list.py
--rw-rw-r--   0 root         (0) root         (0)     7902 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/fleets/fleet_servers.py
--rw-rw-r--   0 root         (0) root         (0)     8836 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/fleets/fleet_update.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:25:47.717259 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/images/
--rw-rw-r--   0 root         (0) root         (0)      545 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/images/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7569 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/images/image_get.py
--rw-rw-r--   0 root         (0) root         (0)     6926 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/images/image_list.py
--rw-rw-r--   0 root         (0) root         (0)     8711 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/images/image_patch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:25:47.717259 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/servers/
--rw-rw-r--   0 root         (0) root         (0)      653 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/servers/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7939 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/servers/fleet_server_connection_info.py
--rw-rw-r--   0 root         (0) root         (0)    13566 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/servers/fleet_server_history.py
--rw-rw-r--   0 root         (0) root         (0)     7754 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/servers/fleet_server_info.py
--rw-rw-r--   0 root         (0) root         (0)     7756 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/servers/server_history.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:25:47.717259 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/watchdogs/
--rw-rw-r--   0 root         (0) root         (0)      546 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/watchdogs/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6576 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/watchdogs/local_watchdog_connect.py
--rw-rw-r--   0 root         (0) root         (0)     6505 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/watchdogs/watchdog_connect.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:25:47.721259 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/wrappers/
--rw-rw-r--   0 root         (0) root         (0)     4219 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/wrappers/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    16497 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/wrappers/_account.py
--rw-rw-r--   0 root         (0) root         (0)     7740 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/wrappers/_ams_info.py
--rw-rw-r--   0 root         (0) root         (0)     9299 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/wrappers/_ams_qo_s.py
--rw-rw-r--   0 root         (0) root         (0)    23216 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/wrappers/_artifacts.py
--rw-rw-r--   0 root         (0) root         (0)     2878 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/wrappers/_auth.py
--rw-rw-r--   0 root         (0) root         (0)    15713 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/wrappers/_development.py
--rw-rw-r--   0 root         (0) root         (0)     4481 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/wrappers/_fleet_commander.py
--rw-rw-r--   0 root         (0) root         (0)    25867 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/wrappers/_fleets.py
--rw-rw-r--   0 root         (0) root         (0)    10383 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/wrappers/_images.py
--rw-rw-r--   0 root         (0) root         (0)    15196 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/wrappers/_servers.py
--rw-rw-r--   0 root         (0) root         (0)     5840 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/wrappers/_watchdogs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:25:47.721259 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk_service_ams.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1065 2024-05-07 06:25:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk_service_ams.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7799 2024-05-07 06:25:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk_service_ams.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-07 06:25:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk_service_ams.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-07 06:25:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk_service_ams.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-05-07 06:25:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk_service_ams.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)      329 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-07 06:25:47.721259 accelbyte_py_sdk_service_ams-0.8.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:44:59.033824 accelbyte_py_sdk_service_ams-0.9.0/
+-rw-r--r--   0 root         (0) root         (0)     1065 2024-05-21 03:44:59.033824 accelbyte_py_sdk_service_ams-0.9.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      843 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:44:59.021825 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:44:59.021825 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:44:59.021825 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/
+-rw-rw-r--   0 root         (0) root         (0)     4248 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:44:59.029824 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/
+-rw-rw-r--   0 root         (0) root         (0)     4009 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3712 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_account_create_request.py
+-rw-rw-r--   0 root         (0) root         (0)     5933 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_account_create_response.py
+-rw-rw-r--   0 root         (0) root         (0)     7626 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_account_limits.py
+-rw-rw-r--   0 root         (0) root         (0)     3710 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_account_link_request.py
+-rw-rw-r--   0 root         (0) root         (0)     5905 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_account_link_response.py
+-rw-rw-r--   0 root         (0) root         (0)     3777 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_account_link_token_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5831 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_account_response.py
+-rw-rw-r--   0 root         (0) root         (0)     3872 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_ams_regions_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4756 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_artifact_list_response.py
+-rw-rw-r--   0 root         (0) root         (0)    10866 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_artifact_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4484 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_artifact_sampling_rule.py
+-rw-rw-r--   0 root         (0) root         (0)     5109 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_artifact_type_sampling_rules.py
+-rw-rw-r--   0 root         (0) root         (0)     3681 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_artifact_url_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5325 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_artifact_usage_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4810 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_available_instance_types_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5643 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_development_server_configuration_create_request.py
+-rw-rw-r--   0 root         (0) root         (0)     3992 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_development_server_configuration_create_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5603 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_development_server_configuration_get_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5300 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_development_server_configuration_list_response.py
+-rw-rw-r--   0 root         (0) root         (0)     7606 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_ds_history_event.py
+-rw-rw-r--   0 root         (0) root         (0)     4833 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_ds_history_list.py
+-rw-rw-r--   0 root         (0) root         (0)     5335 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_ds_host_configuration.py
+-rw-rw-r--   0 root         (0) root         (0)     5170 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_fleet_artifacts_sample_rules.py
+-rw-rw-r--   0 root         (0) root         (0)     5243 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_fleet_claim_by_keys_req.py
+-rw-rw-r--   0 root         (0) root         (0)     4317 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_fleet_claim_req.py
+-rw-rw-r--   0 root         (0) root         (0)     5630 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_fleet_claim_response.py
+-rw-rw-r--   0 root         (0) root         (0)     3672 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_fleet_create_response.py
+-rw-rw-r--   0 root         (0) root         (0)    10552 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_fleet_get_response.py
+-rw-rw-r--   0 root         (0) root         (0)     8648 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_fleet_list_item_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4174 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_fleet_list_response.py
+-rw-rw-r--   0 root         (0) root         (0)    10632 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_fleet_parameters.py
+-rw-rw-r--   0 root         (0) root         (0)     7934 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_fleet_regional_server_counts.py
+-rw-rw-r--   0 root         (0) root         (0)     6137 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_fleet_server_connection_info_response.py
+-rw-rw-r--   0 root         (0) root         (0)     7978 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_fleet_server_history_event_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4354 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_fleet_server_history_response.py
+-rw-rw-r--   0 root         (0) root         (0)    13441 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_fleet_server_info_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5362 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_fleet_servers_response.py
+-rw-rw-r--   0 root         (0) root         (0)     6671 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_image_deployment_profile.py
+-rw-rw-r--   0 root         (0) root         (0)    10824 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_image_details.py
+-rw-rw-r--   0 root         (0) root         (0)     3917 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_image_list.py
+-rw-rw-r--   0 root         (0) root         (0)    10462 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_image_list_item.py
+-rw-rw-r--   0 root         (0) root         (0)     5849 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_image_update.py
+-rw-rw-r--   0 root         (0) root         (0)     7271 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_instance_type_description_response.py
+-rw-rw-r--   0 root         (0) root         (0)     8240 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_paging_info.py
+-rw-rw-r--   0 root         (0) root         (0)     4323 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_port_configuration.py
+-rw-rw-r--   0 root         (0) root         (0)     4066 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_qo_s_endpoint_response.py
+-rw-rw-r--   0 root         (0) root         (0)     6600 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_qo_s_server.py
+-rw-rw-r--   0 root         (0) root         (0)     5104 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_referencing_fleet.py
+-rw-rw-r--   0 root         (0) root         (0)     5941 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_region_config.py
+-rw-rw-r--   0 root         (0) root         (0)     4775 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_time.py
+-rw-rw-r--   0 root         (0) root         (0)     5513 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_timeout.py
+-rw-rw-r--   0 root         (0) root         (0)     3741 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_update_server_request.py
+-rw-rw-r--   0 root         (0) root         (0)     5191 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/response_error_response.py
+-rw-rw-r--   0 root         (0) root         (0)     7999 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/time_location.py
+-rw-rw-r--   0 root         (0) root         (0)     4688 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/time_zone.py
+-rw-rw-r--   0 root         (0) root         (0)     5338 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/time_zone_trans.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:44:59.029824 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/
+-rw-rw-r--   0 root         (0) root         (0)      410 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:44:59.029824 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/account/
+-rw-rw-r--   0 root         (0) root         (0)      715 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/account/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     6823 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/account/account_get.py
+-rw-rw-r--   0 root         (0) root         (0)     7829 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/account/admin_account_create.py
+-rw-rw-r--   0 root         (0) root         (0)     6898 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/account/admin_account_get.py
+-rw-rw-r--   0 root         (0) root         (0)     7188 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/account/admin_account_link_token_get.py
+-rw-rw-r--   0 root         (0) root         (0)     8043 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/account/admin_account_link_token_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:44:59.029824 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/ams_info/
+-rw-rw-r--   0 root         (0) root         (0)      583 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/ams_info/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     6623 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/ams_info/info_regions.py
+-rw-rw-r--   0 root         (0) root         (0)     6790 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/ams_info/info_supported_instances.py
+-rw-rw-r--   0 root         (0) root         (0)     4453 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/ams_info/upload_url_get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:44:59.029824 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/ams_qo_s/
+-rw-rw-r--   0 root         (0) root         (0)      537 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/ams_qo_s/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8566 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/ams_qo_s/qo_s_regions_get.py
+-rw-rw-r--   0 root         (0) root         (0)     8934 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/ams_qo_s/qo_s_regions_update.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:44:59.029824 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/artifacts/
+-rw-rw-r--   0 root         (0) root         (0)      767 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/artifacts/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7939 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/artifacts/artifact_delete.py
+-rw-rw-r--   0 root         (0) root         (0)    16985 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/artifacts/artifact_get.py
+-rw-rw-r--   0 root         (0) root         (0)     8071 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/artifacts/artifact_get_url.py
+-rw-rw-r--   0 root         (0) root         (0)     6724 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/artifacts/artifact_usage_get.py
+-rw-rw-r--   0 root         (0) root         (0)     8204 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/artifacts/fleet_artifact_sampling_739743.py
+-rw-rw-r--   0 root         (0) root         (0)     9258 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/artifacts/fleet_artifact_sampling_a22d2b.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:44:59.029824 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/auth/
+-rw-rw-r--   0 root         (0) root         (0)      477 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/auth/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     5321 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/auth/auth_check.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:44:59.029824 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/development/
+-rw-rw-r--   0 root         (0) root         (0)      762 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/development/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8497 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/development/development_server_conf_2194f5.py
+-rw-rw-r--   0 root         (0) root         (0)     8782 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/development/development_server_conf_282185.py
+-rw-rw-r--   0 root         (0) root         (0)     8819 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/development/development_server_conf_7b687b.py
+-rw-rw-r--   0 root         (0) root         (0)     8882 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/development/development_server_conf_a8e4dd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:44:59.029824 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/fleet_commander/
+-rw-rw-r--   0 root         (0) root         (0)      568 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/fleet_commander/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4429 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/fleet_commander/basic_health_check.py
+-rw-rw-r--   0 root         (0) root         (0)     4383 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/fleet_commander/func1.py
+-rw-rw-r--   0 root         (0) root         (0)     4445 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/fleet_commander/portal_health_check.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:44:59.029824 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/fleets/
+-rw-rw-r--   0 root         (0) root         (0)      759 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/fleets/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8942 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/fleets/fleet_claim_by_id.py
+-rw-rw-r--   0 root         (0) root         (0)     8296 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/fleets/fleet_claim_by_keys.py
+-rw-rw-r--   0 root         (0) root         (0)     7948 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/fleets/fleet_create.py
+-rw-rw-r--   0 root         (0) root         (0)     7685 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/fleets/fleet_delete.py
+-rw-rw-r--   0 root         (0) root         (0)     7806 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/fleets/fleet_get.py
+-rw-rw-r--   0 root         (0) root         (0)     6104 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/fleets/fleet_list.py
+-rw-rw-r--   0 root         (0) root         (0)     7902 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/fleets/fleet_servers.py
+-rw-rw-r--   0 root         (0) root         (0)     8836 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/fleets/fleet_update.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:44:59.033824 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/images/
+-rw-rw-r--   0 root         (0) root         (0)      545 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/images/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7569 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/images/image_get.py
+-rw-rw-r--   0 root         (0) root         (0)     6926 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/images/image_list.py
+-rw-rw-r--   0 root         (0) root         (0)     8711 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/images/image_patch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:44:59.033824 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/servers/
+-rw-rw-r--   0 root         (0) root         (0)      653 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/servers/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7939 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/servers/fleet_server_connection_info.py
+-rw-rw-r--   0 root         (0) root         (0)    13566 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/servers/fleet_server_history.py
+-rw-rw-r--   0 root         (0) root         (0)     7754 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/servers/fleet_server_info.py
+-rw-rw-r--   0 root         (0) root         (0)     7756 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/servers/server_history.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:44:59.033824 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/watchdogs/
+-rw-rw-r--   0 root         (0) root         (0)      546 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/watchdogs/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     6576 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/watchdogs/local_watchdog_connect.py
+-rw-rw-r--   0 root         (0) root         (0)     6505 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/watchdogs/watchdog_connect.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:44:59.033824 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/wrappers/
+-rw-rw-r--   0 root         (0) root         (0)     4219 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/wrappers/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    16497 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/wrappers/_account.py
+-rw-rw-r--   0 root         (0) root         (0)     7740 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/wrappers/_ams_info.py
+-rw-rw-r--   0 root         (0) root         (0)     9299 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/wrappers/_ams_qo_s.py
+-rw-rw-r--   0 root         (0) root         (0)    23216 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/wrappers/_artifacts.py
+-rw-rw-r--   0 root         (0) root         (0)     2878 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/wrappers/_auth.py
+-rw-rw-r--   0 root         (0) root         (0)    15713 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/wrappers/_development.py
+-rw-rw-r--   0 root         (0) root         (0)     4481 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/wrappers/_fleet_commander.py
+-rw-rw-r--   0 root         (0) root         (0)    25867 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/wrappers/_fleets.py
+-rw-rw-r--   0 root         (0) root         (0)    10383 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/wrappers/_images.py
+-rw-rw-r--   0 root         (0) root         (0)    15196 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/wrappers/_servers.py
+-rw-rw-r--   0 root         (0) root         (0)     5840 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/wrappers/_watchdogs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:44:59.033824 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk_service_ams.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1065 2024-05-21 03:44:59.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk_service_ams.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7799 2024-05-21 03:44:59.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk_service_ams.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 03:44:59.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk_service_ams.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-21 03:44:59.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk_service_ams.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-05-21 03:44:59.000000 accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk_service_ams.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)      329 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_ams-0.9.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-21 03:44:59.033824 accelbyte_py_sdk_service_ams-0.9.0/setup.cfg
```

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/PKG-INFO` & `accelbyte_py_sdk_service_ams-0.9.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: accelbyte-py-sdk-service-ams
-Version: 0.8.0
+Version: 0.9.0
 Summary: AccelByte Python SDK - Fleet Commander
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: accelbyte-py-sdk-core
 
 [//]: # (Code generated. DO NOT EDIT!)
 
 # AccelByte Modular Python SDK - Service Module
 
 This is a service module for the [AccelByte Modular Python SDK](https://github.com/AccelByte/accelbyte-python-modular-sdk) package.
 
 ```text
 Fleet Commander
-* Version: 1.17.0
+* Version: 1.18.0
 ```
 
 ## Setup
 
 This SDK requires Python 3.9 to be installed.
 
 ### Install with Pip
```

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/README.md` & `accelbyte_py_sdk_service_ams-0.9.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # AccelByte Modular Python SDK - Service Module
 
 This is a service module for the [AccelByte Modular Python SDK](https://github.com/AccelByte/accelbyte-python-modular-sdk) package.
 
 ```text
 Fleet Commander
-* Version: 1.17.0
+* Version: 1.18.0
 ```
 
 ## Setup
 
 This SDK requires Python 3.9 to be installed.
 
 ### Install with Pip
```

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/__init__.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: service-init.j2
 
 """Auto-generated package that contains models used by the Fleet Commander."""
 
-__version__ = "1.17.0"
+__version__ = "1.18.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 # account
 from .wrappers import account_get
```

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/__init__.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: model-init.j2
 
 """Auto-generated package that contains models used by the Fleet Commander."""
 
-__version__ = "1.17.0"
+__version__ = "1.18.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .api_account_create_request import ApiAccountCreateRequest
 from .api_account_create_response import ApiAccountCreateResponse
```

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_account_create_request.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_account_create_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_account_create_response.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_account_create_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_account_limits.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_account_limits.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_account_link_request.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_account_link_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_account_link_response.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_account_link_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_account_link_token_response.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_account_link_token_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_account_response.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_account_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_ams_regions_response.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_ams_regions_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_artifact_list_response.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_artifact_list_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_artifact_response.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_artifact_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_artifact_sampling_rule.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_artifact_sampling_rule.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_artifact_type_sampling_rules.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_artifact_type_sampling_rules.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_artifact_url_response.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_artifact_url_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_artifact_usage_response.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_artifact_usage_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_available_instance_types_response.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_available_instance_types_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_development_server_configuration_create_request.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_development_server_configuration_create_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_development_server_configuration_create_response.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_development_server_configuration_create_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_development_server_configuration_get_response.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_development_server_configuration_get_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_development_server_configuration_list_response.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_development_server_configuration_list_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_ds_history_event.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_ds_history_event.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_ds_history_list.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_ds_history_list.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_ds_host_configuration.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_ds_host_configuration.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_fleet_artifacts_sample_rules.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_fleet_artifacts_sample_rules.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_fleet_claim_by_keys_req.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_fleet_claim_by_keys_req.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_fleet_claim_req.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_fleet_claim_req.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_fleet_claim_response.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_fleet_claim_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_fleet_create_response.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_fleet_create_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_fleet_get_response.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_fleet_get_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_fleet_list_item_response.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_fleet_list_item_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_fleet_list_response.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_fleet_list_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_fleet_parameters.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_fleet_parameters.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_fleet_regional_server_counts.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_fleet_regional_server_counts.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_fleet_server_connection_info_response.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_fleet_server_connection_info_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_fleet_server_history_event_response.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_fleet_server_history_event_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_fleet_server_history_response.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_fleet_server_history_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_fleet_server_info_response.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_fleet_server_info_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_fleet_servers_response.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_fleet_servers_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_image_deployment_profile.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_image_deployment_profile.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_image_details.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_image_details.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_image_list.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_image_list.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_image_list_item.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_image_list_item.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_image_update.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_image_update.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_instance_type_description_response.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_instance_type_description_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_paging_info.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_paging_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_port_configuration.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_port_configuration.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_qo_s_endpoint_response.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_qo_s_endpoint_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_qo_s_server.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_qo_s_server.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_referencing_fleet.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_referencing_fleet.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_region_config.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_region_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_time.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_time.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_timeout.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_timeout.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_update_server_request.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/api_update_server_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/response_error_response.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/response_error_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/time_location.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/time_location.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/time_zone.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/time_zone.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/time_zone_trans.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/models/time_zone_trans.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/account/__init__.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/account/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the Fleet Commander."""
 
-__version__ = "1.17.0"
+__version__ = "1.18.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .account_get import AccountGet
 from .admin_account_create import AdminAccountCreate
```

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/account/account_get.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/account/account_get.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/account/admin_account_create.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/account/admin_account_create.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/account/admin_account_get.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/account/admin_account_get.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/account/admin_account_link_token_get.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/account/admin_account_link_token_get.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/account/admin_account_link_token_post.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/account/admin_account_link_token_post.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/ams_info/__init__.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/images/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the Fleet Commander."""
 
-__version__ = "1.17.0"
+__version__ = "1.18.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
-from .info_regions import InfoRegions
-from .info_supported_instances import InfoSupportedInstances
-from .upload_url_get import UploadURLGet
+from .image_get import ImageGet
+from .image_list import ImageList
+from .image_patch import ImagePatch
```

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/ams_info/info_regions.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/ams_info/info_regions.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/ams_info/info_supported_instances.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/ams_info/info_supported_instances.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/ams_info/upload_url_get.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/ams_info/upload_url_get.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/ams_qo_s/__init__.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/ams_qo_s/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the Fleet Commander."""
 
-__version__ = "1.17.0"
+__version__ = "1.18.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .qo_s_regions_get import QoSRegionsGet
 from .qo_s_regions_update import QoSRegionsUpdate
```

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/ams_qo_s/qo_s_regions_get.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/ams_qo_s/qo_s_regions_get.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/ams_qo_s/qo_s_regions_update.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/ams_qo_s/qo_s_regions_update.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/artifacts/__init__.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/artifacts/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the Fleet Commander."""
 
-__version__ = "1.17.0"
+__version__ = "1.18.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .artifact_delete import ArtifactDelete
 from .artifact_get import ArtifactGet
```

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/artifacts/artifact_delete.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/artifacts/artifact_delete.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/artifacts/artifact_get.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/artifacts/artifact_get.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/artifacts/artifact_get_url.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/artifacts/artifact_get_url.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/artifacts/artifact_usage_get.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/artifacts/artifact_usage_get.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/artifacts/fleet_artifact_sampling_739743.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/artifacts/fleet_artifact_sampling_739743.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/artifacts/fleet_artifact_sampling_a22d2b.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/artifacts/fleet_artifact_sampling_a22d2b.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/auth/auth_check.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/auth/auth_check.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/development/__init__.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/development/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the Fleet Commander."""
 
-__version__ = "1.17.0"
+__version__ = "1.18.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .development_server_conf_a8e4dd import DevelopmentServerConfigurationCreate
 from .development_server_conf_2194f5 import DevelopmentServerConfigurationDelete
```

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/development/development_server_conf_2194f5.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/development/development_server_conf_2194f5.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/development/development_server_conf_282185.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/development/development_server_conf_282185.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/development/development_server_conf_7b687b.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/development/development_server_conf_7b687b.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/development/development_server_conf_a8e4dd.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/development/development_server_conf_a8e4dd.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/fleet_commander/__init__.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/fleet_commander/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the Fleet Commander."""
 
-__version__ = "1.17.0"
+__version__ = "1.18.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .basic_health_check import BasicHealthCheck
 from .func1 import Func1
```

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/fleet_commander/basic_health_check.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/fleet_commander/basic_health_check.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/fleet_commander/func1.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/fleet_commander/func1.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/fleet_commander/portal_health_check.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/fleet_commander/portal_health_check.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/fleets/__init__.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/fleets/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the Fleet Commander."""
 
-__version__ = "1.17.0"
+__version__ = "1.18.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .fleet_claim_by_id import FleetClaimByID
 from .fleet_claim_by_keys import FleetClaimByKeys
```

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/fleets/fleet_claim_by_id.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/fleets/fleet_claim_by_id.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/fleets/fleet_claim_by_keys.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/fleets/fleet_claim_by_keys.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/fleets/fleet_create.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/fleets/fleet_create.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/fleets/fleet_delete.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/fleets/fleet_delete.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/fleets/fleet_get.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/fleets/fleet_get.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/fleets/fleet_list.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/fleets/fleet_list.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/fleets/fleet_servers.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/fleets/fleet_servers.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/fleets/fleet_update.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/fleets/fleet_update.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/images/image_get.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/images/image_get.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/images/image_list.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/images/image_list.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/images/image_patch.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/images/image_patch.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/servers/__init__.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/servers/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the Fleet Commander."""
 
-__version__ = "1.17.0"
+__version__ = "1.18.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .fleet_server_connection_info import FleetServerConnectionInfo
 from .fleet_server_history import FleetServerHistory
```

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/servers/fleet_server_connection_info.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/servers/fleet_server_connection_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/servers/fleet_server_history.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/servers/fleet_server_history.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/servers/fleet_server_info.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/servers/fleet_server_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/servers/server_history.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/servers/server_history.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/watchdogs/__init__.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/watchdogs/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the Fleet Commander."""
 
-__version__ = "1.17.0"
+__version__ = "1.18.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .local_watchdog_connect import LocalWatchdogConnect
 from .watchdog_connect import WatchdogConnect
```

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/watchdogs/local_watchdog_connect.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/watchdogs/local_watchdog_connect.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/watchdogs/watchdog_connect.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/operations/watchdogs/watchdog_connect.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/wrappers/__init__.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/wrappers/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: wrapper-init.j2
 
 """Auto-generated package that contains models used by the Fleet Commander."""
 
-__version__ = "1.17.0"
+__version__ = "1.18.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from ._account import account_get
 from ._account import account_get_async
```

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/wrappers/_account.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/wrappers/_account.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/wrappers/_ams_info.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/wrappers/_ams_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/wrappers/_ams_qo_s.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/wrappers/_ams_qo_s.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/wrappers/_artifacts.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/wrappers/_artifacts.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/wrappers/_auth.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/wrappers/_auth.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/wrappers/_development.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/wrappers/_development.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/wrappers/_fleet_commander.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/wrappers/_fleet_commander.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/wrappers/_fleets.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/wrappers/_fleets.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/wrappers/_images.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/wrappers/_images.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/wrappers/_servers.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/wrappers/_servers.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/wrappers/_watchdogs.py` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk/api/ams/wrappers/_watchdogs.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk_service_ams.egg-info/PKG-INFO` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk_service_ams.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: accelbyte-py-sdk-service-ams
-Version: 0.8.0
+Version: 0.9.0
 Summary: AccelByte Python SDK - Fleet Commander
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: accelbyte-py-sdk-core
 
 [//]: # (Code generated. DO NOT EDIT!)
 
 # AccelByte Modular Python SDK - Service Module
 
 This is a service module for the [AccelByte Modular Python SDK](https://github.com/AccelByte/accelbyte-python-modular-sdk) package.
 
 ```text
 Fleet Commander
-* Version: 1.17.0
+* Version: 1.18.0
 ```
 
 ## Setup
 
 This SDK requires Python 3.9 to be installed.
 
 ### Install with Pip
```

### Comparing `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk_service_ams.egg-info/SOURCES.txt` & `accelbyte_py_sdk_service_ams-0.9.0/accelbyte_py_sdk_service_ams.egg-info/SOURCES.txt`

 * *Files identical despite different names*

