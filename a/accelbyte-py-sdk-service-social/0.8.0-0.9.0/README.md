# Comparing `tmp/accelbyte-py-sdk-service-social-0.8.0.tar.gz` & `tmp/accelbyte-py-sdk-service-social-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accelbyte-py-sdk-service-social-0.8.0.tar", last modified: Tue Feb 27 05:42:43 2024, max compression
+gzip compressed data, was "accelbyte-py-sdk-service-social-0.9.0.tar", last modified: Wed Mar 13 06:15:01 2024, max compression
```

## Comparing `accelbyte-py-sdk-service-social-0.8.0.tar` & `accelbyte-py-sdk-service-social-0.9.0.tar`

### file list

```diff
@@ -1,192 +1,192 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:42:43.127091 accelbyte-py-sdk-service-social-0.8.0/
--rw-r--r--   0 root         (0) root         (0)     1121 2024-02-27 05:42:43.127091 accelbyte-py-sdk-service-social-0.8.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      871 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:42:43.107091 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:42:43.107091 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:42:43.111091 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/
--rw-rw-r--   0 root         (0) root         (0)    10224 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:42:43.115091 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/
--rw-rw-r--   0 root         (0) root         (0)     4409 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5019 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/a_dto_object_for_resetting_user_stat_items.py
--rw-rw-r--   0 root         (0) root         (0)     5424 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/a_dto_object_for_user_stat_item_value.py
--rw-rw-r--   0 root         (0) root         (0)     4225 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/attribute.py
--rw-rw-r--   0 root         (0) root         (0)     3819 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/bulk_cycle_stats_add.py
--rw-rw-r--   0 root         (0) root         (0)     6187 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/bulk_stat_cycle_operation_result.py
--rw-rw-r--   0 root         (0) root         (0)     3849 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/bulk_stat_cycle_request.py
--rw-rw-r--   0 root         (0) root         (0)     3985 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/bulk_stat_cycle_result.py
--rw-rw-r--   0 root         (0) root         (0)     3756 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/bulk_stat_item_create.py
--rw-rw-r--   0 root         (0) root         (0)     4327 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/bulk_stat_item_inc.py
--rw-rw-r--   0 root         (0) root         (0)     3745 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/bulk_stat_item_reset.py
--rw-rw-r--   0 root         (0) root         (0)     6698 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/bulk_stat_item_update.py
--rw-rw-r--   0 root         (0) root         (0)     6095 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/bulk_stat_operation_result.py
--rw-rw-r--   0 root         (0) root         (0)     5006 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/bulk_user_stat_item_inc.py
--rw-rw-r--   0 root         (0) root         (0)     4425 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/bulk_user_stat_item_reset.py
--rw-rw-r--   0 root         (0) root         (0)     8227 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/bulk_user_stat_item_update.py
--rw-rw-r--   0 root         (0) root         (0)     6320 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/error_entity.py
--rw-rw-r--   0 root         (0) root         (0)     7298 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/field_validation_error.py
--rw-rw-r--   0 root         (0) root         (0)     8091 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/game_profile_header.py
--rw-rw-r--   0 root         (0) root         (0)    11424 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/game_profile_info.py
--rw-rw-r--   0 root         (0) root         (0)     6172 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/game_profile_public_info.py
--rw-rw-r--   0 root         (0) root         (0)     9357 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/game_profile_request.py
--rw-rw-r--   0 root         (0) root         (0)     9493 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/global_stat_item_info.py
--rw-rw-r--   0 root         (0) root         (0)     5051 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/global_stat_item_paging_sliced_result.py
--rw-rw-r--   0 root         (0) root         (0)     5443 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/namespace_slot_config_info.py
--rw-rw-r--   0 root         (0) root         (0)     4264 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/paging.py
--rw-rw-r--   0 root         (0) root         (0)     4595 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/slot_config_update.py
--rw-rw-r--   0 root         (0) root         (0)    13117 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/slot_info.py
--rw-rw-r--   0 root         (0) root         (0)     5308 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/slot_metadata_update.py
--rw-rw-r--   0 root         (0) root         (0)    14918 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/stat_create.py
--rw-rw-r--   0 root         (0) root         (0)    10467 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/stat_cycle_create.py
--rw-rw-r--   0 root         (0) root         (0)    15369 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/stat_cycle_info.py
--rw-rw-r--   0 root         (0) root         (0)     4940 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/stat_cycle_paging_sliced_result.py
--rw-rw-r--   0 root         (0) root         (0)    10467 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/stat_cycle_update.py
--rw-rw-r--   0 root         (0) root         (0)     6321 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/stat_import_info.py
--rw-rw-r--   0 root         (0) root         (0)    17431 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/stat_info.py
--rw-rw-r--   0 root         (0) root         (0)     3602 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/stat_item_inc.py
--rw-rw-r--   0 root         (0) root         (0)     3839 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/stat_item_inc_result.py
--rw-rw-r--   0 root         (0) root         (0)     5968 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/stat_item_update.py
--rw-rw-r--   0 root         (0) root         (0)     5853 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/stat_item_value.py
--rw-rw-r--   0 root         (0) root         (0)     4989 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/stat_item_value_paging_sliced_result.py
--rw-rw-r--   0 root         (0) root         (0)     4843 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/stat_paging_sliced_result.py
--rw-rw-r--   0 root         (0) root         (0)     4048 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/stat_reset_info.py
--rw-rw-r--   0 root         (0) root         (0)    10541 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/stat_update.py
--rw-rw-r--   0 root         (0) root         (0)     4946 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/user_game_profiles.py
--rw-rw-r--   0 root         (0) root         (0)     6038 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/user_slot_config_info.py
--rw-rw-r--   0 root         (0) root         (0)    11553 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/user_stat_cycle_item_info.py
--rw-rw-r--   0 root         (0) root         (0)     5135 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/user_stat_cycle_item_paging_sliced_result.py
--rw-rw-r--   0 root         (0) root         (0)     9350 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/user_stat_item_info.py
--rw-rw-r--   0 root         (0) root         (0)     5013 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/user_stat_item_paging_sliced_result.py
--rw-rw-r--   0 root         (0) root         (0)     5626 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/validation_error_entity.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:42:43.115091 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/
--rw-rw-r--   0 root         (0) root         (0)      435 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:42:43.115091 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/game_profile/
--rw-rw-r--   0 root         (0) root         (0)     1021 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/game_profile/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8282 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/game_profile/get_profile.py
--rw-rw-r--   0 root         (0) root         (0)     7280 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/game_profile/get_user_profiles.py
--rw-rw-r--   0 root         (0) root         (0)     8919 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/game_profile/public_create_profile.py
--rw-rw-r--   0 root         (0) root         (0)     8171 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/game_profile/public_delete_profile.py
--rw-rw-r--   0 root         (0) root         (0)     8328 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/game_profile/public_get_profile.py
--rw-rw-r--   0 root         (0) root         (0)     9351 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/game_profile/public_get_profile_attribute.py
--rw-rw-r--   0 root         (0) root         (0)     8004 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/game_profile/public_get_user_game_profiles.py
--rw-rw-r--   0 root         (0) root         (0)     7306 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/game_profile/public_get_user_profiles.py
--rw-rw-r--   0 root         (0) root         (0)    11213 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/game_profile/public_update_attribute.py
--rw-rw-r--   0 root         (0) root         (0)    10116 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/game_profile/public_update_profile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:42:43.115091 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/global_statistic/
--rw-rw-r--   0 root         (0) root         (0)      724 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/global_statistic/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7680 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/global_statistic/get_global_stat_item_by_4617a3.py
--rw-rw-r--   0 root         (0) root         (0)     7675 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/global_statistic/get_global_stat_item_by_f4e6d4.py
--rw-rw-r--   0 root         (0) root         (0)     9111 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/global_statistic/get_global_stat_items.py
--rw-rw-r--   0 root         (0) root         (0)     9118 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/global_statistic/get_global_stat_items_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:42:43.115091 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/slot/
--rw-rw-r--   0 root         (0) root         (0)      995 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/slot/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7466 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/slot/get_slot_data.py
--rw-rw-r--   0 root         (0) root         (0)     6574 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/slot/get_user_namespace_slots.py
--rw-rw-r--   0 root         (0) root         (0)    12042 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/slot/public_create_user_name_1e93c7.py
--rw-rw-r--   0 root         (0) root         (0)     7564 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/slot/public_delete_user_name_9ed44a.py
--rw-rw-r--   0 root         (0) root         (0)     7512 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/slot/public_get_slot_data.py
--rw-rw-r--   0 root         (0) root         (0)     6627 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/slot/public_get_user_namespa_083368.py
--rw-rw-r--   0 root         (0) root         (0)    12773 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/slot/public_update_user_name_d493ff.py
--rw-rw-r--   0 root         (0) root         (0)     8987 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/slot/public_update_user_name_fc60e7.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:42:43.115091 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/slot_config/
--rw-rw-r--   0 root         (0) root         (0)      834 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/slot_config/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5738 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/slot_config/delete_namespace_slot_config.py
--rw-rw-r--   0 root         (0) root         (0)     6542 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/slot_config/delete_user_slot_config.py
--rw-rw-r--   0 root         (0) root         (0)     5934 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/slot_config/get_namespace_slot_config.py
--rw-rw-r--   0 root         (0) root         (0)     6682 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/slot_config/get_user_slot_config.py
--rw-rw-r--   0 root         (0) root         (0)     7027 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/slot_config/update_namespace_slot_config.py
--rw-rw-r--   0 root         (0) root         (0)     7798 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/slot_config/update_user_slot_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:42:43.119091 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/stat_configuration/
--rw-rw-r--   0 root         (0) root         (0)      834 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/stat_configuration/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8711 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/stat_configuration/create_stat.py
--rw-rw-r--   0 root         (0) root         (0)     8724 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/stat_configuration/create_stat_1.py
--rw-rw-r--   0 root         (0) root         (0)     7270 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/stat_configuration/delete_stat.py
--rw-rw-r--   0 root         (0) root         (0)     7754 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/stat_configuration/delete_tied_stat.py
--rw-rw-r--   0 root         (0) root         (0)     6343 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/stat_configuration/export_stats.py
--rw-rw-r--   0 root         (0) root         (0)     7390 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/stat_configuration/get_stat.py
--rw-rw-r--   0 root         (0) root         (0)    10574 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/stat_configuration/get_stats.py
--rw-rw-r--   0 root         (0) root         (0)     8838 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/stat_configuration/import_stats.py
--rw-rw-r--   0 root         (0) root         (0)    10523 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/stat_configuration/query_stats.py
--rw-rw-r--   0 root         (0) root         (0)     8922 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/stat_configuration/update_stat.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:42:43.119091 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/stat_cycle_configuration/
--rw-rw-r--   0 root         (0) root         (0)     1318 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/stat_cycle_configuration/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     9331 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/stat_cycle_configuration/bulk_add_stats.py
--rw-rw-r--   0 root         (0) root         (0)     8169 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/stat_cycle_configuration/bulk_get_stat_cycle.py
--rw-rw-r--   0 root         (0) root         (0)     8174 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/stat_cycle_configuration/bulk_get_stat_cycle_1.py
--rw-rw-r--   0 root         (0) root         (0)     9085 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/stat_cycle_configuration/create_stat_cycle.py
--rw-rw-r--   0 root         (0) root         (0)     7296 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/stat_cycle_configuration/delete_stat_cycle.py
--rw-rw-r--   0 root         (0) root         (0)     6416 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/stat_cycle_configuration/export_stat_cycle.py
--rw-rw-r--   0 root         (0) root         (0)     7428 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/stat_cycle_configuration/get_stat_cycle.py
--rw-rw-r--   0 root         (0) root         (0)     7447 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/stat_cycle_configuration/get_stat_cycle_1.py
--rw-rw-r--   0 root         (0) root         (0)    12195 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/stat_cycle_configuration/get_stat_cycles.py
--rw-rw-r--   0 root         (0) root         (0)    12205 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/stat_cycle_configuration/get_stat_cycles_1.py
--rw-rw-r--   0 root         (0) root         (0)     8919 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/stat_cycle_configuration/import_stat_cycle.py
--rw-rw-r--   0 root         (0) root         (0)     7860 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/stat_cycle_configuration/stop_stat_cycle.py
--rw-rw-r--   0 root         (0) root         (0)     9667 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/stat_cycle_configuration/update_stat_cycle.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:42:43.123091 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/
--rw-rw-r--   0 root         (0) root         (0)     3232 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    11440 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/admin_list_users_stat_items.py
--rw-rw-r--   0 root         (0) root         (0)     9169 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/bulk_create_user_stat_items.py
--rw-rw-r--   0 root         (0) root         (0)     9248 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/bulk_fetch_or_default_s_50dfdc.py
--rw-rw-r--   0 root         (0) root         (0)    10283 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/bulk_fetch_or_default_s_d6fcc5.py
--rw-rw-r--   0 root         (0) root         (0)     8557 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/bulk_fetch_stat_items.py
--rw-rw-r--   0 root         (0) root         (0)     8569 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/bulk_fetch_stat_items_1.py
--rw-rw-r--   0 root         (0) root         (0)     8364 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/bulk_inc_user_stat_item.py
--rw-rw-r--   0 root         (0) root         (0)     9212 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/bulk_inc_user_stat_item_0f5ee3.py
--rw-rw-r--   0 root         (0) root         (0)     9173 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/bulk_inc_user_stat_item_1.py
--rw-rw-r--   0 root         (0) root         (0)     9212 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/bulk_inc_user_stat_item_b0004a.py
--rw-rw-r--   0 root         (0) root         (0)     8398 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/bulk_inc_user_stat_item_value.py
--rw-rw-r--   0 root         (0) root         (0)    10518 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/bulk_reset_user_stat_it_ed9334.py
--rw-rw-r--   0 root         (0) root         (0)     8509 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/bulk_reset_user_stat_item.py
--rw-rw-r--   0 root         (0) root         (0)     9202 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/bulk_reset_user_stat_item_1.py
--rw-rw-r--   0 root         (0) root         (0)     8513 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/bulk_reset_user_stat_item_2.py
--rw-rw-r--   0 root         (0) root         (0)     9206 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/bulk_reset_user_stat_item_3.py
--rw-rw-r--   0 root         (0) root         (0)    10959 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/bulk_update_user_stat_item.py
--rw-rw-r--   0 root         (0) root         (0)     8834 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/bulk_update_user_stat_item_1.py
--rw-rw-r--   0 root         (0) root         (0)    10972 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/bulk_update_user_stat_item_2.py
--rw-rw-r--   0 root         (0) root         (0)     8849 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/bulk_update_user_stat_item_v2.py
--rw-rw-r--   0 root         (0) root         (0)     9089 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/create_user_stat_item.py
--rw-rw-r--   0 root         (0) root         (0)     8744 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/delete_user_stat_items.py
--rw-rw-r--   0 root         (0) root         (0)     8665 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/delete_user_stat_items_1.py
--rw-rw-r--   0 root         (0) root         (0)    10069 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/delete_user_stat_items_2.py
--rw-rw-r--   0 root         (0) root         (0)     9695 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/get_stat_items.py
--rw-rw-r--   0 root         (0) root         (0)    12561 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/get_user_stat_items.py
--rw-rw-r--   0 root         (0) root         (0)    10973 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/inc_user_stat_item_value.py
--rw-rw-r--   0 root         (0) root         (0)     9212 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/public_bulk_create_user_ce1688.py
--rw-rw-r--   0 root         (0) root         (0)     9215 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/public_bulk_inc_user_st_308993.py
--rw-rw-r--   0 root         (0) root         (0)     8460 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/public_bulk_inc_user_st_374b4e.py
--rw-rw-r--   0 root         (0) root         (0)     8412 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/public_bulk_inc_user_stat_item.py
--rw-rw-r--   0 root         (0) root         (0)     9117 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/public_create_user_stat_item.py
--rw-rw-r--   0 root         (0) root         (0)    11025 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/public_inc_user_stat_it_1d89c5.py
--rw-rw-r--   0 root         (0) root         (0)    10981 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/public_inc_user_stat_item.py
--rw-rw-r--   0 root         (0) root         (0)    10354 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/public_list_all_my_stat_items.py
--rw-rw-r--   0 root         (0) root         (0)    11339 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/public_list_my_stat_items.py
--rw-rw-r--   0 root         (0) root         (0)    11813 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/public_query_user_stat_items.py
--rw-rw-r--   0 root         (0) root         (0)    11591 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/public_query_user_stat_items_1.py
--rw-rw-r--   0 root         (0) root         (0)    11613 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/public_query_user_stat_items_2.py
--rw-rw-r--   0 root         (0) root         (0)    11466 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/reset_user_stat_item_value.py
--rw-rw-r--   0 root         (0) root         (0)     9256 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/reset_user_stat_item_value_1.py
--rw-rw-r--   0 root         (0) root         (0)    12570 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/update_user_stat_item_value.py
--rw-rw-r--   0 root         (0) root         (0)    12584 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/update_user_stat_item_value_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:42:43.123091 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic_cycle/
--rw-rw-r--   0 root         (0) root         (0)      664 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic_cycle/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    13082 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic_cycle/get_user_stat_cycle_items.py
--rw-rw-r--   0 root         (0) root         (0)    12228 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic_cycle/get_user_stat_cycle_items_1.py
--rw-rw-r--   0 root         (0) root         (0)    11730 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic_cycle/public_list_my_stat_cyc_a54f9a.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:42:43.123091 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/wrappers/
--rw-rw-r--   0 root         (0) root         (0)    11595 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/wrappers/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    38282 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/wrappers/_game_profile.py
--rw-rw-r--   0 root         (0) root         (0)    15455 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/wrappers/_global_statistic.py
--rw-rw-r--   0 root         (0) root         (0)    29347 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/wrappers/_slot.py
--rw-rw-r--   0 root         (0) root         (0)    18984 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/wrappers/_slot_config.py
--rw-rw-r--   0 root         (0) root         (0)    37529 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/wrappers/_stat_configuration.py
--rw-rw-r--   0 root         (0) root         (0)    50758 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/wrappers/_stat_cycle_configuration.py
--rw-rw-r--   0 root         (0) root         (0)   189464 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/wrappers/_user_statistic.py
--rw-rw-r--   0 root         (0) root         (0)    15748 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/wrappers/_user_statistic_cycle.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:42:43.123091 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk_service_social.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1121 2024-02-27 05:42:43.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk_service_social.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12422 2024-02-27 05:42:43.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk_service_social.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-27 05:42:43.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk_service_social.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       22 2024-02-27 05:42:43.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk_service_social.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-02-27 05:42:43.000000 accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk_service_social.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)      357 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-social-0.8.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-27 05:42:43.127091 accelbyte-py-sdk-service-social-0.8.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:15:01.147940 accelbyte-py-sdk-service-social-0.9.0/
+-rw-r--r--   0 root         (0) root         (0)     1121 2024-03-13 06:15:01.147940 accelbyte-py-sdk-service-social-0.9.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      871 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:15:01.131940 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:15:01.131940 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:15:01.131940 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/
+-rw-rw-r--   0 root         (0) root         (0)    10224 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:15:01.135940 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/
+-rw-rw-r--   0 root         (0) root         (0)     4409 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     5019 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/a_dto_object_for_resetting_user_stat_items.py
+-rw-rw-r--   0 root         (0) root         (0)     5424 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/a_dto_object_for_user_stat_item_value.py
+-rw-rw-r--   0 root         (0) root         (0)     4225 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/attribute.py
+-rw-rw-r--   0 root         (0) root         (0)     3819 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/bulk_cycle_stats_add.py
+-rw-rw-r--   0 root         (0) root         (0)     6187 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/bulk_stat_cycle_operation_result.py
+-rw-rw-r--   0 root         (0) root         (0)     3849 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/bulk_stat_cycle_request.py
+-rw-rw-r--   0 root         (0) root         (0)     3985 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/bulk_stat_cycle_result.py
+-rw-rw-r--   0 root         (0) root         (0)     3756 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/bulk_stat_item_create.py
+-rw-rw-r--   0 root         (0) root         (0)     4327 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/bulk_stat_item_inc.py
+-rw-rw-r--   0 root         (0) root         (0)     3745 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/bulk_stat_item_reset.py
+-rw-rw-r--   0 root         (0) root         (0)     6698 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/bulk_stat_item_update.py
+-rw-rw-r--   0 root         (0) root         (0)     6095 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/bulk_stat_operation_result.py
+-rw-rw-r--   0 root         (0) root         (0)     5006 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/bulk_user_stat_item_inc.py
+-rw-rw-r--   0 root         (0) root         (0)     4425 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/bulk_user_stat_item_reset.py
+-rw-rw-r--   0 root         (0) root         (0)     8227 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/bulk_user_stat_item_update.py
+-rw-rw-r--   0 root         (0) root         (0)     6320 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/error_entity.py
+-rw-rw-r--   0 root         (0) root         (0)     7298 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/field_validation_error.py
+-rw-rw-r--   0 root         (0) root         (0)     8091 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/game_profile_header.py
+-rw-rw-r--   0 root         (0) root         (0)    11424 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/game_profile_info.py
+-rw-rw-r--   0 root         (0) root         (0)     6172 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/game_profile_public_info.py
+-rw-rw-r--   0 root         (0) root         (0)     9357 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/game_profile_request.py
+-rw-rw-r--   0 root         (0) root         (0)     9493 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/global_stat_item_info.py
+-rw-rw-r--   0 root         (0) root         (0)     5051 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/global_stat_item_paging_sliced_result.py
+-rw-rw-r--   0 root         (0) root         (0)     5443 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/namespace_slot_config_info.py
+-rw-rw-r--   0 root         (0) root         (0)     4264 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/paging.py
+-rw-rw-r--   0 root         (0) root         (0)     4595 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/slot_config_update.py
+-rw-rw-r--   0 root         (0) root         (0)    13117 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/slot_info.py
+-rw-rw-r--   0 root         (0) root         (0)     5308 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/slot_metadata_update.py
+-rw-rw-r--   0 root         (0) root         (0)    14918 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/stat_create.py
+-rw-rw-r--   0 root         (0) root         (0)    10467 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/stat_cycle_create.py
+-rw-rw-r--   0 root         (0) root         (0)    15369 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/stat_cycle_info.py
+-rw-rw-r--   0 root         (0) root         (0)     4940 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/stat_cycle_paging_sliced_result.py
+-rw-rw-r--   0 root         (0) root         (0)    10467 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/stat_cycle_update.py
+-rw-rw-r--   0 root         (0) root         (0)     6321 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/stat_import_info.py
+-rw-rw-r--   0 root         (0) root         (0)    17431 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/stat_info.py
+-rw-rw-r--   0 root         (0) root         (0)     3602 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/stat_item_inc.py
+-rw-rw-r--   0 root         (0) root         (0)     3839 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/stat_item_inc_result.py
+-rw-rw-r--   0 root         (0) root         (0)     5968 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/stat_item_update.py
+-rw-rw-r--   0 root         (0) root         (0)     5853 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/stat_item_value.py
+-rw-rw-r--   0 root         (0) root         (0)     4989 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/stat_item_value_paging_sliced_result.py
+-rw-rw-r--   0 root         (0) root         (0)     4843 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/stat_paging_sliced_result.py
+-rw-rw-r--   0 root         (0) root         (0)     4048 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/stat_reset_info.py
+-rw-rw-r--   0 root         (0) root         (0)    10541 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/stat_update.py
+-rw-rw-r--   0 root         (0) root         (0)     4946 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/user_game_profiles.py
+-rw-rw-r--   0 root         (0) root         (0)     6038 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/user_slot_config_info.py
+-rw-rw-r--   0 root         (0) root         (0)    11553 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/user_stat_cycle_item_info.py
+-rw-rw-r--   0 root         (0) root         (0)     5135 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/user_stat_cycle_item_paging_sliced_result.py
+-rw-rw-r--   0 root         (0) root         (0)     9350 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/user_stat_item_info.py
+-rw-rw-r--   0 root         (0) root         (0)     5013 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/user_stat_item_paging_sliced_result.py
+-rw-rw-r--   0 root         (0) root         (0)     5626 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/validation_error_entity.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:15:01.135940 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/
+-rw-rw-r--   0 root         (0) root         (0)      435 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:15:01.135940 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/game_profile/
+-rw-rw-r--   0 root         (0) root         (0)     1021 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/game_profile/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8282 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/game_profile/get_profile.py
+-rw-rw-r--   0 root         (0) root         (0)     7280 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/game_profile/get_user_profiles.py
+-rw-rw-r--   0 root         (0) root         (0)     8919 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/game_profile/public_create_profile.py
+-rw-rw-r--   0 root         (0) root         (0)     8171 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/game_profile/public_delete_profile.py
+-rw-rw-r--   0 root         (0) root         (0)     8328 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/game_profile/public_get_profile.py
+-rw-rw-r--   0 root         (0) root         (0)     9351 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/game_profile/public_get_profile_attribute.py
+-rw-rw-r--   0 root         (0) root         (0)     8004 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/game_profile/public_get_user_game_profiles.py
+-rw-rw-r--   0 root         (0) root         (0)     7306 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/game_profile/public_get_user_profiles.py
+-rw-rw-r--   0 root         (0) root         (0)    11213 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/game_profile/public_update_attribute.py
+-rw-rw-r--   0 root         (0) root         (0)    10116 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/game_profile/public_update_profile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:15:01.135940 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/global_statistic/
+-rw-rw-r--   0 root         (0) root         (0)      724 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/global_statistic/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7680 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/global_statistic/get_global_stat_item_by_4617a3.py
+-rw-rw-r--   0 root         (0) root         (0)     7675 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/global_statistic/get_global_stat_item_by_f4e6d4.py
+-rw-rw-r--   0 root         (0) root         (0)     9111 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/global_statistic/get_global_stat_items.py
+-rw-rw-r--   0 root         (0) root         (0)     9118 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/global_statistic/get_global_stat_items_1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:15:01.135940 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/slot/
+-rw-rw-r--   0 root         (0) root         (0)      995 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/slot/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7466 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/slot/get_slot_data.py
+-rw-rw-r--   0 root         (0) root         (0)     6574 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/slot/get_user_namespace_slots.py
+-rw-rw-r--   0 root         (0) root         (0)    12042 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/slot/public_create_user_name_1e93c7.py
+-rw-rw-r--   0 root         (0) root         (0)     7564 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/slot/public_delete_user_name_9ed44a.py
+-rw-rw-r--   0 root         (0) root         (0)     7512 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/slot/public_get_slot_data.py
+-rw-rw-r--   0 root         (0) root         (0)     6627 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/slot/public_get_user_namespa_083368.py
+-rw-rw-r--   0 root         (0) root         (0)    12773 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/slot/public_update_user_name_d493ff.py
+-rw-rw-r--   0 root         (0) root         (0)     8987 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/slot/public_update_user_name_fc60e7.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:15:01.139940 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/slot_config/
+-rw-rw-r--   0 root         (0) root         (0)      834 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/slot_config/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     5738 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/slot_config/delete_namespace_slot_config.py
+-rw-rw-r--   0 root         (0) root         (0)     6542 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/slot_config/delete_user_slot_config.py
+-rw-rw-r--   0 root         (0) root         (0)     5934 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/slot_config/get_namespace_slot_config.py
+-rw-rw-r--   0 root         (0) root         (0)     6682 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/slot_config/get_user_slot_config.py
+-rw-rw-r--   0 root         (0) root         (0)     7027 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/slot_config/update_namespace_slot_config.py
+-rw-rw-r--   0 root         (0) root         (0)     7798 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/slot_config/update_user_slot_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:15:01.139940 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/stat_configuration/
+-rw-rw-r--   0 root         (0) root         (0)      834 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/stat_configuration/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8711 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/stat_configuration/create_stat.py
+-rw-rw-r--   0 root         (0) root         (0)     8724 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/stat_configuration/create_stat_1.py
+-rw-rw-r--   0 root         (0) root         (0)     7270 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/stat_configuration/delete_stat.py
+-rw-rw-r--   0 root         (0) root         (0)     7754 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/stat_configuration/delete_tied_stat.py
+-rw-rw-r--   0 root         (0) root         (0)     6343 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/stat_configuration/export_stats.py
+-rw-rw-r--   0 root         (0) root         (0)     7390 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/stat_configuration/get_stat.py
+-rw-rw-r--   0 root         (0) root         (0)    10574 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/stat_configuration/get_stats.py
+-rw-rw-r--   0 root         (0) root         (0)     8838 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/stat_configuration/import_stats.py
+-rw-rw-r--   0 root         (0) root         (0)    10523 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/stat_configuration/query_stats.py
+-rw-rw-r--   0 root         (0) root         (0)     8922 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/stat_configuration/update_stat.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:15:01.139940 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/stat_cycle_configuration/
+-rw-rw-r--   0 root         (0) root         (0)     1318 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/stat_cycle_configuration/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     9331 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/stat_cycle_configuration/bulk_add_stats.py
+-rw-rw-r--   0 root         (0) root         (0)     8169 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/stat_cycle_configuration/bulk_get_stat_cycle.py
+-rw-rw-r--   0 root         (0) root         (0)     8174 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/stat_cycle_configuration/bulk_get_stat_cycle_1.py
+-rw-rw-r--   0 root         (0) root         (0)     9085 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/stat_cycle_configuration/create_stat_cycle.py
+-rw-rw-r--   0 root         (0) root         (0)     7296 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/stat_cycle_configuration/delete_stat_cycle.py
+-rw-rw-r--   0 root         (0) root         (0)     6416 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/stat_cycle_configuration/export_stat_cycle.py
+-rw-rw-r--   0 root         (0) root         (0)     7428 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/stat_cycle_configuration/get_stat_cycle.py
+-rw-rw-r--   0 root         (0) root         (0)     7447 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/stat_cycle_configuration/get_stat_cycle_1.py
+-rw-rw-r--   0 root         (0) root         (0)    12195 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/stat_cycle_configuration/get_stat_cycles.py
+-rw-rw-r--   0 root         (0) root         (0)    12205 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/stat_cycle_configuration/get_stat_cycles_1.py
+-rw-rw-r--   0 root         (0) root         (0)     8919 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/stat_cycle_configuration/import_stat_cycle.py
+-rw-rw-r--   0 root         (0) root         (0)     7860 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/stat_cycle_configuration/stop_stat_cycle.py
+-rw-rw-r--   0 root         (0) root         (0)     9667 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/stat_cycle_configuration/update_stat_cycle.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:15:01.143940 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/
+-rw-rw-r--   0 root         (0) root         (0)     3232 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    11440 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/admin_list_users_stat_items.py
+-rw-rw-r--   0 root         (0) root         (0)     9169 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/bulk_create_user_stat_items.py
+-rw-rw-r--   0 root         (0) root         (0)     9248 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/bulk_fetch_or_default_s_50dfdc.py
+-rw-rw-r--   0 root         (0) root         (0)    10283 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/bulk_fetch_or_default_s_d6fcc5.py
+-rw-rw-r--   0 root         (0) root         (0)     8557 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/bulk_fetch_stat_items.py
+-rw-rw-r--   0 root         (0) root         (0)     8569 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/bulk_fetch_stat_items_1.py
+-rw-rw-r--   0 root         (0) root         (0)     8364 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/bulk_inc_user_stat_item.py
+-rw-rw-r--   0 root         (0) root         (0)     9212 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/bulk_inc_user_stat_item_0f5ee3.py
+-rw-rw-r--   0 root         (0) root         (0)     9173 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/bulk_inc_user_stat_item_1.py
+-rw-rw-r--   0 root         (0) root         (0)     9212 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/bulk_inc_user_stat_item_b0004a.py
+-rw-rw-r--   0 root         (0) root         (0)     8398 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/bulk_inc_user_stat_item_value.py
+-rw-rw-r--   0 root         (0) root         (0)    10518 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/bulk_reset_user_stat_it_ed9334.py
+-rw-rw-r--   0 root         (0) root         (0)     8509 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/bulk_reset_user_stat_item.py
+-rw-rw-r--   0 root         (0) root         (0)     9202 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/bulk_reset_user_stat_item_1.py
+-rw-rw-r--   0 root         (0) root         (0)     8513 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/bulk_reset_user_stat_item_2.py
+-rw-rw-r--   0 root         (0) root         (0)     9206 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/bulk_reset_user_stat_item_3.py
+-rw-rw-r--   0 root         (0) root         (0)    10959 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/bulk_update_user_stat_item.py
+-rw-rw-r--   0 root         (0) root         (0)     8834 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/bulk_update_user_stat_item_1.py
+-rw-rw-r--   0 root         (0) root         (0)    10972 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/bulk_update_user_stat_item_2.py
+-rw-rw-r--   0 root         (0) root         (0)     8849 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/bulk_update_user_stat_item_v2.py
+-rw-rw-r--   0 root         (0) root         (0)     9089 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/create_user_stat_item.py
+-rw-rw-r--   0 root         (0) root         (0)     8744 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/delete_user_stat_items.py
+-rw-rw-r--   0 root         (0) root         (0)     8665 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/delete_user_stat_items_1.py
+-rw-rw-r--   0 root         (0) root         (0)    10069 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/delete_user_stat_items_2.py
+-rw-rw-r--   0 root         (0) root         (0)     9695 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/get_stat_items.py
+-rw-rw-r--   0 root         (0) root         (0)    12561 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/get_user_stat_items.py
+-rw-rw-r--   0 root         (0) root         (0)    10973 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/inc_user_stat_item_value.py
+-rw-rw-r--   0 root         (0) root         (0)     9212 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/public_bulk_create_user_ce1688.py
+-rw-rw-r--   0 root         (0) root         (0)     9215 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/public_bulk_inc_user_st_308993.py
+-rw-rw-r--   0 root         (0) root         (0)     8460 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/public_bulk_inc_user_st_374b4e.py
+-rw-rw-r--   0 root         (0) root         (0)     8412 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/public_bulk_inc_user_stat_item.py
+-rw-rw-r--   0 root         (0) root         (0)     9117 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/public_create_user_stat_item.py
+-rw-rw-r--   0 root         (0) root         (0)    11025 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/public_inc_user_stat_it_1d89c5.py
+-rw-rw-r--   0 root         (0) root         (0)    10981 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/public_inc_user_stat_item.py
+-rw-rw-r--   0 root         (0) root         (0)    10354 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/public_list_all_my_stat_items.py
+-rw-rw-r--   0 root         (0) root         (0)    11339 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/public_list_my_stat_items.py
+-rw-rw-r--   0 root         (0) root         (0)    11813 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/public_query_user_stat_items.py
+-rw-rw-r--   0 root         (0) root         (0)    11591 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/public_query_user_stat_items_1.py
+-rw-rw-r--   0 root         (0) root         (0)    11613 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/public_query_user_stat_items_2.py
+-rw-rw-r--   0 root         (0) root         (0)    11466 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/reset_user_stat_item_value.py
+-rw-rw-r--   0 root         (0) root         (0)     9256 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/reset_user_stat_item_value_1.py
+-rw-rw-r--   0 root         (0) root         (0)    12570 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/update_user_stat_item_value.py
+-rw-rw-r--   0 root         (0) root         (0)    12584 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/update_user_stat_item_value_1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:15:01.143940 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic_cycle/
+-rw-rw-r--   0 root         (0) root         (0)      664 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic_cycle/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    13082 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic_cycle/get_user_stat_cycle_items.py
+-rw-rw-r--   0 root         (0) root         (0)    12228 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic_cycle/get_user_stat_cycle_items_1.py
+-rw-rw-r--   0 root         (0) root         (0)    11730 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic_cycle/public_list_my_stat_cyc_a54f9a.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:15:01.143940 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/wrappers/
+-rw-rw-r--   0 root         (0) root         (0)    11595 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/wrappers/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    38282 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/wrappers/_game_profile.py
+-rw-rw-r--   0 root         (0) root         (0)    15455 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/wrappers/_global_statistic.py
+-rw-rw-r--   0 root         (0) root         (0)    29347 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/wrappers/_slot.py
+-rw-rw-r--   0 root         (0) root         (0)    18984 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/wrappers/_slot_config.py
+-rw-rw-r--   0 root         (0) root         (0)    37529 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/wrappers/_stat_configuration.py
+-rw-rw-r--   0 root         (0) root         (0)    50758 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/wrappers/_stat_cycle_configuration.py
+-rw-rw-r--   0 root         (0) root         (0)   189464 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/wrappers/_user_statistic.py
+-rw-rw-r--   0 root         (0) root         (0)    15748 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/wrappers/_user_statistic_cycle.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:15:01.147940 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk_service_social.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1121 2024-03-13 06:15:01.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk_service_social.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    12422 2024-03-13 06:15:01.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk_service_social.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-03-13 06:15:01.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk_service_social.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-03-13 06:15:01.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk_service_social.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-03-13 06:15:01.000000 accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk_service_social.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)      357 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-social-0.9.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-03-13 06:15:01.147940 accelbyte-py-sdk-service-social-0.9.0/setup.cfg
```

### Comparing `accelbyte-py-sdk-service-social-0.8.0/PKG-INFO` & `accelbyte-py-sdk-service-social-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: accelbyte-py-sdk-service-social
-Version: 0.8.0
+Version: 0.9.0
 Summary: AccelByte Python SDK - AccelByte Gaming Services Social Service
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: accelbyte-py-sdk-core
 
 [//]: # (Code generated. DO NOT EDIT!)
 
 # AccelByte Modular Python SDK - Service Module
 
 This is a service module for the [AccelByte Modular Python SDK](https://github.com/AccelByte/accelbyte-python-modular-sdk) package.
 
 ```text
 AccelByte Gaming Services Social Service
-* Version: 2.12.0
+* Version: 2.12.2
 ```
 
 ## Setup
 
 This SDK requires Python 3.9 to be installed.
 
 ### Install with Pip
```

### Comparing `accelbyte-py-sdk-service-social-0.8.0/README.md` & `accelbyte-py-sdk-service-social-0.9.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # AccelByte Modular Python SDK - Service Module
 
 This is a service module for the [AccelByte Modular Python SDK](https://github.com/AccelByte/accelbyte-python-modular-sdk) package.
 
 ```text
 AccelByte Gaming Services Social Service
-* Version: 2.12.0
+* Version: 2.12.2
 ```
 
 ## Setup
 
 This SDK requires Python 3.9 to be installed.
 
 ### Install with Pip
```

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/__init__.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: service-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Social Service."""
 
-__version__ = "2.12.0"
+__version__ = "2.12.2"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 # game_profile
 from .wrappers import get_profile
```

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/__init__.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: model-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Social Service."""
 
-__version__ = "2.12.0"
+__version__ = "2.12.2"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .a_dto_object_for_resetting_user_stat_items import (
     ADTOObjectForResettingUserStatItems,
```

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/a_dto_object_for_resetting_user_stat_items.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/a_dto_object_for_resetting_user_stat_items.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/a_dto_object_for_user_stat_item_value.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/a_dto_object_for_user_stat_item_value.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/attribute.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/attribute.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/bulk_cycle_stats_add.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/bulk_cycle_stats_add.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/bulk_stat_cycle_operation_result.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/bulk_stat_cycle_operation_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/bulk_stat_cycle_request.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/bulk_stat_cycle_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/bulk_stat_cycle_result.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/bulk_stat_cycle_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/bulk_stat_item_create.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/bulk_stat_item_create.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/bulk_stat_item_inc.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/bulk_stat_item_inc.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/bulk_stat_item_reset.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/bulk_stat_item_reset.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/bulk_stat_item_update.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/bulk_stat_item_update.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/bulk_stat_operation_result.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/bulk_stat_operation_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/bulk_user_stat_item_inc.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/bulk_user_stat_item_inc.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/bulk_user_stat_item_reset.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/bulk_user_stat_item_reset.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/bulk_user_stat_item_update.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/bulk_user_stat_item_update.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/error_entity.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/error_entity.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/field_validation_error.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/field_validation_error.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/game_profile_header.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/game_profile_header.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/game_profile_info.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/game_profile_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/game_profile_public_info.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/game_profile_public_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/game_profile_request.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/game_profile_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/global_stat_item_info.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/global_stat_item_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/global_stat_item_paging_sliced_result.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/global_stat_item_paging_sliced_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/namespace_slot_config_info.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/namespace_slot_config_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/paging.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/paging.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/slot_config_update.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/slot_config_update.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/slot_info.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/slot_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/slot_metadata_update.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/slot_metadata_update.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/stat_create.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/stat_create.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/stat_cycle_create.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/stat_cycle_create.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/stat_cycle_info.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/stat_cycle_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/stat_cycle_paging_sliced_result.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/stat_cycle_paging_sliced_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/stat_cycle_update.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/stat_cycle_update.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/stat_import_info.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/stat_import_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/stat_info.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/stat_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/stat_item_inc.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/stat_item_inc.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/stat_item_inc_result.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/stat_item_inc_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/stat_item_update.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/stat_item_update.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/stat_item_value.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/stat_item_value.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/stat_item_value_paging_sliced_result.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/stat_item_value_paging_sliced_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/stat_paging_sliced_result.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/stat_paging_sliced_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/stat_reset_info.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/stat_reset_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/stat_update.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/stat_update.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/user_game_profiles.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/user_game_profiles.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/user_slot_config_info.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/user_slot_config_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/user_stat_cycle_item_info.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/user_stat_cycle_item_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/user_stat_cycle_item_paging_sliced_result.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/user_stat_cycle_item_paging_sliced_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/user_stat_item_info.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/user_stat_item_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/user_stat_item_paging_sliced_result.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/user_stat_item_paging_sliced_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/models/validation_error_entity.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/models/validation_error_entity.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/game_profile/__init__.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/game_profile/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Social Service."""
 
-__version__ = "2.12.0"
+__version__ = "2.12.2"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .get_profile import GetProfile
 from .get_user_profiles import GetUserProfiles
```

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/game_profile/get_profile.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/game_profile/get_profile.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/game_profile/get_user_profiles.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/game_profile/get_user_profiles.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/game_profile/public_create_profile.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/game_profile/public_create_profile.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/game_profile/public_delete_profile.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/game_profile/public_delete_profile.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/game_profile/public_get_profile.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/game_profile/public_get_profile.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/game_profile/public_get_profile_attribute.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/game_profile/public_get_profile_attribute.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/game_profile/public_get_user_game_profiles.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/game_profile/public_get_user_game_profiles.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/game_profile/public_get_user_profiles.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/game_profile/public_get_user_profiles.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/game_profile/public_update_attribute.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/game_profile/public_update_attribute.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/game_profile/public_update_profile.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/game_profile/public_update_profile.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/global_statistic/__init__.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/global_statistic/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Social Service."""
 
-__version__ = "2.12.0"
+__version__ = "2.12.2"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .get_global_stat_item_by_f4e6d4 import GetGlobalStatItemByStatCode
 from .get_global_stat_item_by_4617a3 import GetGlobalStatItemByStatCode1
```

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/global_statistic/get_global_stat_item_by_4617a3.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/global_statistic/get_global_stat_item_by_4617a3.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/global_statistic/get_global_stat_item_by_f4e6d4.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/global_statistic/get_global_stat_item_by_f4e6d4.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/global_statistic/get_global_stat_items.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/global_statistic/get_global_stat_items.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/global_statistic/get_global_stat_items_1.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/global_statistic/get_global_stat_items_1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/slot/__init__.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/slot/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Social Service."""
 
-__version__ = "2.12.0"
+__version__ = "2.12.2"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .get_slot_data import GetSlotData
 from .get_user_namespace_slots import GetUserNamespaceSlots
```

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/slot/get_slot_data.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/slot/get_slot_data.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/slot/get_user_namespace_slots.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/slot/get_user_namespace_slots.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/slot/public_create_user_name_1e93c7.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/slot/public_create_user_name_1e93c7.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/slot/public_delete_user_name_9ed44a.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/slot/public_delete_user_name_9ed44a.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/slot/public_get_slot_data.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/slot/public_get_slot_data.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/slot/public_get_user_namespa_083368.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/slot/public_get_user_namespa_083368.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/slot/public_update_user_name_d493ff.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/slot/public_update_user_name_d493ff.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/slot/public_update_user_name_fc60e7.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/slot/public_update_user_name_fc60e7.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/slot_config/__init__.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/slot_config/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Social Service."""
 
-__version__ = "2.12.0"
+__version__ = "2.12.2"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .delete_namespace_slot_config import DeleteNamespaceSlotConfig
 from .delete_user_slot_config import DeleteUserSlotConfig
```

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/slot_config/delete_namespace_slot_config.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/slot_config/delete_namespace_slot_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/slot_config/delete_user_slot_config.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/slot_config/delete_user_slot_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/slot_config/get_namespace_slot_config.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/slot_config/get_namespace_slot_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/slot_config/get_user_slot_config.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/slot_config/get_user_slot_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/slot_config/update_namespace_slot_config.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/slot_config/update_namespace_slot_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/slot_config/update_user_slot_config.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/slot_config/update_user_slot_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/stat_configuration/__init__.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/stat_configuration/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Social Service."""
 
-__version__ = "2.12.0"
+__version__ = "2.12.2"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .create_stat import CreateStat
 from .create_stat_1 import CreateStat1
```

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/stat_configuration/create_stat.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/stat_configuration/create_stat.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/stat_configuration/create_stat_1.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/stat_configuration/create_stat_1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/stat_configuration/delete_stat.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/stat_configuration/delete_stat.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/stat_configuration/delete_tied_stat.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/stat_configuration/delete_tied_stat.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/stat_configuration/export_stats.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/stat_configuration/export_stats.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/stat_configuration/get_stat.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/stat_configuration/get_stat.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/stat_configuration/get_stats.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/stat_configuration/get_stats.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/stat_configuration/import_stats.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/stat_configuration/import_stats.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/stat_configuration/query_stats.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/stat_configuration/query_stats.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/stat_configuration/update_stat.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/stat_configuration/update_stat.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/stat_cycle_configuration/__init__.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/stat_cycle_configuration/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Social Service."""
 
-__version__ = "2.12.0"
+__version__ = "2.12.2"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .bulk_add_stats import BulkAddStats
 from .bulk_get_stat_cycle import BulkGetStatCycle
```

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/stat_cycle_configuration/bulk_add_stats.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/stat_cycle_configuration/bulk_add_stats.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/stat_cycle_configuration/bulk_get_stat_cycle.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/stat_cycle_configuration/bulk_get_stat_cycle.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/stat_cycle_configuration/bulk_get_stat_cycle_1.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/stat_cycle_configuration/bulk_get_stat_cycle_1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/stat_cycle_configuration/create_stat_cycle.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/stat_cycle_configuration/create_stat_cycle.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/stat_cycle_configuration/delete_stat_cycle.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/stat_cycle_configuration/delete_stat_cycle.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/stat_cycle_configuration/export_stat_cycle.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/stat_cycle_configuration/export_stat_cycle.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/stat_cycle_configuration/get_stat_cycle.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/stat_cycle_configuration/get_stat_cycle.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/stat_cycle_configuration/get_stat_cycle_1.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/stat_cycle_configuration/get_stat_cycle_1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/stat_cycle_configuration/get_stat_cycles.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/stat_cycle_configuration/get_stat_cycles.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/stat_cycle_configuration/get_stat_cycles_1.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/stat_cycle_configuration/get_stat_cycles_1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/stat_cycle_configuration/import_stat_cycle.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/stat_cycle_configuration/import_stat_cycle.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/stat_cycle_configuration/stop_stat_cycle.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/stat_cycle_configuration/stop_stat_cycle.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/stat_cycle_configuration/update_stat_cycle.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/stat_cycle_configuration/update_stat_cycle.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/__init__.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Social Service."""
 
-__version__ = "2.12.0"
+__version__ = "2.12.2"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .admin_list_users_stat_items import AdminListUsersStatItems
 from .bulk_create_user_stat_items import BulkCreateUserStatItems
```

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/admin_list_users_stat_items.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/admin_list_users_stat_items.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/bulk_create_user_stat_items.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/bulk_create_user_stat_items.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/bulk_fetch_or_default_s_50dfdc.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/bulk_fetch_or_default_s_50dfdc.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/bulk_fetch_or_default_s_d6fcc5.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/bulk_fetch_or_default_s_d6fcc5.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/bulk_fetch_stat_items.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/bulk_fetch_stat_items.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/bulk_fetch_stat_items_1.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/bulk_fetch_stat_items_1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/bulk_inc_user_stat_item.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/bulk_inc_user_stat_item.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/bulk_inc_user_stat_item_0f5ee3.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/bulk_inc_user_stat_item_0f5ee3.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/bulk_inc_user_stat_item_1.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/bulk_inc_user_stat_item_1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/bulk_inc_user_stat_item_b0004a.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/bulk_inc_user_stat_item_b0004a.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/bulk_inc_user_stat_item_value.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/bulk_inc_user_stat_item_value.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/bulk_reset_user_stat_it_ed9334.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/bulk_reset_user_stat_it_ed9334.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/bulk_reset_user_stat_item.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/bulk_reset_user_stat_item.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/bulk_reset_user_stat_item_1.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/bulk_reset_user_stat_item_1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/bulk_reset_user_stat_item_2.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/bulk_reset_user_stat_item_2.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/bulk_reset_user_stat_item_3.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/bulk_reset_user_stat_item_3.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/bulk_update_user_stat_item.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/bulk_update_user_stat_item.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/bulk_update_user_stat_item_1.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/bulk_update_user_stat_item_1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/bulk_update_user_stat_item_2.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/bulk_update_user_stat_item_2.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/bulk_update_user_stat_item_v2.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/bulk_update_user_stat_item_v2.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/create_user_stat_item.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/create_user_stat_item.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/delete_user_stat_items.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/delete_user_stat_items.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/delete_user_stat_items_1.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/delete_user_stat_items_1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/delete_user_stat_items_2.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/delete_user_stat_items_2.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/get_stat_items.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/get_stat_items.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/get_user_stat_items.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/get_user_stat_items.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/inc_user_stat_item_value.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/inc_user_stat_item_value.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/public_bulk_create_user_ce1688.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/public_bulk_create_user_ce1688.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/public_bulk_inc_user_st_308993.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/public_bulk_inc_user_st_308993.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/public_bulk_inc_user_st_374b4e.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/public_bulk_inc_user_st_374b4e.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/public_bulk_inc_user_stat_item.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/public_bulk_inc_user_stat_item.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/public_create_user_stat_item.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/public_create_user_stat_item.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/public_inc_user_stat_it_1d89c5.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/public_inc_user_stat_it_1d89c5.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/public_inc_user_stat_item.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/public_inc_user_stat_item.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/public_list_all_my_stat_items.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/public_list_all_my_stat_items.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/public_list_my_stat_items.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/public_list_my_stat_items.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/public_query_user_stat_items.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/public_query_user_stat_items.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/public_query_user_stat_items_1.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/public_query_user_stat_items_1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/public_query_user_stat_items_2.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/public_query_user_stat_items_2.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/reset_user_stat_item_value.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/reset_user_stat_item_value.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/reset_user_stat_item_value_1.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/reset_user_stat_item_value_1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/update_user_stat_item_value.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/update_user_stat_item_value.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic/update_user_stat_item_value_1.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic/update_user_stat_item_value_1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic_cycle/__init__.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic_cycle/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Social Service."""
 
-__version__ = "2.12.0"
+__version__ = "2.12.2"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .get_user_stat_cycle_items import GetUserStatCycleItems
 from .get_user_stat_cycle_items_1 import GetUserStatCycleItems1
```

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic_cycle/get_user_stat_cycle_items.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic_cycle/get_user_stat_cycle_items.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic_cycle/get_user_stat_cycle_items_1.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic_cycle/get_user_stat_cycle_items_1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/operations/user_statistic_cycle/public_list_my_stat_cyc_a54f9a.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/operations/user_statistic_cycle/public_list_my_stat_cyc_a54f9a.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/wrappers/__init__.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/wrappers/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: wrapper-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Social Service."""
 
-__version__ = "2.12.0"
+__version__ = "2.12.2"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from ._game_profile import get_profile
 from ._game_profile import get_profile_async
```

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/wrappers/_game_profile.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/wrappers/_game_profile.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/wrappers/_global_statistic.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/wrappers/_global_statistic.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/wrappers/_slot.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/wrappers/_slot.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/wrappers/_slot_config.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/wrappers/_slot_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/wrappers/_stat_configuration.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/wrappers/_stat_configuration.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/wrappers/_stat_cycle_configuration.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/wrappers/_stat_cycle_configuration.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/wrappers/_user_statistic.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/wrappers/_user_statistic.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk/api/social/wrappers/_user_statistic_cycle.py` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk/api/social/wrappers/_user_statistic_cycle.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk_service_social.egg-info/PKG-INFO` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk_service_social.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: accelbyte-py-sdk-service-social
-Version: 0.8.0
+Version: 0.9.0
 Summary: AccelByte Python SDK - AccelByte Gaming Services Social Service
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: accelbyte-py-sdk-core
 
 [//]: # (Code generated. DO NOT EDIT!)
 
 # AccelByte Modular Python SDK - Service Module
 
 This is a service module for the [AccelByte Modular Python SDK](https://github.com/AccelByte/accelbyte-python-modular-sdk) package.
 
 ```text
 AccelByte Gaming Services Social Service
-* Version: 2.12.0
+* Version: 2.12.2
 ```
 
 ## Setup
 
 This SDK requires Python 3.9 to be installed.
 
 ### Install with Pip
```

### Comparing `accelbyte-py-sdk-service-social-0.8.0/accelbyte_py_sdk_service_social.egg-info/SOURCES.txt` & `accelbyte-py-sdk-service-social-0.9.0/accelbyte_py_sdk_service_social.egg-info/SOURCES.txt`

 * *Files identical despite different names*

