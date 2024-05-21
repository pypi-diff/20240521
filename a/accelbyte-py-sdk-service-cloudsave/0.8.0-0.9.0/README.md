# Comparing `tmp/accelbyte-py-sdk-service-cloudsave-0.8.0.tar.gz` & `tmp/accelbyte-py-sdk-service-cloudsave-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accelbyte-py-sdk-service-cloudsave-0.8.0.tar", last modified: Tue Feb 27 05:35:50 2024, max compression
+gzip compressed data, was "accelbyte-py-sdk-service-cloudsave-0.9.0.tar", last modified: Wed Mar 13 06:10:32 2024, max compression
```

## Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0.tar` & `accelbyte-py-sdk-service-cloudsave-0.9.0.tar`

### file list

```diff
@@ -1,233 +1,238 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:35:50.668927 accelbyte-py-sdk-service-cloudsave-0.8.0/
--rw-r--r--   0 root         (0) root         (0)     1133 2024-02-27 05:35:50.668927 accelbyte-py-sdk-service-cloudsave-0.8.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      877 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:35:50.648927 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:35:50.648927 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:35:50.648927 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/
--rw-rw-r--   0 root         (0) root         (0)    12802 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:35:50.656927 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/
--rw-rw-r--   0 root         (0) root         (0)     7403 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6785 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_admin_concurrent_record_request.py
--rw-rw-r--   0 root         (0) root         (0)     4756 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_admin_game_concurrent_record_request.py
--rw-rw-r--   0 root         (0) root         (0)     3907 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_admin_game_record_request.py
--rw-rw-r--   0 root         (0) root         (0)     6612 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_admin_game_record_response.py
--rw-rw-r--   0 root         (0) root         (0)     4780 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_admin_player_concurrent_record_request.py
--rw-rw-r--   0 root         (0) root         (0)     4434 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_admin_player_record_key_info.py
--rw-rw-r--   0 root         (0) root         (0)     3927 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_admin_player_record_request.py
--rw-rw-r--   0 root         (0) root         (0)     7286 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_admin_player_record_response.py
--rw-rw-r--   0 root         (0) root         (0)     3692 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_app_config.py
--rw-rw-r--   0 root         (0) root         (0)     7335 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_binary_info_response.py
--rw-rw-r--   0 root         (0) root         (0)     4686 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_binary_record_request.py
--rw-rw-r--   0 root         (0) root         (0)     3929 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_bulk_get_admin_game_record_request.py
--rw-rw-r--   0 root         (0) root         (0)     4376 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_bulk_get_admin_game_record_response.py
--rw-rw-r--   0 root         (0) root         (0)     3951 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_bulk_get_admin_player_record_request.py
--rw-rw-r--   0 root         (0) root         (0)     4412 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_bulk_get_admin_player_record_response.py
--rw-rw-r--   0 root         (0) root         (0)     4394 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_bulk_get_game_binary_record_response.py
--rw-rw-r--   0 root         (0) root         (0)     3873 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_bulk_get_game_record_request.py
--rw-rw-r--   0 root         (0) root         (0)     4284 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_bulk_get_game_record_response.py
--rw-rw-r--   0 root         (0) root         (0)     4439 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_bulk_get_player_binary_record_response.py
--rw-rw-r--   0 root         (0) root         (0)     4320 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_bulk_get_player_record_response.py
--rw-rw-r--   0 root         (0) root         (0)     4394 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_bulk_get_player_record_size_response.py
--rw-rw-r--   0 root         (0) root         (0)     3906 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_bulk_get_player_records_request.py
--rw-rw-r--   0 root         (0) root         (0)     4661 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_bulk_update_player_record_request_detail.py
--rw-rw-r--   0 root         (0) root         (0)     5273 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_bulk_update_player_record_response.py
--rw-rw-r--   0 root         (0) root         (0)     4470 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_bulk_update_player_records_request.py
--rw-rw-r--   0 root         (0) root         (0)     3879 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_bulk_user_i_ds_request.py
--rw-rw-r--   0 root         (0) root         (0)     4126 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_bulk_user_key_request.py
--rw-rw-r--   0 root         (0) root         (0)     4632 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_concurrent_record_request.py
--rw-rw-r--   0 root         (0) root         (0)     3819 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_custom_config.py
--rw-rw-r--   0 root         (0) root         (0)    19080 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_custom_function.py
--rw-rw-r--   0 root         (0) root         (0)     9276 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_game_binary_record_admin_response.py
--rw-rw-r--   0 root         (0) root         (0)     6529 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_game_binary_record_create.py
--rw-rw-r--   0 root         (0) root         (0)     5410 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_game_binary_record_metadata_request.py
--rw-rw-r--   0 root         (0) root         (0)     8135 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_game_binary_record_response.py
--rw-rw-r--   0 root         (0) root         (0)     8722 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_game_record_admin_response.py
--rw-rw-r--   0 root         (0) root         (0)     3842 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_game_record_request.py
--rw-rw-r--   0 root         (0) root         (0)     7572 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_game_record_response.py
--rw-rw-r--   0 root         (0) root         (0)     4863 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_list_admin_game_record_keys_response.py
--rw-rw-r--   0 root         (0) root         (0)     5341 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_list_admin_player_record_keys_response.py
--rw-rw-r--   0 root         (0) root         (0)     5397 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_list_game_binary_records_admin_response.py
--rw-rw-r--   0 root         (0) root         (0)     5291 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_list_game_binary_records_response.py
--rw-rw-r--   0 root         (0) root         (0)     4788 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_list_game_record_keys_response.py
--rw-rw-r--   0 root         (0) root         (0)     5338 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_list_player_binary_records_response.py
--rw-rw-r--   0 root         (0) root         (0)     5219 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_list_player_record_keys_response.py
--rw-rw-r--   0 root         (0) root         (0)     4921 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_list_tags_response.py
--rw-rw-r--   0 root         (0) root         (0)     5438 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_pagination.py
--rw-rw-r--   0 root         (0) root         (0)     6266 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_player_binary_record_create.py
--rw-rw-r--   0 root         (0) root         (0)     4181 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_player_binary_record_metadata_public_request.py
--rw-rw-r--   0 root         (0) root         (0)     5182 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_player_binary_record_metadata_request.py
--rw-rw-r--   0 root         (0) root         (0)     9509 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_player_binary_record_response.py
--rw-rw-r--   0 root         (0) root         (0)     4085 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_player_record_concurrent_update_response.py
--rw-rw-r--   0 root         (0) root         (0)     4373 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_player_record_key_info.py
--rw-rw-r--   0 root         (0) root         (0)     3876 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_player_record_request.py
--rw-rw-r--   0 root         (0) root         (0)     8934 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_player_record_response.py
--rw-rw-r--   0 root         (0) root         (0)     6677 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_player_record_size_response.py
--rw-rw-r--   0 root         (0) root         (0)     7472 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_plugin_request.py
--rw-rw-r--   0 root         (0) root         (0)     8176 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_plugin_response.py
--rw-rw-r--   0 root         (0) root         (0)     4536 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_public_game_binary_record_create.py
--rw-rw-r--   0 root         (0) root         (0)     5309 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_public_player_binary_record_create.py
--rw-rw-r--   0 root         (0) root         (0)     4538 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_response_error.py
--rw-rw-r--   0 root         (0) root         (0)     4256 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_tag_info.py
--rw-rw-r--   0 root         (0) root         (0)     3611 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_tag_request.py
--rw-rw-r--   0 root         (0) root         (0)     4746 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_ttl_config_dto.py
--rw-rw-r--   0 root         (0) root         (0)     3929 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_upload_binary_record_request.py
--rw-rw-r--   0 root         (0) root         (0)     5963 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_upload_binary_record_response.py
--rw-rw-r--   0 root         (0) root         (0)     4386 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_user_key_request.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:35:50.656927 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/
--rw-rw-r--   0 root         (0) root         (0)      438 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:35:50.656927 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_concurrent_record/
--rw-rw-r--   0 root         (0) root         (0)      912 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_concurrent_record/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    10693 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_concurrent_record/admin_put_admin_game_re_99ac43.py
--rw-rw-r--   0 root         (0) root         (0)    12931 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_concurrent_record/admin_put_admin_player__e84e5d.py
--rw-rw-r--   0 root         (0) root         (0)    11005 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_concurrent_record/admin_put_game_record_c_886b02.py
--rw-rw-r--   0 root         (0) root         (0)    13310 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_concurrent_record/admin_put_player_public_1624a9.py
--rw-rw-r--   0 root         (0) root         (0)    13281 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_concurrent_record/admin_put_player_record_233704.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:35:50.656927 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_game_binary_record/
--rw-rw-r--   0 root         (0) root         (0)      988 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_game_binary_record/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7474 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_game_binary_record/admin_delete_game_binar_3752d7.py
--rw-rw-r--   0 root         (0) root         (0)     7400 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_game_binary_record/admin_get_game_binary_r_5df25c.py
--rw-rw-r--   0 root         (0) root         (0)     9321 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_game_binary_record/admin_list_game_binary__f439a9.py
--rw-rw-r--   0 root         (0) root         (0)     8662 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_game_binary_record/admin_post_game_binary__ace069.py
--rw-rw-r--   0 root         (0) root         (0)     9228 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_game_binary_record/admin_post_game_binary__ce9dc6.py
--rw-rw-r--   0 root         (0) root         (0)     8884 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_game_binary_record/admin_put_game_binary_r_47597f.py
--rw-rw-r--   0 root         (0) root         (0)     8978 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_game_binary_record/admin_put_game_binary_r_a490ed.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:35:50.656927 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_game_record/
--rw-rw-r--   0 root         (0) root         (0)      830 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_game_record/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7312 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_game_record/admin_delete_game_recor_636983.py
--rw-rw-r--   0 root         (0) root         (0)     7434 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_game_record/admin_get_game_record_h_f6ed3a.py
--rw-rw-r--   0 root         (0) root         (0)    10795 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_game_record/admin_post_game_record__9a2084.py
--rw-rw-r--   0 root         (0) root         (0)    10587 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_game_record/admin_put_game_record_h_0dd624.py
--rw-rw-r--   0 root         (0) root         (0)     9120 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_game_record/list_game_records_handler_v1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:35:50.656927 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_binary_record/
--rw-rw-r--   0 root         (0) root         (0)     1002 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_binary_record/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8019 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_binary_record/admin_delete_player_bin_892eb5.py
--rw-rw-r--   0 root         (0) root         (0)     8194 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_binary_record/admin_get_player_binary_1076b9.py
--rw-rw-r--   0 root         (0) root         (0)    10079 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_binary_record/admin_list_player_binar_e452ce.py
--rw-rw-r--   0 root         (0) root         (0)     9491 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_binary_record/admin_post_player_binar_e33f40.py
--rw-rw-r--   0 root         (0) root         (0)     9941 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_binary_record/admin_post_player_binar_f1a4e9.py
--rw-rw-r--   0 root         (0) root         (0)     9607 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_binary_record/admin_put_player_binary_6424e4.py
--rw-rw-r--   0 root         (0) root         (0)     9785 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_binary_record/admin_put_player_binary_bcf941.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:35:50.660927 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_record/
--rw-rw-r--   0 root         (0) root         (0)     1539 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_record/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8855 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_record/admin_delete_player_pub_f11fd7.py
--rw-rw-r--   0 root         (0) root         (0)     7781 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_record/admin_delete_player_rec_168241.py
--rw-rw-r--   0 root         (0) root         (0)     8287 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_record/admin_get_player_public_f015b6.py
--rw-rw-r--   0 root         (0) root         (0)     8244 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_record/admin_get_player_record_b37faa.py
--rw-rw-r--   0 root         (0) root         (0)     8212 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_record/admin_get_player_record_d622c9.py
--rw-rw-r--   0 root         (0) root         (0)     9310 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_record/admin_get_player_record_f4a5eb.py
--rw-rw-r--   0 root         (0) root         (0)    10910 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_record/admin_post_player_publi_98e39e.py
--rw-rw-r--   0 root         (0) root         (0)    11245 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_record/admin_post_player_recor_6a96c8.py
--rw-rw-r--   0 root         (0) root         (0)    10765 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_record/admin_put_player_public_819faf.py
--rw-rw-r--   0 root         (0) root         (0)     9073 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_record/admin_put_player_record_253e92.py
--rw-rw-r--   0 root         (0) root         (0)    11074 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_record/admin_put_player_record_a8195d.py
--rw-rw-r--   0 root         (0) root         (0)     9256 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_record/admin_retrieve_player_records.py
--rw-rw-r--   0 root         (0) root         (0)     7997 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_record/bulk_get_player_record__4627ec.py
--rw-rw-r--   0 root         (0) root         (0)     9308 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_record/list_player_record_handler_v1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:35:50.660927 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_record/
--rw-rw-r--   0 root         (0) root         (0)     1420 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_record/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8383 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_record/admin_bulk_get_admin_ga_c5c529.py
--rw-rw-r--   0 root         (0) root         (0)     9297 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_record/admin_bulk_get_admin_pl_b8e62a.py
--rw-rw-r--   0 root         (0) root         (0)     7160 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_record/admin_delete_admin_game_1f080f.py
--rw-rw-r--   0 root         (0) root         (0)     8016 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_record/admin_delete_admin_play_632fe7.py
--rw-rw-r--   0 root         (0) root         (0)     7434 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_record/admin_get_admin_game_record_v1.py
--rw-rw-r--   0 root         (0) root         (0)     8271 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_record/admin_get_admin_player__37ad38.py
--rw-rw-r--   0 root         (0) root         (0)     9247 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_record/admin_list_admin_game_r_476bfb.py
--rw-rw-r--   0 root         (0) root         (0)     9359 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_record/admin_list_admin_user_r_83dd7a.py
--rw-rw-r--   0 root         (0) root         (0)     9782 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_record/admin_post_admin_game_r_e8f678.py
--rw-rw-r--   0 root         (0) root         (0)    10402 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_record/admin_post_player_admin_b138ee.py
--rw-rw-r--   0 root         (0) root         (0)     9500 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_record/admin_put_admin_game_record_v1.py
--rw-rw-r--   0 root         (0) root         (0)    10233 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_record/admin_put_admin_player__6ed45f.py
--rw-rw-r--   0 root         (0) root         (0)     9012 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_record/bulk_get_admin_player_r_e53570.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:35:50.660927 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_tags/
--rw-rw-r--   0 root         (0) root         (0)      660 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_tags/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7087 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_tags/admin_delete_tag_handler_v1.py
--rw-rw-r--   0 root         (0) root         (0)     8329 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_tags/admin_list_tags_handler_v1.py
--rw-rw-r--   0 root         (0) root         (0)     7901 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_tags/admin_post_tag_handler_v1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:35:50.660927 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/concurrent_record/
--rw-rw-r--   0 root         (0) root         (0)      712 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/concurrent_record/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    10363 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/concurrent_record/put_game_record_concurr_33e39a.py
--rw-rw-r--   0 root         (0) root         (0)    12676 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/concurrent_record/put_player_public_recor_3f1a7f.py
--rw-rw-r--   0 root         (0) root         (0)    12663 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/concurrent_record/put_player_record_concu_385e05.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:35:50.660927 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/plugin_config/
--rw-rw-r--   0 root         (0) root         (0)      677 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/plugin_config/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8027 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/plugin_config/create_plugin_config.py
--rw-rw-r--   0 root         (0) root         (0)     6447 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/plugin_config/delete_plugin_config.py
--rw-rw-r--   0 root         (0) root         (0)     6569 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/plugin_config/get_plugin_config.py
--rw-rw-r--   0 root         (0) root         (0)     7989 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/plugin_config/update_plugin_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:35:50.664927 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_game_binary_record/
--rw-rw-r--   0 root         (0) root         (0)      931 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_game_binary_record/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8048 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_game_binary_record/bulk_get_game_binary_record_v1.py
--rw-rw-r--   0 root         (0) root         (0)     7471 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_game_binary_record/delete_game_binary_record_v1.py
--rw-rw-r--   0 root         (0) root         (0)     7334 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_game_binary_record/get_game_binary_record_v1.py
--rw-rw-r--   0 root         (0) root         (0)     9196 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_game_binary_record/list_game_binary_records_v1.py
--rw-rw-r--   0 root         (0) root         (0)     9182 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_game_binary_record/post_game_binary_presig_1e4e53.py
--rw-rw-r--   0 root         (0) root         (0)     8669 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_game_binary_record/post_game_binary_record_v1.py
--rw-rw-r--   0 root         (0) root         (0)     8813 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_game_binary_record/put_game_binary_record_v1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:35:50.664927 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_game_record/
--rw-rw-r--   0 root         (0) root         (0)      785 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_game_record/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7230 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_game_record/delete_game_record_handler_v1.py
--rw-rw-r--   0 root         (0) root         (0)     7619 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_game_record/get_game_record_handler_v1.py
--rw-rw-r--   0 root         (0) root         (0)     8271 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_game_record/get_game_records_bulk.py
--rw-rw-r--   0 root         (0) root         (0)     9948 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_game_record/post_game_record_handler_v1.py
--rw-rw-r--   0 root         (0) root         (0)     9778 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_game_record/put_game_record_handler_v1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:35:50.664927 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_binary_record/
--rw-rw-r--   0 root         (0) root         (0)     1335 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_binary_record/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8188 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_binary_record/bulk_get_my_binary_record_v1.py
--rw-rw-r--   0 root         (0) root         (0)     9024 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_binary_record/bulk_get_other_player_p_6c2093.py
--rw-rw-r--   0 root         (0) root         (0)     8797 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_binary_record/bulk_get_player_public__6635d7.py
--rw-rw-r--   0 root         (0) root         (0)     8317 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_binary_record/delete_player_binary_record_v1.py
--rw-rw-r--   0 root         (0) root         (0)     8204 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_binary_record/get_player_binary_record_v1.py
--rw-rw-r--   0 root         (0) root         (0)     8267 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_binary_record/get_player_public_binar_e2a2d6.py
--rw-rw-r--   0 root         (0) root         (0)     9335 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_binary_record/list_my_binary_records_v1.py
--rw-rw-r--   0 root         (0) root         (0)     9386 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_binary_record/list_other_player_publi_a9eef5.py
--rw-rw-r--   0 root         (0) root         (0)    10030 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_binary_record/post_player_binary_pres_38c5b5.py
--rw-rw-r--   0 root         (0) root         (0)     9493 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_binary_record/post_player_binary_record_v1.py
--rw-rw-r--   0 root         (0) root         (0)     9962 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_binary_record/put_player_binary_recor_012bcd.py
--rw-rw-r--   0 root         (0) root         (0)     9650 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_binary_record/put_player_binary_record_v1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:35:50.664927 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_record/
--rw-rw-r--   0 root         (0) root         (0)     1431 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_record/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8844 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_record/bulk_get_player_public__28e43c.py
--rw-rw-r--   0 root         (0) root         (0)     8151 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_record/delete_player_record_ha_3addde.py
--rw-rw-r--   0 root         (0) root         (0)     9150 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_record/get_other_player_public_17685a.py
--rw-rw-r--   0 root         (0) root         (0)     9373 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_record/get_other_player_public_4438d8.py
--rw-rw-r--   0 root         (0) root         (0)     8599 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_record/get_player_public_recor_5ea27d.py
--rw-rw-r--   0 root         (0) root         (0)     8620 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_record/get_player_record_handler_v1.py
--rw-rw-r--   0 root         (0) root         (0)     8266 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_record/get_player_records_bulk_b10df3.py
--rw-rw-r--   0 root         (0) root         (0)    11178 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_record/post_player_public_reco_b8589e.py
--rw-rw-r--   0 root         (0) root         (0)    11211 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_record/post_player_record_handler_v1.py
--rw-rw-r--   0 root         (0) root         (0)     8053 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_record/public_delete_player_pu_0cc8b5.py
--rw-rw-r--   0 root         (0) root         (0)    11007 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_record/put_player_public_recor_7928cf.py
--rw-rw-r--   0 root         (0) root         (0)    10981 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_record/put_player_record_handler_v1.py
--rw-rw-r--   0 root         (0) root         (0)     8444 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_record/retrieve_player_records.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:35:50.664927 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_tags/
--rw-rw-r--   0 root         (0) root         (0)      536 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_tags/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8325 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_tags/public_list_tags_handler_v1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:35:50.664927 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/ttl_config/
--rw-rw-r--   0 root         (0) root         (0)      616 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/ttl_config/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7550 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/ttl_config/delete_game_binary_reco_40da6b.py
--rw-rw-r--   0 root         (0) root         (0)     7484 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/ttl_config/delete_game_record_ttl_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:35:50.668927 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/wrappers/
--rw-rw-r--   0 root         (0) root         (0)    15113 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/wrappers/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    39009 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/wrappers/_admin_concurrent_record.py
--rw-rw-r--   0 root         (0) root         (0)    26098 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/wrappers/_admin_game_binary_record.py
--rw-rw-r--   0 root         (0) root         (0)    24966 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/wrappers/_admin_game_record.py
--rw-rw-r--   0 root         (0) root         (0)    27381 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/wrappers/_admin_player_binary_record.py
--rw-rw-r--   0 root         (0) root         (0)    62541 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/wrappers/_admin_player_record.py
--rw-rw-r--   0 root         (0) root         (0)    51461 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/wrappers/_admin_record.py
--rw-rw-r--   0 root         (0) root         (0)    10177 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/wrappers/_admin_tags.py
--rw-rw-r--   0 root         (0) root         (0)    21281 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/wrappers/_concurrent_record.py
--rw-rw-r--   0 root         (0) root         (0)    12891 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/wrappers/_plugin_config.py
--rw-rw-r--   0 root         (0) root         (0)    25439 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/wrappers/_public_game_binary_record.py
--rw-rw-r--   0 root         (0) root         (0)    21558 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/wrappers/_public_game_record.py
--rw-rw-r--   0 root         (0) root         (0)    45174 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/wrappers/_public_player_binary_record.py
--rw-rw-r--   0 root         (0) root         (0)    60142 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/wrappers/_public_player_record.py
--rw-rw-r--   0 root         (0) root         (0)     4289 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/wrappers/_public_tags.py
--rw-rw-r--   0 root         (0) root         (0)     7488 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/wrappers/_ttl_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:35:50.668927 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk_service_cloudsave.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1133 2024-02-27 05:35:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk_service_cloudsave.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    17227 2024-02-27 05:35:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk_service_cloudsave.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-27 05:35:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk_service_cloudsave.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       22 2024-02-27 05:35:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk_service_cloudsave.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-02-27 05:35:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk_service_cloudsave.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)      363 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-cloudsave-0.8.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-27 05:35:50.668927 accelbyte-py-sdk-service-cloudsave-0.8.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:10:32.949134 accelbyte-py-sdk-service-cloudsave-0.9.0/
+-rw-r--r--   0 root         (0) root         (0)     1133 2024-03-13 06:10:32.949134 accelbyte-py-sdk-service-cloudsave-0.9.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      877 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:10:32.929134 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:10:32.929134 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:10:32.929134 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/
+-rw-rw-r--   0 root         (0) root         (0)    13106 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:10:32.937134 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/
+-rw-rw-r--   0 root         (0) root         (0)     7753 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7477 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_admin_concurrent_record_request.py
+-rw-rw-r--   0 root         (0) root         (0)     5477 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_admin_game_concurrent_record_request.py
+-rw-rw-r--   0 root         (0) root         (0)     3907 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_admin_game_record_request.py
+-rw-rw-r--   0 root         (0) root         (0)     7299 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_admin_game_record_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5503 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_admin_player_concurrent_record_request.py
+-rw-rw-r--   0 root         (0) root         (0)     4434 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_admin_player_record_key_info.py
+-rw-rw-r--   0 root         (0) root         (0)     3927 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_admin_player_record_request.py
+-rw-rw-r--   0 root         (0) root         (0)     7975 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_admin_player_record_response.py
+-rw-rw-r--   0 root         (0) root         (0)     3692 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_app_config.py
+-rw-rw-r--   0 root         (0) root         (0)     7335 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_binary_info_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4686 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_binary_record_request.py
+-rw-rw-r--   0 root         (0) root         (0)     3929 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_bulk_get_admin_game_record_request.py
+-rw-rw-r--   0 root         (0) root         (0)     4376 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_bulk_get_admin_game_record_response.py
+-rw-rw-r--   0 root         (0) root         (0)     3951 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_bulk_get_admin_player_record_request.py
+-rw-rw-r--   0 root         (0) root         (0)     4412 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_bulk_get_admin_player_record_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4394 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_bulk_get_game_binary_record_response.py
+-rw-rw-r--   0 root         (0) root         (0)     3873 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_bulk_get_game_record_request.py
+-rw-rw-r--   0 root         (0) root         (0)     4284 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_bulk_get_game_record_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4439 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_bulk_get_player_binary_record_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4320 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_bulk_get_player_record_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4394 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_bulk_get_player_record_size_response.py
+-rw-rw-r--   0 root         (0) root         (0)     3906 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_bulk_get_player_records_request.py
+-rw-rw-r--   0 root         (0) root         (0)     4817 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_bulk_update_player_record_by_key_request_detail.py
+-rw-rw-r--   0 root         (0) root         (0)     5420 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_bulk_update_player_record_by_key_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4661 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_bulk_update_player_record_request_detail.py
+-rw-rw-r--   0 root         (0) root         (0)     5273 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_bulk_update_player_record_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4564 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_bulk_update_player_records_by_key_request.py
+-rw-rw-r--   0 root         (0) root         (0)     4470 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_bulk_update_player_records_request.py
+-rw-rw-r--   0 root         (0) root         (0)     3879 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_bulk_user_i_ds_request.py
+-rw-rw-r--   0 root         (0) root         (0)     4126 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_bulk_user_key_request.py
+-rw-rw-r--   0 root         (0) root         (0)     4632 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_concurrent_record_request.py
+-rw-rw-r--   0 root         (0) root         (0)     3819 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_custom_config.py
+-rw-rw-r--   0 root         (0) root         (0)    19080 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_custom_function.py
+-rw-rw-r--   0 root         (0) root         (0)     9969 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_game_binary_record_admin_response.py
+-rw-rw-r--   0 root         (0) root         (0)     6529 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_game_binary_record_create.py
+-rw-rw-r--   0 root         (0) root         (0)     6105 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_game_binary_record_metadata_request.py
+-rw-rw-r--   0 root         (0) root         (0)     8135 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_game_binary_record_response.py
+-rw-rw-r--   0 root         (0) root         (0)     9409 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_game_record_admin_response.py
+-rw-rw-r--   0 root         (0) root         (0)     3842 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_game_record_request.py
+-rw-rw-r--   0 root         (0) root         (0)     8254 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_game_record_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4863 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_list_admin_game_record_keys_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5341 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_list_admin_player_record_keys_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5397 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_list_game_binary_records_admin_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5291 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_list_game_binary_records_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4788 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_list_game_record_keys_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5338 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_list_player_binary_records_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5219 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_list_player_record_keys_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4921 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_list_tags_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5438 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_pagination.py
+-rw-rw-r--   0 root         (0) root         (0)     6266 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_player_binary_record_create.py
+-rw-rw-r--   0 root         (0) root         (0)     4181 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_player_binary_record_metadata_public_request.py
+-rw-rw-r--   0 root         (0) root         (0)     5879 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_player_binary_record_metadata_request.py
+-rw-rw-r--   0 root         (0) root         (0)    10199 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_player_binary_record_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4085 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_player_record_concurrent_update_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4373 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_player_record_key_info.py
+-rw-rw-r--   0 root         (0) root         (0)     3876 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_player_record_request.py
+-rw-rw-r--   0 root         (0) root         (0)     9618 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_player_record_response.py
+-rw-rw-r--   0 root         (0) root         (0)     6677 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_player_record_size_response.py
+-rw-rw-r--   0 root         (0) root         (0)     7472 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_plugin_request.py
+-rw-rw-r--   0 root         (0) root         (0)     8176 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_plugin_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4536 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_public_game_binary_record_create.py
+-rw-rw-r--   0 root         (0) root         (0)     5309 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_public_player_binary_record_create.py
+-rw-rw-r--   0 root         (0) root         (0)     4538 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_response_error.py
+-rw-rw-r--   0 root         (0) root         (0)     4256 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_tag_info.py
+-rw-rw-r--   0 root         (0) root         (0)     3611 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_tag_request.py
+-rw-rw-r--   0 root         (0) root         (0)     4746 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_ttl_config_dto.py
+-rw-rw-r--   0 root         (0) root         (0)     3929 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_upload_binary_record_request.py
+-rw-rw-r--   0 root         (0) root         (0)     5963 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_upload_binary_record_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4386 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_user_key_request.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:10:32.937134 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/
+-rw-rw-r--   0 root         (0) root         (0)      438 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:10:32.937134 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_concurrent_record/
+-rw-rw-r--   0 root         (0) root         (0)      912 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_concurrent_record/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    10830 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_concurrent_record/admin_put_admin_game_re_99ac43.py
+-rw-rw-r--   0 root         (0) root         (0)    13068 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_concurrent_record/admin_put_admin_player__e84e5d.py
+-rw-rw-r--   0 root         (0) root         (0)    11141 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_concurrent_record/admin_put_game_record_c_886b02.py
+-rw-rw-r--   0 root         (0) root         (0)    13446 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_concurrent_record/admin_put_player_public_1624a9.py
+-rw-rw-r--   0 root         (0) root         (0)    13417 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_concurrent_record/admin_put_player_record_233704.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:10:32.937134 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_game_binary_record/
+-rw-rw-r--   0 root         (0) root         (0)      988 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_game_binary_record/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7474 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_game_binary_record/admin_delete_game_binar_3752d7.py
+-rw-rw-r--   0 root         (0) root         (0)     7400 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_game_binary_record/admin_get_game_binary_r_5df25c.py
+-rw-rw-r--   0 root         (0) root         (0)     9321 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_game_binary_record/admin_list_game_binary__f439a9.py
+-rw-rw-r--   0 root         (0) root         (0)     8662 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_game_binary_record/admin_post_game_binary__ace069.py
+-rw-rw-r--   0 root         (0) root         (0)     9228 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_game_binary_record/admin_post_game_binary__ce9dc6.py
+-rw-rw-r--   0 root         (0) root         (0)     8884 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_game_binary_record/admin_put_game_binary_r_47597f.py
+-rw-rw-r--   0 root         (0) root         (0)     8978 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_game_binary_record/admin_put_game_binary_r_a490ed.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:10:32.937134 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_game_record/
+-rw-rw-r--   0 root         (0) root         (0)      830 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_game_record/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7312 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_game_record/admin_delete_game_recor_636983.py
+-rw-rw-r--   0 root         (0) root         (0)     7434 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_game_record/admin_get_game_record_h_f6ed3a.py
+-rw-rw-r--   0 root         (0) root         (0)    10931 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_game_record/admin_post_game_record__9a2084.py
+-rw-rw-r--   0 root         (0) root         (0)    10723 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_game_record/admin_put_game_record_h_0dd624.py
+-rw-rw-r--   0 root         (0) root         (0)     9120 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_game_record/list_game_records_handler_v1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:10:32.937134 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_binary_record/
+-rw-rw-r--   0 root         (0) root         (0)     1002 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_binary_record/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8019 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_binary_record/admin_delete_player_bin_892eb5.py
+-rw-rw-r--   0 root         (0) root         (0)     8194 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_binary_record/admin_get_player_binary_1076b9.py
+-rw-rw-r--   0 root         (0) root         (0)    10079 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_binary_record/admin_list_player_binar_e452ce.py
+-rw-rw-r--   0 root         (0) root         (0)     9491 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_binary_record/admin_post_player_binar_e33f40.py
+-rw-rw-r--   0 root         (0) root         (0)     9941 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_binary_record/admin_post_player_binar_f1a4e9.py
+-rw-rw-r--   0 root         (0) root         (0)     9607 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_binary_record/admin_put_player_binary_6424e4.py
+-rw-rw-r--   0 root         (0) root         (0)     9785 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_binary_record/admin_put_player_binary_bcf941.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:10:32.941134 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_record/
+-rw-rw-r--   0 root         (0) root         (0)     1711 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_record/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8894 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_record/admin_bulk_get_player_r_82c596.py
+-rw-rw-r--   0 root         (0) root         (0)     9370 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_record/admin_bulk_put_player_r_27d5a1.py
+-rw-rw-r--   0 root         (0) root         (0)     8855 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_record/admin_delete_player_pub_f11fd7.py
+-rw-rw-r--   0 root         (0) root         (0)     7781 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_record/admin_delete_player_rec_168241.py
+-rw-rw-r--   0 root         (0) root         (0)     8287 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_record/admin_get_player_public_f015b6.py
+-rw-rw-r--   0 root         (0) root         (0)     8244 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_record/admin_get_player_record_b37faa.py
+-rw-rw-r--   0 root         (0) root         (0)     8212 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_record/admin_get_player_record_d622c9.py
+-rw-rw-r--   0 root         (0) root         (0)     9310 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_record/admin_get_player_record_f4a5eb.py
+-rw-rw-r--   0 root         (0) root         (0)    10910 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_record/admin_post_player_publi_98e39e.py
+-rw-rw-r--   0 root         (0) root         (0)    11381 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_record/admin_post_player_recor_6a96c8.py
+-rw-rw-r--   0 root         (0) root         (0)    10765 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_record/admin_put_player_public_819faf.py
+-rw-rw-r--   0 root         (0) root         (0)     8993 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_record/admin_put_player_record_253e92.py
+-rw-rw-r--   0 root         (0) root         (0)    11210 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_record/admin_put_player_record_a8195d.py
+-rw-rw-r--   0 root         (0) root         (0)     9256 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_record/admin_retrieve_player_records.py
+-rw-rw-r--   0 root         (0) root         (0)     7997 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_record/bulk_get_player_record__4627ec.py
+-rw-rw-r--   0 root         (0) root         (0)     9308 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_record/list_player_record_handler_v1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:10:32.941134 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_record/
+-rw-rw-r--   0 root         (0) root         (0)     1420 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_record/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8383 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_record/admin_bulk_get_admin_ga_c5c529.py
+-rw-rw-r--   0 root         (0) root         (0)     9297 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_record/admin_bulk_get_admin_pl_b8e62a.py
+-rw-rw-r--   0 root         (0) root         (0)     7160 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_record/admin_delete_admin_game_1f080f.py
+-rw-rw-r--   0 root         (0) root         (0)     8016 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_record/admin_delete_admin_play_632fe7.py
+-rw-rw-r--   0 root         (0) root         (0)     7434 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_record/admin_get_admin_game_record_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     8271 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_record/admin_get_admin_player__37ad38.py
+-rw-rw-r--   0 root         (0) root         (0)     9247 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_record/admin_list_admin_game_r_476bfb.py
+-rw-rw-r--   0 root         (0) root         (0)     9359 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_record/admin_list_admin_user_r_83dd7a.py
+-rw-rw-r--   0 root         (0) root         (0)    10409 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_record/admin_post_admin_game_r_e8f678.py
+-rw-rw-r--   0 root         (0) root         (0)    11029 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_record/admin_post_player_admin_b138ee.py
+-rw-rw-r--   0 root         (0) root         (0)    10127 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_record/admin_put_admin_game_record_v1.py
+-rw-rw-r--   0 root         (0) root         (0)    10860 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_record/admin_put_admin_player__6ed45f.py
+-rw-rw-r--   0 root         (0) root         (0)     9012 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_record/bulk_get_admin_player_r_e53570.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:10:32.941134 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_tags/
+-rw-rw-r--   0 root         (0) root         (0)      660 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_tags/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7087 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_tags/admin_delete_tag_handler_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     8329 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_tags/admin_list_tags_handler_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     7901 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_tags/admin_post_tag_handler_v1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:10:32.941134 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/concurrent_record/
+-rw-rw-r--   0 root         (0) root         (0)      712 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/concurrent_record/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    10363 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/concurrent_record/put_game_record_concurr_33e39a.py
+-rw-rw-r--   0 root         (0) root         (0)    12676 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/concurrent_record/put_player_public_recor_3f1a7f.py
+-rw-rw-r--   0 root         (0) root         (0)    12663 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/concurrent_record/put_player_record_concu_385e05.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:10:32.941134 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/plugin_config/
+-rw-rw-r--   0 root         (0) root         (0)      677 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/plugin_config/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8027 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/plugin_config/create_plugin_config.py
+-rw-rw-r--   0 root         (0) root         (0)     6447 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/plugin_config/delete_plugin_config.py
+-rw-rw-r--   0 root         (0) root         (0)     6569 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/plugin_config/get_plugin_config.py
+-rw-rw-r--   0 root         (0) root         (0)     7989 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/plugin_config/update_plugin_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:10:32.941134 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_game_binary_record/
+-rw-rw-r--   0 root         (0) root         (0)      931 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_game_binary_record/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8048 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_game_binary_record/bulk_get_game_binary_record_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     7471 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_game_binary_record/delete_game_binary_record_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     7334 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_game_binary_record/get_game_binary_record_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     9196 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_game_binary_record/list_game_binary_records_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     9182 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_game_binary_record/post_game_binary_presig_1e4e53.py
+-rw-rw-r--   0 root         (0) root         (0)     8669 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_game_binary_record/post_game_binary_record_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     8813 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_game_binary_record/put_game_binary_record_v1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:10:32.941134 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_game_record/
+-rw-rw-r--   0 root         (0) root         (0)      785 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_game_record/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7230 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_game_record/delete_game_record_handler_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     7619 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_game_record/get_game_record_handler_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     8271 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_game_record/get_game_records_bulk.py
+-rw-rw-r--   0 root         (0) root         (0)     9948 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_game_record/post_game_record_handler_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     9778 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_game_record/put_game_record_handler_v1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:10:32.945134 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_binary_record/
+-rw-rw-r--   0 root         (0) root         (0)     1335 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_binary_record/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8188 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_binary_record/bulk_get_my_binary_record_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     9024 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_binary_record/bulk_get_other_player_p_6c2093.py
+-rw-rw-r--   0 root         (0) root         (0)     8797 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_binary_record/bulk_get_player_public__6635d7.py
+-rw-rw-r--   0 root         (0) root         (0)     8317 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_binary_record/delete_player_binary_record_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     8204 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_binary_record/get_player_binary_record_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     8267 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_binary_record/get_player_public_binar_e2a2d6.py
+-rw-rw-r--   0 root         (0) root         (0)     9335 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_binary_record/list_my_binary_records_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     9386 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_binary_record/list_other_player_publi_a9eef5.py
+-rw-rw-r--   0 root         (0) root         (0)    10030 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_binary_record/post_player_binary_pres_38c5b5.py
+-rw-rw-r--   0 root         (0) root         (0)     9493 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_binary_record/post_player_binary_record_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     9962 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_binary_record/put_player_binary_recor_012bcd.py
+-rw-rw-r--   0 root         (0) root         (0)     9650 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_binary_record/put_player_binary_record_v1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:10:32.945134 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_record/
+-rw-rw-r--   0 root         (0) root         (0)     1431 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_record/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8844 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_record/bulk_get_player_public__28e43c.py
+-rw-rw-r--   0 root         (0) root         (0)     8151 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_record/delete_player_record_ha_3addde.py
+-rw-rw-r--   0 root         (0) root         (0)     9150 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_record/get_other_player_public_17685a.py
+-rw-rw-r--   0 root         (0) root         (0)     9373 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_record/get_other_player_public_4438d8.py
+-rw-rw-r--   0 root         (0) root         (0)     8599 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_record/get_player_public_recor_5ea27d.py
+-rw-rw-r--   0 root         (0) root         (0)     8620 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_record/get_player_record_handler_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     8266 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_record/get_player_records_bulk_b10df3.py
+-rw-rw-r--   0 root         (0) root         (0)    11178 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_record/post_player_public_reco_b8589e.py
+-rw-rw-r--   0 root         (0) root         (0)    11211 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_record/post_player_record_handler_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     8053 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_record/public_delete_player_pu_0cc8b5.py
+-rw-rw-r--   0 root         (0) root         (0)    11007 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_record/put_player_public_recor_7928cf.py
+-rw-rw-r--   0 root         (0) root         (0)    10981 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_record/put_player_record_handler_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     8444 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_record/retrieve_player_records.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:10:32.945134 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_tags/
+-rw-rw-r--   0 root         (0) root         (0)      536 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_tags/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8325 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_tags/public_list_tags_handler_v1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:10:32.945134 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/ttl_config/
+-rw-rw-r--   0 root         (0) root         (0)      616 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/ttl_config/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7550 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/ttl_config/delete_game_binary_reco_40da6b.py
+-rw-rw-r--   0 root         (0) root         (0)     7484 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/ttl_config/delete_game_record_ttl_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:10:32.949134 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/wrappers/
+-rw-rw-r--   0 root         (0) root         (0)    15474 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/wrappers/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    40373 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/wrappers/_admin_concurrent_record.py
+-rw-rw-r--   0 root         (0) root         (0)    26098 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/wrappers/_admin_game_binary_record.py
+-rw-rw-r--   0 root         (0) root         (0)    25510 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/wrappers/_admin_game_record.py
+-rw-rw-r--   0 root         (0) root         (0)    27381 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/wrappers/_admin_player_binary_record.py
+-rw-rw-r--   0 root         (0) root         (0)    70918 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/wrappers/_admin_player_record.py
+-rw-rw-r--   0 root         (0) root         (0)    56477 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/wrappers/_admin_record.py
+-rw-rw-r--   0 root         (0) root         (0)    10177 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/wrappers/_admin_tags.py
+-rw-rw-r--   0 root         (0) root         (0)    21281 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/wrappers/_concurrent_record.py
+-rw-rw-r--   0 root         (0) root         (0)    12891 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/wrappers/_plugin_config.py
+-rw-rw-r--   0 root         (0) root         (0)    25439 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/wrappers/_public_game_binary_record.py
+-rw-rw-r--   0 root         (0) root         (0)    21558 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/wrappers/_public_game_record.py
+-rw-rw-r--   0 root         (0) root         (0)    45174 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/wrappers/_public_player_binary_record.py
+-rw-rw-r--   0 root         (0) root         (0)    60142 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/wrappers/_public_player_record.py
+-rw-rw-r--   0 root         (0) root         (0)     4289 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/wrappers/_public_tags.py
+-rw-rw-r--   0 root         (0) root         (0)     7488 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/wrappers/_ttl_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:10:32.949134 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk_service_cloudsave.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1133 2024-03-13 06:10:32.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk_service_cloudsave.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    17695 2024-03-13 06:10:32.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk_service_cloudsave.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-03-13 06:10:32.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk_service_cloudsave.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-03-13 06:10:32.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk_service_cloudsave.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-03-13 06:10:32.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk_service_cloudsave.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)      363 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-cloudsave-0.9.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-03-13 06:10:32.949134 accelbyte-py-sdk-service-cloudsave-0.9.0/setup.cfg
```

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/PKG-INFO` & `accelbyte-py-sdk-service-cloudsave-0.9.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: accelbyte-py-sdk-service-cloudsave
-Version: 0.8.0
+Version: 0.9.0
 Summary: AccelByte Python SDK - AccelByte Gaming Services Cloudsave Service
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: accelbyte-py-sdk-core
 
 [//]: # (Code generated. DO NOT EDIT!)
 
 # AccelByte Modular Python SDK - Service Module
 
 This is a service module for the [AccelByte Modular Python SDK](https://github.com/AccelByte/accelbyte-python-modular-sdk) package.
 
 ```text
 AccelByte Gaming Services Cloudsave Service
-* Version: 3.15.1
+* Version: 3.16.0
 ```
 
 ## Setup
 
 This SDK requires Python 3.9 to be installed.
 
 ### Install with Pip
```

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/README.md` & `accelbyte-py-sdk-service-cloudsave-0.9.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # AccelByte Modular Python SDK - Service Module
 
 This is a service module for the [AccelByte Modular Python SDK](https://github.com/AccelByte/accelbyte-python-modular-sdk) package.
 
 ```text
 AccelByte Gaming Services Cloudsave Service
-* Version: 3.15.1
+* Version: 3.16.0
 ```
 
 ## Setup
 
 This SDK requires Python 3.9 to be installed.
 
 ### Install with Pip
```

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/__init__.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: service-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Cloudsave Service."""
 
-__version__ = "3.15.1"
+__version__ = "3.16.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 # admin_concurrent_record
 from .wrappers import admin_put_admin_game_record_concurrent_handler_v1
@@ -67,14 +67,18 @@
 from .wrappers import admin_post_player_binary_record_v1_async
 from .wrappers import admin_put_player_binary_record_v1
 from .wrappers import admin_put_player_binary_record_v1_async
 from .wrappers import admin_put_player_binary_recor_metadata_v1
 from .wrappers import admin_put_player_binary_recor_metadata_v1_async
 
 # admin_player_record
+from .wrappers import admin_bulk_get_player_records_by_user_i_ds_handler_v1
+from .wrappers import admin_bulk_get_player_records_by_user_i_ds_handler_v1_async
+from .wrappers import admin_bulk_put_player_records_by_key_handler_v1
+from .wrappers import admin_bulk_put_player_records_by_key_handler_v1_async
 from .wrappers import admin_delete_player_public_record_handler_v1
 from .wrappers import admin_delete_player_public_record_handler_v1_async
 from .wrappers import admin_delete_player_record_handler_v1
 from .wrappers import admin_delete_player_record_handler_v1_async
 from .wrappers import admin_get_player_public_record_handler_v1
 from .wrappers import admin_get_player_public_record_handler_v1_async
 from .wrappers import admin_get_player_record_handler_v1
```

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/__init__.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: model-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Cloudsave Service."""
 
-__version__ = "3.15.1"
+__version__ = "3.16.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .models_admin_concurrent_record_request import ModelsAdminConcurrentRecordRequest
 from .models_admin_concurrent_record_request import (
@@ -53,20 +53,29 @@
     ModelsBulkGetPlayerBinaryRecordResponse,
 )
 from .models_bulk_get_player_record_response import ModelsBulkGetPlayerRecordResponse
 from .models_bulk_get_player_record_size_response import (
     ModelsBulkGetPlayerRecordSizeResponse,
 )
 from .models_bulk_get_player_records_request import ModelsBulkGetPlayerRecordsRequest
+from .models_bulk_update_player_record_by_key_request_detail import (
+    ModelsBulkUpdatePlayerRecordByKeyRequestDetail,
+)
+from .models_bulk_update_player_record_by_key_response import (
+    ModelsBulkUpdatePlayerRecordByKeyResponse,
+)
 from .models_bulk_update_player_record_request_detail import (
     ModelsBulkUpdatePlayerRecordRequestDetail,
 )
 from .models_bulk_update_player_record_response import (
     ModelsBulkUpdatePlayerRecordResponse,
 )
+from .models_bulk_update_player_records_by_key_request import (
+    ModelsBulkUpdatePlayerRecordsByKeyRequest,
+)
 from .models_bulk_update_player_records_request import (
     ModelsBulkUpdatePlayerRecordsRequest,
 )
 from .models_bulk_user_i_ds_request import ModelsBulkUserIDsRequest
 from .models_bulk_user_key_request import ModelsBulkUserKeyRequest
 from .models_concurrent_record_request import ModelsConcurrentRecordRequest
 from .models_custom_config import ModelsCustomConfig
```

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_admin_concurrent_record_request.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_game_binary_record_create.py`

 * *Files 15% similar despite different names*

```diff
@@ -32,183 +32,181 @@
 
 
 class SetByEnum(StrEnum):
     CLIENT = "CLIENT"
     SERVER = "SERVER"
 
 
-class ModelsAdminConcurrentRecordRequest(Model):
-    """Models admin concurrent record request (models.AdminConcurrentRecordRequest)
+class ModelsGameBinaryRecordCreate(Model):
+    """Models game binary record create (models.GameBinaryRecordCreate)
 
     Properties:
-        set_by: (set_by) REQUIRED Union[str, SetByEnum]
+        file_type: (file_type) REQUIRED str
 
-        updated_at: (updatedAt) REQUIRED str
+        key: (key) REQUIRED str
 
-        value: (value) REQUIRED Dict[str, Any]
+        set_by: (set_by) REQUIRED Union[str, SetByEnum]
 
         ttl_config: (ttl_config) OPTIONAL ModelsTTLConfigDTO
     """
 
     # region fields
 
+    file_type: str  # REQUIRED
+    key: str  # REQUIRED
     set_by: Union[str, SetByEnum]  # REQUIRED
-    updated_at: str  # REQUIRED
-    value: Dict[str, Any]  # REQUIRED
     ttl_config: ModelsTTLConfigDTO  # OPTIONAL
 
     # endregion fields
 
     # region with_x methods
 
-    def with_set_by(
-        self, value: Union[str, SetByEnum]
-    ) -> ModelsAdminConcurrentRecordRequest:
-        self.set_by = value
+    def with_file_type(self, value: str) -> ModelsGameBinaryRecordCreate:
+        self.file_type = value
         return self
 
-    def with_updated_at(self, value: str) -> ModelsAdminConcurrentRecordRequest:
-        self.updated_at = value
+    def with_key(self, value: str) -> ModelsGameBinaryRecordCreate:
+        self.key = value
         return self
 
-    def with_value(self, value: Dict[str, Any]) -> ModelsAdminConcurrentRecordRequest:
-        self.value = value
+    def with_set_by(self, value: Union[str, SetByEnum]) -> ModelsGameBinaryRecordCreate:
+        self.set_by = value
         return self
 
     def with_ttl_config(
         self, value: ModelsTTLConfigDTO
-    ) -> ModelsAdminConcurrentRecordRequest:
+    ) -> ModelsGameBinaryRecordCreate:
         self.ttl_config = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
+        if hasattr(self, "file_type"):
+            result["file_type"] = str(self.file_type)
+        elif include_empty:
+            result["file_type"] = ""
+        if hasattr(self, "key"):
+            result["key"] = str(self.key)
+        elif include_empty:
+            result["key"] = ""
         if hasattr(self, "set_by"):
             result["set_by"] = str(self.set_by)
         elif include_empty:
             result["set_by"] = Union[str, SetByEnum]()
-        if hasattr(self, "updated_at"):
-            result["updatedAt"] = str(self.updated_at)
-        elif include_empty:
-            result["updatedAt"] = ""
-        if hasattr(self, "value"):
-            result["value"] = {str(k0): v0 for k0, v0 in self.value.items()}
-        elif include_empty:
-            result["value"] = {}
         if hasattr(self, "ttl_config"):
             result["ttl_config"] = self.ttl_config.to_dict(include_empty=include_empty)
         elif include_empty:
             result["ttl_config"] = ModelsTTLConfigDTO()
         return result
 
     # endregion to methods
 
     # region static methods
 
     @classmethod
     def create(
         cls,
+        file_type: str,
+        key: str,
         set_by: Union[str, SetByEnum],
-        updated_at: str,
-        value: Dict[str, Any],
         ttl_config: Optional[ModelsTTLConfigDTO] = None,
         **kwargs,
-    ) -> ModelsAdminConcurrentRecordRequest:
+    ) -> ModelsGameBinaryRecordCreate:
         instance = cls()
+        instance.file_type = file_type
+        instance.key = key
         instance.set_by = set_by
-        instance.updated_at = updated_at
-        instance.value = value
         if ttl_config is not None:
             instance.ttl_config = ttl_config
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> ModelsAdminConcurrentRecordRequest:
+    ) -> ModelsGameBinaryRecordCreate:
         instance = cls()
         if not dict_:
             return instance
+        if "file_type" in dict_ and dict_["file_type"] is not None:
+            instance.file_type = str(dict_["file_type"])
+        elif include_empty:
+            instance.file_type = ""
+        if "key" in dict_ and dict_["key"] is not None:
+            instance.key = str(dict_["key"])
+        elif include_empty:
+            instance.key = ""
         if "set_by" in dict_ and dict_["set_by"] is not None:
             instance.set_by = str(dict_["set_by"])
         elif include_empty:
             instance.set_by = Union[str, SetByEnum]()
-        if "updatedAt" in dict_ and dict_["updatedAt"] is not None:
-            instance.updated_at = str(dict_["updatedAt"])
-        elif include_empty:
-            instance.updated_at = ""
-        if "value" in dict_ and dict_["value"] is not None:
-            instance.value = {str(k0): v0 for k0, v0 in dict_["value"].items()}
-        elif include_empty:
-            instance.value = {}
         if "ttl_config" in dict_ and dict_["ttl_config"] is not None:
             instance.ttl_config = ModelsTTLConfigDTO.create_from_dict(
                 dict_["ttl_config"], include_empty=include_empty
             )
         elif include_empty:
             instance.ttl_config = ModelsTTLConfigDTO()
         return instance
 
     @classmethod
     def create_many_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> Dict[str, ModelsAdminConcurrentRecordRequest]:
+    ) -> Dict[str, ModelsGameBinaryRecordCreate]:
         return (
             {k: cls.create_from_dict(v, include_empty=include_empty) for k, v in dict_}
             if dict_
             else {}
         )
 
     @classmethod
     def create_many_from_list(
         cls, list_: list, include_empty: bool = False
-    ) -> List[ModelsAdminConcurrentRecordRequest]:
+    ) -> List[ModelsGameBinaryRecordCreate]:
         return (
             [cls.create_from_dict(i, include_empty=include_empty) for i in list_]
             if list_
             else []
         )
 
     @classmethod
     def create_from_any(
         cls, any_: any, include_empty: bool = False, many: bool = False
     ) -> Union[
-        ModelsAdminConcurrentRecordRequest,
-        List[ModelsAdminConcurrentRecordRequest],
-        Dict[Any, ModelsAdminConcurrentRecordRequest],
+        ModelsGameBinaryRecordCreate,
+        List[ModelsGameBinaryRecordCreate],
+        Dict[Any, ModelsGameBinaryRecordCreate],
     ]:
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
+            "file_type": "file_type",
+            "key": "key",
             "set_by": "set_by",
-            "updatedAt": "updated_at",
-            "value": "value",
             "ttl_config": "ttl_config",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
+            "file_type": True,
+            "key": True,
             "set_by": True,
-            "updatedAt": True,
-            "value": True,
             "ttl_config": False,
         }
 
     @staticmethod
     def get_enum_map() -> Dict[str, List[Any]]:
         return {
             "set_by": ["CLIENT", "SERVER"],
```

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_admin_game_concurrent_record_request.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_concurrent_record_request.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,16 +24,16 @@
 
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Model
 
 
-class ModelsAdminGameConcurrentRecordRequest(Model):
-    """Models admin game concurrent record request (models.AdminGameConcurrentRecordRequest)
+class ModelsConcurrentRecordRequest(Model):
+    """Models concurrent record request (models.ConcurrentRecordRequest)
 
     Properties:
         updated_at: (updatedAt) REQUIRED str
 
         value: (value) REQUIRED Dict[str, Any]
     """
 
@@ -42,21 +42,19 @@
     updated_at: str  # REQUIRED
     value: Dict[str, Any]  # REQUIRED
 
     # endregion fields
 
     # region with_x methods
 
-    def with_updated_at(self, value: str) -> ModelsAdminGameConcurrentRecordRequest:
+    def with_updated_at(self, value: str) -> ModelsConcurrentRecordRequest:
         self.updated_at = value
         return self
 
-    def with_value(
-        self, value: Dict[str, Any]
-    ) -> ModelsAdminGameConcurrentRecordRequest:
+    def with_value(self, value: Dict[str, Any]) -> ModelsConcurrentRecordRequest:
         self.value = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
@@ -75,24 +73,24 @@
     # endregion to methods
 
     # region static methods
 
     @classmethod
     def create(
         cls, updated_at: str, value: Dict[str, Any], **kwargs
-    ) -> ModelsAdminGameConcurrentRecordRequest:
+    ) -> ModelsConcurrentRecordRequest:
         instance = cls()
         instance.updated_at = updated_at
         instance.value = value
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> ModelsAdminGameConcurrentRecordRequest:
+    ) -> ModelsConcurrentRecordRequest:
         instance = cls()
         if not dict_:
             return instance
         if "updatedAt" in dict_ and dict_["updatedAt"] is not None:
             instance.updated_at = str(dict_["updatedAt"])
         elif include_empty:
             instance.updated_at = ""
@@ -101,38 +99,38 @@
         elif include_empty:
             instance.value = {}
         return instance
 
     @classmethod
     def create_many_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> Dict[str, ModelsAdminGameConcurrentRecordRequest]:
+    ) -> Dict[str, ModelsConcurrentRecordRequest]:
         return (
             {k: cls.create_from_dict(v, include_empty=include_empty) for k, v in dict_}
             if dict_
             else {}
         )
 
     @classmethod
     def create_many_from_list(
         cls, list_: list, include_empty: bool = False
-    ) -> List[ModelsAdminGameConcurrentRecordRequest]:
+    ) -> List[ModelsConcurrentRecordRequest]:
         return (
             [cls.create_from_dict(i, include_empty=include_empty) for i in list_]
             if list_
             else []
         )
 
     @classmethod
     def create_from_any(
         cls, any_: any, include_empty: bool = False, many: bool = False
     ) -> Union[
-        ModelsAdminGameConcurrentRecordRequest,
-        List[ModelsAdminGameConcurrentRecordRequest],
-        Dict[Any, ModelsAdminGameConcurrentRecordRequest],
+        ModelsConcurrentRecordRequest,
+        List[ModelsConcurrentRecordRequest],
+        Dict[Any, ModelsConcurrentRecordRequest],
     ]:
         if many:
             if isinstance(any_, dict):
                 return cls.create_many_from_dict(any_, include_empty=include_empty)
             elif isinstance(any_, list):
                 return cls.create_many_from_list(any_, include_empty=include_empty)
             else:
```

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_admin_game_record_request.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_admin_game_record_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_admin_game_record_response.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_admin_game_record_response.py`

 * *Files 11% similar despite different names*

```diff
@@ -37,23 +37,26 @@
         key: (key) REQUIRED str
 
         namespace: (namespace) REQUIRED str
 
         updated_at: (updated_at) REQUIRED str
 
         value: (value) REQUIRED Dict[str, Any]
+
+        tags: (tags) OPTIONAL List[str]
     """
 
     # region fields
 
     created_at: str  # REQUIRED
     key: str  # REQUIRED
     namespace: str  # REQUIRED
     updated_at: str  # REQUIRED
     value: Dict[str, Any]  # REQUIRED
+    tags: List[str]  # OPTIONAL
 
     # endregion fields
 
     # region with_x methods
 
     def with_created_at(self, value: str) -> ModelsAdminGameRecordResponse:
         self.created_at = value
@@ -71,14 +74,18 @@
         self.updated_at = value
         return self
 
     def with_value(self, value: Dict[str, Any]) -> ModelsAdminGameRecordResponse:
         self.value = value
         return self
 
+    def with_tags(self, value: List[str]) -> ModelsAdminGameRecordResponse:
+        self.tags = value
+        return self
+
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
         if hasattr(self, "created_at"):
@@ -97,36 +104,43 @@
             result["updated_at"] = str(self.updated_at)
         elif include_empty:
             result["updated_at"] = ""
         if hasattr(self, "value"):
             result["value"] = {str(k0): v0 for k0, v0 in self.value.items()}
         elif include_empty:
             result["value"] = {}
+        if hasattr(self, "tags"):
+            result["tags"] = [str(i0) for i0 in self.tags]
+        elif include_empty:
+            result["tags"] = []
         return result
 
     # endregion to methods
 
     # region static methods
 
     @classmethod
     def create(
         cls,
         created_at: str,
         key: str,
         namespace: str,
         updated_at: str,
         value: Dict[str, Any],
+        tags: Optional[List[str]] = None,
         **kwargs,
     ) -> ModelsAdminGameRecordResponse:
         instance = cls()
         instance.created_at = created_at
         instance.key = key
         instance.namespace = namespace
         instance.updated_at = updated_at
         instance.value = value
+        if tags is not None:
+            instance.tags = tags
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
     ) -> ModelsAdminGameRecordResponse:
         instance = cls()
@@ -148,14 +162,18 @@
             instance.updated_at = str(dict_["updated_at"])
         elif include_empty:
             instance.updated_at = ""
         if "value" in dict_ and dict_["value"] is not None:
             instance.value = {str(k0): v0 for k0, v0 in dict_["value"].items()}
         elif include_empty:
             instance.value = {}
+        if "tags" in dict_ and dict_["tags"] is not None:
+            instance.tags = [str(i0) for i0 in dict_["tags"]]
+        elif include_empty:
+            instance.tags = []
         return instance
 
     @classmethod
     def create_many_from_dict(
         cls, dict_: dict, include_empty: bool = False
     ) -> Dict[str, ModelsAdminGameRecordResponse]:
         return (
@@ -196,20 +214,22 @@
     def get_field_info() -> Dict[str, str]:
         return {
             "created_at": "created_at",
             "key": "key",
             "namespace": "namespace",
             "updated_at": "updated_at",
             "value": "value",
+            "tags": "tags",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
             "created_at": True,
             "key": True,
             "namespace": True,
             "updated_at": True,
             "value": True,
+            "tags": False,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_admin_player_concurrent_record_request.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_admin_player_concurrent_record_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,20 +31,23 @@
 class ModelsAdminPlayerConcurrentRecordRequest(Model):
     """Models admin player concurrent record request (models.AdminPlayerConcurrentRecordRequest)
 
     Properties:
         updated_at: (updatedAt) REQUIRED str
 
         value: (value) REQUIRED Dict[str, Any]
+
+        tags: (tags) OPTIONAL List[str]
     """
 
     # region fields
 
     updated_at: str  # REQUIRED
     value: Dict[str, Any]  # REQUIRED
+    tags: List[str]  # OPTIONAL
 
     # endregion fields
 
     # region with_x methods
 
     def with_updated_at(self, value: str) -> ModelsAdminPlayerConcurrentRecordRequest:
         self.updated_at = value
@@ -52,41 +55,55 @@
 
     def with_value(
         self, value: Dict[str, Any]
     ) -> ModelsAdminPlayerConcurrentRecordRequest:
         self.value = value
         return self
 
+    def with_tags(self, value: List[str]) -> ModelsAdminPlayerConcurrentRecordRequest:
+        self.tags = value
+        return self
+
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
         if hasattr(self, "updated_at"):
             result["updatedAt"] = str(self.updated_at)
         elif include_empty:
             result["updatedAt"] = ""
         if hasattr(self, "value"):
             result["value"] = {str(k0): v0 for k0, v0 in self.value.items()}
         elif include_empty:
             result["value"] = {}
+        if hasattr(self, "tags"):
+            result["tags"] = [str(i0) for i0 in self.tags]
+        elif include_empty:
+            result["tags"] = []
         return result
 
     # endregion to methods
 
     # region static methods
 
     @classmethod
     def create(
-        cls, updated_at: str, value: Dict[str, Any], **kwargs
+        cls,
+        updated_at: str,
+        value: Dict[str, Any],
+        tags: Optional[List[str]] = None,
+        **kwargs,
     ) -> ModelsAdminPlayerConcurrentRecordRequest:
         instance = cls()
         instance.updated_at = updated_at
         instance.value = value
+        if tags is not None:
+            instance.tags = tags
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
     ) -> ModelsAdminPlayerConcurrentRecordRequest:
         instance = cls()
@@ -96,14 +113,18 @@
             instance.updated_at = str(dict_["updatedAt"])
         elif include_empty:
             instance.updated_at = ""
         if "value" in dict_ and dict_["value"] is not None:
             instance.value = {str(k0): v0 for k0, v0 in dict_["value"].items()}
         elif include_empty:
             instance.value = {}
+        if "tags" in dict_ and dict_["tags"] is not None:
+            instance.tags = [str(i0) for i0 in dict_["tags"]]
+        elif include_empty:
+            instance.tags = []
         return instance
 
     @classmethod
     def create_many_from_dict(
         cls, dict_: dict, include_empty: bool = False
     ) -> Dict[str, ModelsAdminPlayerConcurrentRecordRequest]:
         return (
@@ -141,17 +162,19 @@
             return cls.create_from_dict(any_, include_empty=include_empty)
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
             "updatedAt": "updated_at",
             "value": "value",
+            "tags": "tags",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
             "updatedAt": True,
             "value": True,
+            "tags": False,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_admin_player_record_key_info.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_admin_player_record_key_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_admin_player_record_request.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_admin_player_record_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_admin_player_record_response.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_admin_player_record_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -39,24 +39,27 @@
         namespace: (namespace) REQUIRED str
 
         updated_at: (updated_at) REQUIRED str
 
         user_id: (user_id) REQUIRED str
 
         value: (value) REQUIRED Dict[str, Any]
+
+        tags: (tags) OPTIONAL List[str]
     """
 
     # region fields
 
     created_at: str  # REQUIRED
     key: str  # REQUIRED
     namespace: str  # REQUIRED
     updated_at: str  # REQUIRED
     user_id: str  # REQUIRED
     value: Dict[str, Any]  # REQUIRED
+    tags: List[str]  # OPTIONAL
 
     # endregion fields
 
     # region with_x methods
 
     def with_created_at(self, value: str) -> ModelsAdminPlayerRecordResponse:
         self.created_at = value
@@ -78,14 +81,18 @@
         self.user_id = value
         return self
 
     def with_value(self, value: Dict[str, Any]) -> ModelsAdminPlayerRecordResponse:
         self.value = value
         return self
 
+    def with_tags(self, value: List[str]) -> ModelsAdminPlayerRecordResponse:
+        self.tags = value
+        return self
+
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
         if hasattr(self, "created_at"):
@@ -108,14 +115,18 @@
             result["user_id"] = str(self.user_id)
         elif include_empty:
             result["user_id"] = ""
         if hasattr(self, "value"):
             result["value"] = {str(k0): v0 for k0, v0 in self.value.items()}
         elif include_empty:
             result["value"] = {}
+        if hasattr(self, "tags"):
+            result["tags"] = [str(i0) for i0 in self.tags]
+        elif include_empty:
+            result["tags"] = []
         return result
 
     # endregion to methods
 
     # region static methods
 
     @classmethod
@@ -123,23 +134,26 @@
         cls,
         created_at: str,
         key: str,
         namespace: str,
         updated_at: str,
         user_id: str,
         value: Dict[str, Any],
+        tags: Optional[List[str]] = None,
         **kwargs,
     ) -> ModelsAdminPlayerRecordResponse:
         instance = cls()
         instance.created_at = created_at
         instance.key = key
         instance.namespace = namespace
         instance.updated_at = updated_at
         instance.user_id = user_id
         instance.value = value
+        if tags is not None:
+            instance.tags = tags
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
     ) -> ModelsAdminPlayerRecordResponse:
         instance = cls()
@@ -165,14 +179,18 @@
             instance.user_id = str(dict_["user_id"])
         elif include_empty:
             instance.user_id = ""
         if "value" in dict_ and dict_["value"] is not None:
             instance.value = {str(k0): v0 for k0, v0 in dict_["value"].items()}
         elif include_empty:
             instance.value = {}
+        if "tags" in dict_ and dict_["tags"] is not None:
+            instance.tags = [str(i0) for i0 in dict_["tags"]]
+        elif include_empty:
+            instance.tags = []
         return instance
 
     @classmethod
     def create_many_from_dict(
         cls, dict_: dict, include_empty: bool = False
     ) -> Dict[str, ModelsAdminPlayerRecordResponse]:
         return (
@@ -214,21 +232,23 @@
         return {
             "created_at": "created_at",
             "key": "key",
             "namespace": "namespace",
             "updated_at": "updated_at",
             "user_id": "user_id",
             "value": "value",
+            "tags": "tags",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
             "created_at": True,
             "key": True,
             "namespace": True,
             "updated_at": True,
             "user_id": True,
             "value": True,
+            "tags": False,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_app_config.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_app_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_binary_info_response.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_binary_info_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_binary_record_request.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_binary_record_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_bulk_get_admin_game_record_request.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_bulk_get_admin_game_record_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_bulk_get_admin_game_record_response.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_bulk_get_admin_game_record_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_bulk_get_admin_player_record_request.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_bulk_get_admin_player_record_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_bulk_get_admin_player_record_response.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_bulk_get_admin_player_record_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_bulk_get_game_binary_record_response.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_bulk_get_game_binary_record_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_bulk_get_game_record_request.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_bulk_get_game_record_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_bulk_get_game_record_response.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_bulk_get_game_record_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_bulk_get_player_binary_record_response.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_bulk_get_player_binary_record_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_bulk_get_player_record_response.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_bulk_get_player_record_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_bulk_get_player_record_size_response.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_bulk_get_player_record_size_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_bulk_get_player_records_request.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_bulk_get_player_records_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_bulk_update_player_record_request_detail.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_bulk_update_player_record_request_detail.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_bulk_update_player_record_response.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_bulk_update_player_record_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_bulk_update_player_records_request.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_bulk_update_player_records_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_bulk_user_i_ds_request.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_bulk_user_i_ds_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_bulk_user_key_request.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_bulk_user_key_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_concurrent_record_request.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_bulk_update_player_record_by_key_request_detail.py`

 * *Files 15% similar despite different names*

```diff
@@ -24,132 +24,136 @@
 
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Model
 
 
-class ModelsConcurrentRecordRequest(Model):
-    """Models concurrent record request (models.ConcurrentRecordRequest)
+class ModelsBulkUpdatePlayerRecordByKeyRequestDetail(Model):
+    """Models bulk update player record by key request detail (models.BulkUpdatePlayerRecordByKeyRequestDetail)
 
     Properties:
-        updated_at: (updatedAt) REQUIRED str
+        user_id: (user_id) REQUIRED str
 
         value: (value) REQUIRED Dict[str, Any]
     """
 
     # region fields
 
-    updated_at: str  # REQUIRED
+    user_id: str  # REQUIRED
     value: Dict[str, Any]  # REQUIRED
 
     # endregion fields
 
     # region with_x methods
 
-    def with_updated_at(self, value: str) -> ModelsConcurrentRecordRequest:
-        self.updated_at = value
+    def with_user_id(
+        self, value: str
+    ) -> ModelsBulkUpdatePlayerRecordByKeyRequestDetail:
+        self.user_id = value
         return self
 
-    def with_value(self, value: Dict[str, Any]) -> ModelsConcurrentRecordRequest:
+    def with_value(
+        self, value: Dict[str, Any]
+    ) -> ModelsBulkUpdatePlayerRecordByKeyRequestDetail:
         self.value = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
-        if hasattr(self, "updated_at"):
-            result["updatedAt"] = str(self.updated_at)
+        if hasattr(self, "user_id"):
+            result["user_id"] = str(self.user_id)
         elif include_empty:
-            result["updatedAt"] = ""
+            result["user_id"] = ""
         if hasattr(self, "value"):
             result["value"] = {str(k0): v0 for k0, v0 in self.value.items()}
         elif include_empty:
             result["value"] = {}
         return result
 
     # endregion to methods
 
     # region static methods
 
     @classmethod
     def create(
-        cls, updated_at: str, value: Dict[str, Any], **kwargs
-    ) -> ModelsConcurrentRecordRequest:
+        cls, user_id: str, value: Dict[str, Any], **kwargs
+    ) -> ModelsBulkUpdatePlayerRecordByKeyRequestDetail:
         instance = cls()
-        instance.updated_at = updated_at
+        instance.user_id = user_id
         instance.value = value
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> ModelsConcurrentRecordRequest:
+    ) -> ModelsBulkUpdatePlayerRecordByKeyRequestDetail:
         instance = cls()
         if not dict_:
             return instance
-        if "updatedAt" in dict_ and dict_["updatedAt"] is not None:
-            instance.updated_at = str(dict_["updatedAt"])
+        if "user_id" in dict_ and dict_["user_id"] is not None:
+            instance.user_id = str(dict_["user_id"])
         elif include_empty:
-            instance.updated_at = ""
+            instance.user_id = ""
         if "value" in dict_ and dict_["value"] is not None:
             instance.value = {str(k0): v0 for k0, v0 in dict_["value"].items()}
         elif include_empty:
             instance.value = {}
         return instance
 
     @classmethod
     def create_many_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> Dict[str, ModelsConcurrentRecordRequest]:
+    ) -> Dict[str, ModelsBulkUpdatePlayerRecordByKeyRequestDetail]:
         return (
             {k: cls.create_from_dict(v, include_empty=include_empty) for k, v in dict_}
             if dict_
             else {}
         )
 
     @classmethod
     def create_many_from_list(
         cls, list_: list, include_empty: bool = False
-    ) -> List[ModelsConcurrentRecordRequest]:
+    ) -> List[ModelsBulkUpdatePlayerRecordByKeyRequestDetail]:
         return (
             [cls.create_from_dict(i, include_empty=include_empty) for i in list_]
             if list_
             else []
         )
 
     @classmethod
     def create_from_any(
         cls, any_: any, include_empty: bool = False, many: bool = False
     ) -> Union[
-        ModelsConcurrentRecordRequest,
-        List[ModelsConcurrentRecordRequest],
-        Dict[Any, ModelsConcurrentRecordRequest],
+        ModelsBulkUpdatePlayerRecordByKeyRequestDetail,
+        List[ModelsBulkUpdatePlayerRecordByKeyRequestDetail],
+        Dict[Any, ModelsBulkUpdatePlayerRecordByKeyRequestDetail],
     ]:
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
-            "updatedAt": "updated_at",
+            "user_id": "user_id",
             "value": "value",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
