# Comparing `tmp/accelbyte_py_sdk_service_reporting-0.7.0.tar.gz` & `tmp/accelbyte_py_sdk_service_reporting-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accelbyte_py_sdk_service_reporting-0.7.0.tar", last modified: Tue May  7 06:29:50 2024, max compression
+gzip compressed data, was "accelbyte_py_sdk_service_reporting-0.8.0.tar", last modified: Tue May 21 03:49:06 2024, max compression
```

## Comparing `accelbyte_py_sdk_service_reporting-0.7.0.tar` & `accelbyte_py_sdk_service_reporting-0.8.0.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:29:50.750686 accelbyte_py_sdk_service_reporting-0.7.0/
--rw-r--r--   0 root         (0) root         (0)     1133 2024-05-07 06:29:50.750686 accelbyte_py_sdk_service_reporting-0.7.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      877 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:29:50.742686 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:29:50.742686 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:29:50.742686 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/
--rw-rw-r--   0 root         (0) root         (0)     3814 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:29:50.746686 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/
--rw-rw-r--   0 root         (0) root         (0)     4317 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5226 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_action_api_request.py
--rw-rw-r--   0 root         (0) root         (0)     5239 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_action_api_response.py
--rw-rw-r--   0 root         (0) root         (0)     4250 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_action_list_api_response.py
--rw-rw-r--   0 root         (0) root         (0)     4293 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_admin_all_reasons_response.py
--rw-rw-r--   0 root         (0) root         (0)     5171 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_admin_reason_list_response.py
--rw-rw-r--   0 root         (0) root         (0)     8332 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_admin_reason_response.py
--rw-rw-r--   0 root         (0) root         (0)     6548 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_ban_account_action_request.py
--rw-rw-r--   0 root         (0) root         (0)     6563 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_ban_account_action_response.py
--rw-rw-r--   0 root         (0) root         (0)     5534 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_category_limit.py
--rw-rw-r--   0 root         (0) root         (0)     5672 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_config_response.py
--rw-rw-r--   0 root         (0) root         (0)     4662 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_create_reason_group_request.py
--rw-rw-r--   0 root         (0) root         (0)     5235 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_create_reason_request.py
--rw-rw-r--   0 root         (0) root         (0)     4567 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_error_response.py
--rw-rw-r--   0 root         (0) root         (0)     5945 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_extension_category_api_request.py
--rw-rw-r--   0 root         (0) root         (0)     5972 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_extension_category_api_response.py
--rw-rw-r--   0 root         (0) root         (0)     4459 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_extension_category_list_api_response.py
--rw-rw-r--   0 root         (0) root         (0)     7157 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_moderation_rule_actions_request.py
--rw-rw-r--   0 root         (0) root         (0)     7180 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_moderation_rule_actions_response.py
--rw-rw-r--   0 root         (0) root         (0)     3914 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_moderation_rule_active_request.py
--rw-rw-r--   0 root         (0) root         (0)     9274 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_moderation_rule_request.py
--rw-rw-r--   0 root         (0) root         (0)    11237 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_moderation_rule_response.py
--rw-rw-r--   0 root         (0) root         (0)     5168 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_moderation_rules_list.py
--rw-rw-r--   0 root         (0) root         (0)     5466 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_pagination.py
--rw-rw-r--   0 root         (0) root         (0)     4408 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_public_reason_group_response.py
--rw-rw-r--   0 root         (0) root         (0)     5215 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_public_reason_list_response.py
--rw-rw-r--   0 root         (0) root         (0)     4530 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_public_reason_response.py
--rw-rw-r--   0 root         (0) root         (0)     5248 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_reason_group_list_response.py
--rw-rw-r--   0 root         (0) root         (0)     5521 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_reason_group_response.py
--rw-rw-r--   0 root         (0) root         (0)     5036 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_report_list_response.py
--rw-rw-r--   0 root         (0) root         (0)    13341 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_report_response.py
--rw-rw-r--   0 root         (0) root         (0)     6299 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_reporting_limit.py
--rw-rw-r--   0 root         (0) root         (0)     9713 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_submit_report_request.py
--rw-rw-r--   0 root         (0) root         (0)    10961 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_submit_report_response.py
--rw-rw-r--   0 root         (0) root         (0)     5036 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_ticket_list_response.py
--rw-rw-r--   0 root         (0) root         (0)    12043 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_ticket_response.py
--rw-rw-r--   0 root         (0) root         (0)     5431 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_ticket_statistic_response.py
--rw-rw-r--   0 root         (0) root         (0)     4364 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_unused_reason_list_response.py
--rw-rw-r--   0 root         (0) root         (0)     4662 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_update_reason_group_request.py
--rw-rw-r--   0 root         (0) root         (0)     5023 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_update_ticket_resolutions_request.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:29:50.746686 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/
--rw-rw-r--   0 root         (0) root         (0)      438 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:29:50.746686 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_configurations/
--rw-rw-r--   0 root         (0) root         (0)      577 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_configurations/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7437 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_configurations/get.py
--rw-rw-r--   0 root         (0) root         (0)     7390 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_configurations/upsert.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:29:50.746686 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_extension_categories_and_auto_moderation_actions/
--rw-rw-r--   0 root         (0) root         (0)      899 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_extension_categories_and_auto_moderation_actions/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6659 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_extension_categories_and_auto_moderation_actions/admin_create_extension__954f3a.py
--rw-rw-r--   0 root         (0) root         (0)     6447 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_extension_categories_and_auto_moderation_actions/admin_create_mod_action.py
--rw-rw-r--   0 root         (0) root         (0)     5331 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_extension_categories_and_auto_moderation_actions/admin_find_action_list.py
--rw-rw-r--   0 root         (0) root         (0)     8063 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_extension_categories_and_auto_moderation_actions/admin_find_extension_ca_6e8210.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:29:50.746686 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_moderation_rule/
--rw-rw-r--   0 root         (0) root         (0)      831 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_moderation_rule/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7891 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_moderation_rule/create_moderation_rule.py
--rw-rw-r--   0 root         (0) root         (0)     6939 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_moderation_rule/delete_moderation_rule.py
--rw-rw-r--   0 root         (0) root         (0)     7138 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_moderation_rule/get_moderation_rule_details.py
--rw-rw-r--   0 root         (0) root         (0)    10141 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_moderation_rule/get_moderation_rules.py
--rw-rw-r--   0 root         (0) root         (0)     8996 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_moderation_rule/update_moderation_rule.py
--rw-rw-r--   0 root         (0) root         (0)     8480 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_moderation_rule/update_moderation_rule_status.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:29:50.746686 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/
--rw-rw-r--   0 root         (0) root         (0)     1055 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6103 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/admin_get_all_reasons.py
--rw-rw-r--   0 root         (0) root         (0)     7038 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/admin_get_reason.py
--rw-rw-r--   0 root         (0) root         (0)     9447 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/admin_get_reasons.py
--rw-rw-r--   0 root         (0) root         (0)     8448 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/admin_get_unused_reasons.py
--rw-rw-r--   0 root         (0) root         (0)     7914 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/admin_list_reason_groups.py
--rw-rw-r--   0 root         (0) root         (0)     7565 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/create_reason.py
--rw-rw-r--   0 root         (0) root         (0)     7844 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/create_reason_group.py
--rw-rw-r--   0 root         (0) root         (0)     6648 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/delete_reason.py
--rw-rw-r--   0 root         (0) root         (0)     6685 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/delete_reason_group.py
--rw-rw-r--   0 root         (0) root         (0)     6974 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/get_reason_group.py
--rw-rw-r--   0 root         (0) root         (0)     8371 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/update_reason.py
--rw-rw-r--   0 root         (0) root         (0)     8670 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/update_reason_group.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:29:50.746686 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_reports/
--rw-rw-r--   0 root         (0) root         (0)      560 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_reports/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8047 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_reports/admin_submit_report.py
--rw-rw-r--   0 root         (0) root         (0)    10455 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_reports/list_reports.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:29:50.750686 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_tickets/
--rw-rw-r--   0 root         (0) root         (0)      759 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_tickets/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6835 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_tickets/delete_ticket.py
--rw-rw-r--   0 root         (0) root         (0)     8603 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_tickets/get_reports_by_ticket.py
--rw-rw-r--   0 root         (0) root         (0)     7028 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_tickets/get_ticket_detail.py
--rw-rw-r--   0 root         (0) root         (0)    13033 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_tickets/list_tickets.py
--rw-rw-r--   0 root         (0) root         (0)     8122 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_tickets/ticket_statistic.py
--rw-rw-r--   0 root         (0) root         (0)     8290 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_tickets/update_ticket_resolutions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:29:50.750686 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/public_reasons/
--rw-rw-r--   0 root         (0) root         (0)      582 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/public_reasons/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     9419 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/public_reasons/public_get_reasons.py
--rw-rw-r--   0 root         (0) root         (0)     7853 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/public_reasons/public_list_reason_groups.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:29:50.750686 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/public_reports/
--rw-rw-r--   0 root         (0) root         (0)      511 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/public_reports/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8262 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/public_reports/submit_report.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:29:50.750686 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/wrappers/
--rw-rw-r--   0 root         (0) root         (0)     4578 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/wrappers/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6347 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/wrappers/_admin_configurations.py
--rw-rw-r--   0 root         (0) root         (0)    10312 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/wrappers/_admin_extension_categories_and_auto_moderation_actions.py
--rw-rw-r--   0 root         (0) root         (0)    19611 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/wrappers/_admin_moderation_rule.py
--rw-rw-r--   0 root         (0) root         (0)    32822 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/wrappers/_admin_reasons.py
--rw-rw-r--   0 root         (0) root         (0)     8390 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/wrappers/_admin_reports.py
--rw-rw-r--   0 root         (0) root         (0)    18658 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/wrappers/_admin_tickets.py
--rw-rw-r--   0 root         (0) root         (0)     6758 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/wrappers/_public_reasons.py
--rw-rw-r--   0 root         (0) root         (0)     5020 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/wrappers/_public_reports.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:29:50.750686 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk_service_reporting.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1133 2024-05-07 06:29:50.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk_service_reporting.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7486 2024-05-07 06:29:50.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk_service_reporting.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-07 06:29:50.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk_service_reporting.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-07 06:29:50.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk_service_reporting.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-05-07 06:29:50.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk_service_reporting.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)      363 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-07 06:29:50.750686 accelbyte_py_sdk_service_reporting-0.7.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:49:06.875113 accelbyte_py_sdk_service_reporting-0.8.0/
+-rw-r--r--   0 root         (0) root         (0)     1133 2024-05-21 03:49:06.875113 accelbyte_py_sdk_service_reporting-0.8.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      877 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:49:06.863113 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:49:06.863113 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:49:06.863113 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/
+-rw-rw-r--   0 root         (0) root         (0)     3814 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:49:06.867113 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/models/
+-rw-rw-r--   0 root         (0) root         (0)     4317 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/models/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     5226 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/models/restapi_action_api_request.py
+-rw-rw-r--   0 root         (0) root         (0)     5239 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/models/restapi_action_api_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4250 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/models/restapi_action_list_api_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4293 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/models/restapi_admin_all_reasons_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5171 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/models/restapi_admin_reason_list_response.py
+-rw-rw-r--   0 root         (0) root         (0)     8332 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/models/restapi_admin_reason_response.py
+-rw-rw-r--   0 root         (0) root         (0)     6548 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/models/restapi_ban_account_action_request.py
+-rw-rw-r--   0 root         (0) root         (0)     6563 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/models/restapi_ban_account_action_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5534 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/models/restapi_category_limit.py
+-rw-rw-r--   0 root         (0) root         (0)     5672 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/models/restapi_config_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4662 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/models/restapi_create_reason_group_request.py
+-rw-rw-r--   0 root         (0) root         (0)     5235 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/models/restapi_create_reason_request.py
+-rw-rw-r--   0 root         (0) root         (0)     4567 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/models/restapi_error_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5945 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/models/restapi_extension_category_api_request.py
+-rw-rw-r--   0 root         (0) root         (0)     5972 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/models/restapi_extension_category_api_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4459 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/models/restapi_extension_category_list_api_response.py
+-rw-rw-r--   0 root         (0) root         (0)     7157 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/models/restapi_moderation_rule_actions_request.py
+-rw-rw-r--   0 root         (0) root         (0)     7180 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/models/restapi_moderation_rule_actions_response.py
+-rw-rw-r--   0 root         (0) root         (0)     3914 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/models/restapi_moderation_rule_active_request.py
+-rw-rw-r--   0 root         (0) root         (0)     9274 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/models/restapi_moderation_rule_request.py
+-rw-rw-r--   0 root         (0) root         (0)    11237 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/models/restapi_moderation_rule_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5168 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/models/restapi_moderation_rules_list.py
+-rw-rw-r--   0 root         (0) root         (0)     5466 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/models/restapi_pagination.py
+-rw-rw-r--   0 root         (0) root         (0)     4408 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/models/restapi_public_reason_group_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5215 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/models/restapi_public_reason_list_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4530 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/models/restapi_public_reason_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5248 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/models/restapi_reason_group_list_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5521 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/models/restapi_reason_group_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5036 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/models/restapi_report_list_response.py
+-rw-rw-r--   0 root         (0) root         (0)    13341 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/models/restapi_report_response.py
+-rw-rw-r--   0 root         (0) root         (0)     6299 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/models/restapi_reporting_limit.py
+-rw-rw-r--   0 root         (0) root         (0)     9713 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/models/restapi_submit_report_request.py
+-rw-rw-r--   0 root         (0) root         (0)    10961 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/models/restapi_submit_report_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5036 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/models/restapi_ticket_list_response.py
+-rw-rw-r--   0 root         (0) root         (0)    12043 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/models/restapi_ticket_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5431 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/models/restapi_ticket_statistic_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4364 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/models/restapi_unused_reason_list_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4662 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/models/restapi_update_reason_group_request.py
+-rw-rw-r--   0 root         (0) root         (0)     5023 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/models/restapi_update_ticket_resolutions_request.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:49:06.867113 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/
+-rw-rw-r--   0 root         (0) root         (0)      438 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:49:06.867113 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/admin_configurations/
+-rw-rw-r--   0 root         (0) root         (0)      577 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/admin_configurations/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7437 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/admin_configurations/get.py
+-rw-rw-r--   0 root         (0) root         (0)     7390 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/admin_configurations/upsert.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:49:06.867113 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/admin_extension_categories_and_auto_moderation_actions/
+-rw-rw-r--   0 root         (0) root         (0)      899 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/admin_extension_categories_and_auto_moderation_actions/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     6659 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/admin_extension_categories_and_auto_moderation_actions/admin_create_extension__954f3a.py
+-rw-rw-r--   0 root         (0) root         (0)     6447 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/admin_extension_categories_and_auto_moderation_actions/admin_create_mod_action.py
+-rw-rw-r--   0 root         (0) root         (0)     5331 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/admin_extension_categories_and_auto_moderation_actions/admin_find_action_list.py
+-rw-rw-r--   0 root         (0) root         (0)     8063 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/admin_extension_categories_and_auto_moderation_actions/admin_find_extension_ca_6e8210.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:49:06.871113 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/admin_moderation_rule/
+-rw-rw-r--   0 root         (0) root         (0)      831 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/admin_moderation_rule/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7891 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/admin_moderation_rule/create_moderation_rule.py
+-rw-rw-r--   0 root         (0) root         (0)     6939 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/admin_moderation_rule/delete_moderation_rule.py
+-rw-rw-r--   0 root         (0) root         (0)     7138 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/admin_moderation_rule/get_moderation_rule_details.py
+-rw-rw-r--   0 root         (0) root         (0)    10141 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/admin_moderation_rule/get_moderation_rules.py
+-rw-rw-r--   0 root         (0) root         (0)     8996 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/admin_moderation_rule/update_moderation_rule.py
+-rw-rw-r--   0 root         (0) root         (0)     8480 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/admin_moderation_rule/update_moderation_rule_status.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:49:06.871113 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/
+-rw-rw-r--   0 root         (0) root         (0)     1055 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     6103 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/admin_get_all_reasons.py
+-rw-rw-r--   0 root         (0) root         (0)     7038 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/admin_get_reason.py
+-rw-rw-r--   0 root         (0) root         (0)     9447 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/admin_get_reasons.py
+-rw-rw-r--   0 root         (0) root         (0)     8448 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/admin_get_unused_reasons.py
+-rw-rw-r--   0 root         (0) root         (0)     7914 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/admin_list_reason_groups.py
+-rw-rw-r--   0 root         (0) root         (0)     7565 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/create_reason.py
+-rw-rw-r--   0 root         (0) root         (0)     7844 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/create_reason_group.py
+-rw-rw-r--   0 root         (0) root         (0)     6648 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/delete_reason.py
+-rw-rw-r--   0 root         (0) root         (0)     6685 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/delete_reason_group.py
+-rw-rw-r--   0 root         (0) root         (0)     6974 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/get_reason_group.py
+-rw-rw-r--   0 root         (0) root         (0)     8371 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/update_reason.py
+-rw-rw-r--   0 root         (0) root         (0)     8670 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/update_reason_group.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:49:06.871113 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/admin_reports/
+-rw-rw-r--   0 root         (0) root         (0)      560 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/admin_reports/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8047 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/admin_reports/admin_submit_report.py
+-rw-rw-r--   0 root         (0) root         (0)    10455 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/admin_reports/list_reports.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:49:06.871113 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/admin_tickets/
+-rw-rw-r--   0 root         (0) root         (0)      759 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/admin_tickets/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     6835 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/admin_tickets/delete_ticket.py
+-rw-rw-r--   0 root         (0) root         (0)     8603 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/admin_tickets/get_reports_by_ticket.py
+-rw-rw-r--   0 root         (0) root         (0)     7028 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/admin_tickets/get_ticket_detail.py
+-rw-rw-r--   0 root         (0) root         (0)    13033 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/admin_tickets/list_tickets.py
+-rw-rw-r--   0 root         (0) root         (0)     8122 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/admin_tickets/ticket_statistic.py
+-rw-rw-r--   0 root         (0) root         (0)     8290 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/admin_tickets/update_ticket_resolutions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:49:06.871113 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/public_reasons/
+-rw-rw-r--   0 root         (0) root         (0)      582 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/public_reasons/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     9419 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/public_reasons/public_get_reasons.py
+-rw-rw-r--   0 root         (0) root         (0)     7853 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/public_reasons/public_list_reason_groups.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:49:06.871113 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/public_reports/
+-rw-rw-r--   0 root         (0) root         (0)      511 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/public_reports/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8262 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/public_reports/submit_report.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:49:06.871113 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/wrappers/
+-rw-rw-r--   0 root         (0) root         (0)     4578 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/wrappers/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     6347 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/wrappers/_admin_configurations.py
+-rw-rw-r--   0 root         (0) root         (0)    10312 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/wrappers/_admin_extension_categories_and_auto_moderation_actions.py
+-rw-rw-r--   0 root         (0) root         (0)    19611 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/wrappers/_admin_moderation_rule.py
+-rw-rw-r--   0 root         (0) root         (0)    32822 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/wrappers/_admin_reasons.py
+-rw-rw-r--   0 root         (0) root         (0)     8390 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/wrappers/_admin_reports.py
+-rw-rw-r--   0 root         (0) root         (0)    18658 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/wrappers/_admin_tickets.py
+-rw-rw-r--   0 root         (0) root         (0)     6758 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/wrappers/_public_reasons.py
+-rw-rw-r--   0 root         (0) root         (0)     5020 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/wrappers/_public_reports.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:49:06.871113 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk_service_reporting.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1133 2024-05-21 03:49:06.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk_service_reporting.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7486 2024-05-21 03:49:06.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk_service_reporting.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 03:49:06.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk_service_reporting.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-21 03:49:06.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk_service_reporting.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-05-21 03:49:06.000000 accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk_service_reporting.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)      363 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_reporting-0.8.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-21 03:49:06.875113 accelbyte_py_sdk_service_reporting-0.8.0/setup.cfg
```

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/PKG-INFO` & `accelbyte_py_sdk_service_reporting-0.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: accelbyte-py-sdk-service-reporting
-Version: 0.7.0
+Version: 0.8.0
 Summary: AccelByte Python SDK - AccelByte Gaming Services Reporting Service
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: accelbyte-py-sdk-core
 
 [//]: # (Code generated. DO NOT EDIT!)
 
 # AccelByte Modular Python SDK - Service Module
 
 This is a service module for the [AccelByte Modular Python SDK](https://github.com/AccelByte/accelbyte-python-modular-sdk) package.
 
 ```text
 AccelByte Gaming Services Reporting Service
