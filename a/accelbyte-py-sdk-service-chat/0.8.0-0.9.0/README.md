# Comparing `tmp/accelbyte-py-sdk-service-chat-0.8.0.tar.gz` & `tmp/accelbyte-py-sdk-service-chat-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accelbyte-py-sdk-service-chat-0.8.0.tar", last modified: Wed Mar 13 06:10:20 2024, max compression
+gzip compressed data, was "accelbyte-py-sdk-service-chat-0.9.0.tar", last modified: Tue Mar 26 05:40:36 2024, max compression
```

## Comparing `accelbyte-py-sdk-service-chat-0.8.0.tar` & `accelbyte-py-sdk-service-chat-0.9.0.tar`

### file list

```diff
@@ -1,171 +1,171 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:10:20.257372 accelbyte-py-sdk-service-chat-0.8.0/
--rw-r--r--   0 root         (0) root         (0)     1113 2024-03-13 06:10:20.253372 accelbyte-py-sdk-service-chat-0.8.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      867 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:10:20.241372 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:10:20.241372 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:10:20.241372 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/
--rw-rw-r--   0 root         (0) root         (0)     6166 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:10:20.249372 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/
--rw-rw-r--   0 root         (0) root         (0)     6562 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3747 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/api_add_member_params.py
--rw-rw-r--   0 root         (0) root         (0)     4530 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/api_create_namespace_topic_params.py
--rw-rw-r--   0 root         (0) root         (0)     8559 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/api_create_topic_params.py
--rw-rw-r--   0 root         (0) root         (0)     9168 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/api_create_topic_response.py
--rw-rw-r--   0 root         (0) root         (0)     4356 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/api_mute_user_request.py
--rw-rw-r--   0 root         (0) root         (0)     5331 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/api_muted_topic_response.py
--rw-rw-r--   0 root         (0) root         (0)     3712 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/api_send_chat_params.py
--rw-rw-r--   0 root         (0) root         (0)     3754 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/api_unmute_user_request.py
--rw-rw-r--   0 root         (0) root         (0)     5130 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/api_update_topic_params.py
--rw-rw-r--   0 root         (0) root         (0)     7048 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/log_app_message_declaration.py
--rw-rw-r--   0 root         (0) root         (0)     5240 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/message_action_add_user_to_topic_result.py
--rw-rw-r--   0 root         (0) root         (0)     4572 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/message_action_delete_topic_result.py
--rw-rw-r--   0 root         (0) root         (0)     8553 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_add_inbox_category_request.py
--rw-rw-r--   0 root         (0) root         (0)     8519 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_add_inbox_category_response.py
--rw-rw-r--   0 root         (0) root         (0)     3884 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_ban_topic_member_param.py
--rw-rw-r--   0 root         (0) root         (0)     3895 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_ban_topic_member_result.py
--rw-rw-r--   0 root         (0) root         (0)     4657 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_category_hook.py
--rw-rw-r--   0 root         (0) root         (0)    10995 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_channel_topic_response.py
--rw-rw-r--   0 root         (0) root         (0)     4738 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_channel_topic_summary_response.py
--rw-rw-r--   0 root         (0) root         (0)     6020 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_channel_topic_with_pagination_response.py
--rw-rw-r--   0 root         (0) root         (0)     6972 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_chat_message_response.py
--rw-rw-r--   0 root         (0) root         (0)     6000 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_chat_message_with_pagination_response.py
--rw-rw-r--   0 root         (0) root         (0)     5795 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_chat_snapshot_message.py
--rw-rw-r--   0 root         (0) root         (0)     8979 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_chat_snapshots.py
--rw-rw-r--   0 root         (0) root         (0)    20800 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_config.py
--rw-rw-r--   0 root         (0) root         (0)    19519 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_config_export.py
--rw-rw-r--   0 root         (0) root         (0)     3988 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_config_list.py
--rw-rw-r--   0 root         (0) root         (0)    19272 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_config_response.py
--rw-rw-r--   0 root         (0) root         (0)     6187 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_dictionary.py
--rw-rw-r--   0 root         (0) root         (0)     4249 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_dictionary_child.py
--rw-rw-r--   0 root         (0) root         (0)     4351 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_dictionary_export.py
--rw-rw-r--   0 root         (0) root         (0)     5571 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_dictionary_export_item.py
--rw-rw-r--   0 root         (0) root         (0)     4296 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_dictionary_group.py
--rw-rw-r--   0 root         (0) root         (0)     4201 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_dictionary_import_result.py
--rw-rw-r--   0 root         (0) root         (0)     4495 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_dictionary_insert_bulk_request.py
--rw-rw-r--   0 root         (0) root         (0)     6162 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_dictionary_insert_request.py
--rw-rw-r--   0 root         (0) root         (0)     5529 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_dictionary_query_result.py
--rw-rw-r--   0 root         (0) root         (0)     6162 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_dictionary_update_request.py
--rw-rw-r--   0 root         (0) root         (0)     8802 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_dictionary_with_children.py
--rw-rw-r--   0 root         (0) root         (0)     6700 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_dictionary_word_changes.py
--rw-rw-r--   0 root         (0) root         (0)     8715 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_get_inbox_categories_response_item.py
--rw-rw-r--   0 root         (0) root         (0)     5622 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_get_inbox_messages_response.py
--rw-rw-r--   0 root         (0) root         (0)    10708 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_get_inbox_messages_response_data.py
--rw-rw-r--   0 root         (0) root         (0)     4139 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_get_inbox_stats_response.py
--rw-rw-r--   0 root         (0) root         (0)     5353 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_get_inbox_users_response.py
--rw-rw-r--   0 root         (0) root         (0)     6520 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_import_config_response.py
--rw-rw-r--   0 root         (0) root         (0)     3807 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_json_schema_type.py
--rw-rw-r--   0 root         (0) root         (0)     5967 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_message_stats.py
--rw-rw-r--   0 root         (0) root         (0)     4277 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_pagination.py
--rw-rw-r--   0 root         (0) root         (0)     4010 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_public_ban_topic_members_request.py
--rw-rw-r--   0 root         (0) root         (0)     4021 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_public_ban_topic_members_response.py
--rw-rw-r--   0 root         (0) root         (0)     4032 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_public_unban_topic_members_request.py
--rw-rw-r--   0 root         (0) root         (0)     4043 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_public_unban_topic_members_response.py
--rw-rw-r--   0 root         (0) root         (0)     7895 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_save_inbox_message_request.py
--rw-rw-r--   0 root         (0) root         (0)     8523 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_save_inbox_message_response.py
--rw-rw-r--   0 root         (0) root         (0)     3912 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_send_inbox_message_request.py
--rw-rw-r--   0 root         (0) root         (0)     3922 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_send_inbox_message_response.py
--rw-rw-r--   0 root         (0) root         (0)     7823 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_topic_info.py
--rw-rw-r--   0 root         (0) root         (0)     7972 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_topic_log_item.py
--rw-rw-r--   0 root         (0) root         (0)     5150 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_topic_log_with_pagination_response.py
--rw-rw-r--   0 root         (0) root         (0)     5793 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_topic_member_response.py
--rw-rw-r--   0 root         (0) root         (0)     6000 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_topic_member_with_pagination_response.py
--rw-rw-r--   0 root         (0) root         (0)     7743 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_topic_response.py
--rw-rw-r--   0 root         (0) root         (0)     3906 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_unban_topic_member_param.py
--rw-rw-r--   0 root         (0) root         (0)     3917 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_unban_topic_member_result.py
--rw-rw-r--   0 root         (0) root         (0)     3950 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_unsend_inbox_message_request.py
--rw-rw-r--   0 root         (0) root         (0)     3942 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_unsend_inbox_message_response.py
--rw-rw-r--   0 root         (0) root         (0)     7982 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_update_inbox_category_request.py
--rw-rw-r--   0 root         (0) root         (0)     6411 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_update_inbox_message_request.py
--rw-rw-r--   0 root         (0) root         (0)     4863 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_user_inbox.py
--rw-rw-r--   0 root         (0) root         (0)     4432 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/response_error.py
--rw-rw-r--   0 root         (0) root         (0)     4611 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/restapi_error_response_body.py
--rw-rw-r--   0 root         (0) root         (0)     4345 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/topic_info_member.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:10:20.249372 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/
--rw-rw-r--   0 root         (0) root         (0)      433 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:10:20.249372 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/config/
--rw-rw-r--   0 root         (0) root         (0)      709 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/config/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5718 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/config/admin_get_all_config_v1.py
--rw-rw-r--   0 root         (0) root         (0)     6704 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/config/admin_get_config_v1.py
--rw-rw-r--   0 root         (0) root         (0)     8035 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/config/admin_update_config_v1.py
--rw-rw-r--   0 root         (0) root         (0)     6190 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/config/export_config.py
--rw-rw-r--   0 root         (0) root         (0)     7168 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/config/import_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:10:20.249372 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/inbox/
--rw-rw-r--   0 root         (0) root         (0)     1493 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/inbox/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7715 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/inbox/admin_add_inbox_category.py
--rw-rw-r--   0 root         (0) root         (0)     7223 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/inbox/admin_delete_inbox_category.py
--rw-rw-r--   0 root         (0) root         (0)     8142 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/inbox/admin_delete_inbox_message.py
--rw-rw-r--   0 root         (0) root         (0)     7571 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/inbox/admin_get_category_schema.py
--rw-rw-r--   0 root         (0) root         (0)     6678 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/inbox/admin_get_inbox_categories.py
--rw-rw-r--   0 root         (0) root         (0)    16036 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/inbox/admin_get_inbox_messages.py
--rw-rw-r--   0 root         (0) root         (0)     7730 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/inbox/admin_get_inbox_stats.py
--rw-rw-r--   0 root         (0) root         (0)    10887 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/inbox/admin_get_inbox_users.py
--rw-rw-r--   0 root         (0) root         (0)     7716 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/inbox/admin_save_inbox_message.py
--rw-rw-r--   0 root         (0) root         (0)     8589 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/inbox/admin_send_inbox_message.py
--rw-rw-r--   0 root         (0) root         (0)     8499 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/inbox/admin_unsend_inbox_message.py
--rw-rw-r--   0 root         (0) root         (0)     8442 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/inbox/admin_update_inbox_category.py
--rw-rw-r--   0 root         (0) root         (0)     8462 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/inbox/admin_update_inbox_message.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:10:20.249372 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/moderation/
--rw-rw-r--   0 root         (0) root         (0)      648 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/moderation/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7353 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/moderation/admin_delete_chat_snapshot.py
--rw-rw-r--   0 root         (0) root         (0)     7465 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/moderation/admin_get_chat_snapshot.py
--rw-rw-r--   0 root         (0) root         (0)     8211 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/moderation/public_get_chat_snapshot.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:10:20.249372 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/operations/
--rw-rw-r--   0 root         (0) root         (0)      517 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/operations/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4821 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/operations/public_get_messages.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:10:20.249372 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/profanity/
--rw-rw-r--   0 root         (0) root         (0)     1017 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/profanity/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7908 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/profanity/admin_profanity_create.py
--rw-rw-r--   0 root         (0) root         (0)     7944 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/profanity/admin_profanity_create_bulk.py
--rw-rw-r--   0 root         (0) root         (0)     7255 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/profanity/admin_profanity_delete.py
--rw-rw-r--   0 root         (0) root         (0)     6546 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/profanity/admin_profanity_export.py
--rw-rw-r--   0 root         (0) root         (0)     8263 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/profanity/admin_profanity_group.py
--rw-rw-r--   0 root         (0) root         (0)    10000 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/profanity/admin_profanity_import.py
--rw-rw-r--   0 root         (0) root         (0)    12964 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/profanity/admin_profanity_query.py
--rw-rw-r--   0 root         (0) root         (0)     8533 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/profanity/admin_profanity_update.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:10:20.253372 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/topic/
--rw-rw-r--   0 root         (0) root         (0)     2333 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/topic/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8074 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/topic/admin_add_topic_member.py
--rw-rw-r--   0 root         (0) root         (0)     8465 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/topic/admin_ban_topic_members.py
--rw-rw-r--   0 root         (0) root         (0)     7492 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/topic/admin_channel_topic_info.py
--rw-rw-r--   0 root         (0) root         (0)     9247 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/topic/admin_channel_topic_list.py
--rw-rw-r--   0 root         (0) root         (0)     6618 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/topic/admin_channel_topic_summary.py
--rw-rw-r--   0 root         (0) root         (0)    15442 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/topic/admin_chat_history.py
--rw-rw-r--   0 root         (0) root         (0)     6738 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/topic/admin_create_namespace_topic.py
--rw-rw-r--   0 root         (0) root         (0)     6528 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/topic/admin_create_topic.py
--rw-rw-r--   0 root         (0) root         (0)     7773 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/topic/admin_delete_chat.py
--rw-rw-r--   0 root         (0) root         (0)     6184 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/topic/admin_delete_topic.py
--rw-rw-r--   0 root         (0) root         (0)    15856 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/topic/admin_query_topic.py
--rw-rw-r--   0 root         (0) root         (0)    13859 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/topic/admin_query_topic_log.py
--rw-rw-r--   0 root         (0) root         (0)    12888 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/topic/admin_query_users_topic.py
--rw-rw-r--   0 root         (0) root         (0)     7006 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/topic/admin_remove_topic_member.py
--rw-rw-r--   0 root         (0) root         (0)     8325 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/topic/admin_send_chat.py
--rw-rw-r--   0 root         (0) root         (0)    14431 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/topic/admin_topic_chat_history.py
--rw-rw-r--   0 root         (0) root         (0)     9036 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/topic/admin_topic_list.py
--rw-rw-r--   0 root         (0) root         (0)    11625 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/topic/admin_topic_members.py
--rw-rw-r--   0 root         (0) root         (0)     7081 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/topic/admin_topic_shards.py
--rw-rw-r--   0 root         (0) root         (0)     8428 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/topic/admin_unban_topic_members.py
--rw-rw-r--   0 root         (0) root         (0)     7240 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/topic/admin_update_topic.py
--rw-rw-r--   0 root         (0) root         (0)     8565 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/topic/public_ban_topic_members.py
--rw-rw-r--   0 root         (0) root         (0)     9959 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/topic/public_chat_history.py
--rw-rw-r--   0 root         (0) root         (0)     7782 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/topic/public_delete_chat.py
--rw-rw-r--   0 root         (0) root         (0)     6533 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/topic/public_get_muted_topics.py
--rw-rw-r--   0 root         (0) root         (0)     8074 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/topic/public_mute_user.py
--rw-rw-r--   0 root         (0) root         (0)     9107 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/topic/public_topic_list.py
--rw-rw-r--   0 root         (0) root         (0)     8613 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/topic/public_unban_topic_members.py
--rw-rw-r--   0 root         (0) root         (0)     8112 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/topic/public_unmute_user.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:10:20.253372 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/wrappers/
--rw-rw-r--   0 root         (0) root         (0)     5981 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/wrappers/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    14149 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/wrappers/_config.py
--rw-rw-r--   0 root         (0) root         (0)    42463 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/wrappers/_inbox.py
--rw-rw-r--   0 root         (0) root         (0)     9877 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/wrappers/_moderation.py
--rw-rw-r--   0 root         (0) root         (0)     2693 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/wrappers/_operations.py
--rw-rw-r--   0 root         (0) root         (0)    26831 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/wrappers/_profanity.py
--rw-rw-r--   0 root         (0) root         (0)    93767 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/wrappers/_topic.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:10:20.253372 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk_service_chat.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1113 2024-03-13 06:10:20.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk_service_chat.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10027 2024-03-13 06:10:20.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk_service_chat.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-13 06:10:20.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk_service_chat.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-13 06:10:20.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk_service_chat.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-03-13 06:10:20.000000 accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk_service_chat.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)      353 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-chat-0.8.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-13 06:10:20.257372 accelbyte-py-sdk-service-chat-0.8.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:40:36.321751 accelbyte-py-sdk-service-chat-0.9.0/
+-rw-r--r--   0 root         (0) root         (0)     1113 2024-03-26 05:40:36.321751 accelbyte-py-sdk-service-chat-0.9.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      867 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:40:36.305752 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:40:36.305752 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:40:36.305752 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/
+-rw-rw-r--   0 root         (0) root         (0)     6166 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:40:36.313752 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/
+-rw-rw-r--   0 root         (0) root         (0)     6562 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3747 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/api_add_member_params.py
+-rw-rw-r--   0 root         (0) root         (0)     4530 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/api_create_namespace_topic_params.py
+-rw-rw-r--   0 root         (0) root         (0)     8559 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/api_create_topic_params.py
+-rw-rw-r--   0 root         (0) root         (0)     9168 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/api_create_topic_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4356 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/api_mute_user_request.py
+-rw-rw-r--   0 root         (0) root         (0)     5331 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/api_muted_topic_response.py
+-rw-rw-r--   0 root         (0) root         (0)     3712 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/api_send_chat_params.py
+-rw-rw-r--   0 root         (0) root         (0)     3754 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/api_unmute_user_request.py
+-rw-rw-r--   0 root         (0) root         (0)     5130 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/api_update_topic_params.py
+-rw-rw-r--   0 root         (0) root         (0)     7048 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/log_app_message_declaration.py
+-rw-rw-r--   0 root         (0) root         (0)     5240 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/message_action_add_user_to_topic_result.py
+-rw-rw-r--   0 root         (0) root         (0)     4572 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/message_action_delete_topic_result.py
+-rw-rw-r--   0 root         (0) root         (0)     8553 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_add_inbox_category_request.py
+-rw-rw-r--   0 root         (0) root         (0)     8570 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_add_inbox_category_response.py
+-rw-rw-r--   0 root         (0) root         (0)     3884 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_ban_topic_member_param.py
+-rw-rw-r--   0 root         (0) root         (0)     3895 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_ban_topic_member_result.py
+-rw-rw-r--   0 root         (0) root         (0)     4894 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_category_hook.py
+-rw-rw-r--   0 root         (0) root         (0)    10995 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_channel_topic_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4738 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_channel_topic_summary_response.py
+-rw-rw-r--   0 root         (0) root         (0)     6020 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_channel_topic_with_pagination_response.py
+-rw-rw-r--   0 root         (0) root         (0)     7084 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_chat_message_response.py
+-rw-rw-r--   0 root         (0) root         (0)     6000 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_chat_message_with_pagination_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5795 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_chat_snapshot_message.py
+-rw-rw-r--   0 root         (0) root         (0)     8979 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_chat_snapshots.py
+-rw-rw-r--   0 root         (0) root         (0)    20800 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_config.py
+-rw-rw-r--   0 root         (0) root         (0)    19519 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_config_export.py
+-rw-rw-r--   0 root         (0) root         (0)     3988 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_config_list.py
+-rw-rw-r--   0 root         (0) root         (0)    19272 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_config_response.py
+-rw-rw-r--   0 root         (0) root         (0)     6243 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_dictionary.py
+-rw-rw-r--   0 root         (0) root         (0)     4249 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_dictionary_child.py
+-rw-rw-r--   0 root         (0) root         (0)     4351 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_dictionary_export.py
+-rw-rw-r--   0 root         (0) root         (0)     5571 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_dictionary_export_item.py
+-rw-rw-r--   0 root         (0) root         (0)     4296 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_dictionary_group.py
+-rw-rw-r--   0 root         (0) root         (0)     4201 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_dictionary_import_result.py
+-rw-rw-r--   0 root         (0) root         (0)     4495 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_dictionary_insert_bulk_request.py
+-rw-rw-r--   0 root         (0) root         (0)     6162 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_dictionary_insert_request.py
+-rw-rw-r--   0 root         (0) root         (0)     5529 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_dictionary_query_result.py
+-rw-rw-r--   0 root         (0) root         (0)     6162 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_dictionary_update_request.py
+-rw-rw-r--   0 root         (0) root         (0)     8858 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_dictionary_with_children.py
+-rw-rw-r--   0 root         (0) root         (0)     6700 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_dictionary_word_changes.py
+-rw-rw-r--   0 root         (0) root         (0)     8715 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_get_inbox_categories_response_item.py
+-rw-rw-r--   0 root         (0) root         (0)     5622 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_get_inbox_messages_response.py
+-rw-rw-r--   0 root         (0) root         (0)    10817 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_get_inbox_messages_response_data.py
+-rw-rw-r--   0 root         (0) root         (0)     4139 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_get_inbox_stats_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5353 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_get_inbox_users_response.py
+-rw-rw-r--   0 root         (0) root         (0)     6520 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_import_config_response.py
+-rw-rw-r--   0 root         (0) root         (0)     3807 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_json_schema_type.py
+-rw-rw-r--   0 root         (0) root         (0)     5967 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_message_stats.py
+-rw-rw-r--   0 root         (0) root         (0)     4277 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_pagination.py
+-rw-rw-r--   0 root         (0) root         (0)     4010 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_public_ban_topic_members_request.py
+-rw-rw-r--   0 root         (0) root         (0)     4021 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_public_ban_topic_members_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4032 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_public_unban_topic_members_request.py
+-rw-rw-r--   0 root         (0) root         (0)     4043 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_public_unban_topic_members_response.py
+-rw-rw-r--   0 root         (0) root         (0)     7895 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_save_inbox_message_request.py
+-rw-rw-r--   0 root         (0) root         (0)     8633 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_save_inbox_message_response.py
+-rw-rw-r--   0 root         (0) root         (0)     3912 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_send_inbox_message_request.py
+-rw-rw-r--   0 root         (0) root         (0)     3922 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_send_inbox_message_response.py
+-rw-rw-r--   0 root         (0) root         (0)     7823 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_topic_info.py
+-rw-rw-r--   0 root         (0) root         (0)     7972 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_topic_log_item.py
+-rw-rw-r--   0 root         (0) root         (0)     5150 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_topic_log_with_pagination_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5793 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_topic_member_response.py
+-rw-rw-r--   0 root         (0) root         (0)     6000 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_topic_member_with_pagination_response.py
+-rw-rw-r--   0 root         (0) root         (0)     7743 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_topic_response.py
+-rw-rw-r--   0 root         (0) root         (0)     3906 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_unban_topic_member_param.py
+-rw-rw-r--   0 root         (0) root         (0)     3917 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_unban_topic_member_result.py
+-rw-rw-r--   0 root         (0) root         (0)     3950 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_unsend_inbox_message_request.py
+-rw-rw-r--   0 root         (0) root         (0)     3942 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_unsend_inbox_message_response.py
+-rw-rw-r--   0 root         (0) root         (0)     7982 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_update_inbox_category_request.py
+-rw-rw-r--   0 root         (0) root         (0)     6411 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_update_inbox_message_request.py
+-rw-rw-r--   0 root         (0) root         (0)     4863 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_user_inbox.py
+-rw-rw-r--   0 root         (0) root         (0)     4432 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/response_error.py
+-rw-rw-r--   0 root         (0) root         (0)     4611 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/restapi_error_response_body.py
+-rw-rw-r--   0 root         (0) root         (0)     4345 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/topic_info_member.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:40:36.313752 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/
+-rw-rw-r--   0 root         (0) root         (0)      433 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:40:36.313752 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/config/
+-rw-rw-r--   0 root         (0) root         (0)      709 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/config/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     5718 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/config/admin_get_all_config_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     6704 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/config/admin_get_config_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     8035 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/config/admin_update_config_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     6190 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/config/export_config.py
+-rw-rw-r--   0 root         (0) root         (0)     7168 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/config/import_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:40:36.317752 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/inbox/
+-rw-rw-r--   0 root         (0) root         (0)     1493 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/inbox/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7715 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/inbox/admin_add_inbox_category.py
+-rw-rw-r--   0 root         (0) root         (0)     7223 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/inbox/admin_delete_inbox_category.py
+-rw-rw-r--   0 root         (0) root         (0)     8142 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/inbox/admin_delete_inbox_message.py
+-rw-rw-r--   0 root         (0) root         (0)     7571 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/inbox/admin_get_category_schema.py
+-rw-rw-r--   0 root         (0) root         (0)     6678 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/inbox/admin_get_inbox_categories.py
+-rw-rw-r--   0 root         (0) root         (0)    16036 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/inbox/admin_get_inbox_messages.py
+-rw-rw-r--   0 root         (0) root         (0)     7730 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/inbox/admin_get_inbox_stats.py
+-rw-rw-r--   0 root         (0) root         (0)    10887 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/inbox/admin_get_inbox_users.py
+-rw-rw-r--   0 root         (0) root         (0)     7716 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/inbox/admin_save_inbox_message.py
+-rw-rw-r--   0 root         (0) root         (0)     8589 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/inbox/admin_send_inbox_message.py
+-rw-rw-r--   0 root         (0) root         (0)     8499 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/inbox/admin_unsend_inbox_message.py
+-rw-rw-r--   0 root         (0) root         (0)     8442 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/inbox/admin_update_inbox_category.py
+-rw-rw-r--   0 root         (0) root         (0)     8462 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/inbox/admin_update_inbox_message.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:40:36.317752 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/moderation/
+-rw-rw-r--   0 root         (0) root         (0)      648 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/moderation/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7353 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/moderation/admin_delete_chat_snapshot.py
+-rw-rw-r--   0 root         (0) root         (0)     7465 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/moderation/admin_get_chat_snapshot.py
+-rw-rw-r--   0 root         (0) root         (0)     8211 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/moderation/public_get_chat_snapshot.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:40:36.317752 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/operations/
+-rw-rw-r--   0 root         (0) root         (0)      517 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/operations/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4821 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/operations/public_get_messages.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:40:36.317752 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/profanity/
+-rw-rw-r--   0 root         (0) root         (0)     1017 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/profanity/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7908 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/profanity/admin_profanity_create.py
+-rw-rw-r--   0 root         (0) root         (0)     7944 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/profanity/admin_profanity_create_bulk.py
+-rw-rw-r--   0 root         (0) root         (0)     7255 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/profanity/admin_profanity_delete.py
+-rw-rw-r--   0 root         (0) root         (0)     6546 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/profanity/admin_profanity_export.py
+-rw-rw-r--   0 root         (0) root         (0)     8263 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/profanity/admin_profanity_group.py
+-rw-rw-r--   0 root         (0) root         (0)    10000 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/profanity/admin_profanity_import.py
+-rw-rw-r--   0 root         (0) root         (0)    12964 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/profanity/admin_profanity_query.py
+-rw-rw-r--   0 root         (0) root         (0)     8533 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/profanity/admin_profanity_update.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:40:36.321751 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/topic/
+-rw-rw-r--   0 root         (0) root         (0)     2333 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/topic/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8074 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/topic/admin_add_topic_member.py
+-rw-rw-r--   0 root         (0) root         (0)     8465 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/topic/admin_ban_topic_members.py
+-rw-rw-r--   0 root         (0) root         (0)     7492 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/topic/admin_channel_topic_info.py
+-rw-rw-r--   0 root         (0) root         (0)     9247 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/topic/admin_channel_topic_list.py
+-rw-rw-r--   0 root         (0) root         (0)     6618 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/topic/admin_channel_topic_summary.py
+-rw-rw-r--   0 root         (0) root         (0)    15442 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/topic/admin_chat_history.py
+-rw-rw-r--   0 root         (0) root         (0)     6738 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/topic/admin_create_namespace_topic.py
+-rw-rw-r--   0 root         (0) root         (0)     6528 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/topic/admin_create_topic.py
+-rw-rw-r--   0 root         (0) root         (0)     7773 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/topic/admin_delete_chat.py
+-rw-rw-r--   0 root         (0) root         (0)     6184 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/topic/admin_delete_topic.py
+-rw-rw-r--   0 root         (0) root         (0)    15856 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/topic/admin_query_topic.py
+-rw-rw-r--   0 root         (0) root         (0)    13859 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/topic/admin_query_topic_log.py
+-rw-rw-r--   0 root         (0) root         (0)    12888 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/topic/admin_query_users_topic.py
+-rw-rw-r--   0 root         (0) root         (0)     7006 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/topic/admin_remove_topic_member.py
+-rw-rw-r--   0 root         (0) root         (0)     8325 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/topic/admin_send_chat.py
+-rw-rw-r--   0 root         (0) root         (0)    14431 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/topic/admin_topic_chat_history.py
+-rw-rw-r--   0 root         (0) root         (0)     9036 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/topic/admin_topic_list.py
+-rw-rw-r--   0 root         (0) root         (0)    11625 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/topic/admin_topic_members.py
+-rw-rw-r--   0 root         (0) root         (0)     7081 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/topic/admin_topic_shards.py
+-rw-rw-r--   0 root         (0) root         (0)     8428 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/topic/admin_unban_topic_members.py
+-rw-rw-r--   0 root         (0) root         (0)     7240 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/topic/admin_update_topic.py
+-rw-rw-r--   0 root         (0) root         (0)     8565 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/topic/public_ban_topic_members.py
+-rw-rw-r--   0 root         (0) root         (0)     9959 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/topic/public_chat_history.py
+-rw-rw-r--   0 root         (0) root         (0)     7782 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/topic/public_delete_chat.py
+-rw-rw-r--   0 root         (0) root         (0)     6533 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/topic/public_get_muted_topics.py
+-rw-rw-r--   0 root         (0) root         (0)     8074 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/topic/public_mute_user.py
+-rw-rw-r--   0 root         (0) root         (0)     9107 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/topic/public_topic_list.py
+-rw-rw-r--   0 root         (0) root         (0)     8613 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/topic/public_unban_topic_members.py
+-rw-rw-r--   0 root         (0) root         (0)     8112 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/topic/public_unmute_user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:40:36.321751 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/wrappers/
+-rw-rw-r--   0 root         (0) root         (0)     5981 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/wrappers/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    14149 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/wrappers/_config.py
+-rw-rw-r--   0 root         (0) root         (0)    42463 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/wrappers/_inbox.py
+-rw-rw-r--   0 root         (0) root         (0)     9877 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/wrappers/_moderation.py
+-rw-rw-r--   0 root         (0) root         (0)     2693 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/wrappers/_operations.py
+-rw-rw-r--   0 root         (0) root         (0)    26831 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/wrappers/_profanity.py
+-rw-rw-r--   0 root         (0) root         (0)    93767 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/wrappers/_topic.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:40:36.321751 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk_service_chat.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1113 2024-03-26 05:40:36.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk_service_chat.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10027 2024-03-26 05:40:36.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk_service_chat.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-03-26 05:40:36.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk_service_chat.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 05:40:36.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk_service_chat.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-03-26 05:40:36.000000 accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk_service_chat.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)      353 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-chat-0.9.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-03-26 05:40:36.321751 accelbyte-py-sdk-service-chat-0.9.0/setup.cfg
```

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/PKG-INFO` & `accelbyte-py-sdk-service-chat-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: accelbyte-py-sdk-service-chat
-Version: 0.8.0
+Version: 0.9.0
 Summary: AccelByte Python SDK - AccelByte Gaming Services Chat Service
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: accelbyte-py-sdk-core
 
 [//]: # (Code generated. DO NOT EDIT!)
```

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/README.md` & `accelbyte-py-sdk-service-chat-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/__init__.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/__init__.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/__init__.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/__init__.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/api_add_member_params.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/api_add_member_params.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/api_create_namespace_topic_params.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/api_create_namespace_topic_params.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/api_create_topic_params.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/api_create_topic_params.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/api_create_topic_response.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/api_create_topic_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/api_mute_user_request.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/api_mute_user_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/api_muted_topic_response.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/api_muted_topic_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/api_send_chat_params.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/api_send_chat_params.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/api_unmute_user_request.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/api_unmute_user_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/api_update_topic_params.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/api_update_topic_params.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/log_app_message_declaration.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/log_app_message_declaration.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/message_action_add_user_to_topic_result.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/message_action_add_user_to_topic_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/message_action_delete_topic_result.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/message_action_delete_topic_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_add_inbox_category_request.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_add_inbox_category_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_add_inbox_category_response.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_add_inbox_category_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,63 +34,63 @@
     """Models add inbox category response (models.AddInboxCategoryResponse)
 
     Properties:
         enabled: (enabled) REQUIRED bool
 
         expires_in: (expiresIn) REQUIRED int
 
-        hook: (hook) REQUIRED ModelsCategoryHook
-
         name: (name) REQUIRED str
 
         save_inbox: (saveInbox) REQUIRED bool
 
         send_notification: (sendNotification) REQUIRED bool
 
+        hook: (hook) OPTIONAL ModelsCategoryHook
+
         json_schema: (jsonSchema) OPTIONAL Dict[str, Any]
     """
 
     # region fields
 
     enabled: bool  # REQUIRED
     expires_in: int  # REQUIRED