-            "updatedAt": True,
+            "user_id": True,
             "value": True,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_custom_config.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_custom_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_custom_function.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_custom_function.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_game_binary_record_admin_response.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_game_binary_record_admin_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,25 +49,28 @@
 
         updated_at: (updated_at) REQUIRED str
 
         binary_info: (binary_info) OPTIONAL ModelsBinaryInfoResponse
 
         set_by: (set_by) OPTIONAL Union[str, SetByEnum]
 
+        tags: (tags) OPTIONAL List[str]
+
         ttl_config: (ttl_config) OPTIONAL ModelsTTLConfigDTO
     """
 
     # region fields
 
     created_at: str  # REQUIRED
     key: str  # REQUIRED
     namespace: str  # REQUIRED
     updated_at: str  # REQUIRED
     binary_info: ModelsBinaryInfoResponse  # OPTIONAL
     set_by: Union[str, SetByEnum]  # OPTIONAL
+    tags: List[str]  # OPTIONAL
     ttl_config: ModelsTTLConfigDTO  # OPTIONAL
 
     # endregion fields
 
     # region with_x methods
 
     def with_created_at(self, value: str) -> ModelsGameBinaryRecordAdminResponse:
@@ -94,14 +97,18 @@
 
     def with_set_by(
         self, value: Union[str, SetByEnum]
     ) -> ModelsGameBinaryRecordAdminResponse:
         self.set_by = value
         return self
 
+    def with_tags(self, value: List[str]) -> ModelsGameBinaryRecordAdminResponse:
+        self.tags = value
+        return self
+
     def with_ttl_config(
         self, value: ModelsTTLConfigDTO
     ) -> ModelsGameBinaryRecordAdminResponse:
         self.ttl_config = value
         return self
 
     # endregion with_x methods
@@ -132,14 +139,18 @@
             )
         elif include_empty:
             result["binary_info"] = ModelsBinaryInfoResponse()
         if hasattr(self, "set_by"):
             result["set_by"] = str(self.set_by)
         elif include_empty:
             result["set_by"] = Union[str, SetByEnum]()
+        if hasattr(self, "tags"):
+            result["tags"] = [str(i0) for i0 in self.tags]
+        elif include_empty:
+            result["tags"] = []
         if hasattr(self, "ttl_config"):
             result["ttl_config"] = self.ttl_config.to_dict(include_empty=include_empty)
         elif include_empty:
             result["ttl_config"] = ModelsTTLConfigDTO()
         return result
 
     # endregion to methods
@@ -151,26 +162,29 @@
         cls,
         created_at: str,
         key: str,
         namespace: str,
         updated_at: str,
         binary_info: Optional[ModelsBinaryInfoResponse] = None,
         set_by: Optional[Union[str, SetByEnum]] = None,
+        tags: Optional[List[str]] = None,
         ttl_config: Optional[ModelsTTLConfigDTO] = None,
         **kwargs,
     ) -> ModelsGameBinaryRecordAdminResponse:
         instance = cls()
         instance.created_at = created_at
         instance.key = key
         instance.namespace = namespace
         instance.updated_at = updated_at
         if binary_info is not None:
             instance.binary_info = binary_info
         if set_by is not None:
             instance.set_by = set_by
+        if tags is not None:
+            instance.tags = tags
         if ttl_config is not None:
             instance.ttl_config = ttl_config
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
@@ -200,14 +214,18 @@
             )
         elif include_empty:
             instance.binary_info = ModelsBinaryInfoResponse()
         if "set_by" in dict_ and dict_["set_by"] is not None:
             instance.set_by = str(dict_["set_by"])
         elif include_empty:
             instance.set_by = Union[str, SetByEnum]()
+        if "tags" in dict_ and dict_["tags"] is not None:
+            instance.tags = [str(i0) for i0 in dict_["tags"]]
+        elif include_empty:
+            instance.tags = []
         if "ttl_config" in dict_ and dict_["ttl_config"] is not None:
             instance.ttl_config = ModelsTTLConfigDTO.create_from_dict(
                 dict_["ttl_config"], include_empty=include_empty
             )
         elif include_empty:
             instance.ttl_config = ModelsTTLConfigDTO()
         return instance
@@ -255,26 +273,28 @@
         return {
             "created_at": "created_at",
             "key": "key",
             "namespace": "namespace",
             "updated_at": "updated_at",
             "binary_info": "binary_info",
             "set_by": "set_by",
+            "tags": "tags",
             "ttl_config": "ttl_config",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
             "created_at": True,
             "key": True,
             "namespace": True,
             "updated_at": True,
             "binary_info": False,
             "set_by": False,
+            "tags": False,
             "ttl_config": False,
         }
 
     @staticmethod
     def get_enum_map() -> Dict[str, List[Any]]:
         return {
             "set_by": ["CLIENT", "SERVER"],
```

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_game_binary_record_create.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_game_binary_record_metadata_request.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,181 +32,165 @@
 
 
 class SetByEnum(StrEnum):
     CLIENT = "CLIENT"
     SERVER = "SERVER"
 
 
-class ModelsGameBinaryRecordCreate(Model):
-    """Models game binary record create (models.GameBinaryRecordCreate)
+class ModelsGameBinaryRecordMetadataRequest(Model):
+    """Models game binary record metadata request (models.GameBinaryRecordMetadataRequest)
 
     Properties:
-        file_type: (file_type) REQUIRED str
-
-        key: (key) REQUIRED str
-
         set_by: (set_by) REQUIRED Union[str, SetByEnum]
 
+        tags: (tags) OPTIONAL List[str]
+
         ttl_config: (ttl_config) OPTIONAL ModelsTTLConfigDTO
     """
 
     # region fields
 
