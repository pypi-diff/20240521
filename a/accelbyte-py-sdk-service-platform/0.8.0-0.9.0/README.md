# Comparing `tmp/accelbyte-py-sdk-service-platform-0.8.0.tar.gz` & `tmp/accelbyte-py-sdk-service-platform-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accelbyte-py-sdk-service-platform-0.8.0.tar", last modified: Tue Feb 27 05:40:41 2024, max compression
+gzip compressed data, was "accelbyte-py-sdk-service-platform-0.9.0.tar", last modified: Wed Mar 13 06:13:44 2024, max compression
```

## Comparing `accelbyte-py-sdk-service-platform-0.8.0.tar` & `accelbyte-py-sdk-service-platform-0.9.0.tar`

### file list

```diff
@@ -1,978 +1,981 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:40:41.268810 accelbyte-py-sdk-service-platform-0.8.0/
--rw-r--r--   0 root         (0) root         (0)     1129 2024-02-27 05:40:41.268810 accelbyte-py-sdk-service-platform-0.8.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      875 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:40:41.180811 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:40:41.180811 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:40:41.184811 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/
--rw-rw-r--   0 root         (0) root         (0)    44384 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:40:41.220810 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/
--rw-rw-r--   0 root         (0) root         (0)    46405 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6887 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/achievement_info.py
--rw-rw-r--   0 root         (0) root         (0)     6536 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/action.py
--rw-rw-r--   0 root         (0) root         (0)     4847 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/action_request.py
--rw-rw-r--   0 root         (0) root         (0)     3817 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/additional_data.py
--rw-rw-r--   0 root         (0) root         (0)     6091 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/additional_data_entitlement.py
--rw-rw-r--   0 root         (0) root         (0)     6160 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/admin_entitlement_decrement.py
--rw-rw-r--   0 root         (0) root         (0)     5427 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/admin_entitlement_sold_request.py
--rw-rw-r--   0 root         (0) root         (0)    15789 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/admin_order_create.py
--rw-rw-r--   0 root         (0) root         (0)    14844 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/adyen_config.py
--rw-rw-r--   0 root         (0) root         (0)     5936 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/ali_pay_config.py
--rw-rw-r--   0 root         (0) root         (0)     3609 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/app_config.py
--rw-rw-r--   0 root         (0) root         (0)    15232 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/app_entitlement_info.py
--rw-rw-r--   0 root         (0) root         (0)     5127 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/app_entitlement_paging_sliced_result.py
--rw-rw-r--   0 root         (0) root         (0)    18681 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/app_info.py
--rw-rw-r--   0 root         (0) root         (0)     4503 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/app_localization.py
--rw-rw-r--   0 root         (0) root         (0)    15911 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/app_update.py
--rw-rw-r--   0 root         (0) root         (0)     5222 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/apple_iap_config_info.py
--rw-rw-r--   0 root         (0) root         (0)     4523 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/apple_iap_config_request.py
--rw-rw-r--   0 root         (0) root         (0)     7917 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/apple_iap_receipt.py
--rw-rw-r--   0 root         (0) root         (0)     5358 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/available_comparison.py
--rw-rw-r--   0 root         (0) root         (0)     7793 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/available_predicate.py
--rw-rw-r--   0 root         (0) root         (0)    10502 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/available_price.py
--rw-rw-r--   0 root         (0) root         (0)     5173 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/base_custom_config.py
--rw-rw-r--   0 root         (0) root         (0)     3952 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/base_tls_config.py
--rw-rw-r--   0 root         (0) root         (0)     7398 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/basic_category_info.py
--rw-rw-r--   0 root         (0) root         (0)    15822 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/basic_item.py
--rw-rw-r--   0 root         (0) root         (0)     6661 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/billing_account.py
--rw-rw-r--   0 root         (0) root         (0)    21684 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/billing_history_info.py
--rw-rw-r--   0 root         (0) root         (0)     5051 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/billing_history_paging_sliced_result.py
--rw-rw-r--   0 root         (0) root         (0)     7057 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/box_item.py
--rw-rw-r--   0 root         (0) root         (0)     5756 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/bulk_credit_request.py
--rw-rw-r--   0 root         (0) root         (0)     6234 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/bulk_credit_result.py
--rw-rw-r--   0 root         (0) root         (0)     5680 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/bulk_debit_request.py
--rw-rw-r--   0 root         (0) root         (0)     6209 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/bulk_debit_result.py
--rw-rw-r--   0 root         (0) root         (0)     5398 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/bulk_entitlement_grant_request.py
--rw-rw-r--   0 root         (0) root         (0)     6545 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/bulk_entitlement_grant_result.py
--rw-rw-r--   0 root         (0) root         (0)     6646 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/bulk_entitlement_revoke_result.py
--rw-rw-r--   0 root         (0) root         (0)     3809 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/bulk_operation_result.py
--rw-rw-r--   0 root         (0) root         (0)     4256 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/bulk_region_data_change_request.py
--rw-rw-r--   0 root         (0) root         (0)    45824 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/bundled_item_info.py
--rw-rw-r--   0 root         (0) root         (0)    15037 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/campaign_create.py
--rw-rw-r--   0 root         (0) root         (0)     6745 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/campaign_dynamic_info.py
--rw-rw-r--   0 root         (0) root         (0)    17678 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/campaign_info.py
--rw-rw-r--   0 root         (0) root         (0)     4921 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/campaign_paging_sliced_result.py
--rw-rw-r--   0 root         (0) root         (0)    14206 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/campaign_update.py
--rw-rw-r--   0 root         (0) root         (0)     4428 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/cancel_request.py
--rw-rw-r--   0 root         (0) root         (0)    17109 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/catalog_change_info.py
--rw-rw-r--   0 root         (0) root         (0)     5618 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/catalog_change_paging_result.py
--rw-rw-r--   0 root         (0) root         (0)     4527 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/catalog_change_statistics.py
--rw-rw-r--   0 root         (0) root         (0)     6626 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/catalog_definition_info.py
--rw-rw-r--   0 root         (0) root         (0)     5016 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/category_create.py
--rw-rw-r--   0 root         (0) root         (0)     8006 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/category_info.py
--rw-rw-r--   0 root         (0) root         (0)     4285 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/category_update.py
--rw-rw-r--   0 root         (0) root         (0)     4573 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/checkout_config.py
--rw-rw-r--   0 root         (0) root         (0)    16858 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/clawback_info.py
--rw-rw-r--   0 root         (0) root         (0)     6028 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/client_request_parameter.py
--rw-rw-r--   0 root         (0) root         (0)     4918 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/client_transaction.py
--rw-rw-r--   0 root         (0) root         (0)     3656 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/code_create.py
--rw-rw-r--   0 root         (0) root         (0)     3759 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/code_create_result.py
--rw-rw-r--   0 root         (0) root         (0)    19154 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/code_info.py
--rw-rw-r--   0 root         (0) root         (0)     4894 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/code_info_paging_sliced_result.py
--rw-rw-r--   0 root         (0) root         (0)     5164 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/condition_group.py
--rw-rw-r--   0 root         (0) root         (0)     4805 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/condition_group_validate_result.py
--rw-rw-r--   0 root         (0) root         (0)     5881 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/condition_match_result.py
--rw-rw-r--   0 root         (0) root         (0)     5207 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/consumable_entitlement_revocation_config.py
--rw-rw-r--   0 root         (0) root         (0)     6759 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/consume_item.py
--rw-rw-r--   0 root         (0) root         (0)     6843 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/credit_payload.py
--rw-rw-r--   0 root         (0) root         (0)     9077 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/credit_request.py
--rw-rw-r--   0 root         (0) root         (0)     6245 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/credit_result.py
--rw-rw-r--   0 root         (0) root         (0)    10457 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/credit_revocation.py
--rw-rw-r--   0 root         (0) root         (0)     6404 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/credit_summary.py
--rw-rw-r--   0 root         (0) root         (0)     3818 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/currency_config.py
--rw-rw-r--   0 root         (0) root         (0)     7842 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/currency_create.py
--rw-rw-r--   0 root         (0) root         (0)     9628 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/currency_info.py
--rw-rw-r--   0 root         (0) root         (0)     7086 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/currency_summary.py
--rw-rw-r--   0 root         (0) root         (0)     4326 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/currency_update.py
--rw-rw-r--   0 root         (0) root         (0)     9690 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/currency_wallet.py
--rw-rw-r--   0 root         (0) root         (0)     3729 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/customization.py
--rw-rw-r--   0 root         (0) root         (0)     9465 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/debit_by_currency_code_request.py
--rw-rw-r--   0 root         (0) root         (0)     8727 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/debit_by_wallet_platform_request.py
--rw-rw-r--   0 root         (0) root         (0)     5973 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/debit_payload.py
--rw-rw-r--   0 root         (0) root         (0)     6735 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/debit_request.py
--rw-rw-r--   0 root         (0) root         (0)     6182 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/debit_result.py
--rw-rw-r--   0 root         (0) root         (0)     4764 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/delete_reward_condition_request.py
--rw-rw-r--   0 root         (0) root         (0)    11458 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/detailed_wallet_transaction_info.py
--rw-rw-r--   0 root         (0) root         (0)     5325 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/detailed_wallet_transaction_paging_sliced_result.py
--rw-rw-r--   0 root         (0) root         (0)     5234 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/dlc_config_reward_short_info.py
--rw-rw-r--   0 root         (0) root         (0)     4557 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/dlc_item.py
--rw-rw-r--   0 root         (0) root         (0)     3987 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/dlc_item_config_info.py
--rw-rw-r--   0 root         (0) root         (0)     4009 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/dlc_item_config_update.py
--rw-rw-r--   0 root         (0) root         (0)    15944 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/dlc_record.py
--rw-rw-r--   0 root         (0) root         (0)     5171 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/durable_entitlement_revocation_config.py
--rw-rw-r--   0 root         (0) root         (0)     5266 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/entitlement_config_info.py
--rw-rw-r--   0 root         (0) root         (0)     5381 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/entitlement_decrement.py
--rw-rw-r--   0 root         (0) root         (0)    28780 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/entitlement_decrement_result.py
--rw-rw-r--   0 root         (0) root         (0)    13320 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/entitlement_grant.py
--rw-rw-r--   0 root         (0) root         (0)     5749 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/entitlement_grant_result.py
--rw-rw-r--   0 root         (0) root         (0)    12212 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/entitlement_history_info.py
--rw-rw-r--   0 root         (0) root         (0)    21339 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/entitlement_ifc.py
--rw-rw-r--   0 root         (0) root         (0)    25710 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/entitlement_info.py
--rw-rw-r--   0 root         (0) root         (0)     5237 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/entitlement_loot_box_reward.py
--rw-rw-r--   0 root         (0) root         (0)     5899 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/entitlement_origin_sync_result.py
--rw-rw-r--   0 root         (0) root         (0)     4420 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/entitlement_ownership.py
--rw-rw-r--   0 root         (0) root         (0)     5054 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/entitlement_paging_sliced_result.py
--rw-rw-r--   0 root         (0) root         (0)     7832 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/entitlement_platform_config_info.py
--rw-rw-r--   0 root         (0) root         (0)     5475 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/entitlement_platform_config_update.py
--rw-rw-r--   0 root         (0) root         (0)     4103 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/entitlement_prechek_result.py
--rw-rw-r--   0 root         (0) root         (0)    10478 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/entitlement_revocation.py
--rw-rw-r--   0 root         (0) root         (0)     5647 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/entitlement_revocation_config.py
--rw-rw-r--   0 root         (0) root         (0)     5372 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/entitlement_revoke_result.py
--rw-rw-r--   0 root         (0) root         (0)     4632 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/entitlement_sold_request.py
--rw-rw-r--   0 root         (0) root         (0)     6979 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/entitlement_sold_result.py
--rw-rw-r--   0 root         (0) root         (0)     3897 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/entitlement_split_request.py
--rw-rw-r--   0 root         (0) root         (0)     4969 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/entitlement_split_result.py
--rw-rw-r--   0 root         (0) root         (0)    17167 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/entitlement_summary.py
--rw-rw-r--   0 root         (0) root         (0)     4779 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/entitlement_transfer_request.py
--rw-rw-r--   0 root         (0) root         (0)     5005 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/entitlement_transfer_result.py
--rw-rw-r--   0 root         (0) root         (0)    10223 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/entitlement_update.py
--rw-rw-r--   0 root         (0) root         (0)     4116 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/epic_games_dlc_sync_request.py
--rw-rw-r--   0 root         (0) root         (0)     4578 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/epic_games_iap_config_info.py
--rw-rw-r--   0 root         (0) root         (0)     3873 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/epic_games_iap_config_request.py
--rw-rw-r--   0 root         (0) root         (0)     4137 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/epic_games_reconcile_request.py
--rw-rw-r--   0 root         (0) root         (0)     7311 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/epic_games_reconcile_result.py
--rw-rw-r--   0 root         (0) root         (0)     6322 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/error_entity.py
--rw-rw-r--   0 root         (0) root         (0)     5594 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/estimated_price_info.py
--rw-rw-r--   0 root         (0) root         (0)     5037 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/event_additional_data.py
--rw-rw-r--   0 root         (0) root         (0)     3790 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/event_payload.py
--rw-rw-r--   0 root         (0) root         (0)     3860 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/export_store_request.py
--rw-rw-r--   0 root         (0) root         (0)     7161 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/export_store_to_csv_request.py
--rw-rw-r--   0 root         (0) root         (0)    10770 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/extension_fulfillment_summary.py
--rw-rw-r--   0 root         (0) root         (0)    21512 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/external_payment_order_create.py
--rw-rw-r--   0 root         (0) root         (0)     7300 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/field_validation_error.py
--rw-rw-r--   0 root         (0) root         (0)     6732 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/fixed_period_rotation_config.py
--rw-rw-r--   0 root         (0) root         (0)     8584 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/ful_fill_item_payload.py
--rw-rw-r--   0 root         (0) root         (0)     5307 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/fulfill_code_request.py
--rw-rw-r--   0 root         (0) root         (0)     5148 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/fulfillment_error.py
--rw-rw-r--   0 root         (0) root         (0)    17981 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/fulfillment_history_info.py
--rw-rw-r--   0 root         (0) root         (0)     5152 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/fulfillment_history_paging_sliced_result.py
--rw-rw-r--   0 root         (0) root         (0)     9156 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/fulfillment_item.py
--rw-rw-r--   0 root         (0) root         (0)    19151 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/fulfillment_request.py
--rw-rw-r--   0 root         (0) root         (0)     8957 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/fulfillment_result.py
--rw-rw-r--   0 root         (0) root         (0)     3920 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/fulfillment_script_create.py
--rw-rw-r--   0 root         (0) root         (0)     4485 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/fulfillment_script_info.py
--rw-rw-r--   0 root         (0) root         (0)     3920 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/fulfillment_script_update.py
--rw-rw-r--   0 root         (0) root         (0)    17250 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/full_app_info.py
--rw-rw-r--   0 root         (0) root         (0)     8587 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/full_category_info.py
--rw-rw-r--   0 root         (0) root         (0)    41260 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/full_item_info.py
--rw-rw-r--   0 root         (0) root         (0)     5518 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/full_item_paging_result.py
--rw-rw-r--   0 root         (0) root         (0)     4923 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/full_item_paging_sliced_result.py
--rw-rw-r--   0 root         (0) root         (0)    17158 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/full_section_info.py
--rw-rw-r--   0 root         (0) root         (0)     8097 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/full_view_info.py
--rw-rw-r--   0 root         (0) root         (0)     6372 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/google_iap_config_info.py
--rw-rw-r--   0 root         (0) root         (0)     4804 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/google_iap_config_request.py
--rw-rw-r--   0 root         (0) root         (0)     8949 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/google_iap_receipt.py
--rw-rw-r--   0 root         (0) root         (0)     4008 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/google_receipt_resolve_result.py
--rw-rw-r--   0 root         (0) root         (0)     4583 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/grant_subscription_days_request.py
--rw-rw-r--   0 root         (0) root         (0)     6765 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/grpc_server_info.py
--rw-rw-r--   0 root         (0) root         (0)     9430 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/hierarchical_category_info.py
--rw-rw-r--   0 root         (0) root         (0)     4958 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/iap_clawback_paging_sliced_result.py
--rw-rw-r--   0 root         (0) root         (0)    13051 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/iap_consume_history_info.py
--rw-rw-r--   0 root         (0) root         (0)     5135 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/iap_consume_history_paging_sliced_result.py
--rw-rw-r--   0 root         (0) root         (0)     4023 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/iap_item_config_info.py
--rw-rw-r--   0 root         (0) root         (0)     4045 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/iap_item_config_update.py
--rw-rw-r--   0 root         (0) root         (0)     6407 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/iap_item_entry.py
--rw-rw-r--   0 root         (0) root         (0)     7538 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/iap_item_flat_entry.py
--rw-rw-r--   0 root         (0) root         (0)     4063 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/iap_item_mapping_info.py
--rw-rw-r--   0 root         (0) root         (0)    19605 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/iap_order_info.py
--rw-rw-r--   0 root         (0) root         (0)     4923 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/iap_order_paging_sliced_result.py
--rw-rw-r--   0 root         (0) root         (0)     6800 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/image.py
--rw-rw-r--   0 root         (0) root         (0)     7251 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/import_error_details.py
--rw-rw-r--   0 root         (0) root         (0)     3772 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/import_store_app_info.py
--rw-rw-r--   0 root         (0) root         (0)     5499 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/import_store_category_info.py
--rw-rw-r--   0 root         (0) root         (0)     9930 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/import_store_error.py
--rw-rw-r--   0 root         (0) root         (0)    10028 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/import_store_history_info.py
--rw-rw-r--   0 root         (0) root         (0)     5734 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/import_store_history_paging_result.py
--rw-rw-r--   0 root         (0) root         (0)     8596 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/import_store_item_info.py
--rw-rw-r--   0 root         (0) root         (0)     5742 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/import_store_result.py
--rw-rw-r--   0 root         (0) root         (0)     4528 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/import_store_section_info.py
--rw-rw-r--   0 root         (0) root         (0)     4412 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/import_store_view_info.py
--rw-rw-r--   0 root         (0) root         (0)     5328 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/in_game_item_sync.py
--rw-rw-r--   0 root         (0) root         (0)     6069 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/inventory_config.py
--rw-rw-r--   0 root         (0) root         (0)     6950 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/invoice_currency_summary.py
--rw-rw-r--   0 root         (0) root         (0)     5289 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/invoice_summary.py
--rw-rw-r--   0 root         (0) root         (0)     4318 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/item_acquire_request.py
--rw-rw-r--   0 root         (0) root         (0)     4378 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/item_acquire_result.py
--rw-rw-r--   0 root         (0) root         (0)    35642 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/item_create.py
--rw-rw-r--   0 root         (0) root         (0)     6942 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/item_dynamic_data_info.py
--rw-rw-r--   0 root         (0) root         (0)     5207 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/item_id.py
--rw-rw-r--   0 root         (0) root         (0)    44612 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/item_info.py
--rw-rw-r--   0 root         (0) root         (0)     9707 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/item_naming.py
--rw-rw-r--   0 root         (0) root         (0)     4845 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/item_paging_sliced_result.py
--rw-rw-r--   0 root         (0) root         (0)     4077 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/item_purchase_condition_validate_request.py
--rw-rw-r--   0 root         (0) root         (0)     6775 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/item_purchase_condition_validate_result.py
--rw-rw-r--   0 root         (0) root         (0)     3726 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/item_return_request.py
--rw-rw-r--   0 root         (0) root         (0)    16290 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/item_revocation.py
--rw-rw-r--   0 root         (0) root         (0)    35348 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/item_snapshot.py
--rw-rw-r--   0 root         (0) root         (0)     7898 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/item_type_config_create.py
--rw-rw-r--   0 root         (0) root         (0)     9730 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/item_type_config_info.py
--rw-rw-r--   0 root         (0) root         (0)     6323 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/item_type_config_update.py
--rw-rw-r--   0 root         (0) root         (0)    35924 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/item_update.py
--rw-rw-r--   0 root         (0) root         (0)     6142 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/key_group_create.py
--rw-rw-r--   0 root         (0) root         (0)     5309 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/key_group_dynamic_info.py
--rw-rw-r--   0 root         (0) root         (0)     9251 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/key_group_info.py
--rw-rw-r--   0 root         (0) root         (0)     4923 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/key_group_paging_sliced_result.py
--rw-rw-r--   0 root         (0) root         (0)     6142 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/key_group_update.py
--rw-rw-r--   0 root         (0) root         (0)    10089 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/key_info.py
--rw-rw-r--   0 root         (0) root         (0)     4814 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/key_paging_slice_result.py
--rw-rw-r--   0 root         (0) root         (0)     6973 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/list_view_info.py
--rw-rw-r--   0 root         (0) root         (0)     6062 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/localization.py
--rw-rw-r--   0 root         (0) root         (0)     6048 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/loot_box_config.py
--rw-rw-r--   0 root         (0) root         (0)     7159 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/loot_box_plugin_config_info.py
--rw-rw-r--   0 root         (0) root         (0)     6382 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/loot_box_plugin_config_update.py
--rw-rw-r--   0 root         (0) root         (0)     7113 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/loot_box_reward.py
--rw-rw-r--   0 root         (0) root         (0)     8739 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/mock_iap_receipt.py
--rw-rw-r--   0 root         (0) root         (0)     6618 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/notification_process_result.py
--rw-rw-r--   0 root         (0) root         (0)     5206 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/oculus_iap_config_info.py
--rw-rw-r--   0 root         (0) root         (0)     4509 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/oculus_iap_config_request.py
--rw-rw-r--   0 root         (0) root         (0)     8247 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/oculus_reconcile_result.py
--rw-rw-r--   0 root         (0) root         (0)    11530 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/operation.py
--rw-rw-r--   0 root         (0) root         (0)     9263 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/operation_request.py
--rw-rw-r--   0 root         (0) root         (0)     4048 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/option_box_config.py
--rw-rw-r--   0 root         (0) root         (0)    40806 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/order.py
--rw-rw-r--   0 root         (0) root         (0)     7905 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/order_bundle_item_info.py
--rw-rw-r--   0 root         (0) root         (0)    10211 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/order_create.py
--rw-rw-r--   0 root         (0) root         (0)     4139 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/order_creation_options.py
--rw-rw-r--   0 root         (0) root         (0)     5190 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/order_grant_info.py
--rw-rw-r--   0 root         (0) root         (0)     9333 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/order_history_info.py
--rw-rw-r--   0 root         (0) root         (0)    35283 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/order_info.py
--rw-rw-r--   0 root         (0) root         (0)     5439 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/order_paging_result.py
--rw-rw-r--   0 root         (0) root         (0)     4864 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/order_paging_sliced_result.py
--rw-rw-r--   0 root         (0) root         (0)     3794 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/order_refund_create.py
--rw-rw-r--   0 root         (0) root         (0)     4537 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/order_statistics.py
--rw-rw-r--   0 root         (0) root         (0)     5318 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/order_summary.py
--rw-rw-r--   0 root         (0) root         (0)     4891 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/order_sync_result.py
--rw-rw-r--   0 root         (0) root         (0)     5342 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/order_update.py
--rw-rw-r--   0 root         (0) root         (0)     3568 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/ownership.py
--rw-rw-r--   0 root         (0) root         (0)     3880 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/ownership_token.py
--rw-rw-r--   0 root         (0) root         (0)     4266 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/paging.py
--rw-rw-r--   0 root         (0) root         (0)     6054 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/pay_pal_config.py
--rw-rw-r--   0 root         (0) root         (0)     5071 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/payment_account.py
--rw-rw-r--   0 root         (0) root         (0)     6102 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/payment_callback_config_info.py
--rw-rw-r--   0 root         (0) root         (0)     5450 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/payment_callback_config_update.py
--rw-rw-r--   0 root         (0) root         (0)    20025 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/payment_merchant_config_info.py
--rw-rw-r--   0 root         (0) root         (0)     5193 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/payment_method.py
--rw-rw-r--   0 root         (0) root         (0)    12501 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/payment_notification_info.py
--rw-rw-r--   0 root         (0) root         (0)     5209 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/payment_notification_paging_sliced_result.py
--rw-rw-r--   0 root         (0) root         (0)    45571 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/payment_order.py
--rw-rw-r--   0 root         (0) root         (0)     6366 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/payment_order_charge_request.py
--rw-rw-r--   0 root         (0) root         (0)     5806 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/payment_order_charge_status.py
--rw-rw-r--   0 root         (0) root         (0)    19652 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/payment_order_create.py
--rw-rw-r--   0 root         (0) root         (0)     9857 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/payment_order_create_result.py
--rw-rw-r--   0 root         (0) root         (0)     9373 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/payment_order_details.py
--rw-rw-r--   0 root         (0) root         (0)    42526 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/payment_order_info.py
--rw-rw-r--   0 root         (0) root         (0)     8607 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/payment_order_notify_simulation.py
--rw-rw-r--   0 root         (0) root         (0)     5013 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/payment_order_paging_sliced_result.py
--rw-rw-r--   0 root         (0) root         (0)     4458 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/payment_order_paid_result.py
--rw-rw-r--   0 root         (0) root         (0)     3805 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/payment_order_refund.py
--rw-rw-r--   0 root         (0) root         (0)     9739 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/payment_order_refund_result.py
--rw-rw-r--   0 root         (0) root         (0)     5217 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/payment_order_sync_result.py
--rw-rw-r--   0 root         (0) root         (0)     5902 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/payment_process_result.py
--rw-rw-r--   0 root         (0) root         (0)    11019 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/payment_provider_config_edit.py
--rw-rw-r--   0 root         (0) root         (0)    12711 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/payment_provider_config_info.py
--rw-rw-r--   0 root         (0) root         (0)     5249 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/payment_provider_config_paging_sliced_result.py
--rw-rw-r--   0 root         (0) root         (0)     6175 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/payment_request.py
--rw-rw-r--   0 root         (0) root         (0)     7352 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/payment_tax_config_edit.py
--rw-rw-r--   0 root         (0) root         (0)     7331 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/payment_tax_config_info.py
--rw-rw-r--   0 root         (0) root         (0)     3642 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/payment_token.py
--rw-rw-r--   0 root         (0) root         (0)     8585 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/payment_url.py
--rw-rw-r--   0 root         (0) root         (0)     7491 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/payment_url_create.py
--rw-rw-r--   0 root         (0) root         (0)     4112 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/platform_dlc_config_info.py
--rw-rw-r--   0 root         (0) root         (0)     4134 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/platform_dlc_config_update.py
--rw-rw-r--   0 root         (0) root         (0)     5358 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/platform_dlc_entry.py
--rw-rw-r--   0 root         (0) root         (0)     6674 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/platform_reward.py
--rw-rw-r--   0 root         (0) root         (0)     4579 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/platform_reward_currency.py
--rw-rw-r--   0 root         (0) root         (0)     5219 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/platform_reward_item.py
--rw-rw-r--   0 root         (0) root         (0)     7240 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/platform_subscribe_request.py
--rw-rw-r--   0 root         (0) root         (0)    10282 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/platform_wallet.py
--rw-rw-r--   0 root         (0) root         (0)     7732 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/platform_wallet_config_info.py
--rw-rw-r--   0 root         (0) root         (0)     5375 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/platform_wallet_config_update.py
--rw-rw-r--   0 root         (0) root         (0)     4297 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/play_station_dlc_sync_multi_service_labels_request.py
--rw-rw-r--   0 root         (0) root         (0)     4005 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/play_station_dlc_sync_request.py
--rw-rw-r--   0 root         (0) root         (0)     9707 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/play_station_iap_config_info.py
--rw-rw-r--   0 root         (0) root         (0)     6644 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/play_station_multi_service_labels_reconcile_request.py
--rw-rw-r--   0 root         (0) root         (0)     6270 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/play_station_reconcile_request.py
--rw-rw-r--   0 root         (0) root         (0)     7202 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/play_station_reconcile_result.py
--rw-rw-r--   0 root         (0) root         (0)     9033 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/playstation_iap_config_request.py
--rw-rw-r--   0 root         (0) root         (0)    46169 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/populated_item_info.py
--rw-rw-r--   0 root         (0) root         (0)     5298 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/pre_check_fulfillment_request.py
--rw-rw-r--   0 root         (0) root         (0)     8520 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/predicate.py
--rw-rw-r--   0 root         (0) root         (0)     6295 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/predicate_validate_result.py
--rw-rw-r--   0 root         (0) root         (0)     6257 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/public_custom_config_info.py
--rw-rw-r--   0 root         (0) root         (0)     4278 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/purchase_condition.py
--rw-rw-r--   0 root         (0) root         (0)     4436 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/purchase_condition_update.py
--rw-rw-r--   0 root         (0) root         (0)     3735 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/purchased_item_count.py
--rw-rw-r--   0 root         (0) root         (0)     6288 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/recurring.py
--rw-rw-r--   0 root         (0) root         (0)     5150 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/recurring_charge_result.py
--rw-rw-r--   0 root         (0) root         (0)     9041 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/redeem_history_info.py
--rw-rw-r--   0 root         (0) root         (0)     5032 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/redeem_history_paging_sliced_result.py
--rw-rw-r--   0 root         (0) root         (0)     4294 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/redeem_request.py
--rw-rw-r--   0 root         (0) root         (0)     3972 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/redeem_result.py
--rw-rw-r--   0 root         (0) root         (0)     6083 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/redeemable_item.py
--rw-rw-r--   0 root         (0) root         (0)     6577 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/region_data_change.py
--rw-rw-r--   0 root         (0) root         (0)    13121 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/region_data_item.py
--rw-rw-r--   0 root         (0) root         (0)    12343 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/region_data_item_dto.py
--rw-rw-r--   0 root         (0) root         (0)     7432 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/request_history.py
--rw-rw-r--   0 root         (0) root         (0)     9434 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/requirement.py
--rw-rw-r--   0 root         (0) root         (0)     6050 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/revocation_config_info.py
--rw-rw-r--   0 root         (0) root         (0)     5345 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/revocation_config_update.py
--rw-rw-r--   0 root         (0) root         (0)     5135 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/revocation_error.py
--rw-rw-r--   0 root         (0) root         (0)    16187 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/revocation_history_info.py
--rw-rw-r--   0 root         (0) root         (0)     5133 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/revocation_history_paging_sliced_result.py
--rw-rw-r--   0 root         (0) root         (0)     7200 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/revocation_plugin_config_info.py
--rw-rw-r--   0 root         (0) root         (0)     6434 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/revocation_plugin_config_update.py
--rw-rw-r--   0 root         (0) root         (0)     6858 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/revocation_request.py
--rw-rw-r--   0 root         (0) root         (0)     8495 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/revocation_result.py
--rw-rw-r--   0 root         (0) root         (0)     6340 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/revoke_currency.py
--rw-rw-r--   0 root         (0) root         (0)     3920 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/revoke_entitlement.py
--rw-rw-r--   0 root         (0) root         (0)     4593 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/revoke_entitlement_payload.py
--rw-rw-r--   0 root         (0) root         (0)     7581 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/revoke_entry.py
--rw-rw-r--   0 root         (0) root         (0)     8281 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/revoke_item.py
--rw-rw-r--   0 root         (0) root         (0)     6455 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/revoke_item_summary.py
--rw-rw-r--   0 root         (0) root         (0)     6305 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/revoke_result.py
--rw-rw-r--   0 root         (0) root         (0)     4535 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/revoke_use_count_request.py
--rw-rw-r--   0 root         (0) root         (0)     6429 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/reward_condition.py
--rw-rw-r--   0 root         (0) root         (0)     9914 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/reward_create.py
--rw-rw-r--   0 root         (0) root         (0)    12718 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/reward_info.py
--rw-rw-r--   0 root         (0) root         (0)     7585 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/reward_item.py
--rw-rw-r--   0 root         (0) root         (0)     8787 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/reward_migration_result.py
--rw-rw-r--   0 root         (0) root         (0)     4883 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/reward_paging_sliced_result.py
--rw-rw-r--   0 root         (0) root         (0)     9914 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/reward_update.py
--rw-rw-r--   0 root         (0) root         (0)    11795 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/rewards_request.py
--rw-rw-r--   0 root         (0) root         (0)     4293 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/sale_config.py
--rw-rw-r--   0 root         (0) root         (0)    12693 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/section_create.py
--rw-rw-r--   0 root         (0) root         (0)    15735 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/section_info.py
--rw-rw-r--   0 root         (0) root         (0)     4116 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/section_item.py
--rw-rw-r--   0 root         (0) root         (0)     4931 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/section_paging_sliced_result.py
--rw-rw-r--   0 root         (0) root         (0)     7158 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/section_plugin_config_info.py
--rw-rw-r--   0 root         (0) root         (0)     6381 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/section_plugin_config_update.py
--rw-rw-r--   0 root         (0) root         (0)    12693 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/section_update.py
--rw-rw-r--   0 root         (0) root         (0)     4851 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/service_plugin_config_info.py
--rw-rw-r--   0 root         (0) root         (0)     4124 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/service_plugin_config_update.py
--rw-rw-r--   0 root         (0) root         (0)     7732 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/slide.py
--rw-rw-r--   0 root         (0) root         (0)    26967 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/stackable_entitlement_info.py
--rw-rw-r--   0 root         (0) root         (0)     4302 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/steam_achievement.py
--rw-rw-r--   0 root         (0) root         (0)     5217 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/steam_achievement_update_request.py
--rw-rw-r--   0 root         (0) root         (0)     4412 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/steam_dlc_sync_request.py
--rw-rw-r--   0 root         (0) root         (0)     7715 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/steam_iap_config.py
--rw-rw-r--   0 root         (0) root         (0)     5584 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/steam_iap_config_info.py
--rw-rw-r--   0 root         (0) root         (0)     4963 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/steam_iap_config_request.py
--rw-rw-r--   0 root         (0) root         (0)     8134 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/steam_sync_request.py
--rw-rw-r--   0 root         (0) root         (0)     6900 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/store_backup_info.py
--rw-rw-r--   0 root         (0) root         (0)     8017 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/store_create.py
--rw-rw-r--   0 root         (0) root         (0)    11835 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/store_info.py
--rw-rw-r--   0 root         (0) root         (0)     8017 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/store_update.py
--rw-rw-r--   0 root         (0) root         (0)     8277 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/stream_event.py
--rw-rw-r--   0 root         (0) root         (0)     9229 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/stream_event_body.py
--rw-rw-r--   0 root         (0) root         (0)     6700 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/stripe_config.py
--rw-rw-r--   0 root         (0) root         (0)     7872 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/sub_item_available_price.py
--rw-rw-r--   0 root         (0) root         (0)     3741 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/subscribable.py
--rw-rw-r--   0 root         (0) root         (0)     7459 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/subscribe_request.py
--rw-rw-r--   0 root         (0) root         (0)    15341 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/subscription_activity_info.py
--rw-rw-r--   0 root         (0) root         (0)     5228 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/subscription_activity_paging_sliced_result.py
--rw-rw-r--   0 root         (0) root         (0)    37996 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/subscription_info.py
--rw-rw-r--   0 root         (0) root         (0)     5011 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/subscription_paging_sliced_result.py
--rw-rw-r--   0 root         (0) root         (0)    10201 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/subscription_summary.py
--rw-rw-r--   0 root         (0) root         (0)     5767 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/tax_result.py
--rw-rw-r--   0 root         (0) root         (0)     4205 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/test_result.py
--rw-rw-r--   0 root         (0) root         (0)     4359 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/ticket_acquire_request.py
--rw-rw-r--   0 root         (0) root         (0)     3837 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/ticket_acquire_result.py
--rw-rw-r--   0 root         (0) root         (0)     4505 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/ticket_booth_id.py
--rw-rw-r--   0 root         (0) root         (0)     3956 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/ticket_dynamic_info.py
--rw-rw-r--   0 root         (0) root         (0)     3843 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/ticket_sale_decrement_request.py
--rw-rw-r--   0 root         (0) root         (0)     4432 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/ticket_sale_increment_request.py
--rw-rw-r--   0 root         (0) root         (0)     4598 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/ticket_sale_increment_result.py
--rw-rw-r--   0 root         (0) root         (0)     5351 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/time_limited_balance.py
--rw-rw-r--   0 root         (0) root         (0)     4338 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/timed_ownership.py
--rw-rw-r--   0 root         (0) root         (0)     4919 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/tls_config.py
--rw-rw-r--   0 root         (0) root         (0)     5143 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/trade_action_paging_sliced_result.py
--rw-rw-r--   0 root         (0) root         (0)     9868 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/trade_chain_action_history_info.py
--rw-rw-r--   0 root         (0) root         (0)     7466 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/trade_chained_action_commit_request.py
--rw-rw-r--   0 root         (0) root         (0)    35344 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/trade_notification.py
--rw-rw-r--   0 root         (0) root         (0)    19184 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/transaction.py
--rw-rw-r--   0 root         (0) root         (0)     5990 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/transaction_amount_details.py
--rw-rw-r--   0 root         (0) root         (0)     6178 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/twitch_iap_config_info.py
--rw-rw-r--   0 root         (0) root         (0)     5562 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/twitch_iap_config_request.py
--rw-rw-r--   0 root         (0) root         (0)     5400 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/twitch_sync_request.py
--rw-rw-r--   0 root         (0) root         (0)     5963 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/twitch_sync_result.py
--rw-rw-r--   0 root         (0) root         (0)     9058 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/user_dlc.py
--rw-rw-r--   0 root         (0) root         (0)    18486 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/user_dlc_record.py
--rw-rw-r--   0 root         (0) root         (0)     5628 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/validation_error_entity.py
--rw-rw-r--   0 root         (0) root         (0)     5463 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/view_create.py
--rw-rw-r--   0 root         (0) root         (0)     9919 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/view_info.py
--rw-rw-r--   0 root         (0) root         (0)     5583 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/view_update.py
--rw-rw-r--   0 root         (0) root         (0)    13479 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/wallet_info.py
--rw-rw-r--   0 root         (0) root         (0)     4883 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/wallet_paging_sliced_result.py
--rw-rw-r--   0 root         (0) root         (0)     5065 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/wallet_revocation_config.py
--rw-rw-r--   0 root         (0) root         (0)    13000 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/wallet_transaction_info.py
--rw-rw-r--   0 root         (0) root         (0)     5133 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/wallet_transaction_paging_sliced_result.py
--rw-rw-r--   0 root         (0) root         (0)     6438 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/wx_pay_config_info.py
--rw-rw-r--   0 root         (0) root         (0)     5784 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/wx_pay_config_request.py
--rw-rw-r--   0 root         (0) root         (0)     6781 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/xbl_achievement_update_request.py
--rw-rw-r--   0 root         (0) root         (0)     3824 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/xbl_dlc_sync_request.py
--rw-rw-r--   0 root         (0) root         (0)     6614 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/xbl_iap_config_info.py
--rw-rw-r--   0 root         (0) root         (0)     3941 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/xbl_iap_config_request.py
--rw-rw-r--   0 root         (0) root         (0)     6079 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/xbl_reconcile_request.py
--rw-rw-r--   0 root         (0) root         (0)     7420 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/xbl_reconcile_result.py
--rw-rw-r--   0 root         (0) root         (0)     4259 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/xbl_user_achievements.py
--rw-rw-r--   0 root         (0) root         (0)     6172 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/xbl_user_session_request.py
--rw-rw-r--   0 root         (0) root         (0)     4513 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/xbox_achievement.py
--rw-rw-r--   0 root         (0) root         (0)     7028 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/xsolla_config.py
--rw-rw-r--   0 root         (0) root         (0)     6638 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/xsolla_paywall_config.py
--rw-rw-r--   0 root         (0) root         (0)     6974 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/xsolla_paywall_config_request.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:40:41.220810 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/
--rw-rw-r--   0 root         (0) root         (0)      437 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:40:41.220810 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/achievement_platform/
--rw-rw-r--   0 root         (0) root         (0)      668 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/achievement_platform/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7746 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/achievement_platform/get_xbl_user_achievements.py
--rw-rw-r--   0 root         (0) root         (0)     8252 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/achievement_platform/unlock_steam_user_achievement.py
--rw-rw-r--   0 root         (0) root         (0)     7840 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/achievement_platform/update_xbl_user_achievement.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:40:41.220810 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/anonymization/
--rw-rw-r--   0 root         (0) root         (0)      938 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/anonymization/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6449 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/anonymization/anonymize_campaign.py
--rw-rw-r--   0 root         (0) root         (0)     6483 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/anonymization/anonymize_entitlement.py
--rw-rw-r--   0 root         (0) root         (0)     6468 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/anonymization/anonymize_fulfillment.py
--rw-rw-r--   0 root         (0) root         (0)     6466 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/anonymization/anonymize_integration.py
--rw-rw-r--   0 root         (0) root         (0)     6427 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/anonymization/anonymize_order.py
--rw-rw-r--   0 root         (0) root         (0)     6461 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/anonymization/anonymize_payment.py
--rw-rw-r--   0 root         (0) root         (0)     6333 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/anonymization/anonymize_revocation.py
--rw-rw-r--   0 root         (0) root         (0)     6511 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/anonymization/anonymize_subscription.py
--rw-rw-r--   0 root         (0) root         (0)     6443 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/anonymization/anonymize_wallet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:40:41.224810 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/campaign/
--rw-rw-r--   0 root         (0) root         (0)     1106 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/campaign/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     9255 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/campaign/apply_user_redemption.py
--rw-rw-r--   0 root         (0) root         (0)     7681 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/campaign/bulk_disable_codes.py
--rw-rw-r--   0 root         (0) root         (0)     7568 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/campaign/bulk_enable_codes.py
--rw-rw-r--   0 root         (0) root         (0)     7460 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/campaign/create_campaign.py
--rw-rw-r--   0 root         (0) root         (0)     8379 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/campaign/create_codes.py
--rw-rw-r--   0 root         (0) root         (0)     6850 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/campaign/disable_code.py
--rw-rw-r--   0 root         (0) root         (0)     7339 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/campaign/download.py
--rw-rw-r--   0 root         (0) root         (0)     6614 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/campaign/enable_code.py
--rw-rw-r--   0 root         (0) root         (0)     6793 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/campaign/get_campaign.py
--rw-rw-r--   0 root         (0) root         (0)     6928 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/campaign/get_campaign_dynamic.py
--rw-rw-r--   0 root         (0) root         (0)     8331 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/campaign/get_code.py
--rw-rw-r--   0 root         (0) root         (0)     8845 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/campaign/query_campaigns.py
--rw-rw-r--   0 root         (0) root         (0)    10629 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/campaign/query_codes.py
--rw-rw-r--   0 root         (0) root         (0)     9870 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/campaign/query_redeem_history.py
--rw-rw-r--   0 root         (0) root         (0)     8643 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/campaign/update_campaign.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:40:41.224810 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/catalog_changes/
--rw-rw-r--   0 root         (0) root         (0)     1503 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/catalog_changes/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    13345 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/catalog_changes/get_statistic.py
--rw-rw-r--   0 root         (0) root         (0)     7048 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/catalog_changes/publish_all.py
--rw-rw-r--   0 root         (0) root         (0)     7501 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/catalog_changes/publish_selected.py
--rw-rw-r--   0 root         (0) root         (0)    19166 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/catalog_changes/query_changes.py
--rw-rw-r--   0 root         (0) root         (0)     6685 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/catalog_changes/select_all_records.py
--rw-rw-r--   0 root         (0) root         (0)    14608 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/catalog_changes/select_all_records_by_criteria.py
--rw-rw-r--   0 root         (0) root         (0)     7640 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/catalog_changes/select_record.py
--rw-rw-r--   0 root         (0) root         (0)     6704 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/catalog_changes/unselect_all_records.py
--rw-rw-r--   0 root         (0) root         (0)     8651 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/catalog_changes/unselect_record.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:40:41.224810 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/category/
--rw-rw-r--   0 root         (0) root         (0)     1169 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/category/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     9467 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/category/create_category.py
--rw-rw-r--   0 root         (0) root         (0)     8263 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/category/delete_category.py
--rw-rw-r--   0 root         (0) root         (0)     8043 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/category/download_categories.py
--rw-rw-r--   0 root         (0) root         (0)     7885 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/category/get_category.py
--rw-rw-r--   0 root         (0) root         (0)     7681 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/category/get_child_categories.py
--rw-rw-r--   0 root         (0) root         (0)     7737 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/category/get_descendant_categories.py
--rw-rw-r--   0 root         (0) root         (0)     6673 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/category/get_root_categories.py
--rw-rw-r--   0 root         (0) root         (0)     6765 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/category/list_categories_basic.py
--rw-rw-r--   0 root         (0) root         (0)     8791 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/category/public_get_category.py
--rw-rw-r--   0 root         (0) root         (0)     8580 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/category/public_get_child_categories.py
--rw-rw-r--   0 root         (0) root         (0)     8641 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/category/public_get_descendant_c_c5054d.py
--rw-rw-r--   0 root         (0) root         (0)     7590 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/category/public_get_root_categories.py
--rw-rw-r--   0 root         (0) root         (0)    10039 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/category/update_category.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:40:41.224810 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/clawback/
--rw-rw-r--   0 root         (0) root         (0)      761 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/clawback/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6726 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/clawback/mock_play_station_stream_event.py
--rw-rw-r--   0 root         (0) root         (0)    13505 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/clawback/query_iap_clawback_history.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:40:41.228810 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/currency/
--rw-rw-r--   0 root         (0) root         (0)      998 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/currency/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7640 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/currency/create_currency.py
--rw-rw-r--   0 root         (0) root         (0)     6901 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/currency/delete_currency.py
--rw-rw-r--   0 root         (0) root         (0)     7029 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/currency/get_currency_config.py
--rw-rw-r--   0 root         (0) root         (0)     7015 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/currency/get_currency_summary.py
--rw-rw-r--   0 root         (0) root         (0)     7232 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/currency/list_currencies.py
--rw-rw-r--   0 root         (0) root         (0)     7072 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/currency/public_list_currencies.py
--rw-rw-r--   0 root         (0) root         (0)     8591 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/currency/update_currency.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:40:41.228810 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/dlc/
--rw-rw-r--   0 root         (0) root         (0)     1589 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/dlc/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5583 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/dlc/delete_dlc_item_config.py
--rw-rw-r--   0 root         (0) root         (0)     5625 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/dlc/delete_platform_dlc_config.py
--rw-rw-r--   0 root         (0) root         (0)     7638 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/dlc/ge_dlc_durable_reward_s_f83f8a.py
--rw-rw-r--   0 root         (0) root         (0)     5950 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/dlc/get_dlc_item_config.py
--rw-rw-r--   0 root         (0) root         (0)     6034 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/dlc/get_platform_dlc_config.py
--rw-rw-r--   0 root         (0) root         (0)     7755 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/dlc/get_user_dlc.py
--rw-rw-r--   0 root         (0) root         (0)     7685 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/dlc/get_user_dlc_by_platform.py
--rw-rw-r--   0 root         (0) root         (0)     8603 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/dlc/public_sync_psn_dlc_inv_429118.py
--rw-rw-r--   0 root         (0) root         (0)     8106 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/dlc/public_sync_psn_dlc_inventory.py
--rw-rw-r--   0 root         (0) root         (0)     7883 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/dlc/sync_epic_game_dlc.py
--rw-rw-r--   0 root         (0) root         (0)     6535 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/dlc/sync_oculus_dlc.py
--rw-rw-r--   0 root         (0) root         (0)     7703 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/dlc/sync_steam_dlc.py
--rw-rw-r--   0 root         (0) root         (0)     7766 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/dlc/sync_xbox_dlc.py
--rw-rw-r--   0 root         (0) root         (0)     7905 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/dlc/update_dlc_item_config.py
--rw-rw-r--   0 root         (0) root         (0)     7536 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/dlc/update_platform_dlc_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:40:41.232810 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/
--rw-rw-r--   0 root         (0) root         (0)     6770 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    10698 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/consume_user_entitlement.py
--rw-rw-r--   0 root         (0) root         (0)     8345 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/disable_user_entitlement.py
--rw-rw-r--   0 root         (0) root         (0)     5910 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/enable_entitlement_orig_c90935.py
--rw-rw-r--   0 root         (0) root         (0)     8418 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/enable_user_entitlement.py
--rw-rw-r--   0 root         (0) root         (0)     8639 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/exists_any_user_active__9d3175.py
--rw-rw-r--   0 root         (0) root         (0)    10362 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/exists_any_user_active__fca16a.py
--rw-rw-r--   0 root         (0) root         (0)     6945 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/get_entitlement.py
--rw-rw-r--   0 root         (0) root         (0)     6926 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/get_entitlement_config_info.py
--rw-rw-r--   0 root         (0) root         (0)     7543 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/get_platform_entitlemen_32e517.py
--rw-rw-r--   0 root         (0) root         (0)     8562 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/get_user_active_entitle_d52ca8.py
--rw-rw-r--   0 root         (0) root         (0)     8757 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/get_user_app_entitlemen_2375db.py
--rw-rw-r--   0 root         (0) root         (0)     7471 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/get_user_app_entitlemen_282639.py
--rw-rw-r--   0 root         (0) root         (0)     7782 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/get_user_entitlement.py
--rw-rw-r--   0 root         (0) root         (0)    11433 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/get_user_entitlement_by_8ab4a0.py
--rw-rw-r--   0 root         (0) root         (0)    11292 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/get_user_entitlement_by_sku.py
--rw-rw-r--   0 root         (0) root         (0)     7589 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/get_user_entitlement_histories.py
--rw-rw-r--   0 root         (0) root         (0)     8625 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/get_user_entitlement_ow_5a8354.py
--rw-rw-r--   0 root         (0) root         (0)    10110 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/get_user_entitlement_ow_dab0ca.py
--rw-rw-r--   0 root         (0) root         (0)    10236 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/get_user_entitlement_ow_ec2b70.py
--rw-rw-r--   0 root         (0) root         (0)     7447 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/grant_entitlements.py
--rw-rw-r--   0 root         (0) root         (0)     8538 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/grant_user_entitlement.py
--rw-rw-r--   0 root         (0) root         (0)     9104 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/pre_check_revoke_user_e_124298.py
--rw-rw-r--   0 root         (0) root         (0)    11214 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_consume_user_ent_7254fa.py
--rw-rw-r--   0 root         (0) root         (0)     8764 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_exists_any_my_ac_dbd2a5.py
--rw-rw-r--   0 root         (0) root         (0)     9565 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_exists_any_user__3977e5.py
--rw-rw-r--   0 root         (0) root         (0)    10027 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_get_entitlement__3fdfe7.py
--rw-rw-r--   0 root         (0) root         (0)     6830 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_get_my_app_entit_4deb3f.py
--rw-rw-r--   0 root         (0) root         (0)     8750 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_get_my_entitleme_22c2fd.py
--rw-rw-r--   0 root         (0) root         (0)     8854 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_get_my_entitleme_cb2911.py
--rw-rw-r--   0 root         (0) root         (0)     7839 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_get_user_app_ent_1e800f.py
--rw-rw-r--   0 root         (0) root         (0)     7503 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_get_user_app_ent_53d109.py
--rw-rw-r--   0 root         (0) root         (0)     7777 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_get_user_entitle_408425.py
--rw-rw-r--   0 root         (0) root         (0)     9629 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_get_user_entitle_815992.py
--rw-rw-r--   0 root         (0) root         (0)     9764 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_get_user_entitle_b1671e.py
--rw-rw-r--   0 root         (0) root         (0)     9428 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_get_user_entitle_b313cf.py
--rw-rw-r--   0 root         (0) root         (0)     8961 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_get_user_entitle_bb9230.py
--rw-rw-r--   0 root         (0) root         (0)     9305 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_get_user_entitle_ee3005.py
--rw-rw-r--   0 root         (0) root         (0)     7814 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_get_user_entitlement.py
--rw-rw-r--   0 root         (0) root         (0)     9711 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_query_user_entit_2398e5.py
--rw-rw-r--   0 root         (0) root         (0)    14302 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_query_user_entitlements.py
--rw-rw-r--   0 root         (0) root         (0)    10507 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_sell_user_entitlement.py
--rw-rw-r--   0 root         (0) root         (0)    10271 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_split_user_entitlement.py
--rw-rw-r--   0 root         (0) root         (0)    10902 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_transfer_user_en_c358c0.py
--rw-rw-r--   0 root         (0) root         (0)    15627 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/query_entitlements.py
--rw-rw-r--   0 root         (0) root         (0)     9420 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/query_entitlements_1.py
--rw-rw-r--   0 root         (0) root         (0)    18615 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/query_user_entitlements.py
--rw-rw-r--   0 root         (0) root         (0)    10575 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/query_user_entitlements_22cea1.py
--rw-rw-r--   0 root         (0) root         (0)     6654 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/revoke_all_entitlements.py
--rw-rw-r--   0 root         (0) root         (0)     7122 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/revoke_entitlements.py
--rw-rw-r--   0 root         (0) root         (0)     9179 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/revoke_use_count.py
--rw-rw-r--   0 root         (0) root         (0)     7833 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/revoke_user_entitlement.py
--rw-rw-r--   0 root         (0) root         (0)     9201 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/revoke_user_entitlement_491388.py
--rw-rw-r--   0 root         (0) root         (0)     7650 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/revoke_user_entitlements.py
--rw-rw-r--   0 root         (0) root         (0)    10371 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/sell_user_entitlement.py
--rw-rw-r--   0 root         (0) root         (0)     9214 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/update_platform_entitle_7fbd45.py
--rw-rw-r--   0 root         (0) root         (0)     9754 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/update_user_entitlement.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:40:41.232810 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/fulfillment/
--rw-rw-r--   0 root         (0) root         (0)      909 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/fulfillment/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8555 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/fulfillment/fulfill_item.py
--rw-rw-r--   0 root         (0) root         (0)     8438 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/fulfillment/fulfill_rewards.py
--rw-rw-r--   0 root         (0) root         (0)     8621 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/fulfillment/fulfill_rewards_v2.py
--rw-rw-r--   0 root         (0) root         (0)     8456 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/fulfillment/pre_check_fulfill_item.py
--rw-rw-r--   0 root         (0) root         (0)     9744 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/fulfillment/public_redeem_code.py
--rw-rw-r--   0 root         (0) root         (0)     9559 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/fulfillment/query_fulfillment_histories.py
--rw-rw-r--   0 root         (0) root         (0)     9368 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/fulfillment/redeem_code.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:40:41.232810 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/fulfillment_script/
--rw-rw-r--   0 root         (0) root         (0)      777 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/fulfillment_script/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7307 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/fulfillment_script/create_fulfillment_script.py
--rw-rw-r--   0 root         (0) root         (0)     5391 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/fulfillment_script/delete_fulfillment_script.py
--rw-rw-r--   0 root         (0) root         (0)     5870 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/fulfillment_script/get_fulfillment_script.py
--rw-rw-r--   0 root         (0) root         (0)     4720 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/fulfillment_script/list_fulfillment_scripts.py
--rw-rw-r--   0 root         (0) root         (0)     7015 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/fulfillment_script/update_fulfillment_script.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:40:41.240810 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/
--rw-rw-r--   0 root         (0) root         (0)     3689 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5550 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/delete_apple_iap_config.py
--rw-rw-r--   0 root         (0) root         (0)     5588 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/delete_epic_games_iap_config.py
--rw-rw-r--   0 root         (0) root         (0)     5559 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/delete_google_iap_config.py
--rw-rw-r--   0 root         (0) root         (0)     5583 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/delete_iap_item_config.py
--rw-rw-r--   0 root         (0) root         (0)     5559 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/delete_oculus_iap_config.py
--rw-rw-r--   0 root         (0) root         (0)     5604 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/delete_playstation_iap_config.py
--rw-rw-r--   0 root         (0) root         (0)     5550 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/delete_steam_iap_config.py
--rw-rw-r--   0 root         (0) root         (0)     5559 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/delete_twitch_iap_config.py
--rw-rw-r--   0 root         (0) root         (0)     5527 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/delete_xbl_ap_config.py
--rw-rw-r--   0 root         (0) root         (0)     5688 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/get_apple_iap_config.py
--rw-rw-r--   0 root         (0) root         (0)     5750 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/get_epic_games_iap_config.py
--rw-rw-r--   0 root         (0) root         (0)     5703 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/get_google_iap_config.py
--rw-rw-r--   0 root         (0) root         (0)     5950 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/get_iap_item_config.py
--rw-rw-r--   0 root         (0) root         (0)     7531 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/get_iap_item_mapping.py
--rw-rw-r--   0 root         (0) root         (0)     5702 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/get_oculus_iap_config.py
--rw-rw-r--   0 root         (0) root         (0)     5778 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/get_play_station_iap_config.py
--rw-rw-r--   0 root         (0) root         (0)     5668 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/get_steam_iap_config.py
--rw-rw-r--   0 root         (0) root         (0)     5703 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/get_twitch_iap_config.py
--rw-rw-r--   0 root         (0) root         (0)     5661 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/get_xbl_iap_config.py
--rw-rw-r--   0 root         (0) root         (0)     8538 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/mock_fulfill_iap_item.py
--rw-rw-r--   0 root         (0) root         (0)     9059 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/public_fulfill_apple_iap_item.py
--rw-rw-r--   0 root         (0) root         (0)     9624 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/public_fulfill_google_iap_item.py
--rw-rw-r--   0 root         (0) root         (0)     9031 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/public_reconcile_play_s_6be6c0.py
--rw-rw-r--   0 root         (0) root         (0)     8548 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/public_reconcile_play_s_7ac4de.py
--rw-rw-r--   0 root         (0) root         (0)     6520 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/query_all_user_iap_orders.py
--rw-rw-r--   0 root         (0) root         (0)    12664 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/query_user_iap_consume_history.py
--rw-rw-r--   0 root         (0) root         (0)    13319 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/query_user_iap_orders.py
--rw-rw-r--   0 root         (0) root         (0)     8295 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/sync_epic_games_inventory.py
--rw-rw-r--   0 root         (0) root         (0)     6959 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/sync_oculus_consumable__f6c91d.py
--rw-rw-r--   0 root         (0) root         (0)     7977 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/sync_steam_inventory.py
--rw-rw-r--   0 root         (0) root         (0)     8023 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/sync_twitch_drops_entit_0c09ca.py
--rw-rw-r--   0 root         (0) root         (0)     7284 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/sync_twitch_drops_entitlement.py
--rw-rw-r--   0 root         (0) root         (0)     8133 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/sync_xbox_inventory.py
--rw-rw-r--   0 root         (0) root         (0)     6899 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/update_apple_iap_config.py
--rw-rw-r--   0 root         (0) root         (0)     6998 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/update_epic_games_iap_config.py
--rw-rw-r--   0 root         (0) root         (0)     6923 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/update_google_iap_config.py
--rw-rw-r--   0 root         (0) root         (0)     6685 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/update_google_p12_file.py
--rw-rw-r--   0 root         (0) root         (0)     7921 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/update_iap_item_config.py
--rw-rw-r--   0 root         (0) root         (0)     6922 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/update_oculus_iap_config.py
--rw-rw-r--   0 root         (0) root         (0)     7408 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/update_playstation_iap_config.py
--rw-rw-r--   0 root         (0) root         (0)     7259 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/update_steam_iap_config.py
--rw-rw-r--   0 root         (0) root         (0)     6923 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/update_twitch_iap_config.py
--rw-rw-r--   0 root         (0) root         (0)     7544 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/update_xbl_bp_cert_file.py
--rw-rw-r--   0 root         (0) root         (0)     6851 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/update_xbl_iap_config.py
--rw-rw-r--   0 root         (0) root         (0)     5825 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/validate_existed_playst_881975.py
--rw-rw-r--   0 root         (0) root         (0)     7028 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/validate_playstation_ia_7dc74e.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:40:41.240810 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/invoice/
--rw-rw-r--   0 root         (0) root         (0)      788 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/invoice/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    10715 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/invoice/download_invoice_details.py
--rw-rw-r--   0 root         (0) root         (0)    11149 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/invoice/generate_invoice_summary.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:40:41.244810 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/
--rw-rw-r--   0 root         (0) root         (0)     3746 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8019 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/acquire_item.py
--rw-rw-r--   0 root         (0) root         (0)    10509 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/bulk_get_locale_items.py
--rw-rw-r--   0 root         (0) root         (0)     9407 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/bulk_update_region_data.py
--rw-rw-r--   0 root         (0) root         (0)    17365 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/create_item.py
--rw-rw-r--   0 root         (0) root         (0)     6839 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/create_item_type_config.py
--rw-rw-r--   0 root         (0) root         (0)     8816 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/defeature_item.py
--rw-rw-r--   0 root         (0) root         (0)     8999 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/delete_item.py
--rw-rw-r--   0 root         (0) root         (0)     5693 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/delete_item_type_config.py
--rw-rw-r--   0 root         (0) root         (0)     7993 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/disable_item.py
--rw-rw-r--   0 root         (0) root         (0)     7982 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/enable_item.py
--rw-rw-r--   0 root         (0) root         (0)     8773 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/feature_item.py
--rw-rw-r--   0 root         (0) root         (0)     8170 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/get_app.py
--rw-rw-r--   0 root         (0) root         (0)     6033 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/get_available_predicate_types.py
--rw-rw-r--   0 root         (0) root         (0)     7594 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/get_bulk_item_id_by_skus.py
--rw-rw-r--   0 root         (0) root         (0)    10209 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/get_estimated_price.py
--rw-rw-r--   0 root         (0) root         (0)     8784 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/get_item.py
--rw-rw-r--   0 root         (0) root         (0)     8823 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/get_item_by_app_id.py
--rw-rw-r--   0 root         (0) root         (0)     8707 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/get_item_by_sku.py
--rw-rw-r--   0 root         (0) root         (0)     6810 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/get_item_dynamic_data.py
--rw-rw-r--   0 root         (0) root         (0)     8756 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/get_item_id_by_sku.py
--rw-rw-r--   0 root         (0) root         (0)     5819 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/get_item_type_config.py
--rw-rw-r--   0 root         (0) root         (0)     8718 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/get_items.py
--rw-rw-r--   0 root         (0) root         (0)    11585 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/get_locale_item.py
--rw-rw-r--   0 root         (0) root         (0)    11517 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/get_locale_item_by_sku.py
--rw-rw-r--   0 root         (0) root         (0)     7904 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/list_basic_items_by_features.py
--rw-rw-r--   0 root         (0) root         (0)     4756 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/list_item_type_configs.py
--rw-rw-r--   0 root         (0) root         (0)    10956 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/public_bulk_get_items.py
--rw-rw-r--   0 root         (0) root         (0)     9370 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/public_get_app.py
--rw-rw-r--   0 root         (0) root         (0)     8715 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/public_get_estimated_price.py
--rw-rw-r--   0 root         (0) root         (0)    12021 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/public_get_item.py
--rw-rw-r--   0 root         (0) root         (0)     9591 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/public_get_item_by_app_id.py
--rw-rw-r--   0 root         (0) root         (0)    10802 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/public_get_item_by_sku.py
--rw-rw-r--   0 root         (0) root         (0)     6645 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/public_get_item_dynamic_data.py
--rw-rw-r--   0 root         (0) root         (0)    21639 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/public_query_items.py
--rw-rw-r--   0 root         (0) root         (0)    14270 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/public_search_items.py
--rw-rw-r--   0 root         (0) root         (0)     7472 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/public_validate_item_pu_bd546e.py
--rw-rw-r--   0 root         (0) root         (0)    22154 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/query_items.py
--rw-rw-r--   0 root         (0) root         (0)    25368 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/query_items_1.py
--rw-rw-r--   0 root         (0) root         (0)    12202 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/query_uncategorized_items.py
--rw-rw-r--   0 root         (0) root         (0)     8212 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/return_item.py
--rw-rw-r--   0 root         (0) root         (0)     7659 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/search_item_type_config.py
--rw-rw-r--   0 root         (0) root         (0)    13681 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/search_items.py
--rw-rw-r--   0 root         (0) root         (0)     9757 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/sync_in_game_item.py
--rw-rw-r--   0 root         (0) root         (0)    10831 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/update_app.py
--rw-rw-r--   0 root         (0) root         (0)    18436 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/update_item.py
--rw-rw-r--   0 root         (0) root         (0)     9735 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/update_item_purchase_condition.py
--rw-rw-r--   0 root         (0) root         (0)     7676 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/update_item_type_config.py
--rw-rw-r--   0 root         (0) root         (0)     9145 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/validate_item_purchase__929f78.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:40:41.244810 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/key_group/
--rw-rw-r--   0 root         (0) root         (0)      895 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/key_group/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7465 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/key_group/create_key_group.py
--rw-rw-r--   0 root         (0) root         (0)     6808 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/key_group/get_key_group.py
--rw-rw-r--   0 root         (0) root         (0)     7055 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/key_group/get_key_group_by_booth_name.py
--rw-rw-r--   0 root         (0) root         (0)     6945 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/key_group/get_key_group_dynamic.py
--rw-rw-r--   0 root         (0) root         (0)     9347 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/key_group/list_keys.py
--rw-rw-r--   0 root         (0) root         (0)     8840 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/key_group/query_key_groups.py
--rw-rw-r--   0 root         (0) root         (0)     8665 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/key_group/update_key_group.py
--rw-rw-r--   0 root         (0) root         (0)     8076 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/key_group/upload_keys.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:40:41.244810 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/order/
--rw-rw-r--   0 root         (0) root         (0)     1820 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/order/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    11472 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/order/admin_create_user_order.py
--rw-rw-r--   0 root         (0) root         (0)     7456 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/order/count_of_purchased_item.py
--rw-rw-r--   0 root         (0) root         (0)     7781 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/order/download_user_order_receipt.py
--rw-rw-r--   0 root         (0) root         (0)     8442 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/order/fulfill_user_order.py
--rw-rw-r--   0 root         (0) root         (0)     6602 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/order/get_order.py
--rw-rw-r--   0 root         (0) root         (0)     5662 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/order/get_order_statistics.py
--rw-rw-r--   0 root         (0) root         (0)     7449 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/order/get_user_order.py
--rw-rw-r--   0 root         (0) root         (0)     7272 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/order/get_user_order_grant.py
--rw-rw-r--   0 root         (0) root         (0)     7324 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/order/get_user_order_histories.py
--rw-rw-r--   0 root         (0) root         (0)     8687 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/order/process_user_order_noti_fdd9f8.py
--rw-rw-r--   0 root         (0) root         (0)     7817 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/order/public_cancel_user_order.py
--rw-rw-r--   0 root         (0) root         (0)    11467 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/order/public_create_user_order.py
--rw-rw-r--   0 root         (0) root         (0)     7813 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/order/public_download_user_or_6ea3e8.py
--rw-rw-r--   0 root         (0) root         (0)     7515 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/order/public_get_user_order.py
--rw-rw-r--   0 root         (0) root         (0)     7342 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/order/public_get_user_order_h_063753.py
--rw-rw-r--   0 root         (0) root         (0)    10777 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/order/public_query_user_orders.py
--rw-rw-r--   0 root         (0) root         (0)    13760 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/order/query_orders.py
--rw-rw-r--   0 root         (0) root         (0)    10727 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/order/query_user_orders.py
--rw-rw-r--   0 root         (0) root         (0)     8393 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/order/refund_order.py
--rw-rw-r--   0 root         (0) root         (0)     9211 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/order/update_user_order_status.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:40:41.244810 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/order_dedicated/
--rw-rw-r--   0 root         (0) root         (0)      506 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/order_dedicated/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7276 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/order_dedicated/sync_orders.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:40:41.248810 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment/
--rw-rw-r--   0 root         (0) root         (0)     1346 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     9065 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment/charge_payment_order.py
--rw-rw-r--   0 root         (0) root         (0)    10139 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment/create_user_payment_order.py
--rw-rw-r--   0 root         (0) root         (0)     7004 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment/get_payment_order.py
--rw-rw-r--   0 root         (0) root         (0)     7189 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment/get_payment_order_charg_9acbf8.py
--rw-rw-r--   0 root         (0) root         (0)     6651 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment/list_ext_order_no_by_ext_tx_id.py
--rw-rw-r--   0 root         (0) root         (0)    15334 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment/query_payment_notifications.py
--rw-rw-r--   0 root         (0) root         (0)    11380 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment/query_payment_orders.py
--rw-rw-r--   0 root         (0) root         (0)     9723 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment/refund_user_payment_order.py
--rw-rw-r--   0 root         (0) root         (0)     8957 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment/simulate_payment_order__cf0fbc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:40:41.248810 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_account/
--rw-rw-r--   0 root         (0) root         (0)      705 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_account/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8283 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_account/public_delete_payment_account.py
--rw-rw-r--   0 root         (0) root         (0)     6627 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_account/public_get_payment_accounts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:40:41.248810 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_callback_config/
--rw-rw-r--   0 root         (0) root         (0)      608 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_callback_config/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6220 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_callback_config/get_payment_callback_config.py
--rw-rw-r--   0 root         (0) root         (0)     7166 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_callback_config/update_payment_callback_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:40:41.252810 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_config/
--rw-rw-r--   0 root         (0) root         (0)     2494 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_config/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7826 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_config/create_payment_provider_config.py
--rw-rw-r--   0 root         (0) root         (0)     7043 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_config/debug_matched_payment_m_9bf142.py
--rw-rw-r--   0 root         (0) root         (0)     7038 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_config/debug_matched_payment_p_02dcf1.py
--rw-rw-r--   0 root         (0) root         (0)     5793 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_config/delete_payment_provider_config.py
--rw-rw-r--   0 root         (0) root         (0)     4746 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_config/get_aggregate_payment_p_41c63c.py
--rw-rw-r--   0 root         (0) root         (0)     5954 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_config/get_payment_merchant_config.py
--rw-rw-r--   0 root         (0) root         (0)     4751 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_config/get_payment_tax_config.py
--rw-rw-r--   0 root         (0) root         (0)     4730 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_config/get_special_payment_providers.py
--rw-rw-r--   0 root         (0) root         (0)     8328 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_config/query_payment_provider_config.py
--rw-rw-r--   0 root         (0) root         (0)     7090 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_config/test_adyen_config.py
--rw-rw-r--   0 root         (0) root         (0)     6868 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_config/test_adyen_config_by_id.py
--rw-rw-r--   0 root         (0) root         (0)     6903 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_config/test_ali_pay_config.py
--rw-rw-r--   0 root         (0) root         (0)     6969 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_config/test_ali_pay_config_by_id.py
--rw-rw-r--   0 root         (0) root         (0)     6921 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_config/test_checkout_config.py
--rw-rw-r--   0 root         (0) root         (0)     6900 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_config/test_checkout_config_by_id.py
--rw-rw-r--   0 root         (0) root         (0)     6926 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_config/test_pay_pal_config.py
--rw-rw-r--   0 root         (0) root         (0)     6924 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_config/test_pay_pal_config_by_id.py
--rw-rw-r--   0 root         (0) root         (0)     6973 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_config/test_stripe_config.py
--rw-rw-r--   0 root         (0) root         (0)     6878 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_config/test_stripe_config_by_id.py
--rw-rw-r--   0 root         (0) root         (0)     5995 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_config/test_wx_pay_config.py
--rw-rw-r--   0 root         (0) root         (0)     6012 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_config/test_wx_pay_config_by_id.py
--rw-rw-r--   0 root         (0) root         (0)     6053 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_config/test_xsolla_config.py
--rw-rw-r--   0 root         (0) root         (0)     6009 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_config/test_xsolla_config_by_id.py
--rw-rw-r--   0 root         (0) root         (0)     9053 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_config/update_adyen_config.py
--rw-rw-r--   0 root         (0) root         (0)     9087 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_config/update_ali_pay_config.py
--rw-rw-r--   0 root         (0) root         (0)     9121 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_config/update_checkout_config.py
--rw-rw-r--   0 root         (0) root         (0)     9073 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_config/update_pay_pal_config.py
--rw-rw-r--   0 root         (0) root         (0)     8877 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_config/update_payment_provider_config.py
--rw-rw-r--   0 root         (0) root         (0)     7373 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_config/update_payment_tax_config.py
--rw-rw-r--   0 root         (0) root         (0)     9073 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_config/update_stripe_config.py
--rw-rw-r--   0 root         (0) root         (0)     8308 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_config/update_wx_pay_config.py
--rw-rw-r--   0 root         (0) root         (0)     6909 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_config/update_wx_pay_config_cert.py
--rw-rw-r--   0 root         (0) root         (0)     8350 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_config/update_xsolla_config.py
--rw-rw-r--   0 root         (0) root         (0)     7279 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_config/update_xsolla_ui_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:40:41.252810 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_dedicated/
--rw-rw-r--   0 root         (0) root         (0)      669 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_dedicated/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    17317 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_dedicated/create_payment_order_by_79f85c.py
--rw-rw-r--   0 root         (0) root         (0)    14953 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_dedicated/refund_payment_order_by_309df5.py
--rw-rw-r--   0 root         (0) root         (0)     7420 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_dedicated/sync_payment_orders.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:40:41.252810 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_station/
--rw-rw-r--   0 root         (0) root         (0)     1595 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_station/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     9272 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_station/get_payment_customization.py
--rw-rw-r--   0 root         (0) root         (0)     9073 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_station/get_payment_public_config.py
--rw-rw-r--   0 root         (0) root         (0)     9767 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_station/get_payment_tax_value.py
--rw-rw-r--   0 root         (0) root         (0)    11264 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_station/pay.py
--rw-rw-r--   0 root         (0) root         (0)     7048 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_station/public_check_payment_or_dec069.py
--rw-rw-r--   0 root         (0) root         (0)     7013 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_station/public_get_payment_methods.py
--rw-rw-r--   0 root         (0) root         (0)     7844 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_station/public_get_payment_url.py
--rw-rw-r--   0 root         (0) root         (0)     6143 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_station/public_get_qr_code.py
--rw-rw-r--   0 root         (0) root         (0)     7438 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_station/public_get_unpaid_payme_26d8dd.py
--rw-rw-r--   0 root         (0) root         (0)    21889 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_station/public_normalize_paymen_6657a5.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:40:41.252810 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/revocation/
--rw-rw-r--   0 root         (0) root         (0)      904 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/revocation/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5484 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/revocation/delete_revocation_config.py
--rw-rw-r--   0 root         (0) root         (0)     7449 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/revocation/do_revocation.py
--rw-rw-r--   0 root         (0) root         (0)     5969 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/revocation/get_revocation_config.py
--rw-rw-r--   0 root         (0) root         (0)    13168 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/revocation/query_revocation_histories.py
--rw-rw-r--   0 root         (0) root         (0)     6829 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/revocation/update_revocation_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:40:41.252810 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/reward/
--rw-rw-r--   0 root         (0) root         (0)     1152 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/reward/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8055 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/reward/check_event_condition.py
--rw-rw-r--   0 root         (0) root         (0)     9060 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/reward/create_reward.py
--rw-rw-r--   0 root         (0) root         (0)     6774 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/reward/delete_reward.py
--rw-rw-r--   0 root         (0) root         (0)     7852 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/reward/delete_reward_condition_record.py
--rw-rw-r--   0 root         (0) root         (0)     5625 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/reward/export_rewards.py
--rw-rw-r--   0 root         (0) root         (0)     6729 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/reward/get_reward.py
--rw-rw-r--   0 root         (0) root         (0)     6726 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/reward/get_reward_1.py
--rw-rw-r--   0 root         (0) root         (0)     6974 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/reward/get_reward_by_code.py
--rw-rw-r--   0 root         (0) root         (0)     8939 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/reward/import_rewards.py
--rw-rw-r--   0 root         (0) root         (0)    10354 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/reward/query_rewards.py
--rw-rw-r--   0 root         (0) root         (0)    10368 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/reward/query_rewards_1.py
--rw-rw-r--   0 root         (0) root         (0)     9501 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/reward/update_reward.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:40:41.256810 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/section/
--rw-rw-r--   0 root         (0) root         (0)      795 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/section/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     9442 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/section/create_section.py
--rw-rw-r--   0 root         (0) root         (0)     7981 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/section/delete_section.py
--rw-rw-r--   0 root         (0) root         (0)     7999 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/section/get_section.py
--rw-rw-r--   0 root         (0) root         (0)    11868 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/section/public_list_active_sections.py
--rw-rw-r--   0 root         (0) root         (0)     6834 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/section/purge_expired_section.py
--rw-rw-r--   0 root         (0) root         (0)    11262 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/section/query_sections.py
--rw-rw-r--   0 root         (0) root         (0)    10409 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/section/update_section.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:40:41.256810 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/service_plugin_config/
--rw-rw-r--   0 root         (0) root         (0)     1560 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/service_plugin_config/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5496 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/service_plugin_config/delete_loot_box_plugin_config.py
--rw-rw-r--   0 root         (0) root         (0)     5529 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/service_plugin_config/delete_revocation_plugi_c2651d.py
--rw-rw-r--   0 root         (0) root         (0)     5496 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/service_plugin_config/delete_section_plugin_config.py
--rw-rw-r--   0 root         (0) root         (0)     5543 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/service_plugin_config/delete_service_plugin_config.py
--rw-rw-r--   0 root         (0) root         (0)     6467 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/service_plugin_config/get_loot_box_grpc_info.py
--rw-rw-r--   0 root         (0) root         (0)     5591 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/service_plugin_config/get_loot_box_plugin_config.py
--rw-rw-r--   0 root         (0) root         (0)     5642 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/service_plugin_config/get_revocation_plugin_config.py
--rw-rw-r--   0 root         (0) root         (0)     5591 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/service_plugin_config/get_section_plugin_config.py
--rw-rw-r--   0 root         (0) root         (0)     5638 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/service_plugin_config/get_service_plugin_config.py
--rw-rw-r--   0 root         (0) root         (0)     7269 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/service_plugin_config/update_loot_box_plugin_config.py
--rw-rw-r--   0 root         (0) root         (0)     7386 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/service_plugin_config/update_revocation_plugi_c19001.py
--rw-rw-r--   0 root         (0) root         (0)     7262 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/service_plugin_config/update_section_plugin_config.py
--rw-rw-r--   0 root         (0) root         (0)     7317 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/service_plugin_config/update_service_plugin_config.py
--rw-rw-r--   0 root         (0) root         (0)     7165 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/service_plugin_config/upload_revocation_plugi_6c586a.py
--rw-rw-r--   0 root         (0) root         (0)     7089 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/service_plugin_config/upload_section_plugin_c_780cdd.py
--rw-rw-r--   0 root         (0) root         (0)     7083 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/service_plugin_config/uplod_loot_box_plugin_c_5c5812.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:40:41.256810 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/session_platform/
--rw-rw-r--   0 root         (0) root         (0)      525 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/session_platform/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7814 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/session_platform/register_xbl_sessions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:40:41.256810 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/store/
--rw-rw-r--   0 root         (0) root         (0)     1495 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/store/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8215 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/store/clone_store.py
--rw-rw-r--   0 root         (0) root         (0)     7412 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/store/create_store.py
--rw-rw-r--   0 root         (0) root         (0)     6120 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/store/delete_published_store.py
--rw-rw-r--   0 root         (0) root         (0)     6988 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/store/delete_store.py
--rw-rw-r--   0 root         (0) root         (0)     5626 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/store/download_csv_templates.py
--rw-rw-r--   0 root         (0) root         (0)     6745 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/store/export_store.py
--rw-rw-r--   0 root         (0) root         (0)     7810 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/store/export_store_1.py
--rw-rw-r--   0 root         (0) root         (0)     8019 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/store/export_store_by_csv.py
--rw-rw-r--   0 root         (0) root         (0)     7219 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/store/get_catalog_definition.py
--rw-rw-r--   0 root         (0) root         (0)     6044 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/store/get_published_store.py
--rw-rw-r--   0 root         (0) root         (0)     6293 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/store/get_published_store_backup.py
--rw-rw-r--   0 root         (0) root         (0)     6666 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/store/get_store.py
--rw-rw-r--   0 root         (0) root         (0)     8926 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/store/import_store.py
--rw-rw-r--   0 root         (0) root         (0)     9058 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/store/import_store_1.py
--rw-rw-r--   0 root         (0) root         (0)    12067 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/store/import_store_by_csv.py
--rw-rw-r--   0 root         (0) root         (0)     5617 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/store/list_stores.py
--rw-rw-r--   0 root         (0) root         (0)     5699 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/store/public_list_stores.py
--rw-rw-r--   0 root         (0) root         (0)    11585 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/store/query_import_history.py
--rw-rw-r--   0 root         (0) root         (0)     6269 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/store/rollback_published_store.py
--rw-rw-r--   0 root         (0) root         (0)     8601 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/store/update_store.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:40:41.260810 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/subscription/
--rw-rw-r--   0 root         (0) root         (0)     2500 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/subscription/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    10657 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/subscription/cancel_subscription.py
--rw-rw-r--   0 root         (0) root         (0)     7635 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/subscription/check_user_subscription_6c59a6.py
--rw-rw-r--   0 root         (0) root         (0)     7461 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/subscription/delete_user_subscription.py
--rw-rw-r--   0 root         (0) root         (0)     7813 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/subscription/get_user_subscription.py
--rw-rw-r--   0 root         (0) root         (0)    10509 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/subscription/get_user_subscription_a_b2b8e9.py
--rw-rw-r--   0 root         (0) root         (0)    10413 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/subscription/get_user_subscription_b_a3096e.py
--rw-rw-r--   0 root         (0) root         (0)     9388 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/subscription/grant_days_to_subscription.py
--rw-rw-r--   0 root         (0) root         (0)     9261 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/subscription/platform_subscribe_subs_ad4f3b.py
--rw-rw-r--   0 root         (0) root         (0)     8974 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/subscription/process_user_subscripti_d07750.py
--rw-rw-r--   0 root         (0) root         (0)     9712 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/subscription/public_cancel_subscription.py
--rw-rw-r--   0 root         (0) root         (0)     9022 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/subscription/public_change_subscript_350ff2.py
--rw-rw-r--   0 root         (0) root         (0)     7709 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/subscription/public_check_user_subsc_16fdcb.py
--rw-rw-r--   0 root         (0) root         (0)    10483 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/subscription/public_get_user_subscri_c8d5b3.py
--rw-rw-r--   0 root         (0) root         (0)     7845 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/subscription/public_get_user_subscription.py
--rw-rw-r--   0 root         (0) root         (0)    13920 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/subscription/public_query_user_subsc_29ae74.py
--rw-rw-r--   0 root         (0) root         (0)    10640 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/subscription/public_subscribe_subscription.py
--rw-rw-r--   0 root         (0) root         (0)    13775 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/subscription/query_subscriptions.py
--rw-rw-r--   0 root         (0) root         (0)    13838 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/subscription/query_user_subscriptions.py
--rw-rw-r--   0 root         (0) root         (0)     7040 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/subscription/recurring_charge_subscription.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:40:41.260810 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/ticket/
--rw-rw-r--   0 root         (0) root         (0)      726 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/ticket/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     9606 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/ticket/acquire_user_ticket.py
--rw-rw-r--   0 root         (0) root         (0)     8398 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/ticket/decrease_ticket_sale.py
--rw-rw-r--   0 root         (0) root         (0)     6839 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/ticket/get_ticket_booth_id.py
--rw-rw-r--   0 root         (0) root         (0)     6899 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/ticket/get_ticket_dynamic.py
--rw-rw-r--   0 root         (0) root         (0)     8584 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/ticket/increase_ticket_sale.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:40:41.260810 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/trade_action/
--rw-rw-r--   0 root         (0) root         (0)      743 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/trade_action/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7151 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/trade_action/commit.py
--rw-rw-r--   0 root         (0) root         (0)    10222 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/trade_action/get_trade_history_by_criteria.py
--rw-rw-r--   0 root         (0) root         (0)     6707 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/trade_action/get_trade_history_by_tr_8b774c.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:40:41.260810 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/view/
--rw-rw-r--   0 root         (0) root         (0)      689 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/view/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8999 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/view/create_view.py
--rw-rw-r--   0 root         (0) root         (0)     7879 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/view/delete_view.py
--rw-rw-r--   0 root         (0) root         (0)     7855 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/view/get_view.py
--rw-rw-r--   0 root         (0) root         (0)     7399 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/view/list_views.py
--rw-rw-r--   0 root         (0) root         (0)     8337 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/view/public_list_views.py
--rw-rw-r--   0 root         (0) root         (0)     9906 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/view/update_view.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:40:41.264810 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/wallet/
--rw-rw-r--   0 root         (0) root         (0)     2161 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/wallet/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7218 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/wallet/bulk_credit.py
--rw-rw-r--   0 root         (0) root         (0)     7197 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/wallet/bulk_debit.py
--rw-rw-r--   0 root         (0) root         (0)     9106 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/wallet/check_balance.py
--rw-rw-r--   0 root         (0) root         (0)     9937 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/wallet/check_wallet.py
--rw-rw-r--   0 root         (0) root         (0)     9224 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/wallet/credit_user_wallet.py
--rw-rw-r--   0 root         (0) root         (0)     9738 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/wallet/debit_by_wallet_platform.py
--rw-rw-r--   0 root         (0) root         (0)     9616 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/wallet/debit_user_wallet.py
--rw-rw-r--   0 root         (0) root         (0)     9652 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/wallet/debit_user_wallet_by_cu_54daab.py
--rw-rw-r--   0 root         (0) root         (0)     7713 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/wallet/disable_user_wallet.py
--rw-rw-r--   0 root         (0) root         (0)     7702 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/wallet/enable_user_wallet.py
--rw-rw-r--   0 root         (0) root         (0)     7434 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/wallet/get_platform_wallet_config.py
--rw-rw-r--   0 root         (0) root         (0)     7583 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/wallet/get_user_wallet.py
--rw-rw-r--   0 root         (0) root         (0)     6747 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/wallet/get_wallet.py
--rw-rw-r--   0 root         (0) root         (0)     9708 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/wallet/list_user_currency_tran_bb67cf.py
--rw-rw-r--   0 root         (0) root         (0)     9692 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/wallet/list_user_wallet_transactions.py
--rw-rw-r--   0 root         (0) root         (0)     9329 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/wallet/pay_with_user_wallet.py
--rw-rw-r--   0 root         (0) root         (0)     6844 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/wallet/public_get_my_wallet.py
--rw-rw-r--   0 root         (0) root         (0)     7392 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/wallet/public_get_wallet.py
--rw-rw-r--   0 root         (0) root         (0)     9425 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/wallet/public_list_user_wallet_ed4de4.py
--rw-rw-r--   0 root         (0) root         (0)     6611 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/wallet/query_user_currency_wallets.py
--rw-rw-r--   0 root         (0) root         (0)    10777 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/wallet/query_wallets.py
--rw-rw-r--   0 root         (0) root         (0)     7483 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/wallet/reset_platform_wallet_config.py
--rw-rw-r--   0 root         (0) root         (0)     8703 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/wallet/update_platform_wallet_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:40:41.268810 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/wrappers/
--rw-rw-r--   0 root         (0) root         (0)    45433 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/wrappers/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    10487 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/wrappers/_achievement_platform.py
--rw-rw-r--   0 root         (0) root         (0)    26101 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/wrappers/_anonymization.py
--rw-rw-r--   0 root         (0) root         (0)    50598 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/wrappers/_campaign.py
--rw-rw-r--   0 root         (0) root         (0)    36673 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/wrappers/_catalog_changes.py
--rw-rw-r--   0 root         (0) root         (0)    44980 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/wrappers/_category.py
--rw-rw-r--   0 root         (0) root         (0)     8439 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/wrappers/_clawback.py
--rw-rw-r--   0 root         (0) root         (0)    22453 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/wrappers/_currency.py
--rw-rw-r--   0 root         (0) root         (0)    45845 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/wrappers/_dlc.py
--rw-rw-r--   0 root         (0) root         (0)   217710 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/wrappers/_entitlement.py
--rw-rw-r--   0 root         (0) root         (0)    28776 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/wrappers/_fulfillment.py
--rw-rw-r--   0 root         (0) root         (0)    12953 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/wrappers/_fulfillment_script.py
--rw-rw-r--   0 root         (0) root         (0)   136811 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/wrappers/_iap.py
--rw-rw-r--   0 root         (0) root         (0)     8814 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/wrappers/_invoice.py
--rw-rw-r--   0 root         (0) root         (0)   214448 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/wrappers/_item.py
--rw-rw-r--   0 root         (0) root         (0)    26602 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/wrappers/_key_group.py
--rw-rw-r--   0 root         (0) root         (0)    73916 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/wrappers/_order.py
--rw-rw-r--   0 root         (0) root         (0)     3784 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/wrappers/_order_dedicated.py
--rw-rw-r--   0 root         (0) root         (0)    37849 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/wrappers/_payment.py
--rw-rw-r--   0 root         (0) root         (0)     7464 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/wrappers/_payment_account.py
--rw-rw-r--   0 root         (0) root         (0)     7193 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/wrappers/_payment_callback_config.py
--rw-rw-r--   0 root         (0) root         (0)    99745 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/wrappers/_payment_config.py
--rw-rw-r--   0 root         (0) root         (0)    40570 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/wrappers/_payment_dedicated.py
--rw-rw-r--   0 root         (0) root         (0)    39913 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/wrappers/_payment_station.py
--rw-rw-r--   0 root         (0) root         (0)    15959 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/wrappers/_revocation.py
--rw-rw-r--   0 root         (0) root         (0)    42027 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/wrappers/_reward.py
--rw-rw-r--   0 root         (0) root         (0)    28694 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/wrappers/_section.py
--rw-rw-r--   0 root         (0) root         (0)    43145 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/wrappers/_service_plugin_config.py
--rw-rw-r--   0 root         (0) root         (0)     4085 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/wrappers/_session_platform.py
--rw-rw-r--   0 root         (0) root         (0)    64567 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/wrappers/_store.py
--rw-rw-r--   0 root         (0) root         (0)    80269 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/wrappers/_subscription.py
--rw-rw-r--   0 root         (0) root         (0)    18108 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/wrappers/_ticket.py
--rw-rw-r--   0 root         (0) root         (0)    10954 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/wrappers/_trade_action.py
--rw-rw-r--   0 root         (0) root         (0)    22228 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/wrappers/_view.py
--rw-rw-r--   0 root         (0) root         (0)    80449 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/wrappers/_wallet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:40:41.268810 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk_service_platform.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1129 2024-02-27 05:40:41.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk_service_platform.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    63851 2024-02-27 05:40:41.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk_service_platform.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-27 05:40:41.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk_service_platform.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       22 2024-02-27 05:40:41.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk_service_platform.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-02-27 05:40:41.000000 accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk_service_platform.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)      361 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-platform-0.8.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-27 05:40:41.268810 accelbyte-py-sdk-service-platform-0.8.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:13:44.665428 accelbyte-py-sdk-service-platform-0.9.0/
+-rw-r--r--   0 root         (0) root         (0)     1129 2024-03-13 06:13:44.665428 accelbyte-py-sdk-service-platform-0.9.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      875 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:13:44.577430 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:13:44.577430 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:13:44.581430 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/
+-rw-rw-r--   0 root         (0) root         (0)    44498 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:13:44.617429 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/
+-rw-rw-r--   0 root         (0) root         (0)    46990 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     6887 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/achievement_info.py
+-rw-rw-r--   0 root         (0) root         (0)     6536 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/action.py
+-rw-rw-r--   0 root         (0) root         (0)     4847 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/action_request.py
+-rw-rw-r--   0 root         (0) root         (0)     3817 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/additional_data.py
+-rw-rw-r--   0 root         (0) root         (0)     6091 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/additional_data_entitlement.py
+-rw-rw-r--   0 root         (0) root         (0)     6160 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/admin_entitlement_decrement.py
+-rw-rw-r--   0 root         (0) root         (0)     5427 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/admin_entitlement_sold_request.py
+-rw-rw-r--   0 root         (0) root         (0)    15789 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/admin_order_create.py
+-rw-rw-r--   0 root         (0) root         (0)    14844 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/adyen_config.py
+-rw-rw-r--   0 root         (0) root         (0)     5936 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/ali_pay_config.py
+-rw-rw-r--   0 root         (0) root         (0)     3609 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/app_config.py
+-rw-rw-r--   0 root         (0) root         (0)    15232 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/app_entitlement_info.py
+-rw-rw-r--   0 root         (0) root         (0)     5127 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/app_entitlement_paging_sliced_result.py
+-rw-rw-r--   0 root         (0) root         (0)    18681 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/app_info.py
+-rw-rw-r--   0 root         (0) root         (0)     4503 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/app_localization.py
+-rw-rw-r--   0 root         (0) root         (0)    15911 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/app_update.py
+-rw-rw-r--   0 root         (0) root         (0)     5222 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/apple_iap_config_info.py
+-rw-rw-r--   0 root         (0) root         (0)     4523 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/apple_iap_config_request.py
+-rw-rw-r--   0 root         (0) root         (0)     7917 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/apple_iap_receipt.py
+-rw-rw-r--   0 root         (0) root         (0)     5358 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/available_comparison.py
+-rw-rw-r--   0 root         (0) root         (0)     7793 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/available_predicate.py
+-rw-rw-r--   0 root         (0) root         (0)    10502 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/available_price.py
+-rw-rw-r--   0 root         (0) root         (0)     5173 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/base_custom_config.py
+-rw-rw-r--   0 root         (0) root         (0)     3952 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/base_tls_config.py
+-rw-rw-r--   0 root         (0) root         (0)     7398 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/basic_category_info.py
+-rw-rw-r--   0 root         (0) root         (0)    15822 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/basic_item.py
+-rw-rw-r--   0 root         (0) root         (0)     6661 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/billing_account.py
+-rw-rw-r--   0 root         (0) root         (0)    21684 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/billing_history_info.py
+-rw-rw-r--   0 root         (0) root         (0)     5051 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/billing_history_paging_sliced_result.py
+-rw-rw-r--   0 root         (0) root         (0)     7057 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/box_item.py
+-rw-rw-r--   0 root         (0) root         (0)     5756 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/bulk_credit_request.py
+-rw-rw-r--   0 root         (0) root         (0)     6234 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/bulk_credit_result.py
+-rw-rw-r--   0 root         (0) root         (0)     5680 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/bulk_debit_request.py
+-rw-rw-r--   0 root         (0) root         (0)     6209 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/bulk_debit_result.py
+-rw-rw-r--   0 root         (0) root         (0)     5398 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/bulk_entitlement_grant_request.py
+-rw-rw-r--   0 root         (0) root         (0)     6545 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/bulk_entitlement_grant_result.py
+-rw-rw-r--   0 root         (0) root         (0)     6646 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/bulk_entitlement_revoke_result.py
+-rw-rw-r--   0 root         (0) root         (0)     3809 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/bulk_operation_result.py
+-rw-rw-r--   0 root         (0) root         (0)     4256 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/bulk_region_data_change_request.py
+-rw-rw-r--   0 root         (0) root         (0)    45824 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/bundled_item_info.py
+-rw-rw-r--   0 root         (0) root         (0)    15037 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/campaign_create.py
+-rw-rw-r--   0 root         (0) root         (0)     6745 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/campaign_dynamic_info.py
+-rw-rw-r--   0 root         (0) root         (0)    17678 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/campaign_info.py
+-rw-rw-r--   0 root         (0) root         (0)     4921 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/campaign_paging_sliced_result.py
+-rw-rw-r--   0 root         (0) root         (0)    14206 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/campaign_update.py
+-rw-rw-r--   0 root         (0) root         (0)     4428 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/cancel_request.py
+-rw-rw-r--   0 root         (0) root         (0)    17109 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/catalog_change_info.py
+-rw-rw-r--   0 root         (0) root         (0)     5618 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/catalog_change_paging_result.py
+-rw-rw-r--   0 root         (0) root         (0)     4527 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/catalog_change_statistics.py
+-rw-rw-r--   0 root         (0) root         (0)     6626 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/catalog_definition_info.py
+-rw-rw-r--   0 root         (0) root         (0)     5016 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/category_create.py
+-rw-rw-r--   0 root         (0) root         (0)     8006 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/category_info.py
+-rw-rw-r--   0 root         (0) root         (0)     4285 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/category_update.py
+-rw-rw-r--   0 root         (0) root         (0)     4573 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/checkout_config.py
+-rw-rw-r--   0 root         (0) root         (0)    16858 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/clawback_info.py
+-rw-rw-r--   0 root         (0) root         (0)     6028 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/client_request_parameter.py
+-rw-rw-r--   0 root         (0) root         (0)     4918 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/client_transaction.py
+-rw-rw-r--   0 root         (0) root         (0)     3656 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/code_create.py
+-rw-rw-r--   0 root         (0) root         (0)     3759 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/code_create_result.py
+-rw-rw-r--   0 root         (0) root         (0)    19154 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/code_info.py
+-rw-rw-r--   0 root         (0) root         (0)     4894 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/code_info_paging_sliced_result.py
+-rw-rw-r--   0 root         (0) root         (0)     5164 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/condition_group.py
+-rw-rw-r--   0 root         (0) root         (0)     4805 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/condition_group_validate_result.py
+-rw-rw-r--   0 root         (0) root         (0)     5881 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/condition_match_result.py
+-rw-rw-r--   0 root         (0) root         (0)     5207 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/consumable_entitlement_revocation_config.py
+-rw-rw-r--   0 root         (0) root         (0)     6759 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/consume_item.py
+-rw-rw-r--   0 root         (0) root         (0)     6843 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/credit_payload.py
+-rw-rw-r--   0 root         (0) root         (0)     9077 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/credit_request.py
+-rw-rw-r--   0 root         (0) root         (0)     6245 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/credit_result.py
+-rw-rw-r--   0 root         (0) root         (0)    10457 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/credit_revocation.py
+-rw-rw-r--   0 root         (0) root         (0)     6404 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/credit_summary.py
+-rw-rw-r--   0 root         (0) root         (0)     3818 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/currency_config.py
+-rw-rw-r--   0 root         (0) root         (0)     7842 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/currency_create.py
+-rw-rw-r--   0 root         (0) root         (0)     9628 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/currency_info.py
+-rw-rw-r--   0 root         (0) root         (0)     7086 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/currency_summary.py
+-rw-rw-r--   0 root         (0) root         (0)     4326 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/currency_update.py
+-rw-rw-r--   0 root         (0) root         (0)     9690 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/currency_wallet.py
+-rw-rw-r--   0 root         (0) root         (0)     3729 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/customization.py
+-rw-rw-r--   0 root         (0) root         (0)     9465 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/debit_by_currency_code_request.py
+-rw-rw-r--   0 root         (0) root         (0)     8727 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/debit_by_wallet_platform_request.py
+-rw-rw-r--   0 root         (0) root         (0)     5973 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/debit_payload.py
+-rw-rw-r--   0 root         (0) root         (0)     6735 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/debit_request.py
+-rw-rw-r--   0 root         (0) root         (0)     6182 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/debit_result.py
+-rw-rw-r--   0 root         (0) root         (0)     4764 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/delete_reward_condition_request.py
+-rw-rw-r--   0 root         (0) root         (0)    11458 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/detailed_wallet_transaction_info.py
+-rw-rw-r--   0 root         (0) root         (0)     5325 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/detailed_wallet_transaction_paging_sliced_result.py
+-rw-rw-r--   0 root         (0) root         (0)     5234 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/dlc_config_reward_short_info.py
+-rw-rw-r--   0 root         (0) root         (0)     4557 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/dlc_item.py
+-rw-rw-r--   0 root         (0) root         (0)     3987 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/dlc_item_config_info.py
+-rw-rw-r--   0 root         (0) root         (0)     4009 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/dlc_item_config_update.py
+-rw-rw-r--   0 root         (0) root         (0)    15944 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/dlc_record.py
+-rw-rw-r--   0 root         (0) root         (0)     5171 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/durable_entitlement_revocation_config.py
+-rw-rw-r--   0 root         (0) root         (0)     5266 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/entitlement_config_info.py
+-rw-rw-r--   0 root         (0) root         (0)     5381 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/entitlement_decrement.py
+-rw-rw-r--   0 root         (0) root         (0)    28780 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/entitlement_decrement_result.py
+-rw-rw-r--   0 root         (0) root         (0)    13320 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/entitlement_grant.py
+-rw-rw-r--   0 root         (0) root         (0)     5749 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/entitlement_grant_result.py
+-rw-rw-r--   0 root         (0) root         (0)    14688 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/entitlement_history_info.py
+-rw-rw-r--   0 root         (0) root         (0)    21339 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/entitlement_ifc.py
+-rw-rw-r--   0 root         (0) root         (0)    25710 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/entitlement_info.py
+-rw-rw-r--   0 root         (0) root         (0)     5237 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/entitlement_loot_box_reward.py
+-rw-rw-r--   0 root         (0) root         (0)     5896 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/entitlement_origin_sync_result.py
+-rw-rw-r--   0 root         (0) root         (0)     4420 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/entitlement_ownership.py
+-rw-rw-r--   0 root         (0) root         (0)     5054 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/entitlement_paging_sliced_result.py
+-rw-rw-r--   0 root         (0) root         (0)     7832 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/entitlement_platform_config_info.py
+-rw-rw-r--   0 root         (0) root         (0)     5475 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/entitlement_platform_config_update.py
+-rw-rw-r--   0 root         (0) root         (0)     4103 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/entitlement_prechek_result.py
+-rw-rw-r--   0 root         (0) root         (0)    10478 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/entitlement_revocation.py
+-rw-rw-r--   0 root         (0) root         (0)     5647 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/entitlement_revocation_config.py
+-rw-rw-r--   0 root         (0) root         (0)     5372 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/entitlement_revoke_result.py
+-rw-rw-r--   0 root         (0) root         (0)     4632 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/entitlement_sold_request.py
+-rw-rw-r--   0 root         (0) root         (0)     6979 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/entitlement_sold_result.py
+-rw-rw-r--   0 root         (0) root         (0)     3897 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/entitlement_split_request.py
+-rw-rw-r--   0 root         (0) root         (0)     4969 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/entitlement_split_result.py
+-rw-rw-r--   0 root         (0) root         (0)    17167 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/entitlement_summary.py
+-rw-rw-r--   0 root         (0) root         (0)     4779 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/entitlement_transfer_request.py
+-rw-rw-r--   0 root         (0) root         (0)     5005 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/entitlement_transfer_result.py
+-rw-rw-r--   0 root         (0) root         (0)    10223 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/entitlement_update.py
+-rw-rw-r--   0 root         (0) root         (0)     4116 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/epic_games_dlc_sync_request.py
+-rw-rw-r--   0 root         (0) root         (0)     4578 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/epic_games_iap_config_info.py
+-rw-rw-r--   0 root         (0) root         (0)     3873 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/epic_games_iap_config_request.py
+-rw-rw-r--   0 root         (0) root         (0)     4137 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/epic_games_reconcile_request.py
+-rw-rw-r--   0 root         (0) root         (0)     7311 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/epic_games_reconcile_result.py
+-rw-rw-r--   0 root         (0) root         (0)     6322 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/error_entity.py
+-rw-rw-r--   0 root         (0) root         (0)     5594 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/estimated_price_info.py
+-rw-rw-r--   0 root         (0) root         (0)     5037 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/event_additional_data.py
+-rw-rw-r--   0 root         (0) root         (0)     3790 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/event_payload.py
+-rw-rw-r--   0 root         (0) root         (0)     3860 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/export_store_request.py
+-rw-rw-r--   0 root         (0) root         (0)     7161 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/export_store_to_csv_request.py
+-rw-rw-r--   0 root         (0) root         (0)    10770 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/extension_fulfillment_summary.py
+-rw-rw-r--   0 root         (0) root         (0)    21512 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/external_payment_order_create.py
+-rw-rw-r--   0 root         (0) root         (0)     7300 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/field_validation_error.py
+-rw-rw-r--   0 root         (0) root         (0)     6732 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/fixed_period_rotation_config.py
+-rw-rw-r--   0 root         (0) root         (0)     8584 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/ful_fill_item_payload.py
+-rw-rw-r--   0 root         (0) root         (0)     5307 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/fulfill_code_request.py
+-rw-rw-r--   0 root         (0) root         (0)     5148 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/fulfillment_error.py
+-rw-rw-r--   0 root         (0) root         (0)    17981 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/fulfillment_history_info.py
+-rw-rw-r--   0 root         (0) root         (0)     5152 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/fulfillment_history_paging_sliced_result.py
+-rw-rw-r--   0 root         (0) root         (0)     9156 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/fulfillment_item.py
+-rw-rw-r--   0 root         (0) root         (0)    19151 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/fulfillment_request.py
+-rw-rw-r--   0 root         (0) root         (0)     8957 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/fulfillment_result.py
+-rw-rw-r--   0 root         (0) root         (0)     3920 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/fulfillment_script_create.py
+-rw-rw-r--   0 root         (0) root         (0)     4485 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/fulfillment_script_info.py
+-rw-rw-r--   0 root         (0) root         (0)     3920 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/fulfillment_script_update.py
+-rw-rw-r--   0 root         (0) root         (0)    17250 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/full_app_info.py
+-rw-rw-r--   0 root         (0) root         (0)     8587 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/full_category_info.py
+-rw-rw-r--   0 root         (0) root         (0)    41260 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/full_item_info.py
+-rw-rw-r--   0 root         (0) root         (0)     5518 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/full_item_paging_result.py
+-rw-rw-r--   0 root         (0) root         (0)     4923 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/full_item_paging_sliced_result.py
+-rw-rw-r--   0 root         (0) root         (0)    17158 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/full_section_info.py
+-rw-rw-r--   0 root         (0) root         (0)     8097 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/full_view_info.py
+-rw-rw-r--   0 root         (0) root         (0)     6372 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/google_iap_config_info.py
+-rw-rw-r--   0 root         (0) root         (0)     4804 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/google_iap_config_request.py
+-rw-rw-r--   0 root         (0) root         (0)     8949 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/google_iap_receipt.py
+-rw-rw-r--   0 root         (0) root         (0)     4008 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/google_receipt_resolve_result.py
+-rw-rw-r--   0 root         (0) root         (0)     4583 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/grant_subscription_days_request.py
+-rw-rw-r--   0 root         (0) root         (0)     6765 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/grpc_server_info.py
+-rw-rw-r--   0 root         (0) root         (0)     9430 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/hierarchical_category_info.py
+-rw-rw-r--   0 root         (0) root         (0)     4958 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/iap_clawback_paging_sliced_result.py
+-rw-rw-r--   0 root         (0) root         (0)    13051 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/iap_consume_history_info.py
+-rw-rw-r--   0 root         (0) root         (0)     5135 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/iap_consume_history_paging_sliced_result.py
+-rw-rw-r--   0 root         (0) root         (0)     4023 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/iap_item_config_info.py
+-rw-rw-r--   0 root         (0) root         (0)     4045 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/iap_item_config_update.py
+-rw-rw-r--   0 root         (0) root         (0)     6407 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/iap_item_entry.py
+-rw-rw-r--   0 root         (0) root         (0)     7538 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/iap_item_flat_entry.py
+-rw-rw-r--   0 root         (0) root         (0)     4063 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/iap_item_mapping_info.py
+-rw-rw-r--   0 root         (0) root         (0)    19605 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/iap_order_info.py
+-rw-rw-r--   0 root         (0) root         (0)     4923 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/iap_order_paging_sliced_result.py
+-rw-rw-r--   0 root         (0) root         (0)     6800 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/image.py
+-rw-rw-r--   0 root         (0) root         (0)     7251 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/import_error_details.py
+-rw-rw-r--   0 root         (0) root         (0)     3772 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/import_store_app_info.py
+-rw-rw-r--   0 root         (0) root         (0)     5499 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/import_store_category_info.py
+-rw-rw-r--   0 root         (0) root         (0)     9930 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/import_store_error.py
+-rw-rw-r--   0 root         (0) root         (0)    10028 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/import_store_history_info.py
+-rw-rw-r--   0 root         (0) root         (0)     5734 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/import_store_history_paging_result.py
+-rw-rw-r--   0 root         (0) root         (0)     8596 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/import_store_item_info.py
+-rw-rw-r--   0 root         (0) root         (0)     5742 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/import_store_result.py
+-rw-rw-r--   0 root         (0) root         (0)     4528 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/import_store_section_info.py
+-rw-rw-r--   0 root         (0) root         (0)     4412 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/import_store_view_info.py
+-rw-rw-r--   0 root         (0) root         (0)     5328 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/in_game_item_sync.py
+-rw-rw-r--   0 root         (0) root         (0)     6069 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/inventory_config.py
+-rw-rw-r--   0 root         (0) root         (0)     6950 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/invoice_currency_summary.py
+-rw-rw-r--   0 root         (0) root         (0)     5289 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/invoice_summary.py
+-rw-rw-r--   0 root         (0) root         (0)     4318 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/item_acquire_request.py
+-rw-rw-r--   0 root         (0) root         (0)     4378 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/item_acquire_result.py
+-rw-rw-r--   0 root         (0) root         (0)    35642 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/item_create.py
+-rw-rw-r--   0 root         (0) root         (0)     6942 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/item_dynamic_data_info.py
+-rw-rw-r--   0 root         (0) root         (0)     5207 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/item_id.py
+-rw-rw-r--   0 root         (0) root         (0)    44612 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/item_info.py
+-rw-rw-r--   0 root         (0) root         (0)     9707 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/item_naming.py
+-rw-rw-r--   0 root         (0) root         (0)     4845 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/item_paging_sliced_result.py
+-rw-rw-r--   0 root         (0) root         (0)     4077 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/item_purchase_condition_validate_request.py
+-rw-rw-r--   0 root         (0) root         (0)     6775 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/item_purchase_condition_validate_result.py
+-rw-rw-r--   0 root         (0) root         (0)     3726 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/item_return_request.py
+-rw-rw-r--   0 root         (0) root         (0)    16290 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/item_revocation.py
+-rw-rw-r--   0 root         (0) root         (0)    35348 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/item_snapshot.py
+-rw-rw-r--   0 root         (0) root         (0)     7898 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/item_type_config_create.py
+-rw-rw-r--   0 root         (0) root         (0)     9730 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/item_type_config_info.py
+-rw-rw-r--   0 root         (0) root         (0)     6323 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/item_type_config_update.py
+-rw-rw-r--   0 root         (0) root         (0)    35924 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/item_update.py
+-rw-rw-r--   0 root         (0) root         (0)     6142 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/key_group_create.py
+-rw-rw-r--   0 root         (0) root         (0)     5309 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/key_group_dynamic_info.py
+-rw-rw-r--   0 root         (0) root         (0)     9251 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/key_group_info.py
+-rw-rw-r--   0 root         (0) root         (0)     4923 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/key_group_paging_sliced_result.py
+-rw-rw-r--   0 root         (0) root         (0)     6142 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/key_group_update.py
+-rw-rw-r--   0 root         (0) root         (0)    10089 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/key_info.py
+-rw-rw-r--   0 root         (0) root         (0)     4814 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/key_paging_slice_result.py
+-rw-rw-r--   0 root         (0) root         (0)     6973 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/list_view_info.py
+-rw-rw-r--   0 root         (0) root         (0)     6062 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/localization.py
+-rw-rw-r--   0 root         (0) root         (0)     6048 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/loot_box_config.py
+-rw-rw-r--   0 root         (0) root         (0)     7159 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/loot_box_plugin_config_info.py
+-rw-rw-r--   0 root         (0) root         (0)     6382 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/loot_box_plugin_config_update.py
+-rw-rw-r--   0 root         (0) root         (0)     7113 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/loot_box_reward.py
+-rw-rw-r--   0 root         (0) root         (0)     8739 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/mock_iap_receipt.py
+-rw-rw-r--   0 root         (0) root         (0)     6618 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/notification_process_result.py
+-rw-rw-r--   0 root         (0) root         (0)     5206 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/oculus_iap_config_info.py
+-rw-rw-r--   0 root         (0) root         (0)     4509 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/oculus_iap_config_request.py
+-rw-rw-r--   0 root         (0) root         (0)     8247 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/oculus_reconcile_result.py
+-rw-rw-r--   0 root         (0) root         (0)    11530 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/operation.py
+-rw-rw-r--   0 root         (0) root         (0)     9263 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/operation_request.py
+-rw-rw-r--   0 root         (0) root         (0)     4048 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/option_box_config.py
+-rw-rw-r--   0 root         (0) root         (0)    40806 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/order.py
+-rw-rw-r--   0 root         (0) root         (0)     7905 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/order_bundle_item_info.py
+-rw-rw-r--   0 root         (0) root         (0)    10211 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/order_create.py
+-rw-rw-r--   0 root         (0) root         (0)     4139 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/order_creation_options.py
+-rw-rw-r--   0 root         (0) root         (0)     5190 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/order_grant_info.py
+-rw-rw-r--   0 root         (0) root         (0)     9333 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/order_history_info.py
+-rw-rw-r--   0 root         (0) root         (0)    35283 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/order_info.py
+-rw-rw-r--   0 root         (0) root         (0)     5439 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/order_paging_result.py
+-rw-rw-r--   0 root         (0) root         (0)     4864 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/order_paging_sliced_result.py
+-rw-rw-r--   0 root         (0) root         (0)     3794 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/order_refund_create.py
+-rw-rw-r--   0 root         (0) root         (0)     4537 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/order_statistics.py
+-rw-rw-r--   0 root         (0) root         (0)     5318 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/order_summary.py
+-rw-rw-r--   0 root         (0) root         (0)     4891 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/order_sync_result.py
+-rw-rw-r--   0 root         (0) root         (0)     5342 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/order_update.py
+-rw-rw-r--   0 root         (0) root         (0)     3568 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/ownership.py
+-rw-rw-r--   0 root         (0) root         (0)     3880 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/ownership_token.py
+-rw-rw-r--   0 root         (0) root         (0)     4266 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/paging.py
+-rw-rw-r--   0 root         (0) root         (0)     6054 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/pay_pal_config.py
+-rw-rw-r--   0 root         (0) root         (0)     5071 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/payment_account.py
+-rw-rw-r--   0 root         (0) root         (0)     6102 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/payment_callback_config_info.py
+-rw-rw-r--   0 root         (0) root         (0)     5450 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/payment_callback_config_update.py
+-rw-rw-r--   0 root         (0) root         (0)    20025 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/payment_merchant_config_info.py
+-rw-rw-r--   0 root         (0) root         (0)     5193 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/payment_method.py
+-rw-rw-r--   0 root         (0) root         (0)    12501 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/payment_notification_info.py
+-rw-rw-r--   0 root         (0) root         (0)     5209 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/payment_notification_paging_sliced_result.py
+-rw-rw-r--   0 root         (0) root         (0)    45571 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/payment_order.py
+-rw-rw-r--   0 root         (0) root         (0)     6366 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/payment_order_charge_request.py
+-rw-rw-r--   0 root         (0) root         (0)     5806 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/payment_order_charge_status.py
+-rw-rw-r--   0 root         (0) root         (0)    19652 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/payment_order_create.py
+-rw-rw-r--   0 root         (0) root         (0)     9857 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/payment_order_create_result.py
+-rw-rw-r--   0 root         (0) root         (0)     9373 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/payment_order_details.py
+-rw-rw-r--   0 root         (0) root         (0)    42526 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/payment_order_info.py
+-rw-rw-r--   0 root         (0) root         (0)     8607 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/payment_order_notify_simulation.py
+-rw-rw-r--   0 root         (0) root         (0)     5013 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/payment_order_paging_sliced_result.py
+-rw-rw-r--   0 root         (0) root         (0)     4458 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/payment_order_paid_result.py
+-rw-rw-r--   0 root         (0) root         (0)     3805 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/payment_order_refund.py
+-rw-rw-r--   0 root         (0) root         (0)     9739 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/payment_order_refund_result.py
+-rw-rw-r--   0 root         (0) root         (0)     5217 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/payment_order_sync_result.py
+-rw-rw-r--   0 root         (0) root         (0)     5902 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/payment_process_result.py
+-rw-rw-r--   0 root         (0) root         (0)    11019 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/payment_provider_config_edit.py
+-rw-rw-r--   0 root         (0) root         (0)    12711 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/payment_provider_config_info.py
+-rw-rw-r--   0 root         (0) root         (0)     5249 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/payment_provider_config_paging_sliced_result.py
+-rw-rw-r--   0 root         (0) root         (0)     6175 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/payment_request.py
+-rw-rw-r--   0 root         (0) root         (0)     7352 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/payment_tax_config_edit.py
+-rw-rw-r--   0 root         (0) root         (0)     7331 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/payment_tax_config_info.py
+-rw-rw-r--   0 root         (0) root         (0)     3642 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/payment_token.py
+-rw-rw-r--   0 root         (0) root         (0)     8585 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/payment_url.py
+-rw-rw-r--   0 root         (0) root         (0)     7491 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/payment_url_create.py
+-rw-rw-r--   0 root         (0) root         (0)     4112 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/platform_dlc_config_info.py
+-rw-rw-r--   0 root         (0) root         (0)     4134 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/platform_dlc_config_update.py
+-rw-rw-r--   0 root         (0) root         (0)     5358 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/platform_dlc_entry.py
+-rw-rw-r--   0 root         (0) root         (0)     6674 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/platform_reward.py
+-rw-rw-r--   0 root         (0) root         (0)     4579 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/platform_reward_currency.py
+-rw-rw-r--   0 root         (0) root         (0)     5219 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/platform_reward_item.py
+-rw-rw-r--   0 root         (0) root         (0)     7240 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/platform_subscribe_request.py
+-rw-rw-r--   0 root         (0) root         (0)    10282 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/platform_wallet.py
+-rw-rw-r--   0 root         (0) root         (0)     7732 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/platform_wallet_config_info.py
+-rw-rw-r--   0 root         (0) root         (0)     5375 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/platform_wallet_config_update.py
+-rw-rw-r--   0 root         (0) root         (0)     4297 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/play_station_dlc_sync_multi_service_labels_request.py
+-rw-rw-r--   0 root         (0) root         (0)     4005 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/play_station_dlc_sync_request.py
+-rw-rw-r--   0 root         (0) root         (0)     9707 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/play_station_iap_config_info.py
+-rw-rw-r--   0 root         (0) root         (0)     6644 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/play_station_multi_service_labels_reconcile_request.py
+-rw-rw-r--   0 root         (0) root         (0)     6270 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/play_station_reconcile_request.py
+-rw-rw-r--   0 root         (0) root         (0)     7202 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/play_station_reconcile_result.py
+-rw-rw-r--   0 root         (0) root         (0)     9033 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/playstation_iap_config_request.py
+-rw-rw-r--   0 root         (0) root         (0)    46169 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/populated_item_info.py
+-rw-rw-r--   0 root         (0) root         (0)     5298 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/pre_check_fulfillment_request.py
+-rw-rw-r--   0 root         (0) root         (0)     8520 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/predicate.py
+-rw-rw-r--   0 root         (0) root         (0)     6295 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/predicate_validate_result.py
+-rw-rw-r--   0 root         (0) root         (0)     6257 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/public_custom_config_info.py
+-rw-rw-r--   0 root         (0) root         (0)    14200 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/public_entitlement_history_info.py
+-rw-rw-r--   0 root         (0) root         (0)     4278 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/purchase_condition.py
+-rw-rw-r--   0 root         (0) root         (0)     4436 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/purchase_condition_update.py
+-rw-rw-r--   0 root         (0) root         (0)     3735 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/purchased_item_count.py
+-rw-rw-r--   0 root         (0) root         (0)     6288 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/recurring.py
+-rw-rw-r--   0 root         (0) root         (0)     5150 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/recurring_charge_result.py
+-rw-rw-r--   0 root         (0) root         (0)     9041 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/redeem_history_info.py
+-rw-rw-r--   0 root         (0) root         (0)     5032 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/redeem_history_paging_sliced_result.py
+-rw-rw-r--   0 root         (0) root         (0)     4294 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/redeem_request.py
+-rw-rw-r--   0 root         (0) root         (0)     3972 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/redeem_result.py
+-rw-rw-r--   0 root         (0) root         (0)     6083 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/redeemable_item.py
+-rw-rw-r--   0 root         (0) root         (0)     6577 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/region_data_change.py
+-rw-rw-r--   0 root         (0) root         (0)    13121 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/region_data_item.py
+-rw-rw-r--   0 root         (0) root         (0)    12343 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/region_data_item_dto.py
+-rw-rw-r--   0 root         (0) root         (0)     7432 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/request_history.py
+-rw-rw-r--   0 root         (0) root         (0)     9434 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/requirement.py
+-rw-rw-r--   0 root         (0) root         (0)     6050 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/revocation_config_info.py
+-rw-rw-r--   0 root         (0) root         (0)     5345 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/revocation_config_update.py
+-rw-rw-r--   0 root         (0) root         (0)     5135 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/revocation_error.py
+-rw-rw-r--   0 root         (0) root         (0)    16187 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/revocation_history_info.py
+-rw-rw-r--   0 root         (0) root         (0)     5133 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/revocation_history_paging_sliced_result.py
+-rw-rw-r--   0 root         (0) root         (0)     7200 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/revocation_plugin_config_info.py
+-rw-rw-r--   0 root         (0) root         (0)     6434 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/revocation_plugin_config_update.py
+-rw-rw-r--   0 root         (0) root         (0)     6858 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/revocation_request.py
+-rw-rw-r--   0 root         (0) root         (0)     8495 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/revocation_result.py
+-rw-rw-r--   0 root         (0) root         (0)     6340 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/revoke_currency.py
+-rw-rw-r--   0 root         (0) root         (0)     3920 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/revoke_entitlement.py
+-rw-rw-r--   0 root         (0) root         (0)     4593 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/revoke_entitlement_payload.py
+-rw-rw-r--   0 root         (0) root         (0)     7581 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/revoke_entry.py
+-rw-rw-r--   0 root         (0) root         (0)     8281 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/revoke_item.py
+-rw-rw-r--   0 root         (0) root         (0)     6455 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/revoke_item_summary.py
+-rw-rw-r--   0 root         (0) root         (0)     6305 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/revoke_result.py
+-rw-rw-r--   0 root         (0) root         (0)     4535 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/revoke_use_count_request.py
+-rw-rw-r--   0 root         (0) root         (0)     6429 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/reward_condition.py
+-rw-rw-r--   0 root         (0) root         (0)     9914 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/reward_create.py
+-rw-rw-r--   0 root         (0) root         (0)    12718 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/reward_info.py
+-rw-rw-r--   0 root         (0) root         (0)     7585 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/reward_item.py
+-rw-rw-r--   0 root         (0) root         (0)     8787 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/reward_migration_result.py
+-rw-rw-r--   0 root         (0) root         (0)     4883 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/reward_paging_sliced_result.py
+-rw-rw-r--   0 root         (0) root         (0)     9914 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/reward_update.py
+-rw-rw-r--   0 root         (0) root         (0)    11795 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/rewards_request.py
+-rw-rw-r--   0 root         (0) root         (0)     4293 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/sale_config.py
+-rw-rw-r--   0 root         (0) root         (0)    12693 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/section_create.py
+-rw-rw-r--   0 root         (0) root         (0)    15735 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/section_info.py
+-rw-rw-r--   0 root         (0) root         (0)     4116 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/section_item.py
+-rw-rw-r--   0 root         (0) root         (0)     4931 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/section_paging_sliced_result.py
+-rw-rw-r--   0 root         (0) root         (0)     7158 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/section_plugin_config_info.py
+-rw-rw-r--   0 root         (0) root         (0)     6381 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/section_plugin_config_update.py
+-rw-rw-r--   0 root         (0) root         (0)    12693 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/section_update.py
+-rw-rw-r--   0 root         (0) root         (0)     4851 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/service_plugin_config_info.py
+-rw-rw-r--   0 root         (0) root         (0)     4124 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/service_plugin_config_update.py
+-rw-rw-r--   0 root         (0) root         (0)     7732 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/slide.py
+-rw-rw-r--   0 root         (0) root         (0)    26967 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/stackable_entitlement_info.py
+-rw-rw-r--   0 root         (0) root         (0)     4302 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/steam_achievement.py
+-rw-rw-r--   0 root         (0) root         (0)     5217 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/steam_achievement_update_request.py
+-rw-rw-r--   0 root         (0) root         (0)     4412 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/steam_dlc_sync_request.py
+-rw-rw-r--   0 root         (0) root         (0)     7715 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/steam_iap_config.py
+-rw-rw-r--   0 root         (0) root         (0)     5584 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/steam_iap_config_info.py
+-rw-rw-r--   0 root         (0) root         (0)     4963 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/steam_iap_config_request.py
+-rw-rw-r--   0 root         (0) root         (0)     8134 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/steam_sync_request.py
+-rw-rw-r--   0 root         (0) root         (0)     6900 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/store_backup_info.py
+-rw-rw-r--   0 root         (0) root         (0)     8017 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/store_create.py
+-rw-rw-r--   0 root         (0) root         (0)    11835 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/store_info.py
+-rw-rw-r--   0 root         (0) root         (0)     8017 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/store_update.py
+-rw-rw-r--   0 root         (0) root         (0)     8277 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/stream_event.py
+-rw-rw-r--   0 root         (0) root         (0)     9229 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/stream_event_body.py
+-rw-rw-r--   0 root         (0) root         (0)     6700 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/stripe_config.py
+-rw-rw-r--   0 root         (0) root         (0)     7872 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/sub_item_available_price.py
+-rw-rw-r--   0 root         (0) root         (0)     3741 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/subscribable.py
+-rw-rw-r--   0 root         (0) root         (0)     7459 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/subscribe_request.py
+-rw-rw-r--   0 root         (0) root         (0)    15341 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/subscription_activity_info.py
+-rw-rw-r--   0 root         (0) root         (0)     5228 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/subscription_activity_paging_sliced_result.py
+-rw-rw-r--   0 root         (0) root         (0)    37996 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/subscription_info.py
+-rw-rw-r--   0 root         (0) root         (0)     5011 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/subscription_paging_sliced_result.py
+-rw-rw-r--   0 root         (0) root         (0)    10201 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/subscription_summary.py
+-rw-rw-r--   0 root         (0) root         (0)     5767 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/tax_result.py
+-rw-rw-r--   0 root         (0) root         (0)     4205 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/test_result.py
+-rw-rw-r--   0 root         (0) root         (0)     4359 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/ticket_acquire_request.py
+-rw-rw-r--   0 root         (0) root         (0)     3837 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/ticket_acquire_result.py
+-rw-rw-r--   0 root         (0) root         (0)     4505 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/ticket_booth_id.py
+-rw-rw-r--   0 root         (0) root         (0)     3956 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/ticket_dynamic_info.py
+-rw-rw-r--   0 root         (0) root         (0)     3843 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/ticket_sale_decrement_request.py
+-rw-rw-r--   0 root         (0) root         (0)     4432 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/ticket_sale_increment_request.py
+-rw-rw-r--   0 root         (0) root         (0)     4598 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/ticket_sale_increment_result.py
+-rw-rw-r--   0 root         (0) root         (0)     5351 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/time_limited_balance.py
+-rw-rw-r--   0 root         (0) root         (0)     4338 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/timed_ownership.py
+-rw-rw-r--   0 root         (0) root         (0)     4919 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/tls_config.py
+-rw-rw-r--   0 root         (0) root         (0)     5143 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/trade_action_paging_sliced_result.py
+-rw-rw-r--   0 root         (0) root         (0)     9868 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/trade_chain_action_history_info.py
+-rw-rw-r--   0 root         (0) root         (0)     7466 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/trade_chained_action_commit_request.py
+-rw-rw-r--   0 root         (0) root         (0)    35344 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/trade_notification.py
+-rw-rw-r--   0 root         (0) root         (0)    19184 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/transaction.py
+-rw-rw-r--   0 root         (0) root         (0)     5990 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/transaction_amount_details.py
+-rw-rw-r--   0 root         (0) root         (0)     6178 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/twitch_iap_config_info.py
+-rw-rw-r--   0 root         (0) root         (0)     5562 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/twitch_iap_config_request.py
+-rw-rw-r--   0 root         (0) root         (0)     5400 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/twitch_sync_request.py
+-rw-rw-r--   0 root         (0) root         (0)     5963 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/twitch_sync_result.py
+-rw-rw-r--   0 root         (0) root         (0)     9058 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/user_dlc.py
+-rw-rw-r--   0 root         (0) root         (0)    18486 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/user_dlc_record.py
+-rw-rw-r--   0 root         (0) root         (0)     5282 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/user_entitlement_history_paging_sliced_result.py
+-rw-rw-r--   0 root         (0) root         (0)     5628 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/validation_error_entity.py
+-rw-rw-r--   0 root         (0) root         (0)     5463 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/view_create.py
+-rw-rw-r--   0 root         (0) root         (0)     9919 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/view_info.py
+-rw-rw-r--   0 root         (0) root         (0)     5583 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/view_update.py
+-rw-rw-r--   0 root         (0) root         (0)    13479 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/wallet_info.py
+-rw-rw-r--   0 root         (0) root         (0)     4883 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/wallet_paging_sliced_result.py
+-rw-rw-r--   0 root         (0) root         (0)     5065 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/wallet_revocation_config.py
+-rw-rw-r--   0 root         (0) root         (0)    13000 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/wallet_transaction_info.py
+-rw-rw-r--   0 root         (0) root         (0)     5133 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/wallet_transaction_paging_sliced_result.py
+-rw-rw-r--   0 root         (0) root         (0)     6438 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/wx_pay_config_info.py
+-rw-rw-r--   0 root         (0) root         (0)     5784 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/wx_pay_config_request.py
+-rw-rw-r--   0 root         (0) root         (0)     6781 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/xbl_achievement_update_request.py
+-rw-rw-r--   0 root         (0) root         (0)     3824 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/xbl_dlc_sync_request.py
+-rw-rw-r--   0 root         (0) root         (0)     7960 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/xbl_iap_config_info.py
+-rw-rw-r--   0 root         (0) root         (0)     3941 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/xbl_iap_config_request.py
+-rw-rw-r--   0 root         (0) root         (0)     6079 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/xbl_reconcile_request.py
+-rw-rw-r--   0 root         (0) root         (0)     7420 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/xbl_reconcile_result.py
+-rw-rw-r--   0 root         (0) root         (0)     4259 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/xbl_user_achievements.py
+-rw-rw-r--   0 root         (0) root         (0)     6172 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/xbl_user_session_request.py
+-rw-rw-r--   0 root         (0) root         (0)     4513 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/xbox_achievement.py
+-rw-rw-r--   0 root         (0) root         (0)     7028 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/xsolla_config.py
+-rw-rw-r--   0 root         (0) root         (0)     6638 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/xsolla_paywall_config.py
+-rw-rw-r--   0 root         (0) root         (0)     6974 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/xsolla_paywall_config_request.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:13:44.617429 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/
+-rw-rw-r--   0 root         (0) root         (0)      437 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:13:44.617429 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/achievement_platform/
+-rw-rw-r--   0 root         (0) root         (0)      668 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/achievement_platform/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7746 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/achievement_platform/get_xbl_user_achievements.py
+-rw-rw-r--   0 root         (0) root         (0)     8252 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/achievement_platform/unlock_steam_user_achievement.py
+-rw-rw-r--   0 root         (0) root         (0)     7840 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/achievement_platform/update_xbl_user_achievement.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:13:44.617429 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/anonymization/
+-rw-rw-r--   0 root         (0) root         (0)      938 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/anonymization/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     6449 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/anonymization/anonymize_campaign.py
+-rw-rw-r--   0 root         (0) root         (0)     6483 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/anonymization/anonymize_entitlement.py
+-rw-rw-r--   0 root         (0) root         (0)     6468 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/anonymization/anonymize_fulfillment.py
+-rw-rw-r--   0 root         (0) root         (0)     6466 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/anonymization/anonymize_integration.py
+-rw-rw-r--   0 root         (0) root         (0)     6427 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/anonymization/anonymize_order.py
+-rw-rw-r--   0 root         (0) root         (0)     6461 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/anonymization/anonymize_payment.py
+-rw-rw-r--   0 root         (0) root         (0)     6333 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/anonymization/anonymize_revocation.py
+-rw-rw-r--   0 root         (0) root         (0)     6511 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/anonymization/anonymize_subscription.py
+-rw-rw-r--   0 root         (0) root         (0)     6443 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/anonymization/anonymize_wallet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:13:44.621429 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/campaign/
+-rw-rw-r--   0 root         (0) root         (0)     1106 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/campaign/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     9255 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/campaign/apply_user_redemption.py
+-rw-rw-r--   0 root         (0) root         (0)     7681 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/campaign/bulk_disable_codes.py
+-rw-rw-r--   0 root         (0) root         (0)     7568 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/campaign/bulk_enable_codes.py
+-rw-rw-r--   0 root         (0) root         (0)     7460 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/campaign/create_campaign.py
+-rw-rw-r--   0 root         (0) root         (0)     8379 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/campaign/create_codes.py
+-rw-rw-r--   0 root         (0) root         (0)     6850 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/campaign/disable_code.py
+-rw-rw-r--   0 root         (0) root         (0)     7339 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/campaign/download.py
+-rw-rw-r--   0 root         (0) root         (0)     6614 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/campaign/enable_code.py
+-rw-rw-r--   0 root         (0) root         (0)     6793 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/campaign/get_campaign.py
+-rw-rw-r--   0 root         (0) root         (0)     6928 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/campaign/get_campaign_dynamic.py
+-rw-rw-r--   0 root         (0) root         (0)     8331 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/campaign/get_code.py
+-rw-rw-r--   0 root         (0) root         (0)     8845 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/campaign/query_campaigns.py
+-rw-rw-r--   0 root         (0) root         (0)    10629 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/campaign/query_codes.py
+-rw-rw-r--   0 root         (0) root         (0)     9870 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/campaign/query_redeem_history.py
+-rw-rw-r--   0 root         (0) root         (0)     8643 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/campaign/update_campaign.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:13:44.621429 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/catalog_changes/
+-rw-rw-r--   0 root         (0) root         (0)     1503 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/catalog_changes/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    13345 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/catalog_changes/get_statistic.py
+-rw-rw-r--   0 root         (0) root         (0)     7048 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/catalog_changes/publish_all.py
+-rw-rw-r--   0 root         (0) root         (0)     7501 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/catalog_changes/publish_selected.py
+-rw-rw-r--   0 root         (0) root         (0)    19166 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/catalog_changes/query_changes.py
+-rw-rw-r--   0 root         (0) root         (0)     6685 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/catalog_changes/select_all_records.py
+-rw-rw-r--   0 root         (0) root         (0)    14608 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/catalog_changes/select_all_records_by_criteria.py
+-rw-rw-r--   0 root         (0) root         (0)     7640 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/catalog_changes/select_record.py
+-rw-rw-r--   0 root         (0) root         (0)     6704 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/catalog_changes/unselect_all_records.py
+-rw-rw-r--   0 root         (0) root         (0)     8651 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/catalog_changes/unselect_record.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:13:44.621429 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/category/
+-rw-rw-r--   0 root         (0) root         (0)     1169 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/category/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     9467 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/category/create_category.py
+-rw-rw-r--   0 root         (0) root         (0)     8263 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/category/delete_category.py
+-rw-rw-r--   0 root         (0) root         (0)     8043 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/category/download_categories.py
+-rw-rw-r--   0 root         (0) root         (0)     7885 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/category/get_category.py
+-rw-rw-r--   0 root         (0) root         (0)     7681 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/category/get_child_categories.py
+-rw-rw-r--   0 root         (0) root         (0)     7737 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/category/get_descendant_categories.py
+-rw-rw-r--   0 root         (0) root         (0)     6673 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/category/get_root_categories.py
+-rw-rw-r--   0 root         (0) root         (0)     6765 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/category/list_categories_basic.py
+-rw-rw-r--   0 root         (0) root         (0)     8791 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/category/public_get_category.py
+-rw-rw-r--   0 root         (0) root         (0)     8580 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/category/public_get_child_categories.py
+-rw-rw-r--   0 root         (0) root         (0)     8641 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/category/public_get_descendant_c_c5054d.py
+-rw-rw-r--   0 root         (0) root         (0)     7590 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/category/public_get_root_categories.py
+-rw-rw-r--   0 root         (0) root         (0)    10039 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/category/update_category.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:13:44.621429 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/clawback/
+-rw-rw-r--   0 root         (0) root         (0)      761 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/clawback/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     6726 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/clawback/mock_play_station_stream_event.py
+-rw-rw-r--   0 root         (0) root         (0)    13505 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/clawback/query_iap_clawback_history.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:13:44.621429 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/currency/
+-rw-rw-r--   0 root         (0) root         (0)      998 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/currency/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7640 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/currency/create_currency.py
+-rw-rw-r--   0 root         (0) root         (0)     6901 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/currency/delete_currency.py
+-rw-rw-r--   0 root         (0) root         (0)     7029 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/currency/get_currency_config.py
+-rw-rw-r--   0 root         (0) root         (0)     7015 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/currency/get_currency_summary.py
+-rw-rw-r--   0 root         (0) root         (0)     7232 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/currency/list_currencies.py
+-rw-rw-r--   0 root         (0) root         (0)     7072 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/currency/public_list_currencies.py
+-rw-rw-r--   0 root         (0) root         (0)     8591 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/currency/update_currency.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:13:44.625429 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/dlc/
+-rw-rw-r--   0 root         (0) root         (0)     1589 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/dlc/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     5583 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/dlc/delete_dlc_item_config.py
+-rw-rw-r--   0 root         (0) root         (0)     5625 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/dlc/delete_platform_dlc_config.py
+-rw-rw-r--   0 root         (0) root         (0)     7638 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/dlc/ge_dlc_durable_reward_s_f83f8a.py
+-rw-rw-r--   0 root         (0) root         (0)     5950 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/dlc/get_dlc_item_config.py
+-rw-rw-r--   0 root         (0) root         (0)     6034 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/dlc/get_platform_dlc_config.py
+-rw-rw-r--   0 root         (0) root         (0)     7755 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/dlc/get_user_dlc.py
+-rw-rw-r--   0 root         (0) root         (0)     7685 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/dlc/get_user_dlc_by_platform.py
+-rw-rw-r--   0 root         (0) root         (0)     8603 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/dlc/public_sync_psn_dlc_inv_429118.py
+-rw-rw-r--   0 root         (0) root         (0)     8106 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/dlc/public_sync_psn_dlc_inventory.py
+-rw-rw-r--   0 root         (0) root         (0)     7883 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/dlc/sync_epic_game_dlc.py
+-rw-rw-r--   0 root         (0) root         (0)     6535 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/dlc/sync_oculus_dlc.py
+-rw-rw-r--   0 root         (0) root         (0)     7703 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/dlc/sync_steam_dlc.py
+-rw-rw-r--   0 root         (0) root         (0)     7766 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/dlc/sync_xbox_dlc.py
+-rw-rw-r--   0 root         (0) root         (0)     7905 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/dlc/update_dlc_item_config.py
+-rw-rw-r--   0 root         (0) root         (0)     7536 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/dlc/update_platform_dlc_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:13:44.629428 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/
+-rw-rw-r--   0 root         (0) root         (0)     6969 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    10698 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/consume_user_entitlement.py
+-rw-rw-r--   0 root         (0) root         (0)     8345 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/disable_user_entitlement.py
+-rw-rw-r--   0 root         (0) root         (0)     5910 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/enable_entitlement_orig_c90935.py
+-rw-rw-r--   0 root         (0) root         (0)     8418 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/enable_user_entitlement.py
+-rw-rw-r--   0 root         (0) root         (0)     8639 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/exists_any_user_active__9d3175.py
+-rw-rw-r--   0 root         (0) root         (0)    10362 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/exists_any_user_active__fca16a.py
+-rw-rw-r--   0 root         (0) root         (0)     6945 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/get_entitlement.py
+-rw-rw-r--   0 root         (0) root         (0)     6926 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/get_entitlement_config_info.py
+-rw-rw-r--   0 root         (0) root         (0)     7543 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/get_platform_entitlemen_32e517.py
+-rw-rw-r--   0 root         (0) root         (0)     8562 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/get_user_active_entitle_d52ca8.py
+-rw-rw-r--   0 root         (0) root         (0)     8757 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/get_user_app_entitlemen_2375db.py
+-rw-rw-r--   0 root         (0) root         (0)     7471 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/get_user_app_entitlemen_282639.py
+-rw-rw-r--   0 root         (0) root         (0)     7782 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/get_user_entitlement.py
+-rw-rw-r--   0 root         (0) root         (0)    11433 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/get_user_entitlement_by_8ab4a0.py
+-rw-rw-r--   0 root         (0) root         (0)    11292 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/get_user_entitlement_by_sku.py
+-rw-rw-r--   0 root         (0) root         (0)     7589 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/get_user_entitlement_histories.py
+-rw-rw-r--   0 root         (0) root         (0)     8625 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/get_user_entitlement_ow_5a8354.py
+-rw-rw-r--   0 root         (0) root         (0)    10110 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/get_user_entitlement_ow_dab0ca.py
+-rw-rw-r--   0 root         (0) root         (0)    10236 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/get_user_entitlement_ow_ec2b70.py
+-rw-rw-r--   0 root         (0) root         (0)     7605 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/grant_entitlements.py
+-rw-rw-r--   0 root         (0) root         (0)     8891 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/grant_user_entitlement.py
+-rw-rw-r--   0 root         (0) root         (0)     9104 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/pre_check_revoke_user_e_124298.py
+-rw-rw-r--   0 root         (0) root         (0)    11214 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_consume_user_ent_7254fa.py
+-rw-rw-r--   0 root         (0) root         (0)     8764 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_exists_any_my_ac_dbd2a5.py
+-rw-rw-r--   0 root         (0) root         (0)     9565 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_exists_any_user__3977e5.py
+-rw-rw-r--   0 root         (0) root         (0)    10027 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_get_entitlement__3fdfe7.py
+-rw-rw-r--   0 root         (0) root         (0)     6830 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_get_my_app_entit_4deb3f.py
+-rw-rw-r--   0 root         (0) root         (0)     8750 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_get_my_entitleme_22c2fd.py
+-rw-rw-r--   0 root         (0) root         (0)     8854 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_get_my_entitleme_cb2911.py
+-rw-rw-r--   0 root         (0) root         (0)     7839 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_get_user_app_ent_1e800f.py
+-rw-rw-r--   0 root         (0) root         (0)     7503 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_get_user_app_ent_53d109.py
+-rw-rw-r--   0 root         (0) root         (0)     7777 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_get_user_entitle_408425.py
+-rw-rw-r--   0 root         (0) root         (0)     9629 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_get_user_entitle_815992.py
+-rw-rw-r--   0 root         (0) root         (0)     9764 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_get_user_entitle_b1671e.py
+-rw-rw-r--   0 root         (0) root         (0)     9428 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_get_user_entitle_b313cf.py
+-rw-rw-r--   0 root         (0) root         (0)     8961 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_get_user_entitle_bb9230.py
+-rw-rw-r--   0 root         (0) root         (0)     9305 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_get_user_entitle_ee3005.py
+-rw-rw-r--   0 root         (0) root         (0)     7814 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_get_user_entitlement.py
+-rw-rw-r--   0 root         (0) root         (0)     9711 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_query_user_entit_2398e5.py
+-rw-rw-r--   0 root         (0) root         (0)    14302 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_query_user_entitlements.py
+-rw-rw-r--   0 root         (0) root         (0)    10507 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_sell_user_entitlement.py
+-rw-rw-r--   0 root         (0) root         (0)    10271 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_split_user_entitlement.py
+-rw-rw-r--   0 root         (0) root         (0)    10902 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_transfer_user_en_c358c0.py
+-rw-rw-r--   0 root         (0) root         (0)    12084 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_user_entitlement_741412.py
+-rw-rw-r--   0 root         (0) root         (0)    15627 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/query_entitlements.py
+-rw-rw-r--   0 root         (0) root         (0)     9420 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/query_entitlements_1.py
+-rw-rw-r--   0 root         (0) root         (0)    18615 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/query_user_entitlements.py
+-rw-rw-r--   0 root         (0) root         (0)    10575 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/query_user_entitlements_22cea1.py
+-rw-rw-r--   0 root         (0) root         (0)     6654 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/revoke_all_entitlements.py
+-rw-rw-r--   0 root         (0) root         (0)     7122 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/revoke_entitlements.py
+-rw-rw-r--   0 root         (0) root         (0)     9179 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/revoke_use_count.py
+-rw-rw-r--   0 root         (0) root         (0)     7833 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/revoke_user_entitlement.py
+-rw-rw-r--   0 root         (0) root         (0)     9201 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/revoke_user_entitlement_491388.py
+-rw-rw-r--   0 root         (0) root         (0)     7650 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/revoke_user_entitlements.py
+-rw-rw-r--   0 root         (0) root         (0)    10371 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/sell_user_entitlement.py
+-rw-rw-r--   0 root         (0) root         (0)     9214 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/update_platform_entitle_7fbd45.py
+-rw-rw-r--   0 root         (0) root         (0)     9754 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/update_user_entitlement.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:13:44.629428 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/fulfillment/
+-rw-rw-r--   0 root         (0) root         (0)      909 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/fulfillment/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8555 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/fulfillment/fulfill_item.py
+-rw-rw-r--   0 root         (0) root         (0)     8438 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/fulfillment/fulfill_rewards.py
+-rw-rw-r--   0 root         (0) root         (0)     8621 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/fulfillment/fulfill_rewards_v2.py
+-rw-rw-r--   0 root         (0) root         (0)     8456 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/fulfillment/pre_check_fulfill_item.py
+-rw-rw-r--   0 root         (0) root         (0)     9744 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/fulfillment/public_redeem_code.py
+-rw-rw-r--   0 root         (0) root         (0)     9559 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/fulfillment/query_fulfillment_histories.py
+-rw-rw-r--   0 root         (0) root         (0)     9368 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/fulfillment/redeem_code.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:13:44.629428 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/fulfillment_script/
+-rw-rw-r--   0 root         (0) root         (0)      777 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/fulfillment_script/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7307 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/fulfillment_script/create_fulfillment_script.py
+-rw-rw-r--   0 root         (0) root         (0)     5391 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/fulfillment_script/delete_fulfillment_script.py
+-rw-rw-r--   0 root         (0) root         (0)     5870 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/fulfillment_script/get_fulfillment_script.py
+-rw-rw-r--   0 root         (0) root         (0)     4720 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/fulfillment_script/list_fulfillment_scripts.py
+-rw-rw-r--   0 root         (0) root         (0)     7015 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/fulfillment_script/update_fulfillment_script.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:13:44.633428 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/
+-rw-rw-r--   0 root         (0) root         (0)     3689 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     5550 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/delete_apple_iap_config.py
+-rw-rw-r--   0 root         (0) root         (0)     5588 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/delete_epic_games_iap_config.py
+-rw-rw-r--   0 root         (0) root         (0)     5559 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/delete_google_iap_config.py
+-rw-rw-r--   0 root         (0) root         (0)     5583 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/delete_iap_item_config.py
+-rw-rw-r--   0 root         (0) root         (0)     5559 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/delete_oculus_iap_config.py
+-rw-rw-r--   0 root         (0) root         (0)     5604 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/delete_playstation_iap_config.py
+-rw-rw-r--   0 root         (0) root         (0)     5550 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/delete_steam_iap_config.py
+-rw-rw-r--   0 root         (0) root         (0)     5559 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/delete_twitch_iap_config.py
+-rw-rw-r--   0 root         (0) root         (0)     5527 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/delete_xbl_ap_config.py
+-rw-rw-r--   0 root         (0) root         (0)     5688 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/get_apple_iap_config.py
+-rw-rw-r--   0 root         (0) root         (0)     5750 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/get_epic_games_iap_config.py
+-rw-rw-r--   0 root         (0) root         (0)     5703 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/get_google_iap_config.py
+-rw-rw-r--   0 root         (0) root         (0)     5950 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/get_iap_item_config.py
+-rw-rw-r--   0 root         (0) root         (0)     7531 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/get_iap_item_mapping.py
+-rw-rw-r--   0 root         (0) root         (0)     5702 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/get_oculus_iap_config.py
+-rw-rw-r--   0 root         (0) root         (0)     5778 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/get_play_station_iap_config.py
+-rw-rw-r--   0 root         (0) root         (0)     5668 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/get_steam_iap_config.py
+-rw-rw-r--   0 root         (0) root         (0)     5703 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/get_twitch_iap_config.py
+-rw-rw-r--   0 root         (0) root         (0)     5661 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/get_xbl_iap_config.py
+-rw-rw-r--   0 root         (0) root         (0)     8538 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/mock_fulfill_iap_item.py
+-rw-rw-r--   0 root         (0) root         (0)     9059 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/public_fulfill_apple_iap_item.py
+-rw-rw-r--   0 root         (0) root         (0)     9624 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/public_fulfill_google_iap_item.py
+-rw-rw-r--   0 root         (0) root         (0)     9031 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/public_reconcile_play_s_6be6c0.py
+-rw-rw-r--   0 root         (0) root         (0)     8548 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/public_reconcile_play_s_7ac4de.py
+-rw-rw-r--   0 root         (0) root         (0)     6520 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/query_all_user_iap_orders.py
+-rw-rw-r--   0 root         (0) root         (0)    12664 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/query_user_iap_consume_history.py
+-rw-rw-r--   0 root         (0) root         (0)    13319 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/query_user_iap_orders.py
+-rw-rw-r--   0 root         (0) root         (0)     8295 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/sync_epic_games_inventory.py
+-rw-rw-r--   0 root         (0) root         (0)     6959 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/sync_oculus_consumable__f6c91d.py
+-rw-rw-r--   0 root         (0) root         (0)     7977 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/sync_steam_inventory.py
+-rw-rw-r--   0 root         (0) root         (0)     8023 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/sync_twitch_drops_entit_0c09ca.py
+-rw-rw-r--   0 root         (0) root         (0)     7284 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/sync_twitch_drops_entitlement.py
+-rw-rw-r--   0 root         (0) root         (0)     8133 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/sync_xbox_inventory.py
+-rw-rw-r--   0 root         (0) root         (0)     6899 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/update_apple_iap_config.py
+-rw-rw-r--   0 root         (0) root         (0)     6998 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/update_epic_games_iap_config.py
+-rw-rw-r--   0 root         (0) root         (0)     6923 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/update_google_iap_config.py
+-rw-rw-r--   0 root         (0) root         (0)     6685 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/update_google_p12_file.py
+-rw-rw-r--   0 root         (0) root         (0)     7921 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/update_iap_item_config.py
+-rw-rw-r--   0 root         (0) root         (0)     6922 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/update_oculus_iap_config.py
+-rw-rw-r--   0 root         (0) root         (0)     7408 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/update_playstation_iap_config.py
+-rw-rw-r--   0 root         (0) root         (0)     7259 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/update_steam_iap_config.py
+-rw-rw-r--   0 root         (0) root         (0)     6923 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/update_twitch_iap_config.py
+-rw-rw-r--   0 root         (0) root         (0)     7910 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/update_xbl_bp_cert_file.py
+-rw-rw-r--   0 root         (0) root         (0)     6851 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/update_xbl_iap_config.py
+-rw-rw-r--   0 root         (0) root         (0)     5825 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/validate_existed_playst_881975.py
+-rw-rw-r--   0 root         (0) root         (0)     7028 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/validate_playstation_ia_7dc74e.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:13:44.633428 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/invoice/
+-rw-rw-r--   0 root         (0) root         (0)      788 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/invoice/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    10715 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/invoice/download_invoice_details.py
+-rw-rw-r--   0 root         (0) root         (0)    11149 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/invoice/generate_invoice_summary.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:13:44.637428 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/
+-rw-rw-r--   0 root         (0) root         (0)     3746 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8019 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/acquire_item.py
+-rw-rw-r--   0 root         (0) root         (0)    10509 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/bulk_get_locale_items.py
+-rw-rw-r--   0 root         (0) root         (0)     9407 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/bulk_update_region_data.py
+-rw-rw-r--   0 root         (0) root         (0)    17365 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/create_item.py
+-rw-rw-r--   0 root         (0) root         (0)     6839 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/create_item_type_config.py
+-rw-rw-r--   0 root         (0) root         (0)     8816 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/defeature_item.py
+-rw-rw-r--   0 root         (0) root         (0)     8999 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/delete_item.py
+-rw-rw-r--   0 root         (0) root         (0)     5693 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/delete_item_type_config.py
+-rw-rw-r--   0 root         (0) root         (0)     7993 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/disable_item.py
+-rw-rw-r--   0 root         (0) root         (0)     7982 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/enable_item.py
+-rw-rw-r--   0 root         (0) root         (0)     8773 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/feature_item.py
+-rw-rw-r--   0 root         (0) root         (0)     8170 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/get_app.py
+-rw-rw-r--   0 root         (0) root         (0)     6033 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/get_available_predicate_types.py
+-rw-rw-r--   0 root         (0) root         (0)     7594 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/get_bulk_item_id_by_skus.py
+-rw-rw-r--   0 root         (0) root         (0)    10209 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/get_estimated_price.py
+-rw-rw-r--   0 root         (0) root         (0)     8784 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/get_item.py
+-rw-rw-r--   0 root         (0) root         (0)     8823 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/get_item_by_app_id.py
+-rw-rw-r--   0 root         (0) root         (0)     8707 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/get_item_by_sku.py
+-rw-rw-r--   0 root         (0) root         (0)     6810 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/get_item_dynamic_data.py
+-rw-rw-r--   0 root         (0) root         (0)     8756 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/get_item_id_by_sku.py
+-rw-rw-r--   0 root         (0) root         (0)     5819 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/get_item_type_config.py
+-rw-rw-r--   0 root         (0) root         (0)     8718 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/get_items.py
+-rw-rw-r--   0 root         (0) root         (0)    11585 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/get_locale_item.py
+-rw-rw-r--   0 root         (0) root         (0)    11517 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/get_locale_item_by_sku.py
+-rw-rw-r--   0 root         (0) root         (0)     7904 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/list_basic_items_by_features.py
+-rw-rw-r--   0 root         (0) root         (0)     4756 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/list_item_type_configs.py
+-rw-rw-r--   0 root         (0) root         (0)    10956 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/public_bulk_get_items.py
+-rw-rw-r--   0 root         (0) root         (0)     9370 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/public_get_app.py
+-rw-rw-r--   0 root         (0) root         (0)     8715 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/public_get_estimated_price.py
+-rw-rw-r--   0 root         (0) root         (0)    12021 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/public_get_item.py
+-rw-rw-r--   0 root         (0) root         (0)     9591 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/public_get_item_by_app_id.py
+-rw-rw-r--   0 root         (0) root         (0)    10802 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/public_get_item_by_sku.py
+-rw-rw-r--   0 root         (0) root         (0)     6645 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/public_get_item_dynamic_data.py
+-rw-rw-r--   0 root         (0) root         (0)    21639 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/public_query_items.py
+-rw-rw-r--   0 root         (0) root         (0)    14270 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/public_search_items.py
+-rw-rw-r--   0 root         (0) root         (0)     7472 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/public_validate_item_pu_bd546e.py
+-rw-rw-r--   0 root         (0) root         (0)    22154 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/query_items.py
+-rw-rw-r--   0 root         (0) root         (0)    25368 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/query_items_1.py
+-rw-rw-r--   0 root         (0) root         (0)    12202 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/query_uncategorized_items.py
+-rw-rw-r--   0 root         (0) root         (0)     8212 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/return_item.py
+-rw-rw-r--   0 root         (0) root         (0)     7659 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/search_item_type_config.py
+-rw-rw-r--   0 root         (0) root         (0)    13681 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/search_items.py
+-rw-rw-r--   0 root         (0) root         (0)     9757 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/sync_in_game_item.py
+-rw-rw-r--   0 root         (0) root         (0)    10831 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/update_app.py
+-rw-rw-r--   0 root         (0) root         (0)    18436 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/update_item.py
+-rw-rw-r--   0 root         (0) root         (0)     9735 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/update_item_purchase_condition.py
+-rw-rw-r--   0 root         (0) root         (0)     7676 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/update_item_type_config.py
+-rw-rw-r--   0 root         (0) root         (0)     9145 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/validate_item_purchase__929f78.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:13:44.641428 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/key_group/
+-rw-rw-r--   0 root         (0) root         (0)      895 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/key_group/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7465 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/key_group/create_key_group.py
+-rw-rw-r--   0 root         (0) root         (0)     6808 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/key_group/get_key_group.py
+-rw-rw-r--   0 root         (0) root         (0)     7055 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/key_group/get_key_group_by_booth_name.py
+-rw-rw-r--   0 root         (0) root         (0)     6945 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/key_group/get_key_group_dynamic.py
+-rw-rw-r--   0 root         (0) root         (0)     9347 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/key_group/list_keys.py
+-rw-rw-r--   0 root         (0) root         (0)     8840 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/key_group/query_key_groups.py
+-rw-rw-r--   0 root         (0) root         (0)     8665 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/key_group/update_key_group.py
+-rw-rw-r--   0 root         (0) root         (0)     8076 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/key_group/upload_keys.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:13:44.641428 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/order/
+-rw-rw-r--   0 root         (0) root         (0)     1820 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/order/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    11472 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/order/admin_create_user_order.py
+-rw-rw-r--   0 root         (0) root         (0)     7456 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/order/count_of_purchased_item.py
+-rw-rw-r--   0 root         (0) root         (0)     7781 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/order/download_user_order_receipt.py
+-rw-rw-r--   0 root         (0) root         (0)     8442 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/order/fulfill_user_order.py
+-rw-rw-r--   0 root         (0) root         (0)     6602 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/order/get_order.py
+-rw-rw-r--   0 root         (0) root         (0)     5662 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/order/get_order_statistics.py
+-rw-rw-r--   0 root         (0) root         (0)     7449 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/order/get_user_order.py
+-rw-rw-r--   0 root         (0) root         (0)     7272 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/order/get_user_order_grant.py
+-rw-rw-r--   0 root         (0) root         (0)     7324 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/order/get_user_order_histories.py
+-rw-rw-r--   0 root         (0) root         (0)     8687 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/order/process_user_order_noti_fdd9f8.py
+-rw-rw-r--   0 root         (0) root         (0)     7817 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/order/public_cancel_user_order.py
+-rw-rw-r--   0 root         (0) root         (0)    11467 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/order/public_create_user_order.py
+-rw-rw-r--   0 root         (0) root         (0)     7813 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/order/public_download_user_or_6ea3e8.py
+-rw-rw-r--   0 root         (0) root         (0)     7515 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/order/public_get_user_order.py
+-rw-rw-r--   0 root         (0) root         (0)     7342 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/order/public_get_user_order_h_063753.py
+-rw-rw-r--   0 root         (0) root         (0)    10777 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/order/public_query_user_orders.py
+-rw-rw-r--   0 root         (0) root         (0)    13760 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/order/query_orders.py
+-rw-rw-r--   0 root         (0) root         (0)    10727 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/order/query_user_orders.py
+-rw-rw-r--   0 root         (0) root         (0)     8393 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/order/refund_order.py
+-rw-rw-r--   0 root         (0) root         (0)     9211 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/order/update_user_order_status.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:13:44.641428 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/order_dedicated/
+-rw-rw-r--   0 root         (0) root         (0)      506 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/order_dedicated/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7276 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/order_dedicated/sync_orders.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:13:44.641428 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment/
+-rw-rw-r--   0 root         (0) root         (0)     1346 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     9065 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment/charge_payment_order.py
+-rw-rw-r--   0 root         (0) root         (0)    10139 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment/create_user_payment_order.py
+-rw-rw-r--   0 root         (0) root         (0)     7004 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment/get_payment_order.py
+-rw-rw-r--   0 root         (0) root         (0)     7189 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment/get_payment_order_charg_9acbf8.py
+-rw-rw-r--   0 root         (0) root         (0)     6651 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment/list_ext_order_no_by_ext_tx_id.py
+-rw-rw-r--   0 root         (0) root         (0)    15334 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment/query_payment_notifications.py
+-rw-rw-r--   0 root         (0) root         (0)    11380 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment/query_payment_orders.py
+-rw-rw-r--   0 root         (0) root         (0)     9723 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment/refund_user_payment_order.py
+-rw-rw-r--   0 root         (0) root         (0)     8957 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment/simulate_payment_order__cf0fbc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:13:44.641428 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_account/
+-rw-rw-r--   0 root         (0) root         (0)      705 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_account/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8283 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_account/public_delete_payment_account.py
+-rw-rw-r--   0 root         (0) root         (0)     6627 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_account/public_get_payment_accounts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:13:44.641428 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_callback_config/
+-rw-rw-r--   0 root         (0) root         (0)      608 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_callback_config/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     6220 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_callback_config/get_payment_callback_config.py
+-rw-rw-r--   0 root         (0) root         (0)     7166 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_callback_config/update_payment_callback_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:13:44.645428 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_config/
+-rw-rw-r--   0 root         (0) root         (0)     2494 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_config/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7826 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_config/create_payment_provider_config.py
+-rw-rw-r--   0 root         (0) root         (0)     7043 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_config/debug_matched_payment_m_9bf142.py
+-rw-rw-r--   0 root         (0) root         (0)     7038 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_config/debug_matched_payment_p_02dcf1.py
+-rw-rw-r--   0 root         (0) root         (0)     5793 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_config/delete_payment_provider_config.py
+-rw-rw-r--   0 root         (0) root         (0)     4746 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_config/get_aggregate_payment_p_41c63c.py
+-rw-rw-r--   0 root         (0) root         (0)     5954 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_config/get_payment_merchant_config.py
+-rw-rw-r--   0 root         (0) root         (0)     4751 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_config/get_payment_tax_config.py
+-rw-rw-r--   0 root         (0) root         (0)     4730 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_config/get_special_payment_providers.py
+-rw-rw-r--   0 root         (0) root         (0)     8328 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_config/query_payment_provider_config.py
+-rw-rw-r--   0 root         (0) root         (0)     7090 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_config/test_adyen_config.py
+-rw-rw-r--   0 root         (0) root         (0)     6868 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_config/test_adyen_config_by_id.py
+-rw-rw-r--   0 root         (0) root         (0)     6903 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_config/test_ali_pay_config.py
+-rw-rw-r--   0 root         (0) root         (0)     6969 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_config/test_ali_pay_config_by_id.py
+-rw-rw-r--   0 root         (0) root         (0)     6921 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_config/test_checkout_config.py
+-rw-rw-r--   0 root         (0) root         (0)     6900 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_config/test_checkout_config_by_id.py
+-rw-rw-r--   0 root         (0) root         (0)     6926 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_config/test_pay_pal_config.py
+-rw-rw-r--   0 root         (0) root         (0)     6924 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_config/test_pay_pal_config_by_id.py
+-rw-rw-r--   0 root         (0) root         (0)     6973 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_config/test_stripe_config.py
+-rw-rw-r--   0 root         (0) root         (0)     6878 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_config/test_stripe_config_by_id.py
+-rw-rw-r--   0 root         (0) root         (0)     5995 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_config/test_wx_pay_config.py
+-rw-rw-r--   0 root         (0) root         (0)     6012 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_config/test_wx_pay_config_by_id.py
+-rw-rw-r--   0 root         (0) root         (0)     6053 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_config/test_xsolla_config.py
+-rw-rw-r--   0 root         (0) root         (0)     6009 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_config/test_xsolla_config_by_id.py
+-rw-rw-r--   0 root         (0) root         (0)     9053 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_config/update_adyen_config.py
+-rw-rw-r--   0 root         (0) root         (0)     9087 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_config/update_ali_pay_config.py
+-rw-rw-r--   0 root         (0) root         (0)     9121 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_config/update_checkout_config.py
+-rw-rw-r--   0 root         (0) root         (0)     9073 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_config/update_pay_pal_config.py
+-rw-rw-r--   0 root         (0) root         (0)     8877 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_config/update_payment_provider_config.py
+-rw-rw-r--   0 root         (0) root         (0)     7373 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_config/update_payment_tax_config.py
+-rw-rw-r--   0 root         (0) root         (0)     9073 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_config/update_stripe_config.py
+-rw-rw-r--   0 root         (0) root         (0)     8308 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_config/update_wx_pay_config.py
+-rw-rw-r--   0 root         (0) root         (0)     6909 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_config/update_wx_pay_config_cert.py
+-rw-rw-r--   0 root         (0) root         (0)     8350 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_config/update_xsolla_config.py
+-rw-rw-r--   0 root         (0) root         (0)     7279 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_config/update_xsolla_ui_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:13:44.645428 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_dedicated/
+-rw-rw-r--   0 root         (0) root         (0)      669 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_dedicated/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    17317 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_dedicated/create_payment_order_by_79f85c.py
+-rw-rw-r--   0 root         (0) root         (0)    14953 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_dedicated/refund_payment_order_by_309df5.py
+-rw-rw-r--   0 root         (0) root         (0)     7420 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_dedicated/sync_payment_orders.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:13:44.649428 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_station/
+-rw-rw-r--   0 root         (0) root         (0)     1595 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_station/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     9272 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_station/get_payment_customization.py
+-rw-rw-r--   0 root         (0) root         (0)     9073 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_station/get_payment_public_config.py
+-rw-rw-r--   0 root         (0) root         (0)     9767 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_station/get_payment_tax_value.py
+-rw-rw-r--   0 root         (0) root         (0)    11264 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_station/pay.py
+-rw-rw-r--   0 root         (0) root         (0)     7048 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_station/public_check_payment_or_dec069.py
+-rw-rw-r--   0 root         (0) root         (0)     7013 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_station/public_get_payment_methods.py
+-rw-rw-r--   0 root         (0) root         (0)     7844 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_station/public_get_payment_url.py
+-rw-rw-r--   0 root         (0) root         (0)     6143 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_station/public_get_qr_code.py
+-rw-rw-r--   0 root         (0) root         (0)     7438 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_station/public_get_unpaid_payme_26d8dd.py
+-rw-rw-r--   0 root         (0) root         (0)    21889 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_station/public_normalize_paymen_6657a5.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:13:44.649428 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/revocation/
+-rw-rw-r--   0 root         (0) root         (0)      904 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/revocation/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     5484 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/revocation/delete_revocation_config.py
+-rw-rw-r--   0 root         (0) root         (0)     7449 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/revocation/do_revocation.py
+-rw-rw-r--   0 root         (0) root         (0)     5969 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/revocation/get_revocation_config.py
+-rw-rw-r--   0 root         (0) root         (0)    13168 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/revocation/query_revocation_histories.py
+-rw-rw-r--   0 root         (0) root         (0)     6829 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/revocation/update_revocation_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:13:44.649428 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/reward/
+-rw-rw-r--   0 root         (0) root         (0)     1152 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/reward/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8055 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/reward/check_event_condition.py
+-rw-rw-r--   0 root         (0) root         (0)     9060 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/reward/create_reward.py
+-rw-rw-r--   0 root         (0) root         (0)     6774 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/reward/delete_reward.py
+-rw-rw-r--   0 root         (0) root         (0)     7852 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/reward/delete_reward_condition_record.py
+-rw-rw-r--   0 root         (0) root         (0)     5625 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/reward/export_rewards.py
+-rw-rw-r--   0 root         (0) root         (0)     6729 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/reward/get_reward.py
+-rw-rw-r--   0 root         (0) root         (0)     6726 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/reward/get_reward_1.py
+-rw-rw-r--   0 root         (0) root         (0)     6974 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/reward/get_reward_by_code.py
+-rw-rw-r--   0 root         (0) root         (0)     8939 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/reward/import_rewards.py
+-rw-rw-r--   0 root         (0) root         (0)    10354 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/reward/query_rewards.py
+-rw-rw-r--   0 root         (0) root         (0)    10368 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/reward/query_rewards_1.py
+-rw-rw-r--   0 root         (0) root         (0)     9501 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/reward/update_reward.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:13:44.649428 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/section/
+-rw-rw-r--   0 root         (0) root         (0)      795 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/section/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     9442 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/section/create_section.py
+-rw-rw-r--   0 root         (0) root         (0)     7981 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/section/delete_section.py
+-rw-rw-r--   0 root         (0) root         (0)     7999 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/section/get_section.py
+-rw-rw-r--   0 root         (0) root         (0)    11868 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/section/public_list_active_sections.py
+-rw-rw-r--   0 root         (0) root         (0)     6834 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/section/purge_expired_section.py
+-rw-rw-r--   0 root         (0) root         (0)    11262 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/section/query_sections.py
+-rw-rw-r--   0 root         (0) root         (0)    10409 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/section/update_section.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:13:44.653428 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/service_plugin_config/
+-rw-rw-r--   0 root         (0) root         (0)     1560 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/service_plugin_config/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     5496 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/service_plugin_config/delete_loot_box_plugin_config.py
+-rw-rw-r--   0 root         (0) root         (0)     5529 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/service_plugin_config/delete_revocation_plugi_c2651d.py
+-rw-rw-r--   0 root         (0) root         (0)     5496 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/service_plugin_config/delete_section_plugin_config.py
+-rw-rw-r--   0 root         (0) root         (0)     5543 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/service_plugin_config/delete_service_plugin_config.py
+-rw-rw-r--   0 root         (0) root         (0)     6467 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/service_plugin_config/get_loot_box_grpc_info.py
+-rw-rw-r--   0 root         (0) root         (0)     5591 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/service_plugin_config/get_loot_box_plugin_config.py
+-rw-rw-r--   0 root         (0) root         (0)     5642 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/service_plugin_config/get_revocation_plugin_config.py
+-rw-rw-r--   0 root         (0) root         (0)     5591 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/service_plugin_config/get_section_plugin_config.py
+-rw-rw-r--   0 root         (0) root         (0)     5638 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/service_plugin_config/get_service_plugin_config.py
+-rw-rw-r--   0 root         (0) root         (0)     7269 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/service_plugin_config/update_loot_box_plugin_config.py
+-rw-rw-r--   0 root         (0) root         (0)     7386 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/service_plugin_config/update_revocation_plugi_c19001.py
+-rw-rw-r--   0 root         (0) root         (0)     7262 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/service_plugin_config/update_section_plugin_config.py
+-rw-rw-r--   0 root         (0) root         (0)     7317 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/service_plugin_config/update_service_plugin_config.py
+-rw-rw-r--   0 root         (0) root         (0)     7165 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/service_plugin_config/upload_revocation_plugi_6c586a.py
+-rw-rw-r--   0 root         (0) root         (0)     7089 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/service_plugin_config/upload_section_plugin_c_780cdd.py
+-rw-rw-r--   0 root         (0) root         (0)     7083 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/service_plugin_config/uplod_loot_box_plugin_c_5c5812.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:13:44.653428 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/session_platform/
+-rw-rw-r--   0 root         (0) root         (0)      525 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/session_platform/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7814 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/session_platform/register_xbl_sessions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:13:44.653428 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/store/
+-rw-rw-r--   0 root         (0) root         (0)     1495 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/store/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8215 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/store/clone_store.py
+-rw-rw-r--   0 root         (0) root         (0)     7412 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/store/create_store.py
+-rw-rw-r--   0 root         (0) root         (0)     6120 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/store/delete_published_store.py
+-rw-rw-r--   0 root         (0) root         (0)     6988 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/store/delete_store.py
+-rw-rw-r--   0 root         (0) root         (0)     5626 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/store/download_csv_templates.py
+-rw-rw-r--   0 root         (0) root         (0)     6745 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/store/export_store.py
+-rw-rw-r--   0 root         (0) root         (0)     7810 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/store/export_store_1.py
+-rw-rw-r--   0 root         (0) root         (0)     8019 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/store/export_store_by_csv.py
+-rw-rw-r--   0 root         (0) root         (0)     7219 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/store/get_catalog_definition.py
+-rw-rw-r--   0 root         (0) root         (0)     6044 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/store/get_published_store.py
+-rw-rw-r--   0 root         (0) root         (0)     6293 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/store/get_published_store_backup.py
+-rw-rw-r--   0 root         (0) root         (0)     6666 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/store/get_store.py
+-rw-rw-r--   0 root         (0) root         (0)     8926 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/store/import_store.py
+-rw-rw-r--   0 root         (0) root         (0)     9058 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/store/import_store_1.py
+-rw-rw-r--   0 root         (0) root         (0)    12067 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/store/import_store_by_csv.py
+-rw-rw-r--   0 root         (0) root         (0)     5617 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/store/list_stores.py
+-rw-rw-r--   0 root         (0) root         (0)     5699 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/store/public_list_stores.py
+-rw-rw-r--   0 root         (0) root         (0)    11585 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/store/query_import_history.py
+-rw-rw-r--   0 root         (0) root         (0)     6269 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/store/rollback_published_store.py
+-rw-rw-r--   0 root         (0) root         (0)     8601 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/store/update_store.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:13:44.653428 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/subscription/
+-rw-rw-r--   0 root         (0) root         (0)     2500 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/subscription/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    10657 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/subscription/cancel_subscription.py
+-rw-rw-r--   0 root         (0) root         (0)     7635 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/subscription/check_user_subscription_6c59a6.py
+-rw-rw-r--   0 root         (0) root         (0)     7461 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/subscription/delete_user_subscription.py
+-rw-rw-r--   0 root         (0) root         (0)     7813 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/subscription/get_user_subscription.py
+-rw-rw-r--   0 root         (0) root         (0)    10509 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/subscription/get_user_subscription_a_b2b8e9.py
+-rw-rw-r--   0 root         (0) root         (0)    10413 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/subscription/get_user_subscription_b_a3096e.py
+-rw-rw-r--   0 root         (0) root         (0)     9388 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/subscription/grant_days_to_subscription.py
+-rw-rw-r--   0 root         (0) root         (0)     9261 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/subscription/platform_subscribe_subs_ad4f3b.py
+-rw-rw-r--   0 root         (0) root         (0)     8974 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/subscription/process_user_subscripti_d07750.py
+-rw-rw-r--   0 root         (0) root         (0)     9712 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/subscription/public_cancel_subscription.py
+-rw-rw-r--   0 root         (0) root         (0)     9022 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/subscription/public_change_subscript_350ff2.py
+-rw-rw-r--   0 root         (0) root         (0)     7709 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/subscription/public_check_user_subsc_16fdcb.py
+-rw-rw-r--   0 root         (0) root         (0)    10483 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/subscription/public_get_user_subscri_c8d5b3.py
+-rw-rw-r--   0 root         (0) root         (0)     7845 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/subscription/public_get_user_subscription.py
+-rw-rw-r--   0 root         (0) root         (0)    13920 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/subscription/public_query_user_subsc_29ae74.py
+-rw-rw-r--   0 root         (0) root         (0)    10640 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/subscription/public_subscribe_subscription.py
+-rw-rw-r--   0 root         (0) root         (0)    13775 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/subscription/query_subscriptions.py
+-rw-rw-r--   0 root         (0) root         (0)    13838 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/subscription/query_user_subscriptions.py
+-rw-rw-r--   0 root         (0) root         (0)     7040 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/subscription/recurring_charge_subscription.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:13:44.657428 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/ticket/
+-rw-rw-r--   0 root         (0) root         (0)      726 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/ticket/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     9606 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/ticket/acquire_user_ticket.py
+-rw-rw-r--   0 root         (0) root         (0)     8398 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/ticket/decrease_ticket_sale.py
+-rw-rw-r--   0 root         (0) root         (0)     6839 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/ticket/get_ticket_booth_id.py
+-rw-rw-r--   0 root         (0) root         (0)     6899 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/ticket/get_ticket_dynamic.py
+-rw-rw-r--   0 root         (0) root         (0)     8584 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/ticket/increase_ticket_sale.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:13:44.657428 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/trade_action/
+-rw-rw-r--   0 root         (0) root         (0)      743 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/trade_action/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7151 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/trade_action/commit.py
+-rw-rw-r--   0 root         (0) root         (0)    10222 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/trade_action/get_trade_history_by_criteria.py
+-rw-rw-r--   0 root         (0) root         (0)     6707 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/trade_action/get_trade_history_by_tr_8b774c.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:13:44.657428 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/view/
+-rw-rw-r--   0 root         (0) root         (0)      689 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/view/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8999 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/view/create_view.py
+-rw-rw-r--   0 root         (0) root         (0)     7879 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/view/delete_view.py
+-rw-rw-r--   0 root         (0) root         (0)     7855 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/view/get_view.py
+-rw-rw-r--   0 root         (0) root         (0)     7399 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/view/list_views.py
+-rw-rw-r--   0 root         (0) root         (0)     8337 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/view/public_list_views.py
+-rw-rw-r--   0 root         (0) root         (0)     9906 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/view/update_view.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:13:44.657428 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/wallet/
+-rw-rw-r--   0 root         (0) root         (0)     2161 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/wallet/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7218 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/wallet/bulk_credit.py
+-rw-rw-r--   0 root         (0) root         (0)     7197 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/wallet/bulk_debit.py
+-rw-rw-r--   0 root         (0) root         (0)     9106 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/wallet/check_balance.py
+-rw-rw-r--   0 root         (0) root         (0)     9937 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/wallet/check_wallet.py
+-rw-rw-r--   0 root         (0) root         (0)     9224 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/wallet/credit_user_wallet.py
+-rw-rw-r--   0 root         (0) root         (0)     9738 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/wallet/debit_by_wallet_platform.py
+-rw-rw-r--   0 root         (0) root         (0)     9616 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/wallet/debit_user_wallet.py
+-rw-rw-r--   0 root         (0) root         (0)     9652 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/wallet/debit_user_wallet_by_cu_54daab.py
+-rw-rw-r--   0 root         (0) root         (0)     7713 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/wallet/disable_user_wallet.py
+-rw-rw-r--   0 root         (0) root         (0)     7702 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/wallet/enable_user_wallet.py
+-rw-rw-r--   0 root         (0) root         (0)     7434 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/wallet/get_platform_wallet_config.py
+-rw-rw-r--   0 root         (0) root         (0)     7583 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/wallet/get_user_wallet.py
+-rw-rw-r--   0 root         (0) root         (0)     6747 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/wallet/get_wallet.py
+-rw-rw-r--   0 root         (0) root         (0)     9708 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/wallet/list_user_currency_tran_bb67cf.py
+-rw-rw-r--   0 root         (0) root         (0)     9692 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/wallet/list_user_wallet_transactions.py
+-rw-rw-r--   0 root         (0) root         (0)     9329 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/wallet/pay_with_user_wallet.py
+-rw-rw-r--   0 root         (0) root         (0)     6844 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/wallet/public_get_my_wallet.py
+-rw-rw-r--   0 root         (0) root         (0)     7392 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/wallet/public_get_wallet.py
+-rw-rw-r--   0 root         (0) root         (0)     9425 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/wallet/public_list_user_wallet_ed4de4.py
+-rw-rw-r--   0 root         (0) root         (0)     6611 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/wallet/query_user_currency_wallets.py
+-rw-rw-r--   0 root         (0) root         (0)    10777 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/wallet/query_wallets.py
+-rw-rw-r--   0 root         (0) root         (0)     7483 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/wallet/reset_platform_wallet_config.py
+-rw-rw-r--   0 root         (0) root         (0)     8703 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/wallet/update_platform_wallet_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:13:44.661428 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/wrappers/
+-rw-rw-r--   0 root         (0) root         (0)    45555 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/wrappers/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    10487 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/wrappers/_achievement_platform.py
+-rw-rw-r--   0 root         (0) root         (0)    26101 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/wrappers/_anonymization.py
+-rw-rw-r--   0 root         (0) root         (0)    50598 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/wrappers/_campaign.py
+-rw-rw-r--   0 root         (0) root         (0)    36673 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/wrappers/_catalog_changes.py
+-rw-rw-r--   0 root         (0) root         (0)    44980 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/wrappers/_category.py
+-rw-rw-r--   0 root         (0) root         (0)     8439 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/wrappers/_clawback.py
+-rw-rw-r--   0 root         (0) root         (0)    22453 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/wrappers/_currency.py
+-rw-rw-r--   0 root         (0) root         (0)    45845 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/wrappers/_dlc.py
+-rw-rw-r--   0 root         (0) root         (0)   223241 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/wrappers/_entitlement.py
+-rw-rw-r--   0 root         (0) root         (0)    28776 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/wrappers/_fulfillment.py
+-rw-rw-r--   0 root         (0) root         (0)    12953 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/wrappers/_fulfillment_script.py
+-rw-rw-r--   0 root         (0) root         (0)   137043 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/wrappers/_iap.py
+-rw-rw-r--   0 root         (0) root         (0)     8814 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/wrappers/_invoice.py
+-rw-rw-r--   0 root         (0) root         (0)   214448 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/wrappers/_item.py
+-rw-rw-r--   0 root         (0) root         (0)    26602 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/wrappers/_key_group.py
+-rw-rw-r--   0 root         (0) root         (0)    73916 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/wrappers/_order.py
+-rw-rw-r--   0 root         (0) root         (0)     3784 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/wrappers/_order_dedicated.py
+-rw-rw-r--   0 root         (0) root         (0)    37849 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/wrappers/_payment.py
+-rw-rw-r--   0 root         (0) root         (0)     7464 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/wrappers/_payment_account.py
+-rw-rw-r--   0 root         (0) root         (0)     7193 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/wrappers/_payment_callback_config.py
+-rw-rw-r--   0 root         (0) root         (0)    99745 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/wrappers/_payment_config.py
+-rw-rw-r--   0 root         (0) root         (0)    40570 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/wrappers/_payment_dedicated.py
+-rw-rw-r--   0 root         (0) root         (0)    39913 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/wrappers/_payment_station.py
+-rw-rw-r--   0 root         (0) root         (0)    15959 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/wrappers/_revocation.py
+-rw-rw-r--   0 root         (0) root         (0)    42027 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/wrappers/_reward.py
+-rw-rw-r--   0 root         (0) root         (0)    28694 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/wrappers/_section.py
+-rw-rw-r--   0 root         (0) root         (0)    43145 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/wrappers/_service_plugin_config.py
+-rw-rw-r--   0 root         (0) root         (0)     4085 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/wrappers/_session_platform.py
+-rw-rw-r--   0 root         (0) root         (0)    64567 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/wrappers/_store.py
+-rw-rw-r--   0 root         (0) root         (0)    80269 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/wrappers/_subscription.py
+-rw-rw-r--   0 root         (0) root         (0)    18108 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/wrappers/_ticket.py
+-rw-rw-r--   0 root         (0) root         (0)    10954 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/wrappers/_trade_action.py
+-rw-rw-r--   0 root         (0) root         (0)    22228 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/wrappers/_view.py
+-rw-rw-r--   0 root         (0) root         (0)    80449 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/wrappers/_wallet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:13:44.665428 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk_service_platform.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1129 2024-03-13 06:13:44.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk_service_platform.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    64096 2024-03-13 06:13:44.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk_service_platform.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-03-13 06:13:44.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk_service_platform.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-03-13 06:13:44.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk_service_platform.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-03-13 06:13:44.000000 accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk_service_platform.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)      361 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-platform-0.9.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-03-13 06:13:44.665428 accelbyte-py-sdk-service-platform-0.9.0/setup.cfg
```

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/PKG-INFO` & `accelbyte-py-sdk-service-platform-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: accelbyte-py-sdk-service-platform
-Version: 0.8.0
+Version: 0.9.0
 Summary: AccelByte Python SDK - AccelByte Gaming Services Platform Service
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: accelbyte-py-sdk-core
 
 [//]: # (Code generated. DO NOT EDIT!)
 
 # AccelByte Modular Python SDK - Service Module
 
 This is a service module for the [AccelByte Modular Python SDK](https://github.com/AccelByte/accelbyte-python-modular-sdk) package.
 
 ```text
 AccelByte Gaming Services Platform Service
-* Version: 4.47.0
+* Version: 4.48.0
 ```
 
 ## Setup
 
 This SDK requires Python 3.9 to be installed.
 
 ### Install with Pip
```

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/README.md` & `accelbyte-py-sdk-service-platform-0.9.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # AccelByte Modular Python SDK - Service Module
 
 This is a service module for the [AccelByte Modular Python SDK](https://github.com/AccelByte/accelbyte-python-modular-sdk) package.
 
 ```text
 AccelByte Gaming Services Platform Service
-* Version: 4.47.0
+* Version: 4.48.0
 ```
 
 ## Setup
 
 This SDK requires Python 3.9 to be installed.
 
 ### Install with Pip
```

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/__init__.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: service-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Platform Service."""
 
-__version__ = "4.47.0"
+__version__ = "4.48.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 # achievement_platform
 from .wrappers import get_xbl_user_achievements
@@ -259,14 +259,16 @@
 from .wrappers import public_query_user_entitlements_by_app_type_async
 from .wrappers import public_sell_user_entitlement
 from .wrappers import public_sell_user_entitlement_async
 from .wrappers import public_split_user_entitlement
 from .wrappers import public_split_user_entitlement_async
 from .wrappers import public_transfer_user_entitlement
 from .wrappers import public_transfer_user_entitlement_async
+from .wrappers import public_user_entitlement_history
+from .wrappers import public_user_entitlement_history_async
 from .wrappers import query_entitlements
 from .wrappers import query_entitlements_async
 from .wrappers import query_entitlements_1
 from .wrappers import query_entitlements_1_async
 from .wrappers import query_user_entitlements
 from .wrappers import query_user_entitlements_async
 from .wrappers import query_user_entitlements_by_app_type
```

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/__init__.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: model-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Platform Service."""
 
-__version__ = "4.47.0"
+__version__ = "4.48.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .achievement_info import AchievementInfo
 from .action import Action
@@ -205,15 +205,14 @@
     EntitlementOriginSyncStatusEnum as DLCRecordEntitlementOriginSyncStatusEnum,
 )
 from .dlc_record import StatusEnum as DLCRecordStatusEnum
 from .durable_entitlement_revocation_config import DurableEntitlementRevocationConfig
 from .durable_entitlement_revocation_config import (
     StrategyEnum as DurableEntitlementRevocationConfigStrategyEnum,
 )
-from .entitlement_origin_sync_result import EntitlementOriginSyncResult
 from .entitlement_config_info import EntitlementConfigInfo
 from .entitlement_decrement import EntitlementDecrement
 from .entitlement_decrement_result import EntitlementDecrementResult
 from .entitlement_decrement_result import (
     ClazzEnum as EntitlementDecrementResultClazzEnum,
 )
 from .entitlement_decrement_result import (
@@ -231,14 +230,15 @@
 from .entitlement_decrement_result import TypeEnum as EntitlementDecrementResultTypeEnum
 from .entitlement_grant import EntitlementGrant
 from .entitlement_grant import OriginEnum as EntitlementGrantOriginEnum
 from .entitlement_grant import SourceEnum as EntitlementGrantSourceEnum
 from .entitlement_grant_result import EntitlementGrantResult
 from .entitlement_history_info import EntitlementHistoryInfo
 from .entitlement_history_info import ActionEnum as EntitlementHistoryInfoActionEnum
+from .entitlement_history_info import ClazzEnum as EntitlementHistoryInfoClazzEnum
 from .entitlement_history_info import OriginEnum as EntitlementHistoryInfoOriginEnum
 from .entitlement_ifc import EntitlementIfc
 from .entitlement_ifc import AppTypeEnum as EntitlementIfcAppTypeEnum
 from .entitlement_ifc import ClazzEnum as EntitlementIfcClazzEnum
 from .entitlement_ifc import OriginEnum as EntitlementIfcOriginEnum
 from .entitlement_ifc import StatusEnum as EntitlementIfcStatusEnum
 from .entitlement_ifc import TypeEnum as EntitlementIfcTypeEnum
@@ -246,14 +246,15 @@
 from .entitlement_info import ClazzEnum as EntitlementInfoClazzEnum
 from .entitlement_info import StatusEnum as EntitlementInfoStatusEnum
 from .entitlement_info import AppTypeEnum as EntitlementInfoAppTypeEnum
 from .entitlement_info import OriginEnum as EntitlementInfoOriginEnum
 from .entitlement_info import SourceEnum as EntitlementInfoSourceEnum
 from .entitlement_info import TypeEnum as EntitlementInfoTypeEnum
 from .entitlement_loot_box_reward import EntitlementLootBoxReward
+from .entitlement_origin_sync_result import EntitlementOriginSyncResult
 from .entitlement_ownership import EntitlementOwnership
 from .entitlement_paging_sliced_result import EntitlementPagingSlicedResult
 from .entitlement_platform_config_info import EntitlementPlatformConfigInfo
 from .entitlement_platform_config_update import EntitlementPlatformConfigUpdate
 from .entitlement_platform_config_update import (
     AllowedPlatformOriginsEnum as EntitlementPlatformConfigUpdateAllowedPlatformOriginsEnum,
 )
@@ -654,14 +655,24 @@
 from .predicate import ComparisonEnum as PredicateComparisonEnum
 from .predicate import PredicateTypeEnum as PredicatePredicateTypeEnum
 from .predicate_validate_result import PredicateValidateResult
 from .public_custom_config_info import PublicCustomConfigInfo
 from .public_custom_config_info import (
     ConnectionTypeEnum as PublicCustomConfigInfoConnectionTypeEnum,
 )
+from .public_entitlement_history_info import PublicEntitlementHistoryInfo
+from .public_entitlement_history_info import (
+    ActionEnum as PublicEntitlementHistoryInfoActionEnum,
+)
+from .public_entitlement_history_info import (
+    ClazzEnum as PublicEntitlementHistoryInfoClazzEnum,
+)
+from .public_entitlement_history_info import (
+    OriginEnum as PublicEntitlementHistoryInfoOriginEnum,
+)
 from .purchase_condition import PurchaseCondition
 from .purchase_condition_update import PurchaseConditionUpdate
 from .purchased_item_count import PurchasedItemCount
 from .recurring import Recurring
 from .recurring import CycleEnum as RecurringCycleEnum
 from .recurring_charge_result import RecurringChargeResult
 from .redeemable_item import RedeemableItem
@@ -831,14 +842,17 @@
 from .user_dlc import PlatformEnum as UserDLCPlatformEnum
 from .user_dlc_record import UserDLCRecord
 from .user_dlc_record import (
     EntitlementOriginSyncStatusEnum as UserDLCRecordEntitlementOriginSyncStatusEnum,
 )
 from .user_dlc_record import PlatformEnum as UserDLCRecordPlatformEnum
 from .user_dlc_record import StatusEnum as UserDLCRecordStatusEnum
+from .user_entitlement_history_paging_sliced_result import (
+    UserEntitlementHistoryPagingSlicedResult,
+)
 from .validation_error_entity import ValidationErrorEntity
 from .view_create import ViewCreate
 from .view_info import ViewInfo
 from .view_update import ViewUpdate
 from .wallet_info import WalletInfo
 from .wallet_info import StatusEnum as WalletInfoStatusEnum
 from .wallet_paging_sliced_result import WalletPagingSlicedResult
```

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/achievement_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/achievement_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/action.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/action.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/action_request.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/action_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/additional_data.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/additional_data.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/additional_data_entitlement.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/additional_data_entitlement.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/admin_entitlement_decrement.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/admin_entitlement_decrement.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/admin_entitlement_sold_request.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/admin_entitlement_sold_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/admin_order_create.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/admin_order_create.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/adyen_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/adyen_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/ali_pay_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/ali_pay_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/app_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/app_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/app_entitlement_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/app_entitlement_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/app_entitlement_paging_sliced_result.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/app_entitlement_paging_sliced_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/app_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/app_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/app_localization.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/app_localization.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/app_update.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/app_update.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/apple_iap_config_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/apple_iap_config_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/apple_iap_config_request.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/apple_iap_config_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/apple_iap_receipt.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/apple_iap_receipt.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/available_comparison.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/available_comparison.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/available_predicate.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/available_predicate.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/available_price.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/available_price.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/base_custom_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/base_custom_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/base_tls_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/base_tls_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/basic_category_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/basic_category_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/basic_item.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/basic_item.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/billing_account.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/billing_account.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/billing_history_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/billing_history_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/billing_history_paging_sliced_result.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/billing_history_paging_sliced_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/box_item.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/box_item.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/bulk_credit_request.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/bulk_credit_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/bulk_credit_result.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/bulk_credit_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/bulk_debit_request.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/bulk_debit_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/bulk_debit_result.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/bulk_debit_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/bulk_entitlement_grant_request.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/bulk_entitlement_grant_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/bulk_entitlement_grant_result.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/bulk_entitlement_grant_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/bulk_entitlement_revoke_result.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/bulk_entitlement_revoke_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/bulk_operation_result.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/bulk_operation_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/bulk_region_data_change_request.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/bulk_region_data_change_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/bundled_item_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/bundled_item_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/campaign_create.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/campaign_create.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/campaign_dynamic_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/campaign_dynamic_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/campaign_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/campaign_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/campaign_paging_sliced_result.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/campaign_paging_sliced_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/campaign_update.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/campaign_update.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/cancel_request.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/cancel_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/catalog_change_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/catalog_change_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/catalog_change_paging_result.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/catalog_change_paging_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/catalog_change_statistics.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/catalog_change_statistics.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/catalog_definition_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/catalog_definition_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/category_create.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/category_create.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/category_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/category_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/category_update.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/category_update.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/checkout_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/checkout_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/clawback_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/clawback_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/client_request_parameter.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/client_request_parameter.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/client_transaction.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/client_transaction.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/code_create.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/code_create.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/code_create_result.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/code_create_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/code_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/code_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/code_info_paging_sliced_result.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/code_info_paging_sliced_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/condition_group.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/condition_group.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/condition_group_validate_result.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/condition_group_validate_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/condition_match_result.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/condition_match_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/consumable_entitlement_revocation_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/consumable_entitlement_revocation_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/consume_item.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/consume_item.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/credit_payload.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/credit_payload.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/credit_request.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/credit_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/credit_result.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/credit_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/credit_revocation.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/credit_revocation.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/credit_summary.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/credit_summary.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/currency_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/currency_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/currency_create.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/currency_create.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/currency_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/currency_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/currency_summary.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/currency_summary.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/currency_update.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/currency_update.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/currency_wallet.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/currency_wallet.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/customization.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/customization.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/debit_by_currency_code_request.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/debit_by_currency_code_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/debit_by_wallet_platform_request.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/debit_by_wallet_platform_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/debit_payload.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/debit_payload.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/debit_request.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/debit_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/debit_result.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/debit_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/delete_reward_condition_request.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/delete_reward_condition_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/detailed_wallet_transaction_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/detailed_wallet_transaction_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/detailed_wallet_transaction_paging_sliced_result.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/detailed_wallet_transaction_paging_sliced_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/dlc_config_reward_short_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/dlc_config_reward_short_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/dlc_item.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/dlc_item.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/dlc_item_config_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/dlc_item_config_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/dlc_item_config_update.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/dlc_item_config_update.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/dlc_record.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/dlc_record.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -24,18 +24,18 @@
 
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Model
 from accelbyte_py_sdk.core import StrEnum
 
+from ..models.entitlement_origin_sync_result import EntitlementOriginSyncResult
 from ..models.platform_reward import PlatformReward
 from ..models.revocation_result import RevocationResult
 from ..models.revoke_result import RevokeResult
-from ..models.entitlement_origin_sync_result import EntitlementOriginSyncResult
 
 
 class EntitlementOriginSyncStatusEnum(StrEnum):
     NOT_SYNCED = "NOT_SYNCED"
     SYNCED = "SYNCED"
     SYNCED_FAILED = "SYNCED_FAILED"
```

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/durable_entitlement_revocation_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/durable_entitlement_revocation_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/entitlement_config_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/entitlement_config_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/entitlement_decrement.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/entitlement_decrement.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/entitlement_decrement_result.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/entitlement_decrement_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/entitlement_grant.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/entitlement_grant.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/entitlement_grant_result.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/entitlement_grant_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/entitlement_history_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/entitlement_history_info.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,14 +35,24 @@
     ENABLE = "ENABLE"
     GRANT = "GRANT"
     REVOKE = "REVOKE"
     SELL_BACK = "SELL_BACK"
     UPDATE = "UPDATE"
 
 
+class ClazzEnum(StrEnum):
+    APP = "APP"
+    CODE = "CODE"
+    ENTITLEMENT = "ENTITLEMENT"
+    LOOTBOX = "LOOTBOX"
+    MEDIA = "MEDIA"
+    OPTIONBOX = "OPTIONBOX"
+    SUBSCRIPTION = "SUBSCRIPTION"
+
+
 class OriginEnum(StrEnum):
     EPIC = "Epic"
     GOOGLEPLAY = "GooglePlay"
     IOS = "IOS"
     NINTENDO = "Nintendo"
     OCULUS = "Oculus"
     OTHER = "Other"
@@ -67,34 +77,43 @@
 
         operator: (operator) REQUIRED str
 
         updated_at: (updatedAt) REQUIRED str
 
         user_id: (userId) REQUIRED str
 
+        clazz: (clazz) OPTIONAL Union[str, ClazzEnum]
+
+        item_id: (itemId) OPTIONAL str
+
         origin: (origin) OPTIONAL Union[str, OriginEnum]
 
         reason: (reason) OPTIONAL str
 
+        sku: (sku) OPTIONAL str
+
         use_count: (useCount) OPTIONAL int
 
         use_count_change: (useCountChange) OPTIONAL int
     """
 
     # region fields
 
     action: Union[str, ActionEnum]  # REQUIRED
     created_at: str  # REQUIRED
     entitlement_id: str  # REQUIRED
     namespace: str  # REQUIRED
     operator: str  # REQUIRED
     updated_at: str  # REQUIRED
     user_id: str  # REQUIRED
+    clazz: Union[str, ClazzEnum]  # OPTIONAL
+    item_id: str  # OPTIONAL
     origin: Union[str, OriginEnum]  # OPTIONAL
     reason: str  # OPTIONAL
+    sku: str  # OPTIONAL
     use_count: int  # OPTIONAL
     use_count_change: int  # OPTIONAL
 
     # endregion fields
 
     # region with_x methods
 
@@ -122,22 +141,34 @@
         self.updated_at = value
         return self
 
     def with_user_id(self, value: str) -> EntitlementHistoryInfo:
         self.user_id = value
         return self
 
+    def with_clazz(self, value: Union[str, ClazzEnum]) -> EntitlementHistoryInfo:
+        self.clazz = value
+        return self
+
+    def with_item_id(self, value: str) -> EntitlementHistoryInfo:
+        self.item_id = value
+        return self
+
     def with_origin(self, value: Union[str, OriginEnum]) -> EntitlementHistoryInfo:
         self.origin = value
         return self
 
     def with_reason(self, value: str) -> EntitlementHistoryInfo:
         self.reason = value
         return self
 
+    def with_sku(self, value: str) -> EntitlementHistoryInfo:
+        self.sku = value
+        return self
+
     def with_use_count(self, value: int) -> EntitlementHistoryInfo:
         self.use_count = value
         return self
 
     def with_use_count_change(self, value: int) -> EntitlementHistoryInfo:
         self.use_count_change = value
         return self
@@ -172,22 +203,34 @@
             result["updatedAt"] = str(self.updated_at)
         elif include_empty:
             result["updatedAt"] = ""
         if hasattr(self, "user_id"):
             result["userId"] = str(self.user_id)
         elif include_empty:
             result["userId"] = ""
+        if hasattr(self, "clazz"):
+            result["clazz"] = str(self.clazz)
+        elif include_empty:
+            result["clazz"] = Union[str, ClazzEnum]()
+        if hasattr(self, "item_id"):
+            result["itemId"] = str(self.item_id)
+        elif include_empty:
+            result["itemId"] = ""
         if hasattr(self, "origin"):
             result["origin"] = str(self.origin)
         elif include_empty:
             result["origin"] = Union[str, OriginEnum]()
         if hasattr(self, "reason"):
             result["reason"] = str(self.reason)
         elif include_empty:
             result["reason"] = ""
+        if hasattr(self, "sku"):
+            result["sku"] = str(self.sku)
+        elif include_empty:
+            result["sku"] = ""
         if hasattr(self, "use_count"):
             result["useCount"] = int(self.use_count)
         elif include_empty:
             result["useCount"] = 0
         if hasattr(self, "use_count_change"):
             result["useCountChange"] = int(self.use_count_change)
         elif include_empty:
@@ -204,32 +247,41 @@
         action: Union[str, ActionEnum],
         created_at: str,
         entitlement_id: str,
         namespace: str,
         operator: str,
         updated_at: str,
         user_id: str,
+        clazz: Optional[Union[str, ClazzEnum]] = None,
+        item_id: Optional[str] = None,
         origin: Optional[Union[str, OriginEnum]] = None,
         reason: Optional[str] = None,
+        sku: Optional[str] = None,
         use_count: Optional[int] = None,
         use_count_change: Optional[int] = None,
         **kwargs,
     ) -> EntitlementHistoryInfo:
         instance = cls()
         instance.action = action
         instance.created_at = created_at
         instance.entitlement_id = entitlement_id
         instance.namespace = namespace
         instance.operator = operator
         instance.updated_at = updated_at
         instance.user_id = user_id
+        if clazz is not None:
+            instance.clazz = clazz
+        if item_id is not None:
+            instance.item_id = item_id
         if origin is not None:
             instance.origin = origin
         if reason is not None:
             instance.reason = reason
+        if sku is not None:
+            instance.sku = sku
         if use_count is not None:
             instance.use_count = use_count
         if use_count_change is not None:
             instance.use_count_change = use_count_change
         return instance
 
     @classmethod
@@ -263,22 +315,34 @@
             instance.updated_at = str(dict_["updatedAt"])
         elif include_empty:
             instance.updated_at = ""
         if "userId" in dict_ and dict_["userId"] is not None:
             instance.user_id = str(dict_["userId"])
         elif include_empty:
             instance.user_id = ""
+        if "clazz" in dict_ and dict_["clazz"] is not None:
+            instance.clazz = str(dict_["clazz"])
+        elif include_empty:
+            instance.clazz = Union[str, ClazzEnum]()
+        if "itemId" in dict_ and dict_["itemId"] is not None:
+            instance.item_id = str(dict_["itemId"])
+        elif include_empty:
+            instance.item_id = ""
         if "origin" in dict_ and dict_["origin"] is not None:
             instance.origin = str(dict_["origin"])
         elif include_empty:
             instance.origin = Union[str, OriginEnum]()
         if "reason" in dict_ and dict_["reason"] is not None:
             instance.reason = str(dict_["reason"])
         elif include_empty:
             instance.reason = ""
+        if "sku" in dict_ and dict_["sku"] is not None:
+            instance.sku = str(dict_["sku"])
+        elif include_empty:
+            instance.sku = ""
         if "useCount" in dict_ and dict_["useCount"] is not None:
             instance.use_count = int(dict_["useCount"])
         elif include_empty:
             instance.use_count = 0
         if "useCountChange" in dict_ and dict_["useCountChange"] is not None:
             instance.use_count_change = int(dict_["useCountChange"])
         elif include_empty:
@@ -329,32 +393,38 @@
             "action": "action",
             "createdAt": "created_at",
             "entitlementId": "entitlement_id",
             "namespace": "namespace",
             "operator": "operator",
             "updatedAt": "updated_at",
             "userId": "user_id",
+            "clazz": "clazz",
+            "itemId": "item_id",
             "origin": "origin",
             "reason": "reason",
+            "sku": "sku",
             "useCount": "use_count",
             "useCountChange": "use_count_change",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
             "action": True,
             "createdAt": True,
             "entitlementId": True,
             "namespace": True,
             "operator": True,
             "updatedAt": True,
             "userId": True,
+            "clazz": False,
+            "itemId": False,
             "origin": False,
             "reason": False,
+            "sku": False,
             "useCount": False,
             "useCountChange": False,
         }
 
     @staticmethod
     def get_enum_map() -> Dict[str, List[Any]]:
         return {
@@ -363,14 +433,23 @@
                 "DISABLE",
                 "ENABLE",
                 "GRANT",
                 "REVOKE",
                 "SELL_BACK",
                 "UPDATE",
             ],
+            "clazz": [
+                "APP",
+                "CODE",
+                "ENTITLEMENT",
+                "LOOTBOX",
+                "MEDIA",
+                "OPTIONBOX",
+                "SUBSCRIPTION",
+            ],
             "origin": [
                 "Epic",
                 "GooglePlay",
                 "IOS",
                 "Nintendo",
                 "Oculus",
                 "Other",
```

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/entitlement_ifc.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/entitlement_ifc.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/entitlement_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/entitlement_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/entitlement_loot_box_reward.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/entitlement_loot_box_reward.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/entitlement_origin_sync_result.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/entitlement_origin_sync_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 from accelbyte_py_sdk.core import Model
 
 from ..models.platform_reward import PlatformReward
 from ..models.reward_migration_result import RewardMigrationResult
 
 
 class EntitlementOriginSyncResult(Model):
-    """Entitlement origin sync result (entitlement origin sync result)
+    """entitlement origin sync result (EntitlementOriginSyncResult)
 
     Properties:
         reason: (reason) OPTIONAL str
 
         reward: (reward) OPTIONAL PlatformReward
 
         summary: (summary) OPTIONAL List[RewardMigrationResult]
```

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/entitlement_ownership.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/entitlement_ownership.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/entitlement_paging_sliced_result.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/entitlement_paging_sliced_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/entitlement_platform_config_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/entitlement_platform_config_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/entitlement_platform_config_update.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/entitlement_platform_config_update.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/entitlement_prechek_result.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/entitlement_prechek_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/entitlement_revocation.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/entitlement_revocation.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/entitlement_revocation_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/entitlement_revocation_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/entitlement_revoke_result.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/entitlement_revoke_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/entitlement_sold_request.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/entitlement_sold_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/entitlement_sold_result.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/entitlement_sold_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/entitlement_split_request.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/entitlement_split_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/entitlement_split_result.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/entitlement_split_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/entitlement_summary.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/entitlement_summary.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/entitlement_transfer_request.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/entitlement_transfer_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/entitlement_transfer_result.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/entitlement_transfer_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/entitlement_update.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/entitlement_update.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/epic_games_dlc_sync_request.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/epic_games_dlc_sync_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/epic_games_iap_config_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/epic_games_iap_config_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/epic_games_iap_config_request.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/epic_games_iap_config_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/epic_games_reconcile_request.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/epic_games_reconcile_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/epic_games_reconcile_result.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/epic_games_reconcile_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/error_entity.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/error_entity.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/estimated_price_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/estimated_price_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/event_additional_data.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/event_additional_data.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/event_payload.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/event_payload.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/export_store_request.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/export_store_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/export_store_to_csv_request.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/export_store_to_csv_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/extension_fulfillment_summary.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/extension_fulfillment_summary.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/external_payment_order_create.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/external_payment_order_create.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/field_validation_error.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/field_validation_error.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/fixed_period_rotation_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/fixed_period_rotation_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/ful_fill_item_payload.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/ful_fill_item_payload.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/fulfill_code_request.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/fulfill_code_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/fulfillment_error.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/fulfillment_error.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/fulfillment_history_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/fulfillment_history_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/fulfillment_history_paging_sliced_result.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/fulfillment_history_paging_sliced_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/fulfillment_item.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/fulfillment_item.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/fulfillment_request.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/fulfillment_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/fulfillment_result.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/fulfillment_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/fulfillment_script_create.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/fulfillment_script_create.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/fulfillment_script_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/fulfillment_script_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/fulfillment_script_update.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/fulfillment_script_update.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/full_app_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/full_app_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/full_category_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/full_category_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/full_item_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/full_item_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/full_item_paging_result.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/full_item_paging_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/full_item_paging_sliced_result.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/full_item_paging_sliced_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/full_section_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/full_section_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/full_view_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/full_view_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/google_iap_config_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/google_iap_config_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/google_iap_config_request.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/google_iap_config_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/google_iap_receipt.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/google_iap_receipt.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/google_receipt_resolve_result.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/google_receipt_resolve_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/grant_subscription_days_request.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/grant_subscription_days_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/grpc_server_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/grpc_server_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/hierarchical_category_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/hierarchical_category_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/iap_clawback_paging_sliced_result.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/iap_clawback_paging_sliced_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/iap_consume_history_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/iap_consume_history_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/iap_consume_history_paging_sliced_result.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/iap_consume_history_paging_sliced_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/iap_item_config_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/iap_item_config_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/iap_item_config_update.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/iap_item_config_update.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/iap_item_entry.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/iap_item_entry.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/iap_item_flat_entry.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/iap_item_flat_entry.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/iap_item_mapping_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/iap_item_mapping_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/iap_order_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/iap_order_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/iap_order_paging_sliced_result.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/iap_order_paging_sliced_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/image.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/image.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/import_error_details.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/import_error_details.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/import_store_app_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/import_store_app_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/import_store_category_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/import_store_category_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/import_store_error.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/import_store_error.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/import_store_history_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/import_store_history_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/import_store_history_paging_result.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/import_store_history_paging_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/import_store_item_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/import_store_item_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/import_store_result.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/import_store_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/import_store_section_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/import_store_section_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/import_store_view_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/import_store_view_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/in_game_item_sync.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/in_game_item_sync.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/inventory_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/inventory_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/invoice_currency_summary.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/invoice_currency_summary.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/invoice_summary.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/invoice_summary.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/item_acquire_request.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/item_acquire_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/item_acquire_result.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/item_acquire_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/item_create.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/item_create.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/item_dynamic_data_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/item_dynamic_data_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/item_id.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/item_id.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/item_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/item_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/item_naming.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/item_naming.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/item_paging_sliced_result.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/item_paging_sliced_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/item_purchase_condition_validate_request.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/item_purchase_condition_validate_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/item_purchase_condition_validate_result.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/item_purchase_condition_validate_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/item_return_request.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/item_return_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/item_revocation.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/item_revocation.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/item_snapshot.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/item_snapshot.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/item_type_config_create.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/item_type_config_create.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/item_type_config_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/item_type_config_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/item_type_config_update.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/item_type_config_update.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/item_update.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/item_update.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/key_group_create.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/key_group_create.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/key_group_dynamic_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/key_group_dynamic_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/key_group_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/key_group_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/key_group_paging_sliced_result.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/key_group_paging_sliced_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/key_group_update.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/key_group_update.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/key_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/key_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/key_paging_slice_result.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/key_paging_slice_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/list_view_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/list_view_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/localization.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/localization.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/loot_box_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/loot_box_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/loot_box_plugin_config_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/loot_box_plugin_config_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/loot_box_plugin_config_update.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/loot_box_plugin_config_update.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/loot_box_reward.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/loot_box_reward.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/mock_iap_receipt.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/mock_iap_receipt.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/notification_process_result.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/notification_process_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/oculus_iap_config_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/oculus_iap_config_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/oculus_iap_config_request.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/oculus_iap_config_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/oculus_reconcile_result.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/oculus_reconcile_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/operation.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/operation.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/operation_request.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/operation_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/option_box_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/option_box_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/order.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/order.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/order_bundle_item_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/order_bundle_item_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/order_create.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/order_create.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/order_creation_options.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/order_creation_options.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/order_grant_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/order_grant_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/order_history_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/order_history_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/order_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/order_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/order_paging_result.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/order_paging_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/order_paging_sliced_result.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/order_paging_sliced_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/order_refund_create.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/order_refund_create.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/order_statistics.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/order_statistics.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/order_summary.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/order_summary.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/order_sync_result.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/order_sync_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/order_update.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/order_update.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/ownership.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/ownership.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/ownership_token.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/ownership_token.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/paging.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/paging.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/pay_pal_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/pay_pal_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/payment_account.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/payment_account.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/payment_callback_config_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/payment_callback_config_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/payment_callback_config_update.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/payment_callback_config_update.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/payment_merchant_config_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/payment_merchant_config_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/payment_method.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/payment_method.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/payment_notification_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/payment_notification_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/payment_notification_paging_sliced_result.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/payment_notification_paging_sliced_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/payment_order.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/payment_order.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/payment_order_charge_request.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/payment_order_charge_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/payment_order_charge_status.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/payment_order_charge_status.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/payment_order_create.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/payment_order_create.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/payment_order_create_result.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/payment_order_create_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/payment_order_details.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/payment_order_details.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/payment_order_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/payment_order_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/payment_order_notify_simulation.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/payment_order_notify_simulation.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/payment_order_paging_sliced_result.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/payment_order_paging_sliced_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/payment_order_paid_result.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/payment_order_paid_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/payment_order_refund.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/payment_order_refund.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/payment_order_refund_result.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/payment_order_refund_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/payment_order_sync_result.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/payment_order_sync_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/payment_process_result.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/payment_process_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/payment_provider_config_edit.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/payment_provider_config_edit.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/payment_provider_config_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/payment_provider_config_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/payment_provider_config_paging_sliced_result.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/payment_provider_config_paging_sliced_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/payment_request.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/payment_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/payment_tax_config_edit.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/payment_tax_config_edit.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/payment_tax_config_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/payment_tax_config_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/payment_token.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/payment_token.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/payment_url.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/payment_url.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/payment_url_create.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/payment_url_create.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/platform_dlc_config_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/platform_dlc_config_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/platform_dlc_config_update.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/platform_dlc_config_update.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/platform_dlc_entry.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/platform_dlc_entry.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/platform_reward.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/platform_reward.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/platform_reward_currency.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/platform_reward_currency.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/platform_reward_item.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/platform_reward_item.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/platform_subscribe_request.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/platform_subscribe_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/platform_wallet.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/platform_wallet.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/platform_wallet_config_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/platform_wallet_config_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/platform_wallet_config_update.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/platform_wallet_config_update.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/play_station_dlc_sync_multi_service_labels_request.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/play_station_dlc_sync_multi_service_labels_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/play_station_dlc_sync_request.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/play_station_dlc_sync_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/play_station_iap_config_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/play_station_iap_config_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/play_station_multi_service_labels_reconcile_request.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/play_station_multi_service_labels_reconcile_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/play_station_reconcile_request.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/play_station_reconcile_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/play_station_reconcile_result.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/play_station_reconcile_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/playstation_iap_config_request.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/playstation_iap_config_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/populated_item_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/populated_item_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/pre_check_fulfillment_request.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/pre_check_fulfillment_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/predicate.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/predicate.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/predicate_validate_result.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/predicate_validate_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/public_custom_config_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/public_custom_config_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/purchase_condition.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/purchase_condition.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/purchase_condition_update.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/purchase_condition_update.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/purchased_item_count.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/purchased_item_count.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/recurring.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/recurring.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/recurring_charge_result.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/recurring_charge_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/redeem_history_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/redeem_history_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/redeem_history_paging_sliced_result.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/redeem_history_paging_sliced_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/redeem_request.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/redeem_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/redeem_result.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/redeem_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/redeemable_item.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/redeemable_item.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/region_data_change.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/region_data_change.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/region_data_item.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/region_data_item.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/region_data_item_dto.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/region_data_item_dto.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/request_history.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/request_history.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/requirement.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/requirement.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/revocation_config_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/revocation_config_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/revocation_config_update.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/revocation_config_update.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/revocation_error.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/revocation_error.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/revocation_history_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/revocation_history_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/revocation_history_paging_sliced_result.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/revocation_history_paging_sliced_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/revocation_plugin_config_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/revocation_plugin_config_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/revocation_plugin_config_update.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/revocation_plugin_config_update.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/revocation_request.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/revocation_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/revocation_result.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/revocation_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/revoke_currency.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/revoke_currency.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/revoke_entitlement.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/revoke_entitlement.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/revoke_entitlement_payload.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/revoke_entitlement_payload.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/revoke_entry.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/revoke_entry.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/revoke_item.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/revoke_item.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/revoke_item_summary.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/revoke_item_summary.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/revoke_result.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/revoke_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/revoke_use_count_request.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/revoke_use_count_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/reward_condition.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/reward_condition.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/reward_create.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/reward_create.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/reward_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/reward_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/reward_item.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/reward_item.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/reward_migration_result.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/reward_migration_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/reward_paging_sliced_result.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/reward_paging_sliced_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/reward_update.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/reward_update.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/rewards_request.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/rewards_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/sale_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/sale_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/section_create.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/section_create.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/section_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/section_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/section_item.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/section_item.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/section_paging_sliced_result.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/section_paging_sliced_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/section_plugin_config_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/section_plugin_config_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/section_plugin_config_update.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/section_plugin_config_update.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/section_update.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/section_update.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/service_plugin_config_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/service_plugin_config_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/service_plugin_config_update.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/service_plugin_config_update.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/slide.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/slide.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/stackable_entitlement_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/stackable_entitlement_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/steam_achievement.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/steam_achievement.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/steam_achievement_update_request.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/steam_achievement_update_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/steam_dlc_sync_request.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/steam_dlc_sync_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/steam_iap_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/steam_iap_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/steam_iap_config_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/steam_iap_config_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/steam_iap_config_request.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/steam_iap_config_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/steam_sync_request.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/steam_sync_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/store_backup_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/store_backup_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/store_create.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/store_create.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/store_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/store_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/store_update.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/store_update.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/stream_event.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/stream_event.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/stream_event_body.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/stream_event_body.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/stripe_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/stripe_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/sub_item_available_price.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/sub_item_available_price.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/subscribable.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/subscribable.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/subscribe_request.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/subscribe_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/subscription_activity_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/subscription_activity_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/subscription_activity_paging_sliced_result.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/subscription_activity_paging_sliced_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/subscription_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/subscription_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/subscription_paging_sliced_result.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/subscription_paging_sliced_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/subscription_summary.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/subscription_summary.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/tax_result.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/tax_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/test_result.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/test_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/ticket_acquire_request.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/ticket_acquire_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/ticket_acquire_result.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/ticket_acquire_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/ticket_booth_id.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/ticket_booth_id.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/ticket_dynamic_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/ticket_dynamic_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/ticket_sale_decrement_request.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/ticket_sale_decrement_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/ticket_sale_increment_request.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/ticket_sale_increment_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/ticket_sale_increment_result.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/ticket_sale_increment_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/time_limited_balance.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/time_limited_balance.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/timed_ownership.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/timed_ownership.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/tls_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/tls_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/trade_action_paging_sliced_result.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/trade_action_paging_sliced_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/trade_chain_action_history_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/trade_chain_action_history_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/trade_chained_action_commit_request.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/trade_chained_action_commit_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/trade_notification.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/trade_notification.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/transaction.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/transaction.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/transaction_amount_details.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/transaction_amount_details.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/twitch_iap_config_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/twitch_iap_config_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/twitch_iap_config_request.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/twitch_iap_config_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/twitch_sync_request.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/twitch_sync_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/twitch_sync_result.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/twitch_sync_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/user_dlc.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/user_dlc.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/user_dlc_record.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/user_dlc_record.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -24,18 +24,18 @@
 
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Model
 from accelbyte_py_sdk.core import StrEnum
 
+from ..models.entitlement_origin_sync_result import EntitlementOriginSyncResult
 from ..models.platform_reward import PlatformReward
 from ..models.revocation_result import RevocationResult
 from ..models.revoke_result import RevokeResult
-from ..models.entitlement_origin_sync_result import EntitlementOriginSyncResult
 
 
 class EntitlementOriginSyncStatusEnum(StrEnum):
     NOT_SYNCED = "NOT_SYNCED"
     SYNCED = "SYNCED"
     SYNCED_FAILED = "SYNCED_FAILED"
```

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/validation_error_entity.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/validation_error_entity.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/view_create.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/view_create.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/view_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/view_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/view_update.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/view_update.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/wallet_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/wallet_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/wallet_paging_sliced_result.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/wallet_paging_sliced_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/wallet_revocation_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/wallet_revocation_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/wallet_transaction_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/wallet_transaction_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/wallet_transaction_paging_sliced_result.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/wallet_transaction_paging_sliced_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/wx_pay_config_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/wx_pay_config_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/wx_pay_config_request.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/wx_pay_config_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/xbl_achievement_update_request.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/xbl_achievement_update_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/xbl_dlc_sync_request.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/xbl_dlc_sync_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/xbl_iap_config_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/xbl_iap_config_info.py`

 * *Files 22% similar despite different names*

```diff
@@ -30,36 +30,43 @@
 
 class XblIAPConfigInfo(Model):
     """Xbl IAP config info (XblIAPConfigInfo)
 
     Properties:
         namespace: (namespace) REQUIRED str
 
+        business_partner_cert_expired_time: (businessPartnerCertExpiredTime) OPTIONAL str
+
         business_partner_cert_file_name: (businessPartnerCertFileName) OPTIONAL str
 
         password: (password) OPTIONAL str
 
         relying_party_cert: (relyingPartyCert) OPTIONAL str
     """
 
     # region fields
 
     namespace: str  # REQUIRED
+    business_partner_cert_expired_time: str  # OPTIONAL
     business_partner_cert_file_name: str  # OPTIONAL
     password: str  # OPTIONAL
     relying_party_cert: str  # OPTIONAL
 
     # endregion fields
 
     # region with_x methods
 
     def with_namespace(self, value: str) -> XblIAPConfigInfo:
         self.namespace = value
         return self
 
+    def with_business_partner_cert_expired_time(self, value: str) -> XblIAPConfigInfo:
+        self.business_partner_cert_expired_time = value
+        return self
+
     def with_business_partner_cert_file_name(self, value: str) -> XblIAPConfigInfo:
         self.business_partner_cert_file_name = value
         return self
 
     def with_password(self, value: str) -> XblIAPConfigInfo:
         self.password = value
         return self
@@ -74,14 +81,20 @@
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
         if hasattr(self, "namespace"):
             result["namespace"] = str(self.namespace)
         elif include_empty:
             result["namespace"] = ""
+        if hasattr(self, "business_partner_cert_expired_time"):
+            result["businessPartnerCertExpiredTime"] = str(
+                self.business_partner_cert_expired_time
+            )
+        elif include_empty:
+            result["businessPartnerCertExpiredTime"] = ""
         if hasattr(self, "business_partner_cert_file_name"):
             result["businessPartnerCertFileName"] = str(
                 self.business_partner_cert_file_name
             )
         elif include_empty:
             result["businessPartnerCertFileName"] = ""
         if hasattr(self, "password"):
@@ -98,21 +111,26 @@
 
     # region static methods
 
     @classmethod
     def create(
         cls,
         namespace: str,
+        business_partner_cert_expired_time: Optional[str] = None,
         business_partner_cert_file_name: Optional[str] = None,
         password: Optional[str] = None,
         relying_party_cert: Optional[str] = None,
         **kwargs,
     ) -> XblIAPConfigInfo:
         instance = cls()
         instance.namespace = namespace
+        if business_partner_cert_expired_time is not None:
+            instance.business_partner_cert_expired_time = (
+                business_partner_cert_expired_time
+            )
         if business_partner_cert_file_name is not None:
             instance.business_partner_cert_file_name = business_partner_cert_file_name
         if password is not None:
             instance.password = password
         if relying_party_cert is not None:
             instance.relying_party_cert = relying_party_cert
         return instance
@@ -125,14 +143,23 @@
         if not dict_:
             return instance
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
         elif include_empty:
             instance.namespace = ""
         if (
+            "businessPartnerCertExpiredTime" in dict_
+            and dict_["businessPartnerCertExpiredTime"] is not None
+        ):
+            instance.business_partner_cert_expired_time = str(
+                dict_["businessPartnerCertExpiredTime"]
+            )
+        elif include_empty:
+            instance.business_partner_cert_expired_time = ""
+        if (
             "businessPartnerCertFileName" in dict_
             and dict_["businessPartnerCertFileName"] is not None
         ):
             instance.business_partner_cert_file_name = str(
                 dict_["businessPartnerCertFileName"]
             )
         elif include_empty:
@@ -181,22 +208,24 @@
         else:
             return cls.create_from_dict(any_, include_empty=include_empty)
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
             "namespace": "namespace",
+            "businessPartnerCertExpiredTime": "business_partner_cert_expired_time",
             "businessPartnerCertFileName": "business_partner_cert_file_name",
             "password": "password",
             "relyingPartyCert": "relying_party_cert",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
             "namespace": True,
+            "businessPartnerCertExpiredTime": False,
             "businessPartnerCertFileName": False,
             "password": False,
             "relyingPartyCert": False,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/xbl_iap_config_request.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/xbl_iap_config_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/xbl_reconcile_request.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/xbl_reconcile_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/xbl_reconcile_result.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/xbl_reconcile_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/xbl_user_achievements.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/xbl_user_achievements.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/xbl_user_session_request.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/xbl_user_session_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/xbox_achievement.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/xbox_achievement.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/xsolla_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/xsolla_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/xsolla_paywall_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/xsolla_paywall_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/models/xsolla_paywall_config_request.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/models/xsolla_paywall_config_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/achievement_platform/__init__.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/achievement_platform/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Platform Service."""
 
-__version__ = "4.47.0"
+__version__ = "4.48.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .get_xbl_user_achievements import GetXblUserAchievements
 from .unlock_steam_user_achievement import UnlockSteamUserAchievement
```

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/achievement_platform/get_xbl_user_achievements.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/achievement_platform/get_xbl_user_achievements.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/achievement_platform/unlock_steam_user_achievement.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/achievement_platform/unlock_steam_user_achievement.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/achievement_platform/update_xbl_user_achievement.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/achievement_platform/update_xbl_user_achievement.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/anonymization/__init__.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/anonymization/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Platform Service."""
 
-__version__ = "4.47.0"
+__version__ = "4.48.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .anonymize_campaign import AnonymizeCampaign
 from .anonymize_entitlement import AnonymizeEntitlement
```

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/anonymization/anonymize_campaign.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/anonymization/anonymize_campaign.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/anonymization/anonymize_entitlement.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/anonymization/anonymize_entitlement.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/anonymization/anonymize_fulfillment.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/anonymization/anonymize_fulfillment.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/anonymization/anonymize_integration.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/anonymization/anonymize_integration.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/anonymization/anonymize_order.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/anonymization/anonymize_order.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/anonymization/anonymize_payment.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/anonymization/anonymize_payment.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/anonymization/anonymize_revocation.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/anonymization/anonymize_revocation.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/anonymization/anonymize_subscription.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/anonymization/anonymize_subscription.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/anonymization/anonymize_wallet.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/anonymization/anonymize_wallet.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/campaign/__init__.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/campaign/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Platform Service."""
 
-__version__ = "4.47.0"
+__version__ = "4.48.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .apply_user_redemption import ApplyUserRedemption
 from .bulk_disable_codes import BulkDisableCodes
```

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/campaign/apply_user_redemption.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/campaign/apply_user_redemption.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/campaign/bulk_disable_codes.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/campaign/bulk_disable_codes.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/campaign/bulk_enable_codes.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/campaign/bulk_enable_codes.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/campaign/create_campaign.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/campaign/create_campaign.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/campaign/create_codes.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/campaign/create_codes.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/campaign/disable_code.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/campaign/disable_code.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/campaign/download.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/campaign/download.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/campaign/enable_code.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/campaign/enable_code.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/campaign/get_campaign.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/campaign/get_campaign.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/campaign/get_campaign_dynamic.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/campaign/get_campaign_dynamic.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/campaign/get_code.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/campaign/get_code.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/campaign/query_campaigns.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/campaign/query_campaigns.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/campaign/query_codes.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/campaign/query_codes.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/campaign/query_redeem_history.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/campaign/query_redeem_history.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/campaign/update_campaign.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/campaign/update_campaign.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/catalog_changes/__init__.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/catalog_changes/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Platform Service."""
 
-__version__ = "4.47.0"
+__version__ = "4.48.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .get_statistic import GetStatistic
 from .get_statistic import (
```

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/catalog_changes/get_statistic.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/catalog_changes/get_statistic.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/catalog_changes/publish_all.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/catalog_changes/publish_all.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/catalog_changes/publish_selected.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/catalog_changes/publish_selected.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/catalog_changes/query_changes.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/catalog_changes/query_changes.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/catalog_changes/select_all_records.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/catalog_changes/select_all_records.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/catalog_changes/select_all_records_by_criteria.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/catalog_changes/select_all_records_by_criteria.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/catalog_changes/select_record.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/catalog_changes/select_record.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/catalog_changes/unselect_all_records.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/catalog_changes/unselect_all_records.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/catalog_changes/unselect_record.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/catalog_changes/unselect_record.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/category/__init__.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/category/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Platform Service."""
 
-__version__ = "4.47.0"
+__version__ = "4.48.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .create_category import CreateCategory
 from .delete_category import DeleteCategory
```

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/category/create_category.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/category/create_category.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/category/delete_category.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/category/delete_category.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/category/download_categories.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/category/download_categories.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/category/get_category.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/category/get_category.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/category/get_child_categories.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/category/get_child_categories.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/category/get_descendant_categories.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/category/get_descendant_categories.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/category/get_root_categories.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/category/get_root_categories.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/category/list_categories_basic.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/category/list_categories_basic.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/category/public_get_category.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/category/public_get_category.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/category/public_get_child_categories.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/category/public_get_child_categories.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/category/public_get_descendant_c_c5054d.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/category/public_get_descendant_c_c5054d.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/category/public_get_root_categories.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/category/public_get_root_categories.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/category/update_category.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/category/update_category.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/clawback/__init__.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/clawback/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Platform Service."""
 
-__version__ = "4.47.0"
+__version__ = "4.48.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .mock_play_station_stream_event import MockPlayStationStreamEvent
 from .query_iap_clawback_history import QueryIAPClawbackHistory
```

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/clawback/mock_play_station_stream_event.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/clawback/mock_play_station_stream_event.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/clawback/query_iap_clawback_history.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/clawback/query_iap_clawback_history.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/currency/__init__.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/currency/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Platform Service."""
 
-__version__ = "4.47.0"
+__version__ = "4.48.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .create_currency import CreateCurrency
 from .delete_currency import DeleteCurrency
```

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/currency/create_currency.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/currency/create_currency.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/currency/delete_currency.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/currency/delete_currency.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/currency/get_currency_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/currency/get_currency_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/currency/get_currency_summary.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/currency/get_currency_summary.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/currency/list_currencies.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/currency/list_currencies.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/currency/public_list_currencies.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/currency/public_list_currencies.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/currency/update_currency.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/currency/update_currency.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/dlc/__init__.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/dlc/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Platform Service."""
 
-__version__ = "4.47.0"
+__version__ = "4.48.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .delete_dlc_item_config import DeleteDLCItemConfig
 from .delete_platform_dlc_config import DeletePlatformDLCConfig
```

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/dlc/delete_dlc_item_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/dlc/delete_dlc_item_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/dlc/delete_platform_dlc_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/dlc/delete_platform_dlc_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/dlc/ge_dlc_durable_reward_s_f83f8a.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/dlc/ge_dlc_durable_reward_s_f83f8a.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/dlc/get_dlc_item_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/dlc/get_dlc_item_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/dlc/get_platform_dlc_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/dlc/get_platform_dlc_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/dlc/get_user_dlc.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/dlc/get_user_dlc.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/dlc/get_user_dlc_by_platform.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/dlc/get_user_dlc_by_platform.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/dlc/public_sync_psn_dlc_inv_429118.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/dlc/public_sync_psn_dlc_inv_429118.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/dlc/public_sync_psn_dlc_inventory.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/dlc/public_sync_psn_dlc_inventory.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/dlc/sync_epic_game_dlc.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/dlc/sync_epic_game_dlc.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/dlc/sync_oculus_dlc.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/dlc/sync_oculus_dlc.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/dlc/sync_steam_dlc.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/dlc/sync_steam_dlc.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/dlc/sync_xbox_dlc.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/dlc/sync_xbox_dlc.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/dlc/update_dlc_item_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/dlc/update_dlc_item_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/dlc/update_platform_dlc_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/dlc/update_platform_dlc_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/__init__.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Platform Service."""
 
-__version__ = "4.47.0"
+__version__ = "4.48.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .consume_user_entitlement import ConsumeUserEntitlement
 from .disable_user_entitlement import DisableUserEntitlement
@@ -93,14 +93,18 @@
 from .public_query_user_entit_2398e5 import PublicQueryUserEntitlementsByAppType
 from .public_query_user_entit_2398e5 import (
     AppTypeEnum as PublicQueryUserEntitlementsByAppTypeAppTypeEnum,
 )
 from .public_sell_user_entitlement import PublicSellUserEntitlement
 from .public_split_user_entitlement import PublicSplitUserEntitlement
 from .public_transfer_user_en_c358c0 import PublicTransferUserEntitlement
+from .public_user_entitlement_741412 import PublicUserEntitlementHistory
+from .public_user_entitlement_741412 import (
+    EntitlementClazzEnum as PublicUserEntitlementHistoryEntitlementClazzEnum,
+)
 from .query_entitlements import QueryEntitlements
 from .query_entitlements import (
     AppTypeEnum as QueryEntitlementsAppTypeEnum,
     EntitlementClazzEnum as QueryEntitlementsEntitlementClazzEnum,
     OriginEnum as QueryEntitlementsOriginEnum,
 )
 from .query_entitlements_1 import QueryEntitlements1
```

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/consume_user_entitlement.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/consume_user_entitlement.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/disable_user_entitlement.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/disable_user_entitlement.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/enable_entitlement_orig_c90935.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/enable_entitlement_orig_c90935.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/enable_user_entitlement.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/enable_user_entitlement.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/exists_any_user_active__9d3175.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/exists_any_user_active__9d3175.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/exists_any_user_active__fca16a.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/exists_any_user_active__fca16a.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/get_entitlement.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/get_entitlement.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/get_entitlement_config_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/get_entitlement_config_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/get_platform_entitlemen_32e517.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/get_platform_entitlemen_32e517.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/get_user_active_entitle_d52ca8.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/get_user_active_entitle_d52ca8.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/get_user_app_entitlemen_2375db.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/get_user_app_entitlemen_2375db.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/get_user_app_entitlemen_282639.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/get_user_app_entitlemen_282639.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/get_user_entitlement.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/get_user_entitlement.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/get_user_entitlement_by_8ab4a0.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/get_user_entitlement_by_8ab4a0.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/get_user_entitlement_by_sku.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/get_user_entitlement_by_sku.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/get_user_entitlement_histories.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/get_user_entitlement_histories.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/get_user_entitlement_ow_5a8354.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/get_user_entitlement_ow_5a8354.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/get_user_entitlement_ow_dab0ca.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/get_user_entitlement_ow_dab0ca.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/get_user_entitlement_ow_ec2b70.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/get_user_entitlement_ow_ec2b70.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/grant_entitlements.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/grant_entitlements.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,16 +34,28 @@
 from ...models import ValidationErrorEntity
 
 
 class GrantEntitlements(Operation):
     """Grant entitlements to different users (grantEntitlements)
 
     Grant entitlements to multiple users, skipped granting will be treated as fail.
-    Other detail info:
 
+    Notes:
+
+    Support Item Types:
+
+      *  APP
+      *  INGAMEITEM
+      *  CODE
+      *  SUBSCRIPTION
+      *  MEDIA
+      *  OPTIONBOX
+      *  LOOTBOX
+
+    Other detail info:
       * Required permission : resource="ADMIN:NAMESPACE:{namespace}:ENTITLEMENT", action=4 (UPDATE)
       *  Returns : bulk grant entitlements result
 
     Required Permission(s):
         - ADMIN:NAMESPACE:{namespace}:ENTITLEMENT [UPDATE]
 
     Properties:
```

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/grant_user_entitlement.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/grant_user_entitlement.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,16 +35,30 @@
 from ...models import ValidationErrorEntity
 
 
 class GrantUserEntitlement(Operation):
     """Grant user entitlement (grantUserEntitlement)
 
     Grant user entitlement.
-    Other detail info:
 
+    Notes:
+
+    will skip un-supported item if input un-supported item types, please use /admin/namespaces/{namespace}/users/{userId}/fulfillment endpoint if want to fulfill other item type, like coin item
+
+    Support Item Types:
+
+      *  APP
+      *  INGAMEITEM
+      *  CODE
+      *  SUBSCRIPTION
+      *  MEDIA
+      *  OPTIONBOX
+      *  LOOTBOX
+
+    Other detail info:
       * Required permission : resource="ADMIN:NAMESPACE:{namespace}:USER:{userId}:ENTITLEMENT", action=1 (CREATE)
       *  Returns : granted entitlement
 
     Required Permission(s):
         - ADMIN:NAMESPACE:{namespace}:USER:{userId}:ENTITLEMENT [CREATE]
 
     Properties:
```

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/pre_check_revoke_user_e_124298.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/pre_check_revoke_user_e_124298.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_consume_user_ent_7254fa.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_consume_user_ent_7254fa.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_exists_any_my_ac_dbd2a5.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_exists_any_my_ac_dbd2a5.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_exists_any_user__3977e5.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_exists_any_user__3977e5.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_get_entitlement__3fdfe7.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_get_entitlement__3fdfe7.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_get_my_app_entit_4deb3f.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_get_my_app_entit_4deb3f.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_get_my_entitleme_22c2fd.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_get_my_entitleme_22c2fd.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_get_my_entitleme_cb2911.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_get_my_entitleme_cb2911.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_get_user_app_ent_1e800f.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_get_user_app_ent_1e800f.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_get_user_app_ent_53d109.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_get_user_app_ent_53d109.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_get_user_entitle_408425.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_get_user_entitle_408425.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_get_user_entitle_815992.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_get_user_entitle_815992.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_get_user_entitle_b1671e.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_get_user_entitle_b1671e.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_get_user_entitle_b313cf.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_get_user_entitle_b313cf.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_get_user_entitle_bb9230.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_get_user_entitle_bb9230.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_get_user_entitle_ee3005.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_get_user_entitle_ee3005.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_get_user_entitlement.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_get_user_entitlement.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_query_user_entit_2398e5.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_query_user_entit_2398e5.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_query_user_entitlements.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_query_user_entitlements.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_sell_user_entitlement.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_sell_user_entitlement.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_split_user_entitlement.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_split_user_entitlement.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_transfer_user_en_c358c0.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/public_transfer_user_en_c358c0.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/query_entitlements.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/query_entitlements.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/query_entitlements_1.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/query_entitlements_1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/query_user_entitlements.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/query_user_entitlements.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/query_user_entitlements_22cea1.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/query_user_entitlements_22cea1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/revoke_all_entitlements.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/revoke_all_entitlements.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/revoke_entitlements.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/revoke_entitlements.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/revoke_use_count.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/revoke_use_count.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/revoke_user_entitlement.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/revoke_user_entitlement.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/revoke_user_entitlement_491388.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/revoke_user_entitlement_491388.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/revoke_user_entitlements.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/revoke_user_entitlements.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/sell_user_entitlement.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/sell_user_entitlement.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/update_platform_entitle_7fbd45.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/update_platform_entitle_7fbd45.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/entitlement/update_user_entitlement.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/entitlement/update_user_entitlement.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/fulfillment/__init__.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/fulfillment/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Platform Service."""
 
-__version__ = "4.47.0"
+__version__ = "4.48.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .fulfill_item import FulfillItem
 from .fulfill_rewards import FulfillRewards
```

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/fulfillment/fulfill_item.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/fulfillment/fulfill_item.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/fulfillment/fulfill_rewards.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/fulfillment/fulfill_rewards.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/fulfillment/fulfill_rewards_v2.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/fulfillment/fulfill_rewards_v2.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/fulfillment/pre_check_fulfill_item.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/fulfillment/pre_check_fulfill_item.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/fulfillment/public_redeem_code.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/fulfillment/public_redeem_code.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/fulfillment/query_fulfillment_histories.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/fulfillment/query_fulfillment_histories.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/fulfillment/redeem_code.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/fulfillment/redeem_code.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/fulfillment_script/__init__.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/fulfillment_script/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Platform Service."""
 
-__version__ = "4.47.0"
+__version__ = "4.48.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .create_fulfillment_script import CreateFulfillmentScript
 from .delete_fulfillment_script import DeleteFulfillmentScript
```

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/fulfillment_script/create_fulfillment_script.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/fulfillment_script/create_fulfillment_script.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/fulfillment_script/delete_fulfillment_script.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/fulfillment_script/delete_fulfillment_script.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/fulfillment_script/get_fulfillment_script.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/fulfillment_script/get_fulfillment_script.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/fulfillment_script/list_fulfillment_scripts.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/fulfillment_script/list_fulfillment_scripts.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/fulfillment_script/update_fulfillment_script.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/fulfillment_script/update_fulfillment_script.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/__init__.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Platform Service."""
 
-__version__ = "4.47.0"
+__version__ = "4.48.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .delete_apple_iap_config import DeleteAppleIAPConfig
 from .delete_epic_games_iap_config import DeleteEpicGamesIAPConfig
```

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/delete_apple_iap_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/delete_apple_iap_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/delete_epic_games_iap_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/delete_epic_games_iap_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/delete_google_iap_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/delete_google_iap_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/delete_iap_item_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/delete_iap_item_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/delete_oculus_iap_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/delete_oculus_iap_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/delete_playstation_iap_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/delete_playstation_iap_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/delete_steam_iap_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/delete_steam_iap_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/delete_twitch_iap_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/delete_twitch_iap_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/delete_xbl_ap_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/delete_xbl_ap_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/get_apple_iap_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/get_apple_iap_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/get_epic_games_iap_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/get_epic_games_iap_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/get_google_iap_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/get_google_iap_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/get_iap_item_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/get_iap_item_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/get_iap_item_mapping.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/get_iap_item_mapping.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/get_oculus_iap_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/get_oculus_iap_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/get_play_station_iap_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/get_play_station_iap_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/get_steam_iap_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/get_steam_iap_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/get_twitch_iap_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/get_twitch_iap_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/get_xbl_iap_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/get_xbl_iap_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/mock_fulfill_iap_item.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/mock_fulfill_iap_item.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/public_fulfill_apple_iap_item.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/public_fulfill_apple_iap_item.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/public_fulfill_google_iap_item.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/public_fulfill_google_iap_item.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/public_reconcile_play_s_6be6c0.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/public_reconcile_play_s_6be6c0.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/public_reconcile_play_s_7ac4de.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/public_reconcile_play_s_7ac4de.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/query_all_user_iap_orders.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/query_all_user_iap_orders.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/query_user_iap_consume_history.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/query_user_iap_consume_history.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/query_user_iap_orders.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/query_user_iap_orders.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/sync_epic_games_inventory.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/sync_epic_games_inventory.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/sync_oculus_consumable__f6c91d.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/sync_oculus_consumable__f6c91d.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/sync_steam_inventory.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/sync_steam_inventory.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/sync_twitch_drops_entit_0c09ca.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/sync_twitch_drops_entit_0c09ca.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/sync_twitch_drops_entitlement.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/sync_twitch_drops_entitlement.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/sync_xbox_inventory.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/sync_xbox_inventory.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/update_apple_iap_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/update_apple_iap_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/update_epic_games_iap_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/update_epic_games_iap_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/update_google_iap_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/update_google_iap_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/update_google_p12_file.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/update_google_p12_file.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/update_iap_item_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/update_iap_item_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/update_oculus_iap_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/update_oculus_iap_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/update_playstation_iap_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/update_playstation_iap_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/update_steam_iap_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/update_steam_iap_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/update_twitch_iap_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/update_twitch_iap_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/update_xbl_bp_cert_file.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/key_group/upload_keys.py`

 * *Files 13% similar despite different names*

```diff
@@ -25,63 +25,69 @@
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
-from ...models import XblIAPConfigInfo
+from ...models import BulkOperationResult
+from ...models import ErrorEntity
 
 
-class UpdateXblBPCertFile(Operation):
-    """Upload xbl business partner cert file (updateXblBPCertFile)
+class UploadKeys(Operation):
+    """Upload keys to key group (uploadKeys)
+
+    This API is used to upload keys with csv format to a key group.
 
-    Upload xbl business partner cert file.
     Other detail info:
 
-      * Required permission : resource="ADMIN:NAMESPACE:{namespace}:IAP:CONFIG", action=4 (UPDATE)
-      *  Returns : updated xbl iap config
+      * Required permission : resource="ADMIN:NAMESPACE:{namespace}:KEYGROUP", action=4 (UPDATE)
+      *  Returns : item data
 
     Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:IAP:CONFIG [UPDATE]
+        - ADMIN:NAMESPACE:{namespace}:KEYGROUP [UPDATE]
 
     Properties:
-        url: /platform/admin/namespaces/{namespace}/iap/config/xbl/cert
+        url: /platform/admin/namespaces/{namespace}/keygroups/{keyGroupId}/keys
 
-        method: PUT
+        method: POST
 
-        tags: ["IAP"]
+        tags: ["KeyGroup"]
 
         consumes: ["multipart/form-data"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH] or [BEARER_AUTH]
 
         file: (file) OPTIONAL Any in form_data
 
-        password: (password) OPTIONAL str in form_data
+        key_group_id: (keyGroupId) REQUIRED str in path
 
         namespace: (namespace) REQUIRED str in path
 
     Responses:
-        200: OK - XblIAPConfigInfo (successful operation)
+        200: OK - BulkOperationResult (successful operation)
+
+        400: Bad Request - ErrorEntity (37221: Invalid key file)
+
+        404: Not Found - ErrorEntity (37241: Key group [{keyGroupId}] does not exist in namespace [{namespace}])
     """
 
     # region fields
 
-    _url: str = "/platform/admin/namespaces/{namespace}/iap/config/xbl/cert"
-    _method: str = "PUT"
+    _url: str = "/platform/admin/namespaces/{namespace}/keygroups/{keyGroupId}/keys"
+    _method: str = "POST"
     _consumes: List[str] = ["multipart/form-data"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"], ["BEARER_AUTH"]]
     _location_query: str = None
 
     file: Any  # OPTIONAL in [form_data]
-    password: str  # OPTIONAL in [form_data]
+    key_group_id: str  # REQUIRED in [path]
     namespace: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
@@ -122,75 +128,81 @@
             "path": self.get_path_params(),
         }
 
     def get_form_data_params(self) -> dict:
         result = {}
         if hasattr(self, "file"):
             result[("file", "file")] = self.file
-        if hasattr(self, "password"):
-            result["password"] = self.password
         return result
 
     def get_path_params(self) -> dict:
         result = {}
+        if hasattr(self, "key_group_id"):
+            result["keyGroupId"] = self.key_group_id
         if hasattr(self, "namespace"):
             result["namespace"] = self.namespace
         return result
 
     # endregion get_x_params methods
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_file(self, value: Any) -> UpdateXblBPCertFile:
+    def with_file(self, value: Any) -> UploadKeys:
         self.file = value
         return self
 
-    def with_password(self, value: str) -> UpdateXblBPCertFile:
-        self.password = value
+    def with_key_group_id(self, value: str) -> UploadKeys:
+        self.key_group_id = value
         return self
 
-    def with_namespace(self, value: str) -> UpdateXblBPCertFile:
+    def with_namespace(self, value: str) -> UploadKeys:
         self.namespace = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
         if hasattr(self, "file") and self.file:
             result["file"] = Any(self.file)
         elif include_empty:
             result["file"] = Any()
-        if hasattr(self, "password") and self.password:
-            result["password"] = str(self.password)
+        if hasattr(self, "key_group_id") and self.key_group_id:
+            result["keyGroupId"] = str(self.key_group_id)
         elif include_empty:
-            result["password"] = ""
+            result["keyGroupId"] = ""
         if hasattr(self, "namespace") and self.namespace:
             result["namespace"] = str(self.namespace)
         elif include_empty:
             result["namespace"] = ""
         return result
 
     # endregion to methods
 
     # region response methods
 
     # noinspection PyMethodMayBeStatic
     def parse_response(
         self, code: int, content_type: str, content: Any
-    ) -> Tuple[Union[None, XblIAPConfigInfo], Union[None, HttpResponse]]:
+    ) -> Tuple[
+        Union[None, BulkOperationResult], Union[None, ErrorEntity, HttpResponse]
+    ]:
         """Parse the given response.
 
-        200: OK - XblIAPConfigInfo (successful operation)
+        200: OK - BulkOperationResult (successful operation)
+
+        400: Bad Request - ErrorEntity (37221: Invalid key file)
+
+        404: Not Found - ErrorEntity (37241: Key group [{keyGroupId}] does not exist in namespace [{namespace}])
 
         ---: HttpResponse (Undocumented Response)
 
         ---: HttpResponse (Unexpected Content-Type Error)
 
         ---: HttpResponse (Unhandled Error)
         """
@@ -198,71 +210,68 @@
             code=code, content_type=content_type, content=content
         )
         if error is not None:
             return None, None if error.is_no_content() else error
         code, content_type, content = pre_processed_response
 
         if code == 200:
-            return XblIAPConfigInfo.create_from_dict(content), None
+            return BulkOperationResult.create_from_dict(content), None
+        if code == 400:
+            return None, ErrorEntity.create_from_dict(content)
+        if code == 404:
+            return None, ErrorEntity.create_from_dict(content)
 
         return self.handle_undocumented_response(
             code=code, content_type=content_type, content=content
         )
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
     def create(
-        cls,
-        namespace: str,
-        file: Optional[Any] = None,
-        password: Optional[str] = None,
-        **kwargs,
-    ) -> UpdateXblBPCertFile:
+        cls, key_group_id: str, namespace: str, file: Optional[Any] = None, **kwargs
+    ) -> UploadKeys:
         instance = cls()
+        instance.key_group_id = key_group_id
         instance.namespace = namespace
         if file is not None:
             instance.file = file
-        if password is not None:
-            instance.password = password
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
-    def create_from_dict(
-        cls, dict_: dict, include_empty: bool = False
-    ) -> UpdateXblBPCertFile:
+    def create_from_dict(cls, dict_: dict, include_empty: bool = False) -> UploadKeys:
         instance = cls()
         if "file" in dict_ and dict_["file"] is not None:
             instance.file = Any(dict_["file"])
         elif include_empty:
             instance.file = Any()
-        if "password" in dict_ and dict_["password"] is not None:
-            instance.password = str(dict_["password"])
+        if "keyGroupId" in dict_ and dict_["keyGroupId"] is not None:
+            instance.key_group_id = str(dict_["keyGroupId"])
         elif include_empty:
-            instance.password = ""
+            instance.key_group_id = ""
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
         elif include_empty:
             instance.namespace = ""
         return instance
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
             "file": "file",
-            "password": "password",
+            "keyGroupId": "key_group_id",
             "namespace": "namespace",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
             "file": False,
-            "password": False,
+            "keyGroupId": True,
             "namespace": True,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/update_xbl_iap_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/update_xbl_iap_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/validate_existed_playst_881975.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/validate_existed_playst_881975.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/iap/validate_playstation_ia_7dc74e.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/iap/validate_playstation_ia_7dc74e.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/invoice/__init__.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/invoice/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Platform Service."""
 
-__version__ = "4.47.0"
+__version__ = "4.48.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .download_invoice_details import DownloadInvoiceDetails
 from .download_invoice_details import (
```

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/invoice/download_invoice_details.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/invoice/download_invoice_details.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/invoice/generate_invoice_summary.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/invoice/generate_invoice_summary.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/__init__.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Platform Service."""
 
-__version__ = "4.47.0"
+__version__ = "4.48.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .acquire_item import AcquireItem
 from .bulk_get_locale_items import BulkGetLocaleItems
```

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/acquire_item.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/acquire_item.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/bulk_get_locale_items.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/bulk_get_locale_items.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/bulk_update_region_data.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/bulk_update_region_data.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/create_item.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/create_item.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/create_item_type_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/create_item_type_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/defeature_item.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/defeature_item.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/delete_item.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/delete_item.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/delete_item_type_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/delete_item_type_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/disable_item.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/disable_item.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/enable_item.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/enable_item.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/feature_item.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/feature_item.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/get_app.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/get_app.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/get_available_predicate_types.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/get_available_predicate_types.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/get_bulk_item_id_by_skus.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/get_bulk_item_id_by_skus.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/get_estimated_price.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/get_estimated_price.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/get_item.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/get_item.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/get_item_by_app_id.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/get_item_by_app_id.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/get_item_by_sku.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/get_item_by_sku.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/get_item_dynamic_data.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/get_item_dynamic_data.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/get_item_id_by_sku.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/get_item_id_by_sku.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/get_item_type_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/get_item_type_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/get_items.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/get_items.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/get_locale_item.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/get_locale_item.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/get_locale_item_by_sku.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/get_locale_item_by_sku.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/list_basic_items_by_features.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/list_basic_items_by_features.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/list_item_type_configs.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/list_item_type_configs.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/public_bulk_get_items.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/public_bulk_get_items.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/public_get_app.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/public_get_app.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/public_get_estimated_price.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/public_get_estimated_price.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/public_get_item.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/public_get_item.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/public_get_item_by_app_id.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/public_get_item_by_app_id.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/public_get_item_by_sku.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/public_get_item_by_sku.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/public_get_item_dynamic_data.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/public_get_item_dynamic_data.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/public_query_items.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/public_query_items.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/public_search_items.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/public_search_items.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/public_validate_item_pu_bd546e.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/public_validate_item_pu_bd546e.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/query_items.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/query_items.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/query_items_1.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/query_items_1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/query_uncategorized_items.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/query_uncategorized_items.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/return_item.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/return_item.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/search_item_type_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/search_item_type_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/search_items.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/search_items.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/sync_in_game_item.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/sync_in_game_item.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/update_app.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/update_app.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/update_item.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/update_item.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/update_item_purchase_condition.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/update_item_purchase_condition.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/update_item_type_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/update_item_type_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/item/validate_item_purchase__929f78.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/item/validate_item_purchase__929f78.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/key_group/__init__.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/key_group/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Platform Service."""
 
-__version__ = "4.47.0"
+__version__ = "4.48.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .create_key_group import CreateKeyGroup
 from .get_key_group import GetKeyGroup
```

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/key_group/create_key_group.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/key_group/create_key_group.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/key_group/get_key_group.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/key_group/get_key_group.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/key_group/get_key_group_by_booth_name.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/key_group/get_key_group_by_booth_name.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/key_group/get_key_group_dynamic.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/key_group/get_key_group_dynamic.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/key_group/list_keys.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/key_group/list_keys.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/key_group/query_key_groups.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/key_group/query_key_groups.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/key_group/update_key_group.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/key_group/update_key_group.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/key_group/upload_keys.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/wallet/disable_user_wallet.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,71 +24,69 @@
 
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
+from accelbyte_py_sdk.core import deprecated
 
-from ...models import BulkOperationResult
 from ...models import ErrorEntity
 
 
-class UploadKeys(Operation):
-    """Upload keys to key group (uploadKeys)
-
-    This API is used to upload keys with csv format to a key group.
+class DisableUserWallet(Operation):
+    """Disable a user wallet (disableUserWallet)
 
+    disable a user wallet.
     Other detail info:
 
-      * Required permission : resource="ADMIN:NAMESPACE:{namespace}:KEYGROUP", action=4 (UPDATE)
-      *  Returns : item data
+      * Required permission : resource="ADMIN:NAMESPACE:{namespace}:USER:{userId}:WALLET", action=4 (UPDATE)
 
     Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:KEYGROUP [UPDATE]
+        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:WALLET [UPDATE]
 
     Properties:
-        url: /platform/admin/namespaces/{namespace}/keygroups/{keyGroupId}/keys
+        url: /platform/admin/namespaces/{namespace}/users/{userId}/wallets/{walletId}/disable
 
-        method: POST
+        method: PUT
 
-        tags: ["KeyGroup"]
+        tags: ["Wallet"]
 
-        consumes: ["multipart/form-data"]
+        consumes: ["application/json"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH] or [BEARER_AUTH]
 
-        file: (file) OPTIONAL Any in form_data
+        namespace: (namespace) REQUIRED str in path
 
-        key_group_id: (keyGroupId) REQUIRED str in path
+        user_id: (userId) REQUIRED str in path
 
-        namespace: (namespace) REQUIRED str in path
+        wallet_id: (walletId) REQUIRED str in path
 
     Responses:
-        200: OK - BulkOperationResult (successful operation)
+        204: No Content - (Successful operation)
 
-        400: Bad Request - ErrorEntity (37221: Invalid key file)
+        404: Not Found - ErrorEntity (35141: Wallet [{walletId}] does not exist)
 
-        404: Not Found - ErrorEntity (37241: Key group [{keyGroupId}] does not exist in namespace [{namespace}])
+        409: Conflict - ErrorEntity (20006: optimistic lock)
     """
 
     # region fields
 
-    _url: str = "/platform/admin/namespaces/{namespace}/keygroups/{keyGroupId}/keys"
-    _method: str = "POST"
-    _consumes: List[str] = ["multipart/form-data"]
+    _url: str = "/platform/admin/namespaces/{namespace}/users/{userId}/wallets/{walletId}/disable"
+    _method: str = "PUT"
+    _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"], ["BEARER_AUTH"]]
     _location_query: str = None
 
-    file: Any  # OPTIONAL in [form_data]
-    key_group_id: str  # REQUIRED in [path]
     namespace: str  # REQUIRED in [path]
+    user_id: str  # REQUIRED in [path]
+    wallet_id: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
@@ -120,158 +118,152 @@
 
     # endregion get methods
 
     # region get_x_params methods
 
     def get_all_params(self) -> dict:
         return {
-            "form_data": self.get_form_data_params(),
             "path": self.get_path_params(),
         }
 
-    def get_form_data_params(self) -> dict:
-        result = {}
-        if hasattr(self, "file"):
-            result[("file", "file")] = self.file
-        return result
-
     def get_path_params(self) -> dict:
         result = {}
-        if hasattr(self, "key_group_id"):
-            result["keyGroupId"] = self.key_group_id
         if hasattr(self, "namespace"):
             result["namespace"] = self.namespace
+        if hasattr(self, "user_id"):
+            result["userId"] = self.user_id
+        if hasattr(self, "wallet_id"):
+            result["walletId"] = self.wallet_id
         return result
 
     # endregion get_x_params methods
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_file(self, value: Any) -> UploadKeys:
-        self.file = value
+    def with_namespace(self, value: str) -> DisableUserWallet:
+        self.namespace = value
         return self
 
-    def with_key_group_id(self, value: str) -> UploadKeys:
-        self.key_group_id = value
+    def with_user_id(self, value: str) -> DisableUserWallet:
+        self.user_id = value
         return self
 
-    def with_namespace(self, value: str) -> UploadKeys:
-        self.namespace = value
+    def with_wallet_id(self, value: str) -> DisableUserWallet:
+        self.wallet_id = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
-        if hasattr(self, "file") and self.file:
-            result["file"] = Any(self.file)
-        elif include_empty:
-            result["file"] = Any()
-        if hasattr(self, "key_group_id") and self.key_group_id:
-            result["keyGroupId"] = str(self.key_group_id)
-        elif include_empty:
-            result["keyGroupId"] = ""
         if hasattr(self, "namespace") and self.namespace:
             result["namespace"] = str(self.namespace)
         elif include_empty:
             result["namespace"] = ""
+        if hasattr(self, "user_id") and self.user_id:
+            result["userId"] = str(self.user_id)
+        elif include_empty:
+            result["userId"] = ""
+        if hasattr(self, "wallet_id") and self.wallet_id:
+            result["walletId"] = str(self.wallet_id)
+        elif include_empty:
+            result["walletId"] = ""
         return result
 
     # endregion to methods
 
     # region response methods
 
     # noinspection PyMethodMayBeStatic
     def parse_response(
         self, code: int, content_type: str, content: Any
-    ) -> Tuple[
-        Union[None, BulkOperationResult], Union[None, ErrorEntity, HttpResponse]
-    ]:
+    ) -> Tuple[None, Union[None, ErrorEntity, HttpResponse]]:
         """Parse the given response.
 
-        200: OK - BulkOperationResult (successful operation)
+        204: No Content - (Successful operation)
 
-        400: Bad Request - ErrorEntity (37221: Invalid key file)
+        404: Not Found - ErrorEntity (35141: Wallet [{walletId}] does not exist)
 
-        404: Not Found - ErrorEntity (37241: Key group [{keyGroupId}] does not exist in namespace [{namespace}])
+        409: Conflict - ErrorEntity (20006: optimistic lock)
 
         ---: HttpResponse (Undocumented Response)
 
         ---: HttpResponse (Unexpected Content-Type Error)
 
         ---: HttpResponse (Unhandled Error)
         """
         pre_processed_response, error = self.pre_process_response(
             code=code, content_type=content_type, content=content
         )
         if error is not None:
             return None, None if error.is_no_content() else error
         code, content_type, content = pre_processed_response
 
-        if code == 200:
-            return BulkOperationResult.create_from_dict(content), None
-        if code == 400:
-            return None, ErrorEntity.create_from_dict(content)
+        if code == 204:
+            return None, None
         if code == 404:
             return None, ErrorEntity.create_from_dict(content)
+        if code == 409:
+            return None, ErrorEntity.create_from_dict(content)
 
         return self.handle_undocumented_response(
             code=code, content_type=content_type, content=content
         )
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
     def create(
-        cls, key_group_id: str, namespace: str, file: Optional[Any] = None, **kwargs
-    ) -> UploadKeys:
+        cls, namespace: str, user_id: str, wallet_id: str, **kwargs
+    ) -> DisableUserWallet:
         instance = cls()
-        instance.key_group_id = key_group_id
         instance.namespace = namespace
-        if file is not None:
-            instance.file = file
+        instance.user_id = user_id
+        instance.wallet_id = wallet_id
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
-    def create_from_dict(cls, dict_: dict, include_empty: bool = False) -> UploadKeys:
+    def create_from_dict(
+        cls, dict_: dict, include_empty: bool = False
+    ) -> DisableUserWallet:
         instance = cls()
-        if "file" in dict_ and dict_["file"] is not None:
-            instance.file = Any(dict_["file"])
-        elif include_empty:
-            instance.file = Any()
-        if "keyGroupId" in dict_ and dict_["keyGroupId"] is not None:
-            instance.key_group_id = str(dict_["keyGroupId"])
-        elif include_empty:
-            instance.key_group_id = ""
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
         elif include_empty:
             instance.namespace = ""
+        if "userId" in dict_ and dict_["userId"] is not None:
+            instance.user_id = str(dict_["userId"])
+        elif include_empty:
+            instance.user_id = ""
+        if "walletId" in dict_ and dict_["walletId"] is not None:
+            instance.wallet_id = str(dict_["walletId"])
+        elif include_empty:
+            instance.wallet_id = ""
         return instance
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
-            "file": "file",
-            "keyGroupId": "key_group_id",
             "namespace": "namespace",
+            "userId": "user_id",
+            "walletId": "wallet_id",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
-            "file": False,
-            "keyGroupId": True,
             "namespace": True,
+            "userId": True,
+            "walletId": True,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/order/__init__.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/order/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Platform Service."""
 
-__version__ = "4.47.0"
+__version__ = "4.48.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .admin_create_user_order import AdminCreateUserOrder
 from .count_of_purchased_item import CountOfPurchasedItem
```

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/order/admin_create_user_order.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/order/admin_create_user_order.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/order/count_of_purchased_item.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/order/count_of_purchased_item.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/order/download_user_order_receipt.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/order/download_user_order_receipt.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/order/fulfill_user_order.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/order/fulfill_user_order.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/order/get_order.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/order/get_order.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/order/get_order_statistics.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/order/get_order_statistics.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/order/get_user_order.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/order/get_user_order.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/order/get_user_order_grant.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/order/get_user_order_grant.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/order/get_user_order_histories.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/order/get_user_order_histories.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/order/process_user_order_noti_fdd9f8.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/order/process_user_order_noti_fdd9f8.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/order/public_cancel_user_order.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/order/public_cancel_user_order.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/order/public_create_user_order.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/order/public_create_user_order.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/order/public_download_user_or_6ea3e8.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/order/public_download_user_or_6ea3e8.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/order/public_get_user_order.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/order/public_get_user_order.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/order/public_get_user_order_h_063753.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/order/public_get_user_order_h_063753.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/order/public_query_user_orders.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/order/public_query_user_orders.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/order/query_orders.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/order/query_orders.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/order/query_user_orders.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/order/query_user_orders.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/order/refund_order.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/order/refund_order.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/order/update_user_order_status.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/order/update_user_order_status.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/order_dedicated/sync_orders.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/order_dedicated/sync_orders.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment/__init__.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Platform Service."""
 
-__version__ = "4.47.0"
+__version__ = "4.48.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .charge_payment_order import ChargePaymentOrder
 from .create_user_payment_order import CreateUserPaymentOrder
```

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment/charge_payment_order.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment/charge_payment_order.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment/create_user_payment_order.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment/create_user_payment_order.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment/get_payment_order.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment/get_payment_order.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment/get_payment_order_charg_9acbf8.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment/get_payment_order_charg_9acbf8.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment/list_ext_order_no_by_ext_tx_id.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment/list_ext_order_no_by_ext_tx_id.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment/query_payment_notifications.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment/query_payment_notifications.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment/query_payment_orders.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment/query_payment_orders.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment/refund_user_payment_order.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment/refund_user_payment_order.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment/simulate_payment_order__cf0fbc.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment/simulate_payment_order__cf0fbc.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_account/__init__.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_account/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Platform Service."""
 
-__version__ = "4.47.0"
+__version__ = "4.48.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .public_delete_payment_account import PublicDeletePaymentAccount
 from .public_delete_payment_account import (
```

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_account/public_delete_payment_account.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_account/public_delete_payment_account.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_account/public_get_payment_accounts.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_account/public_get_payment_accounts.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_callback_config/__init__.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_callback_config/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Platform Service."""
 
-__version__ = "4.47.0"
+__version__ = "4.48.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .get_payment_callback_config import GetPaymentCallbackConfig
 from .update_payment_callback_config import UpdatePaymentCallbackConfig
```

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_callback_config/get_payment_callback_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_callback_config/get_payment_callback_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_callback_config/update_payment_callback_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_callback_config/update_payment_callback_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_config/__init__.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_config/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Platform Service."""
 
-__version__ = "4.47.0"
+__version__ = "4.48.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .create_payment_provider_config import CreatePaymentProviderConfig
 from .debug_matched_payment_m_9bf142 import DebugMatchedPaymentMerchantConfig
```

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_config/create_payment_provider_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_config/create_payment_provider_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_config/debug_matched_payment_m_9bf142.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_config/debug_matched_payment_m_9bf142.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_config/debug_matched_payment_p_02dcf1.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_config/debug_matched_payment_p_02dcf1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_config/delete_payment_provider_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_config/delete_payment_provider_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_config/get_aggregate_payment_p_41c63c.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_config/get_aggregate_payment_p_41c63c.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_config/get_payment_merchant_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_config/get_payment_merchant_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_config/get_payment_tax_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_config/get_payment_tax_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_config/get_special_payment_providers.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_config/get_special_payment_providers.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_config/query_payment_provider_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_config/query_payment_provider_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_config/test_adyen_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_config/test_adyen_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_config/test_adyen_config_by_id.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_config/test_adyen_config_by_id.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_config/test_ali_pay_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_config/test_ali_pay_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_config/test_ali_pay_config_by_id.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_config/test_ali_pay_config_by_id.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_config/test_checkout_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_config/test_checkout_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_config/test_checkout_config_by_id.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_config/test_checkout_config_by_id.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_config/test_pay_pal_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_config/test_pay_pal_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_config/test_pay_pal_config_by_id.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_config/test_pay_pal_config_by_id.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_config/test_stripe_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_config/test_stripe_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_config/test_stripe_config_by_id.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_config/test_stripe_config_by_id.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_config/test_wx_pay_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_config/test_wx_pay_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_config/test_wx_pay_config_by_id.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_config/test_wx_pay_config_by_id.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_config/test_xsolla_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_config/test_xsolla_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_config/test_xsolla_config_by_id.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_config/test_xsolla_config_by_id.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_config/update_adyen_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_config/update_adyen_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_config/update_ali_pay_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_config/update_ali_pay_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_config/update_checkout_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_config/update_checkout_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_config/update_pay_pal_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_config/update_pay_pal_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_config/update_payment_provider_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_config/update_payment_provider_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_config/update_payment_tax_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_config/update_payment_tax_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_config/update_stripe_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_config/update_stripe_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_config/update_wx_pay_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_config/update_wx_pay_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_config/update_wx_pay_config_cert.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_config/update_wx_pay_config_cert.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_config/update_xsolla_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_config/update_xsolla_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_config/update_xsolla_ui_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_config/update_xsolla_ui_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_dedicated/__init__.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_dedicated/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Platform Service."""
 
-__version__ = "4.47.0"
+__version__ = "4.48.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .create_payment_order_by_79f85c import CreatePaymentOrderByDedicated
 from .refund_payment_order_by_309df5 import RefundPaymentOrderByDedicated
```

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_dedicated/create_payment_order_by_79f85c.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_dedicated/create_payment_order_by_79f85c.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_dedicated/refund_payment_order_by_309df5.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_dedicated/refund_payment_order_by_309df5.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_dedicated/sync_payment_orders.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_dedicated/sync_payment_orders.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_station/__init__.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_station/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Platform Service."""
 
-__version__ = "4.47.0"
+__version__ = "4.48.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .get_payment_customization import GetPaymentCustomization
 from .get_payment_customization import (
```

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_station/get_payment_customization.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_station/get_payment_customization.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_station/get_payment_public_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_station/get_payment_public_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_station/get_payment_tax_value.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_station/get_payment_tax_value.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_station/pay.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_station/pay.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_station/public_check_payment_or_dec069.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_station/public_check_payment_or_dec069.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_station/public_get_payment_methods.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_station/public_get_payment_methods.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_station/public_get_payment_url.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_station/public_get_payment_url.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_station/public_get_qr_code.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_station/public_get_qr_code.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_station/public_get_unpaid_payme_26d8dd.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_station/public_get_unpaid_payme_26d8dd.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/payment_station/public_normalize_paymen_6657a5.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/payment_station/public_normalize_paymen_6657a5.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/revocation/__init__.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/revocation/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Platform Service."""
 
-__version__ = "4.47.0"
+__version__ = "4.48.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .delete_revocation_config import DeleteRevocationConfig
 from .do_revocation import DoRevocation
```

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/revocation/delete_revocation_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/revocation/delete_revocation_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/revocation/do_revocation.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/revocation/do_revocation.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/revocation/get_revocation_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/revocation/get_revocation_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/revocation/query_revocation_histories.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/revocation/query_revocation_histories.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/revocation/update_revocation_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/revocation/update_revocation_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/reward/__init__.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/reward/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Platform Service."""
 
-__version__ = "4.47.0"
+__version__ = "4.48.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .check_event_condition import CheckEventCondition
 from .create_reward import CreateReward
```

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/reward/check_event_condition.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/reward/check_event_condition.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/reward/create_reward.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/reward/create_reward.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/reward/delete_reward.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/reward/delete_reward.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/reward/delete_reward_condition_record.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/reward/delete_reward_condition_record.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/reward/export_rewards.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/reward/export_rewards.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/reward/get_reward.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/reward/get_reward.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/reward/get_reward_1.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/reward/get_reward_1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/reward/get_reward_by_code.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/reward/get_reward_by_code.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/reward/import_rewards.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/reward/import_rewards.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/reward/query_rewards.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/reward/query_rewards.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/reward/query_rewards_1.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/reward/query_rewards_1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/reward/update_reward.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/reward/update_reward.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/section/__init__.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/section/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Platform Service."""
 
-__version__ = "4.47.0"
+__version__ = "4.48.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .create_section import CreateSection
 from .delete_section import DeleteSection
```

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/section/create_section.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/section/create_section.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/section/delete_section.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/section/delete_section.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/section/get_section.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/section/get_section.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/section/public_list_active_sections.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/section/public_list_active_sections.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/section/purge_expired_section.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/section/purge_expired_section.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/section/query_sections.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/section/query_sections.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/section/update_section.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/section/update_section.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/service_plugin_config/__init__.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/service_plugin_config/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Platform Service."""
 
-__version__ = "4.47.0"
+__version__ = "4.48.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .delete_loot_box_plugin_config import DeleteLootBoxPluginConfig
 from .delete_revocation_plugi_c2651d import DeleteRevocationPluginConfig
```

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/service_plugin_config/delete_loot_box_plugin_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/service_plugin_config/delete_loot_box_plugin_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/service_plugin_config/delete_revocation_plugi_c2651d.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/service_plugin_config/delete_revocation_plugi_c2651d.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/service_plugin_config/delete_section_plugin_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/service_plugin_config/delete_section_plugin_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/service_plugin_config/delete_service_plugin_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/service_plugin_config/delete_service_plugin_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/service_plugin_config/get_loot_box_grpc_info.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/service_plugin_config/get_loot_box_grpc_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/service_plugin_config/get_loot_box_plugin_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/service_plugin_config/get_loot_box_plugin_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/service_plugin_config/get_revocation_plugin_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/service_plugin_config/get_revocation_plugin_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/service_plugin_config/get_section_plugin_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/service_plugin_config/get_section_plugin_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/service_plugin_config/get_service_plugin_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/service_plugin_config/get_service_plugin_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/service_plugin_config/update_loot_box_plugin_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/service_plugin_config/update_loot_box_plugin_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/service_plugin_config/update_revocation_plugi_c19001.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/service_plugin_config/update_revocation_plugi_c19001.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/service_plugin_config/update_section_plugin_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/service_plugin_config/update_section_plugin_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/service_plugin_config/update_service_plugin_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/service_plugin_config/update_service_plugin_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/service_plugin_config/upload_revocation_plugi_6c586a.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/service_plugin_config/upload_revocation_plugi_6c586a.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/service_plugin_config/upload_section_plugin_c_780cdd.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/service_plugin_config/upload_section_plugin_c_780cdd.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/service_plugin_config/uplod_loot_box_plugin_c_5c5812.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/service_plugin_config/uplod_loot_box_plugin_c_5c5812.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/session_platform/__init__.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/session_platform/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,14 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Platform Service."""
 
-__version__ = "4.47.0"
+__version__ = "4.48.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .register_xbl_sessions import RegisterXblSessions
```

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/session_platform/register_xbl_sessions.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/session_platform/register_xbl_sessions.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/store/__init__.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/store/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Platform Service."""
 
-__version__ = "4.47.0"
+__version__ = "4.48.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .clone_store import CloneStore
 from .create_store import CreateStore
```

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/store/clone_store.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/store/clone_store.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/store/create_store.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/store/create_store.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/store/delete_published_store.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/store/delete_published_store.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/store/delete_store.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/store/delete_store.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/store/download_csv_templates.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/store/download_csv_templates.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/store/export_store.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/store/export_store.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/store/export_store_1.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/store/export_store_1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/store/export_store_by_csv.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/store/export_store_by_csv.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/store/get_catalog_definition.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/store/get_catalog_definition.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/store/get_published_store.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/store/get_published_store.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/store/get_published_store_backup.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/store/get_published_store_backup.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/store/get_store.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/store/get_store.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/store/import_store.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/store/import_store.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/store/import_store_1.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/store/import_store_1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/store/import_store_by_csv.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/store/import_store_by_csv.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/store/list_stores.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/store/list_stores.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/store/public_list_stores.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/store/public_list_stores.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/store/query_import_history.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/store/query_import_history.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/store/rollback_published_store.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/store/rollback_published_store.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/store/update_store.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/store/update_store.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/subscription/__init__.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/subscription/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Platform Service."""
 
-__version__ = "4.47.0"
+__version__ = "4.48.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .cancel_subscription import CancelSubscription
 from .check_user_subscription_6c59a6 import CheckUserSubscriptionSubscribableByItemId
```

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/subscription/cancel_subscription.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/subscription/cancel_subscription.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/subscription/check_user_subscription_6c59a6.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/subscription/check_user_subscription_6c59a6.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/subscription/delete_user_subscription.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/subscription/delete_user_subscription.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/subscription/get_user_subscription.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/subscription/get_user_subscription.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/subscription/get_user_subscription_a_b2b8e9.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/subscription/get_user_subscription_a_b2b8e9.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/subscription/get_user_subscription_b_a3096e.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/subscription/get_user_subscription_b_a3096e.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/subscription/grant_days_to_subscription.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/subscription/grant_days_to_subscription.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/subscription/platform_subscribe_subs_ad4f3b.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/subscription/platform_subscribe_subs_ad4f3b.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/subscription/process_user_subscripti_d07750.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/subscription/process_user_subscripti_d07750.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/subscription/public_cancel_subscription.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/subscription/public_cancel_subscription.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/subscription/public_change_subscript_350ff2.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/subscription/public_change_subscript_350ff2.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/subscription/public_check_user_subsc_16fdcb.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/subscription/public_check_user_subsc_16fdcb.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/subscription/public_get_user_subscri_c8d5b3.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/subscription/public_get_user_subscri_c8d5b3.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/subscription/public_get_user_subscription.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/subscription/public_get_user_subscription.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/subscription/public_query_user_subsc_29ae74.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/subscription/public_query_user_subsc_29ae74.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/subscription/public_subscribe_subscription.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/subscription/public_subscribe_subscription.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/subscription/query_subscriptions.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/subscription/query_subscriptions.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/subscription/query_user_subscriptions.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/subscription/query_user_subscriptions.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/subscription/recurring_charge_subscription.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/subscription/recurring_charge_subscription.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/ticket/__init__.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/ticket/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Platform Service."""
 
-__version__ = "4.47.0"
+__version__ = "4.48.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .acquire_user_ticket import AcquireUserTicket
 from .decrease_ticket_sale import DecreaseTicketSale
```

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/ticket/acquire_user_ticket.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/ticket/acquire_user_ticket.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/ticket/decrease_ticket_sale.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/ticket/decrease_ticket_sale.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/ticket/get_ticket_booth_id.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/ticket/get_ticket_booth_id.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/ticket/get_ticket_dynamic.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/ticket/get_ticket_dynamic.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/ticket/increase_ticket_sale.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/ticket/increase_ticket_sale.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/trade_action/__init__.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/trade_action/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Platform Service."""
 
-__version__ = "4.47.0"
+__version__ = "4.48.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .commit import Commit
 from .get_trade_history_by_criteria import GetTradeHistoryByCriteria
```

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/trade_action/commit.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/trade_action/commit.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/trade_action/get_trade_history_by_criteria.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/trade_action/get_trade_history_by_criteria.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/trade_action/get_trade_history_by_tr_8b774c.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/trade_action/get_trade_history_by_tr_8b774c.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/view/__init__.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/view/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Platform Service."""
 
-__version__ = "4.47.0"
+__version__ = "4.48.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .create_view import CreateView
 from .delete_view import DeleteView
```

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/view/create_view.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/view/create_view.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/view/delete_view.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/view/delete_view.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/view/get_view.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/view/get_view.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/view/list_views.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/view/list_views.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/view/public_list_views.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/view/public_list_views.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/view/update_view.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/view/update_view.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/wallet/__init__.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/wallet/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Platform Service."""
 
-__version__ = "4.47.0"
+__version__ = "4.48.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .bulk_credit import BulkCredit
 from .bulk_debit import BulkDebit
```

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/wallet/bulk_credit.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/wallet/bulk_credit.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/wallet/bulk_debit.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/wallet/bulk_debit.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/wallet/check_balance.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/wallet/check_balance.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/wallet/check_wallet.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/wallet/check_wallet.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/wallet/credit_user_wallet.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/wallet/credit_user_wallet.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/wallet/debit_by_wallet_platform.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/wallet/debit_by_wallet_platform.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/wallet/debit_user_wallet.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/wallet/debit_user_wallet.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/wallet/debit_user_wallet_by_cu_54daab.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/wallet/debit_user_wallet_by_cu_54daab.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/wallet/disable_user_wallet.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/wallet/enable_user_wallet.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,27 +29,27 @@
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 from accelbyte_py_sdk.core import deprecated
 
 from ...models import ErrorEntity
 
 
-class DisableUserWallet(Operation):
-    """Disable a user wallet (disableUserWallet)
+class EnableUserWallet(Operation):
+    """Enable a user wallet (enableUserWallet)
 
-    disable a user wallet.
+    enable a user wallet.
     Other detail info:
 
       * Required permission : resource="ADMIN:NAMESPACE:{namespace}:USER:{userId}:WALLET", action=4 (UPDATE)
 
     Required Permission(s):
         - ADMIN:NAMESPACE:{namespace}:USER:{userId}:WALLET [UPDATE]
 
     Properties:
-        url: /platform/admin/namespaces/{namespace}/users/{userId}/wallets/{walletId}/disable
+        url: /platform/admin/namespaces/{namespace}/users/{userId}/wallets/{walletId}/enable
 
         method: PUT
 
         tags: ["Wallet"]
 
         consumes: ["application/json"]
 
@@ -69,15 +69,15 @@
         404: Not Found - ErrorEntity (35141: Wallet [{walletId}] does not exist)
 
         409: Conflict - ErrorEntity (20006: optimistic lock)
     """
 
     # region fields
 
-    _url: str = "/platform/admin/namespaces/{namespace}/users/{userId}/wallets/{walletId}/disable"
+    _url: str = "/platform/admin/namespaces/{namespace}/users/{userId}/wallets/{walletId}/enable"
     _method: str = "PUT"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"], ["BEARER_AUTH"]]
     _location_query: str = None
 
     namespace: str  # REQUIRED in [path]
@@ -139,23 +139,23 @@
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_namespace(self, value: str) -> DisableUserWallet:
+    def with_namespace(self, value: str) -> EnableUserWallet:
         self.namespace = value
         return self
 
-    def with_user_id(self, value: str) -> DisableUserWallet:
+    def with_user_id(self, value: str) -> EnableUserWallet:
         self.user_id = value
         return self
 
-    def with_wallet_id(self, value: str) -> DisableUserWallet:
+    def with_wallet_id(self, value: str) -> EnableUserWallet:
         self.wallet_id = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
@@ -218,27 +218,27 @@
     # endregion response methods
 
     # region static methods
 
     @classmethod
     def create(
         cls, namespace: str, user_id: str, wallet_id: str, **kwargs
-    ) -> DisableUserWallet:
+    ) -> EnableUserWallet:
         instance = cls()
         instance.namespace = namespace
         instance.user_id = user_id
         instance.wallet_id = wallet_id
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> DisableUserWallet:
+    ) -> EnableUserWallet:
         instance = cls()
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
         elif include_empty:
             instance.namespace = ""
         if "userId" in dict_ and dict_["userId"] is not None:
             instance.user_id = str(dict_["userId"])
```

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/wallet/enable_user_wallet.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/wallet/get_user_wallet.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,31 +27,33 @@
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 from accelbyte_py_sdk.core import deprecated
 
 from ...models import ErrorEntity
+from ...models import WalletInfo
 
 
-class EnableUserWallet(Operation):
-    """Enable a user wallet (enableUserWallet)
+class GetUserWallet(Operation):
+    """Get a user wallet (getUserWallet)
 
-    enable a user wallet.
+    get a user wallet.
     Other detail info:
 
-      * Required permission : resource="ADMIN:NAMESPACE:{namespace}:USER:{userId}:WALLET", action=4 (UPDATE)
+      * Required permission : resource="ADMIN:NAMESPACE:{namespace}:USER:{userId}:WALLET", action=2 (READ)
+      *  Returns : wallet info
 
     Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:WALLET [UPDATE]
+        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:WALLET [READ]
 
     Properties:
-        url: /platform/admin/namespaces/{namespace}/users/{userId}/wallets/{walletId}/enable
+        url: /platform/admin/namespaces/{namespace}/users/{userId}/wallets/{walletId}
 
-        method: PUT
+        method: GET
 
         tags: ["Wallet"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
@@ -60,25 +62,25 @@
         namespace: (namespace) REQUIRED str in path
 
         user_id: (userId) REQUIRED str in path
 
         wallet_id: (walletId) REQUIRED str in path
 
     Responses:
-        204: No Content - (Successful operation)
+        200: OK - WalletInfo (successful operation)
 
         404: Not Found - ErrorEntity (35141: Wallet [{walletId}] does not exist)
-
-        409: Conflict - ErrorEntity (20006: optimistic lock)
     """
 
     # region fields
 
-    _url: str = "/platform/admin/namespaces/{namespace}/users/{userId}/wallets/{walletId}/enable"
-    _method: str = "PUT"
+    _url: str = (
+        "/platform/admin/namespaces/{namespace}/users/{userId}/wallets/{walletId}"
+    )
+    _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"], ["BEARER_AUTH"]]
     _location_query: str = None
 
     namespace: str  # REQUIRED in [path]
     user_id: str  # REQUIRED in [path]
@@ -139,23 +141,23 @@
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_namespace(self, value: str) -> EnableUserWallet:
+    def with_namespace(self, value: str) -> GetUserWallet:
         self.namespace = value
         return self
 
-    def with_user_id(self, value: str) -> EnableUserWallet:
+    def with_user_id(self, value: str) -> GetUserWallet:
         self.user_id = value
         return self
 
-    def with_wallet_id(self, value: str) -> EnableUserWallet:
+    def with_wallet_id(self, value: str) -> GetUserWallet:
         self.wallet_id = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
@@ -178,67 +180,63 @@
     # endregion to methods
 
     # region response methods
 
     # noinspection PyMethodMayBeStatic
     def parse_response(
         self, code: int, content_type: str, content: Any
-    ) -> Tuple[None, Union[None, ErrorEntity, HttpResponse]]:
+    ) -> Tuple[Union[None, WalletInfo], Union[None, ErrorEntity, HttpResponse]]:
         """Parse the given response.
 
-        204: No Content - (Successful operation)
+        200: OK - WalletInfo (successful operation)
 
         404: Not Found - ErrorEntity (35141: Wallet [{walletId}] does not exist)
 
-        409: Conflict - ErrorEntity (20006: optimistic lock)
-
         ---: HttpResponse (Undocumented Response)
 
         ---: HttpResponse (Unexpected Content-Type Error)
 
         ---: HttpResponse (Unhandled Error)
         """
         pre_processed_response, error = self.pre_process_response(
             code=code, content_type=content_type, content=content
         )
         if error is not None:
             return None, None if error.is_no_content() else error
         code, content_type, content = pre_processed_response
 
-        if code == 204:
-            return None, None
+        if code == 200:
+            return WalletInfo.create_from_dict(content), None
         if code == 404:
             return None, ErrorEntity.create_from_dict(content)
-        if code == 409:
-            return None, ErrorEntity.create_from_dict(content)
 
         return self.handle_undocumented_response(
             code=code, content_type=content_type, content=content
         )
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
     def create(
         cls, namespace: str, user_id: str, wallet_id: str, **kwargs
-    ) -> EnableUserWallet:
+    ) -> GetUserWallet:
         instance = cls()
         instance.namespace = namespace
         instance.user_id = user_id
         instance.wallet_id = wallet_id
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> EnableUserWallet:
+    ) -> GetUserWallet:
         instance = cls()
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
         elif include_empty:
             instance.namespace = ""
         if "userId" in dict_ and dict_["userId"] is not None:
             instance.user_id = str(dict_["userId"])
```

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/wallet/get_platform_wallet_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/wallet/get_platform_wallet_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/wallet/get_user_wallet.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/wallet/get_wallet.py`

 * *Files 12% similar despite different names*

```diff
@@ -30,64 +30,59 @@
 from accelbyte_py_sdk.core import HttpResponse
 from accelbyte_py_sdk.core import deprecated
 
 from ...models import ErrorEntity
 from ...models import WalletInfo
 
 
-class GetUserWallet(Operation):
-    """Get a user wallet (getUserWallet)
+class GetWallet(Operation):
+    """Get a wallet by wallet id (getWallet)
 
-    get a user wallet.
+    get a wallet by wallet id.
     Other detail info:
 
-      * Required permission : resource="ADMIN:NAMESPACE:{namespace}:USER:{userId}:WALLET", action=2 (READ)
+      * Required permission : resource="ADMIN:NAMESPACE:{namespace}:WALLET", action=2 (READ)
       *  Returns : wallet info
 
     Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:WALLET [READ]
+        - ADMIN:NAMESPACE:{namespace}:WALLET [READ]
 
     Properties:
-        url: /platform/admin/namespaces/{namespace}/users/{userId}/wallets/{walletId}
+        url: /platform/admin/namespaces/{namespace}/wallets/{walletId}
 
         method: GET
 
         tags: ["Wallet"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH] or [BEARER_AUTH]
 
         namespace: (namespace) REQUIRED str in path
 
-        user_id: (userId) REQUIRED str in path
-
         wallet_id: (walletId) REQUIRED str in path
 
     Responses:
         200: OK - WalletInfo (successful operation)
 
         404: Not Found - ErrorEntity (35141: Wallet [{walletId}] does not exist)
     """
 
     # region fields
 
-    _url: str = (
-        "/platform/admin/namespaces/{namespace}/users/{userId}/wallets/{walletId}"
-    )
+    _url: str = "/platform/admin/namespaces/{namespace}/wallets/{walletId}"
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"], ["BEARER_AUTH"]]
     _location_query: str = None
 
     namespace: str  # REQUIRED in [path]
-    user_id: str  # REQUIRED in [path]
     wallet_id: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
@@ -127,54 +122,44 @@
             "path": self.get_path_params(),
         }
 
     def get_path_params(self) -> dict:
         result = {}
         if hasattr(self, "namespace"):
             result["namespace"] = self.namespace
-        if hasattr(self, "user_id"):
-            result["userId"] = self.user_id
         if hasattr(self, "wallet_id"):
             result["walletId"] = self.wallet_id
         return result
 
     # endregion get_x_params methods
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_namespace(self, value: str) -> GetUserWallet:
+    def with_namespace(self, value: str) -> GetWallet:
         self.namespace = value
         return self
 
-    def with_user_id(self, value: str) -> GetUserWallet:
-        self.user_id = value
-        return self
-
-    def with_wallet_id(self, value: str) -> GetUserWallet:
+    def with_wallet_id(self, value: str) -> GetWallet:
         self.wallet_id = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
         if hasattr(self, "namespace") and self.namespace:
             result["namespace"] = str(self.namespace)
         elif include_empty:
             result["namespace"] = ""
-        if hasattr(self, "user_id") and self.user_id:
-            result["userId"] = str(self.user_id)
-        elif include_empty:
-            result["userId"] = ""
         if hasattr(self, "wallet_id") and self.wallet_id:
             result["walletId"] = str(self.wallet_id)
         elif include_empty:
             result["walletId"] = ""
         return result
 
     # endregion to methods
@@ -214,54 +199,43 @@
         )
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
-    def create(
-        cls, namespace: str, user_id: str, wallet_id: str, **kwargs
-    ) -> GetUserWallet:
+    def create(cls, namespace: str, wallet_id: str, **kwargs) -> GetWallet:
         instance = cls()
         instance.namespace = namespace
-        instance.user_id = user_id
         instance.wallet_id = wallet_id
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
-    def create_from_dict(
-        cls, dict_: dict, include_empty: bool = False
-    ) -> GetUserWallet:
+    def create_from_dict(cls, dict_: dict, include_empty: bool = False) -> GetWallet:
         instance = cls()
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
         elif include_empty:
             instance.namespace = ""
-        if "userId" in dict_ and dict_["userId"] is not None:
-            instance.user_id = str(dict_["userId"])
-        elif include_empty:
-            instance.user_id = ""
         if "walletId" in dict_ and dict_["walletId"] is not None:
             instance.wallet_id = str(dict_["walletId"])
         elif include_empty:
             instance.wallet_id = ""
         return instance
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
             "namespace": "namespace",
-            "userId": "user_id",
             "walletId": "wallet_id",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
             "namespace": True,
-            "userId": True,
             "walletId": True,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/wallet/get_wallet.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/wallet/query_user_currency_wallets.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,66 +24,62 @@
 
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
-from accelbyte_py_sdk.core import deprecated
 
-from ...models import ErrorEntity
-from ...models import WalletInfo
+from ...models import CurrencyWallet
 
 
-class GetWallet(Operation):
-    """Get a wallet by wallet id (getWallet)
+class QueryUserCurrencyWallets(Operation):
+    """Get user currency wallet summary (queryUserCurrencyWallets)
 
-    get a wallet by wallet id.
+    Get user currency wallet summary.
     Other detail info:
 
-      * Required permission : resource="ADMIN:NAMESPACE:{namespace}:WALLET", action=2 (READ)
-      *  Returns : wallet info
+      * Required permission : resource="ADMIN:NAMESPACE:{namespace}:USER:{userId}:WALLET", action=2 (READ)
+      *  Returns : currency wallet summary
 
     Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:WALLET [READ]
+        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:WALLET [READ]
 
     Properties:
-        url: /platform/admin/namespaces/{namespace}/wallets/{walletId}
+        url: /platform/admin/namespaces/{namespace}/users/{userId}/wallets/currencies/summary
 
         method: GET
 
         tags: ["Wallet"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH] or [BEARER_AUTH]
 
         namespace: (namespace) REQUIRED str in path
 
-        wallet_id: (walletId) REQUIRED str in path
+        user_id: (userId) REQUIRED str in path
 
     Responses:
-        200: OK - WalletInfo (successful operation)
-
-        404: Not Found - ErrorEntity (35141: Wallet [{walletId}] does not exist)
+        200: OK - List[CurrencyWallet] (successful operation)
     """
 
     # region fields
 
-    _url: str = "/platform/admin/namespaces/{namespace}/wallets/{walletId}"
+    _url: str = "/platform/admin/namespaces/{namespace}/users/{userId}/wallets/currencies/summary"
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"], ["BEARER_AUTH"]]
     _location_query: str = None
 
     namespace: str  # REQUIRED in [path]
-    wallet_id: str  # REQUIRED in [path]
+    user_id: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
@@ -122,63 +118,61 @@
             "path": self.get_path_params(),
         }
 
     def get_path_params(self) -> dict:
         result = {}
         if hasattr(self, "namespace"):
             result["namespace"] = self.namespace
-        if hasattr(self, "wallet_id"):
-            result["walletId"] = self.wallet_id
+        if hasattr(self, "user_id"):
+            result["userId"] = self.user_id
         return result
 
     # endregion get_x_params methods
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_namespace(self, value: str) -> GetWallet:
+    def with_namespace(self, value: str) -> QueryUserCurrencyWallets:
         self.namespace = value
         return self
 
-    def with_wallet_id(self, value: str) -> GetWallet:
-        self.wallet_id = value
+    def with_user_id(self, value: str) -> QueryUserCurrencyWallets:
+        self.user_id = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
         if hasattr(self, "namespace") and self.namespace:
             result["namespace"] = str(self.namespace)
         elif include_empty:
             result["namespace"] = ""
-        if hasattr(self, "wallet_id") and self.wallet_id:
-            result["walletId"] = str(self.wallet_id)
+        if hasattr(self, "user_id") and self.user_id:
+            result["userId"] = str(self.user_id)
         elif include_empty:
-            result["walletId"] = ""
+            result["userId"] = ""
         return result
 
     # endregion to methods
 
     # region response methods
 
     # noinspection PyMethodMayBeStatic
     def parse_response(
         self, code: int, content_type: str, content: Any
-    ) -> Tuple[Union[None, WalletInfo], Union[None, ErrorEntity, HttpResponse]]:
+    ) -> Tuple[Union[None, List[CurrencyWallet]], Union[None, HttpResponse]]:
         """Parse the given response.
 
-        200: OK - WalletInfo (successful operation)
-
-        404: Not Found - ErrorEntity (35141: Wallet [{walletId}] does not exist)
+        200: OK - List[CurrencyWallet] (successful operation)
 
         ---: HttpResponse (Undocumented Response)
 
         ---: HttpResponse (Unexpected Content-Type Error)
 
         ---: HttpResponse (Unhandled Error)
         """
@@ -186,56 +180,56 @@
             code=code, content_type=content_type, content=content
         )
         if error is not None:
             return None, None if error.is_no_content() else error
         code, content_type, content = pre_processed_response
 
         if code == 200:
-            return WalletInfo.create_from_dict(content), None
-        if code == 404:
-            return None, ErrorEntity.create_from_dict(content)
+            return [CurrencyWallet.create_from_dict(i) for i in content], None
 
         return self.handle_undocumented_response(
             code=code, content_type=content_type, content=content
         )
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
-    def create(cls, namespace: str, wallet_id: str, **kwargs) -> GetWallet:
+    def create(cls, namespace: str, user_id: str, **kwargs) -> QueryUserCurrencyWallets:
         instance = cls()
         instance.namespace = namespace
-        instance.wallet_id = wallet_id
+        instance.user_id = user_id
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
-    def create_from_dict(cls, dict_: dict, include_empty: bool = False) -> GetWallet:
+    def create_from_dict(
+        cls, dict_: dict, include_empty: bool = False
+    ) -> QueryUserCurrencyWallets:
         instance = cls()
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
         elif include_empty:
             instance.namespace = ""
-        if "walletId" in dict_ and dict_["walletId"] is not None:
-            instance.wallet_id = str(dict_["walletId"])
+        if "userId" in dict_ and dict_["userId"] is not None:
+            instance.user_id = str(dict_["userId"])
         elif include_empty:
-            instance.wallet_id = ""
+            instance.user_id = ""
         return instance
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
             "namespace": "namespace",
-            "walletId": "wallet_id",
+            "userId": "user_id",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
             "namespace": True,
-            "walletId": True,
+            "userId": True,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/wallet/list_user_currency_tran_bb67cf.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/wallet/list_user_currency_tran_bb67cf.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/wallet/list_user_wallet_transactions.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/wallet/list_user_wallet_transactions.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/wallet/pay_with_user_wallet.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/wallet/pay_with_user_wallet.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/wallet/public_get_my_wallet.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/wallet/public_get_my_wallet.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/wallet/public_get_wallet.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/wallet/public_get_wallet.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/wallet/public_list_user_wallet_ed4de4.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/wallet/public_list_user_wallet_ed4de4.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/wallet/query_wallets.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/wallet/query_wallets.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/wallet/reset_platform_wallet_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/wallet/reset_platform_wallet_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/operations/wallet/update_platform_wallet_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/operations/wallet/update_platform_wallet_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/wrappers/__init__.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/wrappers/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: wrapper-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Platform Service."""
 
-__version__ = "4.47.0"
+__version__ = "4.48.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from ._achievement_platform import get_xbl_user_achievements
 from ._achievement_platform import get_xbl_user_achievements_async
@@ -250,14 +250,16 @@
 from ._entitlement import public_query_user_entitlements_by_app_type_async
 from ._entitlement import public_sell_user_entitlement
 from ._entitlement import public_sell_user_entitlement_async
 from ._entitlement import public_split_user_entitlement
 from ._entitlement import public_split_user_entitlement_async
 from ._entitlement import public_transfer_user_entitlement
 from ._entitlement import public_transfer_user_entitlement_async
+from ._entitlement import public_user_entitlement_history
+from ._entitlement import public_user_entitlement_history_async
 from ._entitlement import query_entitlements
 from ._entitlement import query_entitlements_async
 from ._entitlement import query_entitlements_1
 from ._entitlement import query_entitlements_1_async
 from ._entitlement import query_user_entitlements
 from ._entitlement import query_user_entitlements_async
 from ._entitlement import query_user_entitlements_by_app_type
```

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/wrappers/_achievement_platform.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/wrappers/_achievement_platform.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/wrappers/_anonymization.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/wrappers/_anonymization.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/wrappers/_campaign.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/wrappers/_campaign.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/wrappers/_catalog_changes.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/wrappers/_catalog_changes.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/wrappers/_category.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/wrappers/_category.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/wrappers/_clawback.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/wrappers/_clawback.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/wrappers/_currency.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/wrappers/_currency.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/wrappers/_dlc.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/wrappers/_dlc.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/wrappers/_entitlement.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/wrappers/_entitlement.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,14 +59,15 @@
 from ..models import EntitlementUpdate
 from ..models import ErrorEntity
 from ..models import Ownership
 from ..models import OwnershipToken
 from ..models import RevokeUseCountRequest
 from ..models import StackableEntitlementInfo
 from ..models import TimedOwnership
+from ..models import UserEntitlementHistoryPagingSlicedResult
 from ..models import ValidationErrorEntity
 
 from ..operations.entitlement import ConsumeUserEntitlement
 from ..operations.entitlement import DisableUserEntitlement
 from ..operations.entitlement import EnableEntitlementOriginFeature
 from ..operations.entitlement import EnableUserEntitlement
 from ..operations.entitlement import ExistsAnyUserActiveEntitlement
@@ -144,14 +145,18 @@
 from ..operations.entitlement import PublicQueryUserEntitlementsByAppType
 from ..operations.entitlement import (
     PublicQueryUserEntitlementsByAppTypeAppTypeEnum,
 )
 from ..operations.entitlement import PublicSellUserEntitlement
 from ..operations.entitlement import PublicSplitUserEntitlement
 from ..operations.entitlement import PublicTransferUserEntitlement
+from ..operations.entitlement import PublicUserEntitlementHistory
+from ..operations.entitlement import (
+    PublicUserEntitlementHistoryEntitlementClazzEnum,
+)
 from ..operations.entitlement import QueryEntitlements
 from ..operations.entitlement import (
     QueryEntitlementsAppTypeEnum,
     QueryEntitlementsEntitlementClazzEnum,
     QueryEntitlementsOriginEnum,
 )
 from ..operations.entitlement import QueryEntitlements1
@@ -189,15 +194,19 @@
     EntitlementDecrementResultClazzEnum,
     EntitlementDecrementResultOriginEnum,
     EntitlementDecrementResultSourceEnum,
     EntitlementDecrementResultStatusEnum,
     EntitlementDecrementResultTypeEnum,
 )
 from ..models import EntitlementGrantOriginEnum, EntitlementGrantSourceEnum
-from ..models import EntitlementHistoryInfoActionEnum, EntitlementHistoryInfoOriginEnum
+from ..models import (
+    EntitlementHistoryInfoActionEnum,
+    EntitlementHistoryInfoClazzEnum,
+    EntitlementHistoryInfoOriginEnum,
+)
 from ..models import (
     EntitlementIfcAppTypeEnum,
     EntitlementIfcClazzEnum,
     EntitlementIfcOriginEnum,
     EntitlementIfcStatusEnum,
     EntitlementIfcTypeEnum,
 )
@@ -2455,16 +2464,28 @@
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Grant entitlements to different users (grantEntitlements)
 
     Grant entitlements to multiple users, skipped granting will be treated as fail.
-    Other detail info:
 
+    Notes:
+
+    Support Item Types:
+
+      *  APP
+      *  INGAMEITEM
+      *  CODE
+      *  SUBSCRIPTION
+      *  MEDIA
+      *  OPTIONBOX
+      *  LOOTBOX
+
+    Other detail info:
       * Required permission : resource="ADMIN:NAMESPACE:{namespace}:ENTITLEMENT", action=4 (UPDATE)
       *  Returns : bulk grant entitlements result
 
     Required Permission(s):
         - ADMIN:NAMESPACE:{namespace}:ENTITLEMENT [UPDATE]
 
     Properties:
@@ -2506,16 +2527,28 @@
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Grant entitlements to different users (grantEntitlements)
 
     Grant entitlements to multiple users, skipped granting will be treated as fail.
-    Other detail info:
 
+    Notes:
+
+    Support Item Types:
+
+      *  APP
+      *  INGAMEITEM
+      *  CODE
+      *  SUBSCRIPTION
+      *  MEDIA
+      *  OPTIONBOX
+      *  LOOTBOX
+
+    Other detail info:
       * Required permission : resource="ADMIN:NAMESPACE:{namespace}:ENTITLEMENT", action=4 (UPDATE)
       *  Returns : bulk grant entitlements result
 
     Required Permission(s):
         - ADMIN:NAMESPACE:{namespace}:ENTITLEMENT [UPDATE]
 
     Properties:
@@ -2560,16 +2593,30 @@
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Grant user entitlement (grantUserEntitlement)
 
     Grant user entitlement.
-    Other detail info:
 
+    Notes:
+
+    will skip un-supported item if input un-supported item types, please use /admin/namespaces/{namespace}/users/{userId}/fulfillment endpoint if want to fulfill other item type, like coin item
+
+    Support Item Types:
+
+      *  APP
+      *  INGAMEITEM
+      *  CODE
+      *  SUBSCRIPTION
+      *  MEDIA
+      *  OPTIONBOX
+      *  LOOTBOX
+
+    Other detail info:
       * Required permission : resource="ADMIN:NAMESPACE:{namespace}:USER:{userId}:ENTITLEMENT", action=1 (CREATE)
       *  Returns : granted entitlement
 
     Required Permission(s):
         - ADMIN:NAMESPACE:{namespace}:USER:{userId}:ENTITLEMENT [CREATE]
 
     Properties:
@@ -2617,16 +2664,30 @@
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Grant user entitlement (grantUserEntitlement)
 
     Grant user entitlement.
-    Other detail info:
 
+    Notes:
+
+    will skip un-supported item if input un-supported item types, please use /admin/namespaces/{namespace}/users/{userId}/fulfillment endpoint if want to fulfill other item type, like coin item
+
+    Support Item Types:
+
+      *  APP
+      *  INGAMEITEM
+      *  CODE
+      *  SUBSCRIPTION
+      *  MEDIA
+      *  OPTIONBOX
+      *  LOOTBOX
+
+    Other detail info:
       * Required permission : resource="ADMIN:NAMESPACE:{namespace}:USER:{userId}:ENTITLEMENT", action=1 (CREATE)
       *  Returns : granted entitlement
 
     Required Permission(s):
         - ADMIN:NAMESPACE:{namespace}:USER:{userId}:ENTITLEMENT [CREATE]
 
     Properties:
@@ -5457,14 +5518,160 @@
         namespace=namespace,
     )
     return await run_request_async(
         request, additional_headers=x_additional_headers, **kwargs
     )
 
 
+@same_doc_as(PublicUserEntitlementHistory)
+def public_user_entitlement_history(
+    user_id: str,
+    end_date: Optional[str] = None,
+    entitlement_clazz: Optional[
+        Union[str, PublicUserEntitlementHistoryEntitlementClazzEnum]
+    ] = None,
+    limit: Optional[int] = None,
+    offset: Optional[int] = None,
+    start_date: Optional[str] = None,
+    namespace: Optional[str] = None,
+    x_additional_headers: Optional[Dict[str, str]] = None,
+    **kwargs
+):
+    """Get user entitlements histories. (publicUserEntitlementHistory)
+
+    Get user entitlement history
+
+    Other detail info:
+
+      * Required permission : resource="NAMESPACE:{namespace}:USER:{userId}:ENTITLEMENT", action=2 (READ)
+      *  Returns : user entitlement history list
+
+    Required Permission(s):
+        - NAMESPACE:{namespace}:USER:{userId}:ENTITLEMENT [READ]
+
+    Properties:
+        url: /platform/public/namespaces/{namespace}/users/{userId}/entitlements/history
+
+        method: GET
+
+        tags: ["Entitlement"]
+
+        consumes: []
+
+        produces: ["application/json"]
+
+        securities: [BEARER_AUTH] or [BEARER_AUTH]
+
+        namespace: (namespace) REQUIRED str in path
+
+        user_id: (userId) REQUIRED str in path
+
+        end_date: (endDate) OPTIONAL str in query
+
+        entitlement_clazz: (entitlementClazz) OPTIONAL Union[str, EntitlementClazzEnum] in query
+
+        limit: (limit) OPTIONAL int in query
+
+        offset: (offset) OPTIONAL int in query
+
+        start_date: (startDate) OPTIONAL str in query
+
+    Responses:
+        200: OK - List[UserEntitlementHistoryPagingSlicedResult] (successful operation)
+    """
+    if namespace is None:
+        namespace, error = get_services_namespace()
+        if error:
+            return None, error
+    request = PublicUserEntitlementHistory.create(
+        user_id=user_id,
+        end_date=end_date,
+        entitlement_clazz=entitlement_clazz,
+        limit=limit,
+        offset=offset,
+        start_date=start_date,
+        namespace=namespace,
+    )
+    return run_request(request, additional_headers=x_additional_headers, **kwargs)
+
+
+@same_doc_as(PublicUserEntitlementHistory)
+async def public_user_entitlement_history_async(
+    user_id: str,
+    end_date: Optional[str] = None,
+    entitlement_clazz: Optional[
+        Union[str, PublicUserEntitlementHistoryEntitlementClazzEnum]
+    ] = None,
+    limit: Optional[int] = None,
+    offset: Optional[int] = None,
+    start_date: Optional[str] = None,
+    namespace: Optional[str] = None,
+    x_additional_headers: Optional[Dict[str, str]] = None,
+    **kwargs
+):
+    """Get user entitlements histories. (publicUserEntitlementHistory)
+
+    Get user entitlement history
+
+    Other detail info:
+
+      * Required permission : resource="NAMESPACE:{namespace}:USER:{userId}:ENTITLEMENT", action=2 (READ)
+      *  Returns : user entitlement history list
+
+    Required Permission(s):
+        - NAMESPACE:{namespace}:USER:{userId}:ENTITLEMENT [READ]
+
+    Properties:
+        url: /platform/public/namespaces/{namespace}/users/{userId}/entitlements/history
+
+        method: GET
+
+        tags: ["Entitlement"]
+
+        consumes: []
+
+        produces: ["application/json"]
+
+        securities: [BEARER_AUTH] or [BEARER_AUTH]
+
+        namespace: (namespace) REQUIRED str in path
+
+        user_id: (userId) REQUIRED str in path
+
+        end_date: (endDate) OPTIONAL str in query
+
+        entitlement_clazz: (entitlementClazz) OPTIONAL Union[str, EntitlementClazzEnum] in query
+
+        limit: (limit) OPTIONAL int in query
+
+        offset: (offset) OPTIONAL int in query
+
+        start_date: (startDate) OPTIONAL str in query
+
+    Responses:
+        200: OK - List[UserEntitlementHistoryPagingSlicedResult] (successful operation)
+    """
+    if namespace is None:
+        namespace, error = get_services_namespace()
+        if error:
+            return None, error
+    request = PublicUserEntitlementHistory.create(
+        user_id=user_id,
+        end_date=end_date,
+        entitlement_clazz=entitlement_clazz,
+        limit=limit,
+        offset=offset,
+        start_date=start_date,
+        namespace=namespace,
+    )
+    return await run_request_async(
+        request, additional_headers=x_additional_headers, **kwargs
+    )
+
+
 @same_doc_as(QueryEntitlements)
 def query_entitlements(
     active_only: Optional[bool] = None,
     app_type: Optional[Union[str, QueryEntitlementsAppTypeEnum]] = None,
     entitlement_clazz: Optional[
         Union[str, QueryEntitlementsEntitlementClazzEnum]
     ] = None,
```

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/wrappers/_fulfillment.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/wrappers/_fulfillment.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/wrappers/_fulfillment_script.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/wrappers/_fulfillment_script.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/wrappers/_iap.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/wrappers/_iap.py`

 * *Files 0% similar despite different names*

```diff
@@ -4454,14 +4454,16 @@
 
         password: (password) OPTIONAL str in form_data
 
         namespace: (namespace) REQUIRED str in path
 
     Responses:
         200: OK - XblIAPConfigInfo (successful operation)
+
+        400: Bad Request - ErrorEntity (39221: Invalid Xbox Business Partner Certificate or password: [{message}])
     """
     if namespace is None:
         namespace, error = get_services_namespace()
         if error:
             return None, error
     request = UpdateXblBPCertFile.create(
         file=file,
@@ -4507,14 +4509,16 @@
 
         password: (password) OPTIONAL str in form_data
 
         namespace: (namespace) REQUIRED str in path
 
     Responses:
         200: OK - XblIAPConfigInfo (successful operation)
+
+        400: Bad Request - ErrorEntity (39221: Invalid Xbox Business Partner Certificate or password: [{message}])
     """
     if namespace is None:
         namespace, error = get_services_namespace()
         if error:
             return None, error
     request = UpdateXblBPCertFile.create(
         file=file,
```

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/wrappers/_invoice.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/wrappers/_invoice.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/wrappers/_item.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/wrappers/_item.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/wrappers/_key_group.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/wrappers/_key_group.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/wrappers/_order.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/wrappers/_order.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/wrappers/_order_dedicated.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/wrappers/_order_dedicated.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/wrappers/_payment.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/wrappers/_payment.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/wrappers/_payment_account.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/wrappers/_payment_account.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/wrappers/_payment_callback_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/wrappers/_payment_callback_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/wrappers/_payment_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/wrappers/_payment_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/wrappers/_payment_dedicated.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/wrappers/_payment_dedicated.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/wrappers/_payment_station.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/wrappers/_payment_station.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/wrappers/_revocation.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/wrappers/_revocation.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/wrappers/_reward.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/wrappers/_reward.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/wrappers/_section.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/wrappers/_section.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/wrappers/_service_plugin_config.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/wrappers/_service_plugin_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/wrappers/_session_platform.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/wrappers/_session_platform.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/wrappers/_store.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/wrappers/_store.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/wrappers/_subscription.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/wrappers/_subscription.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/wrappers/_ticket.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/wrappers/_ticket.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/wrappers/_trade_action.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/wrappers/_trade_action.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/wrappers/_view.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/wrappers/_view.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk/api/platform/wrappers/_wallet.py` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk/api/platform/wrappers/_wallet.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk_service_platform.egg-info/PKG-INFO` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk_service_platform.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: accelbyte-py-sdk-service-platform
-Version: 0.8.0
+Version: 0.9.0
 Summary: AccelByte Python SDK - AccelByte Gaming Services Platform Service
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: accelbyte-py-sdk-core
 
 [//]: # (Code generated. DO NOT EDIT!)
 
 # AccelByte Modular Python SDK - Service Module
 
 This is a service module for the [AccelByte Modular Python SDK](https://github.com/AccelByte/accelbyte-python-modular-sdk) package.
 
 ```text
 AccelByte Gaming Services Platform Service
-* Version: 4.47.0
+* Version: 4.48.0
 ```
 
 ## Setup
 
 This SDK requires Python 3.9 to be installed.
 
 ### Install with Pip
```

### Comparing `accelbyte-py-sdk-service-platform-0.8.0/accelbyte_py_sdk_service_platform.egg-info/SOURCES.txt` & `accelbyte-py-sdk-service-platform-0.9.0/accelbyte_py_sdk_service_platform.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -289,14 +289,15 @@
 accelbyte_py_sdk/api/platform/models/play_station_reconcile_result.py
 accelbyte_py_sdk/api/platform/models/playstation_iap_config_request.py
 accelbyte_py_sdk/api/platform/models/populated_item_info.py
 accelbyte_py_sdk/api/platform/models/pre_check_fulfillment_request.py
 accelbyte_py_sdk/api/platform/models/predicate.py
 accelbyte_py_sdk/api/platform/models/predicate_validate_result.py
 accelbyte_py_sdk/api/platform/models/public_custom_config_info.py
+accelbyte_py_sdk/api/platform/models/public_entitlement_history_info.py
 accelbyte_py_sdk/api/platform/models/purchase_condition.py
 accelbyte_py_sdk/api/platform/models/purchase_condition_update.py
 accelbyte_py_sdk/api/platform/models/purchased_item_count.py
 accelbyte_py_sdk/api/platform/models/recurring.py
 accelbyte_py_sdk/api/platform/models/recurring_charge_result.py
 accelbyte_py_sdk/api/platform/models/redeem_history_info.py
 accelbyte_py_sdk/api/platform/models/redeem_history_paging_sliced_result.py
@@ -387,14 +388,15 @@
 accelbyte_py_sdk/api/platform/models/transaction_amount_details.py
 accelbyte_py_sdk/api/platform/models/twitch_iap_config_info.py
 accelbyte_py_sdk/api/platform/models/twitch_iap_config_request.py
 accelbyte_py_sdk/api/platform/models/twitch_sync_request.py
 accelbyte_py_sdk/api/platform/models/twitch_sync_result.py
 accelbyte_py_sdk/api/platform/models/user_dlc.py
 accelbyte_py_sdk/api/platform/models/user_dlc_record.py
+accelbyte_py_sdk/api/platform/models/user_entitlement_history_paging_sliced_result.py
 accelbyte_py_sdk/api/platform/models/validation_error_entity.py
 accelbyte_py_sdk/api/platform/models/view_create.py
 accelbyte_py_sdk/api/platform/models/view_info.py
 accelbyte_py_sdk/api/platform/models/view_update.py
 accelbyte_py_sdk/api/platform/models/wallet_info.py
 accelbyte_py_sdk/api/platform/models/wallet_paging_sliced_result.py
 accelbyte_py_sdk/api/platform/models/wallet_revocation_config.py
@@ -536,14 +538,15 @@
 accelbyte_py_sdk/api/platform/operations/entitlement/public_get_user_entitle_ee3005.py
 accelbyte_py_sdk/api/platform/operations/entitlement/public_get_user_entitlement.py
 accelbyte_py_sdk/api/platform/operations/entitlement/public_query_user_entit_2398e5.py
 accelbyte_py_sdk/api/platform/operations/entitlement/public_query_user_entitlements.py
 accelbyte_py_sdk/api/platform/operations/entitlement/public_sell_user_entitlement.py
 accelbyte_py_sdk/api/platform/operations/entitlement/public_split_user_entitlement.py
 accelbyte_py_sdk/api/platform/operations/entitlement/public_transfer_user_en_c358c0.py
+accelbyte_py_sdk/api/platform/operations/entitlement/public_user_entitlement_741412.py
 accelbyte_py_sdk/api/platform/operations/entitlement/query_entitlements.py
 accelbyte_py_sdk/api/platform/operations/entitlement/query_entitlements_1.py
 accelbyte_py_sdk/api/platform/operations/entitlement/query_user_entitlements.py
 accelbyte_py_sdk/api/platform/operations/entitlement/query_user_entitlements_22cea1.py
 accelbyte_py_sdk/api/platform/operations/entitlement/revoke_all_entitlements.py
 accelbyte_py_sdk/api/platform/operations/entitlement/revoke_entitlements.py
 accelbyte_py_sdk/api/platform/operations/entitlement/revoke_use_count.py
```