-    hook: ModelsCategoryHook  # REQUIRED
     name: str  # REQUIRED
     save_inbox: bool  # REQUIRED
     send_notification: bool  # REQUIRED
+    hook: ModelsCategoryHook  # OPTIONAL
     json_schema: Dict[str, Any]  # OPTIONAL
 
     # endregion fields
 
     # region with_x methods
 
     def with_enabled(self, value: bool) -> ModelsAddInboxCategoryResponse:
         self.enabled = value
         return self
 
     def with_expires_in(self, value: int) -> ModelsAddInboxCategoryResponse:
         self.expires_in = value
         return self
 
-    def with_hook(self, value: ModelsCategoryHook) -> ModelsAddInboxCategoryResponse:
-        self.hook = value
-        return self
-
     def with_name(self, value: str) -> ModelsAddInboxCategoryResponse:
         self.name = value
         return self
 
     def with_save_inbox(self, value: bool) -> ModelsAddInboxCategoryResponse:
         self.save_inbox = value
         return self
 
     def with_send_notification(self, value: bool) -> ModelsAddInboxCategoryResponse:
         self.send_notification = value
         return self
 
+    def with_hook(self, value: ModelsCategoryHook) -> ModelsAddInboxCategoryResponse:
+        self.hook = value
+        return self
+
     def with_json_schema(self, value: Dict[str, Any]) -> ModelsAddInboxCategoryResponse:
         self.json_schema = value
         return self
 
     # endregion with_x methods
 
     # region to methods