-    file_type: str  # REQUIRED
-    key: str  # REQUIRED
     set_by: Union[str, SetByEnum]  # REQUIRED
+    tags: List[str]  # OPTIONAL
     ttl_config: ModelsTTLConfigDTO  # OPTIONAL
 
     # endregion fields
 
     # region with_x methods
 
-    def with_file_type(self, value: str) -> ModelsGameBinaryRecordCreate:
-        self.file_type = value
-        return self
-
-    def with_key(self, value: str) -> ModelsGameBinaryRecordCreate:
-        self.key = value
+    def with_set_by(
+        self, value: Union[str, SetByEnum]
+    ) -> ModelsGameBinaryRecordMetadataRequest:
+        self.set_by = value
         return self
 
-    def with_set_by(self, value: Union[str, SetByEnum]) -> ModelsGameBinaryRecordCreate:
-        self.set_by = value
+    def with_tags(self, value: List[str]) -> ModelsGameBinaryRecordMetadataRequest:
+        self.tags = value
         return self
 
     def with_ttl_config(
         self, value: ModelsTTLConfigDTO
-    ) -> ModelsGameBinaryRecordCreate:
+    ) -> ModelsGameBinaryRecordMetadataRequest:
         self.ttl_config = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
-        if hasattr(self, "file_type"):
-            result["file_type"] = str(self.file_type)
-        elif include_empty:
-            result["file_type"] = ""
-        if hasattr(self, "key"):
-            result["key"] = str(self.key)
-        elif include_empty:
-            result["key"] = ""
         if hasattr(self, "set_by"):
             result["set_by"] = str(self.set_by)
         elif include_empty:
             result["set_by"] = Union[str, SetByEnum]()
+        if hasattr(self, "tags"):
+            result["tags"] = [str(i0) for i0 in self.tags]
+        elif include_empty:
+            result["tags"] = []
         if hasattr(self, "ttl_config"):
             result["ttl_config"] = self.ttl_config.to_dict(include_empty=include_empty)
         elif include_empty:
             result["ttl_config"] = ModelsTTLConfigDTO()
         return result
 
     # endregion to methods
 
     # region static methods
 
     @classmethod
     def create(
         cls,
-        file_type: str,
-        key: str,
         set_by: Union[str, SetByEnum],
+        tags: Optional[List[str]] = None,
         ttl_config: Optional[ModelsTTLConfigDTO] = None,
         **kwargs,
-    ) -> ModelsGameBinaryRecordCreate:
+    ) -> ModelsGameBinaryRecordMetadataRequest:
         instance = cls()
-        instance.file_type = file_type
-        instance.key = key
         instance.set_by = set_by
+        if tags is not None:
+            instance.tags = tags
         if ttl_config is not None:
             instance.ttl_config = ttl_config
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> ModelsGameBinaryRecordCreate:
+    ) -> ModelsGameBinaryRecordMetadataRequest:
         instance = cls()
         if not dict_:
             return instance
-        if "file_type" in dict_ and dict_["file_type"] is not None:
-            instance.file_type = str(dict_["file_type"])
-        elif include_empty:
-            instance.file_type = ""
-        if "key" in dict_ and dict_["key"] is not None:
-            instance.key = str(dict_["key"])
-        elif include_empty:
-            instance.key = ""
         if "set_by" in dict_ and dict_["set_by"] is not None:
             instance.set_by = str(dict_["set_by"])
         elif include_empty:
             instance.set_by = Union[str, SetByEnum]()
+        if "tags" in dict_ and dict_["tags"] is not None:
+            instance.tags = [str(i0) for i0 in dict_["tags"]]
+        elif include_empty:
+            instance.tags = []
         if "ttl_config" in dict_ and dict_["ttl_config"] is not None:
             instance.ttl_config = ModelsTTLConfigDTO.create_from_dict(
                 dict_["ttl_config"], include_empty=include_empty
             )
         elif include_empty:
             instance.ttl_config = ModelsTTLConfigDTO()
         return instance
 
     @classmethod
     def create_many_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> Dict[str, ModelsGameBinaryRecordCreate]:
+    ) -> Dict[str, ModelsGameBinaryRecordMetadataRequest]:
         return (
             {k: cls.create_from_dict(v, include_empty=include_empty) for k, v in dict_}
             if dict_
             else {}
         )
 
     @classmethod
     def create_many_from_list(
         cls, list_: list, include_empty: bool = False
-    ) -> List[ModelsGameBinaryRecordCreate]:
+    ) -> List[ModelsGameBinaryRecordMetadataRequest]:
         return (
             [cls.create_from_dict(i, include_empty=include_empty) for i in list_]
             if list_
             else []
         )
 
     @classmethod
     def create_from_any(
         cls, any_: any, include_empty: bool = False, many: bool = False
     ) -> Union[
-        ModelsGameBinaryRecordCreate,
-        List[ModelsGameBinaryRecordCreate],
-        Dict[Any, ModelsGameBinaryRecordCreate],
+        ModelsGameBinaryRecordMetadataRequest,
+        List[ModelsGameBinaryRecordMetadataRequest],
+        Dict[Any, ModelsGameBinaryRecordMetadataRequest],
     ]:
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
-            "file_type": "file_type",
-            "key": "key",
             "set_by": "set_by",
+            "tags": "tags",
             "ttl_config": "ttl_config",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
-            "file_type": True,
-            "key": True,
             "set_by": True,
+            "tags": False,
             "ttl_config": False,
         }
 
     @staticmethod
     def get_enum_map() -> Dict[str, List[Any]]:
         return {
             "set_by": ["CLIENT", "SERVER"],
```

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_game_binary_record_metadata_request.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_player_binary_record_metadata_request.py`

 * *Files 16% similar despite different names*

```diff
@@ -24,154 +24,169 @@
 
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Model
 from accelbyte_py_sdk.core import StrEnum
 
-from ..models.models_ttl_config_dto import ModelsTTLConfigDTO
-
 
 class SetByEnum(StrEnum):
     CLIENT = "CLIENT"
     SERVER = "SERVER"
 
 
-class ModelsGameBinaryRecordMetadataRequest(Model):
-    """Models game binary record metadata request (models.GameBinaryRecordMetadataRequest)
+class ModelsPlayerBinaryRecordMetadataRequest(Model):
+    """Models player binary record metadata request (models.PlayerBinaryRecordMetadataRequest)
 
     Properties:
-        set_by: (set_by) REQUIRED Union[str, SetByEnum]
+        is_public: (is_public) OPTIONAL bool
+
+        set_by: (set_by) OPTIONAL Union[str, SetByEnum]
 
-        ttl_config: (ttl_config) OPTIONAL ModelsTTLConfigDTO
+        tags: (tags) OPTIONAL List[str]
     """
 
     # region fields
 
-    set_by: Union[str, SetByEnum]  # REQUIRED
-    ttl_config: ModelsTTLConfigDTO  # OPTIONAL
+    is_public: bool  # OPTIONAL
+    set_by: Union[str, SetByEnum]  # OPTIONAL
+    tags: List[str]  # OPTIONAL
 
     # endregion fields
 
     # region with_x methods
 
+    def with_is_public(self, value: bool) -> ModelsPlayerBinaryRecordMetadataRequest:
+        self.is_public = value
+        return self
+
     def with_set_by(
         self, value: Union[str, SetByEnum]
-    ) -> ModelsGameBinaryRecordMetadataRequest:
+    ) -> ModelsPlayerBinaryRecordMetadataRequest:
         self.set_by = value
         return self
 
-    def with_ttl_config(
-        self, value: ModelsTTLConfigDTO
-    ) -> ModelsGameBinaryRecordMetadataRequest:
-        self.ttl_config = value
+    def with_tags(self, value: List[str]) -> ModelsPlayerBinaryRecordMetadataRequest:
+        self.tags = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
+        if hasattr(self, "is_public"):
+            result["is_public"] = bool(self.is_public)
+        elif include_empty:
+            result["is_public"] = False
         if hasattr(self, "set_by"):
             result["set_by"] = str(self.set_by)
         elif include_empty:
             result["set_by"] = Union[str, SetByEnum]()
-        if hasattr(self, "ttl_config"):
-            result["ttl_config"] = self.ttl_config.to_dict(include_empty=include_empty)
+        if hasattr(self, "tags"):
+            result["tags"] = [str(i0) for i0 in self.tags]
         elif include_empty:
-            result["ttl_config"] = ModelsTTLConfigDTO()
+            result["tags"] = []
         return result
 
     # endregion to methods
 
     # region static methods
 
     @classmethod
     def create(
         cls,
-        set_by: Union[str, SetByEnum],
-        ttl_config: Optional[ModelsTTLConfigDTO] = None,
+        is_public: Optional[bool] = None,
+        set_by: Optional[Union[str, SetByEnum]] = None,
+        tags: Optional[List[str]] = None,
         **kwargs,
-    ) -> ModelsGameBinaryRecordMetadataRequest:
+    ) -> ModelsPlayerBinaryRecordMetadataRequest:
         instance = cls()
-        instance.set_by = set_by
-        if ttl_config is not None:
-            instance.ttl_config = ttl_config
+        if is_public is not None:
+            instance.is_public = is_public
+        if set_by is not None:
+            instance.set_by = set_by
+        if tags is not None:
+            instance.tags = tags
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> ModelsGameBinaryRecordMetadataRequest:
+    ) -> ModelsPlayerBinaryRecordMetadataRequest:
         instance = cls()
         if not dict_:
             return instance
+        if "is_public" in dict_ and dict_["is_public"] is not None:
+            instance.is_public = bool(dict_["is_public"])
+        elif include_empty:
+            instance.is_public = False
         if "set_by" in dict_ and dict_["set_by"] is not None:
             instance.set_by = str(dict_["set_by"])
         elif include_empty:
             instance.set_by = Union[str, SetByEnum]()
-        if "ttl_config" in dict_ and dict_["ttl_config"] is not None:
-            instance.ttl_config = ModelsTTLConfigDTO.create_from_dict(
-                dict_["ttl_config"], include_empty=include_empty
-            )
+        if "tags" in dict_ and dict_["tags"] is not None:
+            instance.tags = [str(i0) for i0 in dict_["tags"]]
         elif include_empty:
-            instance.ttl_config = ModelsTTLConfigDTO()
+            instance.tags = []
         return instance
 
     @classmethod
     def create_many_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> Dict[str, ModelsGameBinaryRecordMetadataRequest]:
+    ) -> Dict[str, ModelsPlayerBinaryRecordMetadataRequest]:
         return (
             {k: cls.create_from_dict(v, include_empty=include_empty) for k, v in dict_}
             if dict_
             else {}
         )
 
     @classmethod
     def create_many_from_list(
         cls, list_: list, include_empty: bool = False
-    ) -> List[ModelsGameBinaryRecordMetadataRequest]:
+    ) -> List[ModelsPlayerBinaryRecordMetadataRequest]:
         return (
             [cls.create_from_dict(i, include_empty=include_empty) for i in list_]
             if list_
             else []
         )
 
     @classmethod
     def create_from_any(
         cls, any_: any, include_empty: bool = False, many: bool = False
     ) -> Union[
-        ModelsGameBinaryRecordMetadataRequest,
-        List[ModelsGameBinaryRecordMetadataRequest],
-        Dict[Any, ModelsGameBinaryRecordMetadataRequest],
+        ModelsPlayerBinaryRecordMetadataRequest,
+        List[ModelsPlayerBinaryRecordMetadataRequest],
+        Dict[Any, ModelsPlayerBinaryRecordMetadataRequest],
     ]:
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
+            "is_public": "is_public",
             "set_by": "set_by",
-            "ttl_config": "ttl_config",
+            "tags": "tags",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
-            "set_by": True,
-            "ttl_config": False,
+            "is_public": False,
+            "set_by": False,
+            "tags": False,
         }
 
     @staticmethod
     def get_enum_map() -> Dict[str, List[Any]]:
         return {
             "set_by": ["CLIENT", "SERVER"],
         }
```

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_game_binary_record_response.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_game_binary_record_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_game_record_admin_response.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_game_record_admin_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,25 +48,28 @@
 
         updated_at: (updated_at) REQUIRED str
 
         value: (value) REQUIRED Dict[str, Any]
 
         set_by: (set_by) OPTIONAL Union[str, SetByEnum]
 
+        tags: (tags) OPTIONAL List[str]
+
         ttl_config: (ttl_config) OPTIONAL ModelsTTLConfigDTO
     """
 
     # region fields
 
     created_at: str  # REQUIRED
     key: str  # REQUIRED
     namespace: str  # REQUIRED
     updated_at: str  # REQUIRED
     value: Dict[str, Any]  # REQUIRED
     set_by: Union[str, SetByEnum]  # OPTIONAL
+    tags: List[str]  # OPTIONAL
     ttl_config: ModelsTTLConfigDTO  # OPTIONAL
 
     # endregion fields
 
     # region with_x methods
 
     def with_created_at(self, value: str) -> ModelsGameRecordAdminResponse:
@@ -91,14 +94,18 @@
 
     def with_set_by(
         self, value: Union[str, SetByEnum]
     ) -> ModelsGameRecordAdminResponse:
         self.set_by = value
         return self
 
+    def with_tags(self, value: List[str]) -> ModelsGameRecordAdminResponse:
+        self.tags = value
+        return self
+
     def with_ttl_config(
         self, value: ModelsTTLConfigDTO
     ) -> ModelsGameRecordAdminResponse:
         self.ttl_config = value
         return self
 
     # endregion with_x methods
@@ -127,14 +134,18 @@
             result["value"] = {str(k0): v0 for k0, v0 in self.value.items()}
         elif include_empty:
             result["value"] = {}
         if hasattr(self, "set_by"):
             result["set_by"] = str(self.set_by)
         elif include_empty:
             result["set_by"] = Union[str, SetByEnum]()
+        if hasattr(self, "tags"):
+            result["tags"] = [str(i0) for i0 in self.tags]
+        elif include_empty:
+            result["tags"] = []
         if hasattr(self, "ttl_config"):
             result["ttl_config"] = self.ttl_config.to_dict(include_empty=include_empty)
         elif include_empty:
             result["ttl_config"] = ModelsTTLConfigDTO()
         return result
 
     # endregion to methods
@@ -146,25 +157,28 @@
         cls,
         created_at: str,
         key: str,
         namespace: str,
         updated_at: str,
         value: Dict[str, Any],
         set_by: Optional[Union[str, SetByEnum]] = None,
+        tags: Optional[List[str]] = None,
         ttl_config: Optional[ModelsTTLConfigDTO] = None,
         **kwargs,
     ) -> ModelsGameRecordAdminResponse:
         instance = cls()
         instance.created_at = created_at
         instance.key = key
         instance.namespace = namespace
         instance.updated_at = updated_at
         instance.value = value
         if set_by is not None:
             instance.set_by = set_by
+        if tags is not None:
+            instance.tags = tags
         if ttl_config is not None:
             instance.ttl_config = ttl_config
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
@@ -192,14 +206,18 @@
             instance.value = {str(k0): v0 for k0, v0 in dict_["value"].items()}
         elif include_empty:
             instance.value = {}
         if "set_by" in dict_ and dict_["set_by"] is not None:
             instance.set_by = str(dict_["set_by"])
         elif include_empty:
             instance.set_by = Union[str, SetByEnum]()
+        if "tags" in dict_ and dict_["tags"] is not None:
+            instance.tags = [str(i0) for i0 in dict_["tags"]]
+        elif include_empty:
+            instance.tags = []
         if "ttl_config" in dict_ and dict_["ttl_config"] is not None:
             instance.ttl_config = ModelsTTLConfigDTO.create_from_dict(
                 dict_["ttl_config"], include_empty=include_empty
             )
         elif include_empty:
             instance.ttl_config = ModelsTTLConfigDTO()
         return instance
@@ -247,26 +265,28 @@
         return {
             "created_at": "created_at",
             "key": "key",
             "namespace": "namespace",
             "updated_at": "updated_at",
             "value": "value",
             "set_by": "set_by",
+            "tags": "tags",
             "ttl_config": "ttl_config",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
             "created_at": True,
             "key": True,
             "namespace": True,
             "updated_at": True,
             "value": True,
             "set_by": False,
+            "tags": False,
             "ttl_config": False,
         }
 
     @staticmethod
     def get_enum_map() -> Dict[str, List[Any]]:
         return {
             "set_by": ["CLIENT", "SERVER"],
```

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_game_record_request.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_game_record_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_game_record_response.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_game_record_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,24 +45,27 @@
         namespace: (namespace) REQUIRED str
 
         updated_at: (updated_at) REQUIRED str
 
         value: (value) REQUIRED Dict[str, Any]
 
         set_by: (set_by) OPTIONAL Union[str, SetByEnum]
+
+        tags: (tags) OPTIONAL List[str]
     """
 
     # region fields
 
     created_at: str  # REQUIRED
     key: str  # REQUIRED
     namespace: str  # REQUIRED
     updated_at: str  # REQUIRED
     value: Dict[str, Any]  # REQUIRED
     set_by: Union[str, SetByEnum]  # OPTIONAL
+    tags: List[str]  # OPTIONAL
 
     # endregion fields
 
     # region with_x methods
 
     def with_created_at(self, value: str) -> ModelsGameRecordResponse:
         self.created_at = value
@@ -84,14 +87,18 @@
         self.value = value
         return self
 
     def with_set_by(self, value: Union[str, SetByEnum]) -> ModelsGameRecordResponse:
         self.set_by = value
         return self
 
+    def with_tags(self, value: List[str]) -> ModelsGameRecordResponse:
+        self.tags = value
+        return self
+
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
         if hasattr(self, "created_at"):
@@ -114,14 +121,18 @@
             result["value"] = {str(k0): v0 for k0, v0 in self.value.items()}
         elif include_empty:
             result["value"] = {}
         if hasattr(self, "set_by"):
             result["set_by"] = str(self.set_by)
         elif include_empty:
             result["set_by"] = Union[str, SetByEnum]()
+        if hasattr(self, "tags"):
+            result["tags"] = [str(i0) for i0 in self.tags]
+        elif include_empty:
+            result["tags"] = []
         return result
 
     # endregion to methods
 
     # region static methods
 
     @classmethod
@@ -129,24 +140,27 @@
         cls,
         created_at: str,
         key: str,
         namespace: str,
         updated_at: str,
         value: Dict[str, Any],
         set_by: Optional[Union[str, SetByEnum]] = None,
+        tags: Optional[List[str]] = None,
         **kwargs,
     ) -> ModelsGameRecordResponse:
         instance = cls()
         instance.created_at = created_at
         instance.key = key
         instance.namespace = namespace
         instance.updated_at = updated_at
         instance.value = value
         if set_by is not None:
             instance.set_by = set_by
+        if tags is not None:
+            instance.tags = tags
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
     ) -> ModelsGameRecordResponse:
         instance = cls()
@@ -172,14 +186,18 @@
             instance.value = {str(k0): v0 for k0, v0 in dict_["value"].items()}
         elif include_empty:
             instance.value = {}
         if "set_by" in dict_ and dict_["set_by"] is not None:
             instance.set_by = str(dict_["set_by"])
         elif include_empty:
             instance.set_by = Union[str, SetByEnum]()
