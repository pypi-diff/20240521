# Comparing `tmp/accelbyte_py_sdk_service_gdpr-0.8.0.tar.gz` & `tmp/accelbyte_py_sdk_service_gdpr-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accelbyte_py_sdk_service_gdpr-0.8.0.tar", last modified: Tue May  7 06:27:42 2024, max compression
+gzip compressed data, was "accelbyte_py_sdk_service_gdpr-0.9.0.tar", last modified: Tue May 21 03:46:55 2024, max compression
```

## Comparing `accelbyte_py_sdk_service_gdpr-0.8.0.tar` & `accelbyte_py_sdk_service_gdpr-0.9.0.tar`

### file list

```diff
@@ -1,73 +1,90 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:27:42.310171 accelbyte_py_sdk_service_gdpr-0.8.0/
--rw-r--r--   0 root         (0) root         (0)     1112 2024-05-07 06:27:42.310171 accelbyte_py_sdk_service_gdpr-0.8.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      866 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:27:42.302171 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:27:42.302171 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:27:42.302171 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/
--rw-rw-r--   0 root         (0) root         (0)     3744 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:27:42.306171 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/models/
--rw-rw-r--   0 root         (0) root         (0)     1754 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/models/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4398 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/models/dto_extend_config_dto.py
--rw-rw-r--   0 root         (0) root         (0)     4663 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/models/dto_service_config_dto.py
--rw-rw-r--   0 root         (0) root         (0)     7023 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/models/dto_service_configuration_dto.py
--rw-rw-r--   0 root         (0) root         (0)     4427 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/models/dto_service_configuration_update_request.py
--rw-rw-r--   0 root         (0) root         (0)     4382 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/models/dto_services_configuration_response.py
--rw-rw-r--   0 root         (0) root         (0)     5241 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/models/models_data_retrieval_response.py
--rw-rw-r--   0 root         (0) root         (0)     6657 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/models/models_deletion_data.py
--rw-rw-r--   0 root         (0) root         (0)     7490 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/models/models_deletion_status.py
--rw-rw-r--   0 root         (0) root         (0)     5062 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/models/models_list_deletion_data_response.py
--rw-rw-r--   0 root         (0) root         (0)     5062 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/models/models_list_personal_data_response.py
--rw-rw-r--   0 root         (0) root         (0)     5433 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/models/models_pagination.py
--rw-rw-r--   0 root         (0) root         (0)     8595 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/models/models_personal_data.py
--rw-rw-r--   0 root         (0) root         (0)     4517 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/models/models_request_delete_response.py
--rw-rw-r--   0 root         (0) root         (0)     3632 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/models/models_user_data_url.py
--rw-rw-r--   0 root         (0) root         (0)     5368 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/models/models_user_personal_data.py
--rw-rw-r--   0 root         (0) root         (0)     5091 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/models/models_user_personal_data_response.py
--rw-rw-r--   0 root         (0) root         (0)     4432 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/models/response_error.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:27:42.306171 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/
--rw-rw-r--   0 root         (0) root         (0)      432 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:27:42.306171 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/configuration/
--rw-rw-r--   0 root         (0) root         (0)      982 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/configuration/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6653 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/configuration/admin_get_services_conf_be46ef.py
--rw-rw-r--   0 root         (0) root         (0)     6353 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/configuration/admin_reset_services_co_abf06c.py
--rw-rw-r--   0 root         (0) root         (0)     7885 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/configuration/admin_update_services_c_ea010e.py
--rw-rw-r--   0 root         (0) root         (0)     7972 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/configuration/delete_admin_email_conf_009cca.py
--rw-rw-r--   0 root         (0) root         (0)     6269 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/configuration/get_admin_email_configuration.py
--rw-rw-r--   0 root         (0) root         (0)     7338 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/configuration/save_admin_email_configuration.py
--rw-rw-r--   0 root         (0) root         (0)     7354 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/configuration/update_admin_email_conf_71e966.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:27:42.306171 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/
--rw-rw-r--   0 root         (0) root         (0)     1268 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7654 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/admin_cancel_user_accou_de1ba5.py
--rw-rw-r--   0 root         (0) root         (0)    11263 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/admin_get_list_deletion_227d7d.py
--rw-rw-r--   0 root         (0) root         (0)     7579 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/admin_get_user_account__84ef5a.py
--rw-rw-r--   0 root         (0) root         (0)     7816 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/admin_submit_user_accou_b7780f.py
--rw-rw-r--   0 root         (0) root         (0)     5608 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/public_cancel_my_accoun_107811.py
--rw-rw-r--   0 root         (0) root         (0)     7499 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/public_cancel_user_acco_16b962.py
--rw-rw-r--   0 root         (0) root         (0)     5554 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/public_get_my_account_d_8595d0.py
--rw-rw-r--   0 root         (0) root         (0)     7455 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/public_get_user_account_09e4f2.py
--rw-rw-r--   0 root         (0) root         (0)     8284 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/public_submit_my_accoun_f5ded3.py
--rw-rw-r--   0 root         (0) root         (0)     8882 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/public_submit_user_acco_a6db4f.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:27:42.306171 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_retrieval/
--rw-rw-r--   0 root         (0) root         (0)     1140 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_retrieval/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8366 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_retrieval/admin_cancel_user_perso_78952d.py
--rw-rw-r--   0 root         (0) root         (0)     9407 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_retrieval/admin_generate_personal_48c32b.py
--rw-rw-r--   0 root         (0) root         (0)     9638 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_retrieval/admin_get_list_personal_424fda.py
--rw-rw-r--   0 root         (0) root         (0)     9128 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_retrieval/admin_get_user_personal_a892c0.py
--rw-rw-r--   0 root         (0) root         (0)     8482 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_retrieval/admin_request_data_retrieval.py
--rw-rw-r--   0 root         (0) root         (0)     8413 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_retrieval/public_cancel_user_pers_19dafa.py
--rw-rw-r--   0 root         (0) root         (0)     9455 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_retrieval/public_generate_persona_6b68a4.py
--rw-rw-r--   0 root         (0) root         (0)     9176 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_retrieval/public_get_user_persona_7e40c3.py
--rw-rw-r--   0 root         (0) root         (0)     8359 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_retrieval/public_request_data_retrieval.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:27:42.310171 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/wrappers/
--rw-rw-r--   0 root         (0) root         (0)     4025 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/wrappers/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    20661 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/wrappers/_configuration.py
--rw-rw-r--   0 root         (0) root         (0)    31388 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/wrappers/_data_deletion.py
--rw-rw-r--   0 root         (0) root         (0)    30852 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/wrappers/_data_retrieval.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:27:42.310171 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk_service_gdpr.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1112 2024-05-07 06:27:42.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk_service_gdpr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4108 2024-05-07 06:27:42.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk_service_gdpr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-07 06:27:42.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk_service_gdpr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-07 06:27:42.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk_service_gdpr.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-05-07 06:27:42.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk_service_gdpr.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)      353 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-07 06:27:42.310171 accelbyte_py_sdk_service_gdpr-0.8.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:46:55.818662 accelbyte_py_sdk_service_gdpr-0.9.0/
+-rw-r--r--   0 root         (0) root         (0)     1113 2024-05-21 03:46:55.818662 accelbyte_py_sdk_service_gdpr-0.9.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      867 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gdpr-0.9.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:46:55.810662 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:46:55.810662 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:46:55.810662 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/
+-rw-rw-r--   0 root         (0) root         (0)     4888 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:46:55.814662 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/models/
+-rw-rw-r--   0 root         (0) root         (0)     2190 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/models/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4398 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/models/dto_extend_config_dto.py
+-rw-rw-r--   0 root         (0) root         (0)     4631 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/models/dto_platform_account_closure_client_request.py
+-rw-rw-r--   0 root         (0) root         (0)     6734 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/models/dto_platform_account_closure_client_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5399 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/models/dto_service_config_dto.py
+-rw-rw-r--   0 root         (0) root         (0)     7023 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/models/dto_service_configuration_dto.py
+-rw-rw-r--   0 root         (0) root         (0)     4427 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/models/dto_service_configuration_update_request.py
+-rw-rw-r--   0 root         (0) root         (0)     4382 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/models/dto_services_configuration_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5551 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/models/dto_user_platform_account_closure_histories_response.py
+-rw-rw-r--   0 root         (0) root         (0)     7582 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/models/dto_user_platform_account_closure_history.py
+-rw-rw-r--   0 root         (0) root         (0)     5241 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/models/models_data_retrieval_response.py
+-rw-rw-r--   0 root         (0) root         (0)     6657 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/models/models_deletion_data.py
+-rw-rw-r--   0 root         (0) root         (0)     7490 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/models/models_deletion_status.py
+-rw-rw-r--   0 root         (0) root         (0)     5062 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/models/models_list_deletion_data_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5062 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/models/models_list_personal_data_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5433 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/models/models_pagination.py
+-rw-rw-r--   0 root         (0) root         (0)     8595 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/models/models_personal_data.py
+-rw-rw-r--   0 root         (0) root         (0)     4517 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/models/models_request_delete_response.py
+-rw-rw-r--   0 root         (0) root         (0)     3632 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/models/models_user_data_url.py
+-rw-rw-r--   0 root         (0) root         (0)     5368 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/models/models_user_personal_data.py
+-rw-rw-r--   0 root         (0) root         (0)     5091 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/models/models_user_personal_data_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4432 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/models/response_error.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:46:55.814662 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/operations/
+-rw-rw-r--   0 root         (0) root         (0)      433 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/operations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:46:55.814662 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/operations/configuration/
+-rw-rw-r--   0 root         (0) root         (0)     1303 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/operations/configuration/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     6871 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/operations/configuration/admin_get_platform_acco_c23147.py
+-rw-rw-r--   0 root         (0) root         (0)     6653 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/operations/configuration/admin_get_services_conf_be46ef.py
+-rw-rw-r--   0 root         (0) root         (0)     6553 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/operations/configuration/admin_reset_platform_ac_c4b31b.py
+-rw-rw-r--   0 root         (0) root         (0)     6353 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/operations/configuration/admin_reset_services_co_abf06c.py
+-rw-rw-r--   0 root         (0) root         (0)     8111 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/operations/configuration/admin_update_platform_a_1f24aa.py
+-rw-rw-r--   0 root         (0) root         (0)     7885 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/operations/configuration/admin_update_services_c_ea010e.py
+-rw-rw-r--   0 root         (0) root         (0)     7972 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/operations/configuration/delete_admin_email_conf_009cca.py
+-rw-rw-r--   0 root         (0) root         (0)     6269 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/operations/configuration/get_admin_email_configuration.py
+-rw-rw-r--   0 root         (0) root         (0)     7338 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/operations/configuration/save_admin_email_configuration.py
+-rw-rw-r--   0 root         (0) root         (0)     7354 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/operations/configuration/update_admin_email_conf_71e966.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:46:55.814662 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/
+-rw-rw-r--   0 root         (0) root         (0)     1269 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7654 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/admin_cancel_user_accou_de1ba5.py
+-rw-rw-r--   0 root         (0) root         (0)    11263 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/admin_get_list_deletion_227d7d.py
+-rw-rw-r--   0 root         (0) root         (0)     7579 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/admin_get_user_account__84ef5a.py
+-rw-rw-r--   0 root         (0) root         (0)     7816 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/admin_submit_user_accou_b7780f.py
+-rw-rw-r--   0 root         (0) root         (0)     5608 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/public_cancel_my_accoun_107811.py
+-rw-rw-r--   0 root         (0) root         (0)     7499 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/public_cancel_user_acco_16b962.py
+-rw-rw-r--   0 root         (0) root         (0)     5554 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/public_get_my_account_d_8595d0.py
+-rw-rw-r--   0 root         (0) root         (0)     7455 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/public_get_user_account_09e4f2.py
+-rw-rw-r--   0 root         (0) root         (0)     8284 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/public_submit_my_accoun_f5ded3.py
+-rw-rw-r--   0 root         (0) root         (0)     8882 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/public_submit_user_acco_a6db4f.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:46:55.814662 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/operations/data_retrieval/
+-rw-rw-r--   0 root         (0) root         (0)     1141 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/operations/data_retrieval/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8366 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/operations/data_retrieval/admin_cancel_user_perso_78952d.py
+-rw-rw-r--   0 root         (0) root         (0)     9407 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/operations/data_retrieval/admin_generate_personal_48c32b.py
+-rw-rw-r--   0 root         (0) root         (0)     9638 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/operations/data_retrieval/admin_get_list_personal_424fda.py
+-rw-rw-r--   0 root         (0) root         (0)     9128 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/operations/data_retrieval/admin_get_user_personal_a892c0.py
+-rw-rw-r--   0 root         (0) root         (0)     8482 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/operations/data_retrieval/admin_request_data_retrieval.py
+-rw-rw-r--   0 root         (0) root         (0)     8413 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/operations/data_retrieval/public_cancel_user_pers_19dafa.py
+-rw-rw-r--   0 root         (0) root         (0)     9455 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/operations/data_retrieval/public_generate_persona_6b68a4.py
+-rw-rw-r--   0 root         (0) root         (0)     9176 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/operations/data_retrieval/public_get_user_persona_7e40c3.py
+-rw-rw-r--   0 root         (0) root         (0)     8359 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/operations/data_retrieval/public_request_data_retrieval.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:46:55.814662 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/operations/platform_account_closure_client/
+-rw-rw-r--   0 root         (0) root         (0)      715 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/operations/platform_account_closure_client/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7706 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/operations/platform_account_closure_client/admin_delete_platform_a_6b01ab.py
+-rw-rw-r--   0 root         (0) root         (0)     8028 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/operations/platform_account_closure_client/admin_get_platform_acco_4a3f07.py
+-rw-rw-r--   0 root         (0) root         (0)     8854 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/operations/platform_account_closure_client/admin_update_platform_a_818a23.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:46:55.814662 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/operations/platform_account_closure_history/
+-rw-rw-r--   0 root         (0) root         (0)      554 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/operations/platform_account_closure_history/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    10606 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/operations/platform_account_closure_history/admin_get_user_platform_8a8aa4.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:46:55.818662 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/wrappers/
+-rw-rw-r--   0 root         (0) root         (0)     5420 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/wrappers/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    29852 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/wrappers/_configuration.py
+-rw-rw-r--   0 root         (0) root         (0)    31388 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/wrappers/_data_deletion.py
+-rw-rw-r--   0 root         (0) root         (0)    30852 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/wrappers/_data_retrieval.py
+-rw-rw-r--   0 root         (0) root         (0)    10866 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/wrappers/_platform_account_closure_client.py
+-rw-rw-r--   0 root         (0) root         (0)     5165 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/wrappers/_platform_account_closure_history.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:46:55.818662 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk_service_gdpr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1113 2024-05-21 03:46:55.000000 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk_service_gdpr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5410 2024-05-21 03:46:55.000000 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk_service_gdpr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 03:46:55.000000 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk_service_gdpr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-21 03:46:55.000000 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk_service_gdpr.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-05-21 03:46:55.000000 accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk_service_gdpr.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)      353 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_gdpr-0.9.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-21 03:46:55.818662 accelbyte_py_sdk_service_gdpr-0.9.0/setup.cfg
```

### Comparing `accelbyte_py_sdk_service_gdpr-0.8.0/PKG-INFO` & `accelbyte_py_sdk_service_gdpr-0.9.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: accelbyte-py-sdk-service-gdpr
-Version: 0.8.0
+Version: 0.9.0
 Summary: AccelByte Python SDK - AccelByte Gaming Services Gdpr Service
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: accelbyte-py-sdk-core
 
 [//]: # (Code generated. DO NOT EDIT!)
 
 # AccelByte Modular Python SDK - Service Module
 
 This is a service module for the [AccelByte Modular Python SDK](https://github.com/AccelByte/accelbyte-python-modular-sdk) package.
 
 ```text
 AccelByte Gaming Services Gdpr Service
-* Version: 2.9.0
+* Version: 2.10.0
 ```
 
 ## Setup
 
 This SDK requires Python 3.9 to be installed.
 
 ### Install with Pip
```

### Comparing `accelbyte_py_sdk_service_gdpr-0.8.0/README.md` & `accelbyte_py_sdk_service_gdpr-0.9.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # AccelByte Modular Python SDK - Service Module
 
 This is a service module for the [AccelByte Modular Python SDK](https://github.com/AccelByte/accelbyte-python-modular-sdk) package.
 
 ```text
 AccelByte Gaming Services Gdpr Service
-* Version: 2.9.0
+* Version: 2.10.0
 ```
 
 ## Setup
 
 This SDK requires Python 3.9 to be installed.
 
 ### Install with Pip
```

### Comparing `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/__init__.py` & `accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,25 +4,31 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: service-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Gdpr Service."""
 
-__version__ = "2.9.0"
+__version__ = "2.10.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 # configuration
+from .wrappers import admin_get_platform_account_closure_services_configuration
+from .wrappers import admin_get_platform_account_closure_services_configuration_async
 from .wrappers import admin_get_services_configuration
 from .wrappers import admin_get_services_configuration_async
+from .wrappers import admin_reset_platform_account_closure_services_configuration
+from .wrappers import admin_reset_platform_account_closure_services_configuration_async
 from .wrappers import admin_reset_services_configuration
 from .wrappers import admin_reset_services_configuration_async
+from .wrappers import admin_update_platform_account_closure_services_configuration
+from .wrappers import admin_update_platform_account_closure_services_configuration_async
 from .wrappers import admin_update_services_configuration
 from .wrappers import admin_update_services_configuration_async
 from .wrappers import delete_admin_email_configuration
 from .wrappers import delete_admin_email_configuration_async
 from .wrappers import get_admin_email_configuration
 from .wrappers import get_admin_email_configuration_async
 from .wrappers import save_admin_email_configuration
@@ -67,7 +73,19 @@
 from .wrappers import public_cancel_user_personal_data_request_async
 from .wrappers import public_generate_personal_data_url
 from .wrappers import public_generate_personal_data_url_async
 from .wrappers import public_get_user_personal_data_requests
 from .wrappers import public_get_user_personal_data_requests_async
 from .wrappers import public_request_data_retrieval
 from .wrappers import public_request_data_retrieval_async
+
+# platform_account_closure_client
+from .wrappers import admin_delete_platform_account_closure_client
+from .wrappers import admin_delete_platform_account_closure_client_async
+from .wrappers import admin_get_platform_account_closure_client
+from .wrappers import admin_get_platform_account_closure_client_async
+from .wrappers import admin_update_platform_account_closure_client
+from .wrappers import admin_update_platform_account_closure_client_async
+
+# platform_account_closure_history
+from .wrappers import admin_get_user_platform_account_closure_histories
+from .wrappers import admin_get_user_platform_account_closure_histories_async
```

### Comparing `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/models/__init__.py` & `accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/models/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,31 +4,43 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: model-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Gdpr Service."""
 
-__version__ = "2.9.0"
+__version__ = "2.10.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .dto_extend_config_dto import DtoExtendConfigDTO
+from .dto_platform_account_closure_client_request import (
+    DtoPlatformAccountClosureClientRequest,
+)
+from .dto_platform_account_closure_client_response import (
+    DtoPlatformAccountClosureClientResponse,
+)
 from .dto_service_config_dto import DtoServiceConfigDTO
 from .dto_service_config_dto import ProtocolEnum as DtoServiceConfigDTOProtocolEnum
 from .dto_service_configuration_dto import DtoServiceConfigurationDTO
 from .dto_service_configuration_dto import (
     TypeEnum as DtoServiceConfigurationDTOTypeEnum,
 )
 from .dto_service_configuration_update_request import (
     DtoServiceConfigurationUpdateRequest,
 )
 from .dto_services_configuration_response import DtoServicesConfigurationResponse
+from .dto_user_platform_account_closure_histories_response import (
+    DtoUserPlatformAccountClosureHistoriesResponse,
+)
+from .dto_user_platform_account_closure_history import (
+    DtoUserPlatformAccountClosureHistory,
+)
 from .models_data_retrieval_response import ModelsDataRetrievalResponse
 from .models_deletion_data import ModelsDeletionData
 from .models_deletion_status import ModelsDeletionStatus
 from .models_list_deletion_data_response import ModelsListDeletionDataResponse
 from .models_list_personal_data_response import ModelsListPersonalDataResponse
 from .models_pagination import ModelsPagination
 from .models_personal_data import ModelsPersonalData
```

### Comparing `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/models/dto_extend_config_dto.py` & `accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/models/dto_extend_config_dto.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/models/dto_service_config_dto.py` & `accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/models/dto_service_config_dto.py`

 * *Files 9% similar despite different names*

```diff
@@ -36,60 +36,77 @@
 class DtoServiceConfigDTO(Model):
     """Dto service config DTO (dto.ServiceConfigDTO)
 
     Properties:
         protocol: (protocol) REQUIRED Union[str, ProtocolEnum]
 
         url: (url) REQUIRED str
+
+        skip_ack: (skipAck) OPTIONAL bool
     """
 
     # region fields
 
     protocol: Union[str, ProtocolEnum]  # REQUIRED
     url: str  # REQUIRED
+    skip_ack: bool  # OPTIONAL
 
     # endregion fields
 
     # region with_x methods
 
     def with_protocol(self, value: Union[str, ProtocolEnum]) -> DtoServiceConfigDTO:
         self.protocol = value
         return self
 
     def with_url(self, value: str) -> DtoServiceConfigDTO:
         self.url = value
         return self
 
+    def with_skip_ack(self, value: bool) -> DtoServiceConfigDTO:
+        self.skip_ack = value
+        return self
+
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
         if hasattr(self, "protocol"):
             result["protocol"] = str(self.protocol)
         elif include_empty:
             result["protocol"] = Union[str, ProtocolEnum]()
         if hasattr(self, "url"):
             result["url"] = str(self.url)
         elif include_empty:
             result["url"] = ""
+        if hasattr(self, "skip_ack"):
+            result["skipAck"] = bool(self.skip_ack)
+        elif include_empty:
+            result["skipAck"] = False
         return result
 
     # endregion to methods
 
     # region static methods
 
     @classmethod
     def create(
-        cls, protocol: Union[str, ProtocolEnum], url: str, **kwargs
+        cls,
+        protocol: Union[str, ProtocolEnum],
+        url: str,
+        skip_ack: Optional[bool] = None,
+        **kwargs,
     ) -> DtoServiceConfigDTO:
         instance = cls()
         instance.protocol = protocol
         instance.url = url
+        if skip_ack is not None:
+            instance.skip_ack = skip_ack
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
     ) -> DtoServiceConfigDTO:
         instance = cls()
@@ -99,14 +116,18 @@
             instance.protocol = str(dict_["protocol"])
         elif include_empty:
             instance.protocol = Union[str, ProtocolEnum]()
         if "url" in dict_ and dict_["url"] is not None:
             instance.url = str(dict_["url"])
         elif include_empty:
             instance.url = ""
+        if "skipAck" in dict_ and dict_["skipAck"] is not None:
+            instance.skip_ack = bool(dict_["skipAck"])
+        elif include_empty:
+            instance.skip_ack = False
         return instance
 
     @classmethod
     def create_many_from_dict(
         cls, dict_: dict, include_empty: bool = False
     ) -> Dict[str, DtoServiceConfigDTO]:
         return (
@@ -142,21 +163,23 @@
             return cls.create_from_dict(any_, include_empty=include_empty)
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
             "protocol": "protocol",
             "url": "url",
+            "skipAck": "skip_ack",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
             "protocol": True,
             "url": True,
+            "skipAck": False,
         }
 
     @staticmethod
     def get_enum_map() -> Dict[str, List[Any]]:
         return {
             "protocol": ["GRPC"],
         }
```

### Comparing `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/models/dto_service_configuration_dto.py` & `accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/models/dto_service_configuration_dto.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/models/dto_service_configuration_update_request.py` & `accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/models/dto_service_configuration_update_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/models/dto_services_configuration_response.py` & `accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/models/dto_services_configuration_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/models/models_data_retrieval_response.py` & `accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/models/models_data_retrieval_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/models/models_deletion_data.py` & `accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/models/models_deletion_data.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/models/models_deletion_status.py` & `accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/models/models_deletion_status.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/models/models_list_deletion_data_response.py` & `accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/models/models_list_deletion_data_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/models/models_list_personal_data_response.py` & `accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/models/models_list_personal_data_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/models/models_pagination.py` & `accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/models/models_pagination.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/models/models_personal_data.py` & `accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/models/models_personal_data.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/models/models_request_delete_response.py` & `accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/models/models_request_delete_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/models/models_user_data_url.py` & `accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/models/models_user_data_url.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/models/models_user_personal_data.py` & `accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/models/models_user_personal_data.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/models/models_user_personal_data_response.py` & `accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/models/models_user_personal_data_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/models/response_error.py` & `accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/models/response_error.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/configuration/__init__.py` & `accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/operations/configuration/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,20 +4,29 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Gdpr Service."""
 
-__version__ = "2.9.0"
+__version__ = "2.10.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
+from .admin_get_platform_acco_c23147 import (
+    AdminGetPlatformAccountClosureServicesConfiguration,
+)
 from .admin_get_services_conf_be46ef import AdminGetServicesConfiguration
+from .admin_reset_platform_ac_c4b31b import (
+    AdminResetPlatformAccountClosureServicesConfiguration,
+)
 from .admin_reset_services_co_abf06c import AdminResetServicesConfiguration
+from .admin_update_platform_a_1f24aa import (
+    AdminUpdatePlatformAccountClosureServicesConfiguration,
+)
 from .admin_update_services_c_ea010e import AdminUpdateServicesConfiguration
 from .delete_admin_email_conf_009cca import DeleteAdminEmailConfiguration
 from .get_admin_email_configuration import GetAdminEmailConfiguration
 from .save_admin_email_configuration import SaveAdminEmailConfiguration
 from .update_admin_email_conf_71e966 import UpdateAdminEmailConfiguration
```

### Comparing `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/configuration/admin_get_services_conf_be46ef.py` & `accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/operations/configuration/admin_get_services_conf_be46ef.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/configuration/admin_reset_services_co_abf06c.py` & `accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/operations/configuration/admin_reset_services_co_abf06c.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/configuration/admin_update_services_c_ea010e.py` & `accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/operations/configuration/admin_update_services_c_ea010e.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/configuration/delete_admin_email_conf_009cca.py` & `accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/operations/configuration/delete_admin_email_conf_009cca.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/configuration/get_admin_email_configuration.py` & `accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/operations/configuration/get_admin_email_configuration.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/configuration/save_admin_email_configuration.py` & `accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/operations/configuration/save_admin_email_configuration.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/configuration/update_admin_email_conf_71e966.py` & `accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/operations/configuration/update_admin_email_conf_71e966.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/__init__.py` & `accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Gdpr Service."""
 
-__version__ = "2.9.0"
+__version__ = "2.10.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .admin_cancel_user_accou_de1ba5 import AdminCancelUserAccountDeletionRequest
 from .admin_get_list_deletion_227d7d import AdminGetListDeletionDataRequest
```

### Comparing `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/admin_cancel_user_accou_de1ba5.py` & `accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/admin_cancel_user_accou_de1ba5.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/admin_get_list_deletion_227d7d.py` & `accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/admin_get_list_deletion_227d7d.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/admin_get_user_account__84ef5a.py` & `accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/admin_get_user_account__84ef5a.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/admin_submit_user_accou_b7780f.py` & `accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/admin_submit_user_accou_b7780f.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/public_cancel_my_accoun_107811.py` & `accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/public_cancel_my_accoun_107811.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/public_cancel_user_acco_16b962.py` & `accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/public_cancel_user_acco_16b962.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/public_get_my_account_d_8595d0.py` & `accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/public_get_my_account_d_8595d0.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/public_get_user_account_09e4f2.py` & `accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/public_get_user_account_09e4f2.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/public_submit_my_accoun_f5ded3.py` & `accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/public_submit_my_accoun_f5ded3.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/public_submit_user_acco_a6db4f.py` & `accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/public_submit_user_acco_a6db4f.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_retrieval/__init__.py` & `accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/operations/data_retrieval/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Gdpr Service."""
 
-__version__ = "2.9.0"
+__version__ = "2.10.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .admin_cancel_user_perso_78952d import AdminCancelUserPersonalDataRequest
 from .admin_generate_personal_48c32b import AdminGeneratePersonalDataURL
```

### Comparing `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_retrieval/admin_cancel_user_perso_78952d.py` & `accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/operations/data_retrieval/admin_cancel_user_perso_78952d.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_retrieval/admin_generate_personal_48c32b.py` & `accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/operations/data_retrieval/admin_generate_personal_48c32b.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_retrieval/admin_get_list_personal_424fda.py` & `accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/operations/data_retrieval/admin_get_list_personal_424fda.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_retrieval/admin_get_user_personal_a892c0.py` & `accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/operations/data_retrieval/admin_get_user_personal_a892c0.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_retrieval/admin_request_data_retrieval.py` & `accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/operations/data_retrieval/admin_request_data_retrieval.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_retrieval/public_cancel_user_pers_19dafa.py` & `accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/operations/data_retrieval/public_cancel_user_pers_19dafa.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_retrieval/public_generate_persona_6b68a4.py` & `accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/operations/data_retrieval/public_generate_persona_6b68a4.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_retrieval/public_get_user_persona_7e40c3.py` & `accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/operations/data_retrieval/public_get_user_persona_7e40c3.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_retrieval/public_request_data_retrieval.py` & `accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/operations/data_retrieval/public_request_data_retrieval.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/wrappers/__init__.py` & `accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/wrappers/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,24 +4,36 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: wrapper-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Gdpr Service."""
 
-__version__ = "2.9.0"
+__version__ = "2.10.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
+from ._configuration import admin_get_platform_account_closure_services_configuration
+from ._configuration import (
+    admin_get_platform_account_closure_services_configuration_async,
+)
 from ._configuration import admin_get_services_configuration
 from ._configuration import admin_get_services_configuration_async
+from ._configuration import admin_reset_platform_account_closure_services_configuration
+from ._configuration import (
+    admin_reset_platform_account_closure_services_configuration_async,
+)
 from ._configuration import admin_reset_services_configuration
 from ._configuration import admin_reset_services_configuration_async
+from ._configuration import admin_update_platform_account_closure_services_configuration
+from ._configuration import (
+    admin_update_platform_account_closure_services_configuration_async,
+)
 from ._configuration import admin_update_services_configuration
 from ._configuration import admin_update_services_configuration_async
 from ._configuration import delete_admin_email_configuration
 from ._configuration import delete_admin_email_configuration_async
 from ._configuration import get_admin_email_configuration
 from ._configuration import get_admin_email_configuration_async
 from ._configuration import save_admin_email_configuration
@@ -64,7 +76,31 @@
 from ._data_retrieval import public_cancel_user_personal_data_request_async
 from ._data_retrieval import public_generate_personal_data_url
 from ._data_retrieval import public_generate_personal_data_url_async
 from ._data_retrieval import public_get_user_personal_data_requests
 from ._data_retrieval import public_get_user_personal_data_requests_async
 from ._data_retrieval import public_request_data_retrieval
 from ._data_retrieval import public_request_data_retrieval_async
+
+from ._platform_account_closure_client import (
+    admin_delete_platform_account_closure_client,
+)
+from ._platform_account_closure_client import (
+    admin_delete_platform_account_closure_client_async,
+)
+from ._platform_account_closure_client import admin_get_platform_account_closure_client
+from ._platform_account_closure_client import (
+    admin_get_platform_account_closure_client_async,
+)
+from ._platform_account_closure_client import (
+    admin_update_platform_account_closure_client,
+)
+from ._platform_account_closure_client import (
+    admin_update_platform_account_closure_client_async,
+)
+
+from ._platform_account_closure_history import (
+    admin_get_user_platform_account_closure_histories,
+)
+from ._platform_account_closure_history import (
+    admin_get_user_platform_account_closure_histories_async,
+)
```

### Comparing `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/wrappers/_configuration.py` & `accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/wrappers/_configuration.py`

 * *Files 20% similar despite different names*

```diff
@@ -29,23 +29,130 @@
 from accelbyte_py_sdk.core import run_request_async
 from accelbyte_py_sdk.core import same_doc_as
 
 from ..models import DtoServiceConfigurationUpdateRequest
 from ..models import DtoServicesConfigurationResponse
 from ..models import ResponseError
 
+from ..operations.configuration import (
+    AdminGetPlatformAccountClosureServicesConfiguration,
+)
 from ..operations.configuration import AdminGetServicesConfiguration
+from ..operations.configuration import (
+    AdminResetPlatformAccountClosureServicesConfiguration,
+)
 from ..operations.configuration import AdminResetServicesConfiguration
+from ..operations.configuration import (
+    AdminUpdatePlatformAccountClosureServicesConfiguration,
+)
 from ..operations.configuration import AdminUpdateServicesConfiguration
 from ..operations.configuration import DeleteAdminEmailConfiguration
 from ..operations.configuration import GetAdminEmailConfiguration
 from ..operations.configuration import SaveAdminEmailConfiguration
 from ..operations.configuration import UpdateAdminEmailConfiguration
 
 
+@same_doc_as(AdminGetPlatformAccountClosureServicesConfiguration)
+def admin_get_platform_account_closure_services_configuration(
+    namespace: Optional[str] = None,
+    x_additional_headers: Optional[Dict[str, str]] = None,
+    **kwargs
+):
+    """Get Registered Platform Account Closure Services Configuration (AdminGetPlatformAccountClosureServicesConfiguration)
+
+    Get registered platform account closure services configuration.
+    Scope: account
+
+    Required Scope(s):
+        - account
+
+    Properties:
+        url: /gdpr/admin/namespaces/{namespace}/services/platforms/closure/config
+
+        method: GET
+
+        tags: ["Configuration"]
+
+        consumes: ["application/json"]
+
+        produces: ["application/json"]
+
+        securities: [BEARER_AUTH]
+
+        namespace: (namespace) REQUIRED str in path
+
+    Responses:
+        200: OK - DtoServicesConfigurationResponse (OK)
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
+    request = AdminGetPlatformAccountClosureServicesConfiguration.create(
+        namespace=namespace,
+    )
+    return run_request(request, additional_headers=x_additional_headers, **kwargs)
+
+
+@same_doc_as(AdminGetPlatformAccountClosureServicesConfiguration)
+async def admin_get_platform_account_closure_services_configuration_async(
+    namespace: Optional[str] = None,
+    x_additional_headers: Optional[Dict[str, str]] = None,
+    **kwargs
+):
+    """Get Registered Platform Account Closure Services Configuration (AdminGetPlatformAccountClosureServicesConfiguration)
+
+    Get registered platform account closure services configuration.
+    Scope: account
+
+    Required Scope(s):
+        - account
+
+    Properties:
+        url: /gdpr/admin/namespaces/{namespace}/services/platforms/closure/config
+
+        method: GET
+
+        tags: ["Configuration"]
+
+        consumes: ["application/json"]
+
+        produces: ["application/json"]
+
+        securities: [BEARER_AUTH]
+
+        namespace: (namespace) REQUIRED str in path
+
+    Responses:
+        200: OK - DtoServicesConfigurationResponse (OK)
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
+    request = AdminGetPlatformAccountClosureServicesConfiguration.create(
+        namespace=namespace,
+    )
+    return await run_request_async(
+        request, additional_headers=x_additional_headers, **kwargs
+    )
+
+
 @same_doc_as(AdminGetServicesConfiguration)
 def admin_get_services_configuration(
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Get Registered Services Configuration (AdminGetServicesConfiguration)
@@ -136,14 +243,110 @@
         namespace=namespace,
     )
     return await run_request_async(
         request, additional_headers=x_additional_headers, **kwargs
     )
 
 
+@same_doc_as(AdminResetPlatformAccountClosureServicesConfiguration)
+def admin_reset_platform_account_closure_services_configuration(
+    namespace: Optional[str] = None,
+    x_additional_headers: Optional[Dict[str, str]] = None,
+    **kwargs
+):
+    """Reset Registered Platform Account Closure Services Configuration (AdminResetPlatformAccountClosureServicesConfiguration)
+
+    **[TEST FACILITY ONLY]**
+    Reset registered platform account closure services configuration to use the default configuration.
+    Scope: account
+
+    Required Scope(s):
+        - account
+
+    Properties:
+        url: /gdpr/admin/namespaces/{namespace}/services/platforms/closure/config
+
+        method: DELETE
+
+        tags: ["Configuration"]
+
+        consumes: ["application/json"]
+
+        produces: ["application/json"]
+
+        securities: [BEARER_AUTH]
+
+        namespace: (namespace) REQUIRED str in path
+
+    Responses:
+        204: No Content - (No Content)
+
+        401: Unauthorized - ResponseError (Unauthorized)
+
+        500: Internal Server Error - ResponseError (Internal Server Error)
+    """
+    if namespace is None:
+        namespace, error = get_services_namespace()
+        if error:
+            return None, error
+    request = AdminResetPlatformAccountClosureServicesConfiguration.create(
+        namespace=namespace,
+    )
+    return run_request(request, additional_headers=x_additional_headers, **kwargs)
+
+
+@same_doc_as(AdminResetPlatformAccountClosureServicesConfiguration)
+async def admin_reset_platform_account_closure_services_configuration_async(
+    namespace: Optional[str] = None,
+    x_additional_headers: Optional[Dict[str, str]] = None,
+    **kwargs
+):
+    """Reset Registered Platform Account Closure Services Configuration (AdminResetPlatformAccountClosureServicesConfiguration)
+
+    **[TEST FACILITY ONLY]**
+    Reset registered platform account closure services configuration to use the default configuration.
+    Scope: account
+
+    Required Scope(s):
+        - account
+
+    Properties:
+        url: /gdpr/admin/namespaces/{namespace}/services/platforms/closure/config
+
+        method: DELETE
+
+        tags: ["Configuration"]
+
+        consumes: ["application/json"]
+
+        produces: ["application/json"]
+
+        securities: [BEARER_AUTH]
+
+        namespace: (namespace) REQUIRED str in path
+
+    Responses:
+        204: No Content - (No Content)
+
+        401: Unauthorized - ResponseError (Unauthorized)
+
+        500: Internal Server Error - ResponseError (Internal Server Error)
+    """
+    if namespace is None:
+        namespace, error = get_services_namespace()
+        if error:
+            return None, error
+    request = AdminResetPlatformAccountClosureServicesConfiguration.create(
+        namespace=namespace,
+    )
+    return await run_request_async(
+        request, additional_headers=x_additional_headers, **kwargs
+    )
+
+
 @same_doc_as(AdminResetServicesConfiguration)
 def admin_reset_services_configuration(
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Reset Registered Services Configuration (AdminResetServicesConfiguration)
@@ -232,14 +435,120 @@
         namespace=namespace,
     )
     return await run_request_async(
         request, additional_headers=x_additional_headers, **kwargs
     )
 
 
+@same_doc_as(AdminUpdatePlatformAccountClosureServicesConfiguration)
+def admin_update_platform_account_closure_services_configuration(
+    body: DtoServiceConfigurationUpdateRequest,
+    namespace: Optional[str] = None,
+    x_additional_headers: Optional[Dict[str, str]] = None,
+    **kwargs
+):
+    """Update Registered Platform Account Closure Services Configuration (AdminUpdatePlatformAccountClosureServicesConfiguration)
+
+    Update registered platform account closure services configuration.
+    Scope: account
+
+    Required Scope(s):
+        - account
+
+    Properties:
+        url: /gdpr/admin/namespaces/{namespace}/services/platforms/closure/config
+
+        method: PUT
+
+        tags: ["Configuration"]
+
+        consumes: ["application/json"]
+
+        produces: ["application/json"]
+
+        securities: [BEARER_AUTH]
+
+        body: (body) REQUIRED DtoServiceConfigurationUpdateRequest in body
+
+        namespace: (namespace) REQUIRED str in path
+
+    Responses:
+        200: OK - DtoServiceConfigurationUpdateRequest (OK)
+
+        400: Bad Request - ResponseError (Bad Request)
+
+        401: Unauthorized - ResponseError (Unauthorized)
+
+        500: Internal Server Error - ResponseError (Internal Server Error)
+    """
+    if namespace is None:
+        namespace, error = get_services_namespace()
+        if error:
+            return None, error
+    request = AdminUpdatePlatformAccountClosureServicesConfiguration.create(
+        body=body,
+        namespace=namespace,
+    )
+    return run_request(request, additional_headers=x_additional_headers, **kwargs)
+
+
+@same_doc_as(AdminUpdatePlatformAccountClosureServicesConfiguration)
+async def admin_update_platform_account_closure_services_configuration_async(
+    body: DtoServiceConfigurationUpdateRequest,
+    namespace: Optional[str] = None,
+    x_additional_headers: Optional[Dict[str, str]] = None,
+    **kwargs
+):
+    """Update Registered Platform Account Closure Services Configuration (AdminUpdatePlatformAccountClosureServicesConfiguration)
+
+    Update registered platform account closure services configuration.
+    Scope: account
+
+    Required Scope(s):
+        - account
+
+    Properties:
+        url: /gdpr/admin/namespaces/{namespace}/services/platforms/closure/config
+
+        method: PUT
+
+        tags: ["Configuration"]
+
+        consumes: ["application/json"]
+
+        produces: ["application/json"]
+
+        securities: [BEARER_AUTH]
+
+        body: (body) REQUIRED DtoServiceConfigurationUpdateRequest in body
+
+        namespace: (namespace) REQUIRED str in path
+
+    Responses:
+        200: OK - DtoServiceConfigurationUpdateRequest (OK)
+
+        400: Bad Request - ResponseError (Bad Request)
+
+        401: Unauthorized - ResponseError (Unauthorized)
+
+        500: Internal Server Error - ResponseError (Internal Server Error)
+    """
+    if namespace is None:
+        namespace, error = get_services_namespace()
+        if error:
+            return None, error
+    request = AdminUpdatePlatformAccountClosureServicesConfiguration.create(
+        body=body,
+        namespace=namespace,
+    )
+    return await run_request_async(
+        request, additional_headers=x_additional_headers, **kwargs
+    )
+
+
 @same_doc_as(AdminUpdateServicesConfiguration)
 def admin_update_services_configuration(
     body: DtoServiceConfigurationUpdateRequest,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
```

### Comparing `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/wrappers/_data_deletion.py` & `accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/wrappers/_data_deletion.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/wrappers/_data_retrieval.py` & `accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk/api/gdpr/wrappers/_data_retrieval.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk_service_gdpr.egg-info/PKG-INFO` & `accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk_service_gdpr.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: accelbyte-py-sdk-service-gdpr
-Version: 0.8.0
+Version: 0.9.0
 Summary: AccelByte Python SDK - AccelByte Gaming Services Gdpr Service
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: accelbyte-py-sdk-core
 
 [//]: # (Code generated. DO NOT EDIT!)
 
 # AccelByte Modular Python SDK - Service Module
 
 This is a service module for the [AccelByte Modular Python SDK](https://github.com/AccelByte/accelbyte-python-modular-sdk) package.
 
 ```text
 AccelByte Gaming Services Gdpr Service
-* Version: 2.9.0
+* Version: 2.10.0
 ```
 
 ## Setup
 
 This SDK requires Python 3.9 to be installed.
 
 ### Install with Pip
```

### Comparing `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk_service_gdpr.egg-info/SOURCES.txt` & `accelbyte_py_sdk_service_gdpr-0.9.0/accelbyte_py_sdk_service_gdpr.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,32 +1,39 @@
 README.md
 pyproject.toml
 accelbyte_py_sdk/api/gdpr/__init__.py
 accelbyte_py_sdk/api/gdpr/models/__init__.py
 accelbyte_py_sdk/api/gdpr/models/dto_extend_config_dto.py
+accelbyte_py_sdk/api/gdpr/models/dto_platform_account_closure_client_request.py
+accelbyte_py_sdk/api/gdpr/models/dto_platform_account_closure_client_response.py
 accelbyte_py_sdk/api/gdpr/models/dto_service_config_dto.py
 accelbyte_py_sdk/api/gdpr/models/dto_service_configuration_dto.py
 accelbyte_py_sdk/api/gdpr/models/dto_service_configuration_update_request.py
 accelbyte_py_sdk/api/gdpr/models/dto_services_configuration_response.py
+accelbyte_py_sdk/api/gdpr/models/dto_user_platform_account_closure_histories_response.py
+accelbyte_py_sdk/api/gdpr/models/dto_user_platform_account_closure_history.py
 accelbyte_py_sdk/api/gdpr/models/models_data_retrieval_response.py
 accelbyte_py_sdk/api/gdpr/models/models_deletion_data.py
 accelbyte_py_sdk/api/gdpr/models/models_deletion_status.py
 accelbyte_py_sdk/api/gdpr/models/models_list_deletion_data_response.py
 accelbyte_py_sdk/api/gdpr/models/models_list_personal_data_response.py
 accelbyte_py_sdk/api/gdpr/models/models_pagination.py
 accelbyte_py_sdk/api/gdpr/models/models_personal_data.py
 accelbyte_py_sdk/api/gdpr/models/models_request_delete_response.py
 accelbyte_py_sdk/api/gdpr/models/models_user_data_url.py
 accelbyte_py_sdk/api/gdpr/models/models_user_personal_data.py
 accelbyte_py_sdk/api/gdpr/models/models_user_personal_data_response.py
 accelbyte_py_sdk/api/gdpr/models/response_error.py
 accelbyte_py_sdk/api/gdpr/operations/__init__.py
 accelbyte_py_sdk/api/gdpr/operations/configuration/__init__.py
+accelbyte_py_sdk/api/gdpr/operations/configuration/admin_get_platform_acco_c23147.py
 accelbyte_py_sdk/api/gdpr/operations/configuration/admin_get_services_conf_be46ef.py
+accelbyte_py_sdk/api/gdpr/operations/configuration/admin_reset_platform_ac_c4b31b.py
 accelbyte_py_sdk/api/gdpr/operations/configuration/admin_reset_services_co_abf06c.py
+accelbyte_py_sdk/api/gdpr/operations/configuration/admin_update_platform_a_1f24aa.py
 accelbyte_py_sdk/api/gdpr/operations/configuration/admin_update_services_c_ea010e.py
 accelbyte_py_sdk/api/gdpr/operations/configuration/delete_admin_email_conf_009cca.py
 accelbyte_py_sdk/api/gdpr/operations/configuration/get_admin_email_configuration.py
 accelbyte_py_sdk/api/gdpr/operations/configuration/save_admin_email_configuration.py
 accelbyte_py_sdk/api/gdpr/operations/configuration/update_admin_email_conf_71e966.py
 accelbyte_py_sdk/api/gdpr/operations/data_deletion/__init__.py
 accelbyte_py_sdk/api/gdpr/operations/data_deletion/admin_cancel_user_accou_de1ba5.py
@@ -45,16 +52,24 @@
 accelbyte_py_sdk/api/gdpr/operations/data_retrieval/admin_get_list_personal_424fda.py
 accelbyte_py_sdk/api/gdpr/operations/data_retrieval/admin_get_user_personal_a892c0.py
 accelbyte_py_sdk/api/gdpr/operations/data_retrieval/admin_request_data_retrieval.py
 accelbyte_py_sdk/api/gdpr/operations/data_retrieval/public_cancel_user_pers_19dafa.py
 accelbyte_py_sdk/api/gdpr/operations/data_retrieval/public_generate_persona_6b68a4.py
 accelbyte_py_sdk/api/gdpr/operations/data_retrieval/public_get_user_persona_7e40c3.py
 accelbyte_py_sdk/api/gdpr/operations/data_retrieval/public_request_data_retrieval.py
+accelbyte_py_sdk/api/gdpr/operations/platform_account_closure_client/__init__.py
+accelbyte_py_sdk/api/gdpr/operations/platform_account_closure_client/admin_delete_platform_a_6b01ab.py
+accelbyte_py_sdk/api/gdpr/operations/platform_account_closure_client/admin_get_platform_acco_4a3f07.py
+accelbyte_py_sdk/api/gdpr/operations/platform_account_closure_client/admin_update_platform_a_818a23.py
+accelbyte_py_sdk/api/gdpr/operations/platform_account_closure_history/__init__.py
+accelbyte_py_sdk/api/gdpr/operations/platform_account_closure_history/admin_get_user_platform_8a8aa4.py
 accelbyte_py_sdk/api/gdpr/wrappers/__init__.py
 accelbyte_py_sdk/api/gdpr/wrappers/_configuration.py
 accelbyte_py_sdk/api/gdpr/wrappers/_data_deletion.py
 accelbyte_py_sdk/api/gdpr/wrappers/_data_retrieval.py
+accelbyte_py_sdk/api/gdpr/wrappers/_platform_account_closure_client.py
+accelbyte_py_sdk/api/gdpr/wrappers/_platform_account_closure_history.py
 accelbyte_py_sdk_service_gdpr.egg-info/PKG-INFO
 accelbyte_py_sdk_service_gdpr.egg-info/SOURCES.txt
 accelbyte_py_sdk_service_gdpr.egg-info/dependency_links.txt
 accelbyte_py_sdk_service_gdpr.egg-info/requires.txt
 accelbyte_py_sdk_service_gdpr.egg-info/top_level.txt
```