@@ -101,30 +101,30 @@
             result["enabled"] = bool(self.enabled)
         elif include_empty:
             result["enabled"] = False
         if hasattr(self, "expires_in"):
             result["expiresIn"] = int(self.expires_in)
         elif include_empty:
             result["expiresIn"] = 0
-        if hasattr(self, "hook"):
-            result["hook"] = self.hook.to_dict(include_empty=include_empty)
-        elif include_empty:
-            result["hook"] = ModelsCategoryHook()
         if hasattr(self, "name"):
             result["name"] = str(self.name)
         elif include_empty:
             result["name"] = ""
         if hasattr(self, "save_inbox"):
             result["saveInbox"] = bool(self.save_inbox)
         elif include_empty:
             result["saveInbox"] = False
         if hasattr(self, "send_notification"):
             result["sendNotification"] = bool(self.send_notification)
         elif include_empty:
             result["sendNotification"] = False
+        if hasattr(self, "hook"):
+            result["hook"] = self.hook.to_dict(include_empty=include_empty)
+        elif include_empty:
+            result["hook"] = ModelsCategoryHook()
         if hasattr(self, "json_schema"):
             result["jsonSchema"] = {str(k0): v0 for k0, v0 in self.json_schema.items()}
         elif include_empty:
             result["jsonSchema"] = {}
         return result
 
     # endregion to methods