+        if "tags" in dict_ and dict_["tags"] is not None:
+            instance.tags = [str(i0) for i0 in dict_["tags"]]
+        elif include_empty:
+            instance.tags = []
         return instance
 
     @classmethod
     def create_many_from_dict(
         cls, dict_: dict, include_empty: bool = False
     ) -> Dict[str, ModelsGameRecordResponse]:
         return (
@@ -221,25 +239,27 @@
         return {
             "created_at": "created_at",
             "key": "key",
             "namespace": "namespace",
             "updated_at": "updated_at",
             "value": "value",
             "set_by": "set_by",
+            "tags": "tags",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
             "created_at": True,
             "key": True,
             "namespace": True,
             "updated_at": True,
             "value": True,
             "set_by": False,
+            "tags": False,
         }
 
     @staticmethod
     def get_enum_map() -> Dict[str, List[Any]]:
         return {
             "set_by": ["CLIENT", "SERVER"],
         }
```

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_list_admin_game_record_keys_response.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_list_admin_game_record_keys_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_list_admin_player_record_keys_response.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_list_admin_player_record_keys_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_list_game_binary_records_admin_response.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_list_game_binary_records_admin_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_list_game_binary_records_response.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_list_game_binary_records_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_list_game_record_keys_response.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_list_game_record_keys_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_list_player_binary_records_response.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_list_player_binary_records_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_list_player_record_keys_response.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_list_player_record_keys_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_list_tags_response.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_list_tags_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_pagination.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_pagination.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_player_binary_record_create.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_player_binary_record_create.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_player_binary_record_metadata_public_request.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_player_binary_record_metadata_public_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_player_binary_record_metadata_request.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_bulk_update_player_record_by_key_response.py`

 * *Files 15% similar despite different names*

```diff
@@ -22,153 +22,154 @@
 # pylint: disable=too-many-statements
 # pylint: disable=unused-import
 
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Model
-from accelbyte_py_sdk.core import StrEnum
 
 
-class SetByEnum(StrEnum):
-    CLIENT = "CLIENT"
-    SERVER = "SERVER"
-
-
-class ModelsPlayerBinaryRecordMetadataRequest(Model):
-    """Models player binary record metadata request (models.PlayerBinaryRecordMetadataRequest)
+class ModelsBulkUpdatePlayerRecordByKeyResponse(Model):
+    """Models bulk update player record by key response (models.BulkUpdatePlayerRecordByKeyResponse)
 
     Properties:
-        is_public: (is_public) OPTIONAL bool
+        detail: (detail) REQUIRED Dict[str, Any]
+
+        success: (success) REQUIRED bool
 
-        set_by: (set_by) OPTIONAL Union[str, SetByEnum]
+        user_id: (user_id) REQUIRED str
     """
 
     # region fields
 
-    is_public: bool  # OPTIONAL
-    set_by: Union[str, SetByEnum]  # OPTIONAL
+    detail: Dict[str, Any]  # REQUIRED
+    success: bool  # REQUIRED
+    user_id: str  # REQUIRED
 
     # endregion fields
 
     # region with_x methods
 
-    def with_is_public(self, value: bool) -> ModelsPlayerBinaryRecordMetadataRequest:
-        self.is_public = value
+    def with_detail(
+        self, value: Dict[str, Any]
+    ) -> ModelsBulkUpdatePlayerRecordByKeyResponse:
+        self.detail = value
         return self
 
-    def with_set_by(
-        self, value: Union[str, SetByEnum]
-    ) -> ModelsPlayerBinaryRecordMetadataRequest:
-        self.set_by = value
+    def with_success(self, value: bool) -> ModelsBulkUpdatePlayerRecordByKeyResponse:
+        self.success = value
+        return self
+
+    def with_user_id(self, value: str) -> ModelsBulkUpdatePlayerRecordByKeyResponse:
+        self.user_id = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
-        if hasattr(self, "is_public"):
-            result["is_public"] = bool(self.is_public)
+        if hasattr(self, "detail"):
+            result["detail"] = {str(k0): v0 for k0, v0 in self.detail.items()}
+        elif include_empty:
+            result["detail"] = {}
+        if hasattr(self, "success"):
+            result["success"] = bool(self.success)
         elif include_empty:
-            result["is_public"] = False
-        if hasattr(self, "set_by"):
-            result["set_by"] = str(self.set_by)
+            result["success"] = False
+        if hasattr(self, "user_id"):
+            result["user_id"] = str(self.user_id)
         elif include_empty:
-            result["set_by"] = Union[str, SetByEnum]()
+            result["user_id"] = ""
         return result
 
     # endregion to methods
 
     # region static methods
 
     @classmethod
     def create(
-        cls,
-        is_public: Optional[bool] = None,
-        set_by: Optional[Union[str, SetByEnum]] = None,
-        **kwargs,
-    ) -> ModelsPlayerBinaryRecordMetadataRequest:
+        cls, detail: Dict[str, Any], success: bool, user_id: str, **kwargs
+    ) -> ModelsBulkUpdatePlayerRecordByKeyResponse:
         instance = cls()
-        if is_public is not None:
-            instance.is_public = is_public
-        if set_by is not None:
-            instance.set_by = set_by
+        instance.detail = detail
+        instance.success = success
+        instance.user_id = user_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> ModelsPlayerBinaryRecordMetadataRequest:
+    ) -> ModelsBulkUpdatePlayerRecordByKeyResponse:
         instance = cls()
         if not dict_:
             return instance
-        if "is_public" in dict_ and dict_["is_public"] is not None:
-            instance.is_public = bool(dict_["is_public"])
+        if "detail" in dict_ and dict_["detail"] is not None:
+            instance.detail = {str(k0): v0 for k0, v0 in dict_["detail"].items()}
         elif include_empty:
-            instance.is_public = False
-        if "set_by" in dict_ and dict_["set_by"] is not None:
-            instance.set_by = str(dict_["set_by"])
+            instance.detail = {}
+        if "success" in dict_ and dict_["success"] is not None:
+            instance.success = bool(dict_["success"])
         elif include_empty:
-            instance.set_by = Union[str, SetByEnum]()
+            instance.success = False
+        if "user_id" in dict_ and dict_["user_id"] is not None:
+            instance.user_id = str(dict_["user_id"])
+        elif include_empty:
+            instance.user_id = ""
         return instance
 
     @classmethod
     def create_many_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> Dict[str, ModelsPlayerBinaryRecordMetadataRequest]:
+    ) -> Dict[str, ModelsBulkUpdatePlayerRecordByKeyResponse]:
         return (
             {k: cls.create_from_dict(v, include_empty=include_empty) for k, v in dict_}
             if dict_
             else {}
         )
 
     @classmethod
     def create_many_from_list(
         cls, list_: list, include_empty: bool = False
-    ) -> List[ModelsPlayerBinaryRecordMetadataRequest]:
+    ) -> List[ModelsBulkUpdatePlayerRecordByKeyResponse]:
         return (
             [cls.create_from_dict(i, include_empty=include_empty) for i in list_]
             if list_
             else []
         )
 
     @classmethod
     def create_from_any(
         cls, any_: any, include_empty: bool = False, many: bool = False
     ) -> Union[
-        ModelsPlayerBinaryRecordMetadataRequest,
-        List[ModelsPlayerBinaryRecordMetadataRequest],
-        Dict[Any, ModelsPlayerBinaryRecordMetadataRequest],
+        ModelsBulkUpdatePlayerRecordByKeyResponse,
+        List[ModelsBulkUpdatePlayerRecordByKeyResponse],
+        Dict[Any, ModelsBulkUpdatePlayerRecordByKeyResponse],
     ]:
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
-            "is_public": "is_public",
-            "set_by": "set_by",
+            "detail": "detail",
+            "success": "success",
+            "user_id": "user_id",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
-            "is_public": False,
-            "set_by": False,
-        }
-
-    @staticmethod
-    def get_enum_map() -> Dict[str, List[Any]]:
-        return {
-            "set_by": ["CLIENT", "SERVER"],
+            "detail": True,
+            "success": True,
+            "user_id": True,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_player_binary_record_response.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_player_binary_record_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,26 +51,29 @@
         updated_at: (updated_at) REQUIRED str
 
         user_id: (user_id) REQUIRED str
 
         binary_info: (binary_info) OPTIONAL ModelsBinaryInfoResponse
 
         set_by: (set_by) OPTIONAL Union[str, SetByEnum]
+
+        tags: (tags) OPTIONAL List[str]
     """
 
     # region fields
 
     created_at: str  # REQUIRED
     is_public: bool  # REQUIRED
     key: str  # REQUIRED
     namespace: str  # REQUIRED
     updated_at: str  # REQUIRED
     user_id: str  # REQUIRED
     binary_info: ModelsBinaryInfoResponse  # OPTIONAL
     set_by: Union[str, SetByEnum]  # OPTIONAL
+    tags: List[str]  # OPTIONAL
 
     # endregion fields
 
     # region with_x methods
 
     def with_created_at(self, value: str) -> ModelsPlayerBinaryRecordResponse:
         self.created_at = value
@@ -104,14 +107,18 @@
 
     def with_set_by(
         self, value: Union[str, SetByEnum]
     ) -> ModelsPlayerBinaryRecordResponse:
         self.set_by = value
         return self
 
+    def with_tags(self, value: List[str]) -> ModelsPlayerBinaryRecordResponse:
+        self.tags = value
+        return self
+
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
         if hasattr(self, "created_at"):
@@ -144,14 +151,18 @@
             )
         elif include_empty:
             result["binary_info"] = ModelsBinaryInfoResponse()
         if hasattr(self, "set_by"):
             result["set_by"] = str(self.set_by)
         elif include_empty:
             result["set_by"] = Union[str, SetByEnum]()
+        if hasattr(self, "tags"):
+            result["tags"] = [str(i0) for i0 in self.tags]
+        elif include_empty:
+            result["tags"] = []
         return result
 
     # endregion to methods
 
     # region static methods
 
     @classmethod
@@ -161,27 +172,30 @@
         is_public: bool,
         key: str,
         namespace: str,
         updated_at: str,
         user_id: str,
         binary_info: Optional[ModelsBinaryInfoResponse] = None,
         set_by: Optional[Union[str, SetByEnum]] = None,
+        tags: Optional[List[str]] = None,
         **kwargs,
     ) -> ModelsPlayerBinaryRecordResponse:
         instance = cls()
         instance.created_at = created_at
         instance.is_public = is_public
         instance.key = key
         instance.namespace = namespace
         instance.updated_at = updated_at
         instance.user_id = user_id
         if binary_info is not None:
             instance.binary_info = binary_info
         if set_by is not None:
             instance.set_by = set_by
+        if tags is not None:
+            instance.tags = tags
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
     ) -> ModelsPlayerBinaryRecordResponse:
         instance = cls()
@@ -217,14 +231,18 @@
             )
         elif include_empty:
             instance.binary_info = ModelsBinaryInfoResponse()
         if "set_by" in dict_ and dict_["set_by"] is not None:
             instance.set_by = str(dict_["set_by"])
         elif include_empty:
             instance.set_by = Union[str, SetByEnum]()
+        if "tags" in dict_ and dict_["tags"] is not None:
+            instance.tags = [str(i0) for i0 in dict_["tags"]]
+        elif include_empty:
+            instance.tags = []
         return instance
 
     @classmethod
     def create_many_from_dict(
         cls, dict_: dict, include_empty: bool = False
     ) -> Dict[str, ModelsPlayerBinaryRecordResponse]:
         return (
@@ -268,27 +286,29 @@
             "is_public": "is_public",
             "key": "key",
             "namespace": "namespace",
             "updated_at": "updated_at",
             "user_id": "user_id",
             "binary_info": "binary_info",
             "set_by": "set_by",
+            "tags": "tags",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
             "created_at": True,
             "is_public": True,
             "key": True,
             "namespace": True,
             "updated_at": True,
             "user_id": True,
             "binary_info": False,
             "set_by": False,
+            "tags": False,
         }
 
     @staticmethod
     def get_enum_map() -> Dict[str, List[Any]]:
         return {
             "set_by": ["CLIENT", "SERVER"],
         }
```

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_player_record_concurrent_update_response.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_player_record_concurrent_update_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_player_record_key_info.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_player_record_key_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_player_record_request.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_player_record_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_player_record_response.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_player_record_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,26 +49,29 @@
         updated_at: (updated_at) REQUIRED str
 
         user_id: (user_id) REQUIRED str
 
         value: (value) REQUIRED Dict[str, Any]
 
         set_by: (set_by) OPTIONAL Union[str, SetByEnum]
+
+        tags: (tags) OPTIONAL List[str]
     """
 
     # region fields
 
     created_at: str  # REQUIRED
     is_public: bool  # REQUIRED
     key: str  # REQUIRED
     namespace: str  # REQUIRED
     updated_at: str  # REQUIRED
     user_id: str  # REQUIRED
     value: Dict[str, Any]  # REQUIRED
     set_by: Union[str, SetByEnum]  # OPTIONAL
+    tags: List[str]  # OPTIONAL
 
     # endregion fields
 
     # region with_x methods
 
     def with_created_at(self, value: str) -> ModelsPlayerRecordResponse:
         self.created_at = value
@@ -98,14 +101,18 @@
         self.value = value
         return self
 
     def with_set_by(self, value: Union[str, SetByEnum]) -> ModelsPlayerRecordResponse:
         self.set_by = value
         return self
 
+    def with_tags(self, value: List[str]) -> ModelsPlayerRecordResponse:
+        self.tags = value
+        return self
+
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
         if hasattr(self, "created_at"):
@@ -136,14 +143,18 @@
             result["value"] = {str(k0): v0 for k0, v0 in self.value.items()}
         elif include_empty:
             result["value"] = {}
         if hasattr(self, "set_by"):
             result["set_by"] = str(self.set_by)
         elif include_empty:
             result["set_by"] = Union[str, SetByEnum]()
+        if hasattr(self, "tags"):
+            result["tags"] = [str(i0) for i0 in self.tags]
+        elif include_empty:
+            result["tags"] = []
         return result
 
     # endregion to methods
 
     # region static methods
 
     @classmethod
@@ -153,26 +164,29 @@
         is_public: bool,
         key: str,
         namespace: str,
         updated_at: str,
         user_id: str,
         value: Dict[str, Any],
         set_by: Optional[Union[str, SetByEnum]] = None,
+        tags: Optional[List[str]] = None,
         **kwargs,
     ) -> ModelsPlayerRecordResponse:
         instance = cls()
         instance.created_at = created_at
         instance.is_public = is_public
         instance.key = key
         instance.namespace = namespace
         instance.updated_at = updated_at
         instance.user_id = user_id
         instance.value = value
         if set_by is not None:
             instance.set_by = set_by
+        if tags is not None:
+            instance.tags = tags
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
     ) -> ModelsPlayerRecordResponse:
         instance = cls()
@@ -206,14 +220,18 @@
             instance.value = {str(k0): v0 for k0, v0 in dict_["value"].items()}
         elif include_empty:
             instance.value = {}
         if "set_by" in dict_ and dict_["set_by"] is not None:
             instance.set_by = str(dict_["set_by"])
         elif include_empty:
             instance.set_by = Union[str, SetByEnum]()
+        if "tags" in dict_ and dict_["tags"] is not None:
+            instance.tags = [str(i0) for i0 in dict_["tags"]]
+        elif include_empty:
+            instance.tags = []
         return instance
 
     @classmethod
     def create_many_from_dict(
         cls, dict_: dict, include_empty: bool = False
     ) -> Dict[str, ModelsPlayerRecordResponse]:
         return (
@@ -257,27 +275,29 @@
             "is_public": "is_public",
             "key": "key",
             "namespace": "namespace",
             "updated_at": "updated_at",
             "user_id": "user_id",
             "value": "value",
             "set_by": "set_by",
+            "tags": "tags",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
             "created_at": True,
             "is_public": True,
             "key": True,
             "namespace": True,
             "updated_at": True,
             "user_id": True,
             "value": True,
             "set_by": False,
+            "tags": False,
         }
 
     @staticmethod
     def get_enum_map() -> Dict[str, List[Any]]:
         return {
             "set_by": ["CLIENT", "SERVER"],
         }
```

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_player_record_size_response.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_player_record_size_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_plugin_request.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_plugin_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_plugin_response.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_plugin_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_public_game_binary_record_create.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_public_game_binary_record_create.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_public_player_binary_record_create.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_public_player_binary_record_create.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_response_error.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_response_error.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_tag_info.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_tag_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_tag_request.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_tag_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_ttl_config_dto.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_ttl_config_dto.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_upload_binary_record_request.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_upload_binary_record_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_upload_binary_record_response.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_upload_binary_record_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/models/models_user_key_request.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/models/models_user_key_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_concurrent_record/__init__.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_concurrent_record/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Cloudsave Service."""
 
-__version__ = "3.15.1"
+__version__ = "3.16.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .admin_put_admin_game_re_99ac43 import AdminPutAdminGameRecordConcurrentHandlerV1
 from .admin_put_admin_player__e84e5d import AdminPutAdminPlayerRecordConcurrentHandlerV1
```

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_concurrent_record/admin_put_admin_game_re_99ac43.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_concurrent_record/admin_put_admin_game_re_99ac43.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,19 +77,22 @@
 
 
     ## Parameters Notes
     1. updatedAt (required: true)
     Time format style: RFC3339
     2. value
     Json
+    3. tags (default: *empty array*, type: array of string)
+    Indicate the tagging for the admin record.
     **Request Body Example:**
     ```
     {
     "value": {},
-    "updatedAt": "2022-03-17T10:42:15.444Z"
+    "updatedAt": "2022-03-17T10:42:15.444Z",
+    "tags": ["tag1", "tag2"]
     }
     ```
     ## Optimistic Concurrency Control
 
     This endpoint implement optimistic concurrency control to avoid race condition.
     If the record has been updated since the client fetch it, the server will return HTTP status code 412 (precondition failed)
     and client need to redo the operation (fetch data and do update).
```

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_concurrent_record/admin_put_admin_player__e84e5d.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_concurrent_record/admin_put_admin_player__e84e5d.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,19 +78,22 @@
 
 
     ## Parameters Notes
     1. updatedAt (required: true)
     Time format style: RFC3339
     2. value
     Json
+    3. tags (default: *empty array*, type: array of string)
+    Indicate the tagging for the admin record.
     **Request Body Example:**
     ```
     {
     "value": {},
-    "updatedAt": "2022-03-17T10:42:15.444Z"
+    "updatedAt": "2022-03-17T10:42:15.444Z",
+    "tags": ["tag1", "tag2"]
     }
     ```
 
     ## Optimistic Concurrency Control
 
     This endpoint implement optimistic concurrency control to avoid race condition.
     If the record has been updated since the client fetch it, the server will return HTTP status code 412 (precondition failed)
```

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_concurrent_record/admin_put_game_record_c_886b02.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_concurrent_record/admin_put_game_record_c_886b02.py`

 * *Files 3% similar despite different names*

```diff
@@ -81,20 +81,23 @@
     Indicate which party that could modify the game record.
     SERVER: record can be modified by server only.
     CLIENT: record can be modified by client and server.
     2. updatedAt (required: true)
     Time format style: RFC3339
     3. value
     Json
+    4. tags (default: *empty array*, type: array of string)
+    Indicate the tagging for the game record.
     **Request Body Example:**
     ```
     {
     "set_by": "SERVER",
     "value": {},
-    "updatedAt": "2022-03-17T10:42:15.444Z"
+    "updatedAt": "2022-03-17T10:42:15.444Z",
+    "tags": ["tag1", "tag2"]
     }
     ```
     ## Optimistic Concurrency Control
 
     This endpoint implement optimistic concurrency control to avoid race condition.
     If the record has been updated since the client fetch it, the server will return HTTP status code 412 (precondition failed)
     and client need to redo the operation (fetch data and do update).
```

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_concurrent_record/admin_put_player_public_1624a9.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_concurrent_record/admin_put_player_public_1624a9.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,20 +82,23 @@
     Indicate which party that could modify the game record.
     SERVER: record can be modified by server only.
     CLIENT: record can be modified by client and server.
     2. updatedAt (required: true)
     Time format style: RFC3339
     3. value
     Json
+    4. tags (default: *empty array*, type: array of string)
+    Indicate the tagging for the game record.
     **Request Body Example:**
     ```
     {
     "set_by": "SERVER",
     "value": {},
-    "updatedAt": "2022-03-17T10:42:15.444Z"
+    "updatedAt": "2022-03-17T10:42:15.444Z",
+    "tags": ["tag1", "tag2"]
     }
     ```
 
     ## Optimistic Concurrency Control
 
     This endpoint implement optimistic concurrency control to avoid race condition.
     If the record has been updated since the client fetch it, the server will return HTTP status code 412 (precondition failed)
```

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_concurrent_record/admin_put_player_record_233704.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_concurrent_record/admin_put_player_record_233704.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,20 +82,23 @@
     Indicate which party that could modify the game record.
     SERVER: record can be modified by server only.
     CLIENT: record can be modified by client and server.
     2. updatedAt (required: true)
     Time format style: RFC3339
     3. value
     Json
+    4. tags (default: *empty array*, type: array of string)
+    Indicate the tagging for the game record.
     **Request Body Example:**
     ```
     {
     "set_by": "SERVER",
     "value": {},
-    "updatedAt": "2022-03-17T10:42:15.444Z"
+    "updatedAt": "2022-03-17T10:42:15.444Z",
+    "tags": ["tag1", "tag2"]
     }
     ```
 
     ## Optimistic Concurrency Control
 
     This endpoint implement optimistic concurrency control to avoid race condition.
     If the record has been updated since the client fetch it, the server will return HTTP status code 412 (precondition failed)
```

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_game_binary_record/__init__.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_game_binary_record/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Cloudsave Service."""
 
-__version__ = "3.15.1"
+__version__ = "3.16.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .admin_delete_game_binar_3752d7 import AdminDeleteGameBinaryRecordV1
 from .admin_get_game_binary_r_5df25c import AdminGetGameBinaryRecordV1
```

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_game_binary_record/admin_delete_game_binar_3752d7.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_game_binary_record/admin_delete_game_binar_3752d7.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_game_binary_record/admin_get_game_binary_r_5df25c.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_game_binary_record/admin_get_game_binary_r_5df25c.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_game_binary_record/admin_list_game_binary__f439a9.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_game_binary_record/admin_list_game_binary__f439a9.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_game_binary_record/admin_post_game_binary__ace069.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_game_binary_record/admin_post_game_binary__ace069.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_game_binary_record/admin_post_game_binary__ce9dc6.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_game_binary_record/admin_post_game_binary__ce9dc6.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_game_binary_record/admin_put_game_binary_r_47597f.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_game_binary_record/admin_put_game_binary_r_47597f.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_game_binary_record/admin_put_game_binary_r_a490ed.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_game_binary_record/admin_put_game_binary_r_a490ed.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_game_record/__init__.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_game_record/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Cloudsave Service."""
 
-__version__ = "3.15.1"
+__version__ = "3.16.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .admin_delete_game_recor_636983 import AdminDeleteGameRecordHandlerV1
 from .admin_get_game_record_h_f6ed3a import AdminGetGameRecordHandlerV1
```

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_game_record/admin_delete_game_recor_636983.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_game_record/admin_delete_game_recor_636983.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_game_record/admin_get_game_record_h_f6ed3a.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_game_record/admin_get_game_record_h_f6ed3a.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_game_record/admin_post_game_record__9a2084.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_game_record/admin_post_game_record__9a2084.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,24 +93,27 @@
     Indicate which party that could modify the game record.
     SERVER: record can be modified by server only.
     CLIENT: record can be modified by client and server.
     2. ttl_config (default: *empty*, type: object)
     Indicate the TTL configuration for the game record.
     action:
     - DELETE: record will be deleted after TTL is reached
+    3. tags (default: *empty array*, type: array of string)
+    Indicate the tagging for the game record.
 
     **Request Body Example:**
     ```
     {
     "__META": {
     "set_by": "SERVER",
     "ttl_config": {
     "expires_at": "2026-01-02T15:04:05Z", // should be in RFC3339 format
     "action": "DELETE"
-    }
+    },
+    "tags": ["tag1", "tag2"]
     }
     ...
     }
     ```
 
     Required Permission(s):
         - CLIENT []
```

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_game_record/admin_put_game_record_h_0dd624.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_game_record/admin_put_game_record_h_0dd624.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,24 +81,27 @@
     Indicate which party that could modify the game record.
     SERVER: record can be modified by server only.
     CLIENT: record can be modified by client and server.
     2. ttl_config (default: *empty*, type: object)
     Indicate the TTL configuration for the game record.
     action:
     - DELETE: record will be deleted after TTL is reached
+    3. tags (default: *empty array*, type: array of string)
+    Indicate the tagging for the game record.
 
     **Request Body Example:**
     ```
     {
     "__META": {
     "set_by": "SERVER",
     "ttl_config": {
     "expires_at": "2026-01-02T15:04:05Z", // should be in RFC3339 format
     "action": "DELETE"
-    }
+    },
+    "tags": ["tag1", "tag2"]
     }
     ...
     }
     ```
 
     Required Permission(s):
         - CLIENT []
```

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_game_record/list_game_records_handler_v1.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_game_record/list_game_records_handler_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_binary_record/__init__.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_binary_record/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Cloudsave Service."""
 
-__version__ = "3.15.1"
+__version__ = "3.16.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .admin_delete_player_bin_892eb5 import AdminDeletePlayerBinaryRecordV1
 from .admin_get_player_binary_1076b9 import AdminGetPlayerBinaryRecordV1
```

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_binary_record/admin_delete_player_bin_892eb5.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_binary_record/admin_delete_player_bin_892eb5.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_binary_record/admin_get_player_binary_1076b9.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_binary_record/admin_get_player_binary_1076b9.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_binary_record/admin_list_player_binar_e452ce.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_binary_record/admin_list_player_binar_e452ce.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_binary_record/admin_post_player_binar_e33f40.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_binary_record/admin_post_player_binar_e33f40.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_binary_record/admin_post_player_binar_f1a4e9.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_binary_record/admin_post_player_binar_f1a4e9.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_binary_record/admin_put_player_binary_6424e4.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_binary_record/admin_put_player_binary_6424e4.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_binary_record/admin_put_player_binary_bcf941.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_binary_record/admin_put_player_binary_bcf941.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_record/__init__.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_record/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,20 +4,22 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Cloudsave Service."""
 
-__version__ = "3.15.1"
+__version__ = "3.16.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
+from .admin_bulk_get_player_r_82c596 import AdminBulkGetPlayerRecordsByUserIDsHandlerV1
+from .admin_bulk_put_player_r_27d5a1 import AdminBulkPutPlayerRecordsByKeyHandlerV1
 from .admin_delete_player_pub_f11fd7 import AdminDeletePlayerPublicRecordHandlerV1
 from .admin_delete_player_rec_168241 import AdminDeletePlayerRecordHandlerV1
 from .admin_get_player_public_f015b6 import AdminGetPlayerPublicRecordHandlerV1
 from .admin_get_player_record_b37faa import AdminGetPlayerRecordHandlerV1
 from .admin_get_player_record_f4a5eb import AdminGetPlayerRecordsHandlerV1
 from .admin_get_player_record_d622c9 import AdminGetPlayerRecordSizeHandlerV1
 from .admin_post_player_publi_98e39e import AdminPostPlayerPublicRecordHandlerV1
```

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_record/admin_delete_player_pub_f11fd7.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_record/admin_delete_player_pub_f11fd7.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_record/admin_delete_player_rec_168241.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_record/admin_delete_player_rec_168241.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_record/admin_get_player_public_f015b6.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_record/admin_get_player_public_f015b6.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_record/admin_get_player_record_b37faa.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_record/admin_get_player_record_b37faa.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_record/admin_get_player_record_d622c9.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_record/admin_get_player_record_d622c9.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_record/admin_get_player_record_f4a5eb.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_record/admin_get_player_record_f4a5eb.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_record/admin_post_player_publi_98e39e.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_record/admin_post_player_publi_98e39e.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_record/admin_post_player_recor_6a96c8.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_record/admin_post_player_recor_6a96c8.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,21 +91,24 @@
     **Metadata List:**
     1. set_by (default: CLIENT, type: string)
     Indicate which party that could modify the game record.
     SERVER: record can be modified by server only.
     CLIENT: record can be modified by client and server.
     2. is_public (default: false, type: bool)
     Indicate whether the player record is a public record or not.
+    3. tags (default: *empty array*, type: array of string)
+    Indicate the tagging for the game record.
 
     **Request Body Example:**
     ```
     {
     "__META": {
     "set_by": "SERVER",
-    "is_public": true
+    "is_public": true,
+    "tags": ["tag1", "tag2"]
     }
     ...
     }
     ```
 
     Required Permission(s):
         - CLIENT []
```

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_record/admin_put_player_public_819faf.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_record/admin_put_player_public_819faf.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_record/admin_put_player_record_253e92.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_record/admin_put_player_record_253e92.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         namespace: (namespace) REQUIRED str in path
 
         user_id: (userId) REQUIRED str in path
 
     Responses:
         200: OK - List[ModelsBulkUpdatePlayerRecordResponse] (OK)
 
-        400: Bad Request - ModelsResponseError (18353: invalid request body | 18356: invalid request body: size of the request body must be less than [%d]MB | 18354: records amount exceeded max limit | 18355: unable to marshal request body | 18355: unable to marshal request body)
+        400: Bad Request - ModelsResponseError (18353: invalid request body | 18356: invalid request body: size of the request body must be less than [%d]MB | 18354: records amount exceeded max limit | 18355: unable to marshal request body)
 
         401: Unauthorized - ModelsResponseError (20001: unauthorized access)
 
         403: Forbidden - ModelsResponseError (20013: insufficient permission)
     """
 
     # region fields
@@ -190,15 +190,15 @@
         Union[None, List[ModelsBulkUpdatePlayerRecordResponse]],
         Union[None, HttpResponse, ModelsResponseError],
     ]:
         """Parse the given response.
 
         200: OK - List[ModelsBulkUpdatePlayerRecordResponse] (OK)
 
-        400: Bad Request - ModelsResponseError (18353: invalid request body | 18356: invalid request body: size of the request body must be less than [%d]MB | 18354: records amount exceeded max limit | 18355: unable to marshal request body | 18355: unable to marshal request body)
+        400: Bad Request - ModelsResponseError (18353: invalid request body | 18356: invalid request body: size of the request body must be less than [%d]MB | 18354: records amount exceeded max limit | 18355: unable to marshal request body)
 
         401: Unauthorized - ModelsResponseError (20001: unauthorized access)
 
         403: Forbidden - ModelsResponseError (20013: insufficient permission)
 
         ---: HttpResponse (Undocumented Response)
```

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_record/admin_put_player_record_a8195d.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_record/admin_put_player_record_a8195d.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,21 +79,24 @@
     **Metadata List:**
     1. set_by (default: CLIENT, type: string)
     Indicate which party that could modify the game record.
     SERVER: record can be modified by server only.
     CLIENT: record can be modified by client and server.
     2. is_public (default: false, type: bool)
     Indicate whether the player record is a public record or not.
+    3. tags (default: *empty array*, type: array of string)
+    Indicate the tagging for the game record.
 
     **Request Body Example:**
     ```
     {
     "__META": {
     "set_by": "SERVER",
-    "is_public": true
+    "is_public": true,
+    "tags": ["tag1", "tag2"]
     }
     ...
     }
     ```
 
     Required Permission(s):
         - CLIENT []
```

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_record/admin_retrieve_player_records.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_record/admin_retrieve_player_records.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_record/bulk_get_player_record__4627ec.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_record/bulk_get_player_record__4627ec.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_record/list_player_record_handler_v1.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_record/list_player_record_handler_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_record/__init__.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_record/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Cloudsave Service."""
 
-__version__ = "3.15.1"
+__version__ = "3.16.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .admin_bulk_get_admin_ga_c5c529 import AdminBulkGetAdminGameRecordV1
 from .admin_bulk_get_admin_pl_b8e62a import AdminBulkGetAdminPlayerRecordV1