-* Version: 0.1.34
+* Version: 0.1.36
 ```
 
 ## Setup
 
 This SDK requires Python 3.9 to be installed.
 
 ### Install with Pip
```

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/README.md` & `accelbyte_py_sdk_service_reporting-0.8.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # AccelByte Modular Python SDK - Service Module
 
 This is a service module for the [AccelByte Modular Python SDK](https://github.com/AccelByte/accelbyte-python-modular-sdk) package.
 
 ```text
 AccelByte Gaming Services Reporting Service
-* Version: 0.1.34
+* Version: 0.1.36
 ```
 
 ## Setup
 
 This SDK requires Python 3.9 to be installed.
 
 ### Install with Pip
```

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/__init__.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: service-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Reporting Service."""
 
-__version__ = "0.1.34"
+__version__ = "0.1.36"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 # admin_configurations
 from .wrappers import get
```

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/__init__.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: model-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Reporting Service."""
 
-__version__ = "0.1.34"
+__version__ = "0.1.36"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .restapi_action_api_request import RestapiActionApiRequest
 from .restapi_action_api_response import RestapiActionApiResponse
```

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_action_api_request.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/models/restapi_action_api_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_action_api_response.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/models/restapi_action_api_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_action_list_api_response.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/models/restapi_action_list_api_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_admin_all_reasons_response.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/models/restapi_admin_all_reasons_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_admin_reason_list_response.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/models/restapi_admin_reason_list_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_admin_reason_response.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/models/restapi_admin_reason_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_ban_account_action_request.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/models/restapi_ban_account_action_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_ban_account_action_response.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/models/restapi_ban_account_action_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_category_limit.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/models/restapi_category_limit.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_config_response.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/models/restapi_config_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_create_reason_group_request.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/models/restapi_create_reason_group_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_create_reason_request.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/models/restapi_create_reason_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_error_response.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/models/restapi_error_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_extension_category_api_request.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/models/restapi_extension_category_api_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_extension_category_api_response.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/models/restapi_extension_category_api_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_extension_category_list_api_response.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/models/restapi_extension_category_list_api_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_moderation_rule_actions_request.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/models/restapi_moderation_rule_actions_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_moderation_rule_actions_response.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/models/restapi_moderation_rule_actions_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_moderation_rule_active_request.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/models/restapi_moderation_rule_active_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_moderation_rule_request.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/models/restapi_moderation_rule_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_moderation_rule_response.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/models/restapi_moderation_rule_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_moderation_rules_list.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/models/restapi_moderation_rules_list.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_pagination.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/models/restapi_pagination.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_public_reason_group_response.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/models/restapi_public_reason_group_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_public_reason_list_response.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/models/restapi_public_reason_list_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_public_reason_response.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/models/restapi_public_reason_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_reason_group_list_response.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/models/restapi_reason_group_list_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_reason_group_response.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/models/restapi_reason_group_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_report_list_response.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/models/restapi_report_list_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_report_response.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/models/restapi_report_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_reporting_limit.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/models/restapi_reporting_limit.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_submit_report_request.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/models/restapi_submit_report_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_submit_report_response.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/models/restapi_submit_report_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_ticket_list_response.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/models/restapi_ticket_list_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_ticket_response.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/models/restapi_ticket_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_ticket_statistic_response.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/models/restapi_ticket_statistic_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_unused_reason_list_response.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/models/restapi_unused_reason_list_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_update_reason_group_request.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/models/restapi_update_reason_group_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_update_ticket_resolutions_request.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/models/restapi_update_ticket_resolutions_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_configurations/__init__.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/admin_configurations/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Reporting Service."""
 
-__version__ = "0.1.34"
+__version__ = "0.1.36"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .get import Get
 from .get import (
```

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_configurations/get.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/admin_configurations/get.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_configurations/upsert.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/admin_configurations/upsert.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_extension_categories_and_auto_moderation_actions/__init__.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/admin_extension_categories_and_auto_moderation_actions/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Reporting Service."""
 
-__version__ = "0.1.34"
+__version__ = "0.1.36"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .admin_create_extension__954f3a import AdminCreateExtensionCategory
 from .admin_create_mod_action import AdminCreateModAction
```

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_extension_categories_and_auto_moderation_actions/admin_create_extension__954f3a.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/admin_extension_categories_and_auto_moderation_actions/admin_create_extension__954f3a.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_extension_categories_and_auto_moderation_actions/admin_create_mod_action.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/admin_extension_categories_and_auto_moderation_actions/admin_create_mod_action.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_extension_categories_and_auto_moderation_actions/admin_find_action_list.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/admin_extension_categories_and_auto_moderation_actions/admin_find_action_list.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_extension_categories_and_auto_moderation_actions/admin_find_extension_ca_6e8210.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/admin_extension_categories_and_auto_moderation_actions/admin_find_extension_ca_6e8210.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_moderation_rule/__init__.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/admin_moderation_rule/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Reporting Service."""
 
-__version__ = "0.1.34"
+__version__ = "0.1.36"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .create_moderation_rule import CreateModerationRule
 from .delete_moderation_rule import DeleteModerationRule
```

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_moderation_rule/create_moderation_rule.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/admin_moderation_rule/create_moderation_rule.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_moderation_rule/delete_moderation_rule.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/admin_moderation_rule/delete_moderation_rule.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_moderation_rule/get_moderation_rule_details.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/admin_moderation_rule/get_moderation_rule_details.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_moderation_rule/get_moderation_rules.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/admin_moderation_rule/get_moderation_rules.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_moderation_rule/update_moderation_rule.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/admin_moderation_rule/update_moderation_rule.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_moderation_rule/update_moderation_rule_status.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/admin_moderation_rule/update_moderation_rule_status.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/__init__.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Reporting Service."""
 
-__version__ = "0.1.34"
+__version__ = "0.1.36"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .admin_get_all_reasons import AdminGetAllReasons
 from .admin_get_reason import AdminGetReason
```

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/admin_get_all_reasons.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/admin_get_all_reasons.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/admin_get_reason.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/admin_get_reason.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/admin_get_reasons.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/admin_get_reasons.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/admin_get_unused_reasons.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/admin_get_unused_reasons.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/admin_list_reason_groups.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/admin_list_reason_groups.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/create_reason.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/create_reason.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/create_reason_group.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/create_reason_group.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/delete_reason.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/delete_reason.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/delete_reason_group.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/delete_reason_group.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/get_reason_group.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/get_reason_group.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/update_reason.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/update_reason.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/update_reason_group.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/update_reason_group.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_reports/__init__.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/admin_reports/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Reporting Service."""
 
-__version__ = "0.1.34"
+__version__ = "0.1.36"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .admin_submit_report import AdminSubmitReport
 from .list_reports import ListReports
```

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_reports/admin_submit_report.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/admin_reports/admin_submit_report.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_reports/list_reports.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/admin_reports/list_reports.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_tickets/__init__.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/admin_tickets/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Reporting Service."""
 
-__version__ = "0.1.34"
+__version__ = "0.1.36"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .delete_ticket import DeleteTicket
 from .get_reports_by_ticket import GetReportsByTicket
```

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_tickets/delete_ticket.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/admin_tickets/delete_ticket.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_tickets/get_reports_by_ticket.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/admin_tickets/get_reports_by_ticket.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_tickets/get_ticket_detail.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/admin_tickets/get_ticket_detail.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_tickets/list_tickets.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/admin_tickets/list_tickets.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_tickets/ticket_statistic.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/admin_tickets/ticket_statistic.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_tickets/update_ticket_resolutions.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/admin_tickets/update_ticket_resolutions.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/public_reasons/__init__.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/public_reasons/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Reporting Service."""
 
-__version__ = "0.1.34"
+__version__ = "0.1.36"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .public_get_reasons import PublicGetReasons
 from .public_list_reason_groups import PublicListReasonGroups
```

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/public_reasons/public_get_reasons.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/public_reasons/public_get_reasons.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/public_reasons/public_list_reason_groups.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/public_reasons/public_list_reason_groups.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/public_reports/submit_report.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/operations/public_reports/submit_report.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/wrappers/__init__.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/wrappers/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: wrapper-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Reporting Service."""
 
-__version__ = "0.1.34"
+__version__ = "0.1.36"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from ._admin_configurations import get
 from ._admin_configurations import get_async
```

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/wrappers/_admin_configurations.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/wrappers/_admin_configurations.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/wrappers/_admin_extension_categories_and_auto_moderation_actions.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/wrappers/_admin_extension_categories_and_auto_moderation_actions.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/wrappers/_admin_moderation_rule.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/wrappers/_admin_moderation_rule.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/wrappers/_admin_reasons.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/wrappers/_admin_reasons.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/wrappers/_admin_reports.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/wrappers/_admin_reports.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/wrappers/_admin_tickets.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/wrappers/_admin_tickets.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/wrappers/_public_reasons.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/wrappers/_public_reasons.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/wrappers/_public_reports.py` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk/api/reporting/wrappers/_public_reports.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk_service_reporting.egg-info/PKG-INFO` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk_service_reporting.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: accelbyte-py-sdk-service-reporting
-Version: 0.7.0
+Version: 0.8.0
 Summary: AccelByte Python SDK - AccelByte Gaming Services Reporting Service
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: accelbyte-py-sdk-core
 
 [//]: # (Code generated. DO NOT EDIT!)
 
 # AccelByte Modular Python SDK - Service Module
 
 This is a service module for the [AccelByte Modular Python SDK](https://github.com/AccelByte/accelbyte-python-modular-sdk) package.
 
 ```text
 AccelByte Gaming Services Reporting Service
-* Version: 0.1.34
+* Version: 0.1.36
 ```
 
 ## Setup
 
 This SDK requires Python 3.9 to be installed.
 
 ### Install with Pip
```

### Comparing `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk_service_reporting.egg-info/SOURCES.txt` & `accelbyte_py_sdk_service_reporting-0.8.0/accelbyte_py_sdk_service_reporting.egg-info/SOURCES.txt`

 * *Files identical despite different names*