@@ -132,28 +132,29 @@
     # region static methods
 
     @classmethod
     def create(
         cls,
         enabled: bool,
         expires_in: int,
-        hook: ModelsCategoryHook,
         name: str,
         save_inbox: bool,
         send_notification: bool,
+        hook: Optional[ModelsCategoryHook] = None,
         json_schema: Optional[Dict[str, Any]] = None,
         **kwargs,
     ) -> ModelsAddInboxCategoryResponse:
         instance = cls()
         instance.enabled = enabled
         instance.expires_in = expires_in
-        instance.hook = hook
         instance.name = name
         instance.save_inbox = save_inbox
         instance.send_notification = send_notification
+        if hook is not None:
+            instance.hook = hook
         if json_schema is not None:
             instance.json_schema = json_schema
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
@@ -165,32 +166,32 @@
             instance.enabled = bool(dict_["enabled"])
         elif include_empty:
             instance.enabled = False
         if "expiresIn" in dict_ and dict_["expiresIn"] is not None:
             instance.expires_in = int(dict_["expiresIn"])
         elif include_empty:
             instance.expires_in = 0
-        if "hook" in dict_ and dict_["hook"] is not None:
-            instance.hook = ModelsCategoryHook.create_from_dict(
-                dict_["hook"], include_empty=include_empty
-            )
-        elif include_empty:
-            instance.hook = ModelsCategoryHook()
         if "name" in dict_ and dict_["name"] is not None:
             instance.name = str(dict_["name"])
         elif include_empty:
             instance.name = ""
         if "saveInbox" in dict_ and dict_["saveInbox"] is not None:
             instance.save_inbox = bool(dict_["saveInbox"])
         elif include_empty:
             instance.save_inbox = False
         if "sendNotification" in dict_ and dict_["sendNotification"] is not None:
             instance.send_notification = bool(dict_["sendNotification"])
         elif include_empty:
             instance.send_notification = False
+        if "hook" in dict_ and dict_["hook"] is not None:
+            instance.hook = ModelsCategoryHook.create_from_dict(
+                dict_["hook"], include_empty=include_empty
+            )
+        elif include_empty:
+            instance.hook = ModelsCategoryHook()
         if "jsonSchema" in dict_ and dict_["jsonSchema"] is not None:
             instance.json_schema = {
                 str(k0): v0 for k0, v0 in dict_["jsonSchema"].items()
             }
         elif include_empty:
             instance.json_schema = {}
         return instance
@@ -234,27 +235,27 @@
             return cls.create_from_dict(any_, include_empty=include_empty)
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
             "enabled": "enabled",
             "expiresIn": "expires_in",
-            "hook": "hook",
             "name": "name",
             "saveInbox": "save_inbox",
             "sendNotification": "send_notification",
+            "hook": "hook",
             "jsonSchema": "json_schema",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
             "enabled": True,
             "expiresIn": True,
-            "hook": True,
             "name": True,
             "saveInbox": True,
             "sendNotification": True,
+            "hook": False,
             "jsonSchema": False,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_ban_topic_member_param.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_ban_topic_member_param.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_ban_topic_member_result.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_ban_topic_member_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_category_hook.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_category_hook.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,80 +33,85 @@
     KAFKA = "KAFKA"
 
 
 class ModelsCategoryHook(Model):
     """Models category hook (models.CategoryHook)
 
     Properties:
-        driver: (driver) REQUIRED Union[str, DriverEnum]
+        driver: (driver) OPTIONAL Union[str, DriverEnum]
 
-        params: (params) REQUIRED str
+        params: (params) OPTIONAL Dict[str, Any]
     """
 
     # region fields
 
-    driver: Union[str, DriverEnum]  # REQUIRED
-    params: str  # REQUIRED
+    driver: Union[str, DriverEnum]  # OPTIONAL
+    params: Dict[str, Any]  # OPTIONAL
 
     # endregion fields
 
     # region with_x methods
 
     def with_driver(self, value: Union[str, DriverEnum]) -> ModelsCategoryHook:
         self.driver = value
         return self
 
-    def with_params(self, value: str) -> ModelsCategoryHook:
+    def with_params(self, value: Dict[str, Any]) -> ModelsCategoryHook:
         self.params = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
         if hasattr(self, "driver"):
             result["driver"] = str(self.driver)
         elif include_empty:
             result["driver"] = Union[str, DriverEnum]()
         if hasattr(self, "params"):