```

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_record/admin_bulk_get_admin_ga_c5c529.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_record/admin_bulk_get_admin_ga_c5c529.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_record/admin_bulk_get_admin_pl_b8e62a.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_record/admin_bulk_get_admin_pl_b8e62a.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_record/admin_delete_admin_game_1f080f.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_record/admin_delete_admin_game_1f080f.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_record/admin_delete_admin_play_632fe7.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_record/admin_delete_admin_play_632fe7.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_record/admin_get_admin_game_record_v1.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_record/admin_get_admin_game_record_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_record/admin_get_admin_player__37ad38.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_record/admin_get_admin_player__37ad38.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_record/admin_list_admin_game_r_476bfb.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_record/admin_list_admin_game_r_476bfb.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_record/admin_list_admin_user_r_83dd7a.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_record/admin_list_admin_user_r_83dd7a.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_record/admin_post_admin_game_r_e8f678.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_record/admin_put_admin_game_record_v1.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,64 +30,73 @@
 from accelbyte_py_sdk.core import HttpResponse
 
 from ...models import ModelsAdminGameRecordRequest
 from ...models import ModelsAdminGameRecordResponse
 from ...models import ModelsResponseError
 
 
-class AdminPostAdminGameRecordV1(Operation):
-    """Create or append admin game record (adminPostAdminGameRecordV1)
+class AdminPutAdminGameRecordV1(Operation):
+    """Create or replace admin game record (adminPutAdminGameRecordV1)
 
     ## Description
 
-    This endpoints will create new admin game record or append the existing admin game record.
+    This endpoints will create new admin game record or replace the existing admin game record.
 
     **Append example:**
 
-    Example 1
+    Example
     - Existing JSON:
 
     `{ "data1": "value" }`
 
     - New JSON:
 
     `{ "data2": "new value" }`
 
     - Result:
 
-    `{ "data1": "value", "data2": "new value" }`
-
-
-    Example 2
-    - Existing JSON:
-
-    `{ "data1": { "data2": "value" }`
-
-    - New JSON:
-
-    `{ "data1": { "data3": "new value" }`
-
-    - Result:
+    `{ "data2": "new value" }`
 
-    `{ "data1": { "data2": "value", "data3": "new value" }`
 
 
     ## Restriction
     This is the restriction of Key Naming for the record:
     1. Cannot use **"."** as the key name
     - `{ "data.2": "value" }`
     2. Cannot use **"$"** as the prefix in key names
     - `{ "$data": "value" }`
     3. Cannot use empty string in key names
     - `{ "": "value" }`
 
+
+    ## Record Metadata
+
+    Metadata allows user to define the behaviour of the record.
+    Metadata can be defined in request body with field name **__META**.
+    When creating record, if **__META** field is not defined, the metadata value will use the default value.
+    When updating record, if **__META** field is not defined, the existing metadata value will stay as is.
+
+    **Metadata List:**
+    1. tags (default: *empty array*, type: array of string)
+    Indicate the tagging for the admin record.
+
+    **Request Body Example:**
+    ```
+    {
+    "__META": {
+    "tags": ["tag1", "tag2"]
+    }
+    ...
+    }
+    ```
+
     Properties:
         url: /cloudsave/v1/admin/namespaces/{namespace}/adminrecords/{key}
 
-        method: POST
+        method: PUT
 
         tags: ["AdminRecord"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
@@ -96,29 +105,29 @@
         body: (body) REQUIRED ModelsAdminGameRecordRequest in body
 
         key: (key) REQUIRED str in path
 
         namespace: (namespace) REQUIRED str in path
 
     Responses:
-        201: Created - ModelsAdminGameRecordResponse (Record in namespace-level saved)
+        200: OK - ModelsAdminGameRecordResponse (Record saved)
 
-        400: Bad Request - ModelsResponseError (18134: invalid request body | 20002: validation error | 18136: invalid request body: size of the request body must be less than [%d]MB)
+        400: Bad Request - ModelsResponseError (18144: invalid request body | 20002: validation error | 18146: invalid request body: size of the request body must be less than [%d]MB)
 
         401: Unauthorized - ModelsResponseError (20001: unauthorized access)
 
         403: Forbidden - ModelsResponseError (20013: insufficient permission)
 
-        500: Internal Server Error - ModelsResponseError (18135: unable to marshal request body | 20000: internal server error | 18013: unable to save record | 18165: unable to decode record)
+        500: Internal Server Error - ModelsResponseError (18145: unable to marshal request body | 20000: internal server error | 18164: unable to decode record | 18147: unable to update record)
     """
 
     # region fields
 
     _url: str = "/cloudsave/v1/admin/namespaces/{namespace}/adminrecords/{key}"
-    _method: str = "POST"
+    _method: str = "PUT"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
     body: ModelsAdminGameRecordRequest  # REQUIRED in [body]
     key: str  # REQUIRED in [path]
@@ -185,23 +194,23 @@
 
     # endregion is/has methods
 
     # region with_x methods
 
     def with_body(
         self, value: ModelsAdminGameRecordRequest
-    ) -> AdminPostAdminGameRecordV1:
+    ) -> AdminPutAdminGameRecordV1:
         self.body = value
         return self
 
-    def with_key(self, value: str) -> AdminPostAdminGameRecordV1:
+    def with_key(self, value: str) -> AdminPutAdminGameRecordV1:
         self.key = value
         return self
 
-    def with_namespace(self, value: str) -> AdminPostAdminGameRecordV1:
+    def with_namespace(self, value: str) -> AdminPutAdminGameRecordV1:
         self.namespace = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
@@ -230,38 +239,38 @@
         self, code: int, content_type: str, content: Any
     ) -> Tuple[
         Union[None, ModelsAdminGameRecordResponse],
         Union[None, HttpResponse, ModelsResponseError],
     ]:
         """Parse the given response.
 
-        201: Created - ModelsAdminGameRecordResponse (Record in namespace-level saved)
+        200: OK - ModelsAdminGameRecordResponse (Record saved)
 
-        400: Bad Request - ModelsResponseError (18134: invalid request body | 20002: validation error | 18136: invalid request body: size of the request body must be less than [%d]MB)
+        400: Bad Request - ModelsResponseError (18144: invalid request body | 20002: validation error | 18146: invalid request body: size of the request body must be less than [%d]MB)
 
         401: Unauthorized - ModelsResponseError (20001: unauthorized access)
 
         403: Forbidden - ModelsResponseError (20013: insufficient permission)
 
-        500: Internal Server Error - ModelsResponseError (18135: unable to marshal request body | 20000: internal server error | 18013: unable to save record | 18165: unable to decode record)
+        500: Internal Server Error - ModelsResponseError (18145: unable to marshal request body | 20000: internal server error | 18164: unable to decode record | 18147: unable to update record)
 
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
+        if code == 200:
             return ModelsAdminGameRecordResponse.create_from_dict(content), None
         if code == 400:
             return None, ModelsResponseError.create_from_dict(content)
         if code == 401:
             return None, ModelsResponseError.create_from_dict(content)
         if code == 403:
             return None, ModelsResponseError.create_from_dict(content)
@@ -275,27 +284,27 @@
     # endregion response methods
 
     # region static methods
 
     @classmethod
     def create(
         cls, body: ModelsAdminGameRecordRequest, key: str, namespace: str, **kwargs
-    ) -> AdminPostAdminGameRecordV1:
+    ) -> AdminPutAdminGameRecordV1:
         instance = cls()
         instance.body = body
         instance.key = key
         instance.namespace = namespace
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> AdminPostAdminGameRecordV1:
+    ) -> AdminPutAdminGameRecordV1:
         instance = cls()
         if "body" in dict_ and dict_["body"] is not None:
             instance.body = ModelsAdminGameRecordRequest.create_from_dict(
                 dict_["body"], include_empty=include_empty
             )
         elif include_empty:
             instance.body = ModelsAdminGameRecordRequest()
```

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_record/admin_post_player_admin_b138ee.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_record/post_player_record_handler_v1.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,25 +25,26 @@
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
-from ...models import ModelsAdminPlayerRecordRequest
-from ...models import ModelsAdminPlayerRecordResponse
+from ...models import ModelsPlayerRecordRequest
+from ...models import ModelsPlayerRecordResponse
 from ...models import ModelsResponseError
 
 
-class AdminPostPlayerAdminRecordV1(Operation):
-    """Create or append admin player record (adminPostPlayerAdminRecordV1)
+class PostPlayerRecordHandlerV1(Operation):
+    """Create or append player record (postPlayerRecordHandlerV1)
 
     ## Description
 
-    This endpoints will create new admin player record or append the existing admin game record.
+    This endpoints will create new player record or append the existing player record.
+    Only user that own the existing player record could modify.
 
     **Append example:**
 
     Example 1
     - Existing JSON:
 
     `{ "data1": "value" }`
@@ -76,59 +77,79 @@
     1. Cannot use **"."** as the key name
     - `{ "data.2": "value" }`
     2. Cannot use **"$"** as the prefix in key names
     - `{ "$data": "value" }`
     3. Cannot use empty string in key names
     - `{ "": "value" }`
 
+
+    ## Record Metadata
+
+    Metadata allows user to define the behaviour of the record.
+    Metadata can be defined in request body with field name **__META**.
+    When creating record, if **__META** field is not defined, the metadata value will use the default value.
+    When updating record, if **__META** field is not defined, the existing metadata value will stay as is.
+
+    **Metadata List:**
+    1. is_public (default: false, type: bool)
+    Indicate whether the player record is a public record or not.
+
+    **Request Body Example:**
+    ```
+    {
+    "__META": {
+    "is_public": true
+    }
+    ...
+    }
+    ```
+
     Properties:
-        url: /cloudsave/v1/admin/namespaces/{namespace}/users/{userId}/adminrecords/{key}
+        url: /cloudsave/v1/namespaces/{namespace}/users/{userId}/records/{key}
 
         method: POST
 
-        tags: ["AdminRecord"]
+        tags: ["PublicPlayerRecord"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
-        body: (body) REQUIRED ModelsAdminPlayerRecordRequest in body
+        body: (body) REQUIRED ModelsPlayerRecordRequest in body
 
         key: (key) REQUIRED str in path
 
         namespace: (namespace) REQUIRED str in path
 
         user_id: (userId) REQUIRED str in path
 
     Responses:
-        201: Created - ModelsAdminPlayerRecordResponse (Record in user-level saved)
+        201: Created - ModelsPlayerRecordResponse (Record saved)
 
-        400: Bad Request - ModelsResponseError (18150: invalid request body | 20002: validation error)
+        400: Bad Request - ModelsResponseError (18201: invalid record operator, expect [%s] but actual [%s] | 18030: invalid request body | 20002: validation error | 18060: invalid request body)
 
         401: Unauthorized - ModelsResponseError (20001: unauthorized access)
 
-        403: Forbidden - ModelsResponseError (20013: insufficient permission)
+        403: Forbidden - ModelsResponseError (18035: post action is forbidden on other user's record | 20013: insufficient permission)
 
-        500: Internal Server Error - ModelsResponseError (20000: internal server error | 18033: unable to save record | 18163: unable to decode record)
+        500: Internal Server Error - ModelsResponseError (20000: internal server error | 18033: unable to save record | 18005: unable to decode record)
     """
 
     # region fields
 
-    _url: str = (
-        "/cloudsave/v1/admin/namespaces/{namespace}/users/{userId}/adminrecords/{key}"
-    )
+    _url: str = "/cloudsave/v1/namespaces/{namespace}/users/{userId}/records/{key}"
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
-    body: ModelsAdminPlayerRecordRequest  # REQUIRED in [body]
+    body: ModelsPlayerRecordRequest  # REQUIRED in [body]
     key: str  # REQUIRED in [path]
     namespace: str  # REQUIRED in [path]
     user_id: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
@@ -190,42 +211,40 @@
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_body(
-        self, value: ModelsAdminPlayerRecordRequest
-    ) -> AdminPostPlayerAdminRecordV1:
+    def with_body(self, value: ModelsPlayerRecordRequest) -> PostPlayerRecordHandlerV1:
         self.body = value
         return self
 
-    def with_key(self, value: str) -> AdminPostPlayerAdminRecordV1:
+    def with_key(self, value: str) -> PostPlayerRecordHandlerV1:
         self.key = value
         return self
 
-    def with_namespace(self, value: str) -> AdminPostPlayerAdminRecordV1:
+    def with_namespace(self, value: str) -> PostPlayerRecordHandlerV1:
         self.namespace = value
         return self
 
-    def with_user_id(self, value: str) -> AdminPostPlayerAdminRecordV1:
+    def with_user_id(self, value: str) -> PostPlayerRecordHandlerV1:
         self.user_id = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
         if hasattr(self, "body") and self.body:
             result["body"] = self.body.to_dict(include_empty=include_empty)
         elif include_empty:
-            result["body"] = ModelsAdminPlayerRecordRequest()
+            result["body"] = ModelsPlayerRecordRequest()
         if hasattr(self, "key") and self.key:
             result["key"] = str(self.key)
         elif include_empty:
             result["key"] = ""
         if hasattr(self, "namespace") and self.namespace:
             result["namespace"] = str(self.namespace)
         elif include_empty:
@@ -240,28 +259,28 @@
 
     # region response methods
 
     # noinspection PyMethodMayBeStatic
     def parse_response(
         self, code: int, content_type: str, content: Any
     ) -> Tuple[
-        Union[None, ModelsAdminPlayerRecordResponse],
+        Union[None, ModelsPlayerRecordResponse],
         Union[None, HttpResponse, ModelsResponseError],
     ]:
         """Parse the given response.
 
-        201: Created - ModelsAdminPlayerRecordResponse (Record in user-level saved)
+        201: Created - ModelsPlayerRecordResponse (Record saved)
 
-        400: Bad Request - ModelsResponseError (18150: invalid request body | 20002: validation error)
+        400: Bad Request - ModelsResponseError (18201: invalid record operator, expect [%s] but actual [%s] | 18030: invalid request body | 20002: validation error | 18060: invalid request body)
 
         401: Unauthorized - ModelsResponseError (20001: unauthorized access)
 
-        403: Forbidden - ModelsResponseError (20013: insufficient permission)
+        403: Forbidden - ModelsResponseError (18035: post action is forbidden on other user's record | 20013: insufficient permission)
 
-        500: Internal Server Error - ModelsResponseError (20000: internal server error | 18033: unable to save record | 18163: unable to decode record)
+        500: Internal Server Error - ModelsResponseError (20000: internal server error | 18033: unable to save record | 18005: unable to decode record)
 
         ---: HttpResponse (Undocumented Response)
 
         ---: HttpResponse (Unexpected Content-Type Error)
 
         ---: HttpResponse (Unhandled Error)
         """
@@ -269,15 +288,15 @@
             code=code, content_type=content_type, content=content
         )
         if error is not None:
             return None, None if error.is_no_content() else error
         code, content_type, content = pre_processed_response
 
         if code == 201:
-            return ModelsAdminPlayerRecordResponse.create_from_dict(content), None
+            return ModelsPlayerRecordResponse.create_from_dict(content), None
         if code == 400:
             return None, ModelsResponseError.create_from_dict(content)
         if code == 401:
             return None, ModelsResponseError.create_from_dict(content)
         if code == 403:
             return None, ModelsResponseError.create_from_dict(content)
         if code == 500:
@@ -290,40 +309,40 @@
     # endregion response methods
 
     # region static methods
 
     @classmethod
     def create(
         cls,
-        body: ModelsAdminPlayerRecordRequest,
+        body: ModelsPlayerRecordRequest,
         key: str,
         namespace: str,
         user_id: str,
         **kwargs,
-    ) -> AdminPostPlayerAdminRecordV1:
+    ) -> PostPlayerRecordHandlerV1:
         instance = cls()
         instance.body = body
         instance.key = key
         instance.namespace = namespace
         instance.user_id = user_id
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> AdminPostPlayerAdminRecordV1:
+    ) -> PostPlayerRecordHandlerV1:
         instance = cls()
         if "body" in dict_ and dict_["body"] is not None:
-            instance.body = ModelsAdminPlayerRecordRequest.create_from_dict(
+            instance.body = ModelsPlayerRecordRequest.create_from_dict(
                 dict_["body"], include_empty=include_empty
             )
         elif include_empty:
-            instance.body = ModelsAdminPlayerRecordRequest()
+            instance.body = ModelsPlayerRecordRequest()
         if "key" in dict_ and dict_["key"] is not None:
             instance.key = str(dict_["key"])
         elif include_empty:
             instance.key = ""
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
         elif include_empty:
```

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_record/admin_put_admin_game_record_v1.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_record/admin_put_admin_player__6ed45f.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,27 +25,28 @@
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
-from ...models import ModelsAdminGameRecordRequest
-from ...models import ModelsAdminGameRecordResponse
+from ...models import ModelsAdminPlayerRecordRequest
+from ...models import ModelsAdminPlayerRecordResponse
 from ...models import ModelsResponseError
 
 
-class AdminPutAdminGameRecordV1(Operation):
-    """Create or replace admin game record (adminPutAdminGameRecordV1)
+class AdminPutAdminPlayerRecordV1(Operation):
+    """Create or replace admin player record (adminPutAdminPlayerRecordV1)
 
     ## Description
 
-    This endpoints will create new admin game record or replace the existing admin game record.
+    This endpoints will create new admin player record or replace the existing admin player record.
 
-    **Append example:**
+    **Replace behaviour:**
+    The existing value will be replaced completely with the new value.
 
     Example
     - Existing JSON:
 
     `{ "data1": "value" }`
 
     - New JSON:
@@ -63,57 +64,84 @@
     1. Cannot use **"."** as the key name
     - `{ "data.2": "value" }`
     2. Cannot use **"$"** as the prefix in key names
     - `{ "$data": "value" }`
     3. Cannot use empty string in key names
     - `{ "": "value" }`
 
+
+    ## Record Metadata
+
+    Metadata allows user to define the behaviour of the record.
+    Metadata can be defined in request body with field name **__META**.
+    When creating record, if **__META** field is not defined, the metadata value will use the default value.
+    When updating record, if **__META** field is not defined, the existing metadata value will stay as is.
+
+    **Metadata List:**
+    1. tags (default: *empty array*, type: array of string)
+    Indicate the tagging for the admin record.
+
+    **Request Body Example:**
+    ```
+    {
+    "__META": {
+    "tags": ["tag1", "tag2"]
+    }
+    ...
+    }
+    ```
+
     Properties:
-        url: /cloudsave/v1/admin/namespaces/{namespace}/adminrecords/{key}
+        url: /cloudsave/v1/admin/namespaces/{namespace}/users/{userId}/adminrecords/{key}
 
         method: PUT
 
         tags: ["AdminRecord"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
-        body: (body) REQUIRED ModelsAdminGameRecordRequest in body
+        body: (body) REQUIRED ModelsAdminPlayerRecordRequest in body
 
         key: (key) REQUIRED str in path
 
         namespace: (namespace) REQUIRED str in path
 
+        user_id: (userId) REQUIRED str in path
+
     Responses:
-        200: OK - ModelsAdminGameRecordResponse (Record saved)
+        200: OK - ModelsAdminPlayerRecordResponse (Record in user-level saved)
 
-        400: Bad Request - ModelsResponseError (18144: invalid request body | 20002: validation error | 18146: invalid request body: size of the request body must be less than [%d]MB)
+        400: Bad Request - ModelsResponseError (18156: invalid request body | 20002: validation error)
 
         401: Unauthorized - ModelsResponseError (20001: unauthorized access)
 
         403: Forbidden - ModelsResponseError (20013: insufficient permission)
 
-        500: Internal Server Error - ModelsResponseError (18145: unable to marshal request body | 20000: internal server error | 18164: unable to decode record | 18147: unable to update record)
+        500: Internal Server Error - ModelsResponseError (20000: internal server error | 18061: unable to update record | 18162: unable to decode record)
     """
 
     # region fields
 
-    _url: str = "/cloudsave/v1/admin/namespaces/{namespace}/adminrecords/{key}"
+    _url: str = (
+        "/cloudsave/v1/admin/namespaces/{namespace}/users/{userId}/adminrecords/{key}"
+    )
     _method: str = "PUT"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
-    body: ModelsAdminGameRecordRequest  # REQUIRED in [body]
+    body: ModelsAdminPlayerRecordRequest  # REQUIRED in [body]
     key: str  # REQUIRED in [path]
     namespace: str  # REQUIRED in [path]
+    user_id: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
@@ -160,80 +188,90 @@
 
     def get_path_params(self) -> dict:
         result = {}
         if hasattr(self, "key"):
             result["key"] = self.key
         if hasattr(self, "namespace"):
             result["namespace"] = self.namespace
+        if hasattr(self, "user_id"):
+            result["userId"] = self.user_id
         return result
 
     # endregion get_x_params methods
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
     def with_body(
-        self, value: ModelsAdminGameRecordRequest
-    ) -> AdminPutAdminGameRecordV1:
+        self, value: ModelsAdminPlayerRecordRequest
+    ) -> AdminPutAdminPlayerRecordV1:
         self.body = value
         return self
 
-    def with_key(self, value: str) -> AdminPutAdminGameRecordV1:
+    def with_key(self, value: str) -> AdminPutAdminPlayerRecordV1:
         self.key = value
         return self
 
-    def with_namespace(self, value: str) -> AdminPutAdminGameRecordV1:
+    def with_namespace(self, value: str) -> AdminPutAdminPlayerRecordV1:
         self.namespace = value
         return self
 
+    def with_user_id(self, value: str) -> AdminPutAdminPlayerRecordV1:
+        self.user_id = value
+        return self
+
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
         if hasattr(self, "body") and self.body:
             result["body"] = self.body.to_dict(include_empty=include_empty)
         elif include_empty:
-            result["body"] = ModelsAdminGameRecordRequest()
+            result["body"] = ModelsAdminPlayerRecordRequest()
         if hasattr(self, "key") and self.key:
             result["key"] = str(self.key)
         elif include_empty:
             result["key"] = ""
         if hasattr(self, "namespace") and self.namespace:
             result["namespace"] = str(self.namespace)
         elif include_empty:
             result["namespace"] = ""
+        if hasattr(self, "user_id") and self.user_id:
+            result["userId"] = str(self.user_id)
+        elif include_empty:
+            result["userId"] = ""
         return result
 
     # endregion to methods
 
     # region response methods
 
     # noinspection PyMethodMayBeStatic
     def parse_response(
         self, code: int, content_type: str, content: Any
     ) -> Tuple[
-        Union[None, ModelsAdminGameRecordResponse],
+        Union[None, ModelsAdminPlayerRecordResponse],
         Union[None, HttpResponse, ModelsResponseError],
     ]:
         """Parse the given response.
 
-        200: OK - ModelsAdminGameRecordResponse (Record saved)
+        200: OK - ModelsAdminPlayerRecordResponse (Record in user-level saved)
 
-        400: Bad Request - ModelsResponseError (18144: invalid request body | 20002: validation error | 18146: invalid request body: size of the request body must be less than [%d]MB)
+        400: Bad Request - ModelsResponseError (18156: invalid request body | 20002: validation error)
 
         401: Unauthorized - ModelsResponseError (20001: unauthorized access)
 
         403: Forbidden - ModelsResponseError (20013: insufficient permission)
 
-        500: Internal Server Error - ModelsResponseError (18145: unable to marshal request body | 20000: internal server error | 18164: unable to decode record | 18147: unable to update record)
+        500: Internal Server Error - ModelsResponseError (20000: internal server error | 18061: unable to update record | 18162: unable to decode record)
 
         ---: HttpResponse (Undocumented Response)
 
         ---: HttpResponse (Unexpected Content-Type Error)
 
         ---: HttpResponse (Unhandled Error)
         """
@@ -241,15 +279,15 @@
             code=code, content_type=content_type, content=content
         )
         if error is not None:
             return None, None if error.is_no_content() else error
         code, content_type, content = pre_processed_response
 
         if code == 200:
-            return ModelsAdminGameRecordResponse.create_from_dict(content), None
+            return ModelsAdminPlayerRecordResponse.create_from_dict(content), None
         if code == 400:
             return None, ModelsResponseError.create_from_dict(content)
         if code == 401:
             return None, ModelsResponseError.create_from_dict(content)
         if code == 403:
             return None, ModelsResponseError.create_from_dict(content)
         if code == 500:
@@ -261,55 +299,67 @@
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
     def create(
-        cls, body: ModelsAdminGameRecordRequest, key: str, namespace: str, **kwargs
-    ) -> AdminPutAdminGameRecordV1:
+        cls,
+        body: ModelsAdminPlayerRecordRequest,
+        key: str,
+        namespace: str,
+        user_id: str,
+        **kwargs,
+    ) -> AdminPutAdminPlayerRecordV1:
         instance = cls()
         instance.body = body
         instance.key = key
         instance.namespace = namespace
+        instance.user_id = user_id
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> AdminPutAdminGameRecordV1:
+    ) -> AdminPutAdminPlayerRecordV1:
         instance = cls()
         if "body" in dict_ and dict_["body"] is not None:
-            instance.body = ModelsAdminGameRecordRequest.create_from_dict(
+            instance.body = ModelsAdminPlayerRecordRequest.create_from_dict(
                 dict_["body"], include_empty=include_empty
             )
         elif include_empty:
-            instance.body = ModelsAdminGameRecordRequest()
+            instance.body = ModelsAdminPlayerRecordRequest()
         if "key" in dict_ and dict_["key"] is not None:
             instance.key = str(dict_["key"])
         elif include_empty:
             instance.key = ""
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
         elif include_empty:
             instance.namespace = ""
+        if "userId" in dict_ and dict_["userId"] is not None:
+            instance.user_id = str(dict_["userId"])
+        elif include_empty:
+            instance.user_id = ""
         return instance
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
             "body": "body",
             "key": "key",
             "namespace": "namespace",
+            "userId": "user_id",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
             "body": True,
             "key": True,
             "namespace": True,
+            "userId": True,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_record/admin_put_admin_player__6ed45f.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_record/put_player_record_handler_v1.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,25 +25,26 @@
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
-from ...models import ModelsAdminPlayerRecordRequest
-from ...models import ModelsAdminPlayerRecordResponse
+from ...models import ModelsPlayerRecordRequest
+from ...models import ModelsPlayerRecordResponse
 from ...models import ModelsResponseError
 
 
-class AdminPutAdminPlayerRecordV1(Operation):
-    """Create or replace admin player record (adminPutAdminPlayerRecordV1)
+class PutPlayerRecordHandlerV1(Operation):
+    """Create or replace player record (putPlayerRecordHandlerV1)
 
     ## Description
 
-    This endpoints will create new admin player record or replace the existing admin player record.
+    This endpoints will create new player record or replace the existing player record.
+    Only user that own the existing player record could modify it.
 
     **Replace behaviour:**
     The existing value will be replaced completely with the new value.
 
     Example
     - Existing JSON:
 
@@ -64,59 +65,79 @@
     1. Cannot use **"."** as the key name
     - `{ "data.2": "value" }`
     2. Cannot use **"$"** as the prefix in key names
     - `{ "$data": "value" }`
     3. Cannot use empty string in key names
     - `{ "": "value" }`
 
+
+    ## Record Metadata
+
+    Metadata allows user to define the behaviour of the record.
+    Metadata can be defined in request body with field name **__META**.
+    When creating record, if **__META** field is not defined, the metadata value will use the default value.
+    When updating record, if **__META** field is not defined, the existing metadata value will stay as is.
+
+    **Metadata List:**
+    1. is_public (default: false, type: bool)
+    Indicate whether the player record is a public record or not.
+
+    **Request Body Example:**
+    ```
+    {
+    "__META": {
+    "is_public": true
+    }
+    ...
+    }
+    ```
+
     Properties:
-        url: /cloudsave/v1/admin/namespaces/{namespace}/users/{userId}/adminrecords/{key}
+        url: /cloudsave/v1/namespaces/{namespace}/users/{userId}/records/{key}
 
         method: PUT
 
-        tags: ["AdminRecord"]
+        tags: ["PublicPlayerRecord"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
-        body: (body) REQUIRED ModelsAdminPlayerRecordRequest in body
+        body: (body) REQUIRED ModelsPlayerRecordRequest in body
 
         key: (key) REQUIRED str in path
 
         namespace: (namespace) REQUIRED str in path
 
         user_id: (userId) REQUIRED str in path
 
     Responses:
-        200: OK - ModelsAdminPlayerRecordResponse (Record in user-level saved)
+        200: OK - ModelsPlayerRecordResponse (Record saved)
 
-        400: Bad Request - ModelsResponseError (18156: invalid request body | 20002: validation error)
+        400: Bad Request - ModelsResponseError (18201: invalid record operator, expect [%s] but actual [%s] | 18060: invalid request body | 20002: validation error)
 
         401: Unauthorized - ModelsResponseError (20001: unauthorized access)
 
-        403: Forbidden - ModelsResponseError (20013: insufficient permission)
+        403: Forbidden - ModelsResponseError (18063: put action is forbidden on other user's record | 20013: insufficient permission)
 
-        500: Internal Server Error - ModelsResponseError (20000: internal server error | 18061: unable to update record | 18162: unable to decode record)
+        500: Internal Server Error - ModelsResponseError (20000: internal server error | 18061: unable to update record | 18005: unable to decode record)
     """
 
     # region fields
 
-    _url: str = (
-        "/cloudsave/v1/admin/namespaces/{namespace}/users/{userId}/adminrecords/{key}"
-    )
+    _url: str = "/cloudsave/v1/namespaces/{namespace}/users/{userId}/records/{key}"
     _method: str = "PUT"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
-    body: ModelsAdminPlayerRecordRequest  # REQUIRED in [body]
+    body: ModelsPlayerRecordRequest  # REQUIRED in [body]
     key: str  # REQUIRED in [path]
     namespace: str  # REQUIRED in [path]
     user_id: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
@@ -178,42 +199,40 @@
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_body(
-        self, value: ModelsAdminPlayerRecordRequest
-    ) -> AdminPutAdminPlayerRecordV1:
+    def with_body(self, value: ModelsPlayerRecordRequest) -> PutPlayerRecordHandlerV1:
         self.body = value
         return self
 
-    def with_key(self, value: str) -> AdminPutAdminPlayerRecordV1:
+    def with_key(self, value: str) -> PutPlayerRecordHandlerV1:
         self.key = value
         return self
 
-    def with_namespace(self, value: str) -> AdminPutAdminPlayerRecordV1:
+    def with_namespace(self, value: str) -> PutPlayerRecordHandlerV1:
         self.namespace = value
         return self
 
-    def with_user_id(self, value: str) -> AdminPutAdminPlayerRecordV1:
+    def with_user_id(self, value: str) -> PutPlayerRecordHandlerV1:
         self.user_id = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
         if hasattr(self, "body") and self.body:
             result["body"] = self.body.to_dict(include_empty=include_empty)
         elif include_empty:
-            result["body"] = ModelsAdminPlayerRecordRequest()
+            result["body"] = ModelsPlayerRecordRequest()
         if hasattr(self, "key") and self.key:
             result["key"] = str(self.key)
         elif include_empty:
             result["key"] = ""
         if hasattr(self, "namespace") and self.namespace:
             result["namespace"] = str(self.namespace)
         elif include_empty:
@@ -228,28 +247,28 @@
 
     # region response methods
 
     # noinspection PyMethodMayBeStatic
     def parse_response(
         self, code: int, content_type: str, content: Any
     ) -> Tuple[
-        Union[None, ModelsAdminPlayerRecordResponse],
+        Union[None, ModelsPlayerRecordResponse],
         Union[None, HttpResponse, ModelsResponseError],
     ]:
         """Parse the given response.
 
-        200: OK - ModelsAdminPlayerRecordResponse (Record in user-level saved)
+        200: OK - ModelsPlayerRecordResponse (Record saved)
 
-        400: Bad Request - ModelsResponseError (18156: invalid request body | 20002: validation error)
+        400: Bad Request - ModelsResponseError (18201: invalid record operator, expect [%s] but actual [%s] | 18060: invalid request body | 20002: validation error)
 
         401: Unauthorized - ModelsResponseError (20001: unauthorized access)
 
-        403: Forbidden - ModelsResponseError (20013: insufficient permission)
+        403: Forbidden - ModelsResponseError (18063: put action is forbidden on other user's record | 20013: insufficient permission)
 
-        500: Internal Server Error - ModelsResponseError (20000: internal server error | 18061: unable to update record | 18162: unable to decode record)
+        500: Internal Server Error - ModelsResponseError (20000: internal server error | 18061: unable to update record | 18005: unable to decode record)
 
         ---: HttpResponse (Undocumented Response)
 
         ---: HttpResponse (Unexpected Content-Type Error)
 
         ---: HttpResponse (Unhandled Error)
         """
@@ -257,15 +276,15 @@
             code=code, content_type=content_type, content=content
         )
         if error is not None:
             return None, None if error.is_no_content() else error
         code, content_type, content = pre_processed_response
 
         if code == 200:
-            return ModelsAdminPlayerRecordResponse.create_from_dict(content), None
+            return ModelsPlayerRecordResponse.create_from_dict(content), None
         if code == 400:
             return None, ModelsResponseError.create_from_dict(content)
         if code == 401:
             return None, ModelsResponseError.create_from_dict(content)
         if code == 403:
             return None, ModelsResponseError.create_from_dict(content)
         if code == 500:
@@ -278,40 +297,40 @@
     # endregion response methods
 
     # region static methods
 
     @classmethod
     def create(
         cls,
-        body: ModelsAdminPlayerRecordRequest,
+        body: ModelsPlayerRecordRequest,
         key: str,
         namespace: str,
         user_id: str,
         **kwargs,
-    ) -> AdminPutAdminPlayerRecordV1:
+    ) -> PutPlayerRecordHandlerV1:
         instance = cls()
         instance.body = body
         instance.key = key
         instance.namespace = namespace
         instance.user_id = user_id
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> AdminPutAdminPlayerRecordV1:
+    ) -> PutPlayerRecordHandlerV1:
         instance = cls()
         if "body" in dict_ and dict_["body"] is not None:
-            instance.body = ModelsAdminPlayerRecordRequest.create_from_dict(
+            instance.body = ModelsPlayerRecordRequest.create_from_dict(
                 dict_["body"], include_empty=include_empty
             )
         elif include_empty:
-            instance.body = ModelsAdminPlayerRecordRequest()
+            instance.body = ModelsPlayerRecordRequest()
         if "key" in dict_ and dict_["key"] is not None:
             instance.key = str(dict_["key"])
         elif include_empty:
             instance.key = ""
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
         elif include_empty:
```

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_record/bulk_get_admin_player_r_e53570.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_record/bulk_get_admin_player_r_e53570.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_tags/__init__.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_tags/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Cloudsave Service."""
 
-__version__ = "3.15.1"
+__version__ = "3.16.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .admin_delete_tag_handler_v1 import AdminDeleteTagHandlerV1
 from .admin_list_tags_handler_v1 import AdminListTagsHandlerV1
```

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_tags/admin_delete_tag_handler_v1.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_tags/admin_delete_tag_handler_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_tags/admin_list_tags_handler_v1.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_tags/admin_list_tags_handler_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/admin_tags/admin_post_tag_handler_v1.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_tags/admin_post_tag_handler_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/concurrent_record/__init__.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/concurrent_record/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Cloudsave Service."""
 
-__version__ = "3.15.1"
+__version__ = "3.16.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .put_game_record_concurr_33e39a import PutGameRecordConcurrentHandlerV1
 from .put_player_public_recor_3f1a7f import PutPlayerPublicRecordConcurrentHandlerV1
```

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/concurrent_record/put_game_record_concurr_33e39a.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/concurrent_record/put_game_record_concurr_33e39a.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/concurrent_record/put_player_public_recor_3f1a7f.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/concurrent_record/put_player_public_recor_3f1a7f.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/concurrent_record/put_player_record_concu_385e05.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/concurrent_record/put_player_record_concu_385e05.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/plugin_config/__init__.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/plugin_config/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Cloudsave Service."""
 
-__version__ = "3.15.1"
+__version__ = "3.16.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .create_plugin_config import CreatePluginConfig
 from .delete_plugin_config import DeletePluginConfig
```

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/plugin_config/create_plugin_config.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/plugin_config/create_plugin_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/plugin_config/delete_plugin_config.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/plugin_config/delete_plugin_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/plugin_config/get_plugin_config.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/plugin_config/get_plugin_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/plugin_config/update_plugin_config.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/plugin_config/update_plugin_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_game_binary_record/__init__.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_game_binary_record/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Cloudsave Service."""
 
-__version__ = "3.15.1"
+__version__ = "3.16.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .bulk_get_game_binary_record_v1 import BulkGetGameBinaryRecordV1
 from .delete_game_binary_record_v1 import DeleteGameBinaryRecordV1
```

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_game_binary_record/bulk_get_game_binary_record_v1.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_game_binary_record/bulk_get_game_binary_record_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_game_binary_record/delete_game_binary_record_v1.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_game_binary_record/delete_game_binary_record_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_game_binary_record/get_game_binary_record_v1.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_game_binary_record/get_game_binary_record_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_game_binary_record/list_game_binary_records_v1.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_game_binary_record/list_game_binary_records_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_game_binary_record/post_game_binary_presig_1e4e53.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_game_binary_record/post_game_binary_presig_1e4e53.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_game_binary_record/post_game_binary_record_v1.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_game_binary_record/post_game_binary_record_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_game_binary_record/put_game_binary_record_v1.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_game_binary_record/put_game_binary_record_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_game_record/__init__.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_game_record/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Cloudsave Service."""
 
-__version__ = "3.15.1"
+__version__ = "3.16.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .delete_game_record_handler_v1 import DeleteGameRecordHandlerV1
 from .get_game_record_handler_v1 import GetGameRecordHandlerV1
```

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_game_record/delete_game_record_handler_v1.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_game_record/delete_game_record_handler_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_game_record/get_game_record_handler_v1.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_game_record/get_game_record_handler_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_game_record/get_game_records_bulk.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_game_record/get_game_records_bulk.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_game_record/post_game_record_handler_v1.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_game_record/post_game_record_handler_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_game_record/put_game_record_handler_v1.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_game_record/put_game_record_handler_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_binary_record/__init__.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_binary_record/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Cloudsave Service."""
 
-__version__ = "3.15.1"
+__version__ = "3.16.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .bulk_get_my_binary_record_v1 import BulkGetMyBinaryRecordV1
 from .bulk_get_other_player_p_6c2093 import BulkGetOtherPlayerPublicBinaryRecordsV1
```

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_binary_record/bulk_get_my_binary_record_v1.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_binary_record/bulk_get_my_binary_record_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_binary_record/bulk_get_other_player_p_6c2093.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_binary_record/bulk_get_other_player_p_6c2093.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_binary_record/bulk_get_player_public__6635d7.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_binary_record/bulk_get_player_public__6635d7.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_binary_record/delete_player_binary_record_v1.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_binary_record/delete_player_binary_record_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_binary_record/get_player_binary_record_v1.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_binary_record/get_player_binary_record_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_binary_record/get_player_public_binar_e2a2d6.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_binary_record/get_player_public_binar_e2a2d6.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_binary_record/list_my_binary_records_v1.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_binary_record/list_my_binary_records_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_binary_record/list_other_player_publi_a9eef5.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_binary_record/list_other_player_publi_a9eef5.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_binary_record/post_player_binary_pres_38c5b5.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_binary_record/post_player_binary_pres_38c5b5.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_binary_record/post_player_binary_record_v1.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_binary_record/post_player_binary_record_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_binary_record/put_player_binary_recor_012bcd.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_binary_record/put_player_binary_recor_012bcd.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_binary_record/put_player_binary_record_v1.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_binary_record/put_player_binary_record_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_record/__init__.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_record/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Cloudsave Service."""
 
-__version__ = "3.15.1"
+__version__ = "3.16.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .bulk_get_player_public__28e43c import BulkGetPlayerPublicRecordHandlerV1
 from .delete_player_record_ha_3addde import DeletePlayerRecordHandlerV1
```

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_record/bulk_get_player_public__28e43c.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_record/bulk_get_player_public__28e43c.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_record/delete_player_record_ha_3addde.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_record/delete_player_record_ha_3addde.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_record/get_other_player_public_17685a.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_record/get_other_player_public_17685a.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_record/get_other_player_public_4438d8.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_record/get_other_player_public_4438d8.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_record/get_player_public_recor_5ea27d.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_record/get_player_public_recor_5ea27d.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_record/get_player_record_handler_v1.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_record/get_player_record_handler_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_record/get_player_records_bulk_b10df3.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_record/get_player_records_bulk_b10df3.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_record/post_player_public_reco_b8589e.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_record/post_player_public_reco_b8589e.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_record/post_player_record_handler_v1.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_record/put_player_public_recor_7928cf.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,87 +30,70 @@
 from accelbyte_py_sdk.core import HttpResponse
 
 from ...models import ModelsPlayerRecordRequest
 from ...models import ModelsPlayerRecordResponse
 from ...models import ModelsResponseError
 
 
-class PostPlayerRecordHandlerV1(Operation):
-    """Create or append player record (postPlayerRecordHandlerV1)
+class PutPlayerPublicRecordHandlerV1(Operation):
+    """Create or replace player public record (putPlayerPublicRecordHandlerV1)
 
     ## Description
 
-    This endpoints will create new player record or append the existing player record.
-    Only user that own the existing player record could modify.
+    This endpoints will create new player public record or replace the existing player public record.
 
-    **Append example:**
+    **Replace behaviour:**
+    The existing value will be replaced completely with the new value.
 
-    Example 1
+    Example
     - Existing JSON:
 
     `{ "data1": "value" }`
 
     - New JSON:
 
     `{ "data2": "new value" }`
 
     - Result:
 
-    `{ "data1": "value", "data2": "new value" }`
-
-
-    Example 2
-    - Existing JSON:
-
-    `{ "data1": { "data2": "value" }`
-
-    - New JSON:
-
-    `{ "data1": { "data3": "new value" }`
-
-    - Result:
+    `{ "data2": "new value" }`
 
-    `{ "data1": { "data2": "value", "data3": "new value" }`
 
 
     ## Restriction
     This is the restriction of Key Naming for the record:
     1. Cannot use **"."** as the key name
     - `{ "data.2": "value" }`
     2. Cannot use **"$"** as the prefix in key names
     - `{ "$data": "value" }`
     3. Cannot use empty string in key names
     - `{ "": "value" }`
 
 
-    ## Record Metadata
+    ## Reserved Word
+
+    Reserved Word List: **__META**
+
+    The reserved word cannot be used as a field in record value,
+    If still defining the field when creating or updating the record, it will be ignored.
+
+
+    ## Warning: This endpoint is going to deprecate
+
+    This endpoint is going to deprecate in the future please don't use it.
 
-    Metadata allows user to define the behaviour of the record.
-    Metadata can be defined in request body with field name **__META**.
-    When creating record, if **__META** field is not defined, the metadata value will use the default value.
-    When updating record, if **__META** field is not defined, the existing metadata value will stay as is.
-
-    **Metadata List:**
-    1. is_public (default: false, type: bool)
-    Indicate whether the player record is a public record or not.
-
-    **Request Body Example:**
-    ```
-    {
-    "__META": {
-    "is_public": true
-    }
-    ...
-    }
-    ```
+    For alternative, please use these endpoints:
+    - **POST /cloudsave/v1/namespaces/{namespace}/users/{userId}/records/{key}** and utilizing **__META** functionality
+    - **PUT /cloudsave/v1/namespaces/{namespace}/users/{userId}/records/{key}** and utilizing **__META** functionality
+    - **DELETE /cloudsave/v1/namespaces/{namespace}/users/{userId}/records/{key}**
 
     Properties:
-        url: /cloudsave/v1/namespaces/{namespace}/users/{userId}/records/{key}
+        url: /cloudsave/v1/namespaces/{namespace}/users/{userId}/records/{key}/public
 
-        method: POST
+        method: PUT
 
         tags: ["PublicPlayerRecord"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
@@ -121,29 +104,31 @@
         key: (key) REQUIRED str in path
 
         namespace: (namespace) REQUIRED str in path
 
         user_id: (userId) REQUIRED str in path
 
     Responses:
-        201: Created - ModelsPlayerRecordResponse (Record saved)
+        200: OK - ModelsPlayerRecordResponse (Record saved)
 
-        400: Bad Request - ModelsResponseError (18201: invalid record operator, expect [%s] but actual [%s] | 18030: invalid request body | 20002: validation error | 18060: invalid request body)
+        400: Bad Request - ModelsResponseError (18201: invalid record operator, expect [%s] but actual [%s] | 18100: invalid request body | 20002: validation error)
 
         401: Unauthorized - ModelsResponseError (20001: unauthorized access)
 
-        403: Forbidden - ModelsResponseError (18035: post action is forbidden on other user's record | 20013: insufficient permission)
+        403: Forbidden - ModelsResponseError (20013: insufficient permission)
 
-        500: Internal Server Error - ModelsResponseError (20000: internal server error | 18033: unable to save record | 18005: unable to decode record)
+        500: Internal Server Error - ModelsResponseError (20000: internal server error | 18101: unable to update record | 18005: unable to decode record)
     """
 
     # region fields
 
-    _url: str = "/cloudsave/v1/namespaces/{namespace}/users/{userId}/records/{key}"
-    _method: str = "POST"
+    _url: str = (
+        "/cloudsave/v1/namespaces/{namespace}/users/{userId}/records/{key}/public"
+    )
+    _method: str = "PUT"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
     body: ModelsPlayerRecordRequest  # REQUIRED in [body]
     key: str  # REQUIRED in [path]
@@ -211,27 +196,29 @@
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_body(self, value: ModelsPlayerRecordRequest) -> PostPlayerRecordHandlerV1:
+    def with_body(
+        self, value: ModelsPlayerRecordRequest
+    ) -> PutPlayerPublicRecordHandlerV1:
         self.body = value
         return self
 
-    def with_key(self, value: str) -> PostPlayerRecordHandlerV1:
+    def with_key(self, value: str) -> PutPlayerPublicRecordHandlerV1:
         self.key = value
         return self
 
-    def with_namespace(self, value: str) -> PostPlayerRecordHandlerV1:
+    def with_namespace(self, value: str) -> PutPlayerPublicRecordHandlerV1:
         self.namespace = value
         return self
 
-    def with_user_id(self, value: str) -> PostPlayerRecordHandlerV1:
+    def with_user_id(self, value: str) -> PutPlayerPublicRecordHandlerV1:
         self.user_id = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
@@ -264,38 +251,38 @@
         self, code: int, content_type: str, content: Any
     ) -> Tuple[
         Union[None, ModelsPlayerRecordResponse],
         Union[None, HttpResponse, ModelsResponseError],
     ]:
         """Parse the given response.
 
-        201: Created - ModelsPlayerRecordResponse (Record saved)
+        200: OK - ModelsPlayerRecordResponse (Record saved)
 
-        400: Bad Request - ModelsResponseError (18201: invalid record operator, expect [%s] but actual [%s] | 18030: invalid request body | 20002: validation error | 18060: invalid request body)
+        400: Bad Request - ModelsResponseError (18201: invalid record operator, expect [%s] but actual [%s] | 18100: invalid request body | 20002: validation error)
 
         401: Unauthorized - ModelsResponseError (20001: unauthorized access)
 
-        403: Forbidden - ModelsResponseError (18035: post action is forbidden on other user's record | 20013: insufficient permission)
+        403: Forbidden - ModelsResponseError (20013: insufficient permission)
 
-        500: Internal Server Error - ModelsResponseError (20000: internal server error | 18033: unable to save record | 18005: unable to decode record)
+        500: Internal Server Error - ModelsResponseError (20000: internal server error | 18101: unable to update record | 18005: unable to decode record)
 
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
+        if code == 200:
             return ModelsPlayerRecordResponse.create_from_dict(content), None
         if code == 400:
             return None, ModelsResponseError.create_from_dict(content)
         if code == 401:
             return None, ModelsResponseError.create_from_dict(content)
         if code == 403:
             return None, ModelsResponseError.create_from_dict(content)
@@ -314,28 +301,28 @@
     def create(
         cls,
         body: ModelsPlayerRecordRequest,
         key: str,
         namespace: str,
         user_id: str,
         **kwargs,
-    ) -> PostPlayerRecordHandlerV1:
+    ) -> PutPlayerPublicRecordHandlerV1:
         instance = cls()
         instance.body = body
         instance.key = key
         instance.namespace = namespace
         instance.user_id = user_id
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> PostPlayerRecordHandlerV1:
+    ) -> PutPlayerPublicRecordHandlerV1:
         instance = cls()
         if "body" in dict_ and dict_["body"] is not None:
             instance.body = ModelsPlayerRecordRequest.create_from_dict(
                 dict_["body"], include_empty=include_empty
             )
         elif include_empty:
             instance.body = ModelsPlayerRecordRequest()
```

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_record/public_delete_player_pu_0cc8b5.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_record/public_delete_player_pu_0cc8b5.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_record/put_player_public_recor_7928cf.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_record/retrieve_player_records.py`

 * *Files 22% similar despite different names*

```diff
@@ -25,119 +25,66 @@
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
-from ...models import ModelsPlayerRecordRequest
-from ...models import ModelsPlayerRecordResponse
+from ...models import ModelsListPlayerRecordKeysResponse
 from ...models import ModelsResponseError
 
 
-class PutPlayerPublicRecordHandlerV1(Operation):
-    """Create or replace player public record (putPlayerPublicRecordHandlerV1)
+class RetrievePlayerRecords(Operation):
+    """Query player records key (RetrievePlayerRecords)
 
-    ## Description
-
-    This endpoints will create new player public record or replace the existing player public record.
-
-    **Replace behaviour:**
-    The existing value will be replaced completely with the new value.
-
-    Example
-    - Existing JSON:
-
-    `{ "data1": "value" }`
-
-    - New JSON:
-
-    `{ "data2": "new value" }`
-
-    - Result:
-
-    `{ "data2": "new value" }`
-
-
-
-    ## Restriction
-    This is the restriction of Key Naming for the record:
-    1. Cannot use **"."** as the key name
-    - `{ "data.2": "value" }`
-    2. Cannot use **"$"** as the prefix in key names
-    - `{ "$data": "value" }`
-    3. Cannot use empty string in key names
-    - `{ "": "value" }`
-
-
-    ## Reserved Word
-
-    Reserved Word List: **__META**
-
-    The reserved word cannot be used as a field in record value,
-    If still defining the field when creating or updating the record, it will be ignored.
-
-
-    ## Warning: This endpoint is going to deprecate
-
-    This endpoint is going to deprecate in the future please don't use it.
-
-    For alternative, please use these endpoints:
-    - **POST /cloudsave/v1/namespaces/{namespace}/users/{userId}/records/{key}** and utilizing **__META** functionality
-    - **PUT /cloudsave/v1/namespaces/{namespace}/users/{userId}/records/{key}** and utilizing **__META** functionality
-    - **DELETE /cloudsave/v1/namespaces/{namespace}/users/{userId}/records/{key}**
+    Retrieve list of player records key under given namespace.
 
     Properties:
-        url: /cloudsave/v1/namespaces/{namespace}/users/{userId}/records/{key}/public
+        url: /cloudsave/v1/namespaces/{namespace}/users/me/records
 
-        method: PUT
+        method: GET
 
         tags: ["PublicPlayerRecord"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
-        body: (body) REQUIRED ModelsPlayerRecordRequest in body
-
-        key: (key) REQUIRED str in path
-
         namespace: (namespace) REQUIRED str in path
 
-        user_id: (userId) REQUIRED str in path
+        limit: (limit) OPTIONAL int in query
+
+        offset: (offset) OPTIONAL int in query
 
     Responses:
-        200: OK - ModelsPlayerRecordResponse (Record saved)
+        200: OK - ModelsListPlayerRecordKeysResponse (Successful operation)
 
-        400: Bad Request - ModelsResponseError (18201: invalid record operator, expect [%s] but actual [%s] | 18100: invalid request body | 20002: validation error)
+        400: Bad Request - ModelsResponseError (18113: invalid request body)
 
         401: Unauthorized - ModelsResponseError (20001: unauthorized access)
 
         403: Forbidden - ModelsResponseError (20013: insufficient permission)
 
-        500: Internal Server Error - ModelsResponseError (20000: internal server error | 18101: unable to update record | 18005: unable to decode record)
+        500: Internal Server Error - ModelsResponseError (18114: unable to retrieve list of key records)
     """
 
     # region fields
 
-    _url: str = (
-        "/cloudsave/v1/namespaces/{namespace}/users/{userId}/records/{key}/public"
-    )
-    _method: str = "PUT"
+    _url: str = "/cloudsave/v1/namespaces/{namespace}/users/me/records"
+    _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
-    body: ModelsPlayerRecordRequest  # REQUIRED in [body]
-    key: str  # REQUIRED in [path]
     namespace: str  # REQUIRED in [path]
-    user_id: str  # REQUIRED in [path]
+    limit: int  # OPTIONAL in [query]
+    offset: int  # OPTIONAL in [query]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
@@ -169,105 +116,94 @@
 
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
-        if hasattr(self, "key"):
-            result["key"] = self.key
         if hasattr(self, "namespace"):
             result["namespace"] = self.namespace
-        if hasattr(self, "user_id"):
-            result["userId"] = self.user_id
+        return result
+
+    def get_query_params(self) -> dict:
+        result = {}
+        if hasattr(self, "limit"):
+            result["limit"] = self.limit
+        if hasattr(self, "offset"):
+            result["offset"] = self.offset
         return result
 
     # endregion get_x_params methods
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_body(
-        self, value: ModelsPlayerRecordRequest
-    ) -> PutPlayerPublicRecordHandlerV1:
-        self.body = value
-        return self
-
-    def with_key(self, value: str) -> PutPlayerPublicRecordHandlerV1:
-        self.key = value
+    def with_namespace(self, value: str) -> RetrievePlayerRecords:
+        self.namespace = value
         return self
 
-    def with_namespace(self, value: str) -> PutPlayerPublicRecordHandlerV1:
-        self.namespace = value
+    def with_limit(self, value: int) -> RetrievePlayerRecords:
+        self.limit = value
         return self
 
-    def with_user_id(self, value: str) -> PutPlayerPublicRecordHandlerV1:
-        self.user_id = value
+    def with_offset(self, value: int) -> RetrievePlayerRecords:
+        self.offset = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
-        if hasattr(self, "body") and self.body:
-            result["body"] = self.body.to_dict(include_empty=include_empty)
-        elif include_empty:
-            result["body"] = ModelsPlayerRecordRequest()
-        if hasattr(self, "key") and self.key:
-            result["key"] = str(self.key)
-        elif include_empty:
-            result["key"] = ""
         if hasattr(self, "namespace") and self.namespace:
             result["namespace"] = str(self.namespace)
         elif include_empty:
             result["namespace"] = ""
-        if hasattr(self, "user_id") and self.user_id:
-            result["userId"] = str(self.user_id)
+        if hasattr(self, "limit") and self.limit:
+            result["limit"] = int(self.limit)
         elif include_empty:
-            result["userId"] = ""
+            result["limit"] = 0
+        if hasattr(self, "offset") and self.offset:
+            result["offset"] = int(self.offset)
+        elif include_empty:
+            result["offset"] = 0
         return result
 
     # endregion to methods
 
     # region response methods
 
     # noinspection PyMethodMayBeStatic
     def parse_response(
         self, code: int, content_type: str, content: Any
     ) -> Tuple[
-        Union[None, ModelsPlayerRecordResponse],
+        Union[None, ModelsListPlayerRecordKeysResponse],
         Union[None, HttpResponse, ModelsResponseError],
     ]:
         """Parse the given response.
 
-        200: OK - ModelsPlayerRecordResponse (Record saved)
+        200: OK - ModelsListPlayerRecordKeysResponse (Successful operation)
 
-        400: Bad Request - ModelsResponseError (18201: invalid record operator, expect [%s] but actual [%s] | 18100: invalid request body | 20002: validation error)
+        400: Bad Request - ModelsResponseError (18113: invalid request body)
 
         401: Unauthorized - ModelsResponseError (20001: unauthorized access)
 
         403: Forbidden - ModelsResponseError (20013: insufficient permission)
 
-        500: Internal Server Error - ModelsResponseError (20000: internal server error | 18101: unable to update record | 18005: unable to decode record)
+        500: Internal Server Error - ModelsResponseError (18114: unable to retrieve list of key records)
 
         ---: HttpResponse (Undocumented Response)
 
         ---: HttpResponse (Unexpected Content-Type Error)
 
         ---: HttpResponse (Unhandled Error)
         """
@@ -275,15 +211,15 @@
             code=code, content_type=content_type, content=content
         )
         if error is not None:
             return None, None if error.is_no_content() else error
         code, content_type, content = pre_processed_response
 
         if code == 200:
-            return ModelsPlayerRecordResponse.create_from_dict(content), None
+            return ModelsListPlayerRecordKeysResponse.create_from_dict(content), None
         if code == 400:
             return None, ModelsResponseError.create_from_dict(content)
         if code == 401:
             return None, ModelsResponseError.create_from_dict(content)
         if code == 403:
             return None, ModelsResponseError.create_from_dict(content)
         if code == 500:
@@ -296,66 +232,58 @@
     # endregion response methods
 
     # region static methods
 
     @classmethod
     def create(
         cls,
-        body: ModelsPlayerRecordRequest,
-        key: str,
         namespace: str,
-        user_id: str,
+        limit: Optional[int] = None,
+        offset: Optional[int] = None,
         **kwargs,
-    ) -> PutPlayerPublicRecordHandlerV1:
+    ) -> RetrievePlayerRecords:
         instance = cls()
-        instance.body = body
-        instance.key = key
         instance.namespace = namespace
-        instance.user_id = user_id
+        if limit is not None:
+            instance.limit = limit
+        if offset is not None:
+            instance.offset = offset
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> PutPlayerPublicRecordHandlerV1:
+    ) -> RetrievePlayerRecords:
         instance = cls()
-        if "body" in dict_ and dict_["body"] is not None:
-            instance.body = ModelsPlayerRecordRequest.create_from_dict(
-                dict_["body"], include_empty=include_empty
-            )
-        elif include_empty:
-            instance.body = ModelsPlayerRecordRequest()
-        if "key" in dict_ and dict_["key"] is not None:
-            instance.key = str(dict_["key"])
-        elif include_empty:
-            instance.key = ""
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
         elif include_empty:
             instance.namespace = ""
-        if "userId" in dict_ and dict_["userId"] is not None:
-            instance.user_id = str(dict_["userId"])
+        if "limit" in dict_ and dict_["limit"] is not None:
+            instance.limit = int(dict_["limit"])
+        elif include_empty:
+            instance.limit = 0
+        if "offset" in dict_ and dict_["offset"] is not None:
+            instance.offset = int(dict_["offset"])
         elif include_empty:
-            instance.user_id = ""
+            instance.offset = 0
         return instance
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
-            "body": "body",
-            "key": "key",
             "namespace": "namespace",
-            "userId": "user_id",
+            "limit": "limit",
+            "offset": "offset",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
-            "body": True,
-            "key": True,
             "namespace": True,
-            "userId": True,
+            "limit": False,
+            "offset": False,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_record/put_player_record_handler_v1.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_record/admin_post_player_admin_b138ee.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,43 +25,54 @@
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
-from ...models import ModelsPlayerRecordRequest
-from ...models import ModelsPlayerRecordResponse
+from ...models import ModelsAdminPlayerRecordRequest
+from ...models import ModelsAdminPlayerRecordResponse
 from ...models import ModelsResponseError
 
 
-class PutPlayerRecordHandlerV1(Operation):
-    """Create or replace player record (putPlayerRecordHandlerV1)
+class AdminPostPlayerAdminRecordV1(Operation):
+    """Create or append admin player record (adminPostPlayerAdminRecordV1)
 
     ## Description
 
-    This endpoints will create new player record or replace the existing player record.
-    Only user that own the existing player record could modify it.
+    This endpoints will create new admin player record or append the existing admin game record.
 
-    **Replace behaviour:**
-    The existing value will be replaced completely with the new value.
+    **Append example:**
 
-    Example
+    Example 1
     - Existing JSON:
 
     `{ "data1": "value" }`
 
     - New JSON:
 
     `{ "data2": "new value" }`
 
     - Result:
 
-    `{ "data2": "new value" }`
+    `{ "data1": "value", "data2": "new value" }`
+
+
+    Example 2
+    - Existing JSON:
+
+    `{ "data1": { "data2": "value" }`
+
+    - New JSON:
+
+    `{ "data1": { "data3": "new value" }`
+
+    - Result:
 
+    `{ "data1": { "data2": "value", "data3": "new value" }`
 
 
     ## Restriction
     This is the restriction of Key Naming for the record:
     1. Cannot use **"."** as the key name
     - `{ "data.2": "value" }`
     2. Cannot use **"$"** as the prefix in key names
@@ -74,70 +85,72 @@
 
     Metadata allows user to define the behaviour of the record.
     Metadata can be defined in request body with field name **__META**.
     When creating record, if **__META** field is not defined, the metadata value will use the default value.
     When updating record, if **__META** field is not defined, the existing metadata value will stay as is.
 
     **Metadata List:**
-    1. is_public (default: false, type: bool)
-    Indicate whether the player record is a public record or not.
+    1. tags (default: *empty array*, type: array of string)
+    Indicate the tagging for the admin record.
 
     **Request Body Example:**
     ```
     {
     "__META": {
-    "is_public": true
+    "tags": ["tag1", "tag2"]
     }
     ...
     }
     ```
 
     Properties:
-        url: /cloudsave/v1/namespaces/{namespace}/users/{userId}/records/{key}
+        url: /cloudsave/v1/admin/namespaces/{namespace}/users/{userId}/adminrecords/{key}
 
-        method: PUT
+        method: POST
 
-        tags: ["PublicPlayerRecord"]
+        tags: ["AdminRecord"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
-        body: (body) REQUIRED ModelsPlayerRecordRequest in body
+        body: (body) REQUIRED ModelsAdminPlayerRecordRequest in body
 
         key: (key) REQUIRED str in path
 
         namespace: (namespace) REQUIRED str in path
 
         user_id: (userId) REQUIRED str in path
 
     Responses:
-        200: OK - ModelsPlayerRecordResponse (Record saved)
+        201: Created - ModelsAdminPlayerRecordResponse (Record in user-level saved)
 
-        400: Bad Request - ModelsResponseError (18201: invalid record operator, expect [%s] but actual [%s] | 18060: invalid request body | 20002: validation error)
+        400: Bad Request - ModelsResponseError (18150: invalid request body | 20002: validation error)
 
         401: Unauthorized - ModelsResponseError (20001: unauthorized access)
 
-        403: Forbidden - ModelsResponseError (18063: put action is forbidden on other user's record | 20013: insufficient permission)
+        403: Forbidden - ModelsResponseError (20013: insufficient permission)
 
-        500: Internal Server Error - ModelsResponseError (20000: internal server error | 18061: unable to update record | 18005: unable to decode record)
+        500: Internal Server Error - ModelsResponseError (20000: internal server error | 18033: unable to save record | 18163: unable to decode record)
     """
 
     # region fields
 
-    _url: str = "/cloudsave/v1/namespaces/{namespace}/users/{userId}/records/{key}"
-    _method: str = "PUT"
+    _url: str = (
+        "/cloudsave/v1/admin/namespaces/{namespace}/users/{userId}/adminrecords/{key}"
+    )
+    _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
-    body: ModelsPlayerRecordRequest  # REQUIRED in [body]
+    body: ModelsAdminPlayerRecordRequest  # REQUIRED in [body]
     key: str  # REQUIRED in [path]
     namespace: str  # REQUIRED in [path]
     user_id: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
@@ -199,40 +212,42 @@
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_body(self, value: ModelsPlayerRecordRequest) -> PutPlayerRecordHandlerV1:
+    def with_body(
+        self, value: ModelsAdminPlayerRecordRequest
+    ) -> AdminPostPlayerAdminRecordV1:
         self.body = value
         return self
 
-    def with_key(self, value: str) -> PutPlayerRecordHandlerV1:
+    def with_key(self, value: str) -> AdminPostPlayerAdminRecordV1:
         self.key = value
         return self
 
-    def with_namespace(self, value: str) -> PutPlayerRecordHandlerV1:
+    def with_namespace(self, value: str) -> AdminPostPlayerAdminRecordV1:
         self.namespace = value
         return self
 
-    def with_user_id(self, value: str) -> PutPlayerRecordHandlerV1:
+    def with_user_id(self, value: str) -> AdminPostPlayerAdminRecordV1:
         self.user_id = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
         if hasattr(self, "body") and self.body:
             result["body"] = self.body.to_dict(include_empty=include_empty)
         elif include_empty:
-            result["body"] = ModelsPlayerRecordRequest()
+            result["body"] = ModelsAdminPlayerRecordRequest()
         if hasattr(self, "key") and self.key:
             result["key"] = str(self.key)
         elif include_empty:
             result["key"] = ""
         if hasattr(self, "namespace") and self.namespace:
             result["namespace"] = str(self.namespace)
         elif include_empty:
@@ -247,44 +262,44 @@
 
     # region response methods
 
     # noinspection PyMethodMayBeStatic
     def parse_response(
         self, code: int, content_type: str, content: Any
     ) -> Tuple[
-        Union[None, ModelsPlayerRecordResponse],
+        Union[None, ModelsAdminPlayerRecordResponse],
         Union[None, HttpResponse, ModelsResponseError],
     ]:
         """Parse the given response.
 
-        200: OK - ModelsPlayerRecordResponse (Record saved)
+        201: Created - ModelsAdminPlayerRecordResponse (Record in user-level saved)
 
-        400: Bad Request - ModelsResponseError (18201: invalid record operator, expect [%s] but actual [%s] | 18060: invalid request body | 20002: validation error)
+        400: Bad Request - ModelsResponseError (18150: invalid request body | 20002: validation error)
 
         401: Unauthorized - ModelsResponseError (20001: unauthorized access)
 
-        403: Forbidden - ModelsResponseError (18063: put action is forbidden on other user's record | 20013: insufficient permission)
+        403: Forbidden - ModelsResponseError (20013: insufficient permission)
 
-        500: Internal Server Error - ModelsResponseError (20000: internal server error | 18061: unable to update record | 18005: unable to decode record)
+        500: Internal Server Error - ModelsResponseError (20000: internal server error | 18033: unable to save record | 18163: unable to decode record)
 
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
-            return ModelsPlayerRecordResponse.create_from_dict(content), None
+        if code == 201:
+            return ModelsAdminPlayerRecordResponse.create_from_dict(content), None
         if code == 400:
             return None, ModelsResponseError.create_from_dict(content)
         if code == 401:
             return None, ModelsResponseError.create_from_dict(content)
         if code == 403:
             return None, ModelsResponseError.create_from_dict(content)
         if code == 500:
@@ -297,40 +312,40 @@
     # endregion response methods
 
     # region static methods
 
     @classmethod
     def create(
         cls,
-        body: ModelsPlayerRecordRequest,
+        body: ModelsAdminPlayerRecordRequest,
         key: str,
         namespace: str,
         user_id: str,
         **kwargs,
-    ) -> PutPlayerRecordHandlerV1:
+    ) -> AdminPostPlayerAdminRecordV1:
         instance = cls()
         instance.body = body
         instance.key = key
         instance.namespace = namespace
         instance.user_id = user_id
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> PutPlayerRecordHandlerV1:
+    ) -> AdminPostPlayerAdminRecordV1:
         instance = cls()
         if "body" in dict_ and dict_["body"] is not None:
-            instance.body = ModelsPlayerRecordRequest.create_from_dict(
+            instance.body = ModelsAdminPlayerRecordRequest.create_from_dict(
                 dict_["body"], include_empty=include_empty
             )
         elif include_empty:
-            instance.body = ModelsPlayerRecordRequest()
+            instance.body = ModelsAdminPlayerRecordRequest()
         if "key" in dict_ and dict_["key"] is not None:
             instance.key = str(dict_["key"])
         elif include_empty:
             instance.key = ""
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
         elif include_empty:
```

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_player_record/retrieve_player_records.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_tags/public_list_tags_handler_v1.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,57 +25,59 @@
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
-from ...models import ModelsListPlayerRecordKeysResponse
+from ...models import ModelsListTagsResponse
 from ...models import ModelsResponseError
 
 
-class RetrievePlayerRecords(Operation):
-    """Query player records key (RetrievePlayerRecords)
+class PublicListTagsHandlerV1(Operation):
+    """List tags (publicListTagsHandlerV1)
 
-    Retrieve list of player records key under given namespace.
+    ## Description
+
+    Retrieve list of available tags by namespace
 
     Properties:
-        url: /cloudsave/v1/namespaces/{namespace}/users/me/records
+        url: /cloudsave/v1/namespaces/{namespace}/tags
 
         method: GET
 
-        tags: ["PublicPlayerRecord"]
+        tags: ["PublicTags"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
         namespace: (namespace) REQUIRED str in path
 
         limit: (limit) OPTIONAL int in query
 
         offset: (offset) OPTIONAL int in query
 
     Responses:
-        200: OK - ModelsListPlayerRecordKeysResponse (Successful operation)
+        200: OK - ModelsListTagsResponse (Available tags retrieved)
 
-        400: Bad Request - ModelsResponseError (18113: invalid request body)
+        400: Bad Request - ModelsResponseError (18503: unable to list tags)
 
         401: Unauthorized - ModelsResponseError (20001: unauthorized access)
 
         403: Forbidden - ModelsResponseError (20013: insufficient permission)
 
-        500: Internal Server Error - ModelsResponseError (18114: unable to retrieve list of key records)
+        500: Internal Server Error - ModelsResponseError (18502: unable to list tags)
     """
 
     # region fields
 
-    _url: str = "/cloudsave/v1/namespaces/{namespace}/users/me/records"
+    _url: str = "/cloudsave/v1/namespaces/{namespace}/tags"
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
     namespace: str  # REQUIRED in [path]
@@ -142,23 +144,23 @@
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_namespace(self, value: str) -> RetrievePlayerRecords:
+    def with_namespace(self, value: str) -> PublicListTagsHandlerV1:
         self.namespace = value
         return self
 
-    def with_limit(self, value: int) -> RetrievePlayerRecords:
+    def with_limit(self, value: int) -> PublicListTagsHandlerV1:
         self.limit = value
         return self
 
-    def with_offset(self, value: int) -> RetrievePlayerRecords:
+    def with_offset(self, value: int) -> PublicListTagsHandlerV1:
         self.offset = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
@@ -182,28 +184,28 @@
 
     # region response methods
 
     # noinspection PyMethodMayBeStatic
     def parse_response(
         self, code: int, content_type: str, content: Any
     ) -> Tuple[
-        Union[None, ModelsListPlayerRecordKeysResponse],
+        Union[None, ModelsListTagsResponse],
         Union[None, HttpResponse, ModelsResponseError],
     ]:
         """Parse the given response.
 
-        200: OK - ModelsListPlayerRecordKeysResponse (Successful operation)
+        200: OK - ModelsListTagsResponse (Available tags retrieved)
 
-        400: Bad Request - ModelsResponseError (18113: invalid request body)
+        400: Bad Request - ModelsResponseError (18503: unable to list tags)
 
         401: Unauthorized - ModelsResponseError (20001: unauthorized access)
 
         403: Forbidden - ModelsResponseError (20013: insufficient permission)
 
-        500: Internal Server Error - ModelsResponseError (18114: unable to retrieve list of key records)
+        500: Internal Server Error - ModelsResponseError (18502: unable to list tags)
 
         ---: HttpResponse (Undocumented Response)
 
         ---: HttpResponse (Unexpected Content-Type Error)
 
         ---: HttpResponse (Unhandled Error)
         """
@@ -211,15 +213,15 @@
             code=code, content_type=content_type, content=content
         )
         if error is not None:
             return None, None if error.is_no_content() else error
         code, content_type, content = pre_processed_response
 
         if code == 200:
-            return ModelsListPlayerRecordKeysResponse.create_from_dict(content), None
+            return ModelsListTagsResponse.create_from_dict(content), None
         if code == 400:
             return None, ModelsResponseError.create_from_dict(content)
         if code == 401:
             return None, ModelsResponseError.create_from_dict(content)
         if code == 403:
             return None, ModelsResponseError.create_from_dict(content)
         if code == 500:
@@ -236,29 +238,29 @@
     @classmethod
     def create(
         cls,
         namespace: str,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         **kwargs,
-    ) -> RetrievePlayerRecords:
+    ) -> PublicListTagsHandlerV1:
         instance = cls()
         instance.namespace = namespace
         if limit is not None:
             instance.limit = limit
         if offset is not None:
             instance.offset = offset
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> RetrievePlayerRecords:
+    ) -> PublicListTagsHandlerV1:
         instance = cls()
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
         elif include_empty:
             instance.namespace = ""
         if "limit" in dict_ and dict_["limit"] is not None:
             instance.limit = int(dict_["limit"])
```

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_tags/__init__.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/public_tags/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,14 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Cloudsave Service."""
 
-__version__ = "3.15.1"
+__version__ = "3.16.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .public_list_tags_handler_v1 import PublicListTagsHandlerV1
```

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/public_tags/public_list_tags_handler_v1.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/ttl_config/delete_game_binary_reco_40da6b.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,68 +25,66 @@
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
-from ...models import ModelsListTagsResponse
 from ...models import ModelsResponseError
 
 
-class PublicListTagsHandlerV1(Operation):
-    """List tags (publicListTagsHandlerV1)
+class DeleteGameBinaryRecordTTLConfig(Operation):
+    """Delete game binary record TTL config (deleteGameBinaryRecordTTLConfig)
 
     ## Description
 
-    Retrieve list of available tags by namespace
+    This endpoints will delete the ttl config of the game binary record
 
     Properties:
-        url: /cloudsave/v1/namespaces/{namespace}/tags
+        url: /cloudsave/v1/admin/namespaces/{namespace}/binaries/{key}/ttl
 
-        method: GET
+        method: DELETE
 
-        tags: ["PublicTags"]
+        tags: ["TTLConfig"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
-        namespace: (namespace) REQUIRED str in path
-
-        limit: (limit) OPTIONAL int in query
+        key: (key) REQUIRED str in path
 
-        offset: (offset) OPTIONAL int in query
+        namespace: (namespace) REQUIRED str in path
 
     Responses:
-        200: OK - ModelsListTagsResponse (Available tags retrieved)
+        204: No Content - (TTL config deleted)
 
-        400: Bad Request - ModelsResponseError (18503: unable to list tags)
+        400: Bad Request - ModelsResponseError (20002: validation error)
 
         401: Unauthorized - ModelsResponseError (20001: unauthorized access)
 
         403: Forbidden - ModelsResponseError (20013: insufficient permission)
 
-        500: Internal Server Error - ModelsResponseError (18502: unable to list tags)
+        404: Not Found - ModelsResponseError (18317: record not found)
+
+        500: Internal Server Error - ModelsResponseError (20000: internal server error | 18318: unable to update record)
     """
 
     # region fields
 
-    _url: str = "/cloudsave/v1/namespaces/{namespace}/tags"
-    _method: str = "GET"
+    _url: str = "/cloudsave/v1/admin/namespaces/{namespace}/binaries/{key}/ttl"
+    _method: str = "DELETE"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    key: str  # REQUIRED in [path]
     namespace: str  # REQUIRED in [path]
-    limit: int  # OPTIONAL in [query]
-    offset: int  # OPTIONAL in [query]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
@@ -119,173 +117,146 @@
     # endregion get methods
 
     # region get_x_params methods
 
     def get_all_params(self) -> dict:
         return {
             "path": self.get_path_params(),
-            "query": self.get_query_params(),
         }
 
     def get_path_params(self) -> dict:
         result = {}
+        if hasattr(self, "key"):
+            result["key"] = self.key
         if hasattr(self, "namespace"):
             result["namespace"] = self.namespace
         return result
 
-    def get_query_params(self) -> dict:
-        result = {}
-        if hasattr(self, "limit"):
-            result["limit"] = self.limit
-        if hasattr(self, "offset"):
-            result["offset"] = self.offset
-        return result
-
     # endregion get_x_params methods
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_namespace(self, value: str) -> PublicListTagsHandlerV1:
-        self.namespace = value
-        return self
-
-    def with_limit(self, value: int) -> PublicListTagsHandlerV1:
-        self.limit = value
+    def with_key(self, value: str) -> DeleteGameBinaryRecordTTLConfig:
+        self.key = value
         return self
 
-    def with_offset(self, value: int) -> PublicListTagsHandlerV1:
-        self.offset = value
+    def with_namespace(self, value: str) -> DeleteGameBinaryRecordTTLConfig:
+        self.namespace = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
+        if hasattr(self, "key") and self.key:
+            result["key"] = str(self.key)
+        elif include_empty:
+            result["key"] = ""
         if hasattr(self, "namespace") and self.namespace:
             result["namespace"] = str(self.namespace)
         elif include_empty:
             result["namespace"] = ""
-        if hasattr(self, "limit") and self.limit:
-            result["limit"] = int(self.limit)
-        elif include_empty:
-            result["limit"] = 0
-        if hasattr(self, "offset") and self.offset:
-            result["offset"] = int(self.offset)
-        elif include_empty:
-            result["offset"] = 0
         return result
 
     # endregion to methods
 
     # region response methods
 
     # noinspection PyMethodMayBeStatic
     def parse_response(
         self, code: int, content_type: str, content: Any
-    ) -> Tuple[
-        Union[None, ModelsListTagsResponse],
-        Union[None, HttpResponse, ModelsResponseError],
-    ]:
+    ) -> Tuple[None, Union[None, HttpResponse, ModelsResponseError]]:
         """Parse the given response.
 
-        200: OK - ModelsListTagsResponse (Available tags retrieved)
+        204: No Content - (TTL config deleted)
 
-        400: Bad Request - ModelsResponseError (18503: unable to list tags)
+        400: Bad Request - ModelsResponseError (20002: validation error)
 
         401: Unauthorized - ModelsResponseError (20001: unauthorized access)
 
         403: Forbidden - ModelsResponseError (20013: insufficient permission)
 
-        500: Internal Server Error - ModelsResponseError (18502: unable to list tags)
+        404: Not Found - ModelsResponseError (18317: record not found)
+
+        500: Internal Server Error - ModelsResponseError (20000: internal server error | 18318: unable to update record)
 
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
-            return ModelsListTagsResponse.create_from_dict(content), None
+        if code == 204:
+            return None, None
         if code == 400:
             return None, ModelsResponseError.create_from_dict(content)
         if code == 401:
             return None, ModelsResponseError.create_from_dict(content)
         if code == 403:
             return None, ModelsResponseError.create_from_dict(content)
+        if code == 404:
+            return None, ModelsResponseError.create_from_dict(content)
         if code == 500:
             return None, ModelsResponseError.create_from_dict(content)
 
         return self.handle_undocumented_response(
             code=code, content_type=content_type, content=content
         )
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
     def create(
-        cls,
-        namespace: str,
-        limit: Optional[int] = None,
-        offset: Optional[int] = None,
-        **kwargs,
-    ) -> PublicListTagsHandlerV1:
+        cls, key: str, namespace: str, **kwargs
+    ) -> DeleteGameBinaryRecordTTLConfig:
         instance = cls()
+        instance.key = key
         instance.namespace = namespace
-        if limit is not None:
-            instance.limit = limit
-        if offset is not None:
-            instance.offset = offset
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> PublicListTagsHandlerV1:
+    ) -> DeleteGameBinaryRecordTTLConfig:
         instance = cls()
+        if "key" in dict_ and dict_["key"] is not None:
+            instance.key = str(dict_["key"])
+        elif include_empty:
+            instance.key = ""
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
         elif include_empty:
             instance.namespace = ""
-        if "limit" in dict_ and dict_["limit"] is not None:
-            instance.limit = int(dict_["limit"])
-        elif include_empty:
-            instance.limit = 0
-        if "offset" in dict_ and dict_["offset"] is not None:
-            instance.offset = int(dict_["offset"])
-        elif include_empty:
-            instance.offset = 0
         return instance
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
+            "key": "key",
             "namespace": "namespace",
-            "limit": "limit",
-            "offset": "offset",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
+            "key": True,
             "namespace": True,
-            "limit": False,
-            "offset": False,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/ttl_config/__init__.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/ttl_config/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Cloudsave Service."""
 
-__version__ = "3.15.1"
+__version__ = "3.16.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .delete_game_binary_reco_40da6b import DeleteGameBinaryRecordTTLConfig
 from .delete_game_record_ttl_config import DeleteGameRecordTTLConfig
```

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/ttl_config/delete_game_binary_reco_40da6b.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/ttl_config/delete_game_record_ttl_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,23 +28,23 @@
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
 from ...models import ModelsResponseError
 
 
-class DeleteGameBinaryRecordTTLConfig(Operation):
-    """Delete game binary record TTL config (deleteGameBinaryRecordTTLConfig)
+class DeleteGameRecordTTLConfig(Operation):
+    """Delete game record TTL config (deleteGameRecordTTLConfig)
 
     ## Description
 
-    This endpoints will delete the ttl config of the game binary record
+    This endpoints will delete the ttl config of the game record
 
     Properties:
-        url: /cloudsave/v1/admin/namespaces/{namespace}/binaries/{key}/ttl
+        url: /cloudsave/v1/admin/namespaces/{namespace}/records/{key}/ttl
 
         method: DELETE
 
         tags: ["TTLConfig"]
 
         consumes: ["application/json"]
 
@@ -61,22 +61,22 @@
 
         400: Bad Request - ModelsResponseError (20002: validation error)
 
         401: Unauthorized - ModelsResponseError (20001: unauthorized access)
 
         403: Forbidden - ModelsResponseError (20013: insufficient permission)
 
-        404: Not Found - ModelsResponseError (18317: record not found)
+        404: Not Found - ModelsResponseError (18003: record not found)
 
-        500: Internal Server Error - ModelsResponseError (20000: internal server error | 18318: unable to update record)
+        500: Internal Server Error - ModelsResponseError (20000: internal server error | 18053: unable to update record)
     """
 
     # region fields
 
-    _url: str = "/cloudsave/v1/admin/namespaces/{namespace}/binaries/{key}/ttl"
+    _url: str = "/cloudsave/v1/admin/namespaces/{namespace}/records/{key}/ttl"
     _method: str = "DELETE"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
     key: str  # REQUIRED in [path]
@@ -135,19 +135,19 @@
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_key(self, value: str) -> DeleteGameBinaryRecordTTLConfig:
+    def with_key(self, value: str) -> DeleteGameRecordTTLConfig:
         self.key = value
         return self
 
-    def with_namespace(self, value: str) -> DeleteGameBinaryRecordTTLConfig:
+    def with_namespace(self, value: str) -> DeleteGameRecordTTLConfig:
         self.namespace = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
@@ -177,17 +177,17 @@
 
         400: Bad Request - ModelsResponseError (20002: validation error)
 
         401: Unauthorized - ModelsResponseError (20001: unauthorized access)
 
         403: Forbidden - ModelsResponseError (20013: insufficient permission)
 
-        404: Not Found - ModelsResponseError (18317: record not found)
+        404: Not Found - ModelsResponseError (18003: record not found)
 
-        500: Internal Server Error - ModelsResponseError (20000: internal server error | 18318: unable to update record)
+        500: Internal Server Error - ModelsResponseError (20000: internal server error | 18053: unable to update record)
 
         ---: HttpResponse (Undocumented Response)
 
         ---: HttpResponse (Unexpected Content-Type Error)
 
         ---: HttpResponse (Unhandled Error)
         """
@@ -216,28 +216,26 @@
         )
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
-    def create(
-        cls, key: str, namespace: str, **kwargs
-    ) -> DeleteGameBinaryRecordTTLConfig:
+    def create(cls, key: str, namespace: str, **kwargs) -> DeleteGameRecordTTLConfig:
         instance = cls()
         instance.key = key
         instance.namespace = namespace
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> DeleteGameBinaryRecordTTLConfig:
+    ) -> DeleteGameRecordTTLConfig:
         instance = cls()
         if "key" in dict_ and dict_["key"] is not None:
             instance.key = str(dict_["key"])
         elif include_empty:
             instance.key = ""
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
```

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/operations/ttl_config/delete_game_record_ttl_config.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/operations/admin_player_record/admin_bulk_put_player_r_27d5a1.py`

 * *Files 19% similar despite different names*

```diff
@@ -25,64 +25,67 @@
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
+from ...models import ModelsBulkUpdatePlayerRecordByKeyResponse
+from ...models import ModelsBulkUpdatePlayerRecordsByKeyRequest
 from ...models import ModelsResponseError
 
 
-class DeleteGameRecordTTLConfig(Operation):
-    """Delete game record TTL config (deleteGameRecordTTLConfig)
+class AdminBulkPutPlayerRecordsByKeyHandlerV1(Operation):
+    """Bulk update player records by key (adminBulkPutPlayerRecordsByKeyHandlerV1)
 
-    ## Description
-
-    This endpoints will delete the ttl config of the game record
+    This endpoints will create new player record or replace the existing player record in bulk.
+    Maximum number of user ids per request is 10.
+    Maximum total size of the request payload is 5 MB.
 
     Properties:
-        url: /cloudsave/v1/admin/namespaces/{namespace}/records/{key}/ttl
+        url: /cloudsave/v1/admin/namespaces/{namespace}/users/records/{key}/bulk
 
-        method: DELETE
+        method: PUT
 
-        tags: ["TTLConfig"]
+        tags: ["AdminPlayerRecord"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
+        body: (body) REQUIRED ModelsBulkUpdatePlayerRecordsByKeyRequest in body
+
         key: (key) REQUIRED str in path
 
         namespace: (namespace) REQUIRED str in path
 
     Responses:
-        204: No Content - (TTL config deleted)
+        200: OK - List[ModelsBulkUpdatePlayerRecordByKeyResponse] (OK)
 
-        400: Bad Request - ModelsResponseError (20002: validation error)
+        400: Bad Request - ModelsResponseError (18353: invalid request body | 18356: invalid request body: size of the request body must be less than [%d]MB | 18354: records amount exceeded max limit | 18355: unable to marshal request body)
 
         401: Unauthorized - ModelsResponseError (20001: unauthorized access)
 
         403: Forbidden - ModelsResponseError (20013: insufficient permission)
 
-        404: Not Found - ModelsResponseError (18003: record not found)
-
-        500: Internal Server Error - ModelsResponseError (20000: internal server error | 18053: unable to update record)
+        500: Internal Server Error - ModelsResponseError (20000: internal server error)
     """
 
     # region fields
 
-    _url: str = "/cloudsave/v1/admin/namespaces/{namespace}/records/{key}/ttl"
-    _method: str = "DELETE"
+    _url: str = "/cloudsave/v1/admin/namespaces/{namespace}/users/records/{key}/bulk"
+    _method: str = "PUT"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    body: ModelsBulkUpdatePlayerRecordsByKeyRequest  # REQUIRED in [body]
     key: str  # REQUIRED in [path]
     namespace: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
@@ -116,17 +119,23 @@
 
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
         if hasattr(self, "key"):
             result["key"] = self.key
         if hasattr(self, "namespace"):
             result["namespace"] = self.namespace
         return result
@@ -135,28 +144,38 @@
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_key(self, value: str) -> DeleteGameRecordTTLConfig:
+    def with_body(
+        self, value: ModelsBulkUpdatePlayerRecordsByKeyRequest
+    ) -> AdminBulkPutPlayerRecordsByKeyHandlerV1:
+        self.body = value
+        return self
+
+    def with_key(self, value: str) -> AdminBulkPutPlayerRecordsByKeyHandlerV1:
         self.key = value
         return self
 
-    def with_namespace(self, value: str) -> DeleteGameRecordTTLConfig:
+    def with_namespace(self, value: str) -> AdminBulkPutPlayerRecordsByKeyHandlerV1:
         self.namespace = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
+        if hasattr(self, "body") and self.body:
+            result["body"] = self.body.to_dict(include_empty=include_empty)
+        elif include_empty:
+            result["body"] = ModelsBulkUpdatePlayerRecordsByKeyRequest()
         if hasattr(self, "key") and self.key:
             result["key"] = str(self.key)
         elif include_empty:
             result["key"] = ""
         if hasattr(self, "namespace") and self.namespace:
             result["namespace"] = str(self.namespace)
         elif include_empty:
@@ -166,95 +185,112 @@
     # endregion to methods
 
     # region response methods
 
     # noinspection PyMethodMayBeStatic
     def parse_response(
         self, code: int, content_type: str, content: Any
-    ) -> Tuple[None, Union[None, HttpResponse, ModelsResponseError]]:
+    ) -> Tuple[
+        Union[None, List[ModelsBulkUpdatePlayerRecordByKeyResponse]],
+        Union[None, HttpResponse, ModelsResponseError],
+    ]:
         """Parse the given response.
 
-        204: No Content - (TTL config deleted)
+        200: OK - List[ModelsBulkUpdatePlayerRecordByKeyResponse] (OK)
 
-        400: Bad Request - ModelsResponseError (20002: validation error)
+        400: Bad Request - ModelsResponseError (18353: invalid request body | 18356: invalid request body: size of the request body must be less than [%d]MB | 18354: records amount exceeded max limit | 18355: unable to marshal request body)
 
         401: Unauthorized - ModelsResponseError (20001: unauthorized access)
 
         403: Forbidden - ModelsResponseError (20013: insufficient permission)
 
-        404: Not Found - ModelsResponseError (18003: record not found)
-
-        500: Internal Server Error - ModelsResponseError (20000: internal server error | 18053: unable to update record)
+        500: Internal Server Error - ModelsResponseError (20000: internal server error)
 
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
+            return [
+                ModelsBulkUpdatePlayerRecordByKeyResponse.create_from_dict(i)
+                for i in content
+            ], None
         if code == 400:
             return None, ModelsResponseError.create_from_dict(content)
         if code == 401:
             return None, ModelsResponseError.create_from_dict(content)
         if code == 403:
             return None, ModelsResponseError.create_from_dict(content)
-        if code == 404:
-            return None, ModelsResponseError.create_from_dict(content)
         if code == 500:
             return None, ModelsResponseError.create_from_dict(content)
 
         return self.handle_undocumented_response(
             code=code, content_type=content_type, content=content
         )
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
-    def create(cls, key: str, namespace: str, **kwargs) -> DeleteGameRecordTTLConfig:
+    def create(
+        cls,
+        body: ModelsBulkUpdatePlayerRecordsByKeyRequest,
+        key: str,
+        namespace: str,
+        **kwargs,
+    ) -> AdminBulkPutPlayerRecordsByKeyHandlerV1:
         instance = cls()
+        instance.body = body
         instance.key = key
         instance.namespace = namespace
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> DeleteGameRecordTTLConfig:
+    ) -> AdminBulkPutPlayerRecordsByKeyHandlerV1:
         instance = cls()
+        if "body" in dict_ and dict_["body"] is not None:
+            instance.body = ModelsBulkUpdatePlayerRecordsByKeyRequest.create_from_dict(
+                dict_["body"], include_empty=include_empty
+            )
+        elif include_empty:
+            instance.body = ModelsBulkUpdatePlayerRecordsByKeyRequest()
         if "key" in dict_ and dict_["key"] is not None:
             instance.key = str(dict_["key"])
         elif include_empty:
             instance.key = ""
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
         elif include_empty:
             instance.namespace = ""
         return instance
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
+            "body": "body",
             "key": "key",
             "namespace": "namespace",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
+            "body": True,
             "key": True,
             "namespace": True,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/wrappers/__init__.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/wrappers/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: wrapper-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Cloudsave Service."""
 
-__version__ = "3.15.1"
+__version__ = "3.16.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from ._admin_concurrent_record import admin_put_admin_game_record_concurrent_handler_v1
 from ._admin_concurrent_record import (
@@ -74,14 +74,20 @@
 from ._admin_player_binary_record import admin_post_player_binary_record_v1
 from ._admin_player_binary_record import admin_post_player_binary_record_v1_async
 from ._admin_player_binary_record import admin_put_player_binary_record_v1
 from ._admin_player_binary_record import admin_put_player_binary_record_v1_async
 from ._admin_player_binary_record import admin_put_player_binary_recor_metadata_v1
 from ._admin_player_binary_record import admin_put_player_binary_recor_metadata_v1_async
 
+from ._admin_player_record import admin_bulk_get_player_records_by_user_i_ds_handler_v1
+from ._admin_player_record import (
+    admin_bulk_get_player_records_by_user_i_ds_handler_v1_async,
+)
+from ._admin_player_record import admin_bulk_put_player_records_by_key_handler_v1
+from ._admin_player_record import admin_bulk_put_player_records_by_key_handler_v1_async
 from ._admin_player_record import admin_delete_player_public_record_handler_v1
 from ._admin_player_record import admin_delete_player_public_record_handler_v1_async
 from ._admin_player_record import admin_delete_player_record_handler_v1
 from ._admin_player_record import admin_delete_player_record_handler_v1_async
 from ._admin_player_record import admin_get_player_public_record_handler_v1
 from ._admin_player_record import admin_get_player_public_record_handler_v1_async
 from ._admin_player_record import admin_get_player_record_handler_v1
```

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/wrappers/_admin_concurrent_record.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/wrappers/_admin_concurrent_record.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,19 +100,22 @@
 
 
     ## Parameters Notes
     1. updatedAt (required: true)
     Time format style: RFC3339
     2. value
     Json
+    3. tags (default: *empty array*, type: array of string)
+    Indicate the tagging for the admin record.
     **Request Body Example:**
     ```
     {
     "value": {},
-    "updatedAt": "2022-03-17T10:42:15.444Z"
+    "updatedAt": "2022-03-17T10:42:15.444Z",
+    "tags": ["tag1", "tag2"]
     }
     ```
     ## Optimistic Concurrency Control
 
     This endpoint implement optimistic concurrency control to avoid race condition.
     If the record has been updated since the client fetch it, the server will return HTTP status code 412 (precondition failed)
     and client need to redo the operation (fetch data and do update).
@@ -213,19 +216,22 @@
 
 
     ## Parameters Notes
     1. updatedAt (required: true)
     Time format style: RFC3339
     2. value
     Json
+    3. tags (default: *empty array*, type: array of string)
+    Indicate the tagging for the admin record.
     **Request Body Example:**
     ```
     {
     "value": {},
-    "updatedAt": "2022-03-17T10:42:15.444Z"
+    "updatedAt": "2022-03-17T10:42:15.444Z",
+    "tags": ["tag1", "tag2"]
     }
     ```
     ## Optimistic Concurrency Control
 
     This endpoint implement optimistic concurrency control to avoid race condition.
     If the record has been updated since the client fetch it, the server will return HTTP status code 412 (precondition failed)
     and client need to redo the operation (fetch data and do update).
@@ -330,19 +336,22 @@
 
 
     ## Parameters Notes
     1. updatedAt (required: true)
     Time format style: RFC3339
     2. value
     Json
+    3. tags (default: *empty array*, type: array of string)
+    Indicate the tagging for the admin record.
     **Request Body Example:**
     ```
     {
     "value": {},
-    "updatedAt": "2022-03-17T10:42:15.444Z"
+    "updatedAt": "2022-03-17T10:42:15.444Z",
+    "tags": ["tag1", "tag2"]
     }
     ```
 
     ## Optimistic Concurrency Control
 
     This endpoint implement optimistic concurrency control to avoid race condition.
     If the record has been updated since the client fetch it, the server will return HTTP status code 412 (precondition failed)
@@ -454,19 +463,22 @@
 
 
     ## Parameters Notes
     1. updatedAt (required: true)
     Time format style: RFC3339
     2. value
     Json
+    3. tags (default: *empty array*, type: array of string)
+    Indicate the tagging for the admin record.
     **Request Body Example:**
     ```
     {
     "value": {},
-    "updatedAt": "2022-03-17T10:42:15.444Z"
+    "updatedAt": "2022-03-17T10:42:15.444Z",
+    "tags": ["tag1", "tag2"]
     }
     ```
 
     ## Optimistic Concurrency Control
 
     This endpoint implement optimistic concurrency control to avoid race condition.
     If the record has been updated since the client fetch it, the server will return HTTP status code 412 (precondition failed)
@@ -582,20 +594,23 @@
     Indicate which party that could modify the game record.
     SERVER: record can be modified by server only.
     CLIENT: record can be modified by client and server.
     2. updatedAt (required: true)
     Time format style: RFC3339
     3. value
     Json
+    4. tags (default: *empty array*, type: array of string)
+    Indicate the tagging for the game record.
     **Request Body Example:**
     ```
     {
     "set_by": "SERVER",
     "value": {},
-    "updatedAt": "2022-03-17T10:42:15.444Z"
+    "updatedAt": "2022-03-17T10:42:15.444Z",
+    "tags": ["tag1", "tag2"]
     }
     ```
     ## Optimistic Concurrency Control
 
     This endpoint implement optimistic concurrency control to avoid race condition.
     If the record has been updated since the client fetch it, the server will return HTTP status code 412 (precondition failed)
     and client need to redo the operation (fetch data and do update).
@@ -703,20 +718,23 @@
     Indicate which party that could modify the game record.
     SERVER: record can be modified by server only.
     CLIENT: record can be modified by client and server.
     2. updatedAt (required: true)
     Time format style: RFC3339
     3. value
     Json
+    4. tags (default: *empty array*, type: array of string)
+    Indicate the tagging for the game record.
     **Request Body Example:**
     ```
     {
     "set_by": "SERVER",
     "value": {},
-    "updatedAt": "2022-03-17T10:42:15.444Z"
+    "updatedAt": "2022-03-17T10:42:15.444Z",
+    "tags": ["tag1", "tag2"]
     }
     ```
     ## Optimistic Concurrency Control
 
     This endpoint implement optimistic concurrency control to avoid race condition.
     If the record has been updated since the client fetch it, the server will return HTTP status code 412 (precondition failed)
     and client need to redo the operation (fetch data and do update).
@@ -828,20 +846,23 @@
     Indicate which party that could modify the game record.
     SERVER: record can be modified by server only.
     CLIENT: record can be modified by client and server.
     2. updatedAt (required: true)
     Time format style: RFC3339
     3. value
     Json
+    4. tags (default: *empty array*, type: array of string)
+    Indicate the tagging for the game record.
     **Request Body Example:**
     ```
     {
     "set_by": "SERVER",
     "value": {},
-    "updatedAt": "2022-03-17T10:42:15.444Z"
+    "updatedAt": "2022-03-17T10:42:15.444Z",
+    "tags": ["tag1", "tag2"]
     }
     ```
 
     ## Optimistic Concurrency Control
 
     This endpoint implement optimistic concurrency control to avoid race condition.
     If the record has been updated since the client fetch it, the server will return HTTP status code 412 (precondition failed)
@@ -960,20 +981,23 @@
     Indicate which party that could modify the game record.
     SERVER: record can be modified by server only.
     CLIENT: record can be modified by client and server.
     2. updatedAt (required: true)
     Time format style: RFC3339
     3. value
     Json
+    4. tags (default: *empty array*, type: array of string)
+    Indicate the tagging for the game record.
     **Request Body Example:**
     ```
     {
     "set_by": "SERVER",
     "value": {},
-    "updatedAt": "2022-03-17T10:42:15.444Z"
+    "updatedAt": "2022-03-17T10:42:15.444Z",
+    "tags": ["tag1", "tag2"]
     }
     ```
 
     ## Optimistic Concurrency Control
 
     This endpoint implement optimistic concurrency control to avoid race condition.
     If the record has been updated since the client fetch it, the server will return HTTP status code 412 (precondition failed)
@@ -1094,20 +1118,23 @@
     Indicate which party that could modify the game record.
     SERVER: record can be modified by server only.
     CLIENT: record can be modified by client and server.
     2. updatedAt (required: true)
     Time format style: RFC3339
     3. value
     Json
+    4. tags (default: *empty array*, type: array of string)
+    Indicate the tagging for the game record.
     **Request Body Example:**
     ```
     {
     "set_by": "SERVER",
     "value": {},
-    "updatedAt": "2022-03-17T10:42:15.444Z"
+    "updatedAt": "2022-03-17T10:42:15.444Z",
+    "tags": ["tag1", "tag2"]
     }
     ```
 
     ## Optimistic Concurrency Control
 
     This endpoint implement optimistic concurrency control to avoid race condition.
     If the record has been updated since the client fetch it, the server will return HTTP status code 412 (precondition failed)
@@ -1226,20 +1253,23 @@
     Indicate which party that could modify the game record.
     SERVER: record can be modified by server only.
     CLIENT: record can be modified by client and server.
     2. updatedAt (required: true)
     Time format style: RFC3339
     3. value
     Json
+    4. tags (default: *empty array*, type: array of string)
+    Indicate the tagging for the game record.
     **Request Body Example:**
     ```
     {
     "set_by": "SERVER",
     "value": {},
-    "updatedAt": "2022-03-17T10:42:15.444Z"
+    "updatedAt": "2022-03-17T10:42:15.444Z",
+    "tags": ["tag1", "tag2"]
     }
     ```
 
     ## Optimistic Concurrency Control
 
     This endpoint implement optimistic concurrency control to avoid race condition.
     If the record has been updated since the client fetch it, the server will return HTTP status code 412 (precondition failed)
```

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/wrappers/_admin_game_binary_record.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/wrappers/_admin_game_binary_record.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/wrappers/_admin_game_record.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/wrappers/_admin_game_record.py`

 * *Files 3% similar despite different names*

```diff
@@ -312,24 +312,27 @@
     Indicate which party that could modify the game record.
     SERVER: record can be modified by server only.
     CLIENT: record can be modified by client and server.
     2. ttl_config (default: *empty*, type: object)
     Indicate the TTL configuration for the game record.
     action:
     - DELETE: record will be deleted after TTL is reached
+    3. tags (default: *empty array*, type: array of string)
+    Indicate the tagging for the game record.
 
     **Request Body Example:**
     ```
     {
     "__META": {
     "set_by": "SERVER",
     "ttl_config": {
     "expires_at": "2026-01-02T15:04:05Z", // should be in RFC3339 format
     "action": "DELETE"
-    }
+    },
+    "tags": ["tag1", "tag2"]
     }
     ...
     }
     ```
 
     Required Permission(s):
         - CLIENT []
@@ -442,24 +445,27 @@
     Indicate which party that could modify the game record.
     SERVER: record can be modified by server only.
     CLIENT: record can be modified by client and server.
     2. ttl_config (default: *empty*, type: object)
     Indicate the TTL configuration for the game record.
     action:
     - DELETE: record will be deleted after TTL is reached
+    3. tags (default: *empty array*, type: array of string)
+    Indicate the tagging for the game record.
 
     **Request Body Example:**
     ```
     {
     "__META": {
     "set_by": "SERVER",
     "ttl_config": {
     "expires_at": "2026-01-02T15:04:05Z", // should be in RFC3339 format
     "action": "DELETE"
-    }
+    },
+    "tags": ["tag1", "tag2"]
     }
     ...
     }
     ```
 
     Required Permission(s):
         - CLIENT []
@@ -562,24 +568,27 @@
     Indicate which party that could modify the game record.
     SERVER: record can be modified by server only.
     CLIENT: record can be modified by client and server.
     2. ttl_config (default: *empty*, type: object)
     Indicate the TTL configuration for the game record.
     action:
     - DELETE: record will be deleted after TTL is reached
+    3. tags (default: *empty array*, type: array of string)
+    Indicate the tagging for the game record.
 
     **Request Body Example:**
     ```
     {
     "__META": {
     "set_by": "SERVER",
     "ttl_config": {
     "expires_at": "2026-01-02T15:04:05Z", // should be in RFC3339 format
     "action": "DELETE"
-    }
+    },
+    "tags": ["tag1", "tag2"]
     }
     ...
     }
     ```
 
     Required Permission(s):
         - CLIENT []
@@ -680,24 +689,27 @@
     Indicate which party that could modify the game record.
     SERVER: record can be modified by server only.
     CLIENT: record can be modified by client and server.
     2. ttl_config (default: *empty*, type: object)
     Indicate the TTL configuration for the game record.
     action:
     - DELETE: record will be deleted after TTL is reached
+    3. tags (default: *empty array*, type: array of string)
+    Indicate the tagging for the game record.
 
     **Request Body Example:**
     ```
     {
     "__META": {
     "set_by": "SERVER",
     "ttl_config": {
     "expires_at": "2026-01-02T15:04:05Z", // should be in RFC3339 format
     "action": "DELETE"
-    }
+    },
+    "tags": ["tag1", "tag2"]
     }
     ...
     }
     ```
 
     Required Permission(s):
         - CLIENT []
```

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/wrappers/_admin_player_binary_record.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/wrappers/_admin_player_binary_record.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/wrappers/_admin_player_record.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/wrappers/_admin_player_record.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,25 +27,31 @@
 from accelbyte_py_sdk.core import get_namespace as get_services_namespace
 from accelbyte_py_sdk.core import run_request
 from accelbyte_py_sdk.core import run_request_async
 from accelbyte_py_sdk.core import deprecated
 from accelbyte_py_sdk.core import same_doc_as
 
 from ..models import ModelsBulkGetAdminPlayerRecordResponse
+from ..models import ModelsBulkGetPlayerRecordResponse
 from ..models import ModelsBulkGetPlayerRecordSizeResponse
 from ..models import ModelsBulkGetPlayerRecordsRequest
+from ..models import ModelsBulkUpdatePlayerRecordByKeyResponse
 from ..models import ModelsBulkUpdatePlayerRecordResponse
+from ..models import ModelsBulkUpdatePlayerRecordsByKeyRequest
 from ..models import ModelsBulkUpdatePlayerRecordsRequest
+from ..models import ModelsBulkUserIDsRequest
 from ..models import ModelsBulkUserKeyRequest
 from ..models import ModelsListPlayerRecordKeysResponse
 from ..models import ModelsPlayerRecordRequest
 from ..models import ModelsPlayerRecordResponse
 from ..models import ModelsPlayerRecordSizeResponse
 from ..models import ModelsResponseError
 
+from ..operations.admin_player_record import AdminBulkGetPlayerRecordsByUserIDsHandlerV1
+from ..operations.admin_player_record import AdminBulkPutPlayerRecordsByKeyHandlerV1
 from ..operations.admin_player_record import AdminDeletePlayerPublicRecordHandlerV1
 from ..operations.admin_player_record import AdminDeletePlayerRecordHandlerV1
 from ..operations.admin_player_record import AdminGetPlayerPublicRecordHandlerV1
 from ..operations.admin_player_record import AdminGetPlayerRecordHandlerV1
 from ..operations.admin_player_record import AdminGetPlayerRecordsHandlerV1
 from ..operations.admin_player_record import AdminGetPlayerRecordSizeHandlerV1
 from ..operations.admin_player_record import AdminPostPlayerPublicRecordHandlerV1
@@ -55,14 +61,240 @@
 from ..operations.admin_player_record import AdminPutPlayerRecordsHandlerV1
 from ..operations.admin_player_record import AdminRetrievePlayerRecords
 from ..operations.admin_player_record import BulkGetPlayerRecordSizeHandlerV1
 from ..operations.admin_player_record import ListPlayerRecordHandlerV1
 from ..models import ModelsPlayerRecordResponseSetByEnum
 
 
+@same_doc_as(AdminBulkGetPlayerRecordsByUserIDsHandlerV1)
+def admin_bulk_get_player_records_by_user_i_ds_handler_v1(
+    body: ModelsBulkUserIDsRequest,
+    key: str,
+    namespace: Optional[str] = None,
+    x_additional_headers: Optional[Dict[str, str]] = None,
+    **kwargs
+):
+    """Bulk get player records by multiple user ids (adminBulkGetPlayerRecordsByUserIDsHandlerV1)
+
+    Retrieve player record key and payload in bulk under given namespace.
+    Maximum number of user ids per request is 20.
+
+    Properties:
+        url: /cloudsave/v1/admin/namespaces/{namespace}/users/records/{key}/bulk
+
+        method: POST
+
+        tags: ["AdminPlayerRecord"]
+
+        consumes: ["application/json"]
+
+        produces: ["application/json"]
+
+        securities: [BEARER_AUTH]
+
+        body: (body) REQUIRED ModelsBulkUserIDsRequest in body
+
+        key: (key) REQUIRED str in path
+
+        namespace: (namespace) REQUIRED str in path
+
+    Responses:
+        200: OK - ModelsBulkGetPlayerRecordResponse (OK)
+
+        400: Bad Request - ModelsResponseError (18125: invalid request body | 18126: request record keys list exceed max size [%d])
+
+        401: Unauthorized - ModelsResponseError (20001: unauthorized access)
+
+        403: Forbidden - ModelsResponseError (20013: insufficient permission)
+
+        500: Internal Server Error - ModelsResponseError (18124: unable to get record | 18006: unable to decode record)
+    """
+    if namespace is None:
+        namespace, error = get_services_namespace()
+        if error:
+            return None, error
+    request = AdminBulkGetPlayerRecordsByUserIDsHandlerV1.create(
+        body=body,
+        key=key,
+        namespace=namespace,
+    )
+    return run_request(request, additional_headers=x_additional_headers, **kwargs)
+
+
+@same_doc_as(AdminBulkGetPlayerRecordsByUserIDsHandlerV1)
+async def admin_bulk_get_player_records_by_user_i_ds_handler_v1_async(
+    body: ModelsBulkUserIDsRequest,
+    key: str,
+    namespace: Optional[str] = None,
+    x_additional_headers: Optional[Dict[str, str]] = None,
+    **kwargs
+):
+    """Bulk get player records by multiple user ids (adminBulkGetPlayerRecordsByUserIDsHandlerV1)
+
+    Retrieve player record key and payload in bulk under given namespace.
+    Maximum number of user ids per request is 20.
+
+    Properties:
+        url: /cloudsave/v1/admin/namespaces/{namespace}/users/records/{key}/bulk
+
+        method: POST
+
+        tags: ["AdminPlayerRecord"]
+
+        consumes: ["application/json"]
+
+        produces: ["application/json"]
+
+        securities: [BEARER_AUTH]
+
+        body: (body) REQUIRED ModelsBulkUserIDsRequest in body
+
+        key: (key) REQUIRED str in path
+
+        namespace: (namespace) REQUIRED str in path
+
+    Responses:
+        200: OK - ModelsBulkGetPlayerRecordResponse (OK)
+
+        400: Bad Request - ModelsResponseError (18125: invalid request body | 18126: request record keys list exceed max size [%d])
+
+        401: Unauthorized - ModelsResponseError (20001: unauthorized access)
+
+        403: Forbidden - ModelsResponseError (20013: insufficient permission)
+
+        500: Internal Server Error - ModelsResponseError (18124: unable to get record | 18006: unable to decode record)
+    """
+    if namespace is None:
+        namespace, error = get_services_namespace()
+        if error:
+            return None, error
+    request = AdminBulkGetPlayerRecordsByUserIDsHandlerV1.create(
+        body=body,
+        key=key,
+        namespace=namespace,
+    )
+    return await run_request_async(
+        request, additional_headers=x_additional_headers, **kwargs
+    )
+
+
+@same_doc_as(AdminBulkPutPlayerRecordsByKeyHandlerV1)
+def admin_bulk_put_player_records_by_key_handler_v1(
+    body: ModelsBulkUpdatePlayerRecordsByKeyRequest,
+    key: str,
+    namespace: Optional[str] = None,
+    x_additional_headers: Optional[Dict[str, str]] = None,
+    **kwargs
+):
+    """Bulk update player records by key (adminBulkPutPlayerRecordsByKeyHandlerV1)
+
+    This endpoints will create new player record or replace the existing player record in bulk.
+    Maximum number of user ids per request is 10.
+    Maximum total size of the request payload is 5 MB.
+
+    Properties:
+        url: /cloudsave/v1/admin/namespaces/{namespace}/users/records/{key}/bulk
+
+        method: PUT
+
+        tags: ["AdminPlayerRecord"]
+
+        consumes: ["application/json"]
+
+        produces: ["application/json"]
+
+        securities: [BEARER_AUTH]
+
+        body: (body) REQUIRED ModelsBulkUpdatePlayerRecordsByKeyRequest in body
+
+        key: (key) REQUIRED str in path
+
+        namespace: (namespace) REQUIRED str in path
+
+    Responses:
+        200: OK - List[ModelsBulkUpdatePlayerRecordByKeyResponse] (OK)
+
+        400: Bad Request - ModelsResponseError (18353: invalid request body | 18356: invalid request body: size of the request body must be less than [%d]MB | 18354: records amount exceeded max limit | 18355: unable to marshal request body)
+
+        401: Unauthorized - ModelsResponseError (20001: unauthorized access)
+
+        403: Forbidden - ModelsResponseError (20013: insufficient permission)
+
+        500: Internal Server Error - ModelsResponseError (20000: internal server error)
+    """
+    if namespace is None:
+        namespace, error = get_services_namespace()
+        if error:
+            return None, error
+    request = AdminBulkPutPlayerRecordsByKeyHandlerV1.create(
+        body=body,
+        key=key,
+        namespace=namespace,
+    )
+    return run_request(request, additional_headers=x_additional_headers, **kwargs)
+
+
+@same_doc_as(AdminBulkPutPlayerRecordsByKeyHandlerV1)
+async def admin_bulk_put_player_records_by_key_handler_v1_async(
+    body: ModelsBulkUpdatePlayerRecordsByKeyRequest,
+    key: str,
+    namespace: Optional[str] = None,
+    x_additional_headers: Optional[Dict[str, str]] = None,
+    **kwargs
+):
+    """Bulk update player records by key (adminBulkPutPlayerRecordsByKeyHandlerV1)
+
+    This endpoints will create new player record or replace the existing player record in bulk.
+    Maximum number of user ids per request is 10.
+    Maximum total size of the request payload is 5 MB.
+
+    Properties:
+        url: /cloudsave/v1/admin/namespaces/{namespace}/users/records/{key}/bulk
+
+        method: PUT
+
+        tags: ["AdminPlayerRecord"]
+
+        consumes: ["application/json"]
+
+        produces: ["application/json"]
+
+        securities: [BEARER_AUTH]
+
+        body: (body) REQUIRED ModelsBulkUpdatePlayerRecordsByKeyRequest in body
+
+        key: (key) REQUIRED str in path
+
+        namespace: (namespace) REQUIRED str in path
+
+    Responses:
+        200: OK - List[ModelsBulkUpdatePlayerRecordByKeyResponse] (OK)
+
+        400: Bad Request - ModelsResponseError (18353: invalid request body | 18356: invalid request body: size of the request body must be less than [%d]MB | 18354: records amount exceeded max limit | 18355: unable to marshal request body)
+
+        401: Unauthorized - ModelsResponseError (20001: unauthorized access)
+
+        403: Forbidden - ModelsResponseError (20013: insufficient permission)
+
+        500: Internal Server Error - ModelsResponseError (20000: internal server error)
+    """
+    if namespace is None:
+        namespace, error = get_services_namespace()
+        if error:
+            return None, error
+    request = AdminBulkPutPlayerRecordsByKeyHandlerV1.create(
+        body=body,
+        key=key,
+        namespace=namespace,
+    )
+    return await run_request_async(
+        request, additional_headers=x_additional_headers, **kwargs
+    )
+
+
 @same_doc_as(AdminDeletePlayerPublicRecordHandlerV1)
 def admin_delete_player_public_record_handler_v1(
     key: str,
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
@@ -1030,21 +1262,24 @@
     **Metadata List:**
     1. set_by (default: CLIENT, type: string)
     Indicate which party that could modify the game record.
     SERVER: record can be modified by server only.
     CLIENT: record can be modified by client and server.
     2. is_public (default: false, type: bool)
     Indicate whether the player record is a public record or not.
+    3. tags (default: *empty array*, type: array of string)
+    Indicate the tagging for the game record.
 
     **Request Body Example:**
     ```
     {
     "__META": {
     "set_by": "SERVER",
-    "is_public": true
+    "is_public": true,
+    "tags": ["tag1", "tag2"]
     }
     ...
     }
     ```
 
     Required Permission(s):
         - CLIENT []
@@ -1159,21 +1394,24 @@
     **Metadata List:**
     1. set_by (default: CLIENT, type: string)
     Indicate which party that could modify the game record.
     SERVER: record can be modified by server only.
     CLIENT: record can be modified by client and server.
     2. is_public (default: false, type: bool)
     Indicate whether the player record is a public record or not.
+    3. tags (default: *empty array*, type: array of string)
+    Indicate the tagging for the game record.
 
     **Request Body Example:**
     ```
     {
     "__META": {
     "set_by": "SERVER",
-    "is_public": true
+    "is_public": true,
+    "tags": ["tag1", "tag2"]
     }
     ...
     }
     ```
 
     Required Permission(s):
         - CLIENT []
@@ -1474,21 +1712,24 @@
     **Metadata List:**
     1. set_by (default: CLIENT, type: string)
     Indicate which party that could modify the game record.
     SERVER: record can be modified by server only.
     CLIENT: record can be modified by client and server.
     2. is_public (default: false, type: bool)
     Indicate whether the player record is a public record or not.
+    3. tags (default: *empty array*, type: array of string)
+    Indicate the tagging for the game record.
 
     **Request Body Example:**
     ```
     {
     "__META": {
     "set_by": "SERVER",
-    "is_public": true
+    "is_public": true,
+    "tags": ["tag1", "tag2"]
     }
     ...
     }
     ```
 
     Required Permission(s):
         - CLIENT []
@@ -1591,21 +1832,24 @@
     **Metadata List:**
     1. set_by (default: CLIENT, type: string)
     Indicate which party that could modify the game record.
     SERVER: record can be modified by server only.
     CLIENT: record can be modified by client and server.
     2. is_public (default: false, type: bool)
     Indicate whether the player record is a public record or not.
+    3. tags (default: *empty array*, type: array of string)
+    Indicate the tagging for the game record.
 
     **Request Body Example:**
     ```
     {
     "__META": {
     "set_by": "SERVER",
-    "is_public": true
+    "is_public": true,
+    "tags": ["tag1", "tag2"]
     }
     ...
     }
     ```
 
     Required Permission(s):
         - CLIENT []
@@ -1688,15 +1932,15 @@
         namespace: (namespace) REQUIRED str in path
 
         user_id: (userId) REQUIRED str in path
 
     Responses:
         200: OK - List[ModelsBulkUpdatePlayerRecordResponse] (OK)
 
-        400: Bad Request - ModelsResponseError (18353: invalid request body | 18356: invalid request body: size of the request body must be less than [%d]MB | 18354: records amount exceeded max limit | 18355: unable to marshal request body | 18355: unable to marshal request body)
+        400: Bad Request - ModelsResponseError (18353: invalid request body | 18356: invalid request body: size of the request body must be less than [%d]MB | 18354: records amount exceeded max limit | 18355: unable to marshal request body)
 
         401: Unauthorized - ModelsResponseError (20001: unauthorized access)
 
         403: Forbidden - ModelsResponseError (20013: insufficient permission)
     """
     if namespace is None:
         namespace, error = get_services_namespace()
@@ -1741,15 +1985,15 @@
         namespace: (namespace) REQUIRED str in path
 
         user_id: (userId) REQUIRED str in path
 
     Responses:
         200: OK - List[ModelsBulkUpdatePlayerRecordResponse] (OK)
 
-        400: Bad Request - ModelsResponseError (18353: invalid request body | 18356: invalid request body: size of the request body must be less than [%d]MB | 18354: records amount exceeded max limit | 18355: unable to marshal request body | 18355: unable to marshal request body)
+        400: Bad Request - ModelsResponseError (18353: invalid request body | 18356: invalid request body: size of the request body must be less than [%d]MB | 18354: records amount exceeded max limit | 18355: unable to marshal request body)
 
         401: Unauthorized - ModelsResponseError (20001: unauthorized access)
 
         403: Forbidden - ModelsResponseError (20013: insufficient permission)
     """
     if namespace is None:
         namespace, error = get_services_namespace()
```

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/wrappers/_admin_record.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/wrappers/_admin_record.py`

 * *Files 9% similar despite different names*

```diff
@@ -986,14 +986,36 @@
     1. Cannot use **"."** as the key name
     - `{ "data.2": "value" }`
     2. Cannot use **"$"** as the prefix in key names
     - `{ "$data": "value" }`
     3. Cannot use empty string in key names
     - `{ "": "value" }`
 
+
+    ## Record Metadata
+
+    Metadata allows user to define the behaviour of the record.
+    Metadata can be defined in request body with field name **__META**.
+    When creating record, if **__META** field is not defined, the metadata value will use the default value.
+    When updating record, if **__META** field is not defined, the existing metadata value will stay as is.
+
+    **Metadata List:**
+    1. tags (default: *empty array*, type: array of string)
+    Indicate the tagging for the admin record.
+
+    **Request Body Example:**
+    ```
+    {
+    "__META": {
+    "tags": ["tag1", "tag2"]
+    }
+    ...
+    }
+    ```
+
     Properties:
         url: /cloudsave/v1/admin/namespaces/{namespace}/adminrecords/{key}
 
         method: POST
 
         tags: ["AdminRecord"]
 
@@ -1081,14 +1103,36 @@
     1. Cannot use **"."** as the key name
     - `{ "data.2": "value" }`
     2. Cannot use **"$"** as the prefix in key names
     - `{ "$data": "value" }`
     3. Cannot use empty string in key names
     - `{ "": "value" }`
 
+
+    ## Record Metadata
+
+    Metadata allows user to define the behaviour of the record.
+    Metadata can be defined in request body with field name **__META**.
+    When creating record, if **__META** field is not defined, the metadata value will use the default value.
+    When updating record, if **__META** field is not defined, the existing metadata value will stay as is.
+
+    **Metadata List:**
+    1. tags (default: *empty array*, type: array of string)
+    Indicate the tagging for the admin record.
+
+    **Request Body Example:**
+    ```
+    {
+    "__META": {
+    "tags": ["tag1", "tag2"]
+    }
+    ...
+    }
+    ```
+
     Properties:
         url: /cloudsave/v1/admin/namespaces/{namespace}/adminrecords/{key}
 
         method: POST
 
         tags: ["AdminRecord"]
 
@@ -1179,14 +1223,36 @@
     1. Cannot use **"."** as the key name
     - `{ "data.2": "value" }`
     2. Cannot use **"$"** as the prefix in key names
     - `{ "$data": "value" }`
     3. Cannot use empty string in key names
     - `{ "": "value" }`
 
+
+    ## Record Metadata
+
+    Metadata allows user to define the behaviour of the record.
+    Metadata can be defined in request body with field name **__META**.
+    When creating record, if **__META** field is not defined, the metadata value will use the default value.
+    When updating record, if **__META** field is not defined, the existing metadata value will stay as is.
+
+    **Metadata List:**
+    1. tags (default: *empty array*, type: array of string)
+    Indicate the tagging for the admin record.
+
+    **Request Body Example:**
+    ```
+    {
+    "__META": {
+    "tags": ["tag1", "tag2"]
+    }
+    ...
+    }
+    ```
+
     Properties:
         url: /cloudsave/v1/admin/namespaces/{namespace}/users/{userId}/adminrecords/{key}
 
         method: POST
 
         tags: ["AdminRecord"]
 
@@ -1278,14 +1344,36 @@
     1. Cannot use **"."** as the key name
     - `{ "data.2": "value" }`
     2. Cannot use **"$"** as the prefix in key names
     - `{ "$data": "value" }`
     3. Cannot use empty string in key names
     - `{ "": "value" }`
 
+
+    ## Record Metadata
+
+    Metadata allows user to define the behaviour of the record.
+    Metadata can be defined in request body with field name **__META**.
+    When creating record, if **__META** field is not defined, the metadata value will use the default value.
+    When updating record, if **__META** field is not defined, the existing metadata value will stay as is.
+
+    **Metadata List:**
+    1. tags (default: *empty array*, type: array of string)
+    Indicate the tagging for the admin record.
+
+    **Request Body Example:**
+    ```
+    {
+    "__META": {
+    "tags": ["tag1", "tag2"]
+    }
+    ...
+    }
+    ```
+
     Properties:
         url: /cloudsave/v1/admin/namespaces/{namespace}/users/{userId}/adminrecords/{key}
 
         method: POST
 
         tags: ["AdminRecord"]
 
@@ -1365,14 +1453,36 @@
     1. Cannot use **"."** as the key name
     - `{ "data.2": "value" }`
     2. Cannot use **"$"** as the prefix in key names
     - `{ "$data": "value" }`
     3. Cannot use empty string in key names
     - `{ "": "value" }`
 
+
+    ## Record Metadata
+
+    Metadata allows user to define the behaviour of the record.
+    Metadata can be defined in request body with field name **__META**.
+    When creating record, if **__META** field is not defined, the metadata value will use the default value.
+    When updating record, if **__META** field is not defined, the existing metadata value will stay as is.
+
+    **Metadata List:**
+    1. tags (default: *empty array*, type: array of string)
+    Indicate the tagging for the admin record.
+
+    **Request Body Example:**
+    ```
+    {
+    "__META": {
+    "tags": ["tag1", "tag2"]
+    }
+    ...
+    }
+    ```
+
     Properties:
         url: /cloudsave/v1/admin/namespaces/{namespace}/adminrecords/{key}
 
         method: PUT
 
         tags: ["AdminRecord"]
 
@@ -1447,14 +1557,36 @@
     1. Cannot use **"."** as the key name
     - `{ "data.2": "value" }`
     2. Cannot use **"$"** as the prefix in key names
     - `{ "$data": "value" }`
     3. Cannot use empty string in key names
     - `{ "": "value" }`
 
+
+    ## Record Metadata
+
+    Metadata allows user to define the behaviour of the record.
+    Metadata can be defined in request body with field name **__META**.
+    When creating record, if **__META** field is not defined, the metadata value will use the default value.
+    When updating record, if **__META** field is not defined, the existing metadata value will stay as is.
+
+    **Metadata List:**
+    1. tags (default: *empty array*, type: array of string)
+    Indicate the tagging for the admin record.
+
+    **Request Body Example:**
+    ```
+    {
+    "__META": {
+    "tags": ["tag1", "tag2"]
+    }
+    ...
+    }
+    ```
+
     Properties:
         url: /cloudsave/v1/admin/namespaces/{namespace}/adminrecords/{key}
 
         method: PUT
 
         tags: ["AdminRecord"]
 
@@ -1533,14 +1665,36 @@
     1. Cannot use **"."** as the key name
     - `{ "data.2": "value" }`
     2. Cannot use **"$"** as the prefix in key names
     - `{ "$data": "value" }`
     3. Cannot use empty string in key names
     - `{ "": "value" }`
 
+
+    ## Record Metadata
+
+    Metadata allows user to define the behaviour of the record.
+    Metadata can be defined in request body with field name **__META**.
+    When creating record, if **__META** field is not defined, the metadata value will use the default value.
+    When updating record, if **__META** field is not defined, the existing metadata value will stay as is.
+
+    **Metadata List:**
+    1. tags (default: *empty array*, type: array of string)
+    Indicate the tagging for the admin record.
+
+    **Request Body Example:**
+    ```
+    {
+    "__META": {
+    "tags": ["tag1", "tag2"]
+    }
+    ...
+    }
+    ```
+
     Properties:
         url: /cloudsave/v1/admin/namespaces/{namespace}/users/{userId}/adminrecords/{key}
 
         method: PUT
 
         tags: ["AdminRecord"]
 
@@ -1620,14 +1774,36 @@
     1. Cannot use **"."** as the key name
     - `{ "data.2": "value" }`
     2. Cannot use **"$"** as the prefix in key names
     - `{ "$data": "value" }`
     3. Cannot use empty string in key names
     - `{ "": "value" }`
 
+
+    ## Record Metadata
+
+    Metadata allows user to define the behaviour of the record.
+    Metadata can be defined in request body with field name **__META**.
+    When creating record, if **__META** field is not defined, the metadata value will use the default value.
+    When updating record, if **__META** field is not defined, the existing metadata value will stay as is.
+
+    **Metadata List:**
+    1. tags (default: *empty array*, type: array of string)
+    Indicate the tagging for the admin record.
+
+    **Request Body Example:**
+    ```
+    {
+    "__META": {
+    "tags": ["tag1", "tag2"]
+    }
+    ...
+    }
+    ```
+
     Properties:
         url: /cloudsave/v1/admin/namespaces/{namespace}/users/{userId}/adminrecords/{key}
 
         method: PUT
 
         tags: ["AdminRecord"]
```

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/wrappers/_admin_tags.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/wrappers/_admin_tags.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/wrappers/_concurrent_record.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/wrappers/_concurrent_record.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/wrappers/_plugin_config.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/wrappers/_plugin_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/wrappers/_public_game_binary_record.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/wrappers/_public_game_binary_record.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/wrappers/_public_game_record.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/wrappers/_public_game_record.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/wrappers/_public_player_binary_record.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/wrappers/_public_player_binary_record.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/wrappers/_public_player_record.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/wrappers/_public_player_record.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/wrappers/_public_tags.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/wrappers/_public_tags.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk/api/cloudsave/wrappers/_ttl_config.py` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk/api/cloudsave/wrappers/_ttl_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk_service_cloudsave.egg-info/PKG-INFO` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk_service_cloudsave.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: accelbyte-py-sdk-service-cloudsave
-Version: 0.8.0
+Version: 0.9.0
 Summary: AccelByte Python SDK - AccelByte Gaming Services Cloudsave Service
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: accelbyte-py-sdk-core
 
 [//]: # (Code generated. DO NOT EDIT!)
 
 # AccelByte Modular Python SDK - Service Module
 
 This is a service module for the [AccelByte Modular Python SDK](https://github.com/AccelByte/accelbyte-python-modular-sdk) package.
 
 ```text
 AccelByte Gaming Services Cloudsave Service
-* Version: 3.15.1
+* Version: 3.16.0
 ```
 
 ## Setup
 
 This SDK requires Python 3.9 to be installed.
 
 ### Install with Pip
```

### Comparing `accelbyte-py-sdk-service-cloudsave-0.8.0/accelbyte_py_sdk_service_cloudsave.egg-info/SOURCES.txt` & `accelbyte-py-sdk-service-cloudsave-0.9.0/accelbyte_py_sdk_service_cloudsave.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -20,16 +20,19 @@
 accelbyte_py_sdk/api/cloudsave/models/models_bulk_get_game_binary_record_response.py
 accelbyte_py_sdk/api/cloudsave/models/models_bulk_get_game_record_request.py
 accelbyte_py_sdk/api/cloudsave/models/models_bulk_get_game_record_response.py
 accelbyte_py_sdk/api/cloudsave/models/models_bulk_get_player_binary_record_response.py
 accelbyte_py_sdk/api/cloudsave/models/models_bulk_get_player_record_response.py
 accelbyte_py_sdk/api/cloudsave/models/models_bulk_get_player_record_size_response.py
 accelbyte_py_sdk/api/cloudsave/models/models_bulk_get_player_records_request.py
+accelbyte_py_sdk/api/cloudsave/models/models_bulk_update_player_record_by_key_request_detail.py
+accelbyte_py_sdk/api/cloudsave/models/models_bulk_update_player_record_by_key_response.py
 accelbyte_py_sdk/api/cloudsave/models/models_bulk_update_player_record_request_detail.py
 accelbyte_py_sdk/api/cloudsave/models/models_bulk_update_player_record_response.py
+accelbyte_py_sdk/api/cloudsave/models/models_bulk_update_player_records_by_key_request.py
 accelbyte_py_sdk/api/cloudsave/models/models_bulk_update_player_records_request.py
 accelbyte_py_sdk/api/cloudsave/models/models_bulk_user_i_ds_request.py
 accelbyte_py_sdk/api/cloudsave/models/models_bulk_user_key_request.py
 accelbyte_py_sdk/api/cloudsave/models/models_concurrent_record_request.py
 accelbyte_py_sdk/api/cloudsave/models/models_custom_config.py
 accelbyte_py_sdk/api/cloudsave/models/models_custom_function.py
 accelbyte_py_sdk/api/cloudsave/models/models_game_binary_record_admin_response.py
@@ -94,14 +97,16 @@
 accelbyte_py_sdk/api/cloudsave/operations/admin_player_binary_record/admin_get_player_binary_1076b9.py
 accelbyte_py_sdk/api/cloudsave/operations/admin_player_binary_record/admin_list_player_binar_e452ce.py
 accelbyte_py_sdk/api/cloudsave/operations/admin_player_binary_record/admin_post_player_binar_e33f40.py
 accelbyte_py_sdk/api/cloudsave/operations/admin_player_binary_record/admin_post_player_binar_f1a4e9.py
 accelbyte_py_sdk/api/cloudsave/operations/admin_player_binary_record/admin_put_player_binary_6424e4.py
 accelbyte_py_sdk/api/cloudsave/operations/admin_player_binary_record/admin_put_player_binary_bcf941.py
 accelbyte_py_sdk/api/cloudsave/operations/admin_player_record/__init__.py
+accelbyte_py_sdk/api/cloudsave/operations/admin_player_record/admin_bulk_get_player_r_82c596.py
+accelbyte_py_sdk/api/cloudsave/operations/admin_player_record/admin_bulk_put_player_r_27d5a1.py
 accelbyte_py_sdk/api/cloudsave/operations/admin_player_record/admin_delete_player_pub_f11fd7.py
 accelbyte_py_sdk/api/cloudsave/operations/admin_player_record/admin_delete_player_rec_168241.py
 accelbyte_py_sdk/api/cloudsave/operations/admin_player_record/admin_get_player_public_f015b6.py
 accelbyte_py_sdk/api/cloudsave/operations/admin_player_record/admin_get_player_record_b37faa.py
 accelbyte_py_sdk/api/cloudsave/operations/admin_player_record/admin_get_player_record_d622c9.py
 accelbyte_py_sdk/api/cloudsave/operations/admin_player_record/admin_get_player_record_f4a5eb.py
 accelbyte_py_sdk/api/cloudsave/operations/admin_player_record/admin_post_player_publi_98e39e.py
```

