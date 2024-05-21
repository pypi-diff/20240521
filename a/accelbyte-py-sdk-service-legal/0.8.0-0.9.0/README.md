# Comparing `tmp/accelbyte-py-sdk-service-legal-0.8.0.tar.gz` & `tmp/accelbyte_py_sdk_service_legal-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accelbyte-py-sdk-service-legal-0.8.0.tar", last modified: Tue Mar 26 05:43:05 2024, max compression
+gzip compressed data, was "accelbyte_py_sdk_service_legal-0.9.0.tar", last modified: Tue May  7 06:28:40 2024, max compression
```

## Comparing `accelbyte-py-sdk-service-legal-0.8.0.tar` & `accelbyte_py_sdk_service_legal-0.9.0.tar`

### file list

```diff
@@ -1,176 +1,181 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:43:05.510181 accelbyte-py-sdk-service-legal-0.8.0/
--rw-r--r--   0 root         (0) root         (0)     1117 2024-03-26 05:43:05.510181 accelbyte-py-sdk-service-legal-0.8.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      869 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:43:05.494181 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:43:05.494181 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:43:05.494181 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/
--rw-rw-r--   0 root         (0) root         (0)     7715 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:43:05.498181 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/
--rw-rw-r--   0 root         (0) root         (0)     3740 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7736 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/accept_agreement_request.py
--rw-rw-r--   0 root         (0) root         (0)     4426 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/accept_agreement_response.py
--rw-rw-r--   0 root         (0) root         (0)     8899 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/create_base_policy_request.py
--rw-rw-r--   0 root         (0) root         (0)     8200 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/create_base_policy_request_v2.py
--rw-rw-r--   0 root         (0) root         (0)    11723 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/create_base_policy_response.py
--rw-rw-r--   0 root         (0) root         (0)     5674 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/create_localized_policy_version_request.py
--rw-rw-r--   0 root         (0) root         (0)     6963 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/create_localized_policy_version_response.py
--rw-rw-r--   0 root         (0) root         (0)     5652 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/create_policy_version_request.py
--rw-rw-r--   0 root         (0) root         (0)     8539 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/create_policy_version_response.py
--rw-rw-r--   0 root         (0) root         (0)     6319 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/error_entity.py
--rw-rw-r--   0 root         (0) root         (0)     7297 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/field_validation_error.py
--rw-rw-r--   0 root         (0) root         (0)     3943 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/legal_readiness_status_response.py
--rw-rw-r--   0 root         (0) root         (0)    13110 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/localized_policy_version_object.py
--rw-rw-r--   0 root         (0) root         (0)     5427 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/paged_retrieve_user_accepted_agreement_response.py
--rw-rw-r--   0 root         (0) root         (0)     4263 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/paging.py
--rw-rw-r--   0 root         (0) root         (0)    12243 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/policy_object.py
--rw-rw-r--   0 root         (0) root         (0)     9665 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/policy_version_object.py
--rw-rw-r--   0 root         (0) root         (0)    11681 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/policy_version_with_localized_version_object.py
--rw-rw-r--   0 root         (0) root         (0)    15327 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/retrieve_accepted_agreement_response.py
--rw-rw-r--   0 root         (0) root         (0)    11928 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/retrieve_base_policy_response.py
--rw-rw-r--   0 root         (0) root         (0)    16204 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/retrieve_localized_policy_version_public_response.py
--rw-rw-r--   0 root         (0) root         (0)    13771 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/retrieve_localized_policy_version_response.py
--rw-rw-r--   0 root         (0) root         (0)    17681 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/retrieve_policy_public_response.py
--rw-rw-r--   0 root         (0) root         (0)    13724 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/retrieve_policy_response.py
--rw-rw-r--   0 root         (0) root         (0)     7661 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/retrieve_policy_type_response.py
--rw-rw-r--   0 root         (0) root         (0)    13008 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/retrieve_policy_version_response.py
--rw-rw-r--   0 root         (0) root         (0)    14642 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/retrieve_user_accepted_agreement_response.py
--rw-rw-r--   0 root         (0) root         (0)     4052 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/retrieve_user_eligibilities_indirect_response.py
--rw-rw-r--   0 root         (0) root         (0)    12987 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/retrieve_user_eligibilities_response.py
--rw-rw-r--   0 root         (0) root         (0)     4767 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/retrieve_user_info_cache_status_response.py
--rw-rw-r--   0 root         (0) root         (0)     8217 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/update_base_policy_request.py
--rw-rw-r--   0 root         (0) root         (0)     7516 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/update_base_policy_request_v2.py
--rw-rw-r--   0 root         (0) root         (0)    11723 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/update_base_policy_response.py
--rw-rw-r--   0 root         (0) root         (0)     8074 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/update_localized_policy_version_request.py
--rw-rw-r--   0 root         (0) root         (0)    10944 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/update_localized_policy_version_response.py
--rw-rw-r--   0 root         (0) root         (0)     7888 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/update_policy_request.py
--rw-rw-r--   0 root         (0) root         (0)     5440 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/update_policy_version_request.py
--rw-rw-r--   0 root         (0) root         (0)    10045 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/update_policy_version_response.py
--rw-rw-r--   0 root         (0) root         (0)     6369 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/upload_localized_policy_version_attachment_response.py
--rw-rw-r--   0 root         (0) root         (0)     4900 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/upload_policy_version_attachment_request.py
--rw-rw-r--   0 root         (0) root         (0)     5141 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/user_agreements_response.py
--rw-rw-r--   0 root         (0) root         (0)     4945 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/users_agreements_request.py
--rw-rw-r--   0 root         (0) root         (0)     5625 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/validation_error_entity.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:43:05.498181 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/
--rw-rw-r--   0 root         (0) root         (0)      434 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:43:05.502181 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/admin_user_agreement/
--rw-rw-r--   0 root         (0) root         (0)      545 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/admin_user_agreement/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    10894 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/admin_user_agreement/indirect_bulk_accept_ve_9d5446.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:43:05.502181 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/admin_user_eligibilities/
--rw-rw-r--   0 root         (0) root         (0)      536 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/admin_user_eligibilities/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    10216 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/admin_user_eligibilities/admin_retrieve_eligibilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:43:05.502181 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/agreement/
--rw-rw-r--   0 root         (0) root         (0)     1092 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/agreement/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6564 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/agreement/accept_versioned_policy.py
--rw-rw-r--   0 root         (0) root         (0)     6484 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/agreement/bulk_accept_versioned_policy.py
--rw-rw-r--   0 root         (0) root         (0)     8085 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/agreement/change_preference_consent.py
--rw-rw-r--   0 root         (0) root         (0)     6307 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/agreement/change_preference_consent_1.py
--rw-rw-r--   0 root         (0) root         (0)     9933 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/agreement/indirect_bulk_accept_ve_34e753.py
--rw-rw-r--   0 root         (0) root         (0)     7431 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/agreement/indirect_bulk_accept_ve_f4345a.py
--rw-rw-r--   0 root         (0) root         (0)     5813 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/agreement/retrieve_accepted_agreements.py
--rw-rw-r--   0 root         (0) root         (0)     5056 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/agreement/retrieve_agreements_public.py
--rw-rw-r--   0 root         (0) root         (0)     8879 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/agreement/retrieve_all_users_by_p_90a012.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:43:05.502181 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/agreement_with_namespace/
--rw-rw-r--   0 root         (0) root         (0)      700 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/agreement_with_namespace/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7189 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/agreement_with_namespace/retrieve_accepted_agree_8c230d.py
--rw-rw-r--   0 root         (0) root         (0)     8537 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/agreement_with_namespace/retrieve_accepted_agreements_1.py
--rw-rw-r--   0 root         (0) root         (0)    11063 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/agreement_with_namespace/retrieve_all_users_by_p_3f6faa.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:43:05.502181 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/anonymization/
--rw-rw-r--   0 root         (0) root         (0)      528 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/anonymization/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5912 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/anonymization/anonymize_user_agreement.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:43:05.502181 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/base_legal_policies/
--rw-rw-r--   0 root         (0) root         (0)      806 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/base_legal_policies/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7046 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/base_legal_policies/create_policy.py
--rw-rw-r--   0 root         (0) root         (0)     7801 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/base_legal_policies/partial_update_policy.py
--rw-rw-r--   0 root         (0) root         (0)     4803 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/base_legal_policies/retrieve_all_legal_policies.py
--rw-rw-r--   0 root         (0) root         (0)     6436 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/base_legal_policies/retrieve_all_policy_types.py
--rw-rw-r--   0 root         (0) root         (0)     7097 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/base_legal_policies/retrieve_policy_country.py
--rw-rw-r--   0 root         (0) root         (0)     6140 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/base_legal_policies/retrieve_single_policy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:43:05.502181 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/base_legal_policies_with_namespace/
--rw-rw-r--   0 root         (0) root         (0)      835 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/base_legal_policies_with_namespace/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8076 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/base_legal_policies_with_namespace/create_policy_1.py
--rw-rw-r--   0 root         (0) root         (0)     8262 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/base_legal_policies_with_namespace/partial_update_policy_1.py
--rw-rw-r--   0 root         (0) root         (0)     5921 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/base_legal_policies_with_namespace/retrieve_all_legal_poli_23dd4c.py
--rw-rw-r--   0 root         (0) root         (0)     7443 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/base_legal_policies_with_namespace/retrieve_all_policy_types_1.py
--rw-rw-r--   0 root         (0) root         (0)     7987 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/base_legal_policies_with_namespace/retrieve_policy_country_1.py
--rw-rw-r--   0 root         (0) root         (0)     7022 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/base_legal_policies_with_namespace/retrieve_single_policy_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:43:05.502181 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/eligibilities/
--rw-rw-r--   0 root         (0) root         (0)      618 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/eligibilities/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8954 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/eligibilities/retrieve_eligibilities__345271.py
--rw-rw-r--   0 root         (0) root         (0)     6542 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/eligibilities/retrieve_eligibilities_public.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:43:05.502181 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/localized_policy_versions/
--rw-rw-r--   0 root         (0) root         (0)      956 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/localized_policy_versions/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8119 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/localized_policy_versions/create_localized_policy_19e4a3.py
--rw-rw-r--   0 root         (0) root         (0)     8543 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/localized_policy_versions/request_presigned_url.py
--rw-rw-r--   0 root         (0) root         (0)     6190 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/localized_policy_versions/retrieve_localized_poli_24a671.py
--rw-rw-r--   0 root         (0) root         (0)     6894 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/localized_policy_versions/retrieve_single_localiz_2f6231.py
--rw-rw-r--   0 root         (0) root         (0)     6819 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/localized_policy_versions/retrieve_single_localiz_6ecc81.py
--rw-rw-r--   0 root         (0) root         (0)     6520 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/localized_policy_versions/set_default_policy.py
--rw-rw-r--   0 root         (0) root         (0)     8125 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/localized_policy_versions/update_localized_policy_a8a90f.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:43:05.506181 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/localized_policy_versions_with_namespace/
--rw-rw-r--   0 root         (0) root         (0)      966 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/localized_policy_versions_with_namespace/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     9014 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/localized_policy_versions_with_namespace/create_localized_policy_b58242.py
--rw-rw-r--   0 root         (0) root         (0)     9429 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/localized_policy_versions_with_namespace/request_presigned_url_1.py
--rw-rw-r--   0 root         (0) root         (0)     7079 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/localized_policy_versions_with_namespace/retrieve_localized_poli_4a4859.py
--rw-rw-r--   0 root         (0) root         (0)     7687 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/localized_policy_versions_with_namespace/retrieve_single_localiz_480659.py
--rw-rw-r--   0 root         (0) root         (0)     7788 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/localized_policy_versions_with_namespace/retrieve_single_localiz_f21ac4.py
--rw-rw-r--   0 root         (0) root         (0)     7023 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/localized_policy_versions_with_namespace/set_default_policy_1.py
--rw-rw-r--   0 root         (0) root         (0)     9020 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/localized_policy_versions_with_namespace/update_localized_policy_b28b13.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:43:05.506181 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/policies/
--rw-rw-r--   0 root         (0) root         (0)     1271 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/policies/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4490 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/policies/retrieve_country_list_w_8c69ff.py
--rw-rw-r--   0 root         (0) root         (0)    11624 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/policies/retrieve_latest_policie_29f65f.py
--rw-rw-r--   0 root         (0) root         (0)    12406 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/policies/retrieve_latest_policie_95ffb6.py
--rw-rw-r--   0 root         (0) root         (0)     9389 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/policies/retrieve_latest_policies.py
--rw-rw-r--   0 root         (0) root         (0)     5756 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/policies/retrieve_policies.py
--rw-rw-r--   0 root         (0) root         (0)     5855 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/policies/set_default_policy_2.py
--rw-rw-r--   0 root         (0) root         (0)     6967 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/policies/update_policy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:43:05.506181 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/policies_with_namespace/
--rw-rw-r--   0 root         (0) root         (0)      562 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/policies_with_namespace/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6723 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/policies_with_namespace/set_default_policy_3.py
--rw-rw-r--   0 root         (0) root         (0)     7885 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/policies_with_namespace/update_policy_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:43:05.506181 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/policy_versions/
--rw-rw-r--   0 root         (0) root         (0)      706 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/policy_versions/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7304 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/policy_versions/create_policy_version.py
--rw-rw-r--   0 root         (0) root         (0)     8084 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/policy_versions/publish_policy_version.py
--rw-rw-r--   0 root         (0) root         (0)     7345 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/policy_versions/retrieve_single_policy_version.py
--rw-rw-r--   0 root         (0) root         (0)     7958 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/policy_versions/update_policy_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:43:05.506181 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/policy_versions_with_namespace/
--rw-rw-r--   0 root         (0) root         (0)      716 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/policy_versions_with_namespace/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8195 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/policy_versions_with_namespace/create_policy_version_1.py
--rw-rw-r--   0 root         (0) root         (0)     8976 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/policy_versions_with_namespace/publish_policy_version_1.py
--rw-rw-r--   0 root         (0) root         (0)     8211 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/policy_versions_with_namespace/retrieve_single_policy__f63224.py
--rw-rw-r--   0 root         (0) root         (0)     8840 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/policy_versions_with_namespace/update_policy_version_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:43:05.506181 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/user_info/
--rw-rw-r--   0 root         (0) root         (0)      624 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/user_info/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6052 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/user_info/get_user_info_status.py
--rw-rw-r--   0 root         (0) root         (0)     5626 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/user_info/invalidate_user_info_cache.py
--rw-rw-r--   0 root         (0) root         (0)     5530 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/user_info/sync_user_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:43:05.506181 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/utility/
--rw-rw-r--   0 root         (0) root         (0)      511 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/utility/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4756 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/utility/check_readiness.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:43:05.510181 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/wrappers/
--rw-rw-r--   0 root         (0) root         (0)     9207 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/wrappers/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5300 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/wrappers/_admin_user_agreement.py
--rw-rw-r--   0 root         (0) root         (0)     5552 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/wrappers/_admin_user_eligibilities.py
--rw-rw-r--   0 root         (0) root         (0)    26050 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/wrappers/_agreement.py
--rw-rw-r--   0 root         (0) root         (0)    12067 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/wrappers/_agreement_with_namespace.py
--rw-rw-r--   0 root         (0) root         (0)     3496 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/wrappers/_anonymization.py
--rw-rw-r--   0 root         (0) root         (0)    16473 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/wrappers/_base_legal_policies.py
--rw-rw-r--   0 root         (0) root         (0)    20160 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/wrappers/_base_legal_policies_with_namespace.py
--rw-rw-r--   0 root         (0) root         (0)     8102 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/wrappers/_eligibilities.py
--rw-rw-r--   0 root         (0) root         (0)    21809 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/wrappers/_localized_policy_versions.py
--rw-rw-r--   0 root         (0) root         (0)    26019 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/wrappers/_localized_policy_versions_with_namespace.py
--rw-rw-r--   0 root         (0) root         (0)    24638 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/wrappers/_policies.py
--rw-rw-r--   0 root         (0) root         (0)     7021 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/wrappers/_policies_with_namespace.py
--rw-rw-r--   0 root         (0) root         (0)    13592 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/wrappers/_policy_versions.py
--rw-rw-r--   0 root         (0) root         (0)    15968 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/wrappers/_policy_versions_with_namespace.py
--rw-rw-r--   0 root         (0) root         (0)     8077 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/wrappers/_user_info.py
--rw-rw-r--   0 root         (0) root         (0)     3035 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/wrappers/_utility.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:43:05.510181 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk_service_legal.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1117 2024-03-26 05:43:05.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk_service_legal.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11221 2024-03-26 05:43:05.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk_service_legal.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-26 05:43:05.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk_service_legal.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 05:43:05.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk_service_legal.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-03-26 05:43:05.000000 accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk_service_legal.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)      355 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-legal-0.8.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-26 05:43:05.510181 accelbyte-py-sdk-service-legal-0.8.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:28:40.380595 accelbyte_py_sdk_service_legal-0.9.0/
+-rw-r--r--   0 root         (0) root         (0)     1117 2024-05-07 06:28:40.380595 accelbyte_py_sdk_service_legal-0.9.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      869 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:28:40.364596 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:28:40.364596 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:28:40.364596 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/
+-rw-rw-r--   0 root         (0) root         (0)     7955 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:28:40.368596 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/
+-rw-rw-r--   0 root         (0) root         (0)     3985 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7736 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/accept_agreement_request.py
+-rw-rw-r--   0 root         (0) root         (0)     4426 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/accept_agreement_response.py
+-rw-rw-r--   0 root         (0) root         (0)     8899 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/create_base_policy_request.py
+-rw-rw-r--   0 root         (0) root         (0)     8200 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/create_base_policy_request_v2.py
+-rw-rw-r--   0 root         (0) root         (0)    11723 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/create_base_policy_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5674 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/create_localized_policy_version_request.py
+-rw-rw-r--   0 root         (0) root         (0)     6963 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/create_localized_policy_version_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5652 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/create_policy_version_request.py
+-rw-rw-r--   0 root         (0) root         (0)     8539 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/create_policy_version_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4734 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/download_exported_agreements_in_csv_response.py
+-rw-rw-r--   0 root         (0) root         (0)     7478 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/error_entity.py
+-rw-rw-r--   0 root         (0) root         (0)     7297 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/field_validation_error.py
+-rw-rw-r--   0 root         (0) root         (0)     4711 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/initiate_export_agreements_to_csv_response.py
+-rw-rw-r--   0 root         (0) root         (0)     3943 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/legal_readiness_status_response.py
+-rw-rw-r--   0 root         (0) root         (0)    13110 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/localized_policy_version_object.py
+-rw-rw-r--   0 root         (0) root         (0)     5427 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/paged_retrieve_user_accepted_agreement_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4263 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/paging.py
+-rw-rw-r--   0 root         (0) root         (0)     4339 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/permission.py
+-rw-rw-r--   0 root         (0) root         (0)    12243 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/policy_object.py
+-rw-rw-r--   0 root         (0) root         (0)     9665 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/policy_version_object.py
+-rw-rw-r--   0 root         (0) root         (0)    11681 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/policy_version_with_localized_version_object.py
+-rw-rw-r--   0 root         (0) root         (0)    15327 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/retrieve_accepted_agreement_response.py
+-rw-rw-r--   0 root         (0) root         (0)    11928 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/retrieve_base_policy_response.py
+-rw-rw-r--   0 root         (0) root         (0)    16204 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/retrieve_localized_policy_version_public_response.py
+-rw-rw-r--   0 root         (0) root         (0)    13771 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/retrieve_localized_policy_version_response.py
+-rw-rw-r--   0 root         (0) root         (0)    17681 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/retrieve_policy_public_response.py
+-rw-rw-r--   0 root         (0) root         (0)    13724 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/retrieve_policy_response.py
+-rw-rw-r--   0 root         (0) root         (0)     7661 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/retrieve_policy_type_response.py
+-rw-rw-r--   0 root         (0) root         (0)    13008 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/retrieve_policy_version_response.py
+-rw-rw-r--   0 root         (0) root         (0)    14642 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/retrieve_user_accepted_agreement_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4052 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/retrieve_user_eligibilities_indirect_response.py
+-rw-rw-r--   0 root         (0) root         (0)    12987 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/retrieve_user_eligibilities_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4767 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/retrieve_user_info_cache_status_response.py
+-rw-rw-r--   0 root         (0) root         (0)     8217 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/update_base_policy_request.py
+-rw-rw-r--   0 root         (0) root         (0)     7516 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/update_base_policy_request_v2.py
+-rw-rw-r--   0 root         (0) root         (0)    11723 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/update_base_policy_response.py
+-rw-rw-r--   0 root         (0) root         (0)     8074 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/update_localized_policy_version_request.py
+-rw-rw-r--   0 root         (0) root         (0)    10944 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/update_localized_policy_version_response.py
+-rw-rw-r--   0 root         (0) root         (0)     7888 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/update_policy_request.py
+-rw-rw-r--   0 root         (0) root         (0)     5440 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/update_policy_version_request.py
+-rw-rw-r--   0 root         (0) root         (0)    10045 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/update_policy_version_response.py
+-rw-rw-r--   0 root         (0) root         (0)     6369 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/upload_localized_policy_version_attachment_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4900 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/upload_policy_version_attachment_request.py
+-rw-rw-r--   0 root         (0) root         (0)     5141 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/user_agreements_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4945 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/users_agreements_request.py
+-rw-rw-r--   0 root         (0) root         (0)     5625 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/validation_error_entity.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:28:40.368596 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/
+-rw-rw-r--   0 root         (0) root         (0)      434 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:28:40.368596 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/admin_user_agreement/
+-rw-rw-r--   0 root         (0) root         (0)      545 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/admin_user_agreement/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    10961 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/admin_user_agreement/indirect_bulk_accept_ve_9d5446.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:28:40.372595 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/admin_user_eligibilities/
+-rw-rw-r--   0 root         (0) root         (0)      536 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/admin_user_eligibilities/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    10259 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/admin_user_eligibilities/admin_retrieve_eligibilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:28:40.372595 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/agreement/
+-rw-rw-r--   0 root         (0) root         (0)     1092 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/agreement/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     6813 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/agreement/accept_versioned_policy.py
+-rw-rw-r--   0 root         (0) root         (0)     6690 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/agreement/bulk_accept_versioned_policy.py
+-rw-rw-r--   0 root         (0) root         (0)     8192 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/agreement/change_preference_consent.py
+-rw-rw-r--   0 root         (0) root         (0)     6542 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/agreement/change_preference_consent_1.py
+-rw-rw-r--   0 root         (0) root         (0)    10076 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/agreement/indirect_bulk_accept_ve_34e753.py
+-rw-rw-r--   0 root         (0) root         (0)     7665 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/agreement/indirect_bulk_accept_ve_f4345a.py
+-rw-rw-r--   0 root         (0) root         (0)     5892 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/agreement/retrieve_accepted_agreements.py
+-rw-rw-r--   0 root         (0) root         (0)     5262 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/agreement/retrieve_agreements_public.py
+-rw-rw-r--   0 root         (0) root         (0)     8950 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/agreement/retrieve_all_users_by_p_90a012.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:28:40.372595 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/agreement_with_namespace/
+-rw-rw-r--   0 root         (0) root         (0)      850 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/agreement_with_namespace/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7507 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/agreement_with_namespace/download_exported_agree_a56e5b.py
+-rw-rw-r--   0 root         (0) root         (0)     9972 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/agreement_with_namespace/initiate_export_agreeme_d92c31.py
+-rw-rw-r--   0 root         (0) root         (0)     7250 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/agreement_with_namespace/retrieve_accepted_agree_8c230d.py
+-rw-rw-r--   0 root         (0) root         (0)     8636 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/agreement_with_namespace/retrieve_accepted_agreements_1.py
+-rw-rw-r--   0 root         (0) root         (0)    11157 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/agreement_with_namespace/retrieve_all_users_by_p_3f6faa.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:28:40.372595 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/anonymization/
+-rw-rw-r--   0 root         (0) root         (0)      528 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/anonymization/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     5993 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/anonymization/anonymize_user_agreement.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:28:40.372595 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/base_legal_policies/
+-rw-rw-r--   0 root         (0) root         (0)      806 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/base_legal_policies/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7096 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/base_legal_policies/create_policy.py
+-rw-rw-r--   0 root         (0) root         (0)     7866 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/base_legal_policies/partial_update_policy.py
+-rw-rw-r--   0 root         (0) root         (0)     4857 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/base_legal_policies/retrieve_all_legal_policies.py
+-rw-rw-r--   0 root         (0) root         (0)     6489 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/base_legal_policies/retrieve_all_policy_types.py
+-rw-rw-r--   0 root         (0) root         (0)     7190 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/base_legal_policies/retrieve_policy_country.py
+-rw-rw-r--   0 root         (0) root         (0)     6209 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/base_legal_policies/retrieve_single_policy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:28:40.372595 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/base_legal_policies_with_namespace/
+-rw-rw-r--   0 root         (0) root         (0)      835 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/base_legal_policies_with_namespace/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8129 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/base_legal_policies_with_namespace/create_policy_1.py
+-rw-rw-r--   0 root         (0) root         (0)     8330 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/base_legal_policies_with_namespace/partial_update_policy_1.py
+-rw-rw-r--   0 root         (0) root         (0)     5978 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/base_legal_policies_with_namespace/retrieve_all_legal_poli_23dd4c.py
+-rw-rw-r--   0 root         (0) root         (0)     7499 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/base_legal_policies_with_namespace/retrieve_all_policy_types_1.py
+-rw-rw-r--   0 root         (0) root         (0)     8083 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/base_legal_policies_with_namespace/retrieve_policy_country_1.py
+-rw-rw-r--   0 root         (0) root         (0)     7094 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/base_legal_policies_with_namespace/retrieve_single_policy_1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:28:40.372595 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/eligibilities/
+-rw-rw-r--   0 root         (0) root         (0)      618 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/eligibilities/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     9234 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/eligibilities/retrieve_eligibilities__345271.py
+-rw-rw-r--   0 root         (0) root         (0)     6764 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/eligibilities/retrieve_eligibilities_public.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:28:40.372595 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/localized_policy_versions/
+-rw-rw-r--   0 root         (0) root         (0)      956 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/localized_policy_versions/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8208 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/localized_policy_versions/create_localized_policy_19e4a3.py
+-rw-rw-r--   0 root         (0) root         (0)     8644 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/localized_policy_versions/request_presigned_url.py
+-rw-rw-r--   0 root         (0) root         (0)     6283 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/localized_policy_versions/retrieve_localized_poli_24a671.py
+-rw-rw-r--   0 root         (0) root         (0)     6987 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/localized_policy_versions/retrieve_single_localiz_2f6231.py
+-rw-rw-r--   0 root         (0) root         (0)     7139 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/localized_policy_versions/retrieve_single_localiz_6ecc81.py
+-rw-rw-r--   0 root         (0) root         (0)     6633 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/localized_policy_versions/set_default_policy.py
+-rw-rw-r--   0 root         (0) root         (0)     8214 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/localized_policy_versions/update_localized_policy_a8a90f.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:28:40.376595 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/localized_policy_versions_with_namespace/
+-rw-rw-r--   0 root         (0) root         (0)      966 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/localized_policy_versions_with_namespace/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     9106 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/localized_policy_versions_with_namespace/create_localized_policy_b58242.py
+-rw-rw-r--   0 root         (0) root         (0)     9533 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/localized_policy_versions_with_namespace/request_presigned_url_1.py
+-rw-rw-r--   0 root         (0) root         (0)     7175 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/localized_policy_versions_with_namespace/retrieve_localized_poli_4a4859.py
+-rw-rw-r--   0 root         (0) root         (0)     8014 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/localized_policy_versions_with_namespace/retrieve_single_localiz_480659.py
+-rw-rw-r--   0 root         (0) root         (0)     7884 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/localized_policy_versions_with_namespace/retrieve_single_localiz_f21ac4.py
+-rw-rw-r--   0 root         (0) root         (0)     7123 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/localized_policy_versions_with_namespace/set_default_policy_1.py
+-rw-rw-r--   0 root         (0) root         (0)     9112 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/localized_policy_versions_with_namespace/update_localized_policy_b28b13.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:28:40.376595 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/policies/
+-rw-rw-r--   0 root         (0) root         (0)     1271 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/policies/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4765 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/policies/retrieve_country_list_w_8c69ff.py
+-rw-rw-r--   0 root         (0) root         (0)    11866 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/policies/retrieve_latest_policie_29f65f.py
+-rw-rw-r--   0 root         (0) root         (0)    12729 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/policies/retrieve_latest_policie_95ffb6.py
+-rw-rw-r--   0 root         (0) root         (0)     9673 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/policies/retrieve_latest_policies.py
+-rw-rw-r--   0 root         (0) root         (0)     5829 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/policies/retrieve_policies.py
+-rw-rw-r--   0 root         (0) root         (0)     5919 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/policies/set_default_policy_2.py
+-rw-rw-r--   0 root         (0) root         (0)     7023 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/policies/update_policy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:28:40.376595 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/policies_with_namespace/
+-rw-rw-r--   0 root         (0) root         (0)      562 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/policies_with_namespace/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     6790 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/policies_with_namespace/set_default_policy_3.py
+-rw-rw-r--   0 root         (0) root         (0)     7944 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/policies_with_namespace/update_policy_1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:28:40.376595 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/policy_versions/
+-rw-rw-r--   0 root         (0) root         (0)      706 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/policy_versions/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7369 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/policy_versions/create_policy_version.py
+-rw-rw-r--   0 root         (0) root         (0)     8163 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/policy_versions/publish_policy_version.py
+-rw-rw-r--   0 root         (0) root         (0)     7414 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/policy_versions/retrieve_single_policy_version.py
+-rw-rw-r--   0 root         (0) root         (0)     8030 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/policy_versions/update_policy_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:28:40.376595 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/policy_versions_with_namespace/
+-rw-rw-r--   0 root         (0) root         (0)      716 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/policy_versions_with_namespace/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8283 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/policy_versions_with_namespace/create_policy_version_1.py
+-rw-rw-r--   0 root         (0) root         (0)     9078 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/policy_versions_with_namespace/publish_policy_version_1.py
+-rw-rw-r--   0 root         (0) root         (0)     8303 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/policy_versions_with_namespace/retrieve_single_policy__f63224.py
+-rw-rw-r--   0 root         (0) root         (0)     8951 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/policy_versions_with_namespace/update_policy_version_1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:28:40.376595 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/user_info/
+-rw-rw-r--   0 root         (0) root         (0)      624 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/user_info/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     6101 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/user_info/get_user_info_status.py
+-rw-rw-r--   0 root         (0) root         (0)     5684 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/user_info/invalidate_user_info_cache.py
+-rw-rw-r--   0 root         (0) root         (0)     5588 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/user_info/sync_user_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:28:40.376595 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/utility/
+-rw-rw-r--   0 root         (0) root         (0)      511 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/utility/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4798 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/utility/check_readiness.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:28:40.380595 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/wrappers/
+-rw-rw-r--   0 root         (0) root         (0)     9515 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/wrappers/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4820 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/wrappers/_admin_user_agreement.py
+-rw-rw-r--   0 root         (0) root         (0)     5068 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/wrappers/_admin_user_eligibilities.py
+-rw-rw-r--   0 root         (0) root         (0)    23794 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/wrappers/_agreement.py
+-rw-rw-r--   0 root         (0) root         (0)    18111 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/wrappers/_agreement_with_namespace.py
+-rw-rw-r--   0 root         (0) root         (0)     3108 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/wrappers/_anonymization.py
+-rw-rw-r--   0 root         (0) root         (0)    14141 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/wrappers/_base_legal_policies.py
+-rw-rw-r--   0 root         (0) root         (0)    17588 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/wrappers/_base_legal_policies_with_namespace.py
+-rw-rw-r--   0 root         (0) root         (0)     7834 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/wrappers/_eligibilities.py
+-rw-rw-r--   0 root         (0) root         (0)    19461 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/wrappers/_localized_policy_versions.py
+-rw-rw-r--   0 root         (0) root         (0)    23431 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/wrappers/_localized_policy_versions_with_namespace.py
+-rw-rw-r--   0 root         (0) root         (0)    23372 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/wrappers/_policies.py
+-rw-rw-r--   0 root         (0) root         (0)     6153 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/wrappers/_policies_with_namespace.py
+-rw-rw-r--   0 root         (0) root         (0)    12016 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/wrappers/_policy_versions.py
+-rw-rw-r--   0 root         (0) root         (0)    14400 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/wrappers/_policy_versions_with_namespace.py
+-rw-rw-r--   0 root         (0) root         (0)     6897 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/wrappers/_user_info.py
+-rw-rw-r--   0 root         (0) root         (0)     2631 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/wrappers/_utility.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:28:40.380595 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk_service_legal.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1117 2024-05-07 06:28:40.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk_service_legal.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11625 2024-05-07 06:28:40.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk_service_legal.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-07 06:28:40.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk_service_legal.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-07 06:28:40.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk_service_legal.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-05-07 06:28:40.000000 accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk_service_legal.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)      355 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_legal-0.9.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-07 06:28:40.380595 accelbyte_py_sdk_service_legal-0.9.0/setup.cfg
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/PKG-INFO` & `accelbyte_py_sdk_service_legal-0.9.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: accelbyte-py-sdk-service-legal
-Version: 0.8.0
+Version: 0.9.0
 Summary: AccelByte Python SDK - AccelByte Gaming Services Legal Service
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: accelbyte-py-sdk-core
 
 [//]: # (Code generated. DO NOT EDIT!)
 
 # AccelByte Modular Python SDK - Service Module
 
 This is a service module for the [AccelByte Modular Python SDK](https://github.com/AccelByte/accelbyte-python-modular-sdk) package.
 
 ```text
 AccelByte Gaming Services Legal Service
-* Version: 1.39.0
+* Version: 1.41.0
 ```
 
 ## Setup
 
 This SDK requires Python 3.9 to be installed.
 
 ### Install with Pip
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/README.md` & `accelbyte_py_sdk_service_legal-0.9.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # AccelByte Modular Python SDK - Service Module
 
 This is a service module for the [AccelByte Modular Python SDK](https://github.com/AccelByte/accelbyte-python-modular-sdk) package.
 
 ```text
 AccelByte Gaming Services Legal Service
-* Version: 1.39.0
+* Version: 1.41.0
 ```
 
 ## Setup
 
 This SDK requires Python 3.9 to be installed.
 
 ### Install with Pip
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/__init__.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: service-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Legal Service."""
 
-__version__ = "1.39.0"
+__version__ = "1.41.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 # admin_user_agreement
 from .wrappers import indirect_bulk_accept_versioned_policy
@@ -39,14 +39,18 @@
 from .wrappers import retrieve_accepted_agreements_async
 from .wrappers import retrieve_agreements_public
 from .wrappers import retrieve_agreements_public_async
 from .wrappers import retrieve_all_users_by_policy_version
 from .wrappers import retrieve_all_users_by_policy_version_async
 
 # agreement_with_namespace
+from .wrappers import download_exported_agreements_in_csv
+from .wrappers import download_exported_agreements_in_csv_async
+from .wrappers import initiate_export_agreements_to_csv
+from .wrappers import initiate_export_agreements_to_csv_async
 from .wrappers import retrieve_accepted_agreements_1
 from .wrappers import retrieve_accepted_agreements_1_async
 from .wrappers import retrieve_accepted_agreements_for_multi_users
 from .wrappers import retrieve_accepted_agreements_for_multi_users_async
 from .wrappers import retrieve_all_users_by_policy_version_1
 from .wrappers import retrieve_all_users_by_policy_version_1_async
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/__init__.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: model-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Legal Service."""
 
-__version__ = "1.39.0"
+__version__ = "1.41.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .accept_agreement_request import AcceptAgreementRequest
 from .accept_agreement_response import AcceptAgreementResponse
@@ -21,22 +21,29 @@
 from .create_base_policy_response import CreateBasePolicyResponse
 from .create_localized_policy_version_request import CreateLocalizedPolicyVersionRequest
 from .create_localized_policy_version_response import (
     CreateLocalizedPolicyVersionResponse,
 )
 from .create_policy_version_request import CreatePolicyVersionRequest
 from .create_policy_version_response import CreatePolicyVersionResponse
+from .download_exported_agreements_in_csv_response import (
+    DownloadExportedAgreementsInCSVResponse,
+)
 from .error_entity import ErrorEntity
 from .field_validation_error import FieldValidationError
+from .initiate_export_agreements_to_csv_response import (
+    InitiateExportAgreementsToCSVResponse,
+)
 from .legal_readiness_status_response import LegalReadinessStatusResponse
 from .localized_policy_version_object import LocalizedPolicyVersionObject
 from .paged_retrieve_user_accepted_agreement_response import (
     PagedRetrieveUserAcceptedAgreementResponse,
 )
 from .paging import Paging
+from .permission import Permission
 from .policy_object import PolicyObject
 from .policy_version_object import PolicyVersionObject
 from .policy_version_with_localized_version_object import (
     PolicyVersionWithLocalizedVersionObject,
 )
 from .retrieve_accepted_agreement_response import RetrieveAcceptedAgreementResponse
 from .retrieve_base_policy_response import RetrieveBasePolicyResponse
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/accept_agreement_request.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/accept_agreement_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/accept_agreement_response.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/accept_agreement_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/create_base_policy_request.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/create_base_policy_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/create_base_policy_request_v2.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/create_base_policy_request_v2.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/create_base_policy_response.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/create_base_policy_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/create_localized_policy_version_request.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/create_localized_policy_version_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/create_localized_policy_version_response.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/create_localized_policy_version_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/create_policy_version_request.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/create_policy_version_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/create_policy_version_response.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/create_policy_version_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/error_entity.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/field_validation_error.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,72 +24,83 @@
 
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Model
 
 
-class ErrorEntity(Model):
-    """Error entity (ErrorEntity)
+class FieldValidationError(Model):
+    """Field validation error (FieldValidationError)
 
     Properties:
-        error_code: (errorCode) REQUIRED int
+        error_code: (errorCode) OPTIONAL str
 
-        error_message: (errorMessage) REQUIRED str
+        error_field: (errorField) OPTIONAL str
 
-        dev_stack_trace: (devStackTrace) OPTIONAL str
+        error_message: (errorMessage) OPTIONAL str
+
+        error_value: (errorValue) OPTIONAL str
 
         message_variables: (messageVariables) OPTIONAL Dict[str, str]
     """
 
     # region fields
 
-    error_code: int  # REQUIRED
-    error_message: str  # REQUIRED
-    dev_stack_trace: str  # OPTIONAL
+    error_code: str  # OPTIONAL
+    error_field: str  # OPTIONAL
+    error_message: str  # OPTIONAL
+    error_value: str  # OPTIONAL
     message_variables: Dict[str, str]  # OPTIONAL
 
     # endregion fields
 
     # region with_x methods
 
-    def with_error_code(self, value: int) -> ErrorEntity:
+    def with_error_code(self, value: str) -> FieldValidationError:
         self.error_code = value
         return self
 
-    def with_error_message(self, value: str) -> ErrorEntity:
+    def with_error_field(self, value: str) -> FieldValidationError:
+        self.error_field = value
+        return self
+
+    def with_error_message(self, value: str) -> FieldValidationError:
         self.error_message = value
         return self
 
-    def with_dev_stack_trace(self, value: str) -> ErrorEntity:
-        self.dev_stack_trace = value
+    def with_error_value(self, value: str) -> FieldValidationError:
+        self.error_value = value
         return self
 
-    def with_message_variables(self, value: Dict[str, str]) -> ErrorEntity:
+    def with_message_variables(self, value: Dict[str, str]) -> FieldValidationError:
         self.message_variables = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
         if hasattr(self, "error_code"):
-            result["errorCode"] = int(self.error_code)
+            result["errorCode"] = str(self.error_code)
         elif include_empty:
-            result["errorCode"] = 0
+            result["errorCode"] = ""
+        if hasattr(self, "error_field"):
+            result["errorField"] = str(self.error_field)
+        elif include_empty:
+            result["errorField"] = ""
         if hasattr(self, "error_message"):
             result["errorMessage"] = str(self.error_message)
         elif include_empty:
             result["errorMessage"] = ""
-        if hasattr(self, "dev_stack_trace"):
-            result["devStackTrace"] = str(self.dev_stack_trace)
+        if hasattr(self, "error_value"):
+            result["errorValue"] = str(self.error_value)
         elif include_empty:
-            result["devStackTrace"] = ""
+            result["errorValue"] = ""
         if hasattr(self, "message_variables"):
             result["messageVariables"] = {
                 str(k0): str(v0) for k0, v0 in self.message_variables.items()
             }
         elif include_empty:
             result["messageVariables"] = {}
         return result
@@ -97,100 +108,117 @@
     # endregion to methods
 
     # region static methods
 
     @classmethod
     def create(
         cls,
-        error_code: int,
-        error_message: str,
-        dev_stack_trace: Optional[str] = None,
+        error_code: Optional[str] = None,
+        error_field: Optional[str] = None,
+        error_message: Optional[str] = None,
+        error_value: Optional[str] = None,
         message_variables: Optional[Dict[str, str]] = None,
         **kwargs,
-    ) -> ErrorEntity:
+    ) -> FieldValidationError:
         instance = cls()
-        instance.error_code = error_code
-        instance.error_message = error_message
-        if dev_stack_trace is not None:
-            instance.dev_stack_trace = dev_stack_trace
+        if error_code is not None:
+            instance.error_code = error_code
+        if error_field is not None:
+            instance.error_field = error_field
+        if error_message is not None:
+            instance.error_message = error_message
+        if error_value is not None:
+            instance.error_value = error_value
         if message_variables is not None:
             instance.message_variables = message_variables
         return instance
 
     @classmethod
-    def create_from_dict(cls, dict_: dict, include_empty: bool = False) -> ErrorEntity:
+    def create_from_dict(
+        cls, dict_: dict, include_empty: bool = False
+    ) -> FieldValidationError:
         instance = cls()
         if not dict_:
             return instance
         if "errorCode" in dict_ and dict_["errorCode"] is not None:
-            instance.error_code = int(dict_["errorCode"])
+            instance.error_code = str(dict_["errorCode"])
+        elif include_empty:
+            instance.error_code = ""
+        if "errorField" in dict_ and dict_["errorField"] is not None:
+            instance.error_field = str(dict_["errorField"])
         elif include_empty:
-            instance.error_code = 0
+            instance.error_field = ""
         if "errorMessage" in dict_ and dict_["errorMessage"] is not None:
             instance.error_message = str(dict_["errorMessage"])
         elif include_empty:
             instance.error_message = ""
-        if "devStackTrace" in dict_ and dict_["devStackTrace"] is not None:
-            instance.dev_stack_trace = str(dict_["devStackTrace"])
+        if "errorValue" in dict_ and dict_["errorValue"] is not None:
+            instance.error_value = str(dict_["errorValue"])
         elif include_empty:
-            instance.dev_stack_trace = ""
+            instance.error_value = ""
         if "messageVariables" in dict_ and dict_["messageVariables"] is not None:
             instance.message_variables = {
                 str(k0): str(v0) for k0, v0 in dict_["messageVariables"].items()
             }
         elif include_empty:
             instance.message_variables = {}
         return instance
 
     @classmethod
     def create_many_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> Dict[str, ErrorEntity]:
+    ) -> Dict[str, FieldValidationError]:
         return (
             {k: cls.create_from_dict(v, include_empty=include_empty) for k, v in dict_}
             if dict_
             else {}
         )
 
     @classmethod
     def create_many_from_list(
         cls, list_: list, include_empty: bool = False
-    ) -> List[ErrorEntity]:
+    ) -> List[FieldValidationError]:
         return (
             [cls.create_from_dict(i, include_empty=include_empty) for i in list_]
             if list_
             else []
         )
 
     @classmethod
     def create_from_any(
         cls, any_: any, include_empty: bool = False, many: bool = False
-    ) -> Union[ErrorEntity, List[ErrorEntity], Dict[Any, ErrorEntity]]:
+    ) -> Union[
+        FieldValidationError,
+        List[FieldValidationError],
+        Dict[Any, FieldValidationError],
+    ]:
         if many:
             if isinstance(any_, dict):
                 return cls.create_many_from_dict(any_, include_empty=include_empty)
             elif isinstance(any_, list):
                 return cls.create_many_from_list(any_, include_empty=include_empty)
             else:
                 raise ValueError()
         else:
             return cls.create_from_dict(any_, include_empty=include_empty)
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
             "errorCode": "error_code",
+            "errorField": "error_field",
             "errorMessage": "error_message",
-            "devStackTrace": "dev_stack_trace",
+            "errorValue": "error_value",
             "messageVariables": "message_variables",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
-            "errorCode": True,
-            "errorMessage": True,
-            "devStackTrace": False,
+            "errorCode": False,
+            "errorField": False,
+            "errorMessage": False,
+            "errorValue": False,
             "messageVariables": False,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/field_validation_error.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/error_entity.py`

 * *Files 25% similar despite different names*

```diff
@@ -23,202 +23,200 @@
 # pylint: disable=unused-import
 
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Model
 
+from ..models.permission import Permission
 
-class FieldValidationError(Model):
-    """Field validation error (FieldValidationError)
 
-    Properties:
-        error_code: (errorCode) OPTIONAL str
+class ErrorEntity(Model):
+    """Error entity (ErrorEntity)
 
-        error_field: (errorField) OPTIONAL str
+    Properties:
+        error_code: (errorCode) REQUIRED int
 
-        error_message: (errorMessage) OPTIONAL str
+        error_message: (errorMessage) REQUIRED str
 
-        error_value: (errorValue) OPTIONAL str
+        dev_stack_trace: (devStackTrace) OPTIONAL str
 
         message_variables: (messageVariables) OPTIONAL Dict[str, str]
+
+        required_permission: (requiredPermission) OPTIONAL Permission
     """
 
     # region fields
 
-    error_code: str  # OPTIONAL
-    error_field: str  # OPTIONAL
-    error_message: str  # OPTIONAL
-    error_value: str  # OPTIONAL
+    error_code: int  # REQUIRED
+    error_message: str  # REQUIRED
+    dev_stack_trace: str  # OPTIONAL
     message_variables: Dict[str, str]  # OPTIONAL
+    required_permission: Permission  # OPTIONAL
 
     # endregion fields
 
     # region with_x methods
 
-    def with_error_code(self, value: str) -> FieldValidationError:
+    def with_error_code(self, value: int) -> ErrorEntity:
         self.error_code = value
         return self
 
-    def with_error_field(self, value: str) -> FieldValidationError:
-        self.error_field = value
-        return self
-
-    def with_error_message(self, value: str) -> FieldValidationError:
+    def with_error_message(self, value: str) -> ErrorEntity:
         self.error_message = value
         return self
 
-    def with_error_value(self, value: str) -> FieldValidationError:
-        self.error_value = value
+    def with_dev_stack_trace(self, value: str) -> ErrorEntity:
+        self.dev_stack_trace = value
         return self
 
-    def with_message_variables(self, value: Dict[str, str]) -> FieldValidationError:
+    def with_message_variables(self, value: Dict[str, str]) -> ErrorEntity:
         self.message_variables = value
         return self
 
+    def with_required_permission(self, value: Permission) -> ErrorEntity:
+        self.required_permission = value
+        return self
+
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
         if hasattr(self, "error_code"):
-            result["errorCode"] = str(self.error_code)
-        elif include_empty:
-            result["errorCode"] = ""
-        if hasattr(self, "error_field"):
-            result["errorField"] = str(self.error_field)
+            result["errorCode"] = int(self.error_code)
         elif include_empty:
-            result["errorField"] = ""
+            result["errorCode"] = 0
         if hasattr(self, "error_message"):
             result["errorMessage"] = str(self.error_message)
         elif include_empty:
             result["errorMessage"] = ""
-        if hasattr(self, "error_value"):
-            result["errorValue"] = str(self.error_value)
+        if hasattr(self, "dev_stack_trace"):
+            result["devStackTrace"] = str(self.dev_stack_trace)
         elif include_empty:
-            result["errorValue"] = ""
+            result["devStackTrace"] = ""
         if hasattr(self, "message_variables"):
             result["messageVariables"] = {
                 str(k0): str(v0) for k0, v0 in self.message_variables.items()
             }
         elif include_empty:
             result["messageVariables"] = {}
+        if hasattr(self, "required_permission"):
+            result["requiredPermission"] = self.required_permission.to_dict(
+                include_empty=include_empty
+            )
+        elif include_empty:
+            result["requiredPermission"] = Permission()
         return result
 
     # endregion to methods
 
     # region static methods
 
     @classmethod
     def create(
         cls,
-        error_code: Optional[str] = None,
-        error_field: Optional[str] = None,
-        error_message: Optional[str] = None,
-        error_value: Optional[str] = None,
+        error_code: int,
+        error_message: str,
+        dev_stack_trace: Optional[str] = None,
         message_variables: Optional[Dict[str, str]] = None,
+        required_permission: Optional[Permission] = None,
         **kwargs,
-    ) -> FieldValidationError:
+    ) -> ErrorEntity:
         instance = cls()
-        if error_code is not None:
-            instance.error_code = error_code
-        if error_field is not None:
-            instance.error_field = error_field
-        if error_message is not None:
-            instance.error_message = error_message
-        if error_value is not None:
-            instance.error_value = error_value
+        instance.error_code = error_code
+        instance.error_message = error_message
+        if dev_stack_trace is not None:
+            instance.dev_stack_trace = dev_stack_trace
         if message_variables is not None:
             instance.message_variables = message_variables
+        if required_permission is not None:
+            instance.required_permission = required_permission
         return instance
 
     @classmethod
-    def create_from_dict(
-        cls, dict_: dict, include_empty: bool = False
-    ) -> FieldValidationError:
+    def create_from_dict(cls, dict_: dict, include_empty: bool = False) -> ErrorEntity:
         instance = cls()
         if not dict_:
             return instance
         if "errorCode" in dict_ and dict_["errorCode"] is not None:
-            instance.error_code = str(dict_["errorCode"])
-        elif include_empty:
-            instance.error_code = ""
-        if "errorField" in dict_ and dict_["errorField"] is not None:
-            instance.error_field = str(dict_["errorField"])
+            instance.error_code = int(dict_["errorCode"])
         elif include_empty:
-            instance.error_field = ""
+            instance.error_code = 0
         if "errorMessage" in dict_ and dict_["errorMessage"] is not None:
             instance.error_message = str(dict_["errorMessage"])
         elif include_empty:
             instance.error_message = ""
-        if "errorValue" in dict_ and dict_["errorValue"] is not None:
-            instance.error_value = str(dict_["errorValue"])
+        if "devStackTrace" in dict_ and dict_["devStackTrace"] is not None:
+            instance.dev_stack_trace = str(dict_["devStackTrace"])
         elif include_empty:
-            instance.error_value = ""
+            instance.dev_stack_trace = ""
         if "messageVariables" in dict_ and dict_["messageVariables"] is not None:
             instance.message_variables = {
                 str(k0): str(v0) for k0, v0 in dict_["messageVariables"].items()
             }
         elif include_empty:
             instance.message_variables = {}
+        if "requiredPermission" in dict_ and dict_["requiredPermission"] is not None:
+            instance.required_permission = Permission.create_from_dict(
+                dict_["requiredPermission"], include_empty=include_empty
+            )
+        elif include_empty:
+            instance.required_permission = Permission()
         return instance
 
     @classmethod
     def create_many_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> Dict[str, FieldValidationError]:
+    ) -> Dict[str, ErrorEntity]:
         return (
             {k: cls.create_from_dict(v, include_empty=include_empty) for k, v in dict_}
             if dict_
             else {}
         )
 
     @classmethod
     def create_many_from_list(
         cls, list_: list, include_empty: bool = False
-    ) -> List[FieldValidationError]:
+    ) -> List[ErrorEntity]:
         return (
             [cls.create_from_dict(i, include_empty=include_empty) for i in list_]
             if list_
             else []
         )
 
     @classmethod
     def create_from_any(
         cls, any_: any, include_empty: bool = False, many: bool = False
-    ) -> Union[
-        FieldValidationError,
-        List[FieldValidationError],
-        Dict[Any, FieldValidationError],
-    ]:
+    ) -> Union[ErrorEntity, List[ErrorEntity], Dict[Any, ErrorEntity]]:
         if many:
             if isinstance(any_, dict):
                 return cls.create_many_from_dict(any_, include_empty=include_empty)
             elif isinstance(any_, list):
                 return cls.create_many_from_list(any_, include_empty=include_empty)
             else:
                 raise ValueError()
         else:
             return cls.create_from_dict(any_, include_empty=include_empty)
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
             "errorCode": "error_code",
-            "errorField": "error_field",
             "errorMessage": "error_message",
-            "errorValue": "error_value",
+            "devStackTrace": "dev_stack_trace",
             "messageVariables": "message_variables",
+            "requiredPermission": "required_permission",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
-            "errorCode": False,
-            "errorField": False,
-            "errorMessage": False,
-            "errorValue": False,
+            "errorCode": True,
+            "errorMessage": True,
+            "devStackTrace": False,
             "messageVariables": False,
+            "requiredPermission": False,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/legal_readiness_status_response.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/legal_readiness_status_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/localized_policy_version_object.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/localized_policy_version_object.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/paged_retrieve_user_accepted_agreement_response.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/paged_retrieve_user_accepted_agreement_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/paging.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/paging.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/policy_object.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/policy_object.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/policy_version_object.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/policy_version_object.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/policy_version_with_localized_version_object.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/policy_version_with_localized_version_object.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/retrieve_accepted_agreement_response.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/retrieve_accepted_agreement_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/retrieve_base_policy_response.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/retrieve_base_policy_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/retrieve_localized_policy_version_public_response.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/retrieve_localized_policy_version_public_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/retrieve_localized_policy_version_response.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/retrieve_localized_policy_version_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/retrieve_policy_public_response.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/retrieve_policy_public_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/retrieve_policy_response.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/retrieve_policy_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/retrieve_policy_type_response.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/retrieve_policy_type_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/retrieve_policy_version_response.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/retrieve_policy_version_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/retrieve_user_accepted_agreement_response.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/retrieve_user_accepted_agreement_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/retrieve_user_eligibilities_indirect_response.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/retrieve_user_eligibilities_indirect_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/retrieve_user_eligibilities_response.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/retrieve_user_eligibilities_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/retrieve_user_info_cache_status_response.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/retrieve_user_info_cache_status_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/update_base_policy_request.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/update_base_policy_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/update_base_policy_request_v2.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/update_base_policy_request_v2.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/update_base_policy_response.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/update_base_policy_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/update_localized_policy_version_request.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/update_localized_policy_version_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/update_localized_policy_version_response.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/update_localized_policy_version_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/update_policy_request.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/update_policy_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/update_policy_version_request.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/update_policy_version_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/update_policy_version_response.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/update_policy_version_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/upload_localized_policy_version_attachment_response.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/upload_localized_policy_version_attachment_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/upload_policy_version_attachment_request.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/upload_policy_version_attachment_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/user_agreements_response.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/user_agreements_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/users_agreements_request.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/users_agreements_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/models/validation_error_entity.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/models/validation_error_entity.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/admin_user_agreement/__init__.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/admin_user_agreement/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,14 +4,14 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Legal Service."""
 
-__version__ = "1.39.0"
+__version__ = "1.41.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .indirect_bulk_accept_ve_9d5446 import IndirectBulkAcceptVersionedPolicy
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/admin_user_agreement/indirect_bulk_accept_ve_9d5446.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/admin_user_agreement/indirect_bulk_accept_ve_9d5446.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,32 +32,28 @@
 from ...models import AcceptAgreementRequest
 from ...models import AcceptAgreementResponse
 
 
 class IndirectBulkAcceptVersionedPolicy(Operation):
     """Admin bulk accept Policy Versions (indirectBulkAcceptVersionedPolicy)
 
-    Accepts many legal policy versions all at once. Supply with localized version policy id and userId to accept an agreement. Other detail info:
-      * Required permission : resource="ADMIN:NAMESPACE:{namespace}:USER:{userId}:LEGAL", action=1 (CREATE)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:LEGAL [CREATE]
+    Accepts many legal policy versions all at once. Supply with localized version policy id and userId to accept an agreement.
 
     Properties:
         url: /agreement/admin/namespaces/{namespace}/users/{userId}/agreements/policies
 
         method: POST
 
         tags: ["Admin User Agreement"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         body: (body) OPTIONAL List[AcceptAgreementRequest] in body
 
         namespace: (namespace) REQUIRED str in path
 
         user_id: (userId) REQUIRED str in path
 
@@ -72,20 +68,26 @@
     """
 
     # region fields
 
     _url: str = (
         "/agreement/admin/namespaces/{namespace}/users/{userId}/agreements/policies"
     )
+    _path: str = (
+        "/agreement/admin/namespaces/{namespace}/users/{userId}/agreements/policies"
+    )
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
-    _securities: List[List[str]] = [["BEARER_AUTH"], ["BEARER_AUTH"]]
+    _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "legal"
+
     body: List[AcceptAgreementRequest]  # OPTIONAL in [body]
     namespace: str  # REQUIRED in [path]
     user_id: str  # REQUIRED in [path]
     publisher_user_id: str  # OPTIONAL in [query]
     client_id: str  # REQUIRED in [query]
     country_code: str  # REQUIRED in [query]
 
@@ -94,14 +96,22 @@
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/admin_user_eligibilities/__init__.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/admin_user_eligibilities/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,14 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Legal Service."""
 
-__version__ = "1.39.0"
+__version__ = "1.41.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .admin_retrieve_eligibilities import AdminRetrieveEligibilities
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/admin_user_eligibilities/admin_retrieve_eligibilities.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/admin_user_eligibilities/admin_retrieve_eligibilities.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,33 +35,26 @@
 
 class AdminRetrieveEligibilities(Operation):
     """Check User Legal Eligibility (adminRetrieveEligibilities)
 
     Retrieve the active policies and its conformance status by user.
     This process only supports cross-namespace checking between game namespace and publisher namespace , that means if the active policy already accepted by the same user in publisher namespace, then it will also be considered as eligible in non-publisher namespace.
 
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:{namespace}:USER:{userId}:LEGAL", action=2 (READ)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:LEGAL [READ]
-
     Properties:
         url: /agreement/admin/namespaces/{namespace}/users/{userId}/eligibilities
 
         method: GET
 
         tags: ["Admin User Eligibilities"]
 
         consumes: []
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         namespace: (namespace) REQUIRED str in path
 
         user_id: (userId) REQUIRED str in path
 
         publisher_user_id: (publisherUserId) OPTIONAL str in query
 
@@ -74,20 +67,24 @@
 
         400: Bad Request - ErrorEntity (40045: errors.net.accelbyte.platform.legal.user_id_needed)
     """
 
     # region fields
 
     _url: str = "/agreement/admin/namespaces/{namespace}/users/{userId}/eligibilities"
+    _path: str = "/agreement/admin/namespaces/{namespace}/users/{userId}/eligibilities"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
-    _securities: List[List[str]] = [["BEARER_AUTH"], ["BEARER_AUTH"]]
+    _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "legal"
+
     namespace: str  # REQUIRED in [path]
     user_id: str  # REQUIRED in [path]
     publisher_user_id: str  # OPTIONAL in [query]
     client_id: str  # REQUIRED in [query]
     country_code: str  # REQUIRED in [query]
 
     # endregion fields
@@ -95,14 +92,22 @@
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/agreement/__init__.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/agreement/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Legal Service."""
 
-__version__ = "1.39.0"
+__version__ = "1.41.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .accept_versioned_policy import AcceptVersionedPolicy
 from .bulk_accept_versioned_policy import BulkAcceptVersionedPolicy
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/agreement/accept_versioned_policy.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/agreement/accept_versioned_policy.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,18 +31,15 @@
 
 from ...models import ErrorEntity
 
 
 class AcceptVersionedPolicy(Operation):
     """Accept a Policy Version (acceptVersionedPolicy)
 
-    Accepts a legal policy version. Supply with localized version policy id to accept an agreement.
-    Other detail info:
-
-      * Required permission : login user
+    Accepts a legal policy version. Supply with localized version policy id to accept an agreement
 
     Properties:
         url: /agreement/public/agreements/localized-policy-versions/{localizedPolicyVersionId}
 
         method: POST
 
         tags: ["Agreement"]
@@ -60,31 +57,43 @@
 
         400: Bad Request - ErrorEntity (40045: errors.net.accelbyte.platform.legal.user_id_needed | 40035: errors.net.accelbyte.platform.legal.invalid_localize_policy_version_id)
     """
 
     # region fields
 
     _url: str = "/agreement/public/agreements/localized-policy-versions/{localizedPolicyVersionId}"
+    _path: str = "/agreement/public/agreements/localized-policy-versions/{localizedPolicyVersionId}"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "legal"
+
     localized_policy_version_id: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/agreement/bulk_accept_versioned_policy.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/agreement/bulk_accept_versioned_policy.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,17 +34,14 @@
 from ...models import ErrorEntity
 
 
 class BulkAcceptVersionedPolicy(Operation):
     """Bulk Accept Policy Versions (bulkAcceptVersionedPolicy)
 
     Accepts many legal policy versions all at once. Supply with localized version policy id to accept an agreement.
-    Other detail info:
-
-      * Required permission : login user
 
     Properties:
         url: /agreement/public/agreements/policies
 
         method: POST
 
         tags: ["Agreement"]
@@ -62,31 +59,43 @@
 
         400: Bad Request - ErrorEntity (40045: errors.net.accelbyte.platform.legal.user_id_needed | 40035: errors.net.accelbyte.platform.legal.invalid_localize_policy_version_id)
     """
 
     # region fields
 
     _url: str = "/agreement/public/agreements/policies"
+    _path: str = "/agreement/public/agreements/policies"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "legal"
+
     body: List[AcceptAgreementRequest]  # OPTIONAL in [body]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/agreement/change_preference_consent.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/agreement/change_preference_consent.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,33 +32,28 @@
 from ...models import AcceptAgreementRequest
 from ...models import ErrorEntity
 
 
 class ChangePreferenceConsent(Operation):
     """Change Preference Consent (changePreferenceConsent)
 
-    This API will Update Preference Consent. Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:{namespace}:LEGAL", action=4 (UPDATE)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:LEGAL [UPDATE]
+    This API will Update Preference Consent
 
     Properties:
         url: /agreement/admin/agreements/localized-policy-versions/preferences/namespaces/{namespace}/userId/{userId}
 
         method: PATCH
 
         tags: ["Agreement"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         body: (body) OPTIONAL List[AcceptAgreementRequest] in body
 
         namespace: (namespace) REQUIRED str in path
 
         user_id: (userId) REQUIRED str in path
 
@@ -67,33 +62,45 @@
 
         404: Not Found - ErrorEntity (40047: errors.net.accelbyte.platform.legal.user_agreement_not_found)
     """
 
     # region fields
 
     _url: str = "/agreement/admin/agreements/localized-policy-versions/preferences/namespaces/{namespace}/userId/{userId}"
+    _path: str = "/agreement/admin/agreements/localized-policy-versions/preferences/namespaces/{namespace}/userId/{userId}"
+    _base_path: str = ""
     _method: str = "PATCH"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
-    _securities: List[List[str]] = [["BEARER_AUTH"], ["BEARER_AUTH"]]
+    _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "legal"
+
     body: List[AcceptAgreementRequest]  # OPTIONAL in [body]
     namespace: str  # REQUIRED in [path]
     user_id: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/agreement/change_preference_consent_1.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/agreement/change_preference_consent_1.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,17 +33,14 @@
 from ...models import ErrorEntity
 
 
 class ChangePreferenceConsent1(Operation):
     """Accept/Revoke Marketing Preference Consent (changePreferenceConsent_1)
 
     Change marketing preference consent.
-    Other detail info:
-
-      * Required permission : login user
 
     Properties:
         url: /agreement/public/agreements/localized-policy-versions/preferences
 
         method: PATCH
 
         tags: ["Agreement"]
@@ -61,31 +58,43 @@
 
         400: Bad Request - ErrorEntity (40017: Policy with id : [{policyId}] is not marketing preference | 40045: errors.net.accelbyte.platform.legal.user_id_needed)
     """
 
     # region fields
 
     _url: str = "/agreement/public/agreements/localized-policy-versions/preferences"
+    _path: str = "/agreement/public/agreements/localized-policy-versions/preferences"
+    _base_path: str = ""
     _method: str = "PATCH"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "legal"
+
     body: List[AcceptAgreementRequest]  # OPTIONAL in [body]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/agreement/indirect_bulk_accept_ve_34e753.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/agreement/indirect_bulk_accept_ve_34e753.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,36 +31,30 @@
 from accelbyte_py_sdk.core import deprecated
 
 from ...models import AcceptAgreementRequest
 from ...models import AcceptAgreementResponse
 
 
 class IndirectBulkAcceptVersionedPolicyV2(Operation):
-    """Bulk Accept Policy Versions (Indirect) (indirectBulkAcceptVersionedPolicyV2)
+    """[DEPRECATED] Bulk Accept Policy Versions (Indirect) (indirectBulkAcceptVersionedPolicyV2)
 
     Accepts many legal policy versions all at once. Supply with localized version policy id, version policy id, policy id, userId, namespace, country code and client id to accept an agreement. This endpoint used by APIGateway during new user registration.
-    Other detail info:
-
-      * Required permission : resource="NAMESPACE:{namespace}:LEGAL", action=1 (CREATE)
-
-    Required Permission(s):
-        - NAMESPACE:{namespace}:LEGAL [CREATE]
 
     Properties:
         url: /agreement/public/agreements/policies/namespaces/{namespace}/countries/{countryCode}/clients/{clientId}/users/{userId}
 
         method: POST
 
         tags: ["Agreement"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         body: (body) OPTIONAL List[AcceptAgreementRequest] in body
 
         client_id: (clientId) REQUIRED str in path
 
         country_code: (countryCode) REQUIRED str in path
 
@@ -71,20 +65,24 @@
     Responses:
         201: Created - AcceptAgreementResponse (successful operation)
     """
 
     # region fields
 
     _url: str = "/agreement/public/agreements/policies/namespaces/{namespace}/countries/{countryCode}/clients/{clientId}/users/{userId}"
+    _path: str = "/agreement/public/agreements/policies/namespaces/{namespace}/countries/{countryCode}/clients/{clientId}/users/{userId}"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
-    _securities: List[List[str]] = [["BEARER_AUTH"], ["BEARER_AUTH"]]
+    _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "legal"
+
     body: List[AcceptAgreementRequest]  # OPTIONAL in [body]
     client_id: str  # REQUIRED in [path]
     country_code: str  # REQUIRED in [path]
     namespace: str  # REQUIRED in [path]
     user_id: str  # REQUIRED in [path]
 
     # endregion fields
@@ -92,14 +90,22 @@
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/agreement/indirect_bulk_accept_ve_f4345a.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/agreement/indirect_bulk_accept_ve_f4345a.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,20 +32,17 @@
 
 from ...models import AcceptAgreementRequest
 from ...models import AcceptAgreementResponse
 from ...models import ErrorEntity
 
 
 class IndirectBulkAcceptVersionedPolicy1(Operation):
-    """Bulk Accept Policy Versions (Indirect) (indirectBulkAcceptVersionedPolicy_1)
+    """[DEPRECATED] Bulk Accept Policy Versions (Indirect) (indirectBulkAcceptVersionedPolicy_1)
 
     Accepts many legal policy versions all at once. Supply with localized version policy id and userId to accept an agreement. This endpoint used by Authentication Service during new user registration.
-    Other detail info:
-
-      * Required permission : login user
 
     Properties:
         url: /agreement/public/agreements/policies/users/{userId}
 
         method: POST
 
         tags: ["Agreement"]
@@ -65,32 +62,44 @@
 
         404: Not Found - ErrorEntity (40035: errors.net.accelbyte.platform.legal.policy_version_not_found)
     """
 
     # region fields
 
     _url: str = "/agreement/public/agreements/policies/users/{userId}"
+    _path: str = "/agreement/public/agreements/policies/users/{userId}"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "legal"
+
     body: List[AcceptAgreementRequest]  # OPTIONAL in [body]
     user_id: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/agreement/retrieve_accepted_agreements.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/agreement/retrieve_accepted_agreements.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,59 +31,67 @@
 
 from ...models import RetrieveAcceptedAgreementResponse
 
 
 class RetrieveAcceptedAgreements(Operation):
     """Retrieve Accepted Legal Agreements (retrieveAcceptedAgreements)
 
-    This API will return all accepted Legal Agreements for specified user. Other detail info:
-      * Required permission : resource="ADMIN:NAMESPACE:*:LEGAL", action=2 (READ)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:*:LEGAL [READ]
+    This API will return all accepted Legal Agreements for specified user
 
     Properties:
         url: /agreement/admin/agreements/policies/users/{userId}
 
         method: GET
 
         tags: ["Agreement"]
 
         consumes: []
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         user_id: (userId) REQUIRED str in path
 
     Responses:
         200: OK - List[RetrieveAcceptedAgreementResponse] (successful operation)
     """
 
     # region fields
 
     _url: str = "/agreement/admin/agreements/policies/users/{userId}"
+    _path: str = "/agreement/admin/agreements/policies/users/{userId}"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
-    _securities: List[List[str]] = [["BEARER_AUTH"], ["BEARER_AUTH"]]
+    _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "legal"
+
     user_id: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/agreement/retrieve_agreements_public.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/agreement/retrieve_agreements_public.py`

 * *Files 13% similar despite different names*

```diff
@@ -33,17 +33,14 @@
 from ...models import RetrieveAcceptedAgreementResponse
 
 
 class RetrieveAgreementsPublic(Operation):
     """Retrieve the accepted Legal Agreements (retrieveAgreementsPublic)
 
     Retrieve accepted Legal Agreements.
-    Other detail info:
-
-      * Required permission : login user
 
     Properties:
         url: /agreement/public/agreements/policies
 
         method: GET
 
         tags: ["Agreement"]
@@ -59,29 +56,41 @@
 
         400: Bad Request - ErrorEntity (40045: errors.net.accelbyte.platform.legal.user_id_needed)
     """
 
     # region fields
 
     _url: str = "/agreement/public/agreements/policies"
+    _path: str = "/agreement/public/agreements/policies"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "legal"
+
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/agreement/retrieve_all_users_by_p_90a012.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/agreement/retrieve_all_users_by_p_90a012.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,34 +30,30 @@
 from accelbyte_py_sdk.core import HttpResponse
 
 from ...models import ErrorEntity
 from ...models import PagedRetrieveUserAcceptedAgreementResponse
 
 
 class RetrieveAllUsersByPolicyVersion(Operation):
-    """Retrieve All Users Accepting Legal Agreements (retrieveAllUsersByPolicyVersion)
+    """Retrieve Users Accepting Legal Agreements (retrieveAllUsersByPolicyVersion)
 
-    This API will return all users who has accepted a specific policy version.Other detail info:
-      * Required permission : resource="ADMIN:NAMESPACE:*:LEGAL", action=2 (READ)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:*:LEGAL [READ]
+    This API will return users who has accepted a specific policy version.
 
     Properties:
         url: /agreement/admin/agreements/policy-versions/users
 
         method: GET
 
         tags: ["Agreement"]
 
         consumes: []
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         keyword: (keyword) OPTIONAL str in query
 
         limit: (limit) OPTIONAL int in query
 
         offset: (offset) OPTIONAL int in query
 
@@ -68,34 +64,46 @@
 
         404: Not Found - ErrorEntity (40035: errors.net.accelbyte.platform.legal.policy_version_not_found)
     """
 
     # region fields
 
     _url: str = "/agreement/admin/agreements/policy-versions/users"
+    _path: str = "/agreement/admin/agreements/policy-versions/users"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
-    _securities: List[List[str]] = [["BEARER_AUTH"], ["BEARER_AUTH"]]
+    _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "legal"
+
     keyword: str  # OPTIONAL in [query]
     limit: int  # OPTIONAL in [query]
     offset: int  # OPTIONAL in [query]
     policy_version_id: str  # REQUIRED in [query]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/agreement_with_namespace/__init__.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/agreement_with_namespace/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,16 +4,18 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Legal Service."""
 
-__version__ = "1.39.0"
+__version__ = "1.41.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
+from .download_exported_agree_a56e5b import DownloadExportedAgreementsInCSV
+from .initiate_export_agreeme_d92c31 import InitiateExportAgreementsToCSV
 from .retrieve_accepted_agreements_1 import RetrieveAcceptedAgreements1
 from .retrieve_accepted_agree_8c230d import RetrieveAcceptedAgreementsForMultiUsers
 from .retrieve_all_users_by_p_3f6faa import RetrieveAllUsersByPolicyVersion1
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/agreement_with_namespace/retrieve_accepted_agree_8c230d.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/agreement_with_namespace/retrieve_accepted_agree_8c230d.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,62 +32,70 @@
 from ...models import UserAgreementsResponse
 from ...models import UsersAgreementsRequest
 
 
 class RetrieveAcceptedAgreementsForMultiUsers(Operation):
     """Retrieve Accepted Legal Agreements For Multi Users (retrieveAcceptedAgreementsForMultiUsers)
 
-    This API will return all accepted Legal Agreements for each user, including agreements of game users if publisher user has corresponding game accountOther detail info:
-      * Required permission : resource="ADMIN:NAMESPACE:{namespace}:LEGAL", action=2 (READ)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:LEGAL [READ]
+    This API will return all accepted Legal Agreements for each user, including agreements of game users if publisher user has corresponding game account.
 
     Properties:
         url: /agreement/admin/namespaces/{namespace}/agreements
 
         method: POST
 
         tags: ["Agreement With Namespace"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         body: (body) OPTIONAL UsersAgreementsRequest in body
 
         namespace: (namespace) REQUIRED str in path
 
     Responses:
         200: OK - List[UserAgreementsResponse] (successful operation)
     """
 
     # region fields
 
     _url: str = "/agreement/admin/namespaces/{namespace}/agreements"
+    _path: str = "/agreement/admin/namespaces/{namespace}/agreements"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
-    _securities: List[List[str]] = [["BEARER_AUTH"], ["BEARER_AUTH"]]
+    _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "legal"
+
     body: UsersAgreementsRequest  # OPTIONAL in [body]
     namespace: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/agreement_with_namespace/retrieve_accepted_agreements_1.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/agreement_with_namespace/retrieve_accepted_agreements_1.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,32 +31,28 @@
 
 from ...models import RetrieveAcceptedAgreementResponse
 
 
 class RetrieveAcceptedAgreements1(Operation):
     """Retrieve Accepted Legal Agreements (retrieveAcceptedAgreements_1)
 
-    This API will return all accepted Legal Agreements for specified user. Other detail info:
-      * Required permission : resource="ADMIN:NAMESPACE:{namespace}:LEGAL", action=2 (READ)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:LEGAL [READ]
+    This API will return all accepted Legal Agreements for specified user.
 
     Properties:
         url: /agreement/admin/namespaces/{namespace}/agreements/policies/users/{userId}
 
         method: GET
 
         tags: ["Agreement With Namespace"]
 
         consumes: []
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         namespace: (namespace) REQUIRED str in path
 
         user_id: (userId) REQUIRED str in path
 
         exclude_other_namespaces_policies: (excludeOtherNamespacesPolicies) OPTIONAL bool in query
 
@@ -65,33 +61,47 @@
     """
 
     # region fields
 
     _url: str = (
         "/agreement/admin/namespaces/{namespace}/agreements/policies/users/{userId}"
     )
+    _path: str = (
+        "/agreement/admin/namespaces/{namespace}/agreements/policies/users/{userId}"
+    )
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
-    _securities: List[List[str]] = [["BEARER_AUTH"], ["BEARER_AUTH"]]
+    _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "legal"
+
     namespace: str  # REQUIRED in [path]
     user_id: str  # REQUIRED in [path]
     exclude_other_namespaces_policies: bool  # OPTIONAL in [query]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/agreement_with_namespace/retrieve_all_users_by_p_3f6faa.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/agreement_with_namespace/retrieve_all_users_by_p_3f6faa.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,34 +30,30 @@
 from accelbyte_py_sdk.core import HttpResponse
 
 from ...models import ErrorEntity
 from ...models import PagedRetrieveUserAcceptedAgreementResponse
 
 
 class RetrieveAllUsersByPolicyVersion1(Operation):
-    """Retrieve All Users Accepting Legal Agreements (retrieveAllUsersByPolicyVersion_1)
+    """Retrieve Users Accepting Legal Agreements (retrieveAllUsersByPolicyVersion_1)
 
-    This API will return all users who has accepted a specific policy version.Other detail info:
-      * Required permission : resource="ADMIN:NAMESPACE:{namespace}:LEGAL", action=2 (READ)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:LEGAL [READ]
+    This API will return all users who has accepted a specific policy version.
 
     Properties:
         url: /agreement/admin/namespaces/{namespace}/agreements/policy-versions/users
 
         method: GET
 
         tags: ["Agreement With Namespace"]
 
         consumes: []
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         namespace: (namespace) REQUIRED str in path
 
         convert_game_user_id: (convertGameUserId) OPTIONAL bool in query
 
         keyword: (keyword) OPTIONAL str in query
 
@@ -74,20 +70,26 @@
     """
 
     # region fields
 
     _url: str = (
         "/agreement/admin/namespaces/{namespace}/agreements/policy-versions/users"
     )
+    _path: str = (
+        "/agreement/admin/namespaces/{namespace}/agreements/policy-versions/users"
+    )
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
-    _securities: List[List[str]] = [["BEARER_AUTH"], ["BEARER_AUTH"]]
+    _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "legal"
+
     namespace: str  # REQUIRED in [path]
     convert_game_user_id: bool  # OPTIONAL in [query]
     keyword: str  # OPTIONAL in [query]
     limit: int  # OPTIONAL in [query]
     offset: int  # OPTIONAL in [query]
     policy_version_id: str  # REQUIRED in [query]
 
@@ -96,14 +98,22 @@
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/anonymization/__init__.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/policies_with_namespace/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Legal Service."""
 
-__version__ = "1.39.0"
+__version__ = "1.41.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
-from .anonymize_user_agreement import AnonymizeUserAgreement
+from .set_default_policy_3 import SetDefaultPolicy3
+from .update_policy_1 import UpdatePolicy1
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/anonymization/anonymize_user_agreement.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/anonymization/anonymize_user_agreement.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,61 +31,69 @@
 
 from ...models import ErrorEntity
 
 
 class AnonymizeUserAgreement(Operation):
     """Anonymize user's agreement record (anonymizeUserAgreement)
 
-    This API will anonymize agreement record for specified user. Other detail info:
-      * Required permission : resource="ADMIN:NAMESPACE:*:LEGAL", action=8 (DELETE)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:*:LEGAL [DELETE]
+    This API will anonymize agreement record for specified user.
 
     Properties:
         url: /agreement/admin/users/{userId}/anonymization/agreements
 
         method: DELETE
 
         tags: ["Anonymization"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         user_id: (userId) REQUIRED str in path
 
     Responses:
         204: No Content - (successful anonymize)
 
         404: Not Found - ErrorEntity (40045: errors.net.accelbyte.platform.legal.user_agreement_not_found)
     """
 
     # region fields
 
     _url: str = "/agreement/admin/users/{userId}/anonymization/agreements"
+    _path: str = "/agreement/admin/users/{userId}/anonymization/agreements"
+    _base_path: str = ""
     _method: str = "DELETE"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
-    _securities: List[List[str]] = [["BEARER_AUTH"], ["BEARER_AUTH"]]
+    _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "legal"
+
     user_id: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/base_legal_policies/__init__.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/base_legal_policies/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Legal Service."""
 
-__version__ = "1.39.0"
+__version__ = "1.41.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .create_policy import CreatePolicy
 from .partial_update_policy import PartialUpdatePolicy
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/base_legal_policies/create_policy.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/base_legal_policies/create_policy.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,33 +35,27 @@
 from ...models import ValidationErrorEntity
 
 
 class CreatePolicy(Operation):
     """Create a Base Legal Policy (createPolicy)
 
     Create a legal policy.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:*:LEGAL", action=1 (CREATE)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:*:LEGAL [CREATE]
 
     Properties:
         url: /agreement/admin/base-policies
 
         method: POST
 
         tags: ["Base Legal Policies"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         body: (body) OPTIONAL CreateBasePolicyRequest in body
 
     Responses:
         201: Created - CreateBasePolicyResponse (successful operation)
 
         400: Bad Request - ErrorEntity (40038: errors.net.accelbyte.platform.legal.invalid_affected_client_id | 40026: errors.net.accelbyte.platform.legal.not_allow_create_studio_policy)
@@ -70,31 +64,43 @@
 
         422: Unprocessable Entity - ValidationErrorEntity (20002: validation error)
     """
 
     # region fields
 
     _url: str = "/agreement/admin/base-policies"
+    _path: str = "/agreement/admin/base-policies"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
-    _securities: List[List[str]] = [["BEARER_AUTH"], ["BEARER_AUTH"]]
+    _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "legal"
+
     body: CreateBasePolicyRequest  # OPTIONAL in [body]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/base_legal_policies/partial_update_policy.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/base_legal_policies/partial_update_policy.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,33 +34,27 @@
 from ...models import UpdateBasePolicyResponse
 
 
 class PartialUpdatePolicy(Operation):
     """Update Base Legal Policy (partialUpdatePolicy)
 
     Update an existing base policy.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:*:LEGAL", action=4 (UPDATE)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:*:LEGAL [UPDATE]
 
     Properties:
         url: /agreement/admin/base-policies/{basePolicyId}
 
         method: PATCH
 
         tags: ["Base Legal Policies"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         body: (body) OPTIONAL UpdateBasePolicyRequest in body
 
         base_policy_id: (basePolicyId) REQUIRED str in path
 
     Responses:
         200: OK - UpdateBasePolicyResponse (successful operation)
@@ -69,32 +63,44 @@
 
         404: Not Found - ErrorEntity (40030: errors.net.accelbyte.platform.legal.policy_type_not_exist)
     """
 
     # region fields
 
     _url: str = "/agreement/admin/base-policies/{basePolicyId}"
+    _path: str = "/agreement/admin/base-policies/{basePolicyId}"
+    _base_path: str = ""
     _method: str = "PATCH"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
-    _securities: List[List[str]] = [["BEARER_AUTH"], ["BEARER_AUTH"]]
+    _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "legal"
+
     body: UpdateBasePolicyRequest  # OPTIONAL in [body]
     base_policy_id: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/base_legal_policies/retrieve_all_legal_policies.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/policies/retrieve_country_list_w_8c69ff.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,63 +25,68 @@
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
-from ...models import RetrieveBasePolicyResponse
 
+class RetrieveCountryListWithPolicies(Operation):
+    """Retrieve List of Countries that have Active Legal Policies (retrieveCountryListWithPolicies)
 
-class RetrieveAllLegalPolicies(Operation):
-    """Retrieve All Base Legal Policy (retrieveAllLegalPolicies)
-
-    Retrieve all base policies.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:*:LEGAL", action=2 (READ)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:*:LEGAL [READ]
+    Retrieve List of Countries that have Active Legal Policies.
 
     Properties:
-        url: /agreement/admin/base-policies
+        url: /agreement/public/policies/countries/list
 
         method: GET
 
-        tags: ["Base Legal Policies"]
+        tags: ["Policies"]
 
         consumes: []
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
+
 
     Responses:
-        200: OK - List[RetrieveBasePolicyResponse] (successful operation)
+        200: OK - List[str] (successful operation)
     """
 
     # region fields
 
-    _url: str = "/agreement/admin/base-policies"
+    _url: str = "/agreement/public/policies/countries/list"
+    _path: str = "/agreement/public/policies/countries/list"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
-    _securities: List[List[str]] = [["BEARER_AUTH"], ["BEARER_AUTH"]]
+    _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "legal"
+
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
 
@@ -127,20 +132,18 @@
     # endregion to methods
 
     # region response methods
 
     # noinspection PyMethodMayBeStatic
     def parse_response(
         self, code: int, content_type: str, content: Any
-    ) -> Tuple[
-        Union[None, List[RetrieveBasePolicyResponse]], Union[None, HttpResponse]
-    ]:
+    ) -> Tuple[Union[None, List[str]], Union[None, HttpResponse]]:
         """Parse the given response.
 
-        200: OK - List[RetrieveBasePolicyResponse] (successful operation)
+        200: OK - List[str] (successful operation)
 
         ---: HttpResponse (Undocumented Response)
 
         ---: HttpResponse (Unexpected Content-Type Error)
 
         ---: HttpResponse (Unhandled Error)
         """
@@ -148,37 +151,35 @@
             code=code, content_type=content_type, content=content
         )
         if error is not None:
             return None, None if error.is_no_content() else error
         code, content_type, content = pre_processed_response
 
         if code == 200:
-            return [
-                RetrieveBasePolicyResponse.create_from_dict(i) for i in content
-            ], None
+            return [str(i) for i in content], None
 
         return self.handle_undocumented_response(
             code=code, content_type=content_type, content=content
         )
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
-    def create(cls, **kwargs) -> RetrieveAllLegalPolicies:
+    def create(cls, **kwargs) -> RetrieveCountryListWithPolicies:
         instance = cls()
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> RetrieveAllLegalPolicies:
+    ) -> RetrieveCountryListWithPolicies:
         instance = cls()
         return instance
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {}
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/base_legal_policies/retrieve_all_policy_types.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/base_legal_policies/retrieve_all_policy_types.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,63 +32,69 @@
 from ...models import RetrievePolicyTypeResponse
 
 
 class RetrieveAllPolicyTypes(Operation):
     """Retrieve All Policy Type (retrieveAllPolicyTypes)
 
     Retrieve all supported policy types.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:*:LEGAL", action=2 (READ)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:*:LEGAL [READ]
 
     Properties:
         url: /agreement/admin/policy-types
 
         method: GET
 
         tags: ["Base Legal Policies"]
 
         consumes: []
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         offset: (offset) OPTIONAL int in query
 
         limit: (limit) REQUIRED int in query
 
     Responses:
         200: OK - List[RetrievePolicyTypeResponse] (successful operation)
     """
 
     # region fields
 
     _url: str = "/agreement/admin/policy-types"
+    _path: str = "/agreement/admin/policy-types"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
-    _securities: List[List[str]] = [["BEARER_AUTH"], ["BEARER_AUTH"]]
+    _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "legal"
+
     offset: int  # OPTIONAL in [query]
     limit: int  # REQUIRED in [query]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/base_legal_policies/retrieve_policy_country.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/base_legal_policies/retrieve_policy_country.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,65 +33,71 @@
 from ...models import RetrievePolicyResponse
 
 
 class RetrievePolicyCountry(Operation):
     """Retrieve a Base Legal Policy based on a Particular Country (retrievePolicyCountry)
 
     Retrieve a Base Legal Policy based on a Particular Country.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:*:LEGAL", action=2 (READ)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:*:LEGAL [READ]
 
     Properties:
         url: /agreement/admin/base-policies/{basePolicyId}/countries/{countryCode}
 
         method: GET
 
         tags: ["Base Legal Policies"]
 
         consumes: []
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         base_policy_id: (basePolicyId) REQUIRED str in path
 
         country_code: (countryCode) REQUIRED str in path
 
     Responses:
         200: OK - RetrievePolicyResponse (successful operation)
 
         404: Not Found - ErrorEntity (40041: errors.net.accelbyte.platform.legal.policy_not_found)
     """
 
     # region fields
 
     _url: str = "/agreement/admin/base-policies/{basePolicyId}/countries/{countryCode}"
+    _path: str = "/agreement/admin/base-policies/{basePolicyId}/countries/{countryCode}"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
-    _securities: List[List[str]] = [["BEARER_AUTH"], ["BEARER_AUTH"]]
+    _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "legal"
+
     base_policy_id: str  # REQUIRED in [path]
     country_code: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/base_legal_policies/retrieve_single_policy.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/policies/set_default_policy_2.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,69 +26,74 @@
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
 from ...models import ErrorEntity
-from ...models import RetrieveBasePolicyResponse
 
 
-class RetrieveSinglePolicy(Operation):
-    """Retrieve a Base Legal Policy (retrieveSinglePolicy)
+class SetDefaultPolicy2(Operation):
+    """Set Default Policy (setDefaultPolicy_2)
 
-    Retrieve a base policy.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:*:LEGAL", action=2 (READ)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:*:LEGAL [READ]
+    Update a policy to be the default.
 
     Properties:
-        url: /agreement/admin/base-policies/{basePolicyId}
+        url: /agreement/admin/policies/{policyId}/default
 
-        method: GET
+        method: PATCH
 
-        tags: ["Base Legal Policies"]
+        tags: ["Policies"]
 
         consumes: []
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
-        base_policy_id: (basePolicyId) REQUIRED str in path
+        policy_id: (policyId) REQUIRED str in path
 
     Responses:
-        200: OK - RetrieveBasePolicyResponse (successful operation)
+        200: OK - (operation successful)
 
-        404: Not Found - ErrorEntity (40031: errors.net.accelbyte.platform.legal.base_policy_not_found)
+        400: Bad Request - ErrorEntity (40033: errors.net.accelbyte.platform.legal.invalid_policy_id)
     """
 
     # region fields
 
-    _url: str = "/agreement/admin/base-policies/{basePolicyId}"
-    _method: str = "GET"
+    _url: str = "/agreement/admin/policies/{policyId}/default"
+    _path: str = "/agreement/admin/policies/{policyId}/default"
+    _base_path: str = ""
+    _method: str = "PATCH"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
-    _securities: List[List[str]] = [["BEARER_AUTH"], ["BEARER_AUTH"]]
+    _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
-    base_policy_id: str  # REQUIRED in [path]
+    service_name: Optional[str] = "legal"
+
+    policy_id: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
 
@@ -115,57 +120,55 @@
     def get_all_params(self) -> dict:
         return {
             "path": self.get_path_params(),
         }
 
     def get_path_params(self) -> dict:
         result = {}
-        if hasattr(self, "base_policy_id"):
-            result["basePolicyId"] = self.base_policy_id
+        if hasattr(self, "policy_id"):
+            result["policyId"] = self.policy_id
         return result
 
     # endregion get_x_params methods
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_base_policy_id(self, value: str) -> RetrieveSinglePolicy:
-        self.base_policy_id = value
+    def with_policy_id(self, value: str) -> SetDefaultPolicy2:
+        self.policy_id = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
-        if hasattr(self, "base_policy_id") and self.base_policy_id:
-            result["basePolicyId"] = str(self.base_policy_id)
+        if hasattr(self, "policy_id") and self.policy_id:
+            result["policyId"] = str(self.policy_id)
         elif include_empty:
-            result["basePolicyId"] = ""
+            result["policyId"] = ""
         return result
 
     # endregion to methods
 
     # region response methods
 
     # noinspection PyMethodMayBeStatic
     def parse_response(
         self, code: int, content_type: str, content: Any
-    ) -> Tuple[
-        Union[None, RetrieveBasePolicyResponse], Union[None, ErrorEntity, HttpResponse]
-    ]:
+    ) -> Tuple[Union[None, HttpResponse], Union[None, ErrorEntity, HttpResponse]]:
         """Parse the given response.
 
-        200: OK - RetrieveBasePolicyResponse (successful operation)
+        200: OK - (operation successful)
 
-        404: Not Found - ErrorEntity (40031: errors.net.accelbyte.platform.legal.base_policy_not_found)
+        400: Bad Request - ErrorEntity (40033: errors.net.accelbyte.platform.legal.invalid_policy_id)
 
         ---: HttpResponse (Undocumented Response)
 
         ---: HttpResponse (Unexpected Content-Type Error)
 
         ---: HttpResponse (Unhandled Error)
         """
@@ -173,51 +176,51 @@
             code=code, content_type=content_type, content=content
         )
         if error is not None:
             return None, None if error.is_no_content() else error
         code, content_type, content = pre_processed_response
 
         if code == 200:
-            return RetrieveBasePolicyResponse.create_from_dict(content), None
-        if code == 404:
+            return HttpResponse.create(code, "OK"), None
+        if code == 400:
             return None, ErrorEntity.create_from_dict(content)
 
         return self.handle_undocumented_response(
             code=code, content_type=content_type, content=content
         )
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
-    def create(cls, base_policy_id: str, **kwargs) -> RetrieveSinglePolicy:
+    def create(cls, policy_id: str, **kwargs) -> SetDefaultPolicy2:
         instance = cls()
-        instance.base_policy_id = base_policy_id
+        instance.policy_id = policy_id
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> RetrieveSinglePolicy:
+    ) -> SetDefaultPolicy2:
         instance = cls()
-        if "basePolicyId" in dict_ and dict_["basePolicyId"] is not None:
-            instance.base_policy_id = str(dict_["basePolicyId"])
+        if "policyId" in dict_ and dict_["policyId"] is not None:
+            instance.policy_id = str(dict_["policyId"])
         elif include_empty:
-            instance.base_policy_id = ""
+            instance.policy_id = ""
         return instance
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
-            "basePolicyId": "base_policy_id",
+            "policyId": "policy_id",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
-            "basePolicyId": True,
+            "policyId": True,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/base_legal_policies_with_namespace/__init__.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/base_legal_policies_with_namespace/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Legal Service."""
 
-__version__ = "1.39.0"
+__version__ = "1.41.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .create_policy_1 import CreatePolicy1
 from .partial_update_policy_1 import PartialUpdatePolicy1
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/base_legal_policies_with_namespace/create_policy_1.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/base_legal_policies_with_namespace/create_policy_1.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,33 +35,27 @@
 from ...models import ValidationErrorEntity
 
 
 class CreatePolicy1(Operation):
     """Create a Base Legal Policy (createPolicy_1)
 
     Create a legal policy.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:{namespace}:LEGAL", action=1 (CREATE)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:LEGAL [CREATE]
 
     Properties:
         url: /agreement/admin/namespaces/{namespace}/base-policies
 
         method: POST
 
         tags: ["Base Legal Policies With Namespace"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         body: (body) OPTIONAL CreateBasePolicyRequestV2 in body
 
         namespace: (namespace) REQUIRED str in path
 
     Responses:
         201: Created - CreateBasePolicyResponse (successful operation)
@@ -72,32 +66,44 @@
 
         422: Unprocessable Entity - ValidationErrorEntity (20002: validation error)
     """
 
     # region fields
 
     _url: str = "/agreement/admin/namespaces/{namespace}/base-policies"
+    _path: str = "/agreement/admin/namespaces/{namespace}/base-policies"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
-    _securities: List[List[str]] = [["BEARER_AUTH"], ["BEARER_AUTH"]]
+    _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "legal"
+
     body: CreateBasePolicyRequestV2  # OPTIONAL in [body]
     namespace: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/base_legal_policies_with_namespace/partial_update_policy_1.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/base_legal_policies_with_namespace/partial_update_policy_1.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,33 +34,27 @@
 from ...models import UpdateBasePolicyResponse
 
 
 class PartialUpdatePolicy1(Operation):
     """Update Base Legal Policy (partialUpdatePolicy_1)
 
     Update an existing base policy.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:{namespace}:LEGAL", action=4 (UPDATE)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:LEGAL [UPDATE]
 
     Properties:
         url: /agreement/admin/namespaces/{namespace}/base-policies/{basePolicyId}
 
         method: PATCH
 
         tags: ["Base Legal Policies With Namespace"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         body: (body) OPTIONAL UpdateBasePolicyRequestV2 in body
 
         base_policy_id: (basePolicyId) REQUIRED str in path
 
         namespace: (namespace) REQUIRED str in path
 
@@ -69,33 +63,45 @@
 
         400: Bad Request - ErrorEntity (40032: errors.net.accelbyte.platform.legal.invalid_base_policy)
     """
 
     # region fields
 
     _url: str = "/agreement/admin/namespaces/{namespace}/base-policies/{basePolicyId}"
+    _path: str = "/agreement/admin/namespaces/{namespace}/base-policies/{basePolicyId}"
+    _base_path: str = ""
     _method: str = "PATCH"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
-    _securities: List[List[str]] = [["BEARER_AUTH"], ["BEARER_AUTH"]]
+    _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "legal"
+
     body: UpdateBasePolicyRequestV2  # OPTIONAL in [body]
     base_policy_id: str  # REQUIRED in [path]
     namespace: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/base_legal_policies_with_namespace/retrieve_all_legal_poli_23dd4c.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/base_legal_policies_with_namespace/retrieve_all_legal_poli_23dd4c.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,60 +32,66 @@
 from ...models import RetrieveBasePolicyResponse
 
 
 class RetrieveAllLegalPoliciesByNamespace(Operation):
     """Retrieve All Base Legal Policy in the namespace (retrieveAllLegalPoliciesByNamespace)
 
     Retrieve all base policies in the namespace.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:{namespace}:LEGAL", action=2 (READ)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:LEGAL [READ]
 
     Properties:
         url: /agreement/admin/namespaces/{namespace}/base-policies
 
         method: GET
 
         tags: ["Base Legal Policies With Namespace"]
 
         consumes: []
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         namespace: (namespace) REQUIRED str in path
 
     Responses:
         200: OK - List[RetrieveBasePolicyResponse] (successful operation)
     """
 
     # region fields
 
     _url: str = "/agreement/admin/namespaces/{namespace}/base-policies"
+    _path: str = "/agreement/admin/namespaces/{namespace}/base-policies"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
-    _securities: List[List[str]] = [["BEARER_AUTH"], ["BEARER_AUTH"]]
+    _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "legal"
+
     namespace: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/base_legal_policies_with_namespace/retrieve_all_policy_types_1.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/base_legal_policies_with_namespace/retrieve_all_policy_types_1.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,66 +32,72 @@
 from ...models import RetrievePolicyTypeResponse
 
 
 class RetrieveAllPolicyTypes1(Operation):
     """Retrieve All Policy Type (retrieveAllPolicyTypes_1)
 
     Retrieve all supported policy types.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:{namespace}:LEGAL", action=2 (READ)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:LEGAL [READ]
 
     Properties:
         url: /agreement/admin/namespaces/{namespace}/policy-types
 
         method: GET
 
         tags: ["Base Legal Policies With Namespace"]
 
         consumes: []
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         namespace: (namespace) REQUIRED str in path
 
         offset: (offset) OPTIONAL int in query
 
         limit: (limit) REQUIRED int in query
 
     Responses:
         200: OK - List[RetrievePolicyTypeResponse] (successful operation)
     """
 
     # region fields
 
     _url: str = "/agreement/admin/namespaces/{namespace}/policy-types"
+    _path: str = "/agreement/admin/namespaces/{namespace}/policy-types"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
-    _securities: List[List[str]] = [["BEARER_AUTH"], ["BEARER_AUTH"]]
+    _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "legal"
+
     namespace: str  # REQUIRED in [path]
     offset: int  # OPTIONAL in [query]
     limit: int  # REQUIRED in [query]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/base_legal_policies_with_namespace/retrieve_policy_country_1.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/base_legal_policies_with_namespace/retrieve_policy_country_1.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,33 +33,27 @@
 from ...models import RetrievePolicyResponse
 
 
 class RetrievePolicyCountry1(Operation):
     """Retrieve a Base Legal Policy based on a Particular Country (retrievePolicyCountry_1)
 
     Retrieve a Base Legal Policy based on a Particular Country.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:{namespace}:LEGAL", action=2 (READ)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:LEGAL [READ]
 
     Properties:
         url: /agreement/admin/namespaces/{namespace}/base-policies/{basePolicyId}/countries/{countryCode}
 
         method: GET
 
         tags: ["Base Legal Policies With Namespace"]
 
         consumes: []
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         base_policy_id: (basePolicyId) REQUIRED str in path
 
         country_code: (countryCode) REQUIRED str in path
 
         namespace: (namespace) REQUIRED str in path
 
@@ -68,33 +62,45 @@
 
         404: Not Found - ErrorEntity (40031: errors.net.accelbyte.platform.legal.base_policy_not_found)
     """
 
     # region fields
 
     _url: str = "/agreement/admin/namespaces/{namespace}/base-policies/{basePolicyId}/countries/{countryCode}"
+    _path: str = "/agreement/admin/namespaces/{namespace}/base-policies/{basePolicyId}/countries/{countryCode}"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
-    _securities: List[List[str]] = [["BEARER_AUTH"], ["BEARER_AUTH"]]
+    _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "legal"
+
     base_policy_id: str  # REQUIRED in [path]
     country_code: str  # REQUIRED in [path]
     namespace: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/base_legal_policies_with_namespace/retrieve_single_policy_1.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/base_legal_policies_with_namespace/retrieve_single_policy_1.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,65 +33,71 @@
 from ...models import RetrieveBasePolicyResponse
 
 
 class RetrieveSinglePolicy1(Operation):
     """Retrieve a Base Legal Policy (retrieveSinglePolicy_1)
 
     Retrieve a base policy.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:{namespace}:LEGAL", action=2 (READ)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:LEGAL [READ]
 
     Properties:
         url: /agreement/admin/namespaces/{namespace}/base-policies/{basePolicyId}
 
         method: GET
 
         tags: ["Base Legal Policies With Namespace"]
 
         consumes: []
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         base_policy_id: (basePolicyId) REQUIRED str in path
 
         namespace: (namespace) REQUIRED str in path
 
     Responses:
         200: OK - RetrieveBasePolicyResponse (successful operation)
 
         404: Not Found - ErrorEntity (40041: errors.net.accelbyte.platform.legal.policy_not_found)
     """
 
     # region fields
 
     _url: str = "/agreement/admin/namespaces/{namespace}/base-policies/{basePolicyId}"
+    _path: str = "/agreement/admin/namespaces/{namespace}/base-policies/{basePolicyId}"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
-    _securities: List[List[str]] = [["BEARER_AUTH"], ["BEARER_AUTH"]]
+    _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "legal"
+
     base_policy_id: str  # REQUIRED in [path]
     namespace: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/eligibilities/__init__.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/eligibilities/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Legal Service."""
 
-__version__ = "1.39.0"
+__version__ = "1.41.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .retrieve_eligibilities_public import RetrieveEligibilitiesPublic
 from .retrieve_eligibilities__345271 import RetrieveEligibilitiesPublicIndirect
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/eligibilities/retrieve_eligibilities__345271.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/eligibilities/retrieve_eligibilities__345271.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,18 +35,14 @@
 
 class RetrieveEligibilitiesPublicIndirect(Operation):
     """Check User Legal Eligibility (retrieveEligibilitiesPublicIndirect)
 
     Retrieve the active policies and its conformance status by user.
     This process only supports cross-namespace checking between game namespace and publisher namespace , that means if the active policy already accepted by the same user in publisher namespace, then it will also be considered as eligible in non-publisher namespace.
 
-    Other detail info:
-
-      * Required permission : login user
-
     Properties:
         url: /agreement/public/eligibilities/namespaces/{namespace}/countries/{countryCode}/clients/{clientId}/users/{userId}
 
         method: GET
 
         tags: ["Eligibilities"]
 
@@ -69,34 +65,46 @@
 
         400: Bad Request - ErrorEntity (40045: errors.net.accelbyte.platform.legal.user_id_needed)
     """
 
     # region fields
 
     _url: str = "/agreement/public/eligibilities/namespaces/{namespace}/countries/{countryCode}/clients/{clientId}/users/{userId}"
+    _path: str = "/agreement/public/eligibilities/namespaces/{namespace}/countries/{countryCode}/clients/{clientId}/users/{userId}"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "legal"
+
     client_id: str  # REQUIRED in [path]
     country_code: str  # REQUIRED in [path]
     namespace: str  # REQUIRED in [path]
     user_id: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/eligibilities/retrieve_eligibilities_public.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/eligibilities/retrieve_eligibilities_public.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,18 +35,14 @@
 
 class RetrieveEligibilitiesPublic(Operation):
     """Check User Legal Eligibility (retrieveEligibilitiesPublic)
 
     Retrieve the active policies and its conformance status by user.
     This process supports cross-namespace checking, that means if the active policy already accepted by the same user in other namespace, then it will be considered as eligible.
 
-    Other detail info:
-
-      * Required permission : login user
-
     Properties:
         url: /agreement/public/eligibilities/namespaces/{namespace}
 
         method: GET
 
         tags: ["Eligibilities"]
 
@@ -65,31 +61,43 @@
 
         404: Not Found - ErrorEntity (40041: errors.net.accelbyte.platform.legal.policy_not_found)
     """
 
     # region fields
 
     _url: str = "/agreement/public/eligibilities/namespaces/{namespace}"
+    _path: str = "/agreement/public/eligibilities/namespaces/{namespace}"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "legal"
+
     namespace: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/localized_policy_versions/__init__.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/localized_policy_versions/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Legal Service."""
 
-__version__ = "1.39.0"
+__version__ = "1.41.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .create_localized_policy_19e4a3 import CreateLocalizedPolicyVersion
 from .request_presigned_url import RequestPresignedURL
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/localized_policy_versions/create_localized_policy_19e4a3.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/localized_policy_versions/create_localized_policy_19e4a3.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,33 +34,27 @@
 from ...models import ErrorEntity
 
 
 class CreateLocalizedPolicyVersion(Operation):
     """Create a Localized Version from Country-Specific Policy (createLocalizedPolicyVersion)
 
     Create a version of a particular country-specific policy.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:*:LEGAL", action=1 (CREATE)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:*:LEGAL [CREATE]
 
     Properties:
         url: /agreement/admin/localized-policy-versions/versions/{policyVersionId}
 
         method: POST
 
         tags: ["Localized Policy Versions"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         body: (body) OPTIONAL CreateLocalizedPolicyVersionRequest in body
 
         policy_version_id: (policyVersionId) REQUIRED str in path
 
     Responses:
         201: Created - CreateLocalizedPolicyVersionResponse (successful operation)
@@ -69,32 +63,44 @@
 
         409: Conflict - ErrorEntity (40044: errors.net.accelbyte.platform.legal.localized_policy_version_already_exist)
     """
 
     # region fields
 
     _url: str = "/agreement/admin/localized-policy-versions/versions/{policyVersionId}"
+    _path: str = "/agreement/admin/localized-policy-versions/versions/{policyVersionId}"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
-    _securities: List[List[str]] = [["BEARER_AUTH"], ["BEARER_AUTH"]]
+    _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "legal"
+
     body: CreateLocalizedPolicyVersionRequest  # OPTIONAL in [body]
     policy_version_id: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/localized_policy_versions/request_presigned_url.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/localized_policy_versions/request_presigned_url.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,65 +34,71 @@
 from ...models import UploadPolicyVersionAttachmentRequest
 
 
 class RequestPresignedURL(Operation):
     """Request Presigned URL for Upload Document (requestPresignedURL)
 
     Request presigned URL for upload attachment for a particular localized version of base policy.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:*:LEGAL", action=1 (CREATE)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:*:LEGAL [CREATE]
 
     Properties:
         url: /agreement/admin/localized-policy-versions/{localizedPolicyVersionId}/attachments
 
         method: POST
 
         tags: ["Localized Policy Versions"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         body: (body) OPTIONAL UploadPolicyVersionAttachmentRequest in body
 
         localized_policy_version_id: (localizedPolicyVersionId) REQUIRED str in path
 
     Responses:
         201: Created - UploadLocalizedPolicyVersionAttachmentResponse (successful operation)
 
         400: Bad Request - ErrorEntity (40034: errors.net.accelbyte.platform.legal.invalid_file_type | 40037: errors.net.accelbyte.platform.legal.invalid_localized_policy_version | 40042: errors.net.accelbyte.platform.legal.policy_version_freezed)
     """
 
     # region fields
 
     _url: str = "/agreement/admin/localized-policy-versions/{localizedPolicyVersionId}/attachments"
+    _path: str = "/agreement/admin/localized-policy-versions/{localizedPolicyVersionId}/attachments"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
-    _securities: List[List[str]] = [["BEARER_AUTH"], ["BEARER_AUTH"]]
+    _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "legal"
+
     body: UploadPolicyVersionAttachmentRequest  # OPTIONAL in [body]
     localized_policy_version_id: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/localized_policy_versions/retrieve_localized_poli_24a671.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/localized_policy_versions/retrieve_single_localiz_2f6231.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,67 +25,76 @@
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
+from ...models import ErrorEntity
 from ...models import RetrieveLocalizedPolicyVersionResponse
 
 
-class RetrieveLocalizedPolicyVersions(Operation):
-    """Retrieve Versions from Country-Specific Policy (retrieveLocalizedPolicyVersions)
+class RetrieveSingleLocalizedPolicyVersion(Operation):
+    """Retrieve a Localized Version from Country-Specific Policy (retrieveSingleLocalizedPolicyVersion)
 
-    Retrieve versions of a particular country-specific policy.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:*:LEGAL", action=2 (READ)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:*:LEGAL [READ]
+    Retrieve a version of a particular country-specific policy.
 
     Properties:
-        url: /agreement/admin/localized-policy-versions/versions/{policyVersionId}
+        url: /agreement/admin/localized-policy-versions/{localizedPolicyVersionId}
 
         method: GET
 
         tags: ["Localized Policy Versions"]
 
         consumes: []
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
-        policy_version_id: (policyVersionId) REQUIRED str in path
+        localized_policy_version_id: (localizedPolicyVersionId) REQUIRED str in path
 
     Responses:
-        200: OK - List[RetrieveLocalizedPolicyVersionResponse] (successful operation)
+        200: OK - RetrieveLocalizedPolicyVersionResponse (successful operation)
+
+        404: Not Found - ErrorEntity (2912: errors.net.accelbyte.platform.legal.policy_version_not_found)
     """
 
     # region fields
 
-    _url: str = "/agreement/admin/localized-policy-versions/versions/{policyVersionId}"
+    _url: str = "/agreement/admin/localized-policy-versions/{localizedPolicyVersionId}"
+    _path: str = "/agreement/admin/localized-policy-versions/{localizedPolicyVersionId}"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
-    _securities: List[List[str]] = [["BEARER_AUTH"], ["BEARER_AUTH"]]
+    _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
-    policy_version_id: str  # REQUIRED in [path]
+    service_name: Optional[str] = "legal"
+
+    localized_policy_version_id: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
 
@@ -112,56 +121,63 @@
     def get_all_params(self) -> dict:
         return {
             "path": self.get_path_params(),
         }
 
     def get_path_params(self) -> dict:
         result = {}
-        if hasattr(self, "policy_version_id"):
-            result["policyVersionId"] = self.policy_version_id
+        if hasattr(self, "localized_policy_version_id"):
+            result["localizedPolicyVersionId"] = self.localized_policy_version_id
         return result
 
     # endregion get_x_params methods
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_policy_version_id(self, value: str) -> RetrieveLocalizedPolicyVersions:
-        self.policy_version_id = value
+    def with_localized_policy_version_id(
+        self, value: str
+    ) -> RetrieveSingleLocalizedPolicyVersion:
+        self.localized_policy_version_id = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
-        if hasattr(self, "policy_version_id") and self.policy_version_id:
-            result["policyVersionId"] = str(self.policy_version_id)
+        if (
+            hasattr(self, "localized_policy_version_id")
+            and self.localized_policy_version_id
+        ):
+            result["localizedPolicyVersionId"] = str(self.localized_policy_version_id)
         elif include_empty:
-            result["policyVersionId"] = ""
+            result["localizedPolicyVersionId"] = ""
         return result
 
     # endregion to methods
 
     # region response methods
 
     # noinspection PyMethodMayBeStatic
     def parse_response(
         self, code: int, content_type: str, content: Any
     ) -> Tuple[
-        Union[None, List[RetrieveLocalizedPolicyVersionResponse]],
-        Union[None, HttpResponse],
+        Union[None, RetrieveLocalizedPolicyVersionResponse],
+        Union[None, ErrorEntity, HttpResponse],
     ]:
         """Parse the given response.
 
-        200: OK - List[RetrieveLocalizedPolicyVersionResponse] (successful operation)
+        200: OK - RetrieveLocalizedPolicyVersionResponse (successful operation)
+
+        404: Not Found - ErrorEntity (2912: errors.net.accelbyte.platform.legal.policy_version_not_found)
 
         ---: HttpResponse (Undocumented Response)
 
         ---: HttpResponse (Unexpected Content-Type Error)
 
         ---: HttpResponse (Unhandled Error)
         """
@@ -169,54 +185,61 @@
             code=code, content_type=content_type, content=content
         )
         if error is not None:
             return None, None if error.is_no_content() else error
         code, content_type, content = pre_processed_response
 
         if code == 200:
-            return [
-                RetrieveLocalizedPolicyVersionResponse.create_from_dict(i)
-                for i in content
-            ], None
+            return (
+                RetrieveLocalizedPolicyVersionResponse.create_from_dict(content),
+                None,
+            )
+        if code == 404:
+            return None, ErrorEntity.create_from_dict(content)
 
         return self.handle_undocumented_response(
             code=code, content_type=content_type, content=content
         )
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
     def create(
-        cls, policy_version_id: str, **kwargs
-    ) -> RetrieveLocalizedPolicyVersions:
+        cls, localized_policy_version_id: str, **kwargs
+    ) -> RetrieveSingleLocalizedPolicyVersion:
         instance = cls()
-        instance.policy_version_id = policy_version_id
+        instance.localized_policy_version_id = localized_policy_version_id
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> RetrieveLocalizedPolicyVersions:
+    ) -> RetrieveSingleLocalizedPolicyVersion:
         instance = cls()
-        if "policyVersionId" in dict_ and dict_["policyVersionId"] is not None:
-            instance.policy_version_id = str(dict_["policyVersionId"])
+        if (
+            "localizedPolicyVersionId" in dict_
+            and dict_["localizedPolicyVersionId"] is not None
+        ):
+            instance.localized_policy_version_id = str(
+                dict_["localizedPolicyVersionId"]
+            )
         elif include_empty:
-            instance.policy_version_id = ""
+            instance.localized_policy_version_id = ""
         return instance
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
-            "policyVersionId": "policy_version_id",
+            "localizedPolicyVersionId": "localized_policy_version_id",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
-            "policyVersionId": True,
+            "localizedPolicyVersionId": True,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/localized_policy_versions/retrieve_single_localiz_2f6231.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/localized_policy_versions_with_namespace/retrieve_single_localiz_480659.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,69 +26,80 @@
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
 from ...models import ErrorEntity
-from ...models import RetrieveLocalizedPolicyVersionResponse
+from ...models import RetrieveLocalizedPolicyVersionPublicResponse
 
 
-class RetrieveSingleLocalizedPolicyVersion(Operation):
-    """Retrieve a Localized Version from Country-Specific Policy (retrieveSingleLocalizedPolicyVersion)
+class RetrieveSingleLocalizedPolicyVersion3(Operation):
+    """Retrieve a Localized Version (retrieveSingleLocalizedPolicyVersion_3)
 
-    Retrieve a version of a particular country-specific policy.
+    Retrieve specific localized policy version including the policy version and base policy version where the localized policy version located.
     Other detail info:
 
-      * Required permission : resource="ADMIN:NAMESPACE:*:LEGAL", action=2 (READ)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:*:LEGAL [READ]
-
     Properties:
-        url: /agreement/admin/localized-policy-versions/{localizedPolicyVersionId}
+        url: /agreement/public/namespaces/{namespace}/localized-policy-versions/{localizedPolicyVersionId}
 
         method: GET
 
-        tags: ["Localized Policy Versions"]
+        tags: ["Localized Policy Versions With Namespace"]
 
         consumes: []
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
+
 
         localized_policy_version_id: (localizedPolicyVersionId) REQUIRED str in path
 
+        namespace: (namespace) REQUIRED str in path
+
     Responses:
-        200: OK - RetrieveLocalizedPolicyVersionResponse (successful operation)
+        200: OK - RetrieveLocalizedPolicyVersionPublicResponse (successful operation)
 
-        404: Not Found - ErrorEntity (2912: errors.net.accelbyte.platform.legal.policy_version_not_found)
+        404: Not Found - ErrorEntity (40038: errors.net.accelbyte.platform.legal.localized_policy_version_not_found)
     """
 
     # region fields
 
-    _url: str = "/agreement/admin/localized-policy-versions/{localizedPolicyVersionId}"
+    _url: str = "/agreement/public/namespaces/{namespace}/localized-policy-versions/{localizedPolicyVersionId}"
+    _path: str = "/agreement/public/namespaces/{namespace}/localized-policy-versions/{localizedPolicyVersionId}"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
-    _securities: List[List[str]] = [["BEARER_AUTH"], ["BEARER_AUTH"]]
+    _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "legal"
+
     localized_policy_version_id: str  # REQUIRED in [path]
+    namespace: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
 
@@ -117,61 +128,71 @@
             "path": self.get_path_params(),
         }
 
     def get_path_params(self) -> dict:
         result = {}
         if hasattr(self, "localized_policy_version_id"):
             result["localizedPolicyVersionId"] = self.localized_policy_version_id
+        if hasattr(self, "namespace"):
+            result["namespace"] = self.namespace
         return result
 
     # endregion get_x_params methods
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
     def with_localized_policy_version_id(
         self, value: str
-    ) -> RetrieveSingleLocalizedPolicyVersion:
+    ) -> RetrieveSingleLocalizedPolicyVersion3:
         self.localized_policy_version_id = value
         return self
 
+    def with_namespace(self, value: str) -> RetrieveSingleLocalizedPolicyVersion3:
+        self.namespace = value
+        return self
+
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
         if (
             hasattr(self, "localized_policy_version_id")
             and self.localized_policy_version_id
         ):
             result["localizedPolicyVersionId"] = str(self.localized_policy_version_id)
         elif include_empty:
             result["localizedPolicyVersionId"] = ""
+        if hasattr(self, "namespace") and self.namespace:
+            result["namespace"] = str(self.namespace)
+        elif include_empty:
+            result["namespace"] = ""
         return result
 
     # endregion to methods
 
     # region response methods
 
     # noinspection PyMethodMayBeStatic
     def parse_response(
         self, code: int, content_type: str, content: Any
     ) -> Tuple[
-        Union[None, RetrieveLocalizedPolicyVersionResponse],
+        Union[None, RetrieveLocalizedPolicyVersionPublicResponse],
         Union[None, ErrorEntity, HttpResponse],
     ]:
         """Parse the given response.
 
-        200: OK - RetrieveLocalizedPolicyVersionResponse (successful operation)
+        200: OK - RetrieveLocalizedPolicyVersionPublicResponse (successful operation)
 
-        404: Not Found - ErrorEntity (2912: errors.net.accelbyte.platform.legal.policy_version_not_found)
+        404: Not Found - ErrorEntity (40038: errors.net.accelbyte.platform.legal.localized_policy_version_not_found)
 
         ---: HttpResponse (Undocumented Response)
 
         ---: HttpResponse (Unexpected Content-Type Error)
 
         ---: HttpResponse (Unhandled Error)
         """
@@ -180,15 +201,15 @@
         )
         if error is not None:
             return None, None if error.is_no_content() else error
         code, content_type, content = pre_processed_response
 
         if code == 200:
             return (
-                RetrieveLocalizedPolicyVersionResponse.create_from_dict(content),
+                RetrieveLocalizedPolicyVersionPublicResponse.create_from_dict(content),
                 None,
             )
         if code == 404:
             return None, ErrorEntity.create_from_dict(content)
 
         return self.handle_undocumented_response(
             code=code, content_type=content_type, content=content
@@ -196,44 +217,51 @@
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
     def create(
-        cls, localized_policy_version_id: str, **kwargs
-    ) -> RetrieveSingleLocalizedPolicyVersion:
+        cls, localized_policy_version_id: str, namespace: str, **kwargs
+    ) -> RetrieveSingleLocalizedPolicyVersion3:
         instance = cls()
         instance.localized_policy_version_id = localized_policy_version_id
+        instance.namespace = namespace
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> RetrieveSingleLocalizedPolicyVersion:
+    ) -> RetrieveSingleLocalizedPolicyVersion3:
         instance = cls()
         if (
             "localizedPolicyVersionId" in dict_
             and dict_["localizedPolicyVersionId"] is not None
         ):
             instance.localized_policy_version_id = str(
                 dict_["localizedPolicyVersionId"]
             )
         elif include_empty:
             instance.localized_policy_version_id = ""
+        if "namespace" in dict_ and dict_["namespace"] is not None:
+            instance.namespace = str(dict_["namespace"])
+        elif include_empty:
+            instance.namespace = ""
         return instance
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
             "localizedPolicyVersionId": "localized_policy_version_id",
+            "namespace": "namespace",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
             "localizedPolicyVersionId": True,
+            "namespace": True,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/localized_policy_versions/retrieve_single_localiz_6ecc81.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/localized_policy_versions/retrieve_single_localiz_6ecc81.py`

 * *Files 5% similar despite different names*

```diff
@@ -60,31 +60,45 @@
 
         404: Not Found - ErrorEntity (40038: errors.net.accelbyte.platform.legal.localized_policy_version_not_found)
     """
 
     # region fields
 
     _url: str = "/agreement/public/localized-policy-versions/{localizedPolicyVersionId}"
+    _path: str = (
+        "/agreement/public/localized-policy-versions/{localizedPolicyVersionId}"
+    )
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "legal"
+
     localized_policy_version_id: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/localized_policy_versions/set_default_policy.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/localized_policy_versions/set_default_policy.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,64 +32,72 @@
 from ...models import ErrorEntity
 
 
 class SetDefaultPolicy(Operation):
     """Set Default Localized Policy (setDefaultPolicy)
 
     Update a localized version policy to be the default.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:*:LEGAL", action=4 (UPDATE)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:*:LEGAL [UPDATE]
 
     Properties:
         url: /agreement/admin/localized-policy-versions/{localizedPolicyVersionId}/default
 
         method: PATCH
 
         tags: ["Localized Policy Versions"]
 
         consumes: []
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         localized_policy_version_id: (localizedPolicyVersionId) REQUIRED str in path
 
     Responses:
         200: OK - (Successful operation)
 
         400: Bad Request - ErrorEntity (40035: errors.net.accelbyte.platform.legal.invalid_localize_policy_version)
     """
 
     # region fields
 
     _url: str = (
         "/agreement/admin/localized-policy-versions/{localizedPolicyVersionId}/default"
     )
+    _path: str = (
+        "/agreement/admin/localized-policy-versions/{localizedPolicyVersionId}/default"
+    )
+    _base_path: str = ""
     _method: str = "PATCH"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
-    _securities: List[List[str]] = [["BEARER_AUTH"], ["BEARER_AUTH"]]
+    _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "legal"
+
     localized_policy_version_id: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/localized_policy_versions/update_localized_policy_a8a90f.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/localized_policy_versions/update_localized_policy_a8a90f.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,65 +34,71 @@
 from ...models import UpdateLocalizedPolicyVersionResponse
 
 
 class UpdateLocalizedPolicyVersion(Operation):
     """Update a Localized Version from Country-Specific Policy (updateLocalizedPolicyVersion)
 
     Update a version of a particular country-specific policy.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:*:LEGAL", action=4 (UPDATE)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:*:LEGAL [UPDATE]
 
     Properties:
         url: /agreement/admin/localized-policy-versions/{localizedPolicyVersionId}
 
         method: PUT
 
         tags: ["Localized Policy Versions"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         body: (body) OPTIONAL UpdateLocalizedPolicyVersionRequest in body
 
         localized_policy_version_id: (localizedPolicyVersionId) REQUIRED str in path
 
     Responses:
         200: OK - UpdateLocalizedPolicyVersionResponse (successful operation)
 
         400: Bad Request - ErrorEntity (40035: errors.net.accelbyte.platform.legal.invalid_policy_version)
     """
 
     # region fields
 
     _url: str = "/agreement/admin/localized-policy-versions/{localizedPolicyVersionId}"
+    _path: str = "/agreement/admin/localized-policy-versions/{localizedPolicyVersionId}"
+    _base_path: str = ""
     _method: str = "PUT"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
-    _securities: List[List[str]] = [["BEARER_AUTH"], ["BEARER_AUTH"]]
+    _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "legal"
+
     body: UpdateLocalizedPolicyVersionRequest  # OPTIONAL in [body]
     localized_policy_version_id: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/localized_policy_versions_with_namespace/__init__.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/localized_policy_versions_with_namespace/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Legal Service."""
 
-__version__ = "1.39.0"
+__version__ = "1.41.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .create_localized_policy_b58242 import CreateLocalizedPolicyVersion1
 from .request_presigned_url_1 import RequestPresignedURL1
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/localized_policy_versions_with_namespace/create_localized_policy_b58242.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/localized_policy_versions_with_namespace/create_localized_policy_b58242.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,33 +34,27 @@
 from ...models import ErrorEntity
 
 
 class CreateLocalizedPolicyVersion1(Operation):
     """Create a Localized Version from Country-Specific Policy (createLocalizedPolicyVersion_1)
 
     Create a version of a particular country-specific policy.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:{namespace}:LEGAL", action=1 (CREATE)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:LEGAL [CREATE]
 
     Properties:
         url: /agreement/admin/namespaces/{namespace}/localized-policy-versions/versions/{policyVersionId}
 
         method: POST
 
         tags: ["Localized Policy Versions With Namespace"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         body: (body) OPTIONAL CreateLocalizedPolicyVersionRequest in body
 
         namespace: (namespace) REQUIRED str in path
 
         policy_version_id: (policyVersionId) REQUIRED str in path
 
@@ -71,33 +65,45 @@
 
         409: Conflict - ErrorEntity (40044: errors.net.accelbyte.platform.legal.localized_policy_version_already_exist)
     """
 
     # region fields
 
     _url: str = "/agreement/admin/namespaces/{namespace}/localized-policy-versions/versions/{policyVersionId}"
+    _path: str = "/agreement/admin/namespaces/{namespace}/localized-policy-versions/versions/{policyVersionId}"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
-    _securities: List[List[str]] = [["BEARER_AUTH"], ["BEARER_AUTH"]]
+    _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "legal"
+
     body: CreateLocalizedPolicyVersionRequest  # OPTIONAL in [body]
     namespace: str  # REQUIRED in [path]
     policy_version_id: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/localized_policy_versions_with_namespace/request_presigned_url_1.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/localized_policy_versions_with_namespace/request_presigned_url_1.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,33 +34,27 @@
 from ...models import UploadPolicyVersionAttachmentRequest
 
 
 class RequestPresignedURL1(Operation):
     """Request Presigned URL for Upload Document (requestPresignedURL_1)
 
     Request presigned URL for upload attachment for a particular localized version of base policy.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:{namespace}:LEGAL", action=1 (CREATE)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:LEGAL [CREATE]
 
     Properties:
         url: /agreement/admin/namespaces/{namespace}/localized-policy-versions/{localizedPolicyVersionId}/attachments
 
         method: POST
 
         tags: ["Localized Policy Versions With Namespace"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         body: (body) OPTIONAL UploadPolicyVersionAttachmentRequest in body
 
         localized_policy_version_id: (localizedPolicyVersionId) REQUIRED str in path
 
         namespace: (namespace) REQUIRED str in path
 
@@ -69,33 +63,45 @@
 
         400: Bad Request - ErrorEntity (40034: errors.net.accelbyte.platform.legal.invalid_file_type | 40037: errors.net.accelbyte.platform.legal.invalid_localized_policy_version | 40042: errors.net.accelbyte.platform.legal.policy_version_freezed)
     """
 
     # region fields
 
     _url: str = "/agreement/admin/namespaces/{namespace}/localized-policy-versions/{localizedPolicyVersionId}/attachments"
+    _path: str = "/agreement/admin/namespaces/{namespace}/localized-policy-versions/{localizedPolicyVersionId}/attachments"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
-    _securities: List[List[str]] = [["BEARER_AUTH"], ["BEARER_AUTH"]]
+    _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "legal"
+
     body: UploadPolicyVersionAttachmentRequest  # OPTIONAL in [body]
     localized_policy_version_id: str  # REQUIRED in [path]
     namespace: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/localized_policy_versions_with_namespace/retrieve_localized_poli_4a4859.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/localized_policy_versions_with_namespace/retrieve_localized_poli_4a4859.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,63 +32,69 @@
 from ...models import RetrieveLocalizedPolicyVersionResponse
 
 
 class RetrieveLocalizedPolicyVersions1(Operation):
     """Retrieve Versions from Country-Specific Policy (retrieveLocalizedPolicyVersions_1)
 
     Retrieve versions of a particular country-specific policy.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:{namespace}:LEGAL", action=2 (READ)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:LEGAL [READ]
 
     Properties:
         url: /agreement/admin/namespaces/{namespace}/localized-policy-versions/versions/{policyVersionId}
 
         method: GET
 
         tags: ["Localized Policy Versions With Namespace"]
 
         consumes: []
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         namespace: (namespace) REQUIRED str in path
 
         policy_version_id: (policyVersionId) REQUIRED str in path
 
     Responses:
         200: OK - List[RetrieveLocalizedPolicyVersionResponse] (successful operation)
     """
 
     # region fields
 
     _url: str = "/agreement/admin/namespaces/{namespace}/localized-policy-versions/versions/{policyVersionId}"
+    _path: str = "/agreement/admin/namespaces/{namespace}/localized-policy-versions/versions/{policyVersionId}"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
-    _securities: List[List[str]] = [["BEARER_AUTH"], ["BEARER_AUTH"]]
+    _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "legal"
+
     namespace: str  # REQUIRED in [path]
     policy_version_id: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/localized_policy_versions_with_namespace/retrieve_single_localiz_480659.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/localized_policy_versions_with_namespace/retrieve_single_localiz_f21ac4.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,68 +26,78 @@
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
 from ...models import ErrorEntity
-from ...models import RetrieveLocalizedPolicyVersionPublicResponse
+from ...models import RetrieveLocalizedPolicyVersionResponse
 
 
-class RetrieveSingleLocalizedPolicyVersion3(Operation):
-    """Retrieve a Localized Version (retrieveSingleLocalizedPolicyVersion_3)
+class RetrieveSingleLocalizedPolicyVersion1(Operation):
+    """Retrieve a Localized Version from Country-Specific Policy (retrieveSingleLocalizedPolicyVersion_1)
 
-    Retrieve specific localized policy version including the policy version and base policy version where the localized policy version located.
-    Other detail info:
+    Retrieve a version of a particular country-specific policy.
 
     Properties:
-        url: /agreement/public/namespaces/{namespace}/localized-policy-versions/{localizedPolicyVersionId}
+        url: /agreement/admin/namespaces/{namespace}/localized-policy-versions/{localizedPolicyVersionId}
 
         method: GET
 
         tags: ["Localized Policy Versions With Namespace"]
 
         consumes: []
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
-
         localized_policy_version_id: (localizedPolicyVersionId) REQUIRED str in path
 
         namespace: (namespace) REQUIRED str in path
 
     Responses:
-        200: OK - RetrieveLocalizedPolicyVersionPublicResponse (successful operation)
+        200: OK - RetrieveLocalizedPolicyVersionResponse (successful operation)
 
-        404: Not Found - ErrorEntity (40038: errors.net.accelbyte.platform.legal.localized_policy_version_not_found)
+        404: Not Found - ErrorEntity (2912: errors.net.accelbyte.platform.legal.policy_version_not_found)
     """
 
     # region fields
 
-    _url: str = "/agreement/public/namespaces/{namespace}/localized-policy-versions/{localizedPolicyVersionId}"
+    _url: str = "/agreement/admin/namespaces/{namespace}/localized-policy-versions/{localizedPolicyVersionId}"
+    _path: str = "/agreement/admin/namespaces/{namespace}/localized-policy-versions/{localizedPolicyVersionId}"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "legal"
+
     localized_policy_version_id: str  # REQUIRED in [path]
     namespace: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
 
@@ -130,19 +140,19 @@
 
     # endregion is/has methods
 
     # region with_x methods
 
     def with_localized_policy_version_id(
         self, value: str
-    ) -> RetrieveSingleLocalizedPolicyVersion3:
+    ) -> RetrieveSingleLocalizedPolicyVersion1:
         self.localized_policy_version_id = value
         return self
 
-    def with_namespace(self, value: str) -> RetrieveSingleLocalizedPolicyVersion3:
+    def with_namespace(self, value: str) -> RetrieveSingleLocalizedPolicyVersion1:
         self.namespace = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
@@ -165,22 +175,22 @@
 
     # region response methods
 
     # noinspection PyMethodMayBeStatic
     def parse_response(
         self, code: int, content_type: str, content: Any
     ) -> Tuple[
-        Union[None, RetrieveLocalizedPolicyVersionPublicResponse],
+        Union[None, RetrieveLocalizedPolicyVersionResponse],
         Union[None, ErrorEntity, HttpResponse],
     ]:
         """Parse the given response.
 
-        200: OK - RetrieveLocalizedPolicyVersionPublicResponse (successful operation)
+        200: OK - RetrieveLocalizedPolicyVersionResponse (successful operation)
 
-        404: Not Found - ErrorEntity (40038: errors.net.accelbyte.platform.legal.localized_policy_version_not_found)
+        404: Not Found - ErrorEntity (2912: errors.net.accelbyte.platform.legal.policy_version_not_found)
 
         ---: HttpResponse (Undocumented Response)
 
         ---: HttpResponse (Unexpected Content-Type Error)
 
         ---: HttpResponse (Unhandled Error)
         """
@@ -189,15 +199,15 @@
         )
         if error is not None:
             return None, None if error.is_no_content() else error
         code, content_type, content = pre_processed_response
 
         if code == 200:
             return (
-                RetrieveLocalizedPolicyVersionPublicResponse.create_from_dict(content),
+                RetrieveLocalizedPolicyVersionResponse.create_from_dict(content),
                 None,
             )
         if code == 404:
             return None, ErrorEntity.create_from_dict(content)
 
         return self.handle_undocumented_response(
             code=code, content_type=content_type, content=content
@@ -206,26 +216,26 @@
     # endregion response methods
 
     # region static methods
 
     @classmethod
     def create(
         cls, localized_policy_version_id: str, namespace: str, **kwargs
-    ) -> RetrieveSingleLocalizedPolicyVersion3:
+    ) -> RetrieveSingleLocalizedPolicyVersion1:
         instance = cls()
         instance.localized_policy_version_id = localized_policy_version_id
         instance.namespace = namespace
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> RetrieveSingleLocalizedPolicyVersion3:
+    ) -> RetrieveSingleLocalizedPolicyVersion1:
         instance = cls()
         if (
             "localizedPolicyVersionId" in dict_
             and dict_["localizedPolicyVersionId"] is not None
         ):
             instance.localized_policy_version_id = str(
                 dict_["localizedPolicyVersionId"]
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/localized_policy_versions_with_namespace/retrieve_single_localiz_f21ac4.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/policy_versions/publish_policy_version.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,72 +26,79 @@
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
 from ...models import ErrorEntity
-from ...models import RetrieveLocalizedPolicyVersionResponse
 
 
-class RetrieveSingleLocalizedPolicyVersion1(Operation):
-    """Retrieve a Localized Version from Country-Specific Policy (retrieveSingleLocalizedPolicyVersion_1)
+class PublishPolicyVersion(Operation):
+    """Manually Publish a Version from Country-Specific Policy (publishPolicyVersion)
 
-    Retrieve a version of a particular country-specific policy.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:{namespace}:LEGAL", action=2 (READ)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:LEGAL [READ]
+    Manually publish a version of a particular country-specific policy.
 
     Properties:
-        url: /agreement/admin/namespaces/{namespace}/localized-policy-versions/{localizedPolicyVersionId}
+        url: /agreement/admin/policies/versions/{policyVersionId}/latest
 
-        method: GET
+        method: PATCH
 
-        tags: ["Localized Policy Versions With Namespace"]
+        tags: ["Policy Versions"]
 
         consumes: []
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
-        localized_policy_version_id: (localizedPolicyVersionId) REQUIRED str in path
+        policy_version_id: (policyVersionId) REQUIRED str in path
 
-        namespace: (namespace) REQUIRED str in path
+        should_notify: (shouldNotify) OPTIONAL bool in query
 
     Responses:
-        200: OK - RetrieveLocalizedPolicyVersionResponse (successful operation)
+        200: OK - (operation successful)
 
-        404: Not Found - ErrorEntity (2912: errors.net.accelbyte.platform.legal.policy_version_not_found)
+        400: Bad Request - ErrorEntity (40035: errors.net.accelbyte.platform.legal.invalid_policy_version | 40046: errors.net.accelbyte.platform.legal.default_selection_not_provided | 40030: errors.net.accelbyte.platform.legal.localized_policy_version_not_provided)
+
+        409: Conflict - ErrorEntity (40039: errors.net.accelbyte.platform.legal.localized_policy_version_already_latest | 40043: errors.net.accelbyte.platform.legal.localized_policy_version_already_publish)
     """
 
     # region fields
 
-    _url: str = "/agreement/admin/namespaces/{namespace}/localized-policy-versions/{localizedPolicyVersionId}"
-    _method: str = "GET"
+    _url: str = "/agreement/admin/policies/versions/{policyVersionId}/latest"
+    _path: str = "/agreement/admin/policies/versions/{policyVersionId}/latest"
+    _base_path: str = ""
+    _method: str = "PATCH"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
-    _securities: List[List[str]] = [["BEARER_AUTH"], ["BEARER_AUTH"]]
+    _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
-    localized_policy_version_id: str  # REQUIRED in [path]
-    namespace: str  # REQUIRED in [path]
+    service_name: Optional[str] = "legal"
+
+    policy_version_id: str  # REQUIRED in [path]
+    should_notify: bool  # OPTIONAL in [query]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
 
@@ -114,77 +121,76 @@
     # endregion get methods
 
     # region get_x_params methods
 
     def get_all_params(self) -> dict:
         return {
             "path": self.get_path_params(),
+            "query": self.get_query_params(),
         }
 
     def get_path_params(self) -> dict:
         result = {}
-        if hasattr(self, "localized_policy_version_id"):
-            result["localizedPolicyVersionId"] = self.localized_policy_version_id
-        if hasattr(self, "namespace"):
-            result["namespace"] = self.namespace
+        if hasattr(self, "policy_version_id"):
+            result["policyVersionId"] = self.policy_version_id
+        return result
+
+    def get_query_params(self) -> dict:
+        result = {}
+        if hasattr(self, "should_notify"):
+            result["shouldNotify"] = self.should_notify
         return result
 
     # endregion get_x_params methods
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_localized_policy_version_id(
-        self, value: str
-    ) -> RetrieveSingleLocalizedPolicyVersion1:
-        self.localized_policy_version_id = value
+    def with_policy_version_id(self, value: str) -> PublishPolicyVersion:
+        self.policy_version_id = value
         return self
 
-    def with_namespace(self, value: str) -> RetrieveSingleLocalizedPolicyVersion1:
-        self.namespace = value
+    def with_should_notify(self, value: bool) -> PublishPolicyVersion:
+        self.should_notify = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
-        if (
-            hasattr(self, "localized_policy_version_id")
-            and self.localized_policy_version_id
-        ):
-            result["localizedPolicyVersionId"] = str(self.localized_policy_version_id)
+        if hasattr(self, "policy_version_id") and self.policy_version_id:
+            result["policyVersionId"] = str(self.policy_version_id)
         elif include_empty:
-            result["localizedPolicyVersionId"] = ""
-        if hasattr(self, "namespace") and self.namespace:
-            result["namespace"] = str(self.namespace)
+            result["policyVersionId"] = ""
+        if hasattr(self, "should_notify") and self.should_notify:
+            result["shouldNotify"] = bool(self.should_notify)
         elif include_empty:
-            result["namespace"] = ""
+            result["shouldNotify"] = False
         return result
 
     # endregion to methods
 
     # region response methods
 
     # noinspection PyMethodMayBeStatic
     def parse_response(
         self, code: int, content_type: str, content: Any
-    ) -> Tuple[
-        Union[None, RetrieveLocalizedPolicyVersionResponse],
-        Union[None, ErrorEntity, HttpResponse],
-    ]:
+    ) -> Tuple[Union[None, HttpResponse], Union[None, ErrorEntity, HttpResponse]]:
         """Parse the given response.
 
-        200: OK - RetrieveLocalizedPolicyVersionResponse (successful operation)
+        200: OK - (operation successful)
+
+        400: Bad Request - ErrorEntity (40035: errors.net.accelbyte.platform.legal.invalid_policy_version | 40046: errors.net.accelbyte.platform.legal.default_selection_not_provided | 40030: errors.net.accelbyte.platform.legal.localized_policy_version_not_provided)
 
-        404: Not Found - ErrorEntity (2912: errors.net.accelbyte.platform.legal.policy_version_not_found)
+        409: Conflict - ErrorEntity (40039: errors.net.accelbyte.platform.legal.localized_policy_version_already_latest | 40043: errors.net.accelbyte.platform.legal.localized_policy_version_already_publish)
 
         ---: HttpResponse (Undocumented Response)
 
         ---: HttpResponse (Unexpected Content-Type Error)
 
         ---: HttpResponse (Unhandled Error)
         """
@@ -192,68 +198,63 @@
             code=code, content_type=content_type, content=content
         )
         if error is not None:
             return None, None if error.is_no_content() else error
         code, content_type, content = pre_processed_response
 
         if code == 200:
-            return (
-                RetrieveLocalizedPolicyVersionResponse.create_from_dict(content),
-                None,
-            )
-        if code == 404:
+            return HttpResponse.create(code, "OK"), None
+        if code == 400:
+            return None, ErrorEntity.create_from_dict(content)
+        if code == 409:
             return None, ErrorEntity.create_from_dict(content)
 
         return self.handle_undocumented_response(
             code=code, content_type=content_type, content=content
         )
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
     def create(
-        cls, localized_policy_version_id: str, namespace: str, **kwargs
-    ) -> RetrieveSingleLocalizedPolicyVersion1:
+        cls, policy_version_id: str, should_notify: Optional[bool] = None, **kwargs
+    ) -> PublishPolicyVersion:
         instance = cls()
-        instance.localized_policy_version_id = localized_policy_version_id
-        instance.namespace = namespace
+        instance.policy_version_id = policy_version_id
+        if should_notify is not None:
+            instance.should_notify = should_notify
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> RetrieveSingleLocalizedPolicyVersion1:
+    ) -> PublishPolicyVersion:
         instance = cls()
-        if (
-            "localizedPolicyVersionId" in dict_
-            and dict_["localizedPolicyVersionId"] is not None
-        ):
-            instance.localized_policy_version_id = str(
-                dict_["localizedPolicyVersionId"]
-            )
+        if "policyVersionId" in dict_ and dict_["policyVersionId"] is not None:
+            instance.policy_version_id = str(dict_["policyVersionId"])
         elif include_empty:
-            instance.localized_policy_version_id = ""
-        if "namespace" in dict_ and dict_["namespace"] is not None:
-            instance.namespace = str(dict_["namespace"])
+            instance.policy_version_id = ""
+        if "shouldNotify" in dict_ and dict_["shouldNotify"] is not None:
+            instance.should_notify = bool(dict_["shouldNotify"])
         elif include_empty:
-            instance.namespace = ""
+            instance.should_notify = False
         return instance
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
-            "localizedPolicyVersionId": "localized_policy_version_id",
-            "namespace": "namespace",
+            "policyVersionId": "policy_version_id",
+            "shouldNotify": "should_notify",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
-            "localizedPolicyVersionId": True,
-            "namespace": True,
+            "policyVersionId": True,
+            "shouldNotify": False,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/localized_policy_versions_with_namespace/set_default_policy_1.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/localized_policy_versions_with_namespace/set_default_policy_1.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,63 +30,69 @@
 from accelbyte_py_sdk.core import HttpResponse
 
 
 class SetDefaultPolicy1(Operation):
     """Set Default Localized Policy (setDefaultPolicy_1)
 
     Update a localized version policy to be the default.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:{namespace}:LEGAL", action=4 (UPDATE)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:LEGAL [UPDATE]
 
     Properties:
         url: /agreement/admin/namespaces/{namespace}/localized-policy-versions/{localizedPolicyVersionId}/default
 
         method: PATCH
 
         tags: ["Localized Policy Versions With Namespace"]
 
         consumes: []
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         localized_policy_version_id: (localizedPolicyVersionId) REQUIRED str in path
 
         namespace: (namespace) REQUIRED str in path
 
     Responses:
         200: OK - (successful operation)
     """
 
     # region fields
 
     _url: str = "/agreement/admin/namespaces/{namespace}/localized-policy-versions/{localizedPolicyVersionId}/default"
+    _path: str = "/agreement/admin/namespaces/{namespace}/localized-policy-versions/{localizedPolicyVersionId}/default"
+    _base_path: str = ""
     _method: str = "PATCH"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
-    _securities: List[List[str]] = [["BEARER_AUTH"], ["BEARER_AUTH"]]
+    _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "legal"
+
     localized_policy_version_id: str  # REQUIRED in [path]
     namespace: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/localized_policy_versions_with_namespace/update_localized_policy_b28b13.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/localized_policy_versions_with_namespace/update_localized_policy_b28b13.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,33 +34,27 @@
 from ...models import UpdateLocalizedPolicyVersionResponse
 
 
 class UpdateLocalizedPolicyVersion1(Operation):
     """Update a Localized Version from Country-Specific Policy (updateLocalizedPolicyVersion_1)
 
     Update a version of a particular country-specific policy.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:{namespace}:LEGAL", action=4 (UPDATE)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:LEGAL [UPDATE]
 
     Properties:
         url: /agreement/admin/namespaces/{namespace}/localized-policy-versions/{localizedPolicyVersionId}
 
         method: PUT
 
         tags: ["Localized Policy Versions With Namespace"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         body: (body) OPTIONAL UpdateLocalizedPolicyVersionRequest in body
 
         localized_policy_version_id: (localizedPolicyVersionId) REQUIRED str in path
 
         namespace: (namespace) REQUIRED str in path
 
@@ -69,33 +63,45 @@
 
         400: Bad Request - ErrorEntity (40035: errors.net.accelbyte.platform.legal.invalid_policy_version)
     """
 
     # region fields
 
     _url: str = "/agreement/admin/namespaces/{namespace}/localized-policy-versions/{localizedPolicyVersionId}"
+    _path: str = "/agreement/admin/namespaces/{namespace}/localized-policy-versions/{localizedPolicyVersionId}"
+    _base_path: str = ""
     _method: str = "PUT"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
-    _securities: List[List[str]] = [["BEARER_AUTH"], ["BEARER_AUTH"]]
+    _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "legal"
+
     body: UpdateLocalizedPolicyVersionRequest  # OPTIONAL in [body]
     localized_policy_version_id: str  # REQUIRED in [path]
     namespace: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/policies/__init__.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/policies/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Legal Service."""
 
-__version__ = "1.39.0"
+__version__ = "1.41.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .retrieve_country_list_w_8c69ff import RetrieveCountryListWithPolicies
 from .retrieve_latest_policies import RetrieveLatestPolicies
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/policies/retrieve_country_list_w_8c69ff.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/utility/check_readiness.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,56 +25,69 @@
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
+from ...models import LegalReadinessStatusResponse
 
-class RetrieveCountryListWithPolicies(Operation):
-    """Retrieve List of Countries that have Active Legal Policies (retrieveCountryListWithPolicies)
 
-    Retrieve List of Countries that have Active Legal Policies.
+class CheckReadiness(Operation):
+    """Check Legal Data Readiness (checkReadiness)
+
+    Readiness status defined as at least one legal basePolicy is present and having active basePolicy.
 
     Properties:
-        url: /agreement/public/policies/countries/list
+        url: /agreement/public/readiness
 
         method: GET
 
-        tags: ["Policies"]
+        tags: ["Utility"]
 
         consumes: []
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
-
     Responses:
-        200: OK - List[str] (successful operation)
+        200: OK - LegalReadinessStatusResponse (successful operation)
     """
 
     # region fields
 
-    _url: str = "/agreement/public/policies/countries/list"
+    _url: str = "/agreement/public/readiness"
+    _path: str = "/agreement/public/readiness"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "legal"
+
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
 
@@ -120,18 +133,18 @@
     # endregion to methods
 
     # region response methods
 
     # noinspection PyMethodMayBeStatic
     def parse_response(
         self, code: int, content_type: str, content: Any
-    ) -> Tuple[Union[None, List[str]], Union[None, HttpResponse]]:
+    ) -> Tuple[Union[None, LegalReadinessStatusResponse], Union[None, HttpResponse]]:
         """Parse the given response.
 
-        200: OK - List[str] (successful operation)
+        200: OK - LegalReadinessStatusResponse (successful operation)
 
         ---: HttpResponse (Undocumented Response)
 
         ---: HttpResponse (Unexpected Content-Type Error)
 
         ---: HttpResponse (Unhandled Error)
         """
@@ -139,35 +152,35 @@
             code=code, content_type=content_type, content=content
         )
         if error is not None:
             return None, None if error.is_no_content() else error
         code, content_type, content = pre_processed_response
 
         if code == 200:
-            return [str(i) for i in content], None
+            return LegalReadinessStatusResponse.create_from_dict(content), None
 
         return self.handle_undocumented_response(
             code=code, content_type=content_type, content=content
         )
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
-    def create(cls, **kwargs) -> RetrieveCountryListWithPolicies:
+    def create(cls, **kwargs) -> CheckReadiness:
         instance = cls()
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> RetrieveCountryListWithPolicies:
+    ) -> CheckReadiness:
         instance = cls()
         return instance
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {}
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/policies/retrieve_latest_policie_29f65f.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/policies/retrieve_latest_policie_29f65f.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,15 +51,14 @@
       *  Fill the alwaysIncludeDefault with true if you want to be responded with always include default policy. If there are duplicate policies (default policies and country specific policies with same base policy) it'll include policy with same country code, for example:
         * Document 1 (default): Region US (default), UA
         * Document 2 (default): Region US (default)
         * Document 3 (default): Region US (default)
         * User: Region UA
         * Query: alwaysIncludeDefault: true
         * Response: Document 1 (UA), Document 2 (US), Document 3 (US)
-      *  Required permission: login user
 
     Properties:
         url: /agreement/public/policies/namespaces/{namespace}
 
         method: GET
 
         tags: ["Policies"]
@@ -85,20 +84,24 @@
 
         404: Not Found - ErrorEntity (40040: errors.net.accelbyte.platform.legal.user_has_no_country)
     """
 
     # region fields
 
     _url: str = "/agreement/public/policies/namespaces/{namespace}"
+    _path: str = "/agreement/public/policies/namespaces/{namespace}"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "legal"
+
     namespace: str  # REQUIRED in [path]
     always_include_default: bool  # OPTIONAL in [query]
     default_on_empty: bool  # OPTIONAL in [query]
     policy_type: Union[str, PolicyTypeEnum]  # OPTIONAL in [query]
     tags: str  # OPTIONAL in [query]
 
     # endregion fields
@@ -106,14 +109,22 @@
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/policies/retrieve_latest_policie_95ffb6.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/policies/retrieve_latest_policie_95ffb6.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,20 +86,26 @@
     """
 
     # region fields
 
     _url: str = (
         "/agreement/public/policies/namespaces/{namespace}/countries/{countryCode}"
     )
+    _path: str = (
+        "/agreement/public/policies/namespaces/{namespace}/countries/{countryCode}"
+    )
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "legal"
+
     country_code: str  # REQUIRED in [path]
     namespace: str  # REQUIRED in [path]
     always_include_default: bool  # OPTIONAL in [query]
     default_on_empty: bool  # OPTIONAL in [query]
     policy_type: Union[str, PolicyTypeEnum]  # OPTIONAL in [query]
     tags: str  # OPTIONAL in [query]
 
@@ -108,14 +114,22 @@
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/policies/retrieve_latest_policies.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/policies/retrieve_latest_policies.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,34 +73,46 @@
     Responses:
         200: OK - List[RetrievePolicyPublicResponse] (successful operation)
     """
 
     # region fields
 
     _url: str = "/agreement/public/policies/countries/{countryCode}"
+    _path: str = "/agreement/public/policies/countries/{countryCode}"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "legal"
+
     country_code: str  # REQUIRED in [path]
     default_on_empty: bool  # OPTIONAL in [query]
     policy_type: Union[str, PolicyTypeEnum]  # OPTIONAL in [query]
     tags: str  # OPTIONAL in [query]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/policies/retrieve_policies.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/policies/retrieve_policies.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,60 +32,66 @@
 from ...models import RetrievePolicyResponse
 
 
 class RetrievePolicies(Operation):
     """Retrieve Policies by Country (retrievePolicies)
 
     Retrieve all active policies based on a country.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:*:LEGAL", action=2 (READ)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:*:LEGAL [READ]
 
     Properties:
         url: /agreement/admin/policies/countries/{countryCode}
 
         method: GET
 
         tags: ["Policies"]
 
         consumes: []
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         country_code: (countryCode) REQUIRED str in path
 
     Responses:
         200: OK - List[RetrievePolicyResponse] (successful operation)
     """
 
     # region fields
 
     _url: str = "/agreement/admin/policies/countries/{countryCode}"
+    _path: str = "/agreement/admin/policies/countries/{countryCode}"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
-    _securities: List[List[str]] = [["BEARER_AUTH"], ["BEARER_AUTH"]]
+    _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "legal"
+
     country_code: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/policies/set_default_policy_2.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/policies_with_namespace/set_default_policy_3.py`

 * *Files 15% similar despite different names*

```diff
@@ -28,66 +28,75 @@
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
 from ...models import ErrorEntity
 
 
-class SetDefaultPolicy2(Operation):
-    """Set Default Policy (setDefaultPolicy_2)
+class SetDefaultPolicy3(Operation):
+    """Set Default Policy (setDefaultPolicy_3)
 
     Update a policy to be the default.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:*:LEGAL", action=4 (UPDATE)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:*:LEGAL [UPDATE]
 
     Properties:
-        url: /agreement/admin/policies/{policyId}/default
+        url: /agreement/admin/namespaces/{namespace}/policies/{policyId}/default
 
         method: PATCH
 
-        tags: ["Policies"]
+        tags: ["Policies With Namespace"]
 
         consumes: []
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
+
+        namespace: (namespace) REQUIRED str in path
 
         policy_id: (policyId) REQUIRED str in path
 
     Responses:
         200: OK - (operation successful)
 
         400: Bad Request - ErrorEntity (40033: errors.net.accelbyte.platform.legal.invalid_policy_id)
     """
 
     # region fields
 
-    _url: str = "/agreement/admin/policies/{policyId}/default"
+    _url: str = "/agreement/admin/namespaces/{namespace}/policies/{policyId}/default"
+    _path: str = "/agreement/admin/namespaces/{namespace}/policies/{policyId}/default"
+    _base_path: str = ""
     _method: str = "PATCH"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
-    _securities: List[List[str]] = [["BEARER_AUTH"], ["BEARER_AUTH"]]
+    _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "legal"
+
+    namespace: str  # REQUIRED in [path]
     policy_id: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
 
@@ -114,36 +123,46 @@
     def get_all_params(self) -> dict:
         return {
             "path": self.get_path_params(),
         }
 
     def get_path_params(self) -> dict:
         result = {}
+        if hasattr(self, "namespace"):
+            result["namespace"] = self.namespace
         if hasattr(self, "policy_id"):
             result["policyId"] = self.policy_id
         return result
 
     # endregion get_x_params methods
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_policy_id(self, value: str) -> SetDefaultPolicy2:
+    def with_namespace(self, value: str) -> SetDefaultPolicy3:
+        self.namespace = value
+        return self
+
+    def with_policy_id(self, value: str) -> SetDefaultPolicy3:
         self.policy_id = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
+        if hasattr(self, "namespace") and self.namespace:
+            result["namespace"] = str(self.namespace)
+        elif include_empty:
+            result["namespace"] = ""
         if hasattr(self, "policy_id") and self.policy_id:
             result["policyId"] = str(self.policy_id)
         elif include_empty:
             result["policyId"] = ""
         return result
 
     # endregion to methods
@@ -183,38 +202,45 @@
         )
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
-    def create(cls, policy_id: str, **kwargs) -> SetDefaultPolicy2:
+    def create(cls, namespace: str, policy_id: str, **kwargs) -> SetDefaultPolicy3:
         instance = cls()
+        instance.namespace = namespace
         instance.policy_id = policy_id
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> SetDefaultPolicy2:
+    ) -> SetDefaultPolicy3:
         instance = cls()
+        if "namespace" in dict_ and dict_["namespace"] is not None:
+            instance.namespace = str(dict_["namespace"])
+        elif include_empty:
+            instance.namespace = ""
         if "policyId" in dict_ and dict_["policyId"] is not None:
             instance.policy_id = str(dict_["policyId"])
         elif include_empty:
             instance.policy_id = ""
         return instance
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
+            "namespace": "namespace",
             "policyId": "policy_id",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
+            "namespace": True,
             "policyId": True,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/policies/update_policy.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/policies/update_policy.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,65 +33,71 @@
 from ...models import UpdatePolicyRequest
 
 
 class UpdatePolicy(Operation):
     """Update Country-Specific Policy (updatePolicy)
 
     Update country-specific policy.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:*:LEGAL", action=4 (UPDATE)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:*:LEGAL [UPDATE]
 
     Properties:
         url: /agreement/admin/policies/{policyId}
 
         method: PATCH
 
         tags: ["Policies"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         body: (body) OPTIONAL UpdatePolicyRequest in body
 
         policy_id: (policyId) REQUIRED str in path
 
     Responses:
         200: OK - (operation successful)
 
         400: Bad Request - ErrorEntity (40033: errors.net.accelbyte.platform.legal.invalid_policy_id)
     """
 
     # region fields
 
     _url: str = "/agreement/admin/policies/{policyId}"
+    _path: str = "/agreement/admin/policies/{policyId}"
+    _base_path: str = ""
     _method: str = "PATCH"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
-    _securities: List[List[str]] = [["BEARER_AUTH"], ["BEARER_AUTH"]]
+    _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "legal"
+
     body: UpdatePolicyRequest  # OPTIONAL in [body]
     policy_id: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/policies_with_namespace/__init__.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/policy_versions/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Legal Service."""
 
-__version__ = "1.39.0"
+__version__ = "1.41.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
-from .set_default_policy_3 import SetDefaultPolicy3
-from .update_policy_1 import UpdatePolicy1
+from .create_policy_version import CreatePolicyVersion
+from .publish_policy_version import PublishPolicyVersion
+from .retrieve_single_policy_version import RetrieveSinglePolicyVersion
+from .update_policy_version import UpdatePolicyVersion
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/policies_with_namespace/set_default_policy_3.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/policies_with_namespace/update_policy_1.py`

 * *Files 13% similar despite different names*

```diff
@@ -26,71 +26,81 @@
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
 from ...models import ErrorEntity
+from ...models import UpdatePolicyRequest
 
 
-class SetDefaultPolicy3(Operation):
-    """Set Default Policy (setDefaultPolicy_3)
+class UpdatePolicy1(Operation):
+    """Update Country-Specific Policy (updatePolicy_1)
 
-    Update a policy to be the default.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:{namespace}:LEGAL", action=4 (UPDATE)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:LEGAL [UPDATE]
+    Update country-specific policy.
 
     Properties:
-        url: /agreement/admin/namespaces/{namespace}/policies/{policyId}/default
+        url: /agreement/admin/namespaces/{namespace}/policies/{policyId}
 
         method: PATCH
 
         tags: ["Policies With Namespace"]
 
-        consumes: []
+        consumes: ["application/json"]
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
+
+        body: (body) OPTIONAL UpdatePolicyRequest in body
 
         namespace: (namespace) REQUIRED str in path
 
         policy_id: (policyId) REQUIRED str in path
 
     Responses:
         200: OK - (operation successful)
 
         400: Bad Request - ErrorEntity (40033: errors.net.accelbyte.platform.legal.invalid_policy_id)
     """
 
     # region fields
 
-    _url: str = "/agreement/admin/namespaces/{namespace}/policies/{policyId}/default"
+    _url: str = "/agreement/admin/namespaces/{namespace}/policies/{policyId}"
+    _path: str = "/agreement/admin/namespaces/{namespace}/policies/{policyId}"
+    _base_path: str = ""
     _method: str = "PATCH"
-    _consumes: List[str] = []
+    _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
-    _securities: List[List[str]] = [["BEARER_AUTH"], ["BEARER_AUTH"]]
+    _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "legal"
+
+    body: UpdatePolicyRequest  # OPTIONAL in [body]
     namespace: str  # REQUIRED in [path]
     policy_id: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
 
@@ -112,17 +122,23 @@
 
     # endregion get methods
 
     # region get_x_params methods
 
     def get_all_params(self) -> dict:
         return {
+            "body": self.get_body_params(),
             "path": self.get_path_params(),
         }
 
+    def get_body_params(self) -> Any:
+        if not hasattr(self, "body") or self.body is None:
+            return None
+        return self.body.to_dict()
+
     def get_path_params(self) -> dict:
         result = {}
         if hasattr(self, "namespace"):
             result["namespace"] = self.namespace
         if hasattr(self, "policy_id"):
             result["policyId"] = self.policy_id
         return result
@@ -131,28 +147,36 @@
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_namespace(self, value: str) -> SetDefaultPolicy3:
+    def with_body(self, value: UpdatePolicyRequest) -> UpdatePolicy1:
+        self.body = value
+        return self
+
+    def with_namespace(self, value: str) -> UpdatePolicy1:
         self.namespace = value
         return self
 
-    def with_policy_id(self, value: str) -> SetDefaultPolicy3:
+    def with_policy_id(self, value: str) -> UpdatePolicy1:
         self.policy_id = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
+        if hasattr(self, "body") and self.body:
+            result["body"] = self.body.to_dict(include_empty=include_empty)
+        elif include_empty:
+            result["body"] = UpdatePolicyRequest()
         if hasattr(self, "namespace") and self.namespace:
             result["namespace"] = str(self.namespace)
         elif include_empty:
             result["namespace"] = ""
         if hasattr(self, "policy_id") and self.policy_id:
             result["policyId"] = str(self.policy_id)
         elif include_empty:
@@ -196,45 +220,61 @@
         )
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
-    def create(cls, namespace: str, policy_id: str, **kwargs) -> SetDefaultPolicy3:
+    def create(
+        cls,
+        namespace: str,
+        policy_id: str,
+        body: Optional[UpdatePolicyRequest] = None,
+        **kwargs,
+    ) -> UpdatePolicy1:
         instance = cls()
         instance.namespace = namespace
         instance.policy_id = policy_id
+        if body is not None:
+            instance.body = body
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> SetDefaultPolicy3:
+    ) -> UpdatePolicy1:
         instance = cls()
+        if "body" in dict_ and dict_["body"] is not None:
+            instance.body = UpdatePolicyRequest.create_from_dict(
+                dict_["body"], include_empty=include_empty
+            )
+        elif include_empty:
+            instance.body = UpdatePolicyRequest()
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
         elif include_empty:
             instance.namespace = ""
         if "policyId" in dict_ and dict_["policyId"] is not None:
             instance.policy_id = str(dict_["policyId"])
         elif include_empty:
             instance.policy_id = ""
         return instance
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
+            "body": "body",
             "namespace": "namespace",
             "policyId": "policy_id",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
+            "body": False,
             "namespace": True,
             "policyId": True,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/policies_with_namespace/update_policy_1.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/policy_versions/create_policy_version.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,76 +25,80 @@
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
+from ...models import CreatePolicyVersionRequest
+from ...models import CreatePolicyVersionResponse
 from ...models import ErrorEntity
-from ...models import UpdatePolicyRequest
 
 
-class UpdatePolicy1(Operation):
-    """Update Country-Specific Policy (updatePolicy_1)
+class CreatePolicyVersion(Operation):
+    """Create a Version from Country-Specific Policy (createPolicyVersion)
 
-    Update country-specific policy.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:{namespace}:LEGAL", action=4 (UPDATE)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:LEGAL [UPDATE]
+    Create a version of a particular country-specific policy.
 
     Properties:
-        url: /agreement/admin/namespaces/{namespace}/policies/{policyId}
+        url: /agreement/admin/policies/{policyId}/versions
 
-        method: PATCH
+        method: POST
 
-        tags: ["Policies With Namespace"]
+        tags: ["Policy Versions"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
-
-        body: (body) OPTIONAL UpdatePolicyRequest in body
+        securities: [BEARER_AUTH]
 
-        namespace: (namespace) REQUIRED str in path
+        body: (body) OPTIONAL CreatePolicyVersionRequest in body
 
         policy_id: (policyId) REQUIRED str in path
 
     Responses:
-        200: OK - (operation successful)
+        201: Created - CreatePolicyVersionResponse (successful operation)
 
-        400: Bad Request - ErrorEntity (40033: errors.net.accelbyte.platform.legal.invalid_policy_id)
+        400: Bad Request - ErrorEntity (40033: errors.net.accelbyte.platform.legal.invalid_policy)
     """
 
     # region fields
 
-    _url: str = "/agreement/admin/namespaces/{namespace}/policies/{policyId}"
-    _method: str = "PATCH"
+    _url: str = "/agreement/admin/policies/{policyId}/versions"
+    _path: str = "/agreement/admin/policies/{policyId}/versions"
+    _base_path: str = ""
+    _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
-    _securities: List[List[str]] = [["BEARER_AUTH"], ["BEARER_AUTH"]]
+    _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
-    body: UpdatePolicyRequest  # OPTIONAL in [body]
-    namespace: str  # REQUIRED in [path]
+    service_name: Optional[str] = "legal"
+
+    body: CreatePolicyVersionRequest  # OPTIONAL in [body]
     policy_id: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
 
@@ -127,148 +131,129 @@
     def get_body_params(self) -> Any:
         if not hasattr(self, "body") or self.body is None:
             return None
         return self.body.to_dict()
 
     def get_path_params(self) -> dict:
         result = {}
-        if hasattr(self, "namespace"):
-            result["namespace"] = self.namespace
         if hasattr(self, "policy_id"):
             result["policyId"] = self.policy_id
         return result
 
     # endregion get_x_params methods
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_body(self, value: UpdatePolicyRequest) -> UpdatePolicy1:
+    def with_body(self, value: CreatePolicyVersionRequest) -> CreatePolicyVersion:
         self.body = value
         return self
 
-    def with_namespace(self, value: str) -> UpdatePolicy1:
-        self.namespace = value
-        return self
-
-    def with_policy_id(self, value: str) -> UpdatePolicy1:
+    def with_policy_id(self, value: str) -> CreatePolicyVersion:
         self.policy_id = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
         if hasattr(self, "body") and self.body:
             result["body"] = self.body.to_dict(include_empty=include_empty)
         elif include_empty:
-            result["body"] = UpdatePolicyRequest()
-        if hasattr(self, "namespace") and self.namespace:
-            result["namespace"] = str(self.namespace)
-        elif include_empty:
-            result["namespace"] = ""
+            result["body"] = CreatePolicyVersionRequest()
         if hasattr(self, "policy_id") and self.policy_id:
             result["policyId"] = str(self.policy_id)
         elif include_empty:
             result["policyId"] = ""
         return result
 
     # endregion to methods
 
     # region response methods
 
     # noinspection PyMethodMayBeStatic
     def parse_response(
         self, code: int, content_type: str, content: Any
-    ) -> Tuple[Union[None, HttpResponse], Union[None, ErrorEntity, HttpResponse]]:
+    ) -> Tuple[
+        Union[None, CreatePolicyVersionResponse], Union[None, ErrorEntity, HttpResponse]
+    ]:
         """Parse the given response.
 
-        200: OK - (operation successful)
+        201: Created - CreatePolicyVersionResponse (successful operation)
 
-        400: Bad Request - ErrorEntity (40033: errors.net.accelbyte.platform.legal.invalid_policy_id)
+        400: Bad Request - ErrorEntity (40033: errors.net.accelbyte.platform.legal.invalid_policy)
 
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
-            return HttpResponse.create(code, "OK"), None
+        if code == 201:
+            return CreatePolicyVersionResponse.create_from_dict(content), None
         if code == 400:
             return None, ErrorEntity.create_from_dict(content)
 
         return self.handle_undocumented_response(
             code=code, content_type=content_type, content=content
         )
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
     def create(
-        cls,
-        namespace: str,
-        policy_id: str,
-        body: Optional[UpdatePolicyRequest] = None,
-        **kwargs,
-    ) -> UpdatePolicy1:
+        cls, policy_id: str, body: Optional[CreatePolicyVersionRequest] = None, **kwargs
+    ) -> CreatePolicyVersion:
         instance = cls()
-        instance.namespace = namespace
         instance.policy_id = policy_id
         if body is not None:
             instance.body = body
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> UpdatePolicy1:
+    ) -> CreatePolicyVersion:
         instance = cls()
         if "body" in dict_ and dict_["body"] is not None:
-            instance.body = UpdatePolicyRequest.create_from_dict(
+            instance.body = CreatePolicyVersionRequest.create_from_dict(
                 dict_["body"], include_empty=include_empty
             )
         elif include_empty:
-            instance.body = UpdatePolicyRequest()
-        if "namespace" in dict_ and dict_["namespace"] is not None:
-            instance.namespace = str(dict_["namespace"])
-        elif include_empty:
-            instance.namespace = ""
+            instance.body = CreatePolicyVersionRequest()
         if "policyId" in dict_ and dict_["policyId"] is not None:
             instance.policy_id = str(dict_["policyId"])
         elif include_empty:
             instance.policy_id = ""
         return instance
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
             "body": "body",
-            "namespace": "namespace",
             "policyId": "policy_id",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
             "body": False,
-            "namespace": True,
             "policyId": True,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/policy_versions/__init__.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/policy_versions_with_namespace/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Legal Service."""
 
-__version__ = "1.39.0"
+__version__ = "1.41.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
-from .create_policy_version import CreatePolicyVersion
-from .publish_policy_version import PublishPolicyVersion
-from .retrieve_single_policy_version import RetrieveSinglePolicyVersion
-from .update_policy_version import UpdatePolicyVersion
+from .create_policy_version_1 import CreatePolicyVersion1
+from .publish_policy_version_1 import PublishPolicyVersion1
+from .retrieve_single_policy__f63224 import RetrieveSinglePolicyVersion1
+from .update_policy_version_1 import UpdatePolicyVersion1
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/policy_versions/create_policy_version.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/policy_versions/retrieve_single_policy_version.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,74 +25,79 @@
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
-from ...models import CreatePolicyVersionRequest
-from ...models import CreatePolicyVersionResponse
 from ...models import ErrorEntity
+from ...models import RetrievePolicyVersionResponse
 
 
-class CreatePolicyVersion(Operation):
-    """Create a Version from Country-Specific Policy (createPolicyVersion)
+class RetrieveSinglePolicyVersion(Operation):
+    """Retrieve a Version from Country-Specific Policy (retrieveSinglePolicyVersion)
 
-    Create a version of a particular country-specific policy.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:*:LEGAL", action=1 (CREATE)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:*:LEGAL [CREATE]
+    Retrieve a version of a particular country specific policy. If version is not provided, the Legal Service will assume caller requesting all versions from country-specific policy.
 
     Properties:
         url: /agreement/admin/policies/{policyId}/versions
 
-        method: POST
+        method: GET
 
         tags: ["Policy Versions"]
 
-        consumes: ["application/json"]
+        consumes: []
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
-
-        body: (body) OPTIONAL CreatePolicyVersionRequest in body
+        securities: [BEARER_AUTH]
 
         policy_id: (policyId) REQUIRED str in path
 
+        version_id: (versionId) OPTIONAL str in query
+
     Responses:
-        201: Created - CreatePolicyVersionResponse (successful operation)
+        200: OK - List[RetrievePolicyVersionResponse] (successful operation)
 
-        400: Bad Request - ErrorEntity (40033: errors.net.accelbyte.platform.legal.invalid_policy)
+        404: Not Found - ErrorEntity (40036: errors.net.accelbyte.platform.legal.policy_version_id_not_found)
     """
 
     # region fields
 
     _url: str = "/agreement/admin/policies/{policyId}/versions"
-    _method: str = "POST"
-    _consumes: List[str] = ["application/json"]
+    _path: str = "/agreement/admin/policies/{policyId}/versions"
+    _base_path: str = ""
+    _method: str = "GET"
+    _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
-    _securities: List[List[str]] = [["BEARER_AUTH"], ["BEARER_AUTH"]]
+    _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
-    body: CreatePolicyVersionRequest  # OPTIONAL in [body]
+    service_name: Optional[str] = "legal"
+
     policy_id: str  # REQUIRED in [path]
+    version_id: str  # OPTIONAL in [query]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
 
@@ -114,140 +119,142 @@
 
     # endregion get methods
 
     # region get_x_params methods
 
     def get_all_params(self) -> dict:
         return {
-            "body": self.get_body_params(),
             "path": self.get_path_params(),
+            "query": self.get_query_params(),
         }
 
-    def get_body_params(self) -> Any:
-        if not hasattr(self, "body") or self.body is None:
-            return None
-        return self.body.to_dict()
-
     def get_path_params(self) -> dict:
         result = {}
         if hasattr(self, "policy_id"):
             result["policyId"] = self.policy_id
         return result
 
+    def get_query_params(self) -> dict:
+        result = {}
+        if hasattr(self, "version_id"):
+            result["versionId"] = self.version_id
+        return result
+
     # endregion get_x_params methods
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_body(self, value: CreatePolicyVersionRequest) -> CreatePolicyVersion:
-        self.body = value
+    def with_policy_id(self, value: str) -> RetrieveSinglePolicyVersion:
+        self.policy_id = value
         return self
 
-    def with_policy_id(self, value: str) -> CreatePolicyVersion:
-        self.policy_id = value
+    def with_version_id(self, value: str) -> RetrieveSinglePolicyVersion:
+        self.version_id = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
-        if hasattr(self, "body") and self.body:
-            result["body"] = self.body.to_dict(include_empty=include_empty)
-        elif include_empty:
-            result["body"] = CreatePolicyVersionRequest()
         if hasattr(self, "policy_id") and self.policy_id:
             result["policyId"] = str(self.policy_id)
         elif include_empty:
             result["policyId"] = ""
+        if hasattr(self, "version_id") and self.version_id:
+            result["versionId"] = str(self.version_id)
+        elif include_empty:
+            result["versionId"] = ""
         return result
 
     # endregion to methods
 
     # region response methods
 
     # noinspection PyMethodMayBeStatic
     def parse_response(
         self, code: int, content_type: str, content: Any
     ) -> Tuple[
-        Union[None, CreatePolicyVersionResponse], Union[None, ErrorEntity, HttpResponse]
+        Union[None, List[RetrievePolicyVersionResponse]],
+        Union[None, ErrorEntity, HttpResponse],
     ]:
         """Parse the given response.
 
-        201: Created - CreatePolicyVersionResponse (successful operation)
+        200: OK - List[RetrievePolicyVersionResponse] (successful operation)
 
-        400: Bad Request - ErrorEntity (40033: errors.net.accelbyte.platform.legal.invalid_policy)
+        404: Not Found - ErrorEntity (40036: errors.net.accelbyte.platform.legal.policy_version_id_not_found)
 
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
 
-        if code == 201:
-            return CreatePolicyVersionResponse.create_from_dict(content), None
-        if code == 400:
+        if code == 200:
+            return [
+                RetrievePolicyVersionResponse.create_from_dict(i) for i in content
+            ], None
+        if code == 404:
             return None, ErrorEntity.create_from_dict(content)
 
         return self.handle_undocumented_response(
             code=code, content_type=content_type, content=content
         )
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
     def create(
-        cls, policy_id: str, body: Optional[CreatePolicyVersionRequest] = None, **kwargs
-    ) -> CreatePolicyVersion:
+        cls, policy_id: str, version_id: Optional[str] = None, **kwargs
+    ) -> RetrieveSinglePolicyVersion:
         instance = cls()
         instance.policy_id = policy_id
-        if body is not None:
-            instance.body = body
+        if version_id is not None:
+            instance.version_id = version_id
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> CreatePolicyVersion:
+    ) -> RetrieveSinglePolicyVersion:
         instance = cls()
-        if "body" in dict_ and dict_["body"] is not None:
-            instance.body = CreatePolicyVersionRequest.create_from_dict(
-                dict_["body"], include_empty=include_empty
-            )
-        elif include_empty:
-            instance.body = CreatePolicyVersionRequest()
         if "policyId" in dict_ and dict_["policyId"] is not None:
             instance.policy_id = str(dict_["policyId"])
         elif include_empty:
             instance.policy_id = ""
+        if "versionId" in dict_ and dict_["versionId"] is not None:
+            instance.version_id = str(dict_["versionId"])
+        elif include_empty:
+            instance.version_id = ""
         return instance
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
-            "body": "body",
             "policyId": "policy_id",
+            "versionId": "version_id",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
-            "body": False,
             "policyId": True,
+            "versionId": False,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/policy_versions/publish_policy_version.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/policy_versions_with_namespace/publish_policy_version_1.py`

 * *Files 17% similar despite different names*

```diff
@@ -28,37 +28,33 @@
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
 from ...models import ErrorEntity
 
 
-class PublishPolicyVersion(Operation):
-    """Manually Publish a Version from Country-Specific Policy (publishPolicyVersion)
+class PublishPolicyVersion1(Operation):
+    """Manually Publish a Version from Country-Specific Policy (publishPolicyVersion_1)
 
     Manually publish a version of a particular country-specific policy.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:*:LEGAL", action=4 (UPDATE)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:*:LEGAL [UPDATE]
 
     Properties:
-        url: /agreement/admin/policies/versions/{policyVersionId}/latest
+        url: /agreement/admin/namespaces/{namespace}/policies/versions/{policyVersionId}/latest
 
         method: PATCH
 
-        tags: ["Policy Versions"]
+        tags: ["Policy Versions With Namespace"]
 
         consumes: []
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
+
+        namespace: (namespace) REQUIRED str in path
 
         policy_version_id: (policyVersionId) REQUIRED str in path
 
         should_notify: (shouldNotify) OPTIONAL bool in query
 
     Responses:
         200: OK - (operation successful)
@@ -66,33 +62,46 @@
         400: Bad Request - ErrorEntity (40035: errors.net.accelbyte.platform.legal.invalid_policy_version | 40046: errors.net.accelbyte.platform.legal.default_selection_not_provided | 40030: errors.net.accelbyte.platform.legal.localized_policy_version_not_provided)
 
         409: Conflict - ErrorEntity (40039: errors.net.accelbyte.platform.legal.localized_policy_version_already_latest | 40043: errors.net.accelbyte.platform.legal.localized_policy_version_already_publish)
     """
 
     # region fields
 
-    _url: str = "/agreement/admin/policies/versions/{policyVersionId}/latest"
+    _url: str = "/agreement/admin/namespaces/{namespace}/policies/versions/{policyVersionId}/latest"
+    _path: str = "/agreement/admin/namespaces/{namespace}/policies/versions/{policyVersionId}/latest"
+    _base_path: str = ""
     _method: str = "PATCH"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
-    _securities: List[List[str]] = [["BEARER_AUTH"], ["BEARER_AUTH"]]
+    _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "legal"
+
+    namespace: str  # REQUIRED in [path]
     policy_version_id: str  # REQUIRED in [path]
     should_notify: bool  # OPTIONAL in [query]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
 
@@ -120,14 +129,16 @@
         return {
             "path": self.get_path_params(),
             "query": self.get_query_params(),
         }
 
     def get_path_params(self) -> dict:
         result = {}
+        if hasattr(self, "namespace"):
+            result["namespace"] = self.namespace
         if hasattr(self, "policy_version_id"):
             result["policyVersionId"] = self.policy_version_id
         return result
 
     def get_query_params(self) -> dict:
         result = {}
         if hasattr(self, "should_notify"):
@@ -138,28 +149,36 @@
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_policy_version_id(self, value: str) -> PublishPolicyVersion:
+    def with_namespace(self, value: str) -> PublishPolicyVersion1:
+        self.namespace = value
+        return self
+
+    def with_policy_version_id(self, value: str) -> PublishPolicyVersion1:
         self.policy_version_id = value
         return self
 
-    def with_should_notify(self, value: bool) -> PublishPolicyVersion:
+    def with_should_notify(self, value: bool) -> PublishPolicyVersion1:
         self.should_notify = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
+        if hasattr(self, "namespace") and self.namespace:
+            result["namespace"] = str(self.namespace)
+        elif include_empty:
+            result["namespace"] = ""
         if hasattr(self, "policy_version_id") and self.policy_version_id:
             result["policyVersionId"] = str(self.policy_version_id)
         elif include_empty:
             result["policyVersionId"] = ""
         if hasattr(self, "should_notify") and self.should_notify:
             result["shouldNotify"] = bool(self.should_notify)
         elif include_empty:
@@ -208,47 +227,58 @@
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
     def create(
-        cls, policy_version_id: str, should_notify: Optional[bool] = None, **kwargs
-    ) -> PublishPolicyVersion:
+        cls,
+        namespace: str,
+        policy_version_id: str,
+        should_notify: Optional[bool] = None,
+        **kwargs,
+    ) -> PublishPolicyVersion1:
         instance = cls()
+        instance.namespace = namespace
         instance.policy_version_id = policy_version_id
         if should_notify is not None:
             instance.should_notify = should_notify
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> PublishPolicyVersion:
+    ) -> PublishPolicyVersion1:
         instance = cls()
+        if "namespace" in dict_ and dict_["namespace"] is not None:
+            instance.namespace = str(dict_["namespace"])
+        elif include_empty:
+            instance.namespace = ""
         if "policyVersionId" in dict_ and dict_["policyVersionId"] is not None:
             instance.policy_version_id = str(dict_["policyVersionId"])
         elif include_empty:
             instance.policy_version_id = ""
         if "shouldNotify" in dict_ and dict_["shouldNotify"] is not None:
             instance.should_notify = bool(dict_["shouldNotify"])
         elif include_empty:
             instance.should_notify = False
         return instance
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
+            "namespace": "namespace",
             "policyVersionId": "policy_version_id",
             "shouldNotify": "should_notify",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
+            "namespace": True,
             "policyVersionId": True,
             "shouldNotify": False,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/policy_versions/retrieve_single_policy_version.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/policy_versions/update_policy_version.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,72 +26,81 @@
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
 from ...models import ErrorEntity
-from ...models import RetrievePolicyVersionResponse
+from ...models import UpdatePolicyVersionRequest
+from ...models import UpdatePolicyVersionResponse
 
 
-class RetrieveSinglePolicyVersion(Operation):
-    """Retrieve a Version from Country-Specific Policy (retrieveSinglePolicyVersion)
+class UpdatePolicyVersion(Operation):
+    """Update a Version of Policy (updatePolicyVersion)
 
-    Retrieve a version of a particular country specific policy. If version is not provided, the Legal Service will assume caller requesting all versions from country-specific policy.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:*:LEGAL", action=2 (READ)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:*:LEGAL [READ]
+    Update a particular policy version.
 
     Properties:
-        url: /agreement/admin/policies/{policyId}/versions
+        url: /agreement/admin/policies/versions/{policyVersionId}
 
-        method: GET
+        method: PATCH
 
         tags: ["Policy Versions"]
 
-        consumes: []
+        consumes: ["application/json"]
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
-        policy_id: (policyId) REQUIRED str in path
+        body: (body) OPTIONAL UpdatePolicyVersionRequest in body
 
-        version_id: (versionId) OPTIONAL str in query
+        policy_version_id: (policyVersionId) REQUIRED str in path
 
     Responses:
-        200: OK - List[RetrievePolicyVersionResponse] (successful operation)
+        200: OK - UpdatePolicyVersionResponse (successful operation)
 
-        404: Not Found - ErrorEntity (40036: errors.net.accelbyte.platform.legal.policy_version_id_not_found)
+        400: Bad Request - ErrorEntity (40035: errors.net.accelbyte.platform.legal.invalid_policy_version | 40042: errors.net.accelbyte.platform.legal.policy_version_freezed)
+
+        409: Conflict - ErrorEntity (40043: errors.net.accelbyte.platform.legal.localized_policy_version_already_exist)
     """
 
     # region fields
 
-    _url: str = "/agreement/admin/policies/{policyId}/versions"
-    _method: str = "GET"
-    _consumes: List[str] = []
+    _url: str = "/agreement/admin/policies/versions/{policyVersionId}"
+    _path: str = "/agreement/admin/policies/versions/{policyVersionId}"
+    _base_path: str = ""
+    _method: str = "PATCH"
+    _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
-    _securities: List[List[str]] = [["BEARER_AUTH"], ["BEARER_AUTH"]]
+    _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
-    policy_id: str  # REQUIRED in [path]
-    version_id: str  # OPTIONAL in [query]
+    service_name: Optional[str] = "legal"
+
+    body: UpdatePolicyVersionRequest  # OPTIONAL in [body]
+    policy_version_id: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
 
@@ -113,78 +122,78 @@
 
     # endregion get methods
 
     # region get_x_params methods
 
     def get_all_params(self) -> dict:
         return {
+            "body": self.get_body_params(),
             "path": self.get_path_params(),
-            "query": self.get_query_params(),
         }
 
-    def get_path_params(self) -> dict:
-        result = {}
-        if hasattr(self, "policy_id"):
-            result["policyId"] = self.policy_id
-        return result
+    def get_body_params(self) -> Any:
+        if not hasattr(self, "body") or self.body is None:
+            return None
+        return self.body.to_dict()
 
-    def get_query_params(self) -> dict:
+    def get_path_params(self) -> dict:
         result = {}
-        if hasattr(self, "version_id"):
-            result["versionId"] = self.version_id
+        if hasattr(self, "policy_version_id"):
+            result["policyVersionId"] = self.policy_version_id
         return result
 
     # endregion get_x_params methods
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_policy_id(self, value: str) -> RetrieveSinglePolicyVersion:
-        self.policy_id = value
+    def with_body(self, value: UpdatePolicyVersionRequest) -> UpdatePolicyVersion:
+        self.body = value
         return self
 
-    def with_version_id(self, value: str) -> RetrieveSinglePolicyVersion:
-        self.version_id = value
+    def with_policy_version_id(self, value: str) -> UpdatePolicyVersion:
+        self.policy_version_id = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
-        if hasattr(self, "policy_id") and self.policy_id:
-            result["policyId"] = str(self.policy_id)
+        if hasattr(self, "body") and self.body:
+            result["body"] = self.body.to_dict(include_empty=include_empty)
         elif include_empty:
-            result["policyId"] = ""
-        if hasattr(self, "version_id") and self.version_id:
-            result["versionId"] = str(self.version_id)
+            result["body"] = UpdatePolicyVersionRequest()
+        if hasattr(self, "policy_version_id") and self.policy_version_id:
+            result["policyVersionId"] = str(self.policy_version_id)
         elif include_empty:
-            result["versionId"] = ""
+            result["policyVersionId"] = ""
         return result
 
     # endregion to methods
 
     # region response methods
 
     # noinspection PyMethodMayBeStatic
     def parse_response(
         self, code: int, content_type: str, content: Any
     ) -> Tuple[
-        Union[None, List[RetrievePolicyVersionResponse]],
-        Union[None, ErrorEntity, HttpResponse],
+        Union[None, UpdatePolicyVersionResponse], Union[None, ErrorEntity, HttpResponse]
     ]:
         """Parse the given response.
 
-        200: OK - List[RetrievePolicyVersionResponse] (successful operation)
+        200: OK - UpdatePolicyVersionResponse (successful operation)
+
+        400: Bad Request - ErrorEntity (40035: errors.net.accelbyte.platform.legal.invalid_policy_version | 40042: errors.net.accelbyte.platform.legal.policy_version_freezed)
 
-        404: Not Found - ErrorEntity (40036: errors.net.accelbyte.platform.legal.policy_version_id_not_found)
+        409: Conflict - ErrorEntity (40043: errors.net.accelbyte.platform.legal.localized_policy_version_already_exist)
 
         ---: HttpResponse (Undocumented Response)
 
         ---: HttpResponse (Unexpected Content-Type Error)
 
         ---: HttpResponse (Unhandled Error)
         """
@@ -192,63 +201,68 @@
             code=code, content_type=content_type, content=content
         )
         if error is not None:
             return None, None if error.is_no_content() else error
         code, content_type, content = pre_processed_response
 
         if code == 200:
-            return [
-                RetrievePolicyVersionResponse.create_from_dict(i) for i in content
-            ], None
-        if code == 404:
+            return UpdatePolicyVersionResponse.create_from_dict(content), None
+        if code == 400:
+            return None, ErrorEntity.create_from_dict(content)
+        if code == 409:
             return None, ErrorEntity.create_from_dict(content)
 
         return self.handle_undocumented_response(
             code=code, content_type=content_type, content=content
         )
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
     def create(
-        cls, policy_id: str, version_id: Optional[str] = None, **kwargs
-    ) -> RetrieveSinglePolicyVersion:
+        cls,
+        policy_version_id: str,
+        body: Optional[UpdatePolicyVersionRequest] = None,
+        **kwargs,
+    ) -> UpdatePolicyVersion:
         instance = cls()
-        instance.policy_id = policy_id
-        if version_id is not None:
-            instance.version_id = version_id
+        instance.policy_version_id = policy_version_id
+        if body is not None:
+            instance.body = body
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> RetrieveSinglePolicyVersion:
+    ) -> UpdatePolicyVersion:
         instance = cls()
-        if "policyId" in dict_ and dict_["policyId"] is not None:
-            instance.policy_id = str(dict_["policyId"])
+        if "body" in dict_ and dict_["body"] is not None:
+            instance.body = UpdatePolicyVersionRequest.create_from_dict(
+                dict_["body"], include_empty=include_empty
+            )
         elif include_empty:
-            instance.policy_id = ""
-        if "versionId" in dict_ and dict_["versionId"] is not None:
-            instance.version_id = str(dict_["versionId"])
+            instance.body = UpdatePolicyVersionRequest()
+        if "policyVersionId" in dict_ and dict_["policyVersionId"] is not None:
+            instance.policy_version_id = str(dict_["policyVersionId"])
         elif include_empty:
-            instance.version_id = ""
+            instance.policy_version_id = ""
         return instance
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
-            "policyId": "policy_id",
-            "versionId": "version_id",
+            "body": "body",
+            "policyVersionId": "policy_version_id",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
-            "policyId": True,
-            "versionId": False,
+            "body": False,
+            "policyVersionId": True,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/policy_versions/update_policy_version.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/policy_versions_with_namespace/update_policy_version_1.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,71 +30,84 @@
 from accelbyte_py_sdk.core import HttpResponse
 
 from ...models import ErrorEntity
 from ...models import UpdatePolicyVersionRequest
 from ...models import UpdatePolicyVersionResponse
 
 
-class UpdatePolicyVersion(Operation):
-    """Update a Version of Policy (updatePolicyVersion)
+class UpdatePolicyVersion1(Operation):
+    """Update a Version of Policy (updatePolicyVersion_1)
 
     Update a particular policy version.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:*:LEGAL", action=4 (UPDATE)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:*:LEGAL [UPDATE]
 
     Properties:
-        url: /agreement/admin/policies/versions/{policyVersionId}
+        url: /agreement/admin/namespaces/{namespace}/policies/versions/{policyVersionId}
 
         method: PATCH
 
-        tags: ["Policy Versions"]
+        tags: ["Policy Versions With Namespace"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         body: (body) OPTIONAL UpdatePolicyVersionRequest in body
 
+        namespace: (namespace) REQUIRED str in path
+
         policy_version_id: (policyVersionId) REQUIRED str in path
 
     Responses:
         200: OK - UpdatePolicyVersionResponse (successful operation)
 
         400: Bad Request - ErrorEntity (40035: errors.net.accelbyte.platform.legal.invalid_policy_version | 40042: errors.net.accelbyte.platform.legal.policy_version_freezed)
 
         409: Conflict - ErrorEntity (40043: errors.net.accelbyte.platform.legal.localized_policy_version_already_exist)
     """
 
     # region fields
 
-    _url: str = "/agreement/admin/policies/versions/{policyVersionId}"
+    _url: str = (
+        "/agreement/admin/namespaces/{namespace}/policies/versions/{policyVersionId}"
+    )
+    _path: str = (
+        "/agreement/admin/namespaces/{namespace}/policies/versions/{policyVersionId}"
+    )
+    _base_path: str = ""
     _method: str = "PATCH"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
-    _securities: List[List[str]] = [["BEARER_AUTH"], ["BEARER_AUTH"]]
+    _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "legal"
+
     body: UpdatePolicyVersionRequest  # OPTIONAL in [body]
+    namespace: str  # REQUIRED in [path]
     policy_version_id: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
 
@@ -127,44 +140,54 @@
     def get_body_params(self) -> Any:
         if not hasattr(self, "body") or self.body is None:
             return None
         return self.body.to_dict()
 
     def get_path_params(self) -> dict:
         result = {}
+        if hasattr(self, "namespace"):
+            result["namespace"] = self.namespace
         if hasattr(self, "policy_version_id"):
             result["policyVersionId"] = self.policy_version_id
         return result
 
     # endregion get_x_params methods
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_body(self, value: UpdatePolicyVersionRequest) -> UpdatePolicyVersion:
+    def with_body(self, value: UpdatePolicyVersionRequest) -> UpdatePolicyVersion1:
         self.body = value
         return self
 
-    def with_policy_version_id(self, value: str) -> UpdatePolicyVersion:
+    def with_namespace(self, value: str) -> UpdatePolicyVersion1:
+        self.namespace = value
+        return self
+
+    def with_policy_version_id(self, value: str) -> UpdatePolicyVersion1:
         self.policy_version_id = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
         if hasattr(self, "body") and self.body:
             result["body"] = self.body.to_dict(include_empty=include_empty)
         elif include_empty:
             result["body"] = UpdatePolicyVersionRequest()
+        if hasattr(self, "namespace") and self.namespace:
+            result["namespace"] = str(self.namespace)
+        elif include_empty:
+            result["namespace"] = ""
         if hasattr(self, "policy_version_id") and self.policy_version_id:
             result["policyVersionId"] = str(self.policy_version_id)
         elif include_empty:
             result["policyVersionId"] = ""
         return result
 
     # endregion to methods
@@ -212,51 +235,59 @@
     # endregion response methods
 
     # region static methods
 
     @classmethod
     def create(
         cls,
+        namespace: str,
         policy_version_id: str,
         body: Optional[UpdatePolicyVersionRequest] = None,
         **kwargs,
-    ) -> UpdatePolicyVersion:
+    ) -> UpdatePolicyVersion1:
         instance = cls()
+        instance.namespace = namespace
         instance.policy_version_id = policy_version_id
         if body is not None:
             instance.body = body
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> UpdatePolicyVersion:
+    ) -> UpdatePolicyVersion1:
         instance = cls()
         if "body" in dict_ and dict_["body"] is not None:
             instance.body = UpdatePolicyVersionRequest.create_from_dict(
                 dict_["body"], include_empty=include_empty
             )
         elif include_empty:
             instance.body = UpdatePolicyVersionRequest()
+        if "namespace" in dict_ and dict_["namespace"] is not None:
+            instance.namespace = str(dict_["namespace"])
+        elif include_empty:
+            instance.namespace = ""
         if "policyVersionId" in dict_ and dict_["policyVersionId"] is not None:
             instance.policy_version_id = str(dict_["policyVersionId"])
         elif include_empty:
             instance.policy_version_id = ""
         return instance
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
             "body": "body",
+            "namespace": "namespace",
             "policyVersionId": "policy_version_id",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
             "body": False,
+            "namespace": True,
             "policyVersionId": True,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/policy_versions_with_namespace/create_policy_version_1.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/policy_versions_with_namespace/create_policy_version_1.py`

 * *Files 12% similar despite different names*

```diff
@@ -34,33 +34,27 @@
 from ...models import ErrorEntity
 
 
 class CreatePolicyVersion1(Operation):
     """Create a Version from Country-Specific Policy (createPolicyVersion_1)
 
     Create a version of a particular country-specific policy.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:*:LEGAL", action=1 (CREATE)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:*:LEGAL [CREATE]
 
     Properties:
         url: /agreement/admin/namespaces/{namespace}/policies/{policyId}/versions
 
         method: POST
 
         tags: ["Policy Versions With Namespace"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         body: (body) OPTIONAL CreatePolicyVersionRequest in body
 
         namespace: (namespace) REQUIRED str in path
 
         policy_id: (policyId) REQUIRED str in path
 
@@ -69,33 +63,45 @@
 
         400: Bad Request - ErrorEntity (40033: errors.net.accelbyte.platform.legal.invalid_policy)
     """
 
     # region fields
 
     _url: str = "/agreement/admin/namespaces/{namespace}/policies/{policyId}/versions"
+    _path: str = "/agreement/admin/namespaces/{namespace}/policies/{policyId}/versions"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
-    _securities: List[List[str]] = [["BEARER_AUTH"], ["BEARER_AUTH"]]
+    _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "legal"
+
     body: CreatePolicyVersionRequest  # OPTIONAL in [body]
     namespace: str  # REQUIRED in [path]
     policy_id: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/policy_versions_with_namespace/publish_policy_version_1.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/agreement_with_namespace/download_exported_agree_a56e5b.py`

 * *Files 21% similar despite different names*

```diff
@@ -25,77 +25,80 @@
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
+from ...models import DownloadExportedAgreementsInCSVResponse
 from ...models import ErrorEntity
 
 
-class PublishPolicyVersion1(Operation):
-    """Manually Publish a Version from Country-Specific Policy (publishPolicyVersion_1)
+class DownloadExportedAgreementsInCSV(Operation):
+    """Download Exported Users Accepted Agreements in CSV (downloadExportedAgreementsInCSV)
 
-    Manually publish a version of a particular country-specific policy.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:*:LEGAL", action=4 (UPDATE)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:*:LEGAL [UPDATE]
+    This API will check the status of export process.
+    If the export process has been completed, the response body will include the download url.
 
     Properties:
-        url: /agreement/admin/namespaces/{namespace}/policies/versions/{policyVersionId}/latest
+        url: /agreement/admin/namespaces/{namespace}/agreements/policy-versions/users/export-csv/download
 
-        method: PATCH
+        method: GET
 
-        tags: ["Policy Versions With Namespace"]
+        tags: ["Agreement With Namespace"]
 
         consumes: []
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         namespace: (namespace) REQUIRED str in path
 
-        policy_version_id: (policyVersionId) REQUIRED str in path
-
-        should_notify: (shouldNotify) OPTIONAL bool in query
+        export_id: (exportId) REQUIRED str in query
 
     Responses:
-        200: OK - (operation successful)
-
-        400: Bad Request - ErrorEntity (40035: errors.net.accelbyte.platform.legal.invalid_policy_version | 40046: errors.net.accelbyte.platform.legal.default_selection_not_provided | 40030: errors.net.accelbyte.platform.legal.localized_policy_version_not_provided)
+        200: OK - DownloadExportedAgreementsInCSVResponse (successful operation)
 
-        409: Conflict - ErrorEntity (40039: errors.net.accelbyte.platform.legal.localized_policy_version_already_latest | 40043: errors.net.accelbyte.platform.legal.localized_policy_version_already_publish)
+        404: Not Found - ErrorEntity (40047: Exported agreements for exportId [{exportId}] not found)
     """
 
     # region fields
 
-    _url: str = "/agreement/admin/namespaces/{namespace}/policies/versions/{policyVersionId}/latest"
-    _method: str = "PATCH"
+    _url: str = "/agreement/admin/namespaces/{namespace}/agreements/policy-versions/users/export-csv/download"
+    _path: str = "/agreement/admin/namespaces/{namespace}/agreements/policy-versions/users/export-csv/download"
+    _base_path: str = ""
+    _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
-    _securities: List[List[str]] = [["BEARER_AUTH"], ["BEARER_AUTH"]]
+    _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "legal"
+
     namespace: str  # REQUIRED in [path]
-    policy_version_id: str  # REQUIRED in [path]
-    should_notify: bool  # OPTIONAL in [query]
+    export_id: str  # REQUIRED in [query]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
 
@@ -125,79 +128,70 @@
             "query": self.get_query_params(),
         }
 
     def get_path_params(self) -> dict:
         result = {}
         if hasattr(self, "namespace"):
             result["namespace"] = self.namespace
-        if hasattr(self, "policy_version_id"):
-            result["policyVersionId"] = self.policy_version_id
         return result
 
     def get_query_params(self) -> dict:
         result = {}
-        if hasattr(self, "should_notify"):
-            result["shouldNotify"] = self.should_notify
+        if hasattr(self, "export_id"):
+            result["exportId"] = self.export_id
         return result
 
     # endregion get_x_params methods
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_namespace(self, value: str) -> PublishPolicyVersion1:
+    def with_namespace(self, value: str) -> DownloadExportedAgreementsInCSV:
         self.namespace = value
         return self
 
-    def with_policy_version_id(self, value: str) -> PublishPolicyVersion1:
-        self.policy_version_id = value
-        return self
-
-    def with_should_notify(self, value: bool) -> PublishPolicyVersion1:
-        self.should_notify = value
+    def with_export_id(self, value: str) -> DownloadExportedAgreementsInCSV:
+        self.export_id = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
         if hasattr(self, "namespace") and self.namespace:
             result["namespace"] = str(self.namespace)
         elif include_empty:
             result["namespace"] = ""
-        if hasattr(self, "policy_version_id") and self.policy_version_id:
-            result["policyVersionId"] = str(self.policy_version_id)
-        elif include_empty:
-            result["policyVersionId"] = ""
-        if hasattr(self, "should_notify") and self.should_notify:
-            result["shouldNotify"] = bool(self.should_notify)
+        if hasattr(self, "export_id") and self.export_id:
+            result["exportId"] = str(self.export_id)
         elif include_empty:
-            result["shouldNotify"] = False
+            result["exportId"] = ""
         return result
 
     # endregion to methods
 
     # region response methods
 
     # noinspection PyMethodMayBeStatic
     def parse_response(
         self, code: int, content_type: str, content: Any
-    ) -> Tuple[Union[None, HttpResponse], Union[None, ErrorEntity, HttpResponse]]:
+    ) -> Tuple[
+        Union[None, DownloadExportedAgreementsInCSVResponse],
+        Union[None, ErrorEntity, HttpResponse],
+    ]:
         """Parse the given response.
 
-        200: OK - (operation successful)
+        200: OK - DownloadExportedAgreementsInCSVResponse (successful operation)
 
-        400: Bad Request - ErrorEntity (40035: errors.net.accelbyte.platform.legal.invalid_policy_version | 40046: errors.net.accelbyte.platform.legal.default_selection_not_provided | 40030: errors.net.accelbyte.platform.legal.localized_policy_version_not_provided)
-
-        409: Conflict - ErrorEntity (40039: errors.net.accelbyte.platform.legal.localized_policy_version_already_latest | 40043: errors.net.accelbyte.platform.legal.localized_policy_version_already_publish)
+        404: Not Found - ErrorEntity (40047: Exported agreements for exportId [{exportId}] not found)
 
         ---: HttpResponse (Undocumented Response)
 
         ---: HttpResponse (Unexpected Content-Type Error)
 
         ---: HttpResponse (Unhandled Error)
         """
@@ -205,74 +199,63 @@
             code=code, content_type=content_type, content=content
         )
         if error is not None:
             return None, None if error.is_no_content() else error
         code, content_type, content = pre_processed_response
 
         if code == 200:
-            return HttpResponse.create(code, "OK"), None
-        if code == 400:
-            return None, ErrorEntity.create_from_dict(content)
-        if code == 409:
+            return (
+                DownloadExportedAgreementsInCSVResponse.create_from_dict(content),
+                None,
+            )
+        if code == 404:
             return None, ErrorEntity.create_from_dict(content)
 
         return self.handle_undocumented_response(
             code=code, content_type=content_type, content=content
         )
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
     def create(
-        cls,
-        namespace: str,
-        policy_version_id: str,
-        should_notify: Optional[bool] = None,
-        **kwargs,
-    ) -> PublishPolicyVersion1:
+        cls, namespace: str, export_id: str, **kwargs
+    ) -> DownloadExportedAgreementsInCSV:
         instance = cls()
         instance.namespace = namespace
-        instance.policy_version_id = policy_version_id
-        if should_notify is not None:
-            instance.should_notify = should_notify
+        instance.export_id = export_id
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> PublishPolicyVersion1:
+    ) -> DownloadExportedAgreementsInCSV:
         instance = cls()
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
         elif include_empty:
             instance.namespace = ""
-        if "policyVersionId" in dict_ and dict_["policyVersionId"] is not None:
-            instance.policy_version_id = str(dict_["policyVersionId"])
-        elif include_empty:
-            instance.policy_version_id = ""
-        if "shouldNotify" in dict_ and dict_["shouldNotify"] is not None:
-            instance.should_notify = bool(dict_["shouldNotify"])
+        if "exportId" in dict_ and dict_["exportId"] is not None:
+            instance.export_id = str(dict_["exportId"])
         elif include_empty:
-            instance.should_notify = False
+            instance.export_id = ""
         return instance
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
             "namespace": "namespace",
-            "policyVersionId": "policy_version_id",
-            "shouldNotify": "should_notify",
+            "exportId": "export_id",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
             "namespace": True,
-            "policyVersionId": True,
-            "shouldNotify": False,
+            "exportId": True,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/policy_versions_with_namespace/retrieve_single_policy__f63224.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/policy_versions_with_namespace/retrieve_single_policy__f63224.py`

 * *Files 9% similar despite different names*

```diff
@@ -33,33 +33,27 @@
 from ...models import RetrievePolicyVersionResponse
 
 
 class RetrieveSinglePolicyVersion1(Operation):
     """Retrieve a Version from Country-Specific Policy (retrieveSinglePolicyVersion_1)
 
     Retrieve a version of a particular country specific policy. If version is not provided, the Legal Service will assume caller requesting all versions from country-specific policy.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:*:LEGAL", action=2 (READ)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:*:LEGAL [READ]
 
     Properties:
         url: /agreement/admin/namespaces/{namespace}/policies/{policyId}/versions
 
         method: GET
 
         tags: ["Policy Versions With Namespace"]
 
         consumes: []
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         namespace: (namespace) REQUIRED str in path
 
         policy_id: (policyId) REQUIRED str in path
 
         version_id: (versionId) OPTIONAL str in query
 
@@ -68,33 +62,45 @@
 
         404: Not Found - ErrorEntity (40036: errors.net.accelbyte.platform.legal.policy_version_id_not_found)
     """
 
     # region fields
 
     _url: str = "/agreement/admin/namespaces/{namespace}/policies/{policyId}/versions"
+    _path: str = "/agreement/admin/namespaces/{namespace}/policies/{policyId}/versions"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
-    _securities: List[List[str]] = [["BEARER_AUTH"], ["BEARER_AUTH"]]
+    _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "legal"
+
     namespace: str  # REQUIRED in [path]
     policy_id: str  # REQUIRED in [path]
     version_id: str  # OPTIONAL in [query]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/policy_versions_with_namespace/update_policy_version_1.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/wrappers/_eligibilities.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,285 +1,233 @@
 # Copyright (c) 2021 AccelByte Inc. All Rights Reserved.
 # This is licensed software from AccelByte Inc, for limitations
 # and restrictions contact your company contract manager.
 #
 # Code generated. DO NOT EDIT!
 
-# template file: operation.j2
+# template file: wrapper.j2
 
 # pylint: disable=duplicate-code
 # pylint: disable=line-too-long
 # pylint: disable=missing-function-docstring
+# pylint: disable=missing-function-docstring
 # pylint: disable=missing-module-docstring
 # pylint: disable=too-many-arguments
 # pylint: disable=too-many-branches
 # pylint: disable=too-many-instance-attributes
 # pylint: disable=too-many-lines
 # pylint: disable=too-many-locals
 # pylint: disable=too-many-public-methods
 # pylint: disable=too-many-return-statements
 # pylint: disable=too-many-statements
 # pylint: disable=unused-import
 
-# AccelByte Gaming Services Legal Service
-
-from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
-from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
-from accelbyte_py_sdk.core import HttpResponse
+from accelbyte_py_sdk.core import get_namespace as get_services_namespace
+from accelbyte_py_sdk.core import run_request
+from accelbyte_py_sdk.core import run_request_async
+from accelbyte_py_sdk.core import same_doc_as
+
+from ..models import ErrorEntity
+from ..models import RetrieveUserEligibilitiesIndirectResponse
+from ..models import RetrieveUserEligibilitiesResponse
+
+from ..operations.eligibilities import RetrieveEligibilitiesPublic
+from ..operations.eligibilities import RetrieveEligibilitiesPublicIndirect
+
+
+@same_doc_as(RetrieveEligibilitiesPublic)
+def retrieve_eligibilities_public(
+    namespace: Optional[str] = None,
+    x_additional_headers: Optional[Dict[str, str]] = None,
+    **kwargs
+):
+    """Check User Legal Eligibility (retrieveEligibilitiesPublic)
+
+    Retrieve the active policies and its conformance status by user.
+    This process supports cross-namespace checking, that means if the active policy already accepted by the same user in other namespace, then it will be considered as eligible.
+
+    Properties:
+        url: /agreement/public/eligibilities/namespaces/{namespace}
+
+        method: GET
 
-from ...models import ErrorEntity
-from ...models import UpdatePolicyVersionRequest
-from ...models import UpdatePolicyVersionResponse
+        tags: ["Eligibilities"]
 
+        consumes: []
+
+        produces: ["application/json"]
 
-class UpdatePolicyVersion1(Operation):
-    """Update a Version of Policy (updatePolicyVersion_1)
+        securities: [BEARER_AUTH]
+
+        namespace: (namespace) REQUIRED str in path
+
+    Responses:
+        200: OK - List[RetrieveUserEligibilitiesResponse] (successful operation)
+
+        400: Bad Request - ErrorEntity (40045: errors.net.accelbyte.platform.legal.user_id_needed)
+
+        404: Not Found - ErrorEntity (40041: errors.net.accelbyte.platform.legal.policy_not_found)
+    """
+    if namespace is None:
+        namespace, error = get_services_namespace()
+        if error:
+            return None, error
+    request = RetrieveEligibilitiesPublic.create(
+        namespace=namespace,
+    )
+    return run_request(request, additional_headers=x_additional_headers, **kwargs)
 
-    Update a particular policy version.
-    Other detail info:
 
-      * Required permission : resource="ADMIN:NAMESPACE:*:LEGAL", action=4 (UPDATE)
+@same_doc_as(RetrieveEligibilitiesPublic)
+async def retrieve_eligibilities_public_async(
+    namespace: Optional[str] = None,
+    x_additional_headers: Optional[Dict[str, str]] = None,
+    **kwargs
+):
+    """Check User Legal Eligibility (retrieveEligibilitiesPublic)
 
-    Required Permission(s):
-        - ADMIN:NAMESPACE:*:LEGAL [UPDATE]
+    Retrieve the active policies and its conformance status by user.
+    This process supports cross-namespace checking, that means if the active policy already accepted by the same user in other namespace, then it will be considered as eligible.
 
     Properties:
-        url: /agreement/admin/namespaces/{namespace}/policies/versions/{policyVersionId}
+        url: /agreement/public/eligibilities/namespaces/{namespace}
 
-        method: PATCH
+        method: GET
 
-        tags: ["Policy Versions With Namespace"]
+        tags: ["Eligibilities"]
 
-        consumes: ["application/json"]
+        consumes: []
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
-
-        body: (body) OPTIONAL UpdatePolicyVersionRequest in body
+        securities: [BEARER_AUTH]
 
         namespace: (namespace) REQUIRED str in path
 
-        policy_version_id: (policyVersionId) REQUIRED str in path
-
     Responses:
-        200: OK - UpdatePolicyVersionResponse (successful operation)
+        200: OK - List[RetrieveUserEligibilitiesResponse] (successful operation)
 
-        400: Bad Request - ErrorEntity (40035: errors.net.accelbyte.platform.legal.invalid_policy_version | 40042: errors.net.accelbyte.platform.legal.policy_version_freezed)
+        400: Bad Request - ErrorEntity (40045: errors.net.accelbyte.platform.legal.user_id_needed)
 
-        409: Conflict - ErrorEntity (40043: errors.net.accelbyte.platform.legal.localized_policy_version_already_exist)
+        404: Not Found - ErrorEntity (40041: errors.net.accelbyte.platform.legal.policy_not_found)
     """
+    if namespace is None:
+        namespace, error = get_services_namespace()
+        if error:
+            return None, error
+    request = RetrieveEligibilitiesPublic.create(
+        namespace=namespace,
+    )
+    return await run_request_async(
+        request, additional_headers=x_additional_headers, **kwargs
+    )
+
+
+@same_doc_as(RetrieveEligibilitiesPublicIndirect)
+def retrieve_eligibilities_public_indirect(
+    client_id: str,
+    country_code: str,
+    user_id: str,
+    namespace: Optional[str] = None,
+    x_additional_headers: Optional[Dict[str, str]] = None,
+    **kwargs
+):
+    """Check User Legal Eligibility (retrieveEligibilitiesPublicIndirect)
+
+    Retrieve the active policies and its conformance status by user.
+    This process only supports cross-namespace checking between game namespace and publisher namespace , that means if the active policy already accepted by the same user in publisher namespace, then it will also be considered as eligible in non-publisher namespace.
+
+    Properties:
+        url: /agreement/public/eligibilities/namespaces/{namespace}/countries/{countryCode}/clients/{clientId}/users/{userId}
+
+        method: GET
+
+        tags: ["Eligibilities"]
+
+        consumes: []
+
+        produces: ["application/json"]
 
-    # region fields
+        securities: [BEARER_AUTH]
 
-    _url: str = (
-        "/agreement/admin/namespaces/{namespace}/policies/versions/{policyVersionId}"
+        client_id: (clientId) REQUIRED str in path
+
+        country_code: (countryCode) REQUIRED str in path
+
+        namespace: (namespace) REQUIRED str in path
+
+        user_id: (userId) REQUIRED str in path
+
+    Responses:
+        200: OK - RetrieveUserEligibilitiesIndirectResponse (successful operation)
+
+        400: Bad Request - ErrorEntity (40045: errors.net.accelbyte.platform.legal.user_id_needed)
+    """
+    if namespace is None:
+        namespace, error = get_services_namespace()
+        if error:
+            return None, error
+    request = RetrieveEligibilitiesPublicIndirect.create(
+        client_id=client_id,
+        country_code=country_code,
+        user_id=user_id,
+        namespace=namespace,
     )
-    _method: str = "PATCH"
-    _consumes: List[str] = ["application/json"]
-    _produces: List[str] = ["application/json"]
-    _securities: List[List[str]] = [["BEARER_AUTH"], ["BEARER_AUTH"]]
-    _location_query: str = None
-
-    body: UpdatePolicyVersionRequest  # OPTIONAL in [body]
-    namespace: str  # REQUIRED in [path]
-    policy_version_id: str  # REQUIRED in [path]
-
-    # endregion fields
-
-    # region properties
-
-    @property
-    def url(self) -> str:
-        return self._url
-
-    @property
-    def method(self) -> str:
-        return self._method
-
-    @property
-    def consumes(self) -> List[str]:
-        return self._consumes
-
-    @property
-    def produces(self) -> List[str]:
-        return self._produces
-
-    @property
-    def securities(self) -> List[List[str]]:
-        return self._securities
-
-    @property
-    def location_query(self) -> str:
-        return self._location_query
-
-    # endregion properties
-
-    # region get methods
-
-    # endregion get methods
-
-    # region get_x_params methods
-
-    def get_all_params(self) -> dict:
-        return {
-            "body": self.get_body_params(),
-            "path": self.get_path_params(),
-        }
-
-    def get_body_params(self) -> Any:
-        if not hasattr(self, "body") or self.body is None:
-            return None
-        return self.body.to_dict()
-
-    def get_path_params(self) -> dict:
-        result = {}
-        if hasattr(self, "namespace"):
-            result["namespace"] = self.namespace
-        if hasattr(self, "policy_version_id"):
-            result["policyVersionId"] = self.policy_version_id
-        return result
-
-    # endregion get_x_params methods
-
-    # region is/has methods
-
-    # endregion is/has methods
-
-    # region with_x methods
-
-    def with_body(self, value: UpdatePolicyVersionRequest) -> UpdatePolicyVersion1:
-        self.body = value
-        return self
-
-    def with_namespace(self, value: str) -> UpdatePolicyVersion1:
-        self.namespace = value
-        return self
-
-    def with_policy_version_id(self, value: str) -> UpdatePolicyVersion1:
-        self.policy_version_id = value
-        return self
-
-    # endregion with_x methods
-
-    # region to methods
-
-    def to_dict(self, include_empty: bool = False) -> dict:
-        result: dict = {}
-        if hasattr(self, "body") and self.body:
-            result["body"] = self.body.to_dict(include_empty=include_empty)
-        elif include_empty:
-            result["body"] = UpdatePolicyVersionRequest()
-        if hasattr(self, "namespace") and self.namespace:
-            result["namespace"] = str(self.namespace)
-        elif include_empty:
-            result["namespace"] = ""
-        if hasattr(self, "policy_version_id") and self.policy_version_id:
-            result["policyVersionId"] = str(self.policy_version_id)
-        elif include_empty:
-            result["policyVersionId"] = ""
-        return result
-
-    # endregion to methods
-
-    # region response methods
-
-    # noinspection PyMethodMayBeStatic
-    def parse_response(
-        self, code: int, content_type: str, content: Any
-    ) -> Tuple[
-        Union[None, UpdatePolicyVersionResponse], Union[None, ErrorEntity, HttpResponse]
-    ]:
-        """Parse the given response.
-
-        200: OK - UpdatePolicyVersionResponse (successful operation)
-
-        400: Bad Request - ErrorEntity (40035: errors.net.accelbyte.platform.legal.invalid_policy_version | 40042: errors.net.accelbyte.platform.legal.policy_version_freezed)
-
-        409: Conflict - ErrorEntity (40043: errors.net.accelbyte.platform.legal.localized_policy_version_already_exist)
-
-        ---: HttpResponse (Undocumented Response)
-
-        ---: HttpResponse (Unexpected Content-Type Error)
-
-        ---: HttpResponse (Unhandled Error)
-        """
-        pre_processed_response, error = self.pre_process_response(
-            code=code, content_type=content_type, content=content
-        )
-        if error is not None:
-            return None, None if error.is_no_content() else error
-        code, content_type, content = pre_processed_response
-
-        if code == 200:
-            return UpdatePolicyVersionResponse.create_from_dict(content), None
-        if code == 400:
-            return None, ErrorEntity.create_from_dict(content)
-        if code == 409:
-            return None, ErrorEntity.create_from_dict(content)
-
-        return self.handle_undocumented_response(
-            code=code, content_type=content_type, content=content
-        )
-
-    # endregion response methods
-
-    # region static methods
-
-    @classmethod
-    def create(
-        cls,
-        namespace: str,
-        policy_version_id: str,
-        body: Optional[UpdatePolicyVersionRequest] = None,
-        **kwargs,
-    ) -> UpdatePolicyVersion1:
-        instance = cls()
-        instance.namespace = namespace
-        instance.policy_version_id = policy_version_id
-        if body is not None:
-            instance.body = body
-        if x_flight_id := kwargs.get("x_flight_id", None):
-            instance.x_flight_id = x_flight_id
-        return instance
-
-    @classmethod
-    def create_from_dict(
-        cls, dict_: dict, include_empty: bool = False
-    ) -> UpdatePolicyVersion1:
-        instance = cls()
-        if "body" in dict_ and dict_["body"] is not None:
-            instance.body = UpdatePolicyVersionRequest.create_from_dict(
-                dict_["body"], include_empty=include_empty
-            )
-        elif include_empty:
-            instance.body = UpdatePolicyVersionRequest()
-        if "namespace" in dict_ and dict_["namespace"] is not None:
-            instance.namespace = str(dict_["namespace"])
-        elif include_empty:
-            instance.namespace = ""
-        if "policyVersionId" in dict_ and dict_["policyVersionId"] is not None:
-            instance.policy_version_id = str(dict_["policyVersionId"])
-        elif include_empty:
-            instance.policy_version_id = ""
-        return instance
-
-    @staticmethod
-    def get_field_info() -> Dict[str, str]:
-        return {
-            "body": "body",
-            "namespace": "namespace",
-            "policyVersionId": "policy_version_id",
-        }
-
-    @staticmethod
-    def get_required_map() -> Dict[str, bool]:
-        return {
-            "body": False,
-            "namespace": True,
-            "policyVersionId": True,
-        }
+    return run_request(request, additional_headers=x_additional_headers, **kwargs)
+
+
+@same_doc_as(RetrieveEligibilitiesPublicIndirect)
+async def retrieve_eligibilities_public_indirect_async(
+    client_id: str,
+    country_code: str,
+    user_id: str,
+    namespace: Optional[str] = None,
+    x_additional_headers: Optional[Dict[str, str]] = None,
+    **kwargs
+):
+    """Check User Legal Eligibility (retrieveEligibilitiesPublicIndirect)
+
+    Retrieve the active policies and its conformance status by user.
+    This process only supports cross-namespace checking between game namespace and publisher namespace , that means if the active policy already accepted by the same user in publisher namespace, then it will also be considered as eligible in non-publisher namespace.
+
+    Properties:
+        url: /agreement/public/eligibilities/namespaces/{namespace}/countries/{countryCode}/clients/{clientId}/users/{userId}
+
+        method: GET
+
+        tags: ["Eligibilities"]
 
-    # endregion static methods
+        consumes: []
+
+        produces: ["application/json"]
+
+        securities: [BEARER_AUTH]
+
+        client_id: (clientId) REQUIRED str in path
+
+        country_code: (countryCode) REQUIRED str in path
+
+        namespace: (namespace) REQUIRED str in path
+
+        user_id: (userId) REQUIRED str in path
+
+    Responses:
+        200: OK - RetrieveUserEligibilitiesIndirectResponse (successful operation)
+
+        400: Bad Request - ErrorEntity (40045: errors.net.accelbyte.platform.legal.user_id_needed)
+    """
+    if namespace is None:
+        namespace, error = get_services_namespace()
+        if error:
+            return None, error
+    request = RetrieveEligibilitiesPublicIndirect.create(
+        client_id=client_id,
+        country_code=country_code,
+        user_id=user_id,
+        namespace=namespace,
+    )
+    return await run_request_async(
+        request, additional_headers=x_additional_headers, **kwargs
+    )
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/user_info/__init__.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/user_info/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Legal Service."""
 
-__version__ = "1.39.0"
+__version__ = "1.41.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .get_user_info_status import GetUserInfoStatus
 from .invalidate_user_info_cache import InvalidateUserInfoCache
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/user_info/get_user_info_status.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/user_info/get_user_info_status.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,60 +34,66 @@
 
 class GetUserInfoStatus(Operation):
     """Get user info cache status (getUserInfoStatus)
 
     Get user info cache last updated time per namespace.
     The query parameter namespaces can be a list of namespace separated by comma.
     If query parameter namespaces is empty, user info cache status for all available namespaces will be returned.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:*:LEGAL", action=2 (READ)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:*:LEGAL [READ]
 
     Properties:
         url: /agreement/admin/userInfo
 
         method: GET
 
         tags: ["UserInfo"]
 
         consumes: []
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         namespaces: (namespaces) OPTIONAL str in query
 
     Responses:
         200: OK - List[RetrieveUserInfoCacheStatusResponse] (successful operation)
     """
 
     # region fields
 
     _url: str = "/agreement/admin/userInfo"
+    _path: str = "/agreement/admin/userInfo"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
-    _securities: List[List[str]] = [["BEARER_AUTH"], ["BEARER_AUTH"]]
+    _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "legal"
+
     namespaces: str  # OPTIONAL in [query]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/user_info/invalidate_user_info_cache.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/user_info/invalidate_user_info_cache.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,63 +28,69 @@
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 from accelbyte_py_sdk.core import deprecated
 
 
 class InvalidateUserInfoCache(Operation):
-    """Invalidate user info cache (invalidateUserInfoCache)
+    """[DEPRECATED] Invalidate user info cache (invalidateUserInfoCache)
 
     Invalidate user info cache in agreement service.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:*:LEGAL", action=8 (DELETE)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:*:LEGAL [DELETE]
 
     Properties:
         url: /agreement/admin/userInfo
 
         method: DELETE
 
         tags: ["UserInfo"]
 
         consumes: []
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         namespace: (namespace) OPTIONAL str in query
 
     Responses:
         204: No Content - (Successful operation)
     """
 
     # region fields
 
     _url: str = "/agreement/admin/userInfo"
+    _path: str = "/agreement/admin/userInfo"
+    _base_path: str = ""
     _method: str = "DELETE"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
-    _securities: List[List[str]] = [["BEARER_AUTH"], ["BEARER_AUTH"]]
+    _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "legal"
+
     namespace: str  # OPTIONAL in [query]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/user_info/sync_user_info.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/user_info/sync_user_info.py`

 * *Files 16% similar despite different names*

```diff
@@ -28,63 +28,69 @@
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 from accelbyte_py_sdk.core import deprecated
 
 
 class SyncUserInfo(Operation):
-    """Sync user info with iam service  (syncUserInfo)
+    """[DEPRECATED] Sync user info with iam service  (syncUserInfo)
 
     Sync user info cache in agreement service with iam service.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:*:LEGAL", action=4 (UPDATE)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:*:LEGAL [UPDATE]
 
     Properties:
         url: /agreement/admin/userInfo
 
         method: PUT
 
         tags: ["UserInfo"]
 
         consumes: []
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         namespace: (namespace) REQUIRED str in query
 
     Responses:
         200: OK - (Successful operation)
     """
 
     # region fields
 
     _url: str = "/agreement/admin/userInfo"
+    _path: str = "/agreement/admin/userInfo"
+    _base_path: str = ""
     _method: str = "PUT"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
-    _securities: List[List[str]] = [["BEARER_AUTH"], ["BEARER_AUTH"]]
+    _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "legal"
+
     namespace: str  # REQUIRED in [query]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/operations/utility/check_readiness.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/operations/base_legal_policies/retrieve_all_legal_policies.py`

 * *Files 18% similar despite different names*

```diff
@@ -25,62 +25,69 @@
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
-from ...models import LegalReadinessStatusResponse
+from ...models import RetrieveBasePolicyResponse
 
 
-class CheckReadiness(Operation):
-    """Check Legal Data Readiness (checkReadiness)
+class RetrieveAllLegalPolicies(Operation):
+    """Retrieve All Base Legal Policy (retrieveAllLegalPolicies)
 
-    Readiness status defined as at least one legal basePolicy is present and having active basePolicy.
-    Other detail info:
-        * Required permission : resource="NAMESPACE:{namespace}:LEGAL", action=2 (READ)
-
-    Required Permission(s):
-        - NAMESPACE:{namespace}:LEGAL [READ]
+    Retrieve all base policies.
 
     Properties:
-        url: /agreement/public/readiness
+        url: /agreement/admin/base-policies
 
         method: GET
 
-        tags: ["Utility"]
+        tags: ["Base Legal Policies"]
 
         consumes: []
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
     Responses:
-        200: OK - LegalReadinessStatusResponse (successful operation)
+        200: OK - List[RetrieveBasePolicyResponse] (successful operation)
     """
 
     # region fields
 
-    _url: str = "/agreement/public/readiness"
+    _url: str = "/agreement/admin/base-policies"
+    _path: str = "/agreement/admin/base-policies"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
-    _securities: List[List[str]] = [["BEARER_AUTH"], ["BEARER_AUTH"]]
+    _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "legal"
+
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
 
@@ -126,18 +133,20 @@
     # endregion to methods
 
     # region response methods
 
     # noinspection PyMethodMayBeStatic
     def parse_response(
         self, code: int, content_type: str, content: Any
-    ) -> Tuple[Union[None, LegalReadinessStatusResponse], Union[None, HttpResponse]]:
+    ) -> Tuple[
+        Union[None, List[RetrieveBasePolicyResponse]], Union[None, HttpResponse]
+    ]:
         """Parse the given response.
 
-        200: OK - LegalReadinessStatusResponse (successful operation)
+        200: OK - List[RetrieveBasePolicyResponse] (successful operation)
 
         ---: HttpResponse (Undocumented Response)
 
         ---: HttpResponse (Unexpected Content-Type Error)
 
         ---: HttpResponse (Unhandled Error)
         """
@@ -145,35 +154,37 @@
             code=code, content_type=content_type, content=content
         )
         if error is not None:
             return None, None if error.is_no_content() else error
         code, content_type, content = pre_processed_response
 
         if code == 200:
-            return LegalReadinessStatusResponse.create_from_dict(content), None
+            return [
+                RetrieveBasePolicyResponse.create_from_dict(i) for i in content
+            ], None
 
         return self.handle_undocumented_response(
             code=code, content_type=content_type, content=content
         )
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
-    def create(cls, **kwargs) -> CheckReadiness:
+    def create(cls, **kwargs) -> RetrieveAllLegalPolicies:
         instance = cls()
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> CheckReadiness:
+    ) -> RetrieveAllLegalPolicies:
         instance = cls()
         return instance
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {}
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/wrappers/__init__.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/wrappers/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: wrapper-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Legal Service."""
 
-__version__ = "1.39.0"
+__version__ = "1.41.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from ._admin_user_agreement import indirect_bulk_accept_versioned_policy
 from ._admin_user_agreement import indirect_bulk_accept_versioned_policy_async
@@ -35,14 +35,18 @@
 from ._agreement import retrieve_accepted_agreements
 from ._agreement import retrieve_accepted_agreements_async
 from ._agreement import retrieve_agreements_public
 from ._agreement import retrieve_agreements_public_async
 from ._agreement import retrieve_all_users_by_policy_version
 from ._agreement import retrieve_all_users_by_policy_version_async
 
+from ._agreement_with_namespace import download_exported_agreements_in_csv
+from ._agreement_with_namespace import download_exported_agreements_in_csv_async
+from ._agreement_with_namespace import initiate_export_agreements_to_csv
+from ._agreement_with_namespace import initiate_export_agreements_to_csv_async
 from ._agreement_with_namespace import retrieve_accepted_agreements_1
 from ._agreement_with_namespace import retrieve_accepted_agreements_1_async
 from ._agreement_with_namespace import retrieve_accepted_agreements_for_multi_users
 from ._agreement_with_namespace import (
     retrieve_accepted_agreements_for_multi_users_async,
 )
 from ._agreement_with_namespace import retrieve_all_users_by_policy_version_1
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/wrappers/_admin_user_agreement.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/wrappers/_admin_user_agreement.py`

 * *Files 9% similar despite different names*

```diff
@@ -44,32 +44,28 @@
     publisher_user_id: Optional[str] = None,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Admin bulk accept Policy Versions (indirectBulkAcceptVersionedPolicy)
 
-    Accepts many legal policy versions all at once. Supply with localized version policy id and userId to accept an agreement. Other detail info:
-      * Required permission : resource="ADMIN:NAMESPACE:{namespace}:USER:{userId}:LEGAL", action=1 (CREATE)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:LEGAL [CREATE]
+    Accepts many legal policy versions all at once. Supply with localized version policy id and userId to accept an agreement.
 
     Properties:
         url: /agreement/admin/namespaces/{namespace}/users/{userId}/agreements/policies
 
         method: POST
 
         tags: ["Admin User Agreement"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         body: (body) OPTIONAL List[AcceptAgreementRequest] in body
 
         namespace: (namespace) REQUIRED str in path
 
         user_id: (userId) REQUIRED str in path
 
@@ -106,32 +102,28 @@
     publisher_user_id: Optional[str] = None,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Admin bulk accept Policy Versions (indirectBulkAcceptVersionedPolicy)
 
-    Accepts many legal policy versions all at once. Supply with localized version policy id and userId to accept an agreement. Other detail info:
-      * Required permission : resource="ADMIN:NAMESPACE:{namespace}:USER:{userId}:LEGAL", action=1 (CREATE)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:LEGAL [CREATE]
+    Accepts many legal policy versions all at once. Supply with localized version policy id and userId to accept an agreement.
 
     Properties:
         url: /agreement/admin/namespaces/{namespace}/users/{userId}/agreements/policies
 
         method: POST
 
         tags: ["Admin User Agreement"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         body: (body) OPTIONAL List[AcceptAgreementRequest] in body
 
         namespace: (namespace) REQUIRED str in path
 
         user_id: (userId) REQUIRED str in path
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/wrappers/_admin_user_eligibilities.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/wrappers/_admin_user_eligibilities.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,33 +46,26 @@
     **kwargs
 ):
     """Check User Legal Eligibility (adminRetrieveEligibilities)
 
     Retrieve the active policies and its conformance status by user.
     This process only supports cross-namespace checking between game namespace and publisher namespace , that means if the active policy already accepted by the same user in publisher namespace, then it will also be considered as eligible in non-publisher namespace.
 
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:{namespace}:USER:{userId}:LEGAL", action=2 (READ)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:LEGAL [READ]
-
     Properties:
         url: /agreement/admin/namespaces/{namespace}/users/{userId}/eligibilities
 
         method: GET
 
         tags: ["Admin User Eligibilities"]
 
         consumes: []
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         namespace: (namespace) REQUIRED str in path
 
         user_id: (userId) REQUIRED str in path
 
         publisher_user_id: (publisherUserId) OPTIONAL str in query
 
@@ -110,33 +103,26 @@
     **kwargs
 ):
     """Check User Legal Eligibility (adminRetrieveEligibilities)
 
     Retrieve the active policies and its conformance status by user.
     This process only supports cross-namespace checking between game namespace and publisher namespace , that means if the active policy already accepted by the same user in publisher namespace, then it will also be considered as eligible in non-publisher namespace.
 
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:{namespace}:USER:{userId}:LEGAL", action=2 (READ)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:USER:{userId}:LEGAL [READ]
-
     Properties:
         url: /agreement/admin/namespaces/{namespace}/users/{userId}/eligibilities
 
         method: GET
 
         tags: ["Admin User Eligibilities"]
 
         consumes: []
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         namespace: (namespace) REQUIRED str in path
 
         user_id: (userId) REQUIRED str in path
 
         publisher_user_id: (publisherUserId) OPTIONAL str in query
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/wrappers/_agreement.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/wrappers/_agreement.py`

 * *Files 11% similar despite different names*

```diff
@@ -51,18 +51,15 @@
 def accept_versioned_policy(
     localized_policy_version_id: str,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Accept a Policy Version (acceptVersionedPolicy)
 
-    Accepts a legal policy version. Supply with localized version policy id to accept an agreement.
-    Other detail info:
-
-      * Required permission : login user
+    Accepts a legal policy version. Supply with localized version policy id to accept an agreement
 
     Properties:
         url: /agreement/public/agreements/localized-policy-versions/{localizedPolicyVersionId}
 
         method: POST
 
         tags: ["Agreement"]
@@ -90,18 +87,15 @@
 async def accept_versioned_policy_async(
     localized_policy_version_id: str,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Accept a Policy Version (acceptVersionedPolicy)
 
-    Accepts a legal policy version. Supply with localized version policy id to accept an agreement.
-    Other detail info:
-
-      * Required permission : login user
+    Accepts a legal policy version. Supply with localized version policy id to accept an agreement
 
     Properties:
         url: /agreement/public/agreements/localized-policy-versions/{localizedPolicyVersionId}
 
         method: POST
 
         tags: ["Agreement"]
@@ -132,17 +126,14 @@
     body: Optional[List[AcceptAgreementRequest]] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Bulk Accept Policy Versions (bulkAcceptVersionedPolicy)
 
     Accepts many legal policy versions all at once. Supply with localized version policy id to accept an agreement.
-    Other detail info:
-
-      * Required permission : login user
 
     Properties:
         url: /agreement/public/agreements/policies
 
         method: POST
 
         tags: ["Agreement"]
@@ -171,17 +162,14 @@
     body: Optional[List[AcceptAgreementRequest]] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Bulk Accept Policy Versions (bulkAcceptVersionedPolicy)
 
     Accepts many legal policy versions all at once. Supply with localized version policy id to accept an agreement.
-    Other detail info:
-
-      * Required permission : login user
 
     Properties:
         url: /agreement/public/agreements/policies
 
         method: POST
 
         tags: ["Agreement"]
@@ -213,32 +201,28 @@
     body: Optional[List[AcceptAgreementRequest]] = None,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Change Preference Consent (changePreferenceConsent)
 
-    This API will Update Preference Consent. Other detail info:
-      * Required permission : resource="ADMIN:NAMESPACE:{namespace}:LEGAL", action=4 (UPDATE)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:LEGAL [UPDATE]
+    This API will Update Preference Consent
 
     Properties:
         url: /agreement/admin/agreements/localized-policy-versions/preferences/namespaces/{namespace}/userId/{userId}
 
         method: PATCH
 
         tags: ["Agreement"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         body: (body) OPTIONAL List[AcceptAgreementRequest] in body
 
         namespace: (namespace) REQUIRED str in path
 
         user_id: (userId) REQUIRED str in path
 
@@ -265,32 +249,28 @@
     body: Optional[List[AcceptAgreementRequest]] = None,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Change Preference Consent (changePreferenceConsent)
 
-    This API will Update Preference Consent. Other detail info:
-      * Required permission : resource="ADMIN:NAMESPACE:{namespace}:LEGAL", action=4 (UPDATE)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:LEGAL [UPDATE]
+    This API will Update Preference Consent
 
     Properties:
         url: /agreement/admin/agreements/localized-policy-versions/preferences/namespaces/{namespace}/userId/{userId}
 
         method: PATCH
 
         tags: ["Agreement"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         body: (body) OPTIONAL List[AcceptAgreementRequest] in body
 
         namespace: (namespace) REQUIRED str in path
 
         user_id: (userId) REQUIRED str in path
 
@@ -318,17 +298,14 @@
     body: Optional[List[AcceptAgreementRequest]] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Accept/Revoke Marketing Preference Consent (changePreferenceConsent_1)
 
     Change marketing preference consent.
-    Other detail info:
-
-      * Required permission : login user
 
     Properties:
         url: /agreement/public/agreements/localized-policy-versions/preferences
 
         method: PATCH
 
         tags: ["Agreement"]
@@ -357,17 +334,14 @@
     body: Optional[List[AcceptAgreementRequest]] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Accept/Revoke Marketing Preference Consent (changePreferenceConsent_1)
 
     Change marketing preference consent.
-    Other detail info:
-
-      * Required permission : login user
 
     Properties:
         url: /agreement/public/agreements/localized-policy-versions/preferences
 
         method: PATCH
 
         tags: ["Agreement"]
@@ -400,17 +374,14 @@
     body: Optional[List[AcceptAgreementRequest]] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Bulk Accept Policy Versions (Indirect) (indirectBulkAcceptVersionedPolicy_1)
 
     Accepts many legal policy versions all at once. Supply with localized version policy id and userId to accept an agreement. This endpoint used by Authentication Service during new user registration.
-    Other detail info:
-
-      * Required permission : login user
 
     Properties:
         url: /agreement/public/agreements/policies/users/{userId}
 
         method: POST
 
         tags: ["Agreement"]
@@ -444,17 +415,14 @@
     body: Optional[List[AcceptAgreementRequest]] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Bulk Accept Policy Versions (Indirect) (indirectBulkAcceptVersionedPolicy_1)
 
     Accepts many legal policy versions all at once. Supply with localized version policy id and userId to accept an agreement. This endpoint used by Authentication Service during new user registration.
-    Other detail info:
-
-      * Required permission : login user
 
     Properties:
         url: /agreement/public/agreements/policies/users/{userId}
 
         method: POST
 
         tags: ["Agreement"]
@@ -493,33 +461,27 @@
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Bulk Accept Policy Versions (Indirect) (indirectBulkAcceptVersionedPolicyV2)
 
     Accepts many legal policy versions all at once. Supply with localized version policy id, version policy id, policy id, userId, namespace, country code and client id to accept an agreement. This endpoint used by APIGateway during new user registration.
-    Other detail info:
-
-      * Required permission : resource="NAMESPACE:{namespace}:LEGAL", action=1 (CREATE)
-
-    Required Permission(s):
-        - NAMESPACE:{namespace}:LEGAL [CREATE]
 
     Properties:
         url: /agreement/public/agreements/policies/namespaces/{namespace}/countries/{countryCode}/clients/{clientId}/users/{userId}
 
         method: POST
 
         tags: ["Agreement"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         body: (body) OPTIONAL List[AcceptAgreementRequest] in body
 
         client_id: (clientId) REQUIRED str in path
 
         country_code: (countryCode) REQUIRED str in path
 
@@ -554,33 +516,27 @@
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Bulk Accept Policy Versions (Indirect) (indirectBulkAcceptVersionedPolicyV2)
 
     Accepts many legal policy versions all at once. Supply with localized version policy id, version policy id, policy id, userId, namespace, country code and client id to accept an agreement. This endpoint used by APIGateway during new user registration.
-    Other detail info:
-
-      * Required permission : resource="NAMESPACE:{namespace}:LEGAL", action=1 (CREATE)
-
-    Required Permission(s):
-        - NAMESPACE:{namespace}:LEGAL [CREATE]
 
     Properties:
         url: /agreement/public/agreements/policies/namespaces/{namespace}/countries/{countryCode}/clients/{clientId}/users/{userId}
 
         method: POST
 
         tags: ["Agreement"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         body: (body) OPTIONAL List[AcceptAgreementRequest] in body
 
         client_id: (clientId) REQUIRED str in path
 
         country_code: (countryCode) REQUIRED str in path
 
@@ -609,32 +565,28 @@
 
 @same_doc_as(RetrieveAcceptedAgreements)
 def retrieve_accepted_agreements(
     user_id: str, x_additional_headers: Optional[Dict[str, str]] = None, **kwargs
 ):
     """Retrieve Accepted Legal Agreements (retrieveAcceptedAgreements)
 
-    This API will return all accepted Legal Agreements for specified user. Other detail info:
-      * Required permission : resource="ADMIN:NAMESPACE:*:LEGAL", action=2 (READ)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:*:LEGAL [READ]
+    This API will return all accepted Legal Agreements for specified user
 
     Properties:
         url: /agreement/admin/agreements/policies/users/{userId}
 
         method: GET
 
         tags: ["Agreement"]
 
         consumes: []
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         user_id: (userId) REQUIRED str in path
 
     Responses:
         200: OK - List[RetrieveAcceptedAgreementResponse] (successful operation)
     """
     request = RetrieveAcceptedAgreements.create(
@@ -645,32 +597,28 @@
 
 @same_doc_as(RetrieveAcceptedAgreements)
 async def retrieve_accepted_agreements_async(
     user_id: str, x_additional_headers: Optional[Dict[str, str]] = None, **kwargs
 ):
     """Retrieve Accepted Legal Agreements (retrieveAcceptedAgreements)
 
-    This API will return all accepted Legal Agreements for specified user. Other detail info:
-      * Required permission : resource="ADMIN:NAMESPACE:*:LEGAL", action=2 (READ)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:*:LEGAL [READ]
+    This API will return all accepted Legal Agreements for specified user
 
     Properties:
         url: /agreement/admin/agreements/policies/users/{userId}
 
         method: GET
 
         tags: ["Agreement"]
 
         consumes: []
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         user_id: (userId) REQUIRED str in path
 
     Responses:
         200: OK - List[RetrieveAcceptedAgreementResponse] (successful operation)
     """
     request = RetrieveAcceptedAgreements.create(
@@ -684,17 +632,14 @@
 @same_doc_as(RetrieveAgreementsPublic)
 def retrieve_agreements_public(
     x_additional_headers: Optional[Dict[str, str]] = None, **kwargs
 ):
     """Retrieve the accepted Legal Agreements (retrieveAgreementsPublic)
 
     Retrieve accepted Legal Agreements.
-    Other detail info:
-
-      * Required permission : login user
 
     Properties:
         url: /agreement/public/agreements/policies
 
         method: GET
 
         tags: ["Agreement"]
@@ -717,17 +662,14 @@
 @same_doc_as(RetrieveAgreementsPublic)
 async def retrieve_agreements_public_async(
     x_additional_headers: Optional[Dict[str, str]] = None, **kwargs
 ):
     """Retrieve the accepted Legal Agreements (retrieveAgreementsPublic)
 
     Retrieve accepted Legal Agreements.
-    Other detail info:
-
-      * Required permission : login user
 
     Properties:
         url: /agreement/public/agreements/policies
 
         method: GET
 
         tags: ["Agreement"]
@@ -754,34 +696,30 @@
     policy_version_id: str,
     keyword: Optional[str] = None,
     limit: Optional[int] = None,
     offset: Optional[int] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
-    """Retrieve All Users Accepting Legal Agreements (retrieveAllUsersByPolicyVersion)
-
-    This API will return all users who has accepted a specific policy version.Other detail info:
-      * Required permission : resource="ADMIN:NAMESPACE:*:LEGAL", action=2 (READ)
+    """Retrieve Users Accepting Legal Agreements (retrieveAllUsersByPolicyVersion)
 
-    Required Permission(s):
-        - ADMIN:NAMESPACE:*:LEGAL [READ]
+    This API will return users who has accepted a specific policy version.
 
     Properties:
         url: /agreement/admin/agreements/policy-versions/users
 
         method: GET
 
         tags: ["Agreement"]
 
         consumes: []
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         keyword: (keyword) OPTIONAL str in query
 
         limit: (limit) OPTIONAL int in query
 
         offset: (offset) OPTIONAL int in query
 
@@ -806,34 +744,30 @@
     policy_version_id: str,
     keyword: Optional[str] = None,
     limit: Optional[int] = None,
     offset: Optional[int] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
-    """Retrieve All Users Accepting Legal Agreements (retrieveAllUsersByPolicyVersion)
-
-    This API will return all users who has accepted a specific policy version.Other detail info:
-      * Required permission : resource="ADMIN:NAMESPACE:*:LEGAL", action=2 (READ)
+    """Retrieve Users Accepting Legal Agreements (retrieveAllUsersByPolicyVersion)
 
-    Required Permission(s):
-        - ADMIN:NAMESPACE:*:LEGAL [READ]
+    This API will return users who has accepted a specific policy version.
 
     Properties:
         url: /agreement/admin/agreements/policy-versions/users
 
         method: GET
 
         tags: ["Agreement"]
 
         consumes: []
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         keyword: (keyword) OPTIONAL str in query
 
         limit: (limit) OPTIONAL int in query
 
         offset: (offset) OPTIONAL int in query
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/wrappers/_base_legal_policies.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/wrappers/_base_legal_policies.py`

 * *Files 22% similar despite different names*

```diff
@@ -52,33 +52,27 @@
     body: Optional[CreateBasePolicyRequest] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Create a Base Legal Policy (createPolicy)
 
     Create a legal policy.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:*:LEGAL", action=1 (CREATE)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:*:LEGAL [CREATE]
 
     Properties:
         url: /agreement/admin/base-policies
 
         method: POST
 
         tags: ["Base Legal Policies"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         body: (body) OPTIONAL CreateBasePolicyRequest in body
 
     Responses:
         201: Created - CreateBasePolicyResponse (successful operation)
 
         400: Bad Request - ErrorEntity (40038: errors.net.accelbyte.platform.legal.invalid_affected_client_id | 40026: errors.net.accelbyte.platform.legal.not_allow_create_studio_policy)
@@ -98,33 +92,27 @@
     body: Optional[CreateBasePolicyRequest] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Create a Base Legal Policy (createPolicy)
 
     Create a legal policy.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:*:LEGAL", action=1 (CREATE)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:*:LEGAL [CREATE]
 
     Properties:
         url: /agreement/admin/base-policies
 
         method: POST
 
         tags: ["Base Legal Policies"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         body: (body) OPTIONAL CreateBasePolicyRequest in body
 
     Responses:
         201: Created - CreateBasePolicyResponse (successful operation)
 
         400: Bad Request - ErrorEntity (40038: errors.net.accelbyte.platform.legal.invalid_affected_client_id | 40026: errors.net.accelbyte.platform.legal.not_allow_create_studio_policy)
@@ -147,33 +135,27 @@
     body: Optional[UpdateBasePolicyRequest] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Update Base Legal Policy (partialUpdatePolicy)
 
     Update an existing base policy.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:*:LEGAL", action=4 (UPDATE)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:*:LEGAL [UPDATE]
 
     Properties:
         url: /agreement/admin/base-policies/{basePolicyId}
 
         method: PATCH
 
         tags: ["Base Legal Policies"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         body: (body) OPTIONAL UpdateBasePolicyRequest in body
 
         base_policy_id: (basePolicyId) REQUIRED str in path
 
     Responses:
         200: OK - UpdateBasePolicyResponse (successful operation)
@@ -195,33 +177,27 @@
     body: Optional[UpdateBasePolicyRequest] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Update Base Legal Policy (partialUpdatePolicy)
 
     Update an existing base policy.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:*:LEGAL", action=4 (UPDATE)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:*:LEGAL [UPDATE]
 
     Properties:
         url: /agreement/admin/base-policies/{basePolicyId}
 
         method: PATCH
 
         tags: ["Base Legal Policies"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         body: (body) OPTIONAL UpdateBasePolicyRequest in body
 
         base_policy_id: (basePolicyId) REQUIRED str in path
 
     Responses:
         200: OK - UpdateBasePolicyResponse (successful operation)
@@ -242,33 +218,27 @@
 @same_doc_as(RetrieveAllLegalPolicies)
 def retrieve_all_legal_policies(
     x_additional_headers: Optional[Dict[str, str]] = None, **kwargs
 ):
     """Retrieve All Base Legal Policy (retrieveAllLegalPolicies)
 
     Retrieve all base policies.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:*:LEGAL", action=2 (READ)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:*:LEGAL [READ]
 
     Properties:
         url: /agreement/admin/base-policies
 
         method: GET
 
         tags: ["Base Legal Policies"]
 
         consumes: []
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
     Responses:
         200: OK - List[RetrieveBasePolicyResponse] (successful operation)
     """
     request = RetrieveAllLegalPolicies.create()
     return run_request(request, additional_headers=x_additional_headers, **kwargs)
 
@@ -276,33 +246,27 @@
 @same_doc_as(RetrieveAllLegalPolicies)
 async def retrieve_all_legal_policies_async(
     x_additional_headers: Optional[Dict[str, str]] = None, **kwargs
 ):
     """Retrieve All Base Legal Policy (retrieveAllLegalPolicies)
 
     Retrieve all base policies.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:*:LEGAL", action=2 (READ)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:*:LEGAL [READ]
 
     Properties:
         url: /agreement/admin/base-policies
 
         method: GET
 
         tags: ["Base Legal Policies"]
 
         consumes: []
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
     Responses:
         200: OK - List[RetrieveBasePolicyResponse] (successful operation)
     """
     request = RetrieveAllLegalPolicies.create()
     return await run_request_async(
         request, additional_headers=x_additional_headers, **kwargs
@@ -315,33 +279,27 @@
     offset: Optional[int] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Retrieve All Policy Type (retrieveAllPolicyTypes)
 
     Retrieve all supported policy types.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:*:LEGAL", action=2 (READ)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:*:LEGAL [READ]
 
     Properties:
         url: /agreement/admin/policy-types
 
         method: GET
 
         tags: ["Base Legal Policies"]
 
         consumes: []
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         offset: (offset) OPTIONAL int in query
 
         limit: (limit) REQUIRED int in query
 
     Responses:
         200: OK - List[RetrievePolicyTypeResponse] (successful operation)
@@ -359,33 +317,27 @@
     offset: Optional[int] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Retrieve All Policy Type (retrieveAllPolicyTypes)
 
     Retrieve all supported policy types.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:*:LEGAL", action=2 (READ)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:*:LEGAL [READ]
 
     Properties:
         url: /agreement/admin/policy-types
 
         method: GET
 
         tags: ["Base Legal Policies"]
 
         consumes: []
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         offset: (offset) OPTIONAL int in query
 
         limit: (limit) REQUIRED int in query
 
     Responses:
         200: OK - List[RetrievePolicyTypeResponse] (successful operation)
@@ -405,33 +357,27 @@
     country_code: str,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Retrieve a Base Legal Policy based on a Particular Country (retrievePolicyCountry)
 
     Retrieve a Base Legal Policy based on a Particular Country.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:*:LEGAL", action=2 (READ)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:*:LEGAL [READ]
 
     Properties:
         url: /agreement/admin/base-policies/{basePolicyId}/countries/{countryCode}
 
         method: GET
 
         tags: ["Base Legal Policies"]
 
         consumes: []
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         base_policy_id: (basePolicyId) REQUIRED str in path
 
         country_code: (countryCode) REQUIRED str in path
 
     Responses:
         200: OK - RetrievePolicyResponse (successful operation)
@@ -451,33 +397,27 @@
     country_code: str,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Retrieve a Base Legal Policy based on a Particular Country (retrievePolicyCountry)
 
     Retrieve a Base Legal Policy based on a Particular Country.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:*:LEGAL", action=2 (READ)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:*:LEGAL [READ]
 
     Properties:
         url: /agreement/admin/base-policies/{basePolicyId}/countries/{countryCode}
 
         method: GET
 
         tags: ["Base Legal Policies"]
 
         consumes: []
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         base_policy_id: (basePolicyId) REQUIRED str in path
 
         country_code: (countryCode) REQUIRED str in path
 
     Responses:
         200: OK - RetrievePolicyResponse (successful operation)
@@ -496,33 +436,27 @@
 @same_doc_as(RetrieveSinglePolicy)
 def retrieve_single_policy(
     base_policy_id: str, x_additional_headers: Optional[Dict[str, str]] = None, **kwargs
 ):
     """Retrieve a Base Legal Policy (retrieveSinglePolicy)
 
     Retrieve a base policy.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:*:LEGAL", action=2 (READ)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:*:LEGAL [READ]
 
     Properties:
         url: /agreement/admin/base-policies/{basePolicyId}
 
         method: GET
 
         tags: ["Base Legal Policies"]
 
         consumes: []
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         base_policy_id: (basePolicyId) REQUIRED str in path
 
     Responses:
         200: OK - RetrieveBasePolicyResponse (successful operation)
 
         404: Not Found - ErrorEntity (40031: errors.net.accelbyte.platform.legal.base_policy_not_found)
@@ -536,33 +470,27 @@
 @same_doc_as(RetrieveSinglePolicy)
 async def retrieve_single_policy_async(
     base_policy_id: str, x_additional_headers: Optional[Dict[str, str]] = None, **kwargs
 ):
     """Retrieve a Base Legal Policy (retrieveSinglePolicy)
 
     Retrieve a base policy.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:*:LEGAL", action=2 (READ)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:*:LEGAL [READ]
 
     Properties:
         url: /agreement/admin/base-policies/{basePolicyId}
 
         method: GET
 
         tags: ["Base Legal Policies"]
 
         consumes: []
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         base_policy_id: (basePolicyId) REQUIRED str in path
 
     Responses:
         200: OK - RetrieveBasePolicyResponse (successful operation)
 
         404: Not Found - ErrorEntity (40031: errors.net.accelbyte.platform.legal.base_policy_not_found)
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/wrappers/_base_legal_policies_with_namespace.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/wrappers/_base_legal_policies_with_namespace.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,33 +55,27 @@
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Create a Base Legal Policy (createPolicy_1)
 
     Create a legal policy.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:{namespace}:LEGAL", action=1 (CREATE)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:LEGAL [CREATE]
 
     Properties:
         url: /agreement/admin/namespaces/{namespace}/base-policies
 
         method: POST
 
         tags: ["Base Legal Policies With Namespace"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         body: (body) OPTIONAL CreateBasePolicyRequestV2 in body
 
         namespace: (namespace) REQUIRED str in path
 
     Responses:
         201: Created - CreateBasePolicyResponse (successful operation)
@@ -109,33 +103,27 @@
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Create a Base Legal Policy (createPolicy_1)
 
     Create a legal policy.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:{namespace}:LEGAL", action=1 (CREATE)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:LEGAL [CREATE]
 
     Properties:
         url: /agreement/admin/namespaces/{namespace}/base-policies
 
         method: POST
 
         tags: ["Base Legal Policies With Namespace"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         body: (body) OPTIONAL CreateBasePolicyRequestV2 in body
 
         namespace: (namespace) REQUIRED str in path
 
     Responses:
         201: Created - CreateBasePolicyResponse (successful operation)
@@ -166,33 +154,27 @@
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Update Base Legal Policy (partialUpdatePolicy_1)
 
     Update an existing base policy.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:{namespace}:LEGAL", action=4 (UPDATE)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:LEGAL [UPDATE]
 
     Properties:
         url: /agreement/admin/namespaces/{namespace}/base-policies/{basePolicyId}
 
         method: PATCH
 
         tags: ["Base Legal Policies With Namespace"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         body: (body) OPTIONAL UpdateBasePolicyRequestV2 in body
 
         base_policy_id: (basePolicyId) REQUIRED str in path
 
         namespace: (namespace) REQUIRED str in path
 
@@ -220,33 +202,27 @@
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Update Base Legal Policy (partialUpdatePolicy_1)
 
     Update an existing base policy.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:{namespace}:LEGAL", action=4 (UPDATE)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:LEGAL [UPDATE]
 
     Properties:
         url: /agreement/admin/namespaces/{namespace}/base-policies/{basePolicyId}
 
         method: PATCH
 
         tags: ["Base Legal Policies With Namespace"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         body: (body) OPTIONAL UpdateBasePolicyRequestV2 in body
 
         base_policy_id: (basePolicyId) REQUIRED str in path
 
         namespace: (namespace) REQUIRED str in path
 
@@ -274,33 +250,27 @@
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Retrieve All Base Legal Policy in the namespace (retrieveAllLegalPoliciesByNamespace)
 
     Retrieve all base policies in the namespace.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:{namespace}:LEGAL", action=2 (READ)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:LEGAL [READ]
 
     Properties:
         url: /agreement/admin/namespaces/{namespace}/base-policies
 
         method: GET
 
         tags: ["Base Legal Policies With Namespace"]
 
         consumes: []
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         namespace: (namespace) REQUIRED str in path
 
     Responses:
         200: OK - List[RetrieveBasePolicyResponse] (successful operation)
     """
     if namespace is None:
@@ -318,33 +288,27 @@
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Retrieve All Base Legal Policy in the namespace (retrieveAllLegalPoliciesByNamespace)
 
     Retrieve all base policies in the namespace.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:{namespace}:LEGAL", action=2 (READ)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:LEGAL [READ]
 
     Properties:
         url: /agreement/admin/namespaces/{namespace}/base-policies
 
         method: GET
 
         tags: ["Base Legal Policies With Namespace"]
 
         consumes: []
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         namespace: (namespace) REQUIRED str in path
 
     Responses:
         200: OK - List[RetrieveBasePolicyResponse] (successful operation)
     """
     if namespace is None:
@@ -366,33 +330,27 @@
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Retrieve All Policy Type (retrieveAllPolicyTypes_1)
 
     Retrieve all supported policy types.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:{namespace}:LEGAL", action=2 (READ)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:LEGAL [READ]
 
     Properties:
         url: /agreement/admin/namespaces/{namespace}/policy-types
 
         method: GET
 
         tags: ["Base Legal Policies With Namespace"]
 
         consumes: []
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         namespace: (namespace) REQUIRED str in path
 
         offset: (offset) OPTIONAL int in query
 
         limit: (limit) REQUIRED int in query
 
@@ -418,33 +376,27 @@
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Retrieve All Policy Type (retrieveAllPolicyTypes_1)
 
     Retrieve all supported policy types.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:{namespace}:LEGAL", action=2 (READ)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:LEGAL [READ]
 
     Properties:
         url: /agreement/admin/namespaces/{namespace}/policy-types
 
         method: GET
 
         tags: ["Base Legal Policies With Namespace"]
 
         consumes: []
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         namespace: (namespace) REQUIRED str in path
 
         offset: (offset) OPTIONAL int in query
 
         limit: (limit) REQUIRED int in query
 
@@ -472,33 +424,27 @@
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Retrieve a Base Legal Policy based on a Particular Country (retrievePolicyCountry_1)
 
     Retrieve a Base Legal Policy based on a Particular Country.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:{namespace}:LEGAL", action=2 (READ)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:LEGAL [READ]
 
     Properties:
         url: /agreement/admin/namespaces/{namespace}/base-policies/{basePolicyId}/countries/{countryCode}
 
         method: GET
 
         tags: ["Base Legal Policies With Namespace"]
 
         consumes: []
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         base_policy_id: (basePolicyId) REQUIRED str in path
 
         country_code: (countryCode) REQUIRED str in path
 
         namespace: (namespace) REQUIRED str in path
 
@@ -526,33 +472,27 @@
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Retrieve a Base Legal Policy based on a Particular Country (retrievePolicyCountry_1)
 
     Retrieve a Base Legal Policy based on a Particular Country.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:{namespace}:LEGAL", action=2 (READ)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:LEGAL [READ]
 
     Properties:
         url: /agreement/admin/namespaces/{namespace}/base-policies/{basePolicyId}/countries/{countryCode}
 
         method: GET
 
         tags: ["Base Legal Policies With Namespace"]
 
         consumes: []
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         base_policy_id: (basePolicyId) REQUIRED str in path
 
         country_code: (countryCode) REQUIRED str in path
 
         namespace: (namespace) REQUIRED str in path
 
@@ -581,33 +521,27 @@
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Retrieve a Base Legal Policy (retrieveSinglePolicy_1)
 
     Retrieve a base policy.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:{namespace}:LEGAL", action=2 (READ)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:LEGAL [READ]
 
     Properties:
         url: /agreement/admin/namespaces/{namespace}/base-policies/{basePolicyId}
 
         method: GET
 
         tags: ["Base Legal Policies With Namespace"]
 
         consumes: []
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         base_policy_id: (basePolicyId) REQUIRED str in path
 
         namespace: (namespace) REQUIRED str in path
 
     Responses:
         200: OK - RetrieveBasePolicyResponse (successful operation)
@@ -631,33 +565,27 @@
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Retrieve a Base Legal Policy (retrieveSinglePolicy_1)
 
     Retrieve a base policy.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:{namespace}:LEGAL", action=2 (READ)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:LEGAL [READ]
 
     Properties:
         url: /agreement/admin/namespaces/{namespace}/base-policies/{basePolicyId}
 
         method: GET
 
         tags: ["Base Legal Policies With Namespace"]
 
         consumes: []
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         base_policy_id: (basePolicyId) REQUIRED str in path
 
         namespace: (namespace) REQUIRED str in path
 
     Responses:
         200: OK - RetrieveBasePolicyResponse (successful operation)
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/wrappers/_eligibilities.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/wrappers/_user_info.py`

 * *Files 22% similar despite different names*

```diff
@@ -23,223 +23,241 @@
 
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import get_namespace as get_services_namespace
 from accelbyte_py_sdk.core import run_request
 from accelbyte_py_sdk.core import run_request_async
+from accelbyte_py_sdk.core import deprecated
 from accelbyte_py_sdk.core import same_doc_as
 
-from ..models import ErrorEntity
-from ..models import RetrieveUserEligibilitiesIndirectResponse
-from ..models import RetrieveUserEligibilitiesResponse
+from ..models import RetrieveUserInfoCacheStatusResponse
 
-from ..operations.eligibilities import RetrieveEligibilitiesPublic
-from ..operations.eligibilities import RetrieveEligibilitiesPublicIndirect
+from ..operations.user_info import GetUserInfoStatus
+from ..operations.user_info import InvalidateUserInfoCache
+from ..operations.user_info import SyncUserInfo
 
 
-@same_doc_as(RetrieveEligibilitiesPublic)
-def retrieve_eligibilities_public(
-    namespace: Optional[str] = None,
+@same_doc_as(GetUserInfoStatus)
+def get_user_info_status(
+    namespaces: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
-    """Check User Legal Eligibility (retrieveEligibilitiesPublic)
+    """Get user info cache status (getUserInfoStatus)
+
+    Get user info cache last updated time per namespace.
+    The query parameter namespaces can be a list of namespace separated by comma.
+    If query parameter namespaces is empty, user info cache status for all available namespaces will be returned.
+
+    Properties:
+        url: /agreement/admin/userInfo
+
+        method: GET
+
+        tags: ["UserInfo"]
+
+        consumes: []
 
-    Retrieve the active policies and its conformance status by user.
-    This process supports cross-namespace checking, that means if the active policy already accepted by the same user in other namespace, then it will be considered as eligible.
+        produces: ["application/json"]
+
+        securities: [BEARER_AUTH]
+
+        namespaces: (namespaces) OPTIONAL str in query
+
+    Responses:
+        200: OK - List[RetrieveUserInfoCacheStatusResponse] (successful operation)
+    """
+    request = GetUserInfoStatus.create(
+        namespaces=namespaces,
+    )
+    return run_request(request, additional_headers=x_additional_headers, **kwargs)
 
-    Other detail info:
-        * Required permission : login user
+
+@same_doc_as(GetUserInfoStatus)
+async def get_user_info_status_async(
+    namespaces: Optional[str] = None,
+    x_additional_headers: Optional[Dict[str, str]] = None,
+    **kwargs
+):
+    """Get user info cache status (getUserInfoStatus)
+
+    Get user info cache last updated time per namespace.
+    The query parameter namespaces can be a list of namespace separated by comma.
+    If query parameter namespaces is empty, user info cache status for all available namespaces will be returned.
 
     Properties:
-        url: /agreement/public/eligibilities/namespaces/{namespace}
+        url: /agreement/admin/userInfo
 
         method: GET
 
-        tags: ["Eligibilities"]
+        tags: ["UserInfo"]
 
         consumes: []
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
-        namespace: (namespace) REQUIRED str in path
+        namespaces: (namespaces) OPTIONAL str in query
 
     Responses:
-        200: OK - List[RetrieveUserEligibilitiesResponse] (successful operation)
+        200: OK - List[RetrieveUserInfoCacheStatusResponse] (successful operation)
+    """
+    request = GetUserInfoStatus.create(
+        namespaces=namespaces,
+    )
+    return await run_request_async(
+        request, additional_headers=x_additional_headers, **kwargs
+    )
+
+
+@deprecated
+@same_doc_as(InvalidateUserInfoCache)
+def invalidate_user_info_cache(
+    namespace: Optional[str] = None,
+    x_additional_headers: Optional[Dict[str, str]] = None,
+    **kwargs
+):
+    """Invalidate user info cache (invalidateUserInfoCache)
+
+    Invalidate user info cache in agreement service.
 
-        400: Bad Request - ErrorEntity (40045: errors.net.accelbyte.platform.legal.user_id_needed)
+    Properties:
+        url: /agreement/admin/userInfo
+
+        method: DELETE
+
+        tags: ["UserInfo"]
+
+        consumes: []
+
+        produces: ["application/json"]
+
+        securities: [BEARER_AUTH]
 
-        404: Not Found - ErrorEntity (40041: errors.net.accelbyte.platform.legal.policy_not_found)
+        namespace: (namespace) OPTIONAL str in query
+
+    Responses:
+        204: No Content - (Successful operation)
     """
-    if namespace is None:
-        namespace, error = get_services_namespace()
-        if error:
-            return None, error
-    request = RetrieveEligibilitiesPublic.create(
+    request = InvalidateUserInfoCache.create(
         namespace=namespace,
     )
     return run_request(request, additional_headers=x_additional_headers, **kwargs)
 
 
-@same_doc_as(RetrieveEligibilitiesPublic)
-async def retrieve_eligibilities_public_async(
+@deprecated
+@same_doc_as(InvalidateUserInfoCache)
+async def invalidate_user_info_cache_async(
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
-    """Check User Legal Eligibility (retrieveEligibilitiesPublic)
-
-    Retrieve the active policies and its conformance status by user.
-    This process supports cross-namespace checking, that means if the active policy already accepted by the same user in other namespace, then it will be considered as eligible.
+    """Invalidate user info cache (invalidateUserInfoCache)
 
-    Other detail info:
-        * Required permission : login user
+    Invalidate user info cache in agreement service.
 
     Properties:
-        url: /agreement/public/eligibilities/namespaces/{namespace}
+        url: /agreement/admin/userInfo
 
-        method: GET
+        method: DELETE
 
-        tags: ["Eligibilities"]
+        tags: ["UserInfo"]
 
         consumes: []
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
-        namespace: (namespace) REQUIRED str in path
+        namespace: (namespace) OPTIONAL str in query
 
     Responses:
-        200: OK - List[RetrieveUserEligibilitiesResponse] (successful operation)
-
-        400: Bad Request - ErrorEntity (40045: errors.net.accelbyte.platform.legal.user_id_needed)
-
-        404: Not Found - ErrorEntity (40041: errors.net.accelbyte.platform.legal.policy_not_found)
+        204: No Content - (Successful operation)
     """
-    if namespace is None:
-        namespace, error = get_services_namespace()
-        if error:
-            return None, error
-    request = RetrieveEligibilitiesPublic.create(
+    request = InvalidateUserInfoCache.create(
         namespace=namespace,
     )
     return await run_request_async(
         request, additional_headers=x_additional_headers, **kwargs
     )
 
 
-@same_doc_as(RetrieveEligibilitiesPublicIndirect)
-def retrieve_eligibilities_public_indirect(
-    client_id: str,
-    country_code: str,
-    user_id: str,
+@deprecated
+@same_doc_as(SyncUserInfo)
+def sync_user_info(
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
-    """Check User Legal Eligibility (retrieveEligibilitiesPublicIndirect)
+    """Sync user info with iam service  (syncUserInfo)
 
-    Retrieve the active policies and its conformance status by user.
-    This process only supports cross-namespace checking between game namespace and publisher namespace , that means if the active policy already accepted by the same user in publisher namespace, then it will also be considered as eligible in non-publisher namespace.
-
-    Other detail info:
-        * Required permission : login user
+    Sync user info cache in agreement service with iam service.
 
     Properties:
-        url: /agreement/public/eligibilities/namespaces/{namespace}/countries/{countryCode}/clients/{clientId}/users/{userId}
+        url: /agreement/admin/userInfo
 
-        method: GET
+        method: PUT
 
-        tags: ["Eligibilities"]
+        tags: ["UserInfo"]
 
         consumes: []
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
-        client_id: (clientId) REQUIRED str in path
-
-        country_code: (countryCode) REQUIRED str in path
-
-        namespace: (namespace) REQUIRED str in path
-
-        user_id: (userId) REQUIRED str in path
+        namespace: (namespace) REQUIRED str in query
 
     Responses:
-        200: OK - RetrieveUserEligibilitiesIndirectResponse (successful operation)
-
-        400: Bad Request - ErrorEntity (40045: errors.net.accelbyte.platform.legal.user_id_needed)
+        200: OK - (Successful operation)
     """
     if namespace is None:
         namespace, error = get_services_namespace()
         if error:
             return None, error
-    request = RetrieveEligibilitiesPublicIndirect.create(
-        client_id=client_id,
-        country_code=country_code,
-        user_id=user_id,
+    request = SyncUserInfo.create(
         namespace=namespace,
     )
     return run_request(request, additional_headers=x_additional_headers, **kwargs)
 
 
-@same_doc_as(RetrieveEligibilitiesPublicIndirect)
-async def retrieve_eligibilities_public_indirect_async(
-    client_id: str,
-    country_code: str,
-    user_id: str,
+@deprecated
+@same_doc_as(SyncUserInfo)
+async def sync_user_info_async(
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
-    """Check User Legal Eligibility (retrieveEligibilitiesPublicIndirect)
+    """Sync user info with iam service  (syncUserInfo)
 
-    Retrieve the active policies and its conformance status by user.
-    This process only supports cross-namespace checking between game namespace and publisher namespace , that means if the active policy already accepted by the same user in publisher namespace, then it will also be considered as eligible in non-publisher namespace.
-
-    Other detail info:
-        * Required permission : login user
+    Sync user info cache in agreement service with iam service.
 
     Properties:
-        url: /agreement/public/eligibilities/namespaces/{namespace}/countries/{countryCode}/clients/{clientId}/users/{userId}
+        url: /agreement/admin/userInfo
 
-        method: GET
+        method: PUT
 
-        tags: ["Eligibilities"]
+        tags: ["UserInfo"]
 
         consumes: []
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
-        client_id: (clientId) REQUIRED str in path
-
-        country_code: (countryCode) REQUIRED str in path
-
-        namespace: (namespace) REQUIRED str in path
-
-        user_id: (userId) REQUIRED str in path
+        namespace: (namespace) REQUIRED str in query
 
     Responses:
-        200: OK - RetrieveUserEligibilitiesIndirectResponse (successful operation)
-
-        400: Bad Request - ErrorEntity (40045: errors.net.accelbyte.platform.legal.user_id_needed)
+        200: OK - (Successful operation)
     """
     if namespace is None:
         namespace, error = get_services_namespace()
         if error:
             return None, error
-    request = RetrieveEligibilitiesPublicIndirect.create(
-        client_id=client_id,
-        country_code=country_code,
-        user_id=user_id,
+    request = SyncUserInfo.create(
         namespace=namespace,
     )
     return await run_request_async(
         request, additional_headers=x_additional_headers, **kwargs
     )
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/wrappers/_localized_policy_versions.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/wrappers/_localized_policy_versions_with_namespace.py`

 * *Files 12% similar despite different names*

```diff
@@ -35,632 +35,678 @@
 from ..models import RetrieveLocalizedPolicyVersionPublicResponse
 from ..models import RetrieveLocalizedPolicyVersionResponse
 from ..models import UpdateLocalizedPolicyVersionRequest
 from ..models import UpdateLocalizedPolicyVersionResponse
 from ..models import UploadLocalizedPolicyVersionAttachmentResponse
 from ..models import UploadPolicyVersionAttachmentRequest
 
-from ..operations.localized_policy_versions import CreateLocalizedPolicyVersion
-from ..operations.localized_policy_versions import RequestPresignedURL
-from ..operations.localized_policy_versions import RetrieveLocalizedPolicyVersions
-from ..operations.localized_policy_versions import RetrieveSingleLocalizedPolicyVersion
-from ..operations.localized_policy_versions import RetrieveSingleLocalizedPolicyVersion2
-from ..operations.localized_policy_versions import SetDefaultPolicy
-from ..operations.localized_policy_versions import UpdateLocalizedPolicyVersion
+from ..operations.localized_policy_versions_with_namespace import (
+    CreateLocalizedPolicyVersion1,
+)
+from ..operations.localized_policy_versions_with_namespace import RequestPresignedURL1
+from ..operations.localized_policy_versions_with_namespace import (
+    RetrieveLocalizedPolicyVersions1,
+)
+from ..operations.localized_policy_versions_with_namespace import (
+    RetrieveSingleLocalizedPolicyVersion1,
+)
+from ..operations.localized_policy_versions_with_namespace import (
+    RetrieveSingleLocalizedPolicyVersion3,
+)
+from ..operations.localized_policy_versions_with_namespace import SetDefaultPolicy1
+from ..operations.localized_policy_versions_with_namespace import (
+    UpdateLocalizedPolicyVersion1,
+)
 
 
-@same_doc_as(CreateLocalizedPolicyVersion)
-def create_localized_policy_version(
+@same_doc_as(CreateLocalizedPolicyVersion1)
+def create_localized_policy_version_1(
     policy_version_id: str,
     body: Optional[CreateLocalizedPolicyVersionRequest] = None,
+    namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
-    """Create a Localized Version from Country-Specific Policy (createLocalizedPolicyVersion)
+    """Create a Localized Version from Country-Specific Policy (createLocalizedPolicyVersion_1)
 
     Create a version of a particular country-specific policy.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:*:LEGAL", action=1 (CREATE)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:*:LEGAL [CREATE]
 
     Properties:
-        url: /agreement/admin/localized-policy-versions/versions/{policyVersionId}
+        url: /agreement/admin/namespaces/{namespace}/localized-policy-versions/versions/{policyVersionId}
 
         method: POST
 
-        tags: ["Localized Policy Versions"]
+        tags: ["Localized Policy Versions With Namespace"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         body: (body) OPTIONAL CreateLocalizedPolicyVersionRequest in body
 
+        namespace: (namespace) REQUIRED str in path
+
         policy_version_id: (policyVersionId) REQUIRED str in path
 
     Responses:
         201: Created - CreateLocalizedPolicyVersionResponse (successful operation)
 
         400: Bad Request - ErrorEntity (40033: errors.net.accelbyte.platform.legal.invalid_policy_version)
 
         409: Conflict - ErrorEntity (40044: errors.net.accelbyte.platform.legal.localized_policy_version_already_exist)
     """
-    request = CreateLocalizedPolicyVersion.create(
+    if namespace is None:
+        namespace, error = get_services_namespace()
+        if error:
+            return None, error
+    request = CreateLocalizedPolicyVersion1.create(
         policy_version_id=policy_version_id,
         body=body,
+        namespace=namespace,
     )
     return run_request(request, additional_headers=x_additional_headers, **kwargs)
 
 
-@same_doc_as(CreateLocalizedPolicyVersion)
-async def create_localized_policy_version_async(
+@same_doc_as(CreateLocalizedPolicyVersion1)
+async def create_localized_policy_version_1_async(
     policy_version_id: str,
     body: Optional[CreateLocalizedPolicyVersionRequest] = None,
+    namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
-    """Create a Localized Version from Country-Specific Policy (createLocalizedPolicyVersion)
+    """Create a Localized Version from Country-Specific Policy (createLocalizedPolicyVersion_1)
 
     Create a version of a particular country-specific policy.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:*:LEGAL", action=1 (CREATE)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:*:LEGAL [CREATE]
 
     Properties:
-        url: /agreement/admin/localized-policy-versions/versions/{policyVersionId}
+        url: /agreement/admin/namespaces/{namespace}/localized-policy-versions/versions/{policyVersionId}
 
         method: POST
 
-        tags: ["Localized Policy Versions"]
+        tags: ["Localized Policy Versions With Namespace"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         body: (body) OPTIONAL CreateLocalizedPolicyVersionRequest in body
 
+        namespace: (namespace) REQUIRED str in path
+
         policy_version_id: (policyVersionId) REQUIRED str in path
 
     Responses:
         201: Created - CreateLocalizedPolicyVersionResponse (successful operation)
 
         400: Bad Request - ErrorEntity (40033: errors.net.accelbyte.platform.legal.invalid_policy_version)
 
         409: Conflict - ErrorEntity (40044: errors.net.accelbyte.platform.legal.localized_policy_version_already_exist)
     """
-    request = CreateLocalizedPolicyVersion.create(
+    if namespace is None:
+        namespace, error = get_services_namespace()
+        if error:
+            return None, error
+    request = CreateLocalizedPolicyVersion1.create(
         policy_version_id=policy_version_id,
         body=body,
+        namespace=namespace,
     )
     return await run_request_async(
         request, additional_headers=x_additional_headers, **kwargs
     )
 
 
-@same_doc_as(RequestPresignedURL)
-def request_presigned_url(
+@same_doc_as(RequestPresignedURL1)
+def request_presigned_url_1(
     localized_policy_version_id: str,
     body: Optional[UploadPolicyVersionAttachmentRequest] = None,
+    namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
-    """Request Presigned URL for Upload Document (requestPresignedURL)
+    """Request Presigned URL for Upload Document (requestPresignedURL_1)
 
     Request presigned URL for upload attachment for a particular localized version of base policy.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:*:LEGAL", action=1 (CREATE)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:*:LEGAL [CREATE]
 
     Properties:
-        url: /agreement/admin/localized-policy-versions/{localizedPolicyVersionId}/attachments
+        url: /agreement/admin/namespaces/{namespace}/localized-policy-versions/{localizedPolicyVersionId}/attachments
 
         method: POST
 
-        tags: ["Localized Policy Versions"]
+        tags: ["Localized Policy Versions With Namespace"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         body: (body) OPTIONAL UploadPolicyVersionAttachmentRequest in body
 
         localized_policy_version_id: (localizedPolicyVersionId) REQUIRED str in path
 
+        namespace: (namespace) REQUIRED str in path
+
     Responses:
         201: Created - UploadLocalizedPolicyVersionAttachmentResponse (successful operation)
 
         400: Bad Request - ErrorEntity (40034: errors.net.accelbyte.platform.legal.invalid_file_type | 40037: errors.net.accelbyte.platform.legal.invalid_localized_policy_version | 40042: errors.net.accelbyte.platform.legal.policy_version_freezed)
     """
-    request = RequestPresignedURL.create(
+    if namespace is None:
+        namespace, error = get_services_namespace()
+        if error:
+            return None, error
+    request = RequestPresignedURL1.create(
         localized_policy_version_id=localized_policy_version_id,
         body=body,
+        namespace=namespace,
     )
     return run_request(request, additional_headers=x_additional_headers, **kwargs)
 
 
-@same_doc_as(RequestPresignedURL)
-async def request_presigned_url_async(
+@same_doc_as(RequestPresignedURL1)
+async def request_presigned_url_1_async(
     localized_policy_version_id: str,
     body: Optional[UploadPolicyVersionAttachmentRequest] = None,
+    namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
-    """Request Presigned URL for Upload Document (requestPresignedURL)
+    """Request Presigned URL for Upload Document (requestPresignedURL_1)
 
     Request presigned URL for upload attachment for a particular localized version of base policy.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:*:LEGAL", action=1 (CREATE)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:*:LEGAL [CREATE]
 
     Properties:
-        url: /agreement/admin/localized-policy-versions/{localizedPolicyVersionId}/attachments
+        url: /agreement/admin/namespaces/{namespace}/localized-policy-versions/{localizedPolicyVersionId}/attachments
 
         method: POST
 
-        tags: ["Localized Policy Versions"]
+        tags: ["Localized Policy Versions With Namespace"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         body: (body) OPTIONAL UploadPolicyVersionAttachmentRequest in body
 
         localized_policy_version_id: (localizedPolicyVersionId) REQUIRED str in path
 
+        namespace: (namespace) REQUIRED str in path
+
     Responses:
         201: Created - UploadLocalizedPolicyVersionAttachmentResponse (successful operation)
 
         400: Bad Request - ErrorEntity (40034: errors.net.accelbyte.platform.legal.invalid_file_type | 40037: errors.net.accelbyte.platform.legal.invalid_localized_policy_version | 40042: errors.net.accelbyte.platform.legal.policy_version_freezed)
     """
-    request = RequestPresignedURL.create(
+    if namespace is None:
+        namespace, error = get_services_namespace()
+        if error:
+            return None, error
+    request = RequestPresignedURL1.create(
         localized_policy_version_id=localized_policy_version_id,
         body=body,
+        namespace=namespace,
     )
     return await run_request_async(
         request, additional_headers=x_additional_headers, **kwargs
     )
 
 
-@same_doc_as(RetrieveLocalizedPolicyVersions)
-def retrieve_localized_policy_versions(
+@same_doc_as(RetrieveLocalizedPolicyVersions1)
+def retrieve_localized_policy_versions_1(
     policy_version_id: str,
+    namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
-    """Retrieve Versions from Country-Specific Policy (retrieveLocalizedPolicyVersions)
+    """Retrieve Versions from Country-Specific Policy (retrieveLocalizedPolicyVersions_1)
 
     Retrieve versions of a particular country-specific policy.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:*:LEGAL", action=2 (READ)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:*:LEGAL [READ]
 
     Properties:
-        url: /agreement/admin/localized-policy-versions/versions/{policyVersionId}
+        url: /agreement/admin/namespaces/{namespace}/localized-policy-versions/versions/{policyVersionId}
 
         method: GET
 
-        tags: ["Localized Policy Versions"]
+        tags: ["Localized Policy Versions With Namespace"]
 
         consumes: []
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
+
+        namespace: (namespace) REQUIRED str in path
 
         policy_version_id: (policyVersionId) REQUIRED str in path
 
     Responses:
         200: OK - List[RetrieveLocalizedPolicyVersionResponse] (successful operation)
     """
-    request = RetrieveLocalizedPolicyVersions.create(
+    if namespace is None:
+        namespace, error = get_services_namespace()
+        if error:
+            return None, error
+    request = RetrieveLocalizedPolicyVersions1.create(
         policy_version_id=policy_version_id,
+        namespace=namespace,
     )
     return run_request(request, additional_headers=x_additional_headers, **kwargs)
 
 
-@same_doc_as(RetrieveLocalizedPolicyVersions)
-async def retrieve_localized_policy_versions_async(
+@same_doc_as(RetrieveLocalizedPolicyVersions1)
+async def retrieve_localized_policy_versions_1_async(
     policy_version_id: str,
+    namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
-    """Retrieve Versions from Country-Specific Policy (retrieveLocalizedPolicyVersions)
+    """Retrieve Versions from Country-Specific Policy (retrieveLocalizedPolicyVersions_1)
 
     Retrieve versions of a particular country-specific policy.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:*:LEGAL", action=2 (READ)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:*:LEGAL [READ]
 
     Properties:
-        url: /agreement/admin/localized-policy-versions/versions/{policyVersionId}
+        url: /agreement/admin/namespaces/{namespace}/localized-policy-versions/versions/{policyVersionId}
 
         method: GET
 
-        tags: ["Localized Policy Versions"]
+        tags: ["Localized Policy Versions With Namespace"]
 
         consumes: []
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
+
+        namespace: (namespace) REQUIRED str in path
 
         policy_version_id: (policyVersionId) REQUIRED str in path
 
     Responses:
         200: OK - List[RetrieveLocalizedPolicyVersionResponse] (successful operation)
     """
-    request = RetrieveLocalizedPolicyVersions.create(
+    if namespace is None:
+        namespace, error = get_services_namespace()
+        if error:
+            return None, error
+    request = RetrieveLocalizedPolicyVersions1.create(
         policy_version_id=policy_version_id,
+        namespace=namespace,
     )
     return await run_request_async(
         request, additional_headers=x_additional_headers, **kwargs
     )
 
 
-@same_doc_as(RetrieveSingleLocalizedPolicyVersion)
-def retrieve_single_localized_policy_version(
+@same_doc_as(RetrieveSingleLocalizedPolicyVersion1)
+def retrieve_single_localized_policy_version_1(
     localized_policy_version_id: str,
+    namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
-    """Retrieve a Localized Version from Country-Specific Policy (retrieveSingleLocalizedPolicyVersion)
+    """Retrieve a Localized Version from Country-Specific Policy (retrieveSingleLocalizedPolicyVersion_1)
 
     Retrieve a version of a particular country-specific policy.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:*:LEGAL", action=2 (READ)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:*:LEGAL [READ]
 
     Properties:
-        url: /agreement/admin/localized-policy-versions/{localizedPolicyVersionId}
+        url: /agreement/admin/namespaces/{namespace}/localized-policy-versions/{localizedPolicyVersionId}
 
         method: GET
 
-        tags: ["Localized Policy Versions"]
+        tags: ["Localized Policy Versions With Namespace"]
 
         consumes: []
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         localized_policy_version_id: (localizedPolicyVersionId) REQUIRED str in path
 
+        namespace: (namespace) REQUIRED str in path
+
     Responses:
         200: OK - RetrieveLocalizedPolicyVersionResponse (successful operation)
 
         404: Not Found - ErrorEntity (2912: errors.net.accelbyte.platform.legal.policy_version_not_found)
     """
-    request = RetrieveSingleLocalizedPolicyVersion.create(
+    if namespace is None:
+        namespace, error = get_services_namespace()
+        if error:
+            return None, error
+    request = RetrieveSingleLocalizedPolicyVersion1.create(
         localized_policy_version_id=localized_policy_version_id,
+        namespace=namespace,
     )
     return run_request(request, additional_headers=x_additional_headers, **kwargs)
 
 
-@same_doc_as(RetrieveSingleLocalizedPolicyVersion)
-async def retrieve_single_localized_policy_version_async(
+@same_doc_as(RetrieveSingleLocalizedPolicyVersion1)
+async def retrieve_single_localized_policy_version_1_async(
     localized_policy_version_id: str,
+    namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
-    """Retrieve a Localized Version from Country-Specific Policy (retrieveSingleLocalizedPolicyVersion)
+    """Retrieve a Localized Version from Country-Specific Policy (retrieveSingleLocalizedPolicyVersion_1)
 
     Retrieve a version of a particular country-specific policy.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:*:LEGAL", action=2 (READ)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:*:LEGAL [READ]
 
     Properties:
-        url: /agreement/admin/localized-policy-versions/{localizedPolicyVersionId}
+        url: /agreement/admin/namespaces/{namespace}/localized-policy-versions/{localizedPolicyVersionId}
 
         method: GET
 
-        tags: ["Localized Policy Versions"]
+        tags: ["Localized Policy Versions With Namespace"]
 
         consumes: []
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         localized_policy_version_id: (localizedPolicyVersionId) REQUIRED str in path
 
+        namespace: (namespace) REQUIRED str in path
+
     Responses:
         200: OK - RetrieveLocalizedPolicyVersionResponse (successful operation)
 
         404: Not Found - ErrorEntity (2912: errors.net.accelbyte.platform.legal.policy_version_not_found)
     """
-    request = RetrieveSingleLocalizedPolicyVersion.create(
+    if namespace is None:
+        namespace, error = get_services_namespace()
+        if error:
+            return None, error
+    request = RetrieveSingleLocalizedPolicyVersion1.create(
         localized_policy_version_id=localized_policy_version_id,
+        namespace=namespace,
     )
     return await run_request_async(
         request, additional_headers=x_additional_headers, **kwargs
     )
 
 
-@same_doc_as(RetrieveSingleLocalizedPolicyVersion2)
-def retrieve_single_localized_policy_version_2(
+@same_doc_as(RetrieveSingleLocalizedPolicyVersion3)
+def retrieve_single_localized_policy_version_3(
     localized_policy_version_id: str,
+    namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
-    """Retrieve a Localized Version (retrieveSingleLocalizedPolicyVersion_2)
+    """Retrieve a Localized Version (retrieveSingleLocalizedPolicyVersion_3)
 
     Retrieve specific localized policy version including the policy version and base policy version where the localized policy version located.
     Other detail info:
 
     Properties:
-        url: /agreement/public/localized-policy-versions/{localizedPolicyVersionId}
+        url: /agreement/public/namespaces/{namespace}/localized-policy-versions/{localizedPolicyVersionId}
 
         method: GET
 
-        tags: ["Localized Policy Versions"]
+        tags: ["Localized Policy Versions With Namespace"]
 
         consumes: []
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
 
         localized_policy_version_id: (localizedPolicyVersionId) REQUIRED str in path
 
+        namespace: (namespace) REQUIRED str in path
+
     Responses:
         200: OK - RetrieveLocalizedPolicyVersionPublicResponse (successful operation)
 
         404: Not Found - ErrorEntity (40038: errors.net.accelbyte.platform.legal.localized_policy_version_not_found)
     """
-    request = RetrieveSingleLocalizedPolicyVersion2.create(
+    if namespace is None:
+        namespace, error = get_services_namespace()
+        if error:
+            return None, error
+    request = RetrieveSingleLocalizedPolicyVersion3.create(
         localized_policy_version_id=localized_policy_version_id,
+        namespace=namespace,
     )
     return run_request(request, additional_headers=x_additional_headers, **kwargs)
 
 
-@same_doc_as(RetrieveSingleLocalizedPolicyVersion2)
-async def retrieve_single_localized_policy_version_2_async(
+@same_doc_as(RetrieveSingleLocalizedPolicyVersion3)
+async def retrieve_single_localized_policy_version_3_async(
     localized_policy_version_id: str,
+    namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
-    """Retrieve a Localized Version (retrieveSingleLocalizedPolicyVersion_2)
+    """Retrieve a Localized Version (retrieveSingleLocalizedPolicyVersion_3)
 
     Retrieve specific localized policy version including the policy version and base policy version where the localized policy version located.
     Other detail info:
 
     Properties:
-        url: /agreement/public/localized-policy-versions/{localizedPolicyVersionId}
+        url: /agreement/public/namespaces/{namespace}/localized-policy-versions/{localizedPolicyVersionId}
 
         method: GET
 
-        tags: ["Localized Policy Versions"]
+        tags: ["Localized Policy Versions With Namespace"]
 
         consumes: []
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
 
         localized_policy_version_id: (localizedPolicyVersionId) REQUIRED str in path
 
+        namespace: (namespace) REQUIRED str in path
+
     Responses:
         200: OK - RetrieveLocalizedPolicyVersionPublicResponse (successful operation)
 
         404: Not Found - ErrorEntity (40038: errors.net.accelbyte.platform.legal.localized_policy_version_not_found)
     """
-    request = RetrieveSingleLocalizedPolicyVersion2.create(
+    if namespace is None:
+        namespace, error = get_services_namespace()
+        if error:
+            return None, error
+    request = RetrieveSingleLocalizedPolicyVersion3.create(
         localized_policy_version_id=localized_policy_version_id,
+        namespace=namespace,
     )
     return await run_request_async(
         request, additional_headers=x_additional_headers, **kwargs
     )
 
 
-@same_doc_as(SetDefaultPolicy)
-def set_default_policy(
+@same_doc_as(SetDefaultPolicy1)
+def set_default_policy_1(
     localized_policy_version_id: str,
+    namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
-    """Set Default Localized Policy (setDefaultPolicy)
+    """Set Default Localized Policy (setDefaultPolicy_1)
 
     Update a localized version policy to be the default.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:*:LEGAL", action=4 (UPDATE)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:*:LEGAL [UPDATE]
 
     Properties:
-        url: /agreement/admin/localized-policy-versions/{localizedPolicyVersionId}/default
+        url: /agreement/admin/namespaces/{namespace}/localized-policy-versions/{localizedPolicyVersionId}/default
 
         method: PATCH
 
-        tags: ["Localized Policy Versions"]
+        tags: ["Localized Policy Versions With Namespace"]
 
         consumes: []
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         localized_policy_version_id: (localizedPolicyVersionId) REQUIRED str in path
 
-    Responses:
-        200: OK - (Successful operation)
+        namespace: (namespace) REQUIRED str in path
 
-        400: Bad Request - ErrorEntity (40035: errors.net.accelbyte.platform.legal.invalid_localize_policy_version)
+    Responses:
+        200: OK - (successful operation)
     """
-    request = SetDefaultPolicy.create(
+    if namespace is None:
+        namespace, error = get_services_namespace()
+        if error:
+            return None, error
+    request = SetDefaultPolicy1.create(
         localized_policy_version_id=localized_policy_version_id,
+        namespace=namespace,
     )
     return run_request(request, additional_headers=x_additional_headers, **kwargs)
 
 
-@same_doc_as(SetDefaultPolicy)
-async def set_default_policy_async(
+@same_doc_as(SetDefaultPolicy1)
+async def set_default_policy_1_async(
     localized_policy_version_id: str,
+    namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
-    """Set Default Localized Policy (setDefaultPolicy)
+    """Set Default Localized Policy (setDefaultPolicy_1)
 
     Update a localized version policy to be the default.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:*:LEGAL", action=4 (UPDATE)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:*:LEGAL [UPDATE]
 
     Properties:
-        url: /agreement/admin/localized-policy-versions/{localizedPolicyVersionId}/default
+        url: /agreement/admin/namespaces/{namespace}/localized-policy-versions/{localizedPolicyVersionId}/default
 
         method: PATCH
 
-        tags: ["Localized Policy Versions"]
+        tags: ["Localized Policy Versions With Namespace"]
 
         consumes: []
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         localized_policy_version_id: (localizedPolicyVersionId) REQUIRED str in path
 
-    Responses:
-        200: OK - (Successful operation)
+        namespace: (namespace) REQUIRED str in path
 
-        400: Bad Request - ErrorEntity (40035: errors.net.accelbyte.platform.legal.invalid_localize_policy_version)
+    Responses:
+        200: OK - (successful operation)
     """
-    request = SetDefaultPolicy.create(
+    if namespace is None:
+        namespace, error = get_services_namespace()
+        if error:
+            return None, error
+    request = SetDefaultPolicy1.create(
         localized_policy_version_id=localized_policy_version_id,
+        namespace=namespace,
     )
     return await run_request_async(
         request, additional_headers=x_additional_headers, **kwargs
     )
 
 
-@same_doc_as(UpdateLocalizedPolicyVersion)
-def update_localized_policy_version(
+@same_doc_as(UpdateLocalizedPolicyVersion1)
+def update_localized_policy_version_1(
     localized_policy_version_id: str,
     body: Optional[UpdateLocalizedPolicyVersionRequest] = None,
+    namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
-    """Update a Localized Version from Country-Specific Policy (updateLocalizedPolicyVersion)
+    """Update a Localized Version from Country-Specific Policy (updateLocalizedPolicyVersion_1)
 
     Update a version of a particular country-specific policy.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:*:LEGAL", action=4 (UPDATE)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:*:LEGAL [UPDATE]
 
     Properties:
-        url: /agreement/admin/localized-policy-versions/{localizedPolicyVersionId}
+        url: /agreement/admin/namespaces/{namespace}/localized-policy-versions/{localizedPolicyVersionId}
 
         method: PUT
 
-        tags: ["Localized Policy Versions"]
+        tags: ["Localized Policy Versions With Namespace"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         body: (body) OPTIONAL UpdateLocalizedPolicyVersionRequest in body
 
         localized_policy_version_id: (localizedPolicyVersionId) REQUIRED str in path
 
+        namespace: (namespace) REQUIRED str in path
+
     Responses:
         200: OK - UpdateLocalizedPolicyVersionResponse (successful operation)
 
         400: Bad Request - ErrorEntity (40035: errors.net.accelbyte.platform.legal.invalid_policy_version)
     """
-    request = UpdateLocalizedPolicyVersion.create(
+    if namespace is None:
+        namespace, error = get_services_namespace()
+        if error:
+            return None, error
+    request = UpdateLocalizedPolicyVersion1.create(
         localized_policy_version_id=localized_policy_version_id,
         body=body,
+        namespace=namespace,
     )
     return run_request(request, additional_headers=x_additional_headers, **kwargs)
 
 
-@same_doc_as(UpdateLocalizedPolicyVersion)
-async def update_localized_policy_version_async(
+@same_doc_as(UpdateLocalizedPolicyVersion1)
+async def update_localized_policy_version_1_async(
     localized_policy_version_id: str,
     body: Optional[UpdateLocalizedPolicyVersionRequest] = None,
+    namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
-    """Update a Localized Version from Country-Specific Policy (updateLocalizedPolicyVersion)
+    """Update a Localized Version from Country-Specific Policy (updateLocalizedPolicyVersion_1)
 
     Update a version of a particular country-specific policy.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:*:LEGAL", action=4 (UPDATE)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:*:LEGAL [UPDATE]
 
     Properties:
-        url: /agreement/admin/localized-policy-versions/{localizedPolicyVersionId}
+        url: /agreement/admin/namespaces/{namespace}/localized-policy-versions/{localizedPolicyVersionId}
 
         method: PUT
 
-        tags: ["Localized Policy Versions"]
+        tags: ["Localized Policy Versions With Namespace"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         body: (body) OPTIONAL UpdateLocalizedPolicyVersionRequest in body
 
         localized_policy_version_id: (localizedPolicyVersionId) REQUIRED str in path
 
+        namespace: (namespace) REQUIRED str in path
+
     Responses:
         200: OK - UpdateLocalizedPolicyVersionResponse (successful operation)
 
         400: Bad Request - ErrorEntity (40035: errors.net.accelbyte.platform.legal.invalid_policy_version)
     """
-    request = UpdateLocalizedPolicyVersion.create(
+    if namespace is None:
+        namespace, error = get_services_namespace()
+        if error:
+            return None, error
+    request = UpdateLocalizedPolicyVersion1.create(
         localized_policy_version_id=localized_policy_version_id,
         body=body,
+        namespace=namespace,
     )
     return await run_request_async(
         request, additional_headers=x_additional_headers, **kwargs
     )
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/wrappers/_policies.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/wrappers/_policies.py`

 * *Files 4% similar despite different names*

```diff
@@ -388,15 +388,14 @@
         *  Fill the alwaysIncludeDefault with true if you want to be responded with always include default policy. If there are duplicate policies (default policies and country specific policies with same base policy) it'll include policy with same country code, for example:
           * Document 1 (default): Region US (default), UA
           * Document 2 (default): Region US (default)
           * Document 3 (default): Region US (default)
           * User: Region UA
           * Query: alwaysIncludeDefault: true
           * Response: Document 1 (UA), Document 2 (US), Document 3 (US)
-        *  Required permission: login user
 
     Properties:
         url: /agreement/public/policies/namespaces/{namespace}
 
         method: GET
 
         tags: ["Policies"]
@@ -458,15 +457,14 @@
         *  Fill the alwaysIncludeDefault with true if you want to be responded with always include default policy. If there are duplicate policies (default policies and country specific policies with same base policy) it'll include policy with same country code, for example:
           * Document 1 (default): Region US (default), UA
           * Document 2 (default): Region US (default)
           * Document 3 (default): Region US (default)
           * User: Region UA
           * Query: alwaysIncludeDefault: true
           * Response: Document 1 (UA), Document 2 (US), Document 3 (US)
-        *  Required permission: login user
 
     Properties:
         url: /agreement/public/policies/namespaces/{namespace}
 
         method: GET
 
         tags: ["Policies"]
@@ -511,32 +509,27 @@
 @same_doc_as(RetrievePolicies)
 def retrieve_policies(
     country_code: str, x_additional_headers: Optional[Dict[str, str]] = None, **kwargs
 ):
     """Retrieve Policies by Country (retrievePolicies)
 
     Retrieve all active policies based on a country.
-    Other detail info:
-        * Required permission : resource="ADMIN:NAMESPACE:*:LEGAL", action=2 (READ)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:*:LEGAL [READ]
 
     Properties:
         url: /agreement/admin/policies/countries/{countryCode}
 
         method: GET
 
         tags: ["Policies"]
 
         consumes: []
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         country_code: (countryCode) REQUIRED str in path
 
     Responses:
         200: OK - List[RetrievePolicyResponse] (successful operation)
     """
     request = RetrievePolicies.create(
@@ -548,32 +541,27 @@
 @same_doc_as(RetrievePolicies)
 async def retrieve_policies_async(
     country_code: str, x_additional_headers: Optional[Dict[str, str]] = None, **kwargs
 ):
     """Retrieve Policies by Country (retrievePolicies)
 
     Retrieve all active policies based on a country.
-    Other detail info:
-        * Required permission : resource="ADMIN:NAMESPACE:*:LEGAL", action=2 (READ)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:*:LEGAL [READ]
 
     Properties:
         url: /agreement/admin/policies/countries/{countryCode}
 
         method: GET
 
         tags: ["Policies"]
 
         consumes: []
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         country_code: (countryCode) REQUIRED str in path
 
     Responses:
         200: OK - List[RetrievePolicyResponse] (successful operation)
     """
     request = RetrievePolicies.create(
@@ -587,32 +575,27 @@
 @same_doc_as(SetDefaultPolicy2)
 def set_default_policy_2(
     policy_id: str, x_additional_headers: Optional[Dict[str, str]] = None, **kwargs
 ):
     """Set Default Policy (setDefaultPolicy_2)
 
     Update a policy to be the default.
-    Other detail info:
-        * Required permission : resource="ADMIN:NAMESPACE:*:LEGAL", action=4 (UPDATE)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:*:LEGAL [UPDATE]
 
     Properties:
         url: /agreement/admin/policies/{policyId}/default
 
         method: PATCH
 
         tags: ["Policies"]
 
         consumes: []
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         policy_id: (policyId) REQUIRED str in path
 
     Responses:
         200: OK - (operation successful)
 
         400: Bad Request - ErrorEntity (40033: errors.net.accelbyte.platform.legal.invalid_policy_id)
@@ -626,32 +609,27 @@
 @same_doc_as(SetDefaultPolicy2)
 async def set_default_policy_2_async(
     policy_id: str, x_additional_headers: Optional[Dict[str, str]] = None, **kwargs
 ):
     """Set Default Policy (setDefaultPolicy_2)
 
     Update a policy to be the default.
-    Other detail info:
-        * Required permission : resource="ADMIN:NAMESPACE:*:LEGAL", action=4 (UPDATE)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:*:LEGAL [UPDATE]
 
     Properties:
         url: /agreement/admin/policies/{policyId}/default
 
         method: PATCH
 
         tags: ["Policies"]
 
         consumes: []
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         policy_id: (policyId) REQUIRED str in path
 
     Responses:
         200: OK - (operation successful)
 
         400: Bad Request - ErrorEntity (40033: errors.net.accelbyte.platform.legal.invalid_policy_id)
@@ -670,32 +648,27 @@
     body: Optional[UpdatePolicyRequest] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Update Country-Specific Policy (updatePolicy)
 
     Update country-specific policy.
-    Other detail info:
-        * Required permission : resource="ADMIN:NAMESPACE:*:LEGAL", action=4 (UPDATE)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:*:LEGAL [UPDATE]
 
     Properties:
         url: /agreement/admin/policies/{policyId}
 
         method: PATCH
 
         tags: ["Policies"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         body: (body) OPTIONAL UpdatePolicyRequest in body
 
         policy_id: (policyId) REQUIRED str in path
 
     Responses:
         200: OK - (operation successful)
@@ -715,32 +688,27 @@
     body: Optional[UpdatePolicyRequest] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Update Country-Specific Policy (updatePolicy)
 
     Update country-specific policy.
-    Other detail info:
-        * Required permission : resource="ADMIN:NAMESPACE:*:LEGAL", action=4 (UPDATE)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:*:LEGAL [UPDATE]
 
     Properties:
         url: /agreement/admin/policies/{policyId}
 
         method: PATCH
 
         tags: ["Policies"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         body: (body) OPTIONAL UpdatePolicyRequest in body
 
         policy_id: (policyId) REQUIRED str in path
 
     Responses:
         200: OK - (operation successful)
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/wrappers/_policies_with_namespace.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/wrappers/_policies_with_namespace.py`

 * *Files 18% similar despite different names*

```diff
@@ -42,33 +42,27 @@
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Set Default Policy (setDefaultPolicy_3)
 
     Update a policy to be the default.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:{namespace}:LEGAL", action=4 (UPDATE)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:LEGAL [UPDATE]
 
     Properties:
         url: /agreement/admin/namespaces/{namespace}/policies/{policyId}/default
 
         method: PATCH
 
         tags: ["Policies With Namespace"]
 
         consumes: []
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         namespace: (namespace) REQUIRED str in path
 
         policy_id: (policyId) REQUIRED str in path
 
     Responses:
         200: OK - (operation successful)
@@ -92,33 +86,27 @@
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Set Default Policy (setDefaultPolicy_3)
 
     Update a policy to be the default.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:{namespace}:LEGAL", action=4 (UPDATE)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:LEGAL [UPDATE]
 
     Properties:
         url: /agreement/admin/namespaces/{namespace}/policies/{policyId}/default
 
         method: PATCH
 
         tags: ["Policies With Namespace"]
 
         consumes: []
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         namespace: (namespace) REQUIRED str in path
 
         policy_id: (policyId) REQUIRED str in path
 
     Responses:
         200: OK - (operation successful)
@@ -145,33 +133,27 @@
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Update Country-Specific Policy (updatePolicy_1)
 
     Update country-specific policy.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:{namespace}:LEGAL", action=4 (UPDATE)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:LEGAL [UPDATE]
 
     Properties:
         url: /agreement/admin/namespaces/{namespace}/policies/{policyId}
 
         method: PATCH
 
         tags: ["Policies With Namespace"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         body: (body) OPTIONAL UpdatePolicyRequest in body
 
         namespace: (namespace) REQUIRED str in path
 
         policy_id: (policyId) REQUIRED str in path
 
@@ -199,33 +181,27 @@
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Update Country-Specific Policy (updatePolicy_1)
 
     Update country-specific policy.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:{namespace}:LEGAL", action=4 (UPDATE)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:LEGAL [UPDATE]
 
     Properties:
         url: /agreement/admin/namespaces/{namespace}/policies/{policyId}
 
         method: PATCH
 
         tags: ["Policies With Namespace"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         body: (body) OPTIONAL UpdatePolicyRequest in body
 
         namespace: (namespace) REQUIRED str in path
 
         policy_id: (policyId) REQUIRED str in path
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/wrappers/_policy_versions.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/wrappers/_policy_versions.py`

 * *Files 11% similar despite different names*

```diff
@@ -48,32 +48,27 @@
     body: Optional[CreatePolicyVersionRequest] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Create a Version from Country-Specific Policy (createPolicyVersion)
 
     Create a version of a particular country-specific policy.
-    Other detail info:
-        * Required permission : resource="ADMIN:NAMESPACE:*:LEGAL", action=1 (CREATE)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:*:LEGAL [CREATE]
 
     Properties:
         url: /agreement/admin/policies/{policyId}/versions
 
         method: POST
 
         tags: ["Policy Versions"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         body: (body) OPTIONAL CreatePolicyVersionRequest in body
 
         policy_id: (policyId) REQUIRED str in path
 
     Responses:
         201: Created - CreatePolicyVersionResponse (successful operation)
@@ -93,32 +88,27 @@
     body: Optional[CreatePolicyVersionRequest] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Create a Version from Country-Specific Policy (createPolicyVersion)
 
     Create a version of a particular country-specific policy.
-    Other detail info:
-        * Required permission : resource="ADMIN:NAMESPACE:*:LEGAL", action=1 (CREATE)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:*:LEGAL [CREATE]
 
     Properties:
         url: /agreement/admin/policies/{policyId}/versions
 
         method: POST
 
         tags: ["Policy Versions"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         body: (body) OPTIONAL CreatePolicyVersionRequest in body
 
         policy_id: (policyId) REQUIRED str in path
 
     Responses:
         201: Created - CreatePolicyVersionResponse (successful operation)
@@ -140,32 +130,27 @@
     should_notify: Optional[bool] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Manually Publish a Version from Country-Specific Policy (publishPolicyVersion)
 
     Manually publish a version of a particular country-specific policy.
-    Other detail info:
-        * Required permission : resource="ADMIN:NAMESPACE:*:LEGAL", action=4 (UPDATE)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:*:LEGAL [UPDATE]
 
     Properties:
         url: /agreement/admin/policies/versions/{policyVersionId}/latest
 
         method: PATCH
 
         tags: ["Policy Versions"]
 
         consumes: []
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         policy_version_id: (policyVersionId) REQUIRED str in path
 
         should_notify: (shouldNotify) OPTIONAL bool in query
 
     Responses:
         200: OK - (operation successful)
@@ -187,32 +172,27 @@
     should_notify: Optional[bool] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Manually Publish a Version from Country-Specific Policy (publishPolicyVersion)
 
     Manually publish a version of a particular country-specific policy.
-    Other detail info:
-        * Required permission : resource="ADMIN:NAMESPACE:*:LEGAL", action=4 (UPDATE)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:*:LEGAL [UPDATE]
 
     Properties:
         url: /agreement/admin/policies/versions/{policyVersionId}/latest
 
         method: PATCH
 
         tags: ["Policy Versions"]
 
         consumes: []
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         policy_version_id: (policyVersionId) REQUIRED str in path
 
         should_notify: (shouldNotify) OPTIONAL bool in query
 
     Responses:
         200: OK - (operation successful)
@@ -236,32 +216,27 @@
     version_id: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Retrieve a Version from Country-Specific Policy (retrieveSinglePolicyVersion)
 
     Retrieve a version of a particular country specific policy. If version is not provided, the Legal Service will assume caller requesting all versions from country-specific policy.
-    Other detail info:
-        * Required permission : resource="ADMIN:NAMESPACE:*:LEGAL", action=2 (READ)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:*:LEGAL [READ]
 
     Properties:
         url: /agreement/admin/policies/{policyId}/versions
 
         method: GET
 
         tags: ["Policy Versions"]
 
         consumes: []
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         policy_id: (policyId) REQUIRED str in path
 
         version_id: (versionId) OPTIONAL str in query
 
     Responses:
         200: OK - List[RetrievePolicyVersionResponse] (successful operation)
@@ -281,32 +256,27 @@
     version_id: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Retrieve a Version from Country-Specific Policy (retrieveSinglePolicyVersion)
 
     Retrieve a version of a particular country specific policy. If version is not provided, the Legal Service will assume caller requesting all versions from country-specific policy.
-    Other detail info:
-        * Required permission : resource="ADMIN:NAMESPACE:*:LEGAL", action=2 (READ)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:*:LEGAL [READ]
 
     Properties:
         url: /agreement/admin/policies/{policyId}/versions
 
         method: GET
 
         tags: ["Policy Versions"]
 
         consumes: []
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         policy_id: (policyId) REQUIRED str in path
 
         version_id: (versionId) OPTIONAL str in query
 
     Responses:
         200: OK - List[RetrievePolicyVersionResponse] (successful operation)
@@ -328,32 +298,27 @@
     body: Optional[UpdatePolicyVersionRequest] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Update a Version of Policy (updatePolicyVersion)
 
     Update a particular policy version.
-    Other detail info:
-        * Required permission : resource="ADMIN:NAMESPACE:*:LEGAL", action=4 (UPDATE)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:*:LEGAL [UPDATE]
 
     Properties:
         url: /agreement/admin/policies/versions/{policyVersionId}
 
         method: PATCH
 
         tags: ["Policy Versions"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         body: (body) OPTIONAL UpdatePolicyVersionRequest in body
 
         policy_version_id: (policyVersionId) REQUIRED str in path
 
     Responses:
         200: OK - UpdatePolicyVersionResponse (successful operation)
@@ -375,32 +340,27 @@
     body: Optional[UpdatePolicyVersionRequest] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Update a Version of Policy (updatePolicyVersion)
 
     Update a particular policy version.
-    Other detail info:
-        * Required permission : resource="ADMIN:NAMESPACE:*:LEGAL", action=4 (UPDATE)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:*:LEGAL [UPDATE]
 
     Properties:
         url: /agreement/admin/policies/versions/{policyVersionId}
 
         method: PATCH
 
         tags: ["Policy Versions"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         body: (body) OPTIONAL UpdatePolicyVersionRequest in body
 
         policy_version_id: (policyVersionId) REQUIRED str in path
 
     Responses:
         200: OK - UpdatePolicyVersionResponse (successful operation)
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/wrappers/_policy_versions_with_namespace.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/wrappers/_policy_versions_with_namespace.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,33 +49,27 @@
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Create a Version from Country-Specific Policy (createPolicyVersion_1)
 
     Create a version of a particular country-specific policy.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:*:LEGAL", action=1 (CREATE)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:*:LEGAL [CREATE]
 
     Properties:
         url: /agreement/admin/namespaces/{namespace}/policies/{policyId}/versions
 
         method: POST
 
         tags: ["Policy Versions With Namespace"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         body: (body) OPTIONAL CreatePolicyVersionRequest in body
 
         namespace: (namespace) REQUIRED str in path
 
         policy_id: (policyId) REQUIRED str in path
 
@@ -103,33 +97,27 @@
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Create a Version from Country-Specific Policy (createPolicyVersion_1)
 
     Create a version of a particular country-specific policy.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:*:LEGAL", action=1 (CREATE)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:*:LEGAL [CREATE]
 
     Properties:
         url: /agreement/admin/namespaces/{namespace}/policies/{policyId}/versions
 
         method: POST
 
         tags: ["Policy Versions With Namespace"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         body: (body) OPTIONAL CreatePolicyVersionRequest in body
 
         namespace: (namespace) REQUIRED str in path
 
         policy_id: (policyId) REQUIRED str in path
 
@@ -159,33 +147,27 @@
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Manually Publish a Version from Country-Specific Policy (publishPolicyVersion_1)
 
     Manually publish a version of a particular country-specific policy.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:*:LEGAL", action=4 (UPDATE)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:*:LEGAL [UPDATE]
 
     Properties:
         url: /agreement/admin/namespaces/{namespace}/policies/versions/{policyVersionId}/latest
 
         method: PATCH
 
         tags: ["Policy Versions With Namespace"]
 
         consumes: []
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         namespace: (namespace) REQUIRED str in path
 
         policy_version_id: (policyVersionId) REQUIRED str in path
 
         should_notify: (shouldNotify) OPTIONAL bool in query
 
@@ -215,33 +197,27 @@
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Manually Publish a Version from Country-Specific Policy (publishPolicyVersion_1)
 
     Manually publish a version of a particular country-specific policy.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:*:LEGAL", action=4 (UPDATE)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:*:LEGAL [UPDATE]
 
     Properties:
         url: /agreement/admin/namespaces/{namespace}/policies/versions/{policyVersionId}/latest
 
         method: PATCH
 
         tags: ["Policy Versions With Namespace"]
 
         consumes: []
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         namespace: (namespace) REQUIRED str in path
 
         policy_version_id: (policyVersionId) REQUIRED str in path
 
         should_notify: (shouldNotify) OPTIONAL bool in query
 
@@ -273,33 +249,27 @@
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Retrieve a Version from Country-Specific Policy (retrieveSinglePolicyVersion_1)
 
     Retrieve a version of a particular country specific policy. If version is not provided, the Legal Service will assume caller requesting all versions from country-specific policy.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:*:LEGAL", action=2 (READ)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:*:LEGAL [READ]
 
     Properties:
         url: /agreement/admin/namespaces/{namespace}/policies/{policyId}/versions
 
         method: GET
 
         tags: ["Policy Versions With Namespace"]
 
         consumes: []
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         namespace: (namespace) REQUIRED str in path
 
         policy_id: (policyId) REQUIRED str in path
 
         version_id: (versionId) OPTIONAL str in query
 
@@ -327,33 +297,27 @@
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Retrieve a Version from Country-Specific Policy (retrieveSinglePolicyVersion_1)
 
     Retrieve a version of a particular country specific policy. If version is not provided, the Legal Service will assume caller requesting all versions from country-specific policy.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:*:LEGAL", action=2 (READ)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:*:LEGAL [READ]
 
     Properties:
         url: /agreement/admin/namespaces/{namespace}/policies/{policyId}/versions
 
         method: GET
 
         tags: ["Policy Versions With Namespace"]
 
         consumes: []
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         namespace: (namespace) REQUIRED str in path
 
         policy_id: (policyId) REQUIRED str in path
 
         version_id: (versionId) OPTIONAL str in query
 
@@ -383,33 +347,27 @@
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Update a Version of Policy (updatePolicyVersion_1)
 
     Update a particular policy version.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:*:LEGAL", action=4 (UPDATE)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:*:LEGAL [UPDATE]
 
     Properties:
         url: /agreement/admin/namespaces/{namespace}/policies/versions/{policyVersionId}
 
         method: PATCH
 
         tags: ["Policy Versions With Namespace"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         body: (body) OPTIONAL UpdatePolicyVersionRequest in body
 
         namespace: (namespace) REQUIRED str in path
 
         policy_version_id: (policyVersionId) REQUIRED str in path
 
@@ -439,33 +397,27 @@
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Update a Version of Policy (updatePolicyVersion_1)
 
     Update a particular policy version.
-    Other detail info:
-
-      * Required permission : resource="ADMIN:NAMESPACE:*:LEGAL", action=4 (UPDATE)
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:*:LEGAL [UPDATE]
 
     Properties:
         url: /agreement/admin/namespaces/{namespace}/policies/versions/{policyVersionId}
 
         method: PATCH
 
         tags: ["Policy Versions With Namespace"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
         body: (body) OPTIONAL UpdatePolicyVersionRequest in body
 
         namespace: (namespace) REQUIRED str in path
 
         policy_version_id: (policyVersionId) REQUIRED str in path
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk/api/legal/wrappers/_utility.py` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk/api/legal/wrappers/_utility.py`

 * *Files 16% similar despite different names*

```diff
@@ -35,32 +35,27 @@
 
 
 @same_doc_as(CheckReadiness)
 def check_readiness(x_additional_headers: Optional[Dict[str, str]] = None, **kwargs):
     """Check Legal Data Readiness (checkReadiness)
 
     Readiness status defined as at least one legal basePolicy is present and having active basePolicy.
-    Other detail info:
-        * Required permission : resource="NAMESPACE:{namespace}:LEGAL", action=2 (READ)
-
-    Required Permission(s):
-        - NAMESPACE:{namespace}:LEGAL [READ]
 
     Properties:
         url: /agreement/public/readiness
 
         method: GET
 
         tags: ["Utility"]
 
         consumes: []
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
     Responses:
         200: OK - LegalReadinessStatusResponse (successful operation)
     """
     request = CheckReadiness.create()
     return run_request(request, additional_headers=x_additional_headers, **kwargs)
 
@@ -68,32 +63,27 @@
 @same_doc_as(CheckReadiness)
 async def check_readiness_async(
     x_additional_headers: Optional[Dict[str, str]] = None, **kwargs
 ):
     """Check Legal Data Readiness (checkReadiness)
 
     Readiness status defined as at least one legal basePolicy is present and having active basePolicy.
-    Other detail info:
-        * Required permission : resource="NAMESPACE:{namespace}:LEGAL", action=2 (READ)
-
-    Required Permission(s):
-        - NAMESPACE:{namespace}:LEGAL [READ]
 
     Properties:
         url: /agreement/public/readiness
 
         method: GET
 
         tags: ["Utility"]
 
         consumes: []
 
         produces: ["application/json"]
 
-        securities: [BEARER_AUTH] or [BEARER_AUTH]
+        securities: [BEARER_AUTH]
 
     Responses:
         200: OK - LegalReadinessStatusResponse (successful operation)
     """
     request = CheckReadiness.create()
     return await run_request_async(
         request, additional_headers=x_additional_headers, **kwargs
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk_service_legal.egg-info/PKG-INFO` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk_service_legal.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: accelbyte-py-sdk-service-legal
-Version: 0.8.0
+Version: 0.9.0
 Summary: AccelByte Python SDK - AccelByte Gaming Services Legal Service
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: accelbyte-py-sdk-core
 
 [//]: # (Code generated. DO NOT EDIT!)
 
 # AccelByte Modular Python SDK - Service Module
 
 This is a service module for the [AccelByte Modular Python SDK](https://github.com/AccelByte/accelbyte-python-modular-sdk) package.
 
 ```text
 AccelByte Gaming Services Legal Service
-* Version: 1.39.0
+* Version: 1.41.0
 ```
 
 ## Setup
 
 This SDK requires Python 3.9 to be installed.
 
 ### Install with Pip
```

### Comparing `accelbyte-py-sdk-service-legal-0.8.0/accelbyte_py_sdk_service_legal.egg-info/SOURCES.txt` & `accelbyte_py_sdk_service_legal-0.9.0/accelbyte_py_sdk_service_legal.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,20 +7,23 @@
 accelbyte_py_sdk/api/legal/models/create_base_policy_request.py
 accelbyte_py_sdk/api/legal/models/create_base_policy_request_v2.py
 accelbyte_py_sdk/api/legal/models/create_base_policy_response.py
 accelbyte_py_sdk/api/legal/models/create_localized_policy_version_request.py
 accelbyte_py_sdk/api/legal/models/create_localized_policy_version_response.py
 accelbyte_py_sdk/api/legal/models/create_policy_version_request.py
 accelbyte_py_sdk/api/legal/models/create_policy_version_response.py
+accelbyte_py_sdk/api/legal/models/download_exported_agreements_in_csv_response.py
 accelbyte_py_sdk/api/legal/models/error_entity.py
 accelbyte_py_sdk/api/legal/models/field_validation_error.py
+accelbyte_py_sdk/api/legal/models/initiate_export_agreements_to_csv_response.py
 accelbyte_py_sdk/api/legal/models/legal_readiness_status_response.py
 accelbyte_py_sdk/api/legal/models/localized_policy_version_object.py
 accelbyte_py_sdk/api/legal/models/paged_retrieve_user_accepted_agreement_response.py
 accelbyte_py_sdk/api/legal/models/paging.py
+accelbyte_py_sdk/api/legal/models/permission.py
 accelbyte_py_sdk/api/legal/models/policy_object.py
 accelbyte_py_sdk/api/legal/models/policy_version_object.py
 accelbyte_py_sdk/api/legal/models/policy_version_with_localized_version_object.py
 accelbyte_py_sdk/api/legal/models/retrieve_accepted_agreement_response.py
 accelbyte_py_sdk/api/legal/models/retrieve_base_policy_response.py
 accelbyte_py_sdk/api/legal/models/retrieve_localized_policy_version_public_response.py
 accelbyte_py_sdk/api/legal/models/retrieve_localized_policy_version_response.py
@@ -57,14 +60,16 @@
 accelbyte_py_sdk/api/legal/operations/agreement/change_preference_consent_1.py
 accelbyte_py_sdk/api/legal/operations/agreement/indirect_bulk_accept_ve_34e753.py
 accelbyte_py_sdk/api/legal/operations/agreement/indirect_bulk_accept_ve_f4345a.py
 accelbyte_py_sdk/api/legal/operations/agreement/retrieve_accepted_agreements.py
 accelbyte_py_sdk/api/legal/operations/agreement/retrieve_agreements_public.py
 accelbyte_py_sdk/api/legal/operations/agreement/retrieve_all_users_by_p_90a012.py
 accelbyte_py_sdk/api/legal/operations/agreement_with_namespace/__init__.py
+accelbyte_py_sdk/api/legal/operations/agreement_with_namespace/download_exported_agree_a56e5b.py
+accelbyte_py_sdk/api/legal/operations/agreement_with_namespace/initiate_export_agreeme_d92c31.py
 accelbyte_py_sdk/api/legal/operations/agreement_with_namespace/retrieve_accepted_agree_8c230d.py
 accelbyte_py_sdk/api/legal/operations/agreement_with_namespace/retrieve_accepted_agreements_1.py
 accelbyte_py_sdk/api/legal/operations/agreement_with_namespace/retrieve_all_users_by_p_3f6faa.py
 accelbyte_py_sdk/api/legal/operations/anonymization/__init__.py
 accelbyte_py_sdk/api/legal/operations/anonymization/anonymize_user_agreement.py
 accelbyte_py_sdk/api/legal/operations/base_legal_policies/__init__.py
 accelbyte_py_sdk/api/legal/operations/base_legal_policies/create_policy.py
```