-            result["params"] = str(self.params)
+            result["params"] = {str(k0): v0 for k0, v0 in self.params.items()}
         elif include_empty:
-            result["params"] = ""
+            result["params"] = {}
         return result
 
     # endregion to methods
 
     # region static methods
 
     @classmethod
     def create(
-        cls, driver: Union[str, DriverEnum], params: str, **kwargs
+        cls,
+        driver: Optional[Union[str, DriverEnum]] = None,
+        params: Optional[Dict[str, Any]] = None,
+        **kwargs,
     ) -> ModelsCategoryHook:
         instance = cls()
-        instance.driver = driver
-        instance.params = params
+        if driver is not None:
+            instance.driver = driver
+        if params is not None:
+            instance.params = params
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
     ) -> ModelsCategoryHook:
         instance = cls()
         if not dict_:
             return instance
         if "driver" in dict_ and dict_["driver"] is not None:
             instance.driver = str(dict_["driver"])
         elif include_empty:
             instance.driver = Union[str, DriverEnum]()
         if "params" in dict_ and dict_["params"] is not None:
-            instance.params = str(dict_["params"])
+            instance.params = {str(k0): v0 for k0, v0 in dict_["params"].items()}
         elif include_empty:
-            instance.params = ""
+            instance.params = {}
         return instance
 
     @classmethod
     def create_many_from_dict(
         cls, dict_: dict, include_empty: bool = False
     ) -> Dict[str, ModelsCategoryHook]:
         return (
@@ -147,16 +152,16 @@
             "driver": "driver",
             "params": "params",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
-            "driver": True,
-            "params": True,
+            "driver": False,
+            "params": False,
         }
 
     @staticmethod
     def get_enum_map() -> Dict[str, List[Any]]:
         return {
             "driver": ["KAFKA"],
         }
