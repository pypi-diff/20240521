# Comparing `tmp/accelbyte-py-sdk-service-group-0.8.0.tar.gz` & `tmp/accelbyte-py-sdk-service-group-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accelbyte-py-sdk-service-group-0.8.0.tar", last modified: Tue Feb 27 05:38:02 2024, max compression
+gzip compressed data, was "accelbyte-py-sdk-service-group-0.9.0.tar", last modified: Tue Mar 26 05:42:15 2024, max compression
```

## Comparing `accelbyte-py-sdk-service-group-0.8.0.tar` & `accelbyte-py-sdk-service-group-0.9.0.tar`

### file list

```diff
@@ -1,154 +1,154 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:38:02.827051 accelbyte-py-sdk-service-group-0.8.0/
--rw-r--r--   0 root         (0) root         (0)     1117 2024-02-27 05:38:02.827051 accelbyte-py-sdk-service-group-0.8.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      869 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:38:02.811051 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:38:02.811051 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:38:02.811051 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/
--rw-rw-r--   0 root         (0) root         (0)     8863 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:38:02.815051 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/
--rw-rw-r--   0 root         (0) root         (0)     4719 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3901 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_assign_role_to_member_request_v1.py
--rw-rw-r--   0 root         (0) root         (0)     4612 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_cancel_invitation_group_response_v2.py
--rw-rw-r--   0 root         (0) root         (0)    10023 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_create_group_configuration_request_v1.py
--rw-rw-r--   0 root         (0) root         (0)    10113 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_create_group_configuration_response_v1.py
--rw-rw-r--   0 root         (0) root         (0)     5454 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_create_member_role_request_v1.py
--rw-rw-r--   0 root         (0) root         (0)    10735 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_get_group_configuration_response_v1.py
--rw-rw-r--   0 root         (0) root         (0)     3940 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_get_group_list_request_v2.py
--rw-rw-r--   0 root         (0) root         (0)     5350 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_get_group_member_list_response_v1.py
--rw-rw-r--   0 root         (0) root         (0)     5074 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_get_groups_list_response_v1.py
--rw-rw-r--   0 root         (0) root         (0)     4154 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_get_groups_response_v1.py
--rw-rw-r--   0 root         (0) root         (0)     5305 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_get_member_requests_list_response_v1.py
--rw-rw-r--   0 root         (0) root         (0)     5223 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_get_member_roles_list_response_v1.py
--rw-rw-r--   0 root         (0) root         (0)     6875 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_get_user_group_information_response_v1.py
--rw-rw-r--   0 root         (0) root         (0)     4518 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_group_member.py
--rw-rw-r--   0 root         (0) root         (0)    13350 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_group_response_v1.py
--rw-rw-r--   0 root         (0) root         (0)     5618 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_group_rule.py
--rw-rw-r--   0 root         (0) root         (0)     3925 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_group_rule_group_custom_rule.py
--rw-rw-r--   0 root         (0) root         (0)     5958 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_group_rule_response_v1.py
--rw-rw-r--   0 root         (0) root         (0)     4027 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_group_rule_response_v1_group_custom_rule.py
--rw-rw-r--   0 root         (0) root         (0)     5077 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_join_group_response_v1.py
--rw-rw-r--   0 root         (0) root         (0)     4672 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_kick_group_member_response_v1.py
--rw-rw-r--   0 root         (0) root         (0)     4479 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_leave_group_response_v1.py
--rw-rw-r--   0 root         (0) root         (0)     5307 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_list_configuration_response_v1.py
--rw-rw-r--   0 root         (0) root         (0)     4576 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_member_request_group_response_v1.py
--rw-rw-r--   0 root         (0) root         (0)     5241 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_member_request_response_v1.py
--rw-rw-r--   0 root         (0) root         (0)     6156 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_member_role_response_v1.py
--rw-rw-r--   0 root         (0) root         (0)     5434 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_pagination.py
--rw-rw-r--   0 root         (0) root         (0)    11126 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_public_create_new_group_request_v1.py
--rw-rw-r--   0 root         (0) root         (0)     3923 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_remove_role_from_member_request_v1.py
--rw-rw-r--   0 root         (0) root         (0)     4477 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_role_permission.py
--rw-rw-r--   0 root         (0) root         (0)     4805 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_rule.py
--rw-rw-r--   0 root         (0) root         (0)     5852 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_rule_information.py
--rw-rw-r--   0 root         (0) root         (0)     4986 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_rule_response_v1.py
--rw-rw-r--   0 root         (0) root         (0)     4563 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_update_group_configuration_global_rules_request_v1.py
--rw-rw-r--   0 root         (0) root         (0)     5472 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_update_group_configuration_request_v1.py
--rw-rw-r--   0 root         (0) root         (0)    10113 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_update_group_configuration_response_v1.py
--rw-rw-r--   0 root         (0) root         (0)     4394 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_update_group_custom_attributes_request_v1.py
--rw-rw-r--   0 root         (0) root         (0)     4320 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_update_group_custom_rule_request_v1.py
--rw-rw-r--   0 root         (0) root         (0)     4452 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_update_group_predefined_rule_request_v1.py
--rw-rw-r--   0 root         (0) root         (0)     8722 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_update_group_request_v1.py
--rw-rw-r--   0 root         (0) root         (0)     4046 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_update_group_request_v1_custom_attributes.py
--rw-rw-r--   0 root         (0) root         (0)     4751 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_update_member_role_permissions_request_v1.py
--rw-rw-r--   0 root         (0) root         (0)     4050 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_update_member_role_request_v1.py
--rw-rw-r--   0 root         (0) root         (0)     4527 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_user_invitation_response_v1.py
--rw-rw-r--   0 root         (0) root         (0)     4575 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/response_error_response.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:38:02.815051 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/
--rw-rw-r--   0 root         (0) root         (0)      434 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:38:02.819051 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/configuration/
--rw-rw-r--   0 root         (0) root         (0)     1086 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/configuration/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     9306 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/configuration/create_group_configurat_f2dcd2.py
--rw-rw-r--   0 root         (0) root         (0)     9677 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/configuration/delete_group_configurat_db1475.py
--rw-rw-r--   0 root         (0) root         (0)     8179 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/configuration/delete_group_configuration_v1.py
--rw-rw-r--   0 root         (0) root         (0)     8413 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/configuration/get_group_configuration_f4178c.py
--rw-rw-r--   0 root         (0) root         (0)     7508 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/configuration/initiate_group_configur_384fb1.py
--rw-rw-r--   0 root         (0) root         (0)     9032 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/configuration/list_group_configuratio_ada77c.py
--rw-rw-r--   0 root         (0) root         (0)    11078 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/configuration/update_group_configurat_3473ca.py
--rw-rw-r--   0 root         (0) root         (0)     9954 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/configuration/update_group_configurat_745686.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:38:02.819051 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group/
--rw-rw-r--   0 root         (0) root         (0)     2026 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     9116 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group/create_new_group_public_v1.py
--rw-rw-r--   0 root         (0) root         (0)     9116 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group/create_new_group_public_v2.py
--rw-rw-r--   0 root         (0) root         (0)     7729 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group/delete_group_admin_v1.py
--rw-rw-r--   0 root         (0) root         (0)     9040 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group/delete_group_predefined_67cb4b.py
--rw-rw-r--   0 root         (0) root         (0)     9040 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group/delete_group_predefined_dbecca.py
--rw-rw-r--   0 root         (0) root         (0)     7926 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group/delete_group_public_v1.py
--rw-rw-r--   0 root         (0) root         (0)     7926 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group/delete_group_public_v2.py
--rw-rw-r--   0 root         (0) root         (0)    11380 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group/get_group_list_admin_v1.py
--rw-rw-r--   0 root         (0) root         (0)    10317 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group/get_group_list_public_v1.py
--rw-rw-r--   0 root         (0) root         (0)     7901 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group/get_list_group_by_i_ds__72c106.py
--rw-rw-r--   0 root         (0) root         (0)     7873 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group/get_list_group_by_i_ds_v2.py
--rw-rw-r--   0 root         (0) root         (0)     7843 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group/get_single_group_admin_v1.py
--rw-rw-r--   0 root         (0) root         (0)     7742 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group/get_single_group_public_v1.py
--rw-rw-r--   0 root         (0) root         (0)     9633 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group/update_group_custom_att_4a1290.py
--rw-rw-r--   0 root         (0) root         (0)     9633 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group/update_group_custom_att_c48713.py
--rw-rw-r--   0 root         (0) root         (0)     9436 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group/update_group_custom_rul_0b1934.py
--rw-rw-r--   0 root         (0) root         (0)     9436 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group/update_group_custom_rul_f33cbf.py
--rw-rw-r--   0 root         (0) root         (0)    10686 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group/update_group_predefined_5cebe2.py
--rw-rw-r--   0 root         (0) root         (0)    10686 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group/update_group_predefined_94da96.py
--rw-rw-r--   0 root         (0) root         (0)     9373 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group/update_patch_single_gro_bb3360.py
--rw-rw-r--   0 root         (0) root         (0)     9373 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group/update_patch_single_gro_ce5ae8.py
--rw-rw-r--   0 root         (0) root         (0)     9355 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group/update_put_single_group_5bf5c3.py
--rw-rw-r--   0 root         (0) root         (0)     9278 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group/update_single_group_v1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:38:02.823051 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group_member/
--rw-rw-r--   0 root         (0) root         (0)     2166 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group_member/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8578 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group_member/accept_group_invitation_27bb3d.py
--rw-rw-r--   0 root         (0) root         (0)     8578 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group_member/accept_group_invitation_eae968.py
--rw-rw-r--   0 root         (0) root         (0)     8494 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group_member/accept_group_join_reque_5995a4.py
--rw-rw-r--   0 root         (0) root         (0)     9295 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group_member/accept_group_join_reque_fe83bc.py
--rw-rw-r--   0 root         (0) root         (0)     8734 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group_member/admin_get_user_group_st_657089.py
--rw-rw-r--   0 root         (0) root         (0)     7805 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group_member/cancel_group_join_request_v1.py
--rw-rw-r--   0 root         (0) root         (0)     9072 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group_member/cancel_invitation_group_02cc21.py
--rw-rw-r--   0 root         (0) root         (0)    10363 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group_member/get_group_members_list__2e05f5.py
--rw-rw-r--   0 root         (0) root         (0)    10254 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group_member/get_group_members_list__b75ca5.py
--rw-rw-r--   0 root         (0) root         (0)     8983 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group_member/get_user_group_informat_04a815.py
--rw-rw-r--   0 root         (0) root         (0)     8185 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group_member/get_user_group_informat_51aafe.py
--rw-rw-r--   0 root         (0) root         (0)     8887 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group_member/get_user_group_status_i_e11d20.py
--rw-rw-r--   0 root         (0) root         (0)     9765 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group_member/get_user_joined_group_i_2e0ab3.py
--rw-rw-r--   0 root         (0) root         (0)     8796 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group_member/invite_group_public_v1.py
--rw-rw-r--   0 root         (0) root         (0)     9616 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group_member/invite_group_public_v2.py
--rw-rw-r--   0 root         (0) root         (0)     8230 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group_member/join_group_v1.py
--rw-rw-r--   0 root         (0) root         (0)     8230 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group_member/join_group_v2.py
--rw-rw-r--   0 root         (0) root         (0)     8076 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group_member/kick_group_member_public_v1.py
--rw-rw-r--   0 root         (0) root         (0)     8900 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group_member/kick_group_member_public_v2.py
--rw-rw-r--   0 root         (0) root         (0)     7107 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group_member/leave_group_public_v1.py
--rw-rw-r--   0 root         (0) root         (0)     7896 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group_member/leave_group_public_v2.py
--rw-rw-r--   0 root         (0) root         (0)     8257 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group_member/reject_group_invitation_2bc2a2.py
--rw-rw-r--   0 root         (0) root         (0)     8257 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group_member/reject_group_invitation_c6a225.py
--rw-rw-r--   0 root         (0) root         (0)     9295 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group_member/reject_group_join_reque_70d2ee.py
--rw-rw-r--   0 root         (0) root         (0)     8494 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group_member/reject_group_join_reque_85b3af.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:38:02.823051 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group_roles/
--rw-rw-r--   0 root         (0) root         (0)     1291 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group_roles/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8373 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group_roles/create_member_role_admin_v1.py
--rw-rw-r--   0 root         (0) root         (0)     7961 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group_roles/delete_member_role_admin_v1.py
--rw-rw-r--   0 root         (0) root         (0)     9430 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group_roles/delete_member_role_public_v1.py
--rw-rw-r--   0 root         (0) root         (0)    10233 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group_roles/delete_member_role_public_v2.py
--rw-rw-r--   0 root         (0) root         (0)     8526 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group_roles/get_member_roles_list_admin_v1.py
--rw-rw-r--   0 root         (0) root         (0)     8376 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group_roles/get_member_roles_list_p_25257f.py
--rw-rw-r--   0 root         (0) root         (0)     8437 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group_roles/get_member_roles_list_p_5c76d5.py
--rw-rw-r--   0 root         (0) root         (0)     7984 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group_roles/get_single_member_role__4d5402.py
--rw-rw-r--   0 root         (0) root         (0)     9349 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group_roles/update_member_role_admin_v1.py
--rw-rw-r--   0 root         (0) root         (0)     9835 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group_roles/update_member_role_perm_09ed62.py
--rw-rw-r--   0 root         (0) root         (0)     9419 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group_roles/update_member_role_public_v1.py
--rw-rw-r--   0 root         (0) root         (0)    10222 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group_roles/update_member_role_public_v2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:38:02.823051 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/member_request/
--rw-rw-r--   0 root         (0) root         (0)      829 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/member_request/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8661 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/member_request/get_group_invitation_re_954909.py
--rw-rw-r--   0 root         (0) root         (0)     9605 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/member_request/get_group_invite_reques_8cc920.py
--rw-rw-r--   0 root         (0) root         (0)     9563 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/member_request/get_group_join_request__01154d.py
--rw-rw-r--   0 root         (0) root         (0)     9563 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/member_request/get_group_join_request__0b96ac.py
--rw-rw-r--   0 root         (0) root         (0)     8589 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/member_request/get_my_group_join_request_v2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:38:02.823051 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/wrappers/
--rw-rw-r--   0 root         (0) root         (0)     9213 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/wrappers/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    36350 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/wrappers/_configuration.py
--rw-rw-r--   0 root         (0) root         (0)    96472 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/wrappers/_group.py
--rw-rw-r--   0 root         (0) root         (0)   102651 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/wrappers/_group_member.py
--rw-rw-r--   0 root         (0) root         (0)    46756 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/wrappers/_group_roles.py
--rw-rw-r--   0 root         (0) root         (0)    20405 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/wrappers/_member_request.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:38:02.827051 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk_service_group.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1117 2024-02-27 05:38:02.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk_service_group.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10237 2024-02-27 05:38:02.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk_service_group.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-27 05:38:02.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk_service_group.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       22 2024-02-27 05:38:02.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk_service_group.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-02-27 05:38:02.000000 accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk_service_group.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)      355 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-group-0.8.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-27 05:38:02.827051 accelbyte-py-sdk-service-group-0.8.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:42:15.011347 accelbyte-py-sdk-service-group-0.9.0/
+-rw-r--r--   0 root         (0) root         (0)     1117 2024-03-26 05:42:15.011347 accelbyte-py-sdk-service-group-0.9.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      869 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:42:14.999348 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:42:14.999348 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:42:14.999348 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/
+-rw-rw-r--   0 root         (0) root         (0)     8863 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:42:15.003347 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/
+-rw-rw-r--   0 root         (0) root         (0)     4719 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3901 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_assign_role_to_member_request_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     4612 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_cancel_invitation_group_response_v2.py
+-rw-rw-r--   0 root         (0) root         (0)    10023 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_create_group_configuration_request_v1.py
+-rw-rw-r--   0 root         (0) root         (0)    10113 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_create_group_configuration_response_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     5454 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_create_member_role_request_v1.py
+-rw-rw-r--   0 root         (0) root         (0)    10735 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_get_group_configuration_response_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     3940 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_get_group_list_request_v2.py
+-rw-rw-r--   0 root         (0) root         (0)     5350 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_get_group_member_list_response_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     5074 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_get_groups_list_response_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     4154 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_get_groups_response_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     5305 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_get_member_requests_list_response_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     5223 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_get_member_roles_list_response_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     6875 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_get_user_group_information_response_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     4518 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_group_member.py
+-rw-rw-r--   0 root         (0) root         (0)    13350 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_group_response_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     5618 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_group_rule.py
+-rw-rw-r--   0 root         (0) root         (0)     3925 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_group_rule_group_custom_rule.py
+-rw-rw-r--   0 root         (0) root         (0)     5958 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_group_rule_response_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     4027 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_group_rule_response_v1_group_custom_rule.py
+-rw-rw-r--   0 root         (0) root         (0)     5077 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_join_group_response_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     4672 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_kick_group_member_response_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     4479 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_leave_group_response_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     5307 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_list_configuration_response_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     4576 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_member_request_group_response_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     5241 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_member_request_response_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     6156 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_member_role_response_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     5434 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_pagination.py
+-rw-rw-r--   0 root         (0) root         (0)    11126 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_public_create_new_group_request_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     3923 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_remove_role_from_member_request_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     4477 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_role_permission.py
+-rw-rw-r--   0 root         (0) root         (0)     4805 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_rule.py
+-rw-rw-r--   0 root         (0) root         (0)     5852 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_rule_information.py
+-rw-rw-r--   0 root         (0) root         (0)     4986 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_rule_response_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     4563 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_update_group_configuration_global_rules_request_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     5472 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_update_group_configuration_request_v1.py
+-rw-rw-r--   0 root         (0) root         (0)    10113 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_update_group_configuration_response_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     4394 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_update_group_custom_attributes_request_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     4320 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_update_group_custom_rule_request_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     4452 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_update_group_predefined_rule_request_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     8722 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_update_group_request_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     4046 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_update_group_request_v1_custom_attributes.py
+-rw-rw-r--   0 root         (0) root         (0)     4751 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_update_member_role_permissions_request_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     4050 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_update_member_role_request_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     4527 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_user_invitation_response_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     4575 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/response_error_response.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:42:15.003347 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/
+-rw-rw-r--   0 root         (0) root         (0)      434 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:42:15.003347 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/configuration/
+-rw-rw-r--   0 root         (0) root         (0)     1086 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/configuration/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     9306 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/configuration/create_group_configurat_f2dcd2.py
+-rw-rw-r--   0 root         (0) root         (0)     9677 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/configuration/delete_group_configurat_db1475.py
+-rw-rw-r--   0 root         (0) root         (0)     8179 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/configuration/delete_group_configuration_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     8413 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/configuration/get_group_configuration_f4178c.py
+-rw-rw-r--   0 root         (0) root         (0)     7508 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/configuration/initiate_group_configur_384fb1.py
+-rw-rw-r--   0 root         (0) root         (0)     9032 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/configuration/list_group_configuratio_ada77c.py
+-rw-rw-r--   0 root         (0) root         (0)    11078 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/configuration/update_group_configurat_3473ca.py
+-rw-rw-r--   0 root         (0) root         (0)     9954 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/configuration/update_group_configurat_745686.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:42:15.007347 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group/
+-rw-rw-r--   0 root         (0) root         (0)     2026 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     9116 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group/create_new_group_public_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     9116 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group/create_new_group_public_v2.py
+-rw-rw-r--   0 root         (0) root         (0)     7729 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group/delete_group_admin_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     9040 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group/delete_group_predefined_67cb4b.py
+-rw-rw-r--   0 root         (0) root         (0)     9040 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group/delete_group_predefined_dbecca.py
+-rw-rw-r--   0 root         (0) root         (0)     7926 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group/delete_group_public_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     7926 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group/delete_group_public_v2.py
+-rw-rw-r--   0 root         (0) root         (0)    11380 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group/get_group_list_admin_v1.py
+-rw-rw-r--   0 root         (0) root         (0)    10317 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group/get_group_list_public_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     7901 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group/get_list_group_by_i_ds__72c106.py
+-rw-rw-r--   0 root         (0) root         (0)     7873 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group/get_list_group_by_i_ds_v2.py
+-rw-rw-r--   0 root         (0) root         (0)     7843 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group/get_single_group_admin_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     7742 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group/get_single_group_public_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     9633 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group/update_group_custom_att_4a1290.py
+-rw-rw-r--   0 root         (0) root         (0)     9633 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group/update_group_custom_att_c48713.py
+-rw-rw-r--   0 root         (0) root         (0)     9436 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group/update_group_custom_rul_0b1934.py
+-rw-rw-r--   0 root         (0) root         (0)     9436 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group/update_group_custom_rul_f33cbf.py
+-rw-rw-r--   0 root         (0) root         (0)    10686 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group/update_group_predefined_5cebe2.py
+-rw-rw-r--   0 root         (0) root         (0)    10686 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group/update_group_predefined_94da96.py
+-rw-rw-r--   0 root         (0) root         (0)     9373 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group/update_patch_single_gro_bb3360.py
+-rw-rw-r--   0 root         (0) root         (0)     9373 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group/update_patch_single_gro_ce5ae8.py
+-rw-rw-r--   0 root         (0) root         (0)     9355 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group/update_put_single_group_5bf5c3.py
+-rw-rw-r--   0 root         (0) root         (0)     9278 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group/update_single_group_v1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:42:15.007347 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group_member/
+-rw-rw-r--   0 root         (0) root         (0)     2166 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group_member/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8578 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group_member/accept_group_invitation_27bb3d.py
+-rw-rw-r--   0 root         (0) root         (0)     8578 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group_member/accept_group_invitation_eae968.py
+-rw-rw-r--   0 root         (0) root         (0)     8494 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group_member/accept_group_join_reque_5995a4.py
+-rw-rw-r--   0 root         (0) root         (0)     9295 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group_member/accept_group_join_reque_fe83bc.py
+-rw-rw-r--   0 root         (0) root         (0)     8734 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group_member/admin_get_user_group_st_657089.py
+-rw-rw-r--   0 root         (0) root         (0)     7805 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group_member/cancel_group_join_request_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     9072 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group_member/cancel_invitation_group_02cc21.py
+-rw-rw-r--   0 root         (0) root         (0)    10363 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group_member/get_group_members_list__2e05f5.py
+-rw-rw-r--   0 root         (0) root         (0)    10254 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group_member/get_group_members_list__b75ca5.py
+-rw-rw-r--   0 root         (0) root         (0)     8983 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group_member/get_user_group_informat_04a815.py
+-rw-rw-r--   0 root         (0) root         (0)     8185 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group_member/get_user_group_informat_51aafe.py
+-rw-rw-r--   0 root         (0) root         (0)     8887 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group_member/get_user_group_status_i_e11d20.py
+-rw-rw-r--   0 root         (0) root         (0)     9765 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group_member/get_user_joined_group_i_2e0ab3.py
+-rw-rw-r--   0 root         (0) root         (0)     8796 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group_member/invite_group_public_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     9616 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group_member/invite_group_public_v2.py
+-rw-rw-r--   0 root         (0) root         (0)     8230 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group_member/join_group_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     8230 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group_member/join_group_v2.py
+-rw-rw-r--   0 root         (0) root         (0)     8076 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group_member/kick_group_member_public_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     8900 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group_member/kick_group_member_public_v2.py
+-rw-rw-r--   0 root         (0) root         (0)     7107 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group_member/leave_group_public_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     7896 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group_member/leave_group_public_v2.py
+-rw-rw-r--   0 root         (0) root         (0)     8257 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group_member/reject_group_invitation_2bc2a2.py
+-rw-rw-r--   0 root         (0) root         (0)     8257 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group_member/reject_group_invitation_c6a225.py
+-rw-rw-r--   0 root         (0) root         (0)     9295 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group_member/reject_group_join_reque_70d2ee.py
+-rw-rw-r--   0 root         (0) root         (0)     8494 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group_member/reject_group_join_reque_85b3af.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:42:15.011347 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group_roles/
+-rw-rw-r--   0 root         (0) root         (0)     1291 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group_roles/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8373 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group_roles/create_member_role_admin_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     7961 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group_roles/delete_member_role_admin_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     9430 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group_roles/delete_member_role_public_v1.py
+-rw-rw-r--   0 root         (0) root         (0)    10233 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group_roles/delete_member_role_public_v2.py
+-rw-rw-r--   0 root         (0) root         (0)     8526 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group_roles/get_member_roles_list_admin_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     8376 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group_roles/get_member_roles_list_p_25257f.py
+-rw-rw-r--   0 root         (0) root         (0)     8437 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group_roles/get_member_roles_list_p_5c76d5.py
+-rw-rw-r--   0 root         (0) root         (0)     7984 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group_roles/get_single_member_role__4d5402.py
+-rw-rw-r--   0 root         (0) root         (0)     9349 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group_roles/update_member_role_admin_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     9835 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group_roles/update_member_role_perm_09ed62.py
+-rw-rw-r--   0 root         (0) root         (0)     9419 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group_roles/update_member_role_public_v1.py
+-rw-rw-r--   0 root         (0) root         (0)    10222 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group_roles/update_member_role_public_v2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:42:15.011347 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/member_request/
+-rw-rw-r--   0 root         (0) root         (0)      829 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/member_request/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8661 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/member_request/get_group_invitation_re_954909.py
+-rw-rw-r--   0 root         (0) root         (0)     9605 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/member_request/get_group_invite_reques_8cc920.py
+-rw-rw-r--   0 root         (0) root         (0)     9563 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/member_request/get_group_join_request__01154d.py
+-rw-rw-r--   0 root         (0) root         (0)     9563 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/member_request/get_group_join_request__0b96ac.py
+-rw-rw-r--   0 root         (0) root         (0)     8589 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/member_request/get_my_group_join_request_v2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:42:15.011347 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/wrappers/
+-rw-rw-r--   0 root         (0) root         (0)     9213 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/wrappers/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    36350 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/wrappers/_configuration.py
+-rw-rw-r--   0 root         (0) root         (0)    96472 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/wrappers/_group.py
+-rw-rw-r--   0 root         (0) root         (0)   102651 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/wrappers/_group_member.py
+-rw-rw-r--   0 root         (0) root         (0)    46756 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/wrappers/_group_roles.py
+-rw-rw-r--   0 root         (0) root         (0)    20405 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/wrappers/_member_request.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:42:15.011347 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk_service_group.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1117 2024-03-26 05:42:14.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk_service_group.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10237 2024-03-26 05:42:14.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk_service_group.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-03-26 05:42:14.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk_service_group.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 05:42:14.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk_service_group.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-03-26 05:42:14.000000 accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk_service_group.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)      355 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-group-0.9.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-03-26 05:42:15.011347 accelbyte-py-sdk-service-group-0.9.0/setup.cfg
```

### Comparing `accelbyte-py-sdk-service-group-0.8.0/PKG-INFO` & `accelbyte-py-sdk-service-group-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: accelbyte-py-sdk-service-group
-Version: 0.8.0
+Version: 0.9.0
 Summary: AccelByte Python SDK - AccelByte Gaming Services Group Service
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: accelbyte-py-sdk-core
 
 [//]: # (Code generated. DO NOT EDIT!)
 
 # AccelByte Modular Python SDK - Service Module
 
 This is a service module for the [AccelByte Modular Python SDK](https://github.com/AccelByte/accelbyte-python-modular-sdk) package.
 
 ```text
 AccelByte Gaming Services Group Service
-* Version: 2.19.1
+* Version: 2.19.2
 ```
 
 ## Setup
 
 This SDK requires Python 3.9 to be installed.
 
 ### Install with Pip
```

### Comparing `accelbyte-py-sdk-service-group-0.8.0/README.md` & `accelbyte-py-sdk-service-group-0.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # AccelByte Modular Python SDK - Service Module
 
 This is a service module for the [AccelByte Modular Python SDK](https://github.com/AccelByte/accelbyte-python-modular-sdk) package.
 
 ```text
 AccelByte Gaming Services Group Service
-* Version: 2.19.1
+* Version: 2.19.2
 ```
 
 ## Setup
 
 This SDK requires Python 3.9 to be installed.
 
 ### Install with Pip
```

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/__init__.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: service-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Group Service."""
 
-__version__ = "2.19.1"
+__version__ = "2.19.2"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 # configuration
 from .wrappers import create_group_configuration_admin_v1
```

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/__init__.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: model-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Group Service."""
 
-__version__ = "2.19.1"
+__version__ = "2.19.2"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .models_assign_role_to_member_request_v1 import ModelsAssignRoleToMemberRequestV1
 from .models_cancel_invitation_group_response_v2 import (
```

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_assign_role_to_member_request_v1.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_assign_role_to_member_request_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_cancel_invitation_group_response_v2.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_cancel_invitation_group_response_v2.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_create_group_configuration_request_v1.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_create_group_configuration_request_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_create_group_configuration_response_v1.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_create_group_configuration_response_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_create_member_role_request_v1.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_create_member_role_request_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_get_group_configuration_response_v1.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_get_group_configuration_response_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_get_group_list_request_v2.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_get_group_list_request_v2.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_get_group_member_list_response_v1.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_get_group_member_list_response_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_get_groups_list_response_v1.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_get_groups_list_response_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_get_groups_response_v1.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_get_groups_response_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_get_member_requests_list_response_v1.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_get_member_requests_list_response_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_get_member_roles_list_response_v1.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_get_member_roles_list_response_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_get_user_group_information_response_v1.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_get_user_group_information_response_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_group_member.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_group_member.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_group_response_v1.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_group_response_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_group_rule.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_group_rule.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_group_rule_group_custom_rule.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_group_rule_group_custom_rule.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_group_rule_response_v1.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_group_rule_response_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_group_rule_response_v1_group_custom_rule.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_group_rule_response_v1_group_custom_rule.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_join_group_response_v1.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_join_group_response_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_kick_group_member_response_v1.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_kick_group_member_response_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_leave_group_response_v1.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_leave_group_response_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_list_configuration_response_v1.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_list_configuration_response_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_member_request_group_response_v1.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_member_request_group_response_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_member_request_response_v1.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_member_request_response_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_member_role_response_v1.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_member_role_response_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_pagination.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_pagination.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_public_create_new_group_request_v1.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_public_create_new_group_request_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_remove_role_from_member_request_v1.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_remove_role_from_member_request_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_role_permission.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_role_permission.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_rule.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_rule.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_rule_information.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_rule_information.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_rule_response_v1.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_rule_response_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_update_group_configuration_global_rules_request_v1.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_update_group_configuration_global_rules_request_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_update_group_configuration_request_v1.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_update_group_configuration_request_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_update_group_configuration_response_v1.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_update_group_configuration_response_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_update_group_custom_attributes_request_v1.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_update_group_custom_attributes_request_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_update_group_custom_rule_request_v1.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_update_group_custom_rule_request_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_update_group_predefined_rule_request_v1.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_update_group_predefined_rule_request_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_update_group_request_v1.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_update_group_request_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_update_group_request_v1_custom_attributes.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_update_group_request_v1_custom_attributes.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_update_member_role_permissions_request_v1.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_update_member_role_permissions_request_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_update_member_role_request_v1.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_update_member_role_request_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/models_user_invitation_response_v1.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/models_user_invitation_response_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/models/response_error_response.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/models/response_error_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/configuration/__init__.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/configuration/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Group Service."""
 
-__version__ = "2.19.1"
+__version__ = "2.19.2"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .create_group_configurat_f2dcd2 import CreateGroupConfigurationAdminV1
 from .delete_group_configurat_db1475 import DeleteGroupConfigurationGlobalRuleAdminV1
```

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/configuration/create_group_configurat_f2dcd2.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/configuration/create_group_configurat_f2dcd2.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/configuration/delete_group_configurat_db1475.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/configuration/delete_group_configurat_db1475.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/configuration/delete_group_configuration_v1.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/configuration/delete_group_configuration_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/configuration/get_group_configuration_f4178c.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/configuration/get_group_configuration_f4178c.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/configuration/initiate_group_configur_384fb1.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/configuration/initiate_group_configur_384fb1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/configuration/list_group_configuratio_ada77c.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/configuration/list_group_configuratio_ada77c.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/configuration/update_group_configurat_3473ca.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/configuration/update_group_configurat_3473ca.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/configuration/update_group_configurat_745686.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/configuration/update_group_configurat_745686.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group/__init__.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Group Service."""
 
-__version__ = "2.19.1"
+__version__ = "2.19.2"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .create_new_group_public_v1 import CreateNewGroupPublicV1
 from .create_new_group_public_v2 import CreateNewGroupPublicV2
```

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group/create_new_group_public_v1.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group/create_new_group_public_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group/create_new_group_public_v2.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group/create_new_group_public_v2.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group/delete_group_admin_v1.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group/delete_group_admin_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group/delete_group_predefined_67cb4b.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group/delete_group_predefined_67cb4b.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group/delete_group_predefined_dbecca.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group/delete_group_predefined_dbecca.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group/delete_group_public_v1.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group/delete_group_public_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group/delete_group_public_v2.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group/delete_group_public_v2.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group/get_group_list_admin_v1.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group/get_group_list_admin_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group/get_group_list_public_v1.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group/get_group_list_public_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group/get_list_group_by_i_ds__72c106.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group/get_list_group_by_i_ds__72c106.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group/get_list_group_by_i_ds_v2.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group/get_list_group_by_i_ds_v2.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group/get_single_group_admin_v1.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group/get_single_group_admin_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group/get_single_group_public_v1.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group/get_single_group_public_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group/update_group_custom_att_4a1290.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group/update_group_custom_att_4a1290.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group/update_group_custom_att_c48713.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group/update_group_custom_att_c48713.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group/update_group_custom_rul_0b1934.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group/update_group_custom_rul_0b1934.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group/update_group_custom_rul_f33cbf.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group/update_group_custom_rul_f33cbf.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group/update_group_predefined_5cebe2.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group/update_group_predefined_5cebe2.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group/update_group_predefined_94da96.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group/update_group_predefined_94da96.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group/update_patch_single_gro_bb3360.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group/update_patch_single_gro_bb3360.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group/update_patch_single_gro_ce5ae8.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group/update_patch_single_gro_ce5ae8.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group/update_put_single_group_5bf5c3.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group/update_put_single_group_5bf5c3.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group/update_single_group_v1.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group/update_single_group_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group_member/__init__.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group_member/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Group Service."""
 
-__version__ = "2.19.1"
+__version__ = "2.19.2"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .accept_group_invitation_27bb3d import AcceptGroupInvitationPublicV1
 from .accept_group_invitation_eae968 import AcceptGroupInvitationPublicV2
```

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group_member/accept_group_invitation_27bb3d.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group_member/accept_group_invitation_27bb3d.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group_member/accept_group_invitation_eae968.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group_member/accept_group_invitation_eae968.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group_member/accept_group_join_reque_5995a4.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group_member/accept_group_join_reque_5995a4.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group_member/accept_group_join_reque_fe83bc.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group_member/accept_group_join_reque_fe83bc.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group_member/admin_get_user_group_st_657089.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group_member/admin_get_user_group_st_657089.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group_member/cancel_group_join_request_v1.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group_member/cancel_group_join_request_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group_member/cancel_invitation_group_02cc21.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group_member/cancel_invitation_group_02cc21.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group_member/get_group_members_list__2e05f5.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group_member/get_group_members_list__2e05f5.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group_member/get_group_members_list__b75ca5.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group_member/get_group_members_list__b75ca5.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group_member/get_user_group_informat_04a815.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group_member/get_user_group_informat_04a815.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group_member/get_user_group_informat_51aafe.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group_member/get_user_group_informat_51aafe.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group_member/get_user_group_status_i_e11d20.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group_member/get_user_group_status_i_e11d20.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group_member/get_user_joined_group_i_2e0ab3.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group_member/get_user_joined_group_i_2e0ab3.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group_member/invite_group_public_v1.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group_member/invite_group_public_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group_member/invite_group_public_v2.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group_member/invite_group_public_v2.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group_member/join_group_v1.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group_member/join_group_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group_member/join_group_v2.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group_member/join_group_v2.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group_member/kick_group_member_public_v1.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group_member/kick_group_member_public_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group_member/kick_group_member_public_v2.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group_member/kick_group_member_public_v2.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group_member/leave_group_public_v1.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group_member/leave_group_public_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group_member/leave_group_public_v2.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group_member/leave_group_public_v2.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group_member/reject_group_invitation_2bc2a2.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group_member/reject_group_invitation_2bc2a2.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group_member/reject_group_invitation_c6a225.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group_member/reject_group_invitation_c6a225.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group_member/reject_group_join_reque_70d2ee.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group_member/reject_group_join_reque_70d2ee.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group_member/reject_group_join_reque_85b3af.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group_member/reject_group_join_reque_85b3af.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group_roles/__init__.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group_roles/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Group Service."""
 
-__version__ = "2.19.1"
+__version__ = "2.19.2"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .create_member_role_admin_v1 import CreateMemberRoleAdminV1
 from .delete_member_role_admin_v1 import DeleteMemberRoleAdminV1
```

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group_roles/create_member_role_admin_v1.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group_roles/create_member_role_admin_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group_roles/delete_member_role_admin_v1.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group_roles/delete_member_role_admin_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group_roles/delete_member_role_public_v1.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group_roles/delete_member_role_public_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group_roles/delete_member_role_public_v2.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group_roles/delete_member_role_public_v2.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group_roles/get_member_roles_list_admin_v1.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group_roles/get_member_roles_list_admin_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group_roles/get_member_roles_list_p_25257f.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group_roles/get_member_roles_list_p_25257f.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group_roles/get_member_roles_list_p_5c76d5.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group_roles/get_member_roles_list_p_5c76d5.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group_roles/get_single_member_role__4d5402.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group_roles/get_single_member_role__4d5402.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group_roles/update_member_role_admin_v1.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group_roles/update_member_role_admin_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group_roles/update_member_role_perm_09ed62.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group_roles/update_member_role_perm_09ed62.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group_roles/update_member_role_public_v1.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group_roles/update_member_role_public_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/group_roles/update_member_role_public_v2.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/group_roles/update_member_role_public_v2.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/member_request/__init__.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/member_request/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Group Service."""
 
-__version__ = "2.19.1"
+__version__ = "2.19.2"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .get_group_invitation_re_954909 import GetGroupInvitationRequestPublicV1
 from .get_group_invite_reques_8cc920 import GetGroupInviteRequestPublicV2
```

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/member_request/get_group_invitation_re_954909.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/member_request/get_group_invitation_re_954909.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/member_request/get_group_invite_reques_8cc920.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/member_request/get_group_invite_reques_8cc920.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/member_request/get_group_join_request__01154d.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/member_request/get_group_join_request__01154d.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/member_request/get_group_join_request__0b96ac.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/member_request/get_group_join_request__0b96ac.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/operations/member_request/get_my_group_join_request_v2.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/operations/member_request/get_my_group_join_request_v2.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/wrappers/__init__.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/wrappers/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: wrapper-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Group Service."""
 
-__version__ = "2.19.1"
+__version__ = "2.19.2"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from ._configuration import create_group_configuration_admin_v1
 from ._configuration import create_group_configuration_admin_v1_async
```

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/wrappers/_configuration.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/wrappers/_configuration.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/wrappers/_group.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/wrappers/_group.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/wrappers/_group_member.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/wrappers/_group_member.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/wrappers/_group_roles.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/wrappers/_group_roles.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk/api/group/wrappers/_member_request.py` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk/api/group/wrappers/_member_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk_service_group.egg-info/PKG-INFO` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk_service_group.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: accelbyte-py-sdk-service-group
-Version: 0.8.0
+Version: 0.9.0
 Summary: AccelByte Python SDK - AccelByte Gaming Services Group Service
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: accelbyte-py-sdk-core
 
 [//]: # (Code generated. DO NOT EDIT!)
 
 # AccelByte Modular Python SDK - Service Module
 
 This is a service module for the [AccelByte Modular Python SDK](https://github.com/AccelByte/accelbyte-python-modular-sdk) package.
 
 ```text
 AccelByte Gaming Services Group Service
-* Version: 2.19.1
+* Version: 2.19.2
 ```
 
 ## Setup
 
 This SDK requires Python 3.9 to be installed.
 
 ### Install with Pip
```

### Comparing `accelbyte-py-sdk-service-group-0.8.0/accelbyte_py_sdk_service_group.egg-info/SOURCES.txt` & `accelbyte-py-sdk-service-group-0.9.0/accelbyte_py_sdk_service_group.egg-info/SOURCES.txt`

 * *Files identical despite different names*