```

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_channel_topic_response.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_channel_topic_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_channel_topic_summary_response.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_channel_topic_summary_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_channel_topic_with_pagination_response.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_channel_topic_with_pagination_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_chat_message_response.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_chat_message_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,29 +34,29 @@
     Properties:
         from_: (from) REQUIRED str
 
         id_: (id) REQUIRED str
 
         message: (message) REQUIRED str
 
-        read_at: (readAt) REQUIRED int
+        topic_id: (topicId) REQUIRED str
 
-        received_at: (receivedAt) REQUIRED int
+        read_at: (readAt) OPTIONAL int
 
-        topic_id: (topicId) REQUIRED str
+        received_at: (receivedAt) OPTIONAL int
     """
 
     # region fields
 
     from_: str  # REQUIRED
     id_: str  # REQUIRED
     message: str  # REQUIRED
-    read_at: int  # REQUIRED
-    received_at: int  # REQUIRED
     topic_id: str  # REQUIRED
+    read_at: int  # OPTIONAL
+    received_at: int  # OPTIONAL
 
     # endregion fields
 
     # region with_x methods
 
     def with_from(self, value: str) -> ModelsChatMessageResponse:
         self.from_ = value
@@ -66,26 +66,26 @@
         self.id_ = value
         return self
 
     def with_message(self, value: str) -> ModelsChatMessageResponse:
         self.message = value
         return self
 
+    def with_topic_id(self, value: str) -> ModelsChatMessageResponse:
+        self.topic_id = value
+        return self
+
     def with_read_at(self, value: int) -> ModelsChatMessageResponse:
         self.read_at = value
         return self
 
     def with_received_at(self, value: int) -> ModelsChatMessageResponse:
         self.received_at = value
         return self
 
-    def with_topic_id(self, value: str) -> ModelsChatMessageResponse:
-        self.topic_id = value
-        return self
-
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
         if hasattr(self, "from_"):
@@ -96,50 +96,52 @@
             result["id"] = str(self.id_)
         elif include_empty:
             result["id"] = ""
         if hasattr(self, "message"):
             result["message"] = str(self.message)
         elif include_empty:
             result["message"] = ""
+        if hasattr(self, "topic_id"):
+            result["topicId"] = str(self.topic_id)
+        elif include_empty:
+            result["topicId"] = ""
         if hasattr(self, "read_at"):
             result["readAt"] = int(self.read_at)
         elif include_empty:
             result["readAt"] = 0
         if hasattr(self, "received_at"):
             result["receivedAt"] = int(self.received_at)
         elif include_empty:
             result["receivedAt"] = 0
-        if hasattr(self, "topic_id"):
-            result["topicId"] = str(self.topic_id)
-        elif include_empty:
-            result["topicId"] = ""
         return result
 
     # endregion to methods
 
     # region static methods
 
     @classmethod
     def create(
         cls,
         from_: str,
         id_: str,
         message: str,
-        read_at: int,
-        received_at: int,
         topic_id: str,
+        read_at: Optional[int] = None,
+        received_at: Optional[int] = None,
         **kwargs,
     ) -> ModelsChatMessageResponse:
         instance = cls()
         instance.from_ = from_
         instance.id_ = id_
         instance.message = message
-        instance.read_at = read_at
-        instance.received_at = received_at
         instance.topic_id = topic_id
+        if read_at is not None:
+            instance.read_at = read_at
+        if received_at is not None:
+            instance.received_at = received_at
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
     ) -> ModelsChatMessageResponse:
         instance = cls()
@@ -153,26 +155,26 @@
             instance.id_ = str(dict_["id"])
         elif include_empty:
             instance.id_ = ""
         if "message" in dict_ and dict_["message"] is not None:
             instance.message = str(dict_["message"])
         elif include_empty:
             instance.message = ""
+        if "topicId" in dict_ and dict_["topicId"] is not None:
+            instance.topic_id = str(dict_["topicId"])
+        elif include_empty:
+            instance.topic_id = ""
         if "readAt" in dict_ and dict_["readAt"] is not None:
             instance.read_at = int(dict_["readAt"])
         elif include_empty:
             instance.read_at = 0
         if "receivedAt" in dict_ and dict_["receivedAt"] is not None:
             instance.received_at = int(dict_["receivedAt"])
         elif include_empty:
             instance.received_at = 0
-        if "topicId" in dict_ and dict_["topicId"] is not None:
-            instance.topic_id = str(dict_["topicId"])
-        elif include_empty:
-            instance.topic_id = ""
         return instance
 
     @classmethod
     def create_many_from_dict(
         cls, dict_: dict, include_empty: bool = False
     ) -> Dict[str, ModelsChatMessageResponse]:
         return (
@@ -211,24 +213,24 @@
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
             "from": "from_",
             "id": "id_",
             "message": "message",
+            "topicId": "topic_id",
             "readAt": "read_at",
             "receivedAt": "received_at",
-            "topicId": "topic_id",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
             "from": True,
             "id": True,
             "message": True,
-            "readAt": True,
-            "receivedAt": True,
             "topicId": True,
+            "readAt": False,
+            "receivedAt": False,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_chat_message_with_pagination_response.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_chat_message_with_pagination_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_chat_snapshot_message.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_chat_snapshot_message.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_chat_snapshots.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_chat_snapshots.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_config.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_config_export.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_config_export.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_config_list.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_config_list.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_config_response.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_config_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_dictionary.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_dictionary.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,101 +32,102 @@
     """Models dictionary (models.Dictionary)
 
     Properties:
         id_: (id) REQUIRED str
 
         namespace: (namespace) REQUIRED str
 
-        parent_id: (parentId) REQUIRED str
-
         word: (word) REQUIRED str
 
         word_type: (wordType) REQUIRED str
+
+        parent_id: (parentId) OPTIONAL str
     """
 
     # region fields
 
     id_: str  # REQUIRED
     namespace: str  # REQUIRED
-    parent_id: str  # REQUIRED
     word: str  # REQUIRED
     word_type: str  # REQUIRED
+    parent_id: str  # OPTIONAL
 
     # endregion fields
 
     # region with_x methods
 
     def with_id(self, value: str) -> ModelsDictionary:
         self.id_ = value
         return self
 
     def with_namespace(self, value: str) -> ModelsDictionary:
         self.namespace = value
         return self
 
-    def with_parent_id(self, value: str) -> ModelsDictionary:
-        self.parent_id = value
-        return self
-
     def with_word(self, value: str) -> ModelsDictionary:
         self.word = value
         return self
 
     def with_word_type(self, value: str) -> ModelsDictionary:
         self.word_type = value
         return self
 
+    def with_parent_id(self, value: str) -> ModelsDictionary:
+        self.parent_id = value
+        return self
+
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
         if hasattr(self, "id_"):
             result["id"] = str(self.id_)
         elif include_empty:
             result["id"] = ""
         if hasattr(self, "namespace"):
             result["namespace"] = str(self.namespace)
         elif include_empty:
             result["namespace"] = ""
-        if hasattr(self, "parent_id"):
-            result["parentId"] = str(self.parent_id)
-        elif include_empty:
-            result["parentId"] = ""
         if hasattr(self, "word"):
             result["word"] = str(self.word)
         elif include_empty:
             result["word"] = ""
         if hasattr(self, "word_type"):
             result["wordType"] = str(self.word_type)
         elif include_empty:
             result["wordType"] = ""
+        if hasattr(self, "parent_id"):
+            result["parentId"] = str(self.parent_id)
+        elif include_empty:
+            result["parentId"] = ""
         return result
 
     # endregion to methods
 
     # region static methods
 
     @classmethod
     def create(
         cls,
         id_: str,
         namespace: str,
-        parent_id: str,
         word: str,
         word_type: str,
+        parent_id: Optional[str] = None,
         **kwargs,
     ) -> ModelsDictionary:
         instance = cls()
         instance.id_ = id_
         instance.namespace = namespace
-        instance.parent_id = parent_id
         instance.word = word
         instance.word_type = word_type
+        if parent_id is not None:
+            instance.parent_id = parent_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
     ) -> ModelsDictionary:
         instance = cls()
@@ -136,26 +137,26 @@
             instance.id_ = str(dict_["id"])
         elif include_empty:
             instance.id_ = ""
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
         elif include_empty:
             instance.namespace = ""
-        if "parentId" in dict_ and dict_["parentId"] is not None:
-            instance.parent_id = str(dict_["parentId"])
-        elif include_empty:
-            instance.parent_id = ""
         if "word" in dict_ and dict_["word"] is not None:
             instance.word = str(dict_["word"])
         elif include_empty:
             instance.word = ""
         if "wordType" in dict_ and dict_["wordType"] is not None:
             instance.word_type = str(dict_["wordType"])
         elif include_empty:
             instance.word_type = ""
+        if "parentId" in dict_ and dict_["parentId"] is not None:
+            instance.parent_id = str(dict_["parentId"])
+        elif include_empty:
+            instance.parent_id = ""
         return instance
 
     @classmethod
     def create_many_from_dict(
         cls, dict_: dict, include_empty: bool = False
     ) -> Dict[str, ModelsDictionary]:
         return (
@@ -189,23 +190,23 @@
             return cls.create_from_dict(any_, include_empty=include_empty)
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
             "id": "id_",
             "namespace": "namespace",
-            "parentId": "parent_id",
             "word": "word",
             "wordType": "word_type",
+            "parentId": "parent_id",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
             "id": True,
             "namespace": True,
-            "parentId": True,
             "word": True,
             "wordType": True,
+            "parentId": False,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_dictionary_child.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_dictionary_child.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_dictionary_export.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_dictionary_export.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_dictionary_export_item.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_dictionary_export_item.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_dictionary_group.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_dictionary_group.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_dictionary_import_result.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_dictionary_import_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_dictionary_insert_bulk_request.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_dictionary_insert_bulk_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_dictionary_insert_request.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_dictionary_insert_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_dictionary_query_result.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_dictionary_query_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_dictionary_update_request.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_dictionary_update_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_dictionary_with_children.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_dictionary_with_children.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,51 +34,47 @@
     """Models dictionary with children (models.DictionaryWithChildren)
 
     Properties:
         id_: (id) REQUIRED str
 
         namespace: (namespace) REQUIRED str
 
-        parent_id: (parentId) REQUIRED str
-
         word: (word) REQUIRED str
 
         word_type: (wordType) REQUIRED str
 
         false_negatives: (falseNegatives) OPTIONAL List[ModelsDictionaryChild]
 
         false_positives: (falsePositives) OPTIONAL List[ModelsDictionaryChild]
+
+        parent_id: (parentId) OPTIONAL str
     """
 
     # region fields
 
     id_: str  # REQUIRED
     namespace: str  # REQUIRED
-    parent_id: str  # REQUIRED
     word: str  # REQUIRED
     word_type: str  # REQUIRED
     false_negatives: List[ModelsDictionaryChild]  # OPTIONAL
     false_positives: List[ModelsDictionaryChild]  # OPTIONAL
+    parent_id: str  # OPTIONAL
 
     # endregion fields
 
     # region with_x methods
 
     def with_id(self, value: str) -> ModelsDictionaryWithChildren:
         self.id_ = value
         return self
 
     def with_namespace(self, value: str) -> ModelsDictionaryWithChildren:
         self.namespace = value
         return self
 
-    def with_parent_id(self, value: str) -> ModelsDictionaryWithChildren:
-        self.parent_id = value
-        return self
-
     def with_word(self, value: str) -> ModelsDictionaryWithChildren:
         self.word = value
         return self
 
     def with_word_type(self, value: str) -> ModelsDictionaryWithChildren:
         self.word_type = value
         return self
@@ -91,32 +87,32 @@
 
     def with_false_positives(
         self, value: List[ModelsDictionaryChild]
     ) -> ModelsDictionaryWithChildren:
         self.false_positives = value
         return self
 
+    def with_parent_id(self, value: str) -> ModelsDictionaryWithChildren:
+        self.parent_id = value
+        return self
+
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
         if hasattr(self, "id_"):
             result["id"] = str(self.id_)
         elif include_empty:
             result["id"] = ""
         if hasattr(self, "namespace"):
             result["namespace"] = str(self.namespace)
         elif include_empty:
             result["namespace"] = ""
-        if hasattr(self, "parent_id"):
-            result["parentId"] = str(self.parent_id)
-        elif include_empty:
-            result["parentId"] = ""
         if hasattr(self, "word"):
             result["word"] = str(self.word)
         elif include_empty:
             result["word"] = ""
         if hasattr(self, "word_type"):
             result["wordType"] = str(self.word_type)
         elif include_empty:
@@ -129,42 +125,47 @@
             result["falseNegatives"] = []
         if hasattr(self, "false_positives"):
             result["falsePositives"] = [
                 i0.to_dict(include_empty=include_empty) for i0 in self.false_positives
             ]
         elif include_empty:
             result["falsePositives"] = []
+        if hasattr(self, "parent_id"):
+            result["parentId"] = str(self.parent_id)
+        elif include_empty:
+            result["parentId"] = ""
         return result
 
     # endregion to methods
 
     # region static methods
 
     @classmethod
     def create(
         cls,
         id_: str,
         namespace: str,
-        parent_id: str,
         word: str,
         word_type: str,
         false_negatives: Optional[List[ModelsDictionaryChild]] = None,
         false_positives: Optional[List[ModelsDictionaryChild]] = None,
+        parent_id: Optional[str] = None,
         **kwargs,
     ) -> ModelsDictionaryWithChildren:
         instance = cls()
         instance.id_ = id_
         instance.namespace = namespace
-        instance.parent_id = parent_id
         instance.word = word
         instance.word_type = word_type
         if false_negatives is not None:
             instance.false_negatives = false_negatives
         if false_positives is not None:
             instance.false_positives = false_positives
+        if parent_id is not None:
+            instance.parent_id = parent_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
     ) -> ModelsDictionaryWithChildren:
         instance = cls()
@@ -174,18 +175,14 @@
             instance.id_ = str(dict_["id"])
         elif include_empty:
             instance.id_ = ""
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
         elif include_empty:
             instance.namespace = ""
-        if "parentId" in dict_ and dict_["parentId"] is not None:
-            instance.parent_id = str(dict_["parentId"])
-        elif include_empty:
-            instance.parent_id = ""
         if "word" in dict_ and dict_["word"] is not None:
             instance.word = str(dict_["word"])
         elif include_empty:
             instance.word = ""
         if "wordType" in dict_ and dict_["wordType"] is not None:
             instance.word_type = str(dict_["wordType"])
         elif include_empty:
@@ -200,14 +197,18 @@
         if "falsePositives" in dict_ and dict_["falsePositives"] is not None:
             instance.false_positives = [
                 ModelsDictionaryChild.create_from_dict(i0, include_empty=include_empty)
                 for i0 in dict_["falsePositives"]
             ]
         elif include_empty:
             instance.false_positives = []
+        if "parentId" in dict_ and dict_["parentId"] is not None:
+            instance.parent_id = str(dict_["parentId"])
+        elif include_empty:
+            instance.parent_id = ""
         return instance
 
     @classmethod
     def create_many_from_dict(
         cls, dict_: dict, include_empty: bool = False
     ) -> Dict[str, ModelsDictionaryWithChildren]:
         return (
@@ -245,27 +246,27 @@
             return cls.create_from_dict(any_, include_empty=include_empty)
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
             "id": "id_",
             "namespace": "namespace",
-            "parentId": "parent_id",
             "word": "word",
             "wordType": "word_type",
             "falseNegatives": "false_negatives",
             "falsePositives": "false_positives",
+            "parentId": "parent_id",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
             "id": True,
             "namespace": True,
-            "parentId": True,
             "word": True,
             "wordType": True,
             "falseNegatives": False,
             "falsePositives": False,
+            "parentId": False,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_dictionary_word_changes.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_dictionary_word_changes.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_get_inbox_categories_response_item.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_get_inbox_categories_response_item.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_get_inbox_messages_response.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_get_inbox_messages_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_get_inbox_messages_response_data.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_get_inbox_messages_response_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,41 +46,41 @@
     Properties:
         created_at: (createdAt) REQUIRED int
 
         expired_at: (expiredAt) REQUIRED int
 
         id_: (id) REQUIRED str
 
-        message: (message) REQUIRED Dict[str, Any]
-
         scope: (scope) REQUIRED Union[str, ScopeEnum]
 
         sender_id: (senderId) REQUIRED str
 
         status: (status) REQUIRED Union[str, StatusEnum]
 
         updated_at: (updatedAt) REQUIRED int
 
-        user_ids: (userIds) REQUIRED List[str]
-
         category: (category) OPTIONAL str
+
+        message: (message) OPTIONAL Dict[str, Any]
+
+        user_ids: (userIds) OPTIONAL List[str]
     """
 
     # region fields
 
     created_at: int  # REQUIRED
     expired_at: int  # REQUIRED
     id_: str  # REQUIRED
-    message: Dict[str, Any]  # REQUIRED
     scope: Union[str, ScopeEnum]  # REQUIRED
     sender_id: str  # REQUIRED
     status: Union[str, StatusEnum]  # REQUIRED
     updated_at: int  # REQUIRED
-    user_ids: List[str]  # REQUIRED
     category: str  # OPTIONAL
+    message: Dict[str, Any]  # OPTIONAL
+    user_ids: List[str]  # OPTIONAL
 
     # endregion fields
 
     # region with_x methods
 
     def with_created_at(self, value: int) -> ModelsGetInboxMessagesResponseData:
         self.created_at = value
@@ -90,18 +90,14 @@
         self.expired_at = value
         return self
 
     def with_id(self, value: str) -> ModelsGetInboxMessagesResponseData:
         self.id_ = value
         return self
 
-    def with_message(self, value: Dict[str, Any]) -> ModelsGetInboxMessagesResponseData:
-        self.message = value
-        return self
-
     def with_scope(
         self, value: Union[str, ScopeEnum]
     ) -> ModelsGetInboxMessagesResponseData:
         self.scope = value
         return self
 
     def with_sender_id(self, value: str) -> ModelsGetInboxMessagesResponseData:
@@ -114,22 +110,26 @@
         self.status = value
         return self
 
     def with_updated_at(self, value: int) -> ModelsGetInboxMessagesResponseData:
         self.updated_at = value
         return self
 
-    def with_user_ids(self, value: List[str]) -> ModelsGetInboxMessagesResponseData:
-        self.user_ids = value
-        return self
-
     def with_category(self, value: str) -> ModelsGetInboxMessagesResponseData:
         self.category = value
         return self
 
+    def with_message(self, value: Dict[str, Any]) -> ModelsGetInboxMessagesResponseData:
+        self.message = value
+        return self
+
+    def with_user_ids(self, value: List[str]) -> ModelsGetInboxMessagesResponseData:
+        self.user_ids = value
+        return self
+
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
         if hasattr(self, "created_at"):
@@ -140,18 +140,14 @@
             result["expiredAt"] = int(self.expired_at)
         elif include_empty:
             result["expiredAt"] = 0
         if hasattr(self, "id_"):
             result["id"] = str(self.id_)
         elif include_empty:
             result["id"] = ""
-        if hasattr(self, "message"):
-            result["message"] = {str(k0): v0 for k0, v0 in self.message.items()}
-        elif include_empty:
-            result["message"] = {}
         if hasattr(self, "scope"):
             result["scope"] = str(self.scope)
         elif include_empty:
             result["scope"] = Union[str, ScopeEnum]()
         if hasattr(self, "sender_id"):
             result["senderId"] = str(self.sender_id)
         elif include_empty:
@@ -160,55 +156,61 @@
             result["status"] = str(self.status)
         elif include_empty:
             result["status"] = Union[str, StatusEnum]()
         if hasattr(self, "updated_at"):
             result["updatedAt"] = int(self.updated_at)
         elif include_empty:
             result["updatedAt"] = 0
-        if hasattr(self, "user_ids"):
-            result["userIds"] = [str(i0) for i0 in self.user_ids]
-        elif include_empty:
-            result["userIds"] = []
         if hasattr(self, "category"):
             result["category"] = str(self.category)
         elif include_empty:
             result["category"] = ""
+        if hasattr(self, "message"):
+            result["message"] = {str(k0): v0 for k0, v0 in self.message.items()}
+        elif include_empty:
+            result["message"] = {}
+        if hasattr(self, "user_ids"):
+            result["userIds"] = [str(i0) for i0 in self.user_ids]
+        elif include_empty:
+            result["userIds"] = []
         return result
 
     # endregion to methods
 
     # region static methods
 
     @classmethod
     def create(
         cls,
         created_at: int,
         expired_at: int,
         id_: str,
-        message: Dict[str, Any],
         scope: Union[str, ScopeEnum],
         sender_id: str,
         status: Union[str, StatusEnum],
         updated_at: int,
-        user_ids: List[str],
         category: Optional[str] = None,
+        message: Optional[Dict[str, Any]] = None,
+        user_ids: Optional[List[str]] = None,
         **kwargs,
     ) -> ModelsGetInboxMessagesResponseData:
         instance = cls()
         instance.created_at = created_at
         instance.expired_at = expired_at
         instance.id_ = id_
-        instance.message = message
         instance.scope = scope
         instance.sender_id = sender_id
         instance.status = status
         instance.updated_at = updated_at
-        instance.user_ids = user_ids
         if category is not None:
             instance.category = category
+        if message is not None:
+            instance.message = message
+        if user_ids is not None:
+            instance.user_ids = user_ids
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
     ) -> ModelsGetInboxMessagesResponseData:
         instance = cls()
@@ -222,18 +224,14 @@
             instance.expired_at = int(dict_["expiredAt"])
         elif include_empty:
             instance.expired_at = 0
         if "id" in dict_ and dict_["id"] is not None:
             instance.id_ = str(dict_["id"])
         elif include_empty:
             instance.id_ = ""
-        if "message" in dict_ and dict_["message"] is not None:
-            instance.message = {str(k0): v0 for k0, v0 in dict_["message"].items()}
-        elif include_empty:
-            instance.message = {}
         if "scope" in dict_ and dict_["scope"] is not None:
             instance.scope = str(dict_["scope"])
         elif include_empty:
             instance.scope = Union[str, ScopeEnum]()
         if "senderId" in dict_ and dict_["senderId"] is not None:
             instance.sender_id = str(dict_["senderId"])
         elif include_empty:
@@ -242,22 +240,26 @@
             instance.status = str(dict_["status"])
         elif include_empty:
             instance.status = Union[str, StatusEnum]()
         if "updatedAt" in dict_ and dict_["updatedAt"] is not None:
             instance.updated_at = int(dict_["updatedAt"])
         elif include_empty:
             instance.updated_at = 0
-        if "userIds" in dict_ and dict_["userIds"] is not None:
-            instance.user_ids = [str(i0) for i0 in dict_["userIds"]]
-        elif include_empty:
-            instance.user_ids = []
         if "category" in dict_ and dict_["category"] is not None:
             instance.category = str(dict_["category"])
         elif include_empty:
             instance.category = ""
+        if "message" in dict_ and dict_["message"] is not None:
+            instance.message = {str(k0): v0 for k0, v0 in dict_["message"].items()}
+        elif include_empty:
+            instance.message = {}
+        if "userIds" in dict_ and dict_["userIds"] is not None:
+            instance.user_ids = [str(i0) for i0 in dict_["userIds"]]
+        elif include_empty:
+            instance.user_ids = []
         return instance
 
     @classmethod
     def create_many_from_dict(
         cls, dict_: dict, include_empty: bool = False
     ) -> Dict[str, ModelsGetInboxMessagesResponseData]:
         return (
@@ -296,36 +298,36 @@
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
             "createdAt": "created_at",
             "expiredAt": "expired_at",
             "id": "id_",
-            "message": "message",
             "scope": "scope",
             "senderId": "sender_id",
             "status": "status",
             "updatedAt": "updated_at",
-            "userIds": "user_ids",
             "category": "category",
+            "message": "message",
+            "userIds": "user_ids",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
             "createdAt": True,
             "expiredAt": True,
             "id": True,
-            "message": True,
             "scope": True,
             "senderId": True,
             "status": True,
             "updatedAt": True,
-            "userIds": True,
             "category": False,
+            "message": False,
+            "userIds": False,
         }
 
     @staticmethod
     def get_enum_map() -> Dict[str, List[Any]]:
         return {
             "scope": ["NAMESPACE", "USER"],
             "status": ["DRAFT", "SENT", "UNSENT"],
```

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_get_inbox_stats_response.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_get_inbox_stats_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_get_inbox_users_response.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_get_inbox_users_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_import_config_response.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_import_config_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_json_schema_type.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_json_schema_type.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_message_stats.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_message_stats.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_pagination.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_pagination.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_public_ban_topic_members_request.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_public_ban_topic_members_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_public_ban_topic_members_response.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_public_ban_topic_members_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_public_unban_topic_members_request.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_public_unban_topic_members_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_public_unban_topic_members_response.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_public_unban_topic_members_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_save_inbox_message_request.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_save_inbox_message_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_save_inbox_message_response.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_save_inbox_message_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,32 +46,32 @@
     Properties:
         category: (category) REQUIRED str
 
         expired_at: (expiredAt) REQUIRED int
 
         id_: (id) REQUIRED str
 
-        message: (message) REQUIRED Dict[str, Any]
-
         scope: (scope) REQUIRED Union[str, ScopeEnum]
 
         status: (status) REQUIRED Union[str, StatusEnum]
 
-        user_i_ds: (userIDs) REQUIRED List[str]
+        message: (message) OPTIONAL Dict[str, Any]
+
+        user_i_ds: (userIDs) OPTIONAL List[str]
     """
 
     # region fields
 
     category: str  # REQUIRED
     expired_at: int  # REQUIRED
     id_: str  # REQUIRED
-    message: Dict[str, Any]  # REQUIRED
     scope: Union[str, ScopeEnum]  # REQUIRED
     status: Union[str, StatusEnum]  # REQUIRED
-    user_i_ds: List[str]  # REQUIRED
+    message: Dict[str, Any]  # OPTIONAL
+    user_i_ds: List[str]  # OPTIONAL
 
     # endregion fields
 
     # region with_x methods
 
     def with_category(self, value: str) -> ModelsSaveInboxMessageResponse:
         self.category = value
@@ -81,30 +81,30 @@
         self.expired_at = value
         return self
 
     def with_id(self, value: str) -> ModelsSaveInboxMessageResponse:
         self.id_ = value
         return self
 
-    def with_message(self, value: Dict[str, Any]) -> ModelsSaveInboxMessageResponse:
-        self.message = value
-        return self
-
     def with_scope(
         self, value: Union[str, ScopeEnum]
     ) -> ModelsSaveInboxMessageResponse:
         self.scope = value
         return self
 
     def with_status(
         self, value: Union[str, StatusEnum]
     ) -> ModelsSaveInboxMessageResponse:
         self.status = value
         return self
 
+    def with_message(self, value: Dict[str, Any]) -> ModelsSaveInboxMessageResponse:
+        self.message = value
+        return self
+
     def with_user_i_ds(self, value: List[str]) -> ModelsSaveInboxMessageResponse:
         self.user_i_ds = value
         return self
 
     # endregion with_x methods
 
     # region to methods
@@ -119,26 +119,26 @@
             result["expiredAt"] = int(self.expired_at)
         elif include_empty:
             result["expiredAt"] = 0
         if hasattr(self, "id_"):
             result["id"] = str(self.id_)
         elif include_empty:
             result["id"] = ""
-        if hasattr(self, "message"):
-            result["message"] = {str(k0): v0 for k0, v0 in self.message.items()}
-        elif include_empty:
-            result["message"] = {}
         if hasattr(self, "scope"):
             result["scope"] = str(self.scope)
         elif include_empty:
             result["scope"] = Union[str, ScopeEnum]()
         if hasattr(self, "status"):
             result["status"] = str(self.status)
         elif include_empty:
             result["status"] = Union[str, StatusEnum]()
+        if hasattr(self, "message"):
+            result["message"] = {str(k0): v0 for k0, v0 in self.message.items()}
+        elif include_empty:
+            result["message"] = {}
         if hasattr(self, "user_i_ds"):
             result["userIDs"] = [str(i0) for i0 in self.user_i_ds]
         elif include_empty:
             result["userIDs"] = []
         return result
 
     # endregion to methods
@@ -147,28 +147,30 @@
 
     @classmethod
     def create(
         cls,
         category: str,
         expired_at: int,
         id_: str,
-        message: Dict[str, Any],
         scope: Union[str, ScopeEnum],
         status: Union[str, StatusEnum],
-        user_i_ds: List[str],
+        message: Optional[Dict[str, Any]] = None,
+        user_i_ds: Optional[List[str]] = None,
         **kwargs,
     ) -> ModelsSaveInboxMessageResponse:
         instance = cls()
         instance.category = category
         instance.expired_at = expired_at
         instance.id_ = id_
-        instance.message = message
         instance.scope = scope
         instance.status = status
-        instance.user_i_ds = user_i_ds
+        if message is not None:
+            instance.message = message
+        if user_i_ds is not None:
+            instance.user_i_ds = user_i_ds
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
     ) -> ModelsSaveInboxMessageResponse:
         instance = cls()
@@ -182,26 +184,26 @@
             instance.expired_at = int(dict_["expiredAt"])
         elif include_empty:
             instance.expired_at = 0
         if "id" in dict_ and dict_["id"] is not None:
             instance.id_ = str(dict_["id"])
         elif include_empty:
             instance.id_ = ""
-        if "message" in dict_ and dict_["message"] is not None:
-            instance.message = {str(k0): v0 for k0, v0 in dict_["message"].items()}
-        elif include_empty:
-            instance.message = {}
         if "scope" in dict_ and dict_["scope"] is not None:
             instance.scope = str(dict_["scope"])
         elif include_empty:
             instance.scope = Union[str, ScopeEnum]()
         if "status" in dict_ and dict_["status"] is not None:
             instance.status = str(dict_["status"])
         elif include_empty:
             instance.status = Union[str, StatusEnum]()
+        if "message" in dict_ and dict_["message"] is not None:
+            instance.message = {str(k0): v0 for k0, v0 in dict_["message"].items()}
+        elif include_empty:
+            instance.message = {}
         if "userIDs" in dict_ and dict_["userIDs"] is not None:
             instance.user_i_ds = [str(i0) for i0 in dict_["userIDs"]]
         elif include_empty:
             instance.user_i_ds = []
         return instance
 
     @classmethod
@@ -244,30 +246,30 @@
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
             "category": "category",
             "expiredAt": "expired_at",
             "id": "id_",
-            "message": "message",
             "scope": "scope",
             "status": "status",
+            "message": "message",
             "userIDs": "user_i_ds",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
             "category": True,
             "expiredAt": True,
             "id": True,
-            "message": True,
             "scope": True,
             "status": True,
-            "userIDs": True,
+            "message": False,
+            "userIDs": False,
         }
 
     @staticmethod
     def get_enum_map() -> Dict[str, List[Any]]:
         return {
             "scope": ["NAMESPACE", "USER"],
             "status": ["DRAFT", "SENT", "UNSENT"],
```

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_send_inbox_message_request.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_send_inbox_message_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_send_inbox_message_response.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_send_inbox_message_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_topic_info.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_topic_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_topic_log_item.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_topic_log_item.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_topic_log_with_pagination_response.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_topic_log_with_pagination_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_topic_member_response.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_topic_member_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_topic_member_with_pagination_response.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_topic_member_with_pagination_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_topic_response.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_topic_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_unban_topic_member_param.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_unban_topic_member_param.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_unban_topic_member_result.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_unban_topic_member_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_unsend_inbox_message_request.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_unsend_inbox_message_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_unsend_inbox_message_response.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_unsend_inbox_message_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_update_inbox_category_request.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_update_inbox_category_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_update_inbox_message_request.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_update_inbox_message_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/models_user_inbox.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/models_user_inbox.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/response_error.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/response_error.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/restapi_error_response_body.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/restapi_error_response_body.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/models/topic_info_member.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/models/topic_info_member.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/config/__init__.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/config/__init__.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/config/admin_get_all_config_v1.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/config/admin_get_all_config_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/config/admin_get_config_v1.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/config/admin_get_config_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/config/admin_update_config_v1.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/config/admin_update_config_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/config/export_config.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/config/export_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/config/import_config.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/config/import_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/inbox/__init__.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/inbox/__init__.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/inbox/admin_add_inbox_category.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/inbox/admin_add_inbox_category.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/inbox/admin_delete_inbox_category.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/inbox/admin_delete_inbox_category.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/inbox/admin_delete_inbox_message.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/inbox/admin_delete_inbox_message.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/inbox/admin_get_category_schema.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/inbox/admin_get_category_schema.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/inbox/admin_get_inbox_categories.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/inbox/admin_get_inbox_categories.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/inbox/admin_get_inbox_messages.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/inbox/admin_get_inbox_messages.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/inbox/admin_get_inbox_stats.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/inbox/admin_get_inbox_stats.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/inbox/admin_get_inbox_users.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/inbox/admin_get_inbox_users.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/inbox/admin_save_inbox_message.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/inbox/admin_save_inbox_message.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/inbox/admin_send_inbox_message.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/inbox/admin_send_inbox_message.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/inbox/admin_unsend_inbox_message.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/inbox/admin_unsend_inbox_message.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/inbox/admin_update_inbox_category.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/inbox/admin_update_inbox_category.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/inbox/admin_update_inbox_message.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/inbox/admin_update_inbox_message.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/moderation/__init__.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/moderation/__init__.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/moderation/admin_delete_chat_snapshot.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/moderation/admin_delete_chat_snapshot.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/moderation/admin_get_chat_snapshot.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/moderation/admin_get_chat_snapshot.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/moderation/public_get_chat_snapshot.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/moderation/public_get_chat_snapshot.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/operations/__init__.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/operations/public_get_messages.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/operations/public_get_messages.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/profanity/__init__.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/profanity/__init__.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/profanity/admin_profanity_create.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/profanity/admin_profanity_create.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/profanity/admin_profanity_create_bulk.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/profanity/admin_profanity_create_bulk.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/profanity/admin_profanity_delete.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/profanity/admin_profanity_delete.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/profanity/admin_profanity_export.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/profanity/admin_profanity_export.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/profanity/admin_profanity_group.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/profanity/admin_profanity_group.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/profanity/admin_profanity_import.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/profanity/admin_profanity_import.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/profanity/admin_profanity_query.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/profanity/admin_profanity_query.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/profanity/admin_profanity_update.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/profanity/admin_profanity_update.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/topic/__init__.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/topic/__init__.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/topic/admin_add_topic_member.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/topic/admin_add_topic_member.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/topic/admin_ban_topic_members.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/topic/admin_ban_topic_members.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/topic/admin_channel_topic_info.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/topic/admin_channel_topic_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/topic/admin_channel_topic_list.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/topic/admin_channel_topic_list.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/topic/admin_channel_topic_summary.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/topic/admin_channel_topic_summary.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/topic/admin_chat_history.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/topic/admin_chat_history.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/topic/admin_create_namespace_topic.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/topic/admin_create_namespace_topic.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/topic/admin_create_topic.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/topic/admin_create_topic.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/topic/admin_delete_chat.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/topic/admin_delete_chat.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/topic/admin_delete_topic.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/topic/admin_delete_topic.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/topic/admin_query_topic.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/topic/admin_query_topic.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/topic/admin_query_topic_log.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/topic/admin_query_topic_log.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/topic/admin_query_users_topic.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/topic/admin_query_users_topic.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/topic/admin_remove_topic_member.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/topic/admin_remove_topic_member.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/topic/admin_send_chat.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/topic/admin_send_chat.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/topic/admin_topic_chat_history.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/topic/admin_topic_chat_history.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/topic/admin_topic_list.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/topic/admin_topic_list.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/topic/admin_topic_members.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/topic/admin_topic_members.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/topic/admin_topic_shards.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/topic/admin_topic_shards.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/topic/admin_unban_topic_members.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/topic/admin_unban_topic_members.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/topic/admin_update_topic.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/topic/admin_update_topic.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/topic/public_ban_topic_members.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/topic/public_ban_topic_members.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/topic/public_chat_history.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/topic/public_chat_history.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/topic/public_delete_chat.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/topic/public_delete_chat.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/topic/public_get_muted_topics.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/topic/public_get_muted_topics.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/topic/public_mute_user.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/topic/public_mute_user.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/topic/public_topic_list.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/topic/public_topic_list.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/topic/public_unban_topic_members.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/topic/public_unban_topic_members.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/operations/topic/public_unmute_user.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/operations/topic/public_unmute_user.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/wrappers/__init__.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/wrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/wrappers/_config.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/wrappers/_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/wrappers/_inbox.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/wrappers/_inbox.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/wrappers/_moderation.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/wrappers/_moderation.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/wrappers/_operations.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/wrappers/_operations.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/wrappers/_profanity.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/wrappers/_profanity.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk/api/chat/wrappers/_topic.py` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk/api/chat/wrappers/_topic.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk_service_chat.egg-info/PKG-INFO` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk_service_chat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: accelbyte-py-sdk-service-chat
-Version: 0.8.0
+Version: 0.9.0
 Summary: AccelByte Python SDK - AccelByte Gaming Services Chat Service
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: accelbyte-py-sdk-core
 
 [//]: # (Code generated. DO NOT EDIT!)
```

### Comparing `accelbyte-py-sdk-service-chat-0.8.0/accelbyte_py_sdk_service_chat.egg-info/SOURCES.txt` & `accelbyte-py-sdk-service-chat-0.9.0/accelbyte_py_sdk_service_chat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

