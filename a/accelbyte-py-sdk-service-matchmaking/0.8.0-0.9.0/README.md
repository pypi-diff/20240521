# Comparing `tmp/accelbyte-py-sdk-service-matchmaking-0.8.0.tar.gz` & `tmp/accelbyte-py-sdk-service-matchmaking-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accelbyte-py-sdk-service-matchmaking-0.8.0.tar", last modified: Tue Feb 27 05:40:21 2024, max compression
+gzip compressed data, was "accelbyte-py-sdk-service-matchmaking-0.9.0.tar", last modified: Tue Mar 26 05:43:42 2024, max compression
```

## Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0.tar` & `accelbyte-py-sdk-service-matchmaking-0.9.0.tar`

### file list

```diff
@@ -1,131 +1,131 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:40:21.045095 accelbyte-py-sdk-service-matchmaking-0.8.0/
--rw-r--r--   0 root         (0) root         (0)     1141 2024-02-27 05:40:21.045095 accelbyte-py-sdk-service-matchmaking-0.8.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      881 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:40:21.033095 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:40:21.033095 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:40:21.033095 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/
--rw-rw-r--   0 root         (0) root         (0)     4245 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:40:21.041095 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/
--rw-rw-r--   0 root         (0) root         (0)     5667 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7055 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/log_app_message_declaration.py
--rw-rw-r--   0 root         (0) root         (0)     7956 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_alliance_flexing_rule.py
--rw-rw-r--   0 root         (0) root         (0)     7177 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_alliance_rule.py
--rw-rw-r--   0 root         (0) root         (0)     7177 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_alliance_rule_v1.py
--rw-rw-r--   0 root         (0) root         (0)    15878 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_bucket_mmr_rule.py
--rw-rw-r--   0 root         (0) root         (0)    20462 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_channel.py
--rw-rw-r--   0 root         (0) root         (0)    20551 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_channel_request.py
--rw-rw-r--   0 root         (0) root         (0)    20452 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_channel_v1.py
--rw-rw-r--   0 root         (0) root         (0)     7624 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_combination.py
--rw-rw-r--   0 root         (0) root         (0)    20971 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_create_channel_response.py
--rw-rw-r--   0 root         (0) root         (0)     7211 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_create_mock_ticket.py
--rw-rw-r--   0 root         (0) root         (0)     3788 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_dequeue_request.py
--rw-rw-r--   0 root         (0) root         (0)     5730 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_flexing_rule.py
--rw-rw-r--   0 root         (0) root         (0)     5038 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_get_channels_response.py
--rw-rw-r--   0 root         (0) root         (0)     6950 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_get_mock_matches_response.py
--rw-rw-r--   0 root         (0) root         (0)    11459 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_get_mock_tickets_response.py
--rw-rw-r--   0 root         (0) root         (0)     6527 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_import_config_response.py
--rw-rw-r--   0 root         (0) root         (0)     5642 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_match_add_user_into_session_request.py
--rw-rw-r--   0 root         (0) root         (0)     4231 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_match_option.py
--rw-rw-r--   0 root         (0) root         (0)     4186 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_match_option_rule.py
--rw-rw-r--   0 root         (0) root         (0)     4923 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_match_result_request.py
--rw-rw-r--   0 root         (0) root         (0)     4942 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_match_result_response.py
--rw-rw-r--   0 root         (0) root         (0)     4289 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_matching_ally.py
--rw-rw-r--   0 root         (0) root         (0)     8347 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_matching_party.py
--rw-rw-r--   0 root         (0) root         (0)     5103 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_matching_rule.py
--rw-rw-r--   0 root         (0) root         (0)    17770 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_matchmaking_result.py
--rw-rw-r--   0 root         (0) root         (0)    19153 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_mock_match.py
--rw-rw-r--   0 root         (0) root         (0)    17588 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_mock_ticket.py
--rw-rw-r--   0 root         (0) root         (0)     5440 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_pagination.py
--rw-rw-r--   0 root         (0) root         (0)     4700 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_party_member.py
--rw-rw-r--   0 root         (0) root         (0)     4936 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_player_result_request.py
--rw-rw-r--   0 root         (0) root         (0)     5075 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_player_result_response.py
--rw-rw-r--   0 root         (0) root         (0)     3877 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_query_mock_by.py
--rw-rw-r--   0 root         (0) root         (0)     3810 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_rebalance_request.py
--rw-rw-r--   0 root         (0) root         (0)     4982 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_rebalance_response.py
--rw-rw-r--   0 root         (0) root         (0)     4229 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_region.py
--rw-rw-r--   0 root         (0) root         (0)     4518 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_result_attribute_request.py
--rw-rw-r--   0 root         (0) root         (0)     4530 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_result_attribute_response.py
--rw-rw-r--   0 root         (0) root         (0)     4618 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_role.py
--rw-rw-r--   0 root         (0) root         (0)    18998 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_rule_set.py
--rw-rw-r--   0 root         (0) root         (0)    18155 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_rule_set_v1.py
--rw-rw-r--   0 root         (0) root         (0)     4914 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_selection_rule.py
--rw-rw-r--   0 root         (0) root         (0)     5783 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_sort_ticket.py
--rw-rw-r--   0 root         (0) root         (0)     6548 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_sort_ticket_rule.py
--rw-rw-r--   0 root         (0) root         (0)     7870 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_stat_resume_response.py
--rw-rw-r--   0 root         (0) root         (0)     6029 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_sub_game_mode.py
--rw-rw-r--   0 root         (0) root         (0)     3938 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_ticket_metric_result_record.py
--rw-rw-r--   0 root         (0) root         (0)     7537 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_update_alliance_rule.py
--rw-rw-r--   0 root         (0) root         (0)    19854 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_update_channel_request.py
--rw-rw-r--   0 root         (0) root         (0)     5208 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_update_play_time_weight_request.py
--rw-rw-r--   0 root         (0) root         (0)     5301 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_update_player_playtime_weight_response.py
--rw-rw-r--   0 root         (0) root         (0)    18551 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_update_ruleset.py
--rw-rw-r--   0 root         (0) root         (0)     3241 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_update_ruleset_sub_game_modes.py
--rw-rw-r--   0 root         (0) root         (0)     4439 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/response_error.py
--rw-rw-r--   0 root         (0) root         (0)     4464 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/response_error_v1.py
--rw-rw-r--   0 root         (0) root         (0)    14522 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/service_get_session_history_detailed_response_item.py
--rw-rw-r--   0 root         (0) root         (0)     5504 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/service_get_session_history_search_response.py
--rw-rw-r--   0 root         (0) root         (0)    14071 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/service_get_session_history_search_response_item.py
--rw-rw-r--   0 root         (0) root         (0)     9002 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/service_get_session_history_search_response_item_v2.py
--rw-rw-r--   0 root         (0) root         (0)     5544 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/service_get_session_history_search_response_v2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:40:21.041095 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/
--rw-rw-r--   0 root         (0) root         (0)      440 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:40:21.041095 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/
--rw-rw-r--   0 root         (0) root         (0)     1978 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     9923 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/add_user_into_session_i_3d8cc3.py
--rw-rw-r--   0 root         (0) root         (0)     8050 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/bulk_get_sessions.py
--rw-rw-r--   0 root         (0) root         (0)     8224 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/create_channel_handler.py
--rw-rw-r--   0 root         (0) root         (0)     6980 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/delete_channel_handler.py
--rw-rw-r--   0 root         (0) root         (0)     8553 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/delete_session_in_channel.py
--rw-rw-r--   0 root         (0) root         (0)     9617 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/delete_user_from_sessio_8c8e34.py
--rw-rw-r--   0 root         (0) root         (0)     7762 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/dequeue_session_handler.py
--rw-rw-r--   0 root         (0) root         (0)     6238 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/export_channels.py
--rw-rw-r--   0 root         (0) root         (0)     8272 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/get_all_channels_handler.py
--rw-rw-r--   0 root         (0) root         (0)     7142 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/get_all_party_in_all_channel.py
--rw-rw-r--   0 root         (0) root         (0)     7966 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/get_all_party_in_channel.py
--rw-rw-r--   0 root         (0) root         (0)     8069 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/get_all_sessions_in_channel.py
--rw-rw-r--   0 root         (0) root         (0)     7341 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/get_match_pool_metric.py
--rw-rw-r--   0 root         (0) root         (0)     8382 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/get_session_history_detailed.py
--rw-rw-r--   0 root         (0) root         (0)     7796 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/get_single_matchmaking_channel.py
--rw-rw-r--   0 root         (0) root         (0)     7876 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/get_stat_data.py
--rw-rw-r--   0 root         (0) root         (0)     8779 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/import_channels.py
--rw-rw-r--   0 root         (0) root         (0)     6614 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/public_get_all_matchmak_cd6d3e.py
--rw-rw-r--   0 root         (0) root         (0)     7809 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/public_get_single_match_188a61.py
--rw-rw-r--   0 root         (0) root         (0)     7683 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/query_session_handler.py
--rw-rw-r--   0 root         (0) root         (0)     8035 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/queue_session_handler.py
--rw-rw-r--   0 root         (0) root         (0)     7769 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/rebalance.py
--rw-rw-r--   0 root         (0) root         (0)    12967 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/search_sessions.py
--rw-rw-r--   0 root         (0) root         (0)    13288 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/search_sessions_v2.py
--rw-rw-r--   0 root         (0) root         (0)     7573 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/store_match_results.py
--rw-rw-r--   0 root         (0) root         (0)     8959 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/update_matchmaking_channel.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:40:21.041095 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking_operations/
--rw-rw-r--   0 root         (0) root         (0)      681 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking_operations/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4206 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking_operations/get_healthcheck_info.py
--rw-rw-r--   0 root         (0) root         (0)     4220 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking_operations/handler_v3_healthz.py
--rw-rw-r--   0 root         (0) root         (0)     4753 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking_operations/public_get_messages.py
--rw-rw-r--   0 root         (0) root         (0)     4235 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking_operations/version_check_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:40:21.041095 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/mock_matchmaking/
--rw-rw-r--   0 root         (0) root         (0)      869 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/mock_matchmaking/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     9046 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/mock_matchmaking/bulk_create_mock_tickets.py
--rw-rw-r--   0 root         (0) root         (0)     7703 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/mock_matchmaking/clean_all_mocks.py
--rw-rw-r--   0 root         (0) root         (0)     9198 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/mock_matchmaking/create_mock_tickets.py
--rw-rw-r--   0 root         (0) root         (0)     7939 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/mock_matchmaking/get_all_mock_matches.py
--rw-rw-r--   0 root         (0) root         (0)     7903 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/mock_matchmaking/get_all_mock_tickets.py
--rw-rw-r--   0 root         (0) root         (0)     9116 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/mock_matchmaking/get_mock_matches_by_timestamp.py
--rw-rw-r--   0 root         (0) root         (0)     9072 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/mock_matchmaking/get_mock_tickets_by_timestamp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:40:21.041095 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/social_matchmaking/
--rw-rw-r--   0 root         (0) root         (0)      531 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/social_matchmaking/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8538 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/social_matchmaking/update_play_time_weight.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:40:21.045095 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/wrappers/
--rw-rw-r--   0 root         (0) root         (0)     4642 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/wrappers/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    91511 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/wrappers/_matchmaking.py
--rw-rw-r--   0 root         (0) root         (0)     6232 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/wrappers/_matchmaking_operations.py
--rw-rw-r--   0 root         (0) root         (0)    25954 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/wrappers/_mock_matchmaking.py
--rw-rw-r--   0 root         (0) root         (0)     4871 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/wrappers/_social_matchmaking.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:40:21.045095 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk_service_matchmaking.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1141 2024-02-27 05:40:21.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk_service_matchmaking.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8485 2024-02-27 05:40:21.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk_service_matchmaking.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-27 05:40:21.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk_service_matchmaking.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       22 2024-02-27 05:40:21.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk_service_matchmaking.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-02-27 05:40:21.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk_service_matchmaking.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)      367 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-matchmaking-0.8.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-27 05:40:21.045095 accelbyte-py-sdk-service-matchmaking-0.8.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:43:42.885341 accelbyte-py-sdk-service-matchmaking-0.9.0/
+-rw-r--r--   0 root         (0) root         (0)     1141 2024-03-26 05:43:42.885341 accelbyte-py-sdk-service-matchmaking-0.9.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      881 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:43:42.873342 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:43:42.873342 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:43:42.873342 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/
+-rw-rw-r--   0 root         (0) root         (0)     4245 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:43:42.877342 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/
+-rw-rw-r--   0 root         (0) root         (0)     4869 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7055 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/log_app_message_declaration.py
+-rw-rw-r--   0 root         (0) root         (0)     7956 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_alliance_flexing_rule.py
+-rw-rw-r--   0 root         (0) root         (0)     7177 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_alliance_rule.py
+-rw-rw-r--   0 root         (0) root         (0)     7177 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_alliance_rule_v1.py
+-rw-rw-r--   0 root         (0) root         (0)    15878 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_bucket_mmr_rule.py
+-rw-rw-r--   0 root         (0) root         (0)    20516 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_channel.py
+-rw-rw-r--   0 root         (0) root         (0)    20551 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_channel_request.py
+-rw-rw-r--   0 root         (0) root         (0)    20507 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_channel_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     7680 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_combination.py
+-rw-rw-r--   0 root         (0) root         (0)    21025 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_create_channel_response.py
+-rw-rw-r--   0 root         (0) root         (0)     7211 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_create_mock_ticket.py
+-rw-rw-r--   0 root         (0) root         (0)     3788 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_dequeue_request.py
+-rw-rw-r--   0 root         (0) root         (0)     5730 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_flexing_rule.py
+-rw-rw-r--   0 root         (0) root         (0)     5038 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_get_channels_response.py
+-rw-rw-r--   0 root         (0) root         (0)     6950 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_get_mock_matches_response.py
+-rw-rw-r--   0 root         (0) root         (0)    11459 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_get_mock_tickets_response.py
+-rw-rw-r--   0 root         (0) root         (0)     6527 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_import_config_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5642 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_match_add_user_into_session_request.py
+-rw-rw-r--   0 root         (0) root         (0)     4231 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_match_option.py
+-rw-rw-r--   0 root         (0) root         (0)     4186 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_match_option_rule.py
+-rw-rw-r--   0 root         (0) root         (0)     4923 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_match_result_request.py
+-rw-rw-r--   0 root         (0) root         (0)     4942 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_match_result_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4289 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_matching_ally.py
+-rw-rw-r--   0 root         (0) root         (0)     8411 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_matching_party.py
+-rw-rw-r--   0 root         (0) root         (0)     5103 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_matching_rule.py
+-rw-rw-r--   0 root         (0) root         (0)    17770 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_matchmaking_result.py
+-rw-rw-r--   0 root         (0) root         (0)    19153 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_mock_match.py
+-rw-rw-r--   0 root         (0) root         (0)    17588 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_mock_ticket.py
+-rw-rw-r--   0 root         (0) root         (0)     5440 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_pagination.py
+-rw-rw-r--   0 root         (0) root         (0)     4700 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_party_member.py
+-rw-rw-r--   0 root         (0) root         (0)     4936 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_player_result_request.py
+-rw-rw-r--   0 root         (0) root         (0)     5075 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_player_result_response.py
+-rw-rw-r--   0 root         (0) root         (0)     3877 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_query_mock_by.py
+-rw-rw-r--   0 root         (0) root         (0)     3810 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_rebalance_request.py
+-rw-rw-r--   0 root         (0) root         (0)     4982 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_rebalance_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4229 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_region.py
+-rw-rw-r--   0 root         (0) root         (0)     4518 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_result_attribute_request.py
+-rw-rw-r--   0 root         (0) root         (0)     4530 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_result_attribute_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4618 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_role.py
+-rw-rw-r--   0 root         (0) root         (0)    18813 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_rule_set.py
+-rw-rw-r--   0 root         (0) root         (0)    18101 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_rule_set_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     4442 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_selection_rule.py
+-rw-rw-r--   0 root         (0) root         (0)     4548 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_sort_ticket.py
+-rw-rw-r--   0 root         (0) root         (0)     5291 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_sort_ticket_rule.py
+-rw-rw-r--   0 root         (0) root         (0)     7870 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_stat_resume_response.py
+-rw-rw-r--   0 root         (0) root         (0)     6097 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_sub_game_mode.py
+-rw-rw-r--   0 root         (0) root         (0)     3938 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_ticket_metric_result_record.py
+-rw-rw-r--   0 root         (0) root         (0)     7537 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_update_alliance_rule.py
+-rw-rw-r--   0 root         (0) root         (0)    19854 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_update_channel_request.py
+-rw-rw-r--   0 root         (0) root         (0)     5208 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_update_play_time_weight_request.py
+-rw-rw-r--   0 root         (0) root         (0)     5301 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_update_player_playtime_weight_response.py
+-rw-rw-r--   0 root         (0) root         (0)    17943 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_update_ruleset.py
+-rw-rw-r--   0 root         (0) root         (0)     3241 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_update_ruleset_sub_game_modes.py
+-rw-rw-r--   0 root         (0) root         (0)     4439 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/response_error.py
+-rw-rw-r--   0 root         (0) root         (0)     4464 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/response_error_v1.py
+-rw-rw-r--   0 root         (0) root         (0)    14522 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/service_get_session_history_detailed_response_item.py
+-rw-rw-r--   0 root         (0) root         (0)     5504 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/service_get_session_history_search_response.py
+-rw-rw-r--   0 root         (0) root         (0)    14071 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/service_get_session_history_search_response_item.py
+-rw-rw-r--   0 root         (0) root         (0)     9002 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/service_get_session_history_search_response_item_v2.py
+-rw-rw-r--   0 root         (0) root         (0)     5544 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/service_get_session_history_search_response_v2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:43:42.881341 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/
+-rw-rw-r--   0 root         (0) root         (0)      440 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:43:42.881341 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/
+-rw-rw-r--   0 root         (0) root         (0)     1978 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     9923 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/add_user_into_session_i_3d8cc3.py
+-rw-rw-r--   0 root         (0) root         (0)     8050 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/bulk_get_sessions.py
+-rw-rw-r--   0 root         (0) root         (0)     8224 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/create_channel_handler.py
+-rw-rw-r--   0 root         (0) root         (0)     6980 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/delete_channel_handler.py
+-rw-rw-r--   0 root         (0) root         (0)     8553 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/delete_session_in_channel.py
+-rw-rw-r--   0 root         (0) root         (0)     9617 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/delete_user_from_sessio_8c8e34.py
+-rw-rw-r--   0 root         (0) root         (0)     7762 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/dequeue_session_handler.py
+-rw-rw-r--   0 root         (0) root         (0)     6238 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/export_channels.py
+-rw-rw-r--   0 root         (0) root         (0)     8272 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/get_all_channels_handler.py
+-rw-rw-r--   0 root         (0) root         (0)     7142 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/get_all_party_in_all_channel.py
+-rw-rw-r--   0 root         (0) root         (0)     7966 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/get_all_party_in_channel.py
+-rw-rw-r--   0 root         (0) root         (0)     8069 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/get_all_sessions_in_channel.py
+-rw-rw-r--   0 root         (0) root         (0)     7341 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/get_match_pool_metric.py
+-rw-rw-r--   0 root         (0) root         (0)     8382 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/get_session_history_detailed.py
+-rw-rw-r--   0 root         (0) root         (0)     7796 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/get_single_matchmaking_channel.py
+-rw-rw-r--   0 root         (0) root         (0)     7876 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/get_stat_data.py
+-rw-rw-r--   0 root         (0) root         (0)     8779 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/import_channels.py
+-rw-rw-r--   0 root         (0) root         (0)     6614 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/public_get_all_matchmak_cd6d3e.py
+-rw-rw-r--   0 root         (0) root         (0)     7809 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/public_get_single_match_188a61.py
+-rw-rw-r--   0 root         (0) root         (0)     7683 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/query_session_handler.py
+-rw-rw-r--   0 root         (0) root         (0)     8035 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/queue_session_handler.py
+-rw-rw-r--   0 root         (0) root         (0)     7769 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/rebalance.py
+-rw-rw-r--   0 root         (0) root         (0)    12967 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/search_sessions.py
+-rw-rw-r--   0 root         (0) root         (0)    13288 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/search_sessions_v2.py
+-rw-rw-r--   0 root         (0) root         (0)     7573 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/store_match_results.py
+-rw-rw-r--   0 root         (0) root         (0)     8959 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/update_matchmaking_channel.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:43:42.881341 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking_operations/
+-rw-rw-r--   0 root         (0) root         (0)      681 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking_operations/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4206 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking_operations/get_healthcheck_info.py
+-rw-rw-r--   0 root         (0) root         (0)     4220 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking_operations/handler_v3_healthz.py
+-rw-rw-r--   0 root         (0) root         (0)     4753 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking_operations/public_get_messages.py
+-rw-rw-r--   0 root         (0) root         (0)     4235 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking_operations/version_check_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:43:42.881341 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/mock_matchmaking/
+-rw-rw-r--   0 root         (0) root         (0)      869 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/mock_matchmaking/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     9046 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/mock_matchmaking/bulk_create_mock_tickets.py
+-rw-rw-r--   0 root         (0) root         (0)     7703 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/mock_matchmaking/clean_all_mocks.py
+-rw-rw-r--   0 root         (0) root         (0)     9198 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/mock_matchmaking/create_mock_tickets.py
+-rw-rw-r--   0 root         (0) root         (0)     7939 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/mock_matchmaking/get_all_mock_matches.py
+-rw-rw-r--   0 root         (0) root         (0)     7903 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/mock_matchmaking/get_all_mock_tickets.py
+-rw-rw-r--   0 root         (0) root         (0)     9116 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/mock_matchmaking/get_mock_matches_by_timestamp.py
+-rw-rw-r--   0 root         (0) root         (0)     9072 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/mock_matchmaking/get_mock_tickets_by_timestamp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:43:42.881341 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/social_matchmaking/
+-rw-rw-r--   0 root         (0) root         (0)      531 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/social_matchmaking/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8538 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/social_matchmaking/update_play_time_weight.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:43:42.885341 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/wrappers/
+-rw-rw-r--   0 root         (0) root         (0)     4642 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/wrappers/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    91511 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/wrappers/_matchmaking.py
+-rw-rw-r--   0 root         (0) root         (0)     6232 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/wrappers/_matchmaking_operations.py
+-rw-rw-r--   0 root         (0) root         (0)    25954 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/wrappers/_mock_matchmaking.py
+-rw-rw-r--   0 root         (0) root         (0)     4871 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/wrappers/_social_matchmaking.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:43:42.885341 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk_service_matchmaking.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1141 2024-03-26 05:43:42.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk_service_matchmaking.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8485 2024-03-26 05:43:42.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk_service_matchmaking.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-03-26 05:43:42.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk_service_matchmaking.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 05:43:42.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk_service_matchmaking.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-03-26 05:43:42.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk_service_matchmaking.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)      367 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-matchmaking-0.9.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-03-26 05:43:42.885341 accelbyte-py-sdk-service-matchmaking-0.9.0/setup.cfg
```

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/PKG-INFO` & `accelbyte-py-sdk-service-matchmaking-0.9.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: accelbyte-py-sdk-service-matchmaking
-Version: 0.8.0
+Version: 0.9.0
 Summary: AccelByte Python SDK - AccelByte Gaming Services Matchmaking Service
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: accelbyte-py-sdk-core
 
 [//]: # (Code generated. DO NOT EDIT!)
 
 # AccelByte Modular Python SDK - Service Module
 
 This is a service module for the [AccelByte Modular Python SDK](https://github.com/AccelByte/accelbyte-python-modular-sdk) package.
 
 ```text
 AccelByte Gaming Services Matchmaking Service
-* Version: 2.30.1
+* Version: 2.30.2
 ```
 
 ## Setup
 
 This SDK requires Python 3.9 to be installed.
 
 ### Install with Pip
```

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/README.md` & `accelbyte-py-sdk-service-matchmaking-0.9.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # AccelByte Modular Python SDK - Service Module
 
 This is a service module for the [AccelByte Modular Python SDK](https://github.com/AccelByte/accelbyte-python-modular-sdk) package.
 
 ```text
 AccelByte Gaming Services Matchmaking Service
-* Version: 2.30.1
+* Version: 2.30.2
 ```
 
 ## Setup
 
 This SDK requires Python 3.9 to be installed.
 
 ### Install with Pip
```

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/__init__.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: service-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Matchmaking Service."""
 
-__version__ = "2.30.1"
+__version__ = "2.30.2"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 # matchmaking
 from .wrappers import add_user_into_session_in_channel
```

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/__init__.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: model-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Matchmaking Service."""
 
-__version__ = "2.30.1"
+__version__ = "2.30.2"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .log_app_message_declaration import LogAppMessageDeclaration
 from .models_alliance_flexing_rule import ModelsAllianceFlexingRule
@@ -58,33 +58,18 @@
 from .models_rebalance_request import ModelsRebalanceRequest
 from .models_rebalance_response import ModelsRebalanceResponse
 from .models_region import ModelsRegion
 from .models_result_attribute_request import ModelsResultAttributeRequest
 from .models_result_attribute_response import ModelsResultAttributeResponse
 from .models_role import ModelsRole
 from .models_rule_set import ModelsRuleSet
-from .models_rule_set import (
-    TicketFlexingSelectionEnum as ModelsRuleSetTicketFlexingSelectionEnum,
-)
 from .models_rule_set_v1 import ModelsRuleSetV1
-from .models_rule_set_v1 import (
-    TicketFlexingSelectionEnum as ModelsRuleSetV1TicketFlexingSelectionEnum,
-)
 from .models_selection_rule import ModelsSelectionRule
-from .models_selection_rule import SelectionEnum as ModelsSelectionRuleSelectionEnum
 from .models_sort_ticket import ModelsSortTicket
-from .models_sort_ticket import SearchResultEnum as ModelsSortTicketSearchResultEnum
-from .models_sort_ticket import TicketQueueEnum as ModelsSortTicketTicketQueueEnum
 from .models_sort_ticket_rule import ModelsSortTicketRule
-from .models_sort_ticket_rule import (
-    SearchResultEnum as ModelsSortTicketRuleSearchResultEnum,
-)
-from .models_sort_ticket_rule import (
-    TicketQueueEnum as ModelsSortTicketRuleTicketQueueEnum,
-)
 from .models_stat_resume_response import ModelsStatResumeResponse
 from .models_sub_game_mode import ModelsSubGameMode
 from .models_ticket_metric_result_record import ModelsTicketMetricResultRecord
 from .models_update_alliance_rule import ModelsUpdateAllianceRule
 from .models_update_channel_request import ModelsUpdateChannelRequest
 from .models_update_channel_request import (
     BlockedPlayerOptionEnum as ModelsUpdateChannelRequestBlockedPlayerOptionEnum,
@@ -93,17 +78,14 @@
     SubGamemodeSelectionEnum as ModelsUpdateChannelRequestSubGamemodeSelectionEnum,
 )
 from .models_update_player_playtime_weight_response import (
     ModelsUpdatePlayerPlaytimeWeightResponse,
 )
 from .models_update_play_time_weight_request import ModelsUpdatePlayTimeWeightRequest
 from .models_update_ruleset import ModelsUpdateRuleset
-from .models_update_ruleset import (
-    TicketFlexingSelectionEnum as ModelsUpdateRulesetTicketFlexingSelectionEnum,
-)
 from .models_update_ruleset_sub_game_modes import ModelsUpdateRulesetSubGameModes
 from .response_error import ResponseError
 from .response_error_v1 import ResponseErrorV1
 from .service_get_session_history_detailed_response_item import (
     ServiceGetSessionHistoryDetailedResponseItem,
 )
 from .service_get_session_history_search_response import (
```

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/log_app_message_declaration.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/log_app_message_declaration.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_alliance_flexing_rule.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_alliance_flexing_rule.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_alliance_rule.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_alliance_rule.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_alliance_rule_v1.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_alliance_rule_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_bucket_mmr_rule.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_bucket_mmr_rule.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_channel.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_channel.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,28 +54,28 @@
 
         region_expansion_rate_ms: (region_expansion_rate_ms) REQUIRED int
 
         region_latency_initial_range_ms: (region_latency_initial_range_ms) REQUIRED int
 
         region_latency_max_ms: (region_latency_max_ms) REQUIRED int
 
-        ruleset: (ruleset) REQUIRED ModelsRuleSet
-
         session_queue_timeout_seconds: (session_queue_timeout_seconds) REQUIRED int
 
         slug: (slug) REQUIRED str
 
         social_matchmaking: (social_matchmaking) REQUIRED bool
 
         sub_gamemode_selection: (sub_gamemode_selection) REQUIRED str
 
         updated_at: (updated_at) REQUIRED str
 
         use_sub_gamemode: (use_sub_gamemode) REQUIRED bool
 
+        ruleset: (ruleset) OPTIONAL ModelsRuleSet
+
         ticket_observability_enable: (ticket_observability_enable) OPTIONAL bool
     """
 
     # region fields
 
     blocked_player_option: str  # REQUIRED
     deployment: str  # REQUIRED
@@ -85,21 +85,21 @@
     joinable: bool  # REQUIRED
     max_delay_ms: int  # REQUIRED
     namespace: str  # REQUIRED
     region_expansion_range_ms: int  # REQUIRED
     region_expansion_rate_ms: int  # REQUIRED
     region_latency_initial_range_ms: int  # REQUIRED
     region_latency_max_ms: int  # REQUIRED
-    ruleset: ModelsRuleSet  # REQUIRED
     session_queue_timeout_seconds: int  # REQUIRED
     slug: str  # REQUIRED
     social_matchmaking: bool  # REQUIRED
     sub_gamemode_selection: str  # REQUIRED
     updated_at: str  # REQUIRED
     use_sub_gamemode: bool  # REQUIRED
+    ruleset: ModelsRuleSet  # OPTIONAL
     ticket_observability_enable: bool  # OPTIONAL
 
     # endregion fields
 
     # region with_x methods
 
     def with_blocked_player_option(self, value: str) -> ModelsChannel:
@@ -146,18 +146,14 @@
         self.region_latency_initial_range_ms = value
         return self
 
     def with_region_latency_max_ms(self, value: int) -> ModelsChannel:
         self.region_latency_max_ms = value
         return self
 
-    def with_ruleset(self, value: ModelsRuleSet) -> ModelsChannel:
-        self.ruleset = value
-        return self
-
     def with_session_queue_timeout_seconds(self, value: int) -> ModelsChannel:
         self.session_queue_timeout_seconds = value
         return self
 
     def with_slug(self, value: str) -> ModelsChannel:
         self.slug = value
         return self
@@ -174,14 +170,18 @@
         self.updated_at = value
         return self
 
     def with_use_sub_gamemode(self, value: bool) -> ModelsChannel:
         self.use_sub_gamemode = value
         return self
 
+    def with_ruleset(self, value: ModelsRuleSet) -> ModelsChannel:
+        self.ruleset = value
+        return self
+
     def with_ticket_observability_enable(self, value: bool) -> ModelsChannel:
         self.ticket_observability_enable = value
         return self
 
     # endregion with_x methods
 
     # region to methods
@@ -234,18 +234,14 @@
             )
         elif include_empty:
             result["region_latency_initial_range_ms"] = 0
         if hasattr(self, "region_latency_max_ms"):
             result["region_latency_max_ms"] = int(self.region_latency_max_ms)
         elif include_empty:
             result["region_latency_max_ms"] = 0
-        if hasattr(self, "ruleset"):
-            result["ruleset"] = self.ruleset.to_dict(include_empty=include_empty)
-        elif include_empty:
-            result["ruleset"] = ModelsRuleSet()
         if hasattr(self, "session_queue_timeout_seconds"):
             result["session_queue_timeout_seconds"] = int(
                 self.session_queue_timeout_seconds
             )
         elif include_empty:
             result["session_queue_timeout_seconds"] = 0
         if hasattr(self, "slug"):
@@ -264,14 +260,18 @@
             result["updated_at"] = str(self.updated_at)
         elif include_empty:
             result["updated_at"] = ""
         if hasattr(self, "use_sub_gamemode"):
             result["use_sub_gamemode"] = bool(self.use_sub_gamemode)
         elif include_empty:
             result["use_sub_gamemode"] = False
+        if hasattr(self, "ruleset"):
+            result["ruleset"] = self.ruleset.to_dict(include_empty=include_empty)
+        elif include_empty:
+            result["ruleset"] = ModelsRuleSet()
         if hasattr(self, "ticket_observability_enable"):
             result["ticket_observability_enable"] = bool(
                 self.ticket_observability_enable
             )
         elif include_empty:
             result["ticket_observability_enable"] = False
         return result
@@ -291,21 +291,21 @@
         joinable: bool,
         max_delay_ms: int,
         namespace: str,
         region_expansion_range_ms: int,
         region_expansion_rate_ms: int,
         region_latency_initial_range_ms: int,
         region_latency_max_ms: int,
-        ruleset: ModelsRuleSet,
         session_queue_timeout_seconds: int,
         slug: str,
         social_matchmaking: bool,
         sub_gamemode_selection: str,
         updated_at: str,
         use_sub_gamemode: bool,
+        ruleset: Optional[ModelsRuleSet] = None,
         ticket_observability_enable: Optional[bool] = None,
         **kwargs,
     ) -> ModelsChannel:
         instance = cls()
         instance.blocked_player_option = blocked_player_option
         instance.deployment = deployment
         instance.description = description
@@ -314,21 +314,22 @@
         instance.joinable = joinable
         instance.max_delay_ms = max_delay_ms
         instance.namespace = namespace
         instance.region_expansion_range_ms = region_expansion_range_ms
         instance.region_expansion_rate_ms = region_expansion_rate_ms
         instance.region_latency_initial_range_ms = region_latency_initial_range_ms
         instance.region_latency_max_ms = region_latency_max_ms
-        instance.ruleset = ruleset
         instance.session_queue_timeout_seconds = session_queue_timeout_seconds
         instance.slug = slug
         instance.social_matchmaking = social_matchmaking
         instance.sub_gamemode_selection = sub_gamemode_selection
         instance.updated_at = updated_at
         instance.use_sub_gamemode = use_sub_gamemode
+        if ruleset is not None:
+            instance.ruleset = ruleset
         if ticket_observability_enable is not None:
             instance.ticket_observability_enable = ticket_observability_enable
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
@@ -402,20 +403,14 @@
         if (
             "region_latency_max_ms" in dict_
             and dict_["region_latency_max_ms"] is not None
         ):
             instance.region_latency_max_ms = int(dict_["region_latency_max_ms"])
         elif include_empty:
             instance.region_latency_max_ms = 0
-        if "ruleset" in dict_ and dict_["ruleset"] is not None:
-            instance.ruleset = ModelsRuleSet.create_from_dict(
-                dict_["ruleset"], include_empty=include_empty
-            )
-        elif include_empty:
-            instance.ruleset = ModelsRuleSet()
         if (
             "session_queue_timeout_seconds" in dict_
             and dict_["session_queue_timeout_seconds"] is not None
         ):
             instance.session_queue_timeout_seconds = int(
                 dict_["session_queue_timeout_seconds"]
             )
@@ -440,14 +435,20 @@
             instance.updated_at = str(dict_["updated_at"])
         elif include_empty:
             instance.updated_at = ""
         if "use_sub_gamemode" in dict_ and dict_["use_sub_gamemode"] is not None:
             instance.use_sub_gamemode = bool(dict_["use_sub_gamemode"])
         elif include_empty:
             instance.use_sub_gamemode = False
+        if "ruleset" in dict_ and dict_["ruleset"] is not None:
+            instance.ruleset = ModelsRuleSet.create_from_dict(
+                dict_["ruleset"], include_empty=include_empty
+            )
+        elif include_empty:
+            instance.ruleset = ModelsRuleSet()
         if (
             "ticket_observability_enable" in dict_
             and dict_["ticket_observability_enable"] is not None
         ):
             instance.ticket_observability_enable = bool(
                 dict_["ticket_observability_enable"]
             )
@@ -500,21 +501,21 @@
             "joinable": "joinable",
             "max_delay_ms": "max_delay_ms",
             "namespace": "namespace",
             "region_expansion_range_ms": "region_expansion_range_ms",
             "region_expansion_rate_ms": "region_expansion_rate_ms",
             "region_latency_initial_range_ms": "region_latency_initial_range_ms",
             "region_latency_max_ms": "region_latency_max_ms",
-            "ruleset": "ruleset",
             "session_queue_timeout_seconds": "session_queue_timeout_seconds",
             "slug": "slug",
             "social_matchmaking": "social_matchmaking",
             "sub_gamemode_selection": "sub_gamemode_selection",
             "updated_at": "updated_at",
             "use_sub_gamemode": "use_sub_gamemode",
+            "ruleset": "ruleset",
             "ticket_observability_enable": "ticket_observability_enable",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
             "blocked_player_option": True,
@@ -525,18 +526,18 @@
             "joinable": True,
             "max_delay_ms": True,
             "namespace": True,
             "region_expansion_range_ms": True,
             "region_expansion_rate_ms": True,
             "region_latency_initial_range_ms": True,
             "region_latency_max_ms": True,
-            "ruleset": True,
             "session_queue_timeout_seconds": True,
             "slug": True,
             "social_matchmaking": True,
             "sub_gamemode_selection": True,
             "updated_at": True,
             "use_sub_gamemode": True,
+            "ruleset": False,
             "ticket_observability_enable": False,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_channel_request.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_channel_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_channel_v1.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_channel_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,28 +54,28 @@
 
         region_expansion_rate_ms: (region_expansion_rate_ms) REQUIRED int
 
         region_latency_initial_range_ms: (region_latency_initial_range_ms) REQUIRED int
 
         region_latency_max_ms: (region_latency_max_ms) REQUIRED int
 
-        rule_set: (ruleSet) REQUIRED ModelsRuleSetV1
-
         session_queue_timeout_seconds: (sessionQueueTimeoutSeconds) REQUIRED int
 
         slug: (slug) REQUIRED str
 
         social_matchmaking: (socialMatchmaking) REQUIRED bool
 
         sub_gamemode_selection: (sub_gamemode_selection) REQUIRED str
 
         updated_at: (updatedAt) REQUIRED str
 
         use_sub_gamemode: (use_sub_gamemode) REQUIRED bool
 
+        rule_set: (ruleSet) OPTIONAL ModelsRuleSetV1
+
         ticket_observability_enable: (ticket_observability_enable) OPTIONAL bool
     """
 
     # region fields
 
     blocked_player_option: str  # REQUIRED
     deployment: str  # REQUIRED
@@ -85,21 +85,21 @@
     joinable: bool  # REQUIRED
     max_delay_ms: int  # REQUIRED
     namespace: str  # REQUIRED
     region_expansion_range_ms: int  # REQUIRED
     region_expansion_rate_ms: int  # REQUIRED
     region_latency_initial_range_ms: int  # REQUIRED
     region_latency_max_ms: int  # REQUIRED
-    rule_set: ModelsRuleSetV1  # REQUIRED
     session_queue_timeout_seconds: int  # REQUIRED
     slug: str  # REQUIRED
     social_matchmaking: bool  # REQUIRED
     sub_gamemode_selection: str  # REQUIRED
     updated_at: str  # REQUIRED
     use_sub_gamemode: bool  # REQUIRED
+    rule_set: ModelsRuleSetV1  # OPTIONAL
     ticket_observability_enable: bool  # OPTIONAL
 
     # endregion fields
 
     # region with_x methods
 
     def with_blocked_player_option(self, value: str) -> ModelsChannelV1:
@@ -146,18 +146,14 @@
         self.region_latency_initial_range_ms = value
         return self
 
     def with_region_latency_max_ms(self, value: int) -> ModelsChannelV1:
         self.region_latency_max_ms = value
         return self
 
-    def with_rule_set(self, value: ModelsRuleSetV1) -> ModelsChannelV1:
-        self.rule_set = value
-        return self
-
     def with_session_queue_timeout_seconds(self, value: int) -> ModelsChannelV1:
         self.session_queue_timeout_seconds = value
         return self
 
     def with_slug(self, value: str) -> ModelsChannelV1:
         self.slug = value
         return self
@@ -174,14 +170,18 @@
         self.updated_at = value
         return self
 
     def with_use_sub_gamemode(self, value: bool) -> ModelsChannelV1:
         self.use_sub_gamemode = value
         return self
 
+    def with_rule_set(self, value: ModelsRuleSetV1) -> ModelsChannelV1:
+        self.rule_set = value
+        return self
+
     def with_ticket_observability_enable(self, value: bool) -> ModelsChannelV1:
         self.ticket_observability_enable = value
         return self
 
     # endregion with_x methods
 
     # region to methods
@@ -234,18 +234,14 @@
             )
         elif include_empty:
             result["region_latency_initial_range_ms"] = 0
         if hasattr(self, "region_latency_max_ms"):
             result["region_latency_max_ms"] = int(self.region_latency_max_ms)
         elif include_empty:
             result["region_latency_max_ms"] = 0
-        if hasattr(self, "rule_set"):
-            result["ruleSet"] = self.rule_set.to_dict(include_empty=include_empty)
-        elif include_empty:
-            result["ruleSet"] = ModelsRuleSetV1()
         if hasattr(self, "session_queue_timeout_seconds"):
             result["sessionQueueTimeoutSeconds"] = int(
                 self.session_queue_timeout_seconds
             )
         elif include_empty:
             result["sessionQueueTimeoutSeconds"] = 0
         if hasattr(self, "slug"):
@@ -264,14 +260,18 @@
             result["updatedAt"] = str(self.updated_at)
         elif include_empty:
             result["updatedAt"] = ""
         if hasattr(self, "use_sub_gamemode"):
             result["use_sub_gamemode"] = bool(self.use_sub_gamemode)
         elif include_empty:
             result["use_sub_gamemode"] = False
+        if hasattr(self, "rule_set"):
+            result["ruleSet"] = self.rule_set.to_dict(include_empty=include_empty)
+        elif include_empty:
+            result["ruleSet"] = ModelsRuleSetV1()
         if hasattr(self, "ticket_observability_enable"):
             result["ticket_observability_enable"] = bool(
                 self.ticket_observability_enable
             )
         elif include_empty:
             result["ticket_observability_enable"] = False
         return result
@@ -291,21 +291,21 @@
         joinable: bool,
         max_delay_ms: int,
         namespace: str,
         region_expansion_range_ms: int,
         region_expansion_rate_ms: int,
         region_latency_initial_range_ms: int,
         region_latency_max_ms: int,
-        rule_set: ModelsRuleSetV1,
         session_queue_timeout_seconds: int,
         slug: str,
         social_matchmaking: bool,
         sub_gamemode_selection: str,
         updated_at: str,
         use_sub_gamemode: bool,
+        rule_set: Optional[ModelsRuleSetV1] = None,
         ticket_observability_enable: Optional[bool] = None,
         **kwargs,
     ) -> ModelsChannelV1:
         instance = cls()
         instance.blocked_player_option = blocked_player_option
         instance.deployment = deployment
         instance.description = description
@@ -314,21 +314,22 @@
         instance.joinable = joinable
         instance.max_delay_ms = max_delay_ms
         instance.namespace = namespace
         instance.region_expansion_range_ms = region_expansion_range_ms
         instance.region_expansion_rate_ms = region_expansion_rate_ms
         instance.region_latency_initial_range_ms = region_latency_initial_range_ms
         instance.region_latency_max_ms = region_latency_max_ms
-        instance.rule_set = rule_set
         instance.session_queue_timeout_seconds = session_queue_timeout_seconds
         instance.slug = slug
         instance.social_matchmaking = social_matchmaking
         instance.sub_gamemode_selection = sub_gamemode_selection
         instance.updated_at = updated_at
         instance.use_sub_gamemode = use_sub_gamemode
+        if rule_set is not None:
+            instance.rule_set = rule_set
         if ticket_observability_enable is not None:
             instance.ticket_observability_enable = ticket_observability_enable
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
@@ -400,20 +401,14 @@
         if (
             "region_latency_max_ms" in dict_
             and dict_["region_latency_max_ms"] is not None
         ):
             instance.region_latency_max_ms = int(dict_["region_latency_max_ms"])
         elif include_empty:
             instance.region_latency_max_ms = 0
-        if "ruleSet" in dict_ and dict_["ruleSet"] is not None:
-            instance.rule_set = ModelsRuleSetV1.create_from_dict(
-                dict_["ruleSet"], include_empty=include_empty
-            )
-        elif include_empty:
-            instance.rule_set = ModelsRuleSetV1()
         if (
             "sessionQueueTimeoutSeconds" in dict_
             and dict_["sessionQueueTimeoutSeconds"] is not None
         ):
             instance.session_queue_timeout_seconds = int(
                 dict_["sessionQueueTimeoutSeconds"]
             )
@@ -438,14 +433,20 @@
             instance.updated_at = str(dict_["updatedAt"])
         elif include_empty:
             instance.updated_at = ""
         if "use_sub_gamemode" in dict_ and dict_["use_sub_gamemode"] is not None:
             instance.use_sub_gamemode = bool(dict_["use_sub_gamemode"])
         elif include_empty:
             instance.use_sub_gamemode = False
+        if "ruleSet" in dict_ and dict_["ruleSet"] is not None:
+            instance.rule_set = ModelsRuleSetV1.create_from_dict(
+                dict_["ruleSet"], include_empty=include_empty
+            )
+        elif include_empty:
+            instance.rule_set = ModelsRuleSetV1()
         if (
             "ticket_observability_enable" in dict_
             and dict_["ticket_observability_enable"] is not None
         ):
             instance.ticket_observability_enable = bool(
                 dict_["ticket_observability_enable"]
             )
@@ -498,21 +499,21 @@
             "joinable": "joinable",
             "max_delay_ms": "max_delay_ms",
             "namespace": "namespace",
             "region_expansion_range_ms": "region_expansion_range_ms",
             "region_expansion_rate_ms": "region_expansion_rate_ms",
             "region_latency_initial_range_ms": "region_latency_initial_range_ms",
             "region_latency_max_ms": "region_latency_max_ms",
-            "ruleSet": "rule_set",
             "sessionQueueTimeoutSeconds": "session_queue_timeout_seconds",
             "slug": "slug",
             "socialMatchmaking": "social_matchmaking",
             "sub_gamemode_selection": "sub_gamemode_selection",
             "updatedAt": "updated_at",
             "use_sub_gamemode": "use_sub_gamemode",
+            "ruleSet": "rule_set",
             "ticket_observability_enable": "ticket_observability_enable",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
             "blocked_player_option": True,
@@ -523,18 +524,18 @@
             "joinable": True,
             "max_delay_ms": True,
             "namespace": True,
             "region_expansion_range_ms": True,
             "region_expansion_rate_ms": True,
             "region_latency_initial_range_ms": True,
             "region_latency_max_ms": True,
-            "ruleSet": True,
             "sessionQueueTimeoutSeconds": True,
             "slug": True,
             "socialMatchmaking": True,
             "sub_gamemode_selection": True,
             "updatedAt": True,
             "use_sub_gamemode": True,
+            "ruleSet": False,
             "ticket_observability_enable": False,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_combination.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_combination.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,41 +30,37 @@
 from ..models.models_role import ModelsRole
 
 
 class ModelsCombination(Model):
     """Models combination (models.Combination)
 
     Properties:
-        alliances: (alliances) REQUIRED List[List[ModelsRole]]
-
         has_combination: (has_combination) REQUIRED bool
 
         role_flexing_enable: (role_flexing_enable) REQUIRED bool
 
         role_flexing_player: (role_flexing_player) REQUIRED int
 
         role_flexing_second: (role_flexing_second) REQUIRED int
+
+        alliances: (alliances) OPTIONAL List[List[ModelsRole]]
     """
 
     # region fields
 
-    alliances: List[List[ModelsRole]]  # REQUIRED
     has_combination: bool  # REQUIRED
     role_flexing_enable: bool  # REQUIRED
     role_flexing_player: int  # REQUIRED
     role_flexing_second: int  # REQUIRED
+    alliances: List[List[ModelsRole]]  # OPTIONAL
 
     # endregion fields
 
     # region with_x methods
 
-    def with_alliances(self, value: List[List[ModelsRole]]) -> ModelsCombination:
-        self.alliances = value
-        return self
-
     def with_has_combination(self, value: bool) -> ModelsCombination:
         self.has_combination = value
         return self
 
     def with_role_flexing_enable(self, value: bool) -> ModelsCombination:
         self.role_flexing_enable = value
         return self
@@ -73,27 +69,24 @@
         self.role_flexing_player = value
         return self
 
     def with_role_flexing_second(self, value: int) -> ModelsCombination:
         self.role_flexing_second = value
         return self
 
+    def with_alliances(self, value: List[List[ModelsRole]]) -> ModelsCombination:
+        self.alliances = value
+        return self
+
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
-        if hasattr(self, "alliances"):
-            result["alliances"] = [
-                [i1.to_dict(include_empty=include_empty) for i1 in i0]
-                for i0 in self.alliances
-            ]
-        elif include_empty:
-            result["alliances"] = []
         if hasattr(self, "has_combination"):
             result["has_combination"] = bool(self.has_combination)
         elif include_empty:
             result["has_combination"] = False
         if hasattr(self, "role_flexing_enable"):
             result["role_flexing_enable"] = bool(self.role_flexing_enable)
         elif include_empty:
@@ -102,55 +95,53 @@
             result["role_flexing_player"] = int(self.role_flexing_player)
         elif include_empty:
             result["role_flexing_player"] = 0
         if hasattr(self, "role_flexing_second"):
             result["role_flexing_second"] = int(self.role_flexing_second)
         elif include_empty:
             result["role_flexing_second"] = 0
+        if hasattr(self, "alliances"):
+            result["alliances"] = [
+                [i1.to_dict(include_empty=include_empty) for i1 in i0]
+                for i0 in self.alliances
+            ]
+        elif include_empty:
+            result["alliances"] = []
         return result
 
     # endregion to methods
 
     # region static methods
 
     @classmethod
     def create(
         cls,
-        alliances: List[List[ModelsRole]],
         has_combination: bool,
         role_flexing_enable: bool,
         role_flexing_player: int,
         role_flexing_second: int,
+        alliances: Optional[List[List[ModelsRole]]] = None,
         **kwargs,
     ) -> ModelsCombination:
         instance = cls()
-        instance.alliances = alliances
         instance.has_combination = has_combination
         instance.role_flexing_enable = role_flexing_enable
         instance.role_flexing_player = role_flexing_player
         instance.role_flexing_second = role_flexing_second
+        if alliances is not None:
+            instance.alliances = alliances
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
     ) -> ModelsCombination:
         instance = cls()
         if not dict_:
             return instance
-        if "alliances" in dict_ and dict_["alliances"] is not None:
-            instance.alliances = [
-                [
-                    ModelsRole.create_from_dict(i1, include_empty=include_empty)
-                    for i1 in i0
-                ]
-                for i0 in dict_["alliances"]
-            ]
-        elif include_empty:
-            instance.alliances = []
         if "has_combination" in dict_ and dict_["has_combination"] is not None:
             instance.has_combination = bool(dict_["has_combination"])
         elif include_empty:
             instance.has_combination = False
         if "role_flexing_enable" in dict_ and dict_["role_flexing_enable"] is not None:
             instance.role_flexing_enable = bool(dict_["role_flexing_enable"])
         elif include_empty:
@@ -159,14 +150,24 @@
             instance.role_flexing_player = int(dict_["role_flexing_player"])
         elif include_empty:
             instance.role_flexing_player = 0
         if "role_flexing_second" in dict_ and dict_["role_flexing_second"] is not None:
             instance.role_flexing_second = int(dict_["role_flexing_second"])
         elif include_empty:
             instance.role_flexing_second = 0
+        if "alliances" in dict_ and dict_["alliances"] is not None:
+            instance.alliances = [
+                [
+                    ModelsRole.create_from_dict(i1, include_empty=include_empty)
+                    for i1 in i0
+                ]
+                for i0 in dict_["alliances"]
+            ]
+        elif include_empty:
+            instance.alliances = []
         return instance
 
     @classmethod
     def create_many_from_dict(
         cls, dict_: dict, include_empty: bool = False
     ) -> Dict[str, ModelsCombination]:
         return (
@@ -200,25 +201,25 @@
                 raise ValueError()
         else:
             return cls.create_from_dict(any_, include_empty=include_empty)
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
-            "alliances": "alliances",
             "has_combination": "has_combination",
             "role_flexing_enable": "role_flexing_enable",
             "role_flexing_player": "role_flexing_player",
             "role_flexing_second": "role_flexing_second",
+            "alliances": "alliances",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
-            "alliances": True,
             "has_combination": True,
             "role_flexing_enable": True,
             "role_flexing_player": True,
             "role_flexing_second": True,
+            "alliances": False,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_create_channel_response.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_create_channel_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,28 +54,28 @@
 
         region_expansion_rate_ms: (region_expansion_rate_ms) REQUIRED int
 
         region_latency_initial_range_ms: (region_latency_initial_range_ms) REQUIRED int
 
         region_latency_max_ms: (region_latency_max_ms) REQUIRED int
 
-        ruleset: (ruleset) REQUIRED ModelsRuleSet
-
         session_queue_timeout_seconds: (session_queue_timeout_seconds) REQUIRED int
 
         slug: (slug) REQUIRED str
 
         social_matchmaking: (social_matchmaking) REQUIRED bool
 
         sub_gamemode_selection: (sub_gamemode_selection) REQUIRED str
 
         updated_at: (updated_at) REQUIRED str
 
         use_sub_gamemode: (use_sub_gamemode) REQUIRED bool
 
+        ruleset: (ruleset) OPTIONAL ModelsRuleSet
+
         ticket_observability_enable: (ticket_observability_enable) OPTIONAL bool
     """
 
     # region fields
 
     blocked_player_option: str  # REQUIRED
     deployment: str  # REQUIRED
@@ -85,21 +85,21 @@
     joinable: bool  # REQUIRED
     max_delay_ms: int  # REQUIRED
     namespace: str  # REQUIRED
     region_expansion_range_ms: int  # REQUIRED
     region_expansion_rate_ms: int  # REQUIRED
     region_latency_initial_range_ms: int  # REQUIRED
     region_latency_max_ms: int  # REQUIRED
-    ruleset: ModelsRuleSet  # REQUIRED
     session_queue_timeout_seconds: int  # REQUIRED
     slug: str  # REQUIRED
     social_matchmaking: bool  # REQUIRED
     sub_gamemode_selection: str  # REQUIRED
     updated_at: str  # REQUIRED
     use_sub_gamemode: bool  # REQUIRED
+    ruleset: ModelsRuleSet  # OPTIONAL
     ticket_observability_enable: bool  # OPTIONAL
 
     # endregion fields
 
     # region with_x methods
 
     def with_blocked_player_option(self, value: str) -> ModelsCreateChannelResponse:
@@ -150,18 +150,14 @@
         self.region_latency_initial_range_ms = value
         return self
 
     def with_region_latency_max_ms(self, value: int) -> ModelsCreateChannelResponse:
         self.region_latency_max_ms = value
         return self
 
-    def with_ruleset(self, value: ModelsRuleSet) -> ModelsCreateChannelResponse:
-        self.ruleset = value
-        return self
-
     def with_session_queue_timeout_seconds(
         self, value: int
     ) -> ModelsCreateChannelResponse:
         self.session_queue_timeout_seconds = value
         return self
 
     def with_slug(self, value: str) -> ModelsCreateChannelResponse:
@@ -180,14 +176,18 @@
         self.updated_at = value
         return self
 
     def with_use_sub_gamemode(self, value: bool) -> ModelsCreateChannelResponse:
         self.use_sub_gamemode = value
         return self
 
+    def with_ruleset(self, value: ModelsRuleSet) -> ModelsCreateChannelResponse:
+        self.ruleset = value
+        return self
+
     def with_ticket_observability_enable(
         self, value: bool
     ) -> ModelsCreateChannelResponse:
         self.ticket_observability_enable = value
         return self
 
     # endregion with_x methods
@@ -242,18 +242,14 @@
             )
         elif include_empty:
             result["region_latency_initial_range_ms"] = 0
         if hasattr(self, "region_latency_max_ms"):
             result["region_latency_max_ms"] = int(self.region_latency_max_ms)
         elif include_empty:
             result["region_latency_max_ms"] = 0
-        if hasattr(self, "ruleset"):
-            result["ruleset"] = self.ruleset.to_dict(include_empty=include_empty)
-        elif include_empty:
-            result["ruleset"] = ModelsRuleSet()
         if hasattr(self, "session_queue_timeout_seconds"):
             result["session_queue_timeout_seconds"] = int(
                 self.session_queue_timeout_seconds
             )
         elif include_empty:
             result["session_queue_timeout_seconds"] = 0
         if hasattr(self, "slug"):
@@ -272,14 +268,18 @@
             result["updated_at"] = str(self.updated_at)
         elif include_empty:
             result["updated_at"] = ""
         if hasattr(self, "use_sub_gamemode"):
             result["use_sub_gamemode"] = bool(self.use_sub_gamemode)
         elif include_empty:
             result["use_sub_gamemode"] = False
+        if hasattr(self, "ruleset"):
+            result["ruleset"] = self.ruleset.to_dict(include_empty=include_empty)
+        elif include_empty:
+            result["ruleset"] = ModelsRuleSet()
         if hasattr(self, "ticket_observability_enable"):
             result["ticket_observability_enable"] = bool(
                 self.ticket_observability_enable
             )
         elif include_empty:
             result["ticket_observability_enable"] = False
         return result
@@ -299,21 +299,21 @@
         joinable: bool,
         max_delay_ms: int,
         namespace: str,
         region_expansion_range_ms: int,
         region_expansion_rate_ms: int,
         region_latency_initial_range_ms: int,
         region_latency_max_ms: int,
-        ruleset: ModelsRuleSet,
         session_queue_timeout_seconds: int,
         slug: str,
         social_matchmaking: bool,
         sub_gamemode_selection: str,
         updated_at: str,
         use_sub_gamemode: bool,
+        ruleset: Optional[ModelsRuleSet] = None,
         ticket_observability_enable: Optional[bool] = None,
         **kwargs,
     ) -> ModelsCreateChannelResponse:
         instance = cls()
         instance.blocked_player_option = blocked_player_option
         instance.deployment = deployment
         instance.description = description
@@ -322,21 +322,22 @@
         instance.joinable = joinable
         instance.max_delay_ms = max_delay_ms
         instance.namespace = namespace
         instance.region_expansion_range_ms = region_expansion_range_ms
         instance.region_expansion_rate_ms = region_expansion_rate_ms
         instance.region_latency_initial_range_ms = region_latency_initial_range_ms
         instance.region_latency_max_ms = region_latency_max_ms
-        instance.ruleset = ruleset
         instance.session_queue_timeout_seconds = session_queue_timeout_seconds
         instance.slug = slug
         instance.social_matchmaking = social_matchmaking
         instance.sub_gamemode_selection = sub_gamemode_selection
         instance.updated_at = updated_at
         instance.use_sub_gamemode = use_sub_gamemode
+        if ruleset is not None:
+            instance.ruleset = ruleset
         if ticket_observability_enable is not None:
             instance.ticket_observability_enable = ticket_observability_enable
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
@@ -410,20 +411,14 @@
         if (
             "region_latency_max_ms" in dict_
             and dict_["region_latency_max_ms"] is not None
         ):
             instance.region_latency_max_ms = int(dict_["region_latency_max_ms"])
         elif include_empty:
             instance.region_latency_max_ms = 0
-        if "ruleset" in dict_ and dict_["ruleset"] is not None:
-            instance.ruleset = ModelsRuleSet.create_from_dict(
-                dict_["ruleset"], include_empty=include_empty
-            )
-        elif include_empty:
-            instance.ruleset = ModelsRuleSet()
         if (
             "session_queue_timeout_seconds" in dict_
             and dict_["session_queue_timeout_seconds"] is not None
         ):
             instance.session_queue_timeout_seconds = int(
                 dict_["session_queue_timeout_seconds"]
             )
@@ -448,14 +443,20 @@
             instance.updated_at = str(dict_["updated_at"])
         elif include_empty:
             instance.updated_at = ""
         if "use_sub_gamemode" in dict_ and dict_["use_sub_gamemode"] is not None:
             instance.use_sub_gamemode = bool(dict_["use_sub_gamemode"])
         elif include_empty:
             instance.use_sub_gamemode = False
+        if "ruleset" in dict_ and dict_["ruleset"] is not None:
+            instance.ruleset = ModelsRuleSet.create_from_dict(
+                dict_["ruleset"], include_empty=include_empty
+            )
+        elif include_empty:
+            instance.ruleset = ModelsRuleSet()
         if (
             "ticket_observability_enable" in dict_
             and dict_["ticket_observability_enable"] is not None
         ):
             instance.ticket_observability_enable = bool(
                 dict_["ticket_observability_enable"]
             )
@@ -512,21 +513,21 @@
             "joinable": "joinable",
             "max_delay_ms": "max_delay_ms",
             "namespace": "namespace",
             "region_expansion_range_ms": "region_expansion_range_ms",
             "region_expansion_rate_ms": "region_expansion_rate_ms",
             "region_latency_initial_range_ms": "region_latency_initial_range_ms",
             "region_latency_max_ms": "region_latency_max_ms",
-            "ruleset": "ruleset",
             "session_queue_timeout_seconds": "session_queue_timeout_seconds",
             "slug": "slug",
             "social_matchmaking": "social_matchmaking",
             "sub_gamemode_selection": "sub_gamemode_selection",
             "updated_at": "updated_at",
             "use_sub_gamemode": "use_sub_gamemode",
+            "ruleset": "ruleset",
             "ticket_observability_enable": "ticket_observability_enable",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
             "blocked_player_option": True,
@@ -537,18 +538,18 @@
             "joinable": True,
             "max_delay_ms": True,
             "namespace": True,
             "region_expansion_range_ms": True,
             "region_expansion_rate_ms": True,
             "region_latency_initial_range_ms": True,
             "region_latency_max_ms": True,
-            "ruleset": True,
             "session_queue_timeout_seconds": True,
             "slug": True,
             "social_matchmaking": True,
             "sub_gamemode_selection": True,
             "updated_at": True,
             "use_sub_gamemode": True,
+            "ruleset": False,
             "ticket_observability_enable": False,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_create_mock_ticket.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_create_mock_ticket.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_dequeue_request.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_dequeue_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_flexing_rule.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_flexing_rule.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_get_channels_response.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_get_channels_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_get_mock_matches_response.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_get_mock_matches_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_get_mock_tickets_response.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_get_mock_tickets_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_import_config_response.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_import_config_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_match_add_user_into_session_request.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_match_add_user_into_session_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_match_option.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_match_option.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_match_option_rule.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_match_option_rule.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_match_result_request.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_match_result_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_match_result_response.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_match_result_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_matching_ally.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_matching_ally.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_matching_party.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_matching_party.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,27 +38,27 @@
 
         party_attributes: (party_attributes) REQUIRED Dict[str, Any]
 
         party_id: (party_id) REQUIRED str
 
         party_members: (party_members) REQUIRED List[ModelsPartyMember]
 
-        ticket_created_at: (ticket_created_at) REQUIRED int
-
         ticket_id: (ticket_id) REQUIRED str
+
+        ticket_created_at: (ticket_created_at) OPTIONAL int
     """
 
     # region fields
 
     first_ticket_created_at: int  # REQUIRED
     party_attributes: Dict[str, Any]  # REQUIRED
     party_id: str  # REQUIRED
     party_members: List[ModelsPartyMember]  # REQUIRED
-    ticket_created_at: int  # REQUIRED
     ticket_id: str  # REQUIRED
+    ticket_created_at: int  # OPTIONAL
 
     # endregion fields
 
     # region with_x methods
 
     def with_first_ticket_created_at(self, value: int) -> ModelsMatchingParty:
         self.first_ticket_created_at = value
@@ -72,22 +72,22 @@
         self.party_id = value
         return self
 
     def with_party_members(self, value: List[ModelsPartyMember]) -> ModelsMatchingParty:
         self.party_members = value
         return self
 
-    def with_ticket_created_at(self, value: int) -> ModelsMatchingParty:
-        self.ticket_created_at = value
-        return self
-
     def with_ticket_id(self, value: str) -> ModelsMatchingParty:
         self.ticket_id = value
         return self
 
+    def with_ticket_created_at(self, value: int) -> ModelsMatchingParty:
+        self.ticket_created_at = value
+        return self
+
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
         if hasattr(self, "first_ticket_created_at"):
@@ -106,46 +106,47 @@
             result["party_id"] = ""
         if hasattr(self, "party_members"):
             result["party_members"] = [
                 i0.to_dict(include_empty=include_empty) for i0 in self.party_members
             ]
         elif include_empty:
             result["party_members"] = []
-        if hasattr(self, "ticket_created_at"):
-            result["ticket_created_at"] = int(self.ticket_created_at)
-        elif include_empty:
-            result["ticket_created_at"] = 0
         if hasattr(self, "ticket_id"):
             result["ticket_id"] = str(self.ticket_id)
         elif include_empty:
             result["ticket_id"] = ""
+        if hasattr(self, "ticket_created_at"):
+            result["ticket_created_at"] = int(self.ticket_created_at)
+        elif include_empty:
+            result["ticket_created_at"] = 0
         return result
 
     # endregion to methods
 
     # region static methods
 
     @classmethod
     def create(
         cls,
         first_ticket_created_at: int,
         party_attributes: Dict[str, Any],
         party_id: str,
         party_members: List[ModelsPartyMember],
-        ticket_created_at: int,
         ticket_id: str,
+        ticket_created_at: Optional[int] = None,
         **kwargs,
     ) -> ModelsMatchingParty:
         instance = cls()
         instance.first_ticket_created_at = first_ticket_created_at
         instance.party_attributes = party_attributes
         instance.party_id = party_id
         instance.party_members = party_members
-        instance.ticket_created_at = ticket_created_at
         instance.ticket_id = ticket_id
+        if ticket_created_at is not None:
+            instance.ticket_created_at = ticket_created_at
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
     ) -> ModelsMatchingParty:
         instance = cls()
@@ -171,22 +172,22 @@
         if "party_members" in dict_ and dict_["party_members"] is not None:
             instance.party_members = [
                 ModelsPartyMember.create_from_dict(i0, include_empty=include_empty)
                 for i0 in dict_["party_members"]
             ]
         elif include_empty:
             instance.party_members = []
-        if "ticket_created_at" in dict_ and dict_["ticket_created_at"] is not None:
-            instance.ticket_created_at = int(dict_["ticket_created_at"])
-        elif include_empty:
-            instance.ticket_created_at = 0
         if "ticket_id" in dict_ and dict_["ticket_id"] is not None:
             instance.ticket_id = str(dict_["ticket_id"])
         elif include_empty:
             instance.ticket_id = ""
+        if "ticket_created_at" in dict_ and dict_["ticket_created_at"] is not None:
+            instance.ticket_created_at = int(dict_["ticket_created_at"])
+        elif include_empty:
+            instance.ticket_created_at = 0
         return instance
 
     @classmethod
     def create_many_from_dict(
         cls, dict_: dict, include_empty: bool = False
     ) -> Dict[str, ModelsMatchingParty]:
         return (
@@ -224,23 +225,23 @@
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
             "first_ticket_created_at": "first_ticket_created_at",
             "party_attributes": "party_attributes",
             "party_id": "party_id",
             "party_members": "party_members",
-            "ticket_created_at": "ticket_created_at",
             "ticket_id": "ticket_id",
+            "ticket_created_at": "ticket_created_at",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
             "first_ticket_created_at": True,
             "party_attributes": True,
             "party_id": True,
             "party_members": True,
-            "ticket_created_at": True,
             "ticket_id": True,
+            "ticket_created_at": False,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_matching_rule.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_matching_rule.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_matchmaking_result.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_matchmaking_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_mock_match.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_mock_match.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_mock_ticket.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_mock_ticket.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_pagination.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_pagination.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_party_member.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_party_member.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_player_result_request.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_player_result_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_player_result_response.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_player_result_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_query_mock_by.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_query_mock_by.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_rebalance_request.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_rebalance_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_rebalance_response.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_rebalance_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_region.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_region.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_result_attribute_request.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_result_attribute_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_result_attribute_response.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_result_attribute_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_role.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_role.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_rule_set.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_rule_set.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,165 +22,176 @@
 # pylint: disable=too-many-statements
 # pylint: disable=unused-import
 
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Model
-from accelbyte_py_sdk.core import StrEnum
 
 from ..models.models_alliance_flexing_rule import ModelsAllianceFlexingRule
 from ..models.models_alliance_rule import ModelsAllianceRule
 from ..models.models_bucket_mmr_rule import ModelsBucketMMRRule
 from ..models.models_flexing_rule import ModelsFlexingRule
 from ..models.models_match_option_rule import ModelsMatchOptionRule
 from ..models.models_matching_rule import ModelsMatchingRule
 from ..models.models_selection_rule import ModelsSelectionRule
 from ..models.models_sort_ticket import ModelsSortTicket
 from ..models.models_sort_ticket_rule import ModelsSortTicketRule
 from ..models.models_sub_game_mode import ModelsSubGameMode
 
 
-class TicketFlexingSelectionEnum(StrEnum):
-    NEWEST = "newest"
-    OLDEST = "oldest"
-    PIVOT = "pivot"
-    RANDOM = "random"
-
-
 class ModelsRuleSet(Model):
     """Models rule set (models.RuleSet)
 
     Properties:
-        alliance: (alliance) REQUIRED ModelsAllianceRule
-
         batch_size: (batch_size) REQUIRED int
 
-        flexing_rule: (flexing_rule) REQUIRED List[ModelsFlexingRule]
+        rebalance_enable: (rebalance_enable) REQUIRED bool
 
-        match_options: (match_options) REQUIRED ModelsMatchOptionRule
+        ticket_flexing_selection: (ticket_flexing_selection) REQUIRED str
 
-        matching_rule: (matching_rule) REQUIRED List[ModelsMatchingRule]
+        alliance: (alliance) OPTIONAL ModelsAllianceRule
 
-        rebalance_enable: (rebalance_enable) REQUIRED bool
+        alliance_flexing_rule: (alliance_flexing_rule) OPTIONAL List[ModelsAllianceFlexingRule]
 
-        sort_ticket: (sort_ticket) REQUIRED ModelsSortTicket
+        bucket_mmr_rule: (bucket_mmr_rule) OPTIONAL ModelsBucketMMRRule
 
-        sort_tickets: (sort_tickets) REQUIRED List[ModelsSortTicketRule]
+        flexing_rule: (flexing_rule) OPTIONAL List[ModelsFlexingRule]
 
-        ticket_flexing_selection: (ticket_flexing_selection) REQUIRED Union[str, TicketFlexingSelectionEnum]
+        match_options: (match_options) OPTIONAL ModelsMatchOptionRule
 
-        ticket_flexing_selections: (ticket_flexing_selections) REQUIRED List[ModelsSelectionRule]
+        matching_rule: (matching_rule) OPTIONAL List[ModelsMatchingRule]
 
-        alliance_flexing_rule: (alliance_flexing_rule) OPTIONAL List[ModelsAllianceFlexingRule]
+        sort_ticket: (sort_ticket) OPTIONAL ModelsSortTicket
 
-        bucket_mmr_rule: (bucket_mmr_rule) OPTIONAL ModelsBucketMMRRule
+        sort_tickets: (sort_tickets) OPTIONAL List[ModelsSortTicketRule]
 
         sub_game_modes: (sub_game_modes) OPTIONAL Dict[str, ModelsSubGameMode]
 
+        ticket_flexing_selections: (ticket_flexing_selections) OPTIONAL List[ModelsSelectionRule]
+
         use_newest_ticket_for_flexing: (use_newest_ticket_for_flexing) OPTIONAL bool
     """
 
     # region fields
 
-    alliance: ModelsAllianceRule  # REQUIRED
     batch_size: int  # REQUIRED
-    flexing_rule: List[ModelsFlexingRule]  # REQUIRED
-    match_options: ModelsMatchOptionRule  # REQUIRED
-    matching_rule: List[ModelsMatchingRule]  # REQUIRED
     rebalance_enable: bool  # REQUIRED
-    sort_ticket: ModelsSortTicket  # REQUIRED
-    sort_tickets: List[ModelsSortTicketRule]  # REQUIRED
-    ticket_flexing_selection: Union[str, TicketFlexingSelectionEnum]  # REQUIRED
-    ticket_flexing_selections: List[ModelsSelectionRule]  # REQUIRED
+    ticket_flexing_selection: str  # REQUIRED
+    alliance: ModelsAllianceRule  # OPTIONAL
     alliance_flexing_rule: List[ModelsAllianceFlexingRule]  # OPTIONAL
     bucket_mmr_rule: ModelsBucketMMRRule  # OPTIONAL
+    flexing_rule: List[ModelsFlexingRule]  # OPTIONAL
+    match_options: ModelsMatchOptionRule  # OPTIONAL
+    matching_rule: List[ModelsMatchingRule]  # OPTIONAL
+    sort_ticket: ModelsSortTicket  # OPTIONAL
+    sort_tickets: List[ModelsSortTicketRule]  # OPTIONAL
     sub_game_modes: Dict[str, ModelsSubGameMode]  # OPTIONAL
+    ticket_flexing_selections: List[ModelsSelectionRule]  # OPTIONAL
     use_newest_ticket_for_flexing: bool  # OPTIONAL
 
     # endregion fields
 
     # region with_x methods
 
+    def with_batch_size(self, value: int) -> ModelsRuleSet:
+        self.batch_size = value
+        return self
+
+    def with_rebalance_enable(self, value: bool) -> ModelsRuleSet:
+        self.rebalance_enable = value
+        return self
+
+    def with_ticket_flexing_selection(self, value: str) -> ModelsRuleSet:
+        self.ticket_flexing_selection = value
+        return self
+
     def with_alliance(self, value: ModelsAllianceRule) -> ModelsRuleSet:
         self.alliance = value
         return self
 
-    def with_batch_size(self, value: int) -> ModelsRuleSet:
-        self.batch_size = value
+    def with_alliance_flexing_rule(
+        self, value: List[ModelsAllianceFlexingRule]
+    ) -> ModelsRuleSet:
+        self.alliance_flexing_rule = value
+        return self
+
+    def with_bucket_mmr_rule(self, value: ModelsBucketMMRRule) -> ModelsRuleSet:
+        self.bucket_mmr_rule = value
         return self
 
     def with_flexing_rule(self, value: List[ModelsFlexingRule]) -> ModelsRuleSet:
         self.flexing_rule = value
         return self
 
     def with_match_options(self, value: ModelsMatchOptionRule) -> ModelsRuleSet:
         self.match_options = value
         return self
 
     def with_matching_rule(self, value: List[ModelsMatchingRule]) -> ModelsRuleSet:
         self.matching_rule = value
         return self
 
-    def with_rebalance_enable(self, value: bool) -> ModelsRuleSet:
-        self.rebalance_enable = value
-        return self
-
     def with_sort_ticket(self, value: ModelsSortTicket) -> ModelsRuleSet:
         self.sort_ticket = value
         return self
 
     def with_sort_tickets(self, value: List[ModelsSortTicketRule]) -> ModelsRuleSet:
         self.sort_tickets = value
         return self
 
-    def with_ticket_flexing_selection(
-        self, value: Union[str, TicketFlexingSelectionEnum]
-    ) -> ModelsRuleSet:
-        self.ticket_flexing_selection = value
+    def with_sub_game_modes(self, value: Dict[str, ModelsSubGameMode]) -> ModelsRuleSet:
+        self.sub_game_modes = value
         return self
 
     def with_ticket_flexing_selections(
         self, value: List[ModelsSelectionRule]
     ) -> ModelsRuleSet:
         self.ticket_flexing_selections = value
         return self
 
-    def with_alliance_flexing_rule(
-        self, value: List[ModelsAllianceFlexingRule]
-    ) -> ModelsRuleSet:
-        self.alliance_flexing_rule = value
-        return self
-
-    def with_bucket_mmr_rule(self, value: ModelsBucketMMRRule) -> ModelsRuleSet:
-        self.bucket_mmr_rule = value
-        return self
-
-    def with_sub_game_modes(self, value: Dict[str, ModelsSubGameMode]) -> ModelsRuleSet:
-        self.sub_game_modes = value
-        return self
-
     def with_use_newest_ticket_for_flexing(self, value: bool) -> ModelsRuleSet:
         self.use_newest_ticket_for_flexing = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
+        if hasattr(self, "batch_size"):
+            result["batch_size"] = int(self.batch_size)
+        elif include_empty:
+            result["batch_size"] = 0
+        if hasattr(self, "rebalance_enable"):
+            result["rebalance_enable"] = bool(self.rebalance_enable)
+        elif include_empty:
+            result["rebalance_enable"] = False
+        if hasattr(self, "ticket_flexing_selection"):
+            result["ticket_flexing_selection"] = str(self.ticket_flexing_selection)
+        elif include_empty:
+            result["ticket_flexing_selection"] = ""
         if hasattr(self, "alliance"):
             result["alliance"] = self.alliance.to_dict(include_empty=include_empty)
         elif include_empty:
             result["alliance"] = ModelsAllianceRule()
-        if hasattr(self, "batch_size"):
-            result["batch_size"] = int(self.batch_size)
+        if hasattr(self, "alliance_flexing_rule"):
+            result["alliance_flexing_rule"] = [
+                i0.to_dict(include_empty=include_empty)
+                for i0 in self.alliance_flexing_rule
+            ]
         elif include_empty:
-            result["batch_size"] = 0
+            result["alliance_flexing_rule"] = []
+        if hasattr(self, "bucket_mmr_rule"):
+            result["bucket_mmr_rule"] = self.bucket_mmr_rule.to_dict(
+                include_empty=include_empty
+            )
+        elif include_empty:
+            result["bucket_mmr_rule"] = ModelsBucketMMRRule()
         if hasattr(self, "flexing_rule"):
             result["flexing_rule"] = [
                 i0.to_dict(include_empty=include_empty) for i0 in self.flexing_rule
             ]
         elif include_empty:
             result["flexing_rule"] = []
         if hasattr(self, "match_options"):
@@ -191,63 +202,40 @@
             result["match_options"] = ModelsMatchOptionRule()
         if hasattr(self, "matching_rule"):
             result["matching_rule"] = [
                 i0.to_dict(include_empty=include_empty) for i0 in self.matching_rule
             ]
         elif include_empty:
             result["matching_rule"] = []
-        if hasattr(self, "rebalance_enable"):
-            result["rebalance_enable"] = bool(self.rebalance_enable)
-        elif include_empty:
-            result["rebalance_enable"] = False
         if hasattr(self, "sort_ticket"):
             result["sort_ticket"] = self.sort_ticket.to_dict(
                 include_empty=include_empty
             )
         elif include_empty:
             result["sort_ticket"] = ModelsSortTicket()
         if hasattr(self, "sort_tickets"):
             result["sort_tickets"] = [
                 i0.to_dict(include_empty=include_empty) for i0 in self.sort_tickets
             ]
         elif include_empty:
             result["sort_tickets"] = []
-        if hasattr(self, "ticket_flexing_selection"):
-            result["ticket_flexing_selection"] = str(self.ticket_flexing_selection)
+        if hasattr(self, "sub_game_modes"):
+            result["sub_game_modes"] = {
+                str(k0): v0.to_dict(include_empty=include_empty)
+                for k0, v0 in self.sub_game_modes.items()
+            }
         elif include_empty:
-            result["ticket_flexing_selection"] = Union[
-                str, TicketFlexingSelectionEnum
-            ]()
+            result["sub_game_modes"] = {}
         if hasattr(self, "ticket_flexing_selections"):
             result["ticket_flexing_selections"] = [
                 i0.to_dict(include_empty=include_empty)
                 for i0 in self.ticket_flexing_selections
             ]
         elif include_empty:
             result["ticket_flexing_selections"] = []
-        if hasattr(self, "alliance_flexing_rule"):
-            result["alliance_flexing_rule"] = [
-                i0.to_dict(include_empty=include_empty)
-                for i0 in self.alliance_flexing_rule
-            ]
-        elif include_empty:
-            result["alliance_flexing_rule"] = []
-        if hasattr(self, "bucket_mmr_rule"):
-            result["bucket_mmr_rule"] = self.bucket_mmr_rule.to_dict(
-                include_empty=include_empty
-            )
-        elif include_empty:
-            result["bucket_mmr_rule"] = ModelsBucketMMRRule()
-        if hasattr(self, "sub_game_modes"):
-            result["sub_game_modes"] = {
-                str(k0): v0.to_dict(include_empty=include_empty)
-                for k0, v0 in self.sub_game_modes.items()
-            }
-        elif include_empty:
-            result["sub_game_modes"] = {}
         if hasattr(self, "use_newest_ticket_for_flexing"):
             result["use_newest_ticket_for_flexing"] = bool(
                 self.use_newest_ticket_for_flexing
             )
         elif include_empty:
             result["use_newest_ticket_for_flexing"] = False
         return result
@@ -255,68 +243,104 @@
     # endregion to methods
 
     # region static methods
 
     @classmethod
     def create(
         cls,
-        alliance: ModelsAllianceRule,
         batch_size: int,
-        flexing_rule: List[ModelsFlexingRule],
-        match_options: ModelsMatchOptionRule,
-        matching_rule: List[ModelsMatchingRule],
         rebalance_enable: bool,
-        sort_ticket: ModelsSortTicket,
-        sort_tickets: List[ModelsSortTicketRule],
-        ticket_flexing_selection: Union[str, TicketFlexingSelectionEnum],
-        ticket_flexing_selections: List[ModelsSelectionRule],
+        ticket_flexing_selection: str,
+        alliance: Optional[ModelsAllianceRule] = None,
         alliance_flexing_rule: Optional[List[ModelsAllianceFlexingRule]] = None,
         bucket_mmr_rule: Optional[ModelsBucketMMRRule] = None,
+        flexing_rule: Optional[List[ModelsFlexingRule]] = None,
+        match_options: Optional[ModelsMatchOptionRule] = None,
+        matching_rule: Optional[List[ModelsMatchingRule]] = None,
+        sort_ticket: Optional[ModelsSortTicket] = None,
+        sort_tickets: Optional[List[ModelsSortTicketRule]] = None,
         sub_game_modes: Optional[Dict[str, ModelsSubGameMode]] = None,
+        ticket_flexing_selections: Optional[List[ModelsSelectionRule]] = None,
         use_newest_ticket_for_flexing: Optional[bool] = None,
         **kwargs,
     ) -> ModelsRuleSet:
         instance = cls()
-        instance.alliance = alliance
         instance.batch_size = batch_size
-        instance.flexing_rule = flexing_rule
-        instance.match_options = match_options
-        instance.matching_rule = matching_rule
         instance.rebalance_enable = rebalance_enable
-        instance.sort_ticket = sort_ticket
-        instance.sort_tickets = sort_tickets
         instance.ticket_flexing_selection = ticket_flexing_selection
-        instance.ticket_flexing_selections = ticket_flexing_selections
+        if alliance is not None:
+            instance.alliance = alliance
         if alliance_flexing_rule is not None:
             instance.alliance_flexing_rule = alliance_flexing_rule
         if bucket_mmr_rule is not None:
             instance.bucket_mmr_rule = bucket_mmr_rule
+        if flexing_rule is not None:
+            instance.flexing_rule = flexing_rule
+        if match_options is not None:
+            instance.match_options = match_options
+        if matching_rule is not None:
+            instance.matching_rule = matching_rule
+        if sort_ticket is not None:
+            instance.sort_ticket = sort_ticket
+        if sort_tickets is not None:
+            instance.sort_tickets = sort_tickets
         if sub_game_modes is not None:
             instance.sub_game_modes = sub_game_modes
+        if ticket_flexing_selections is not None:
+            instance.ticket_flexing_selections = ticket_flexing_selections
         if use_newest_ticket_for_flexing is not None:
             instance.use_newest_ticket_for_flexing = use_newest_ticket_for_flexing
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
     ) -> ModelsRuleSet:
         instance = cls()
         if not dict_:
             return instance
+        if "batch_size" in dict_ and dict_["batch_size"] is not None:
+            instance.batch_size = int(dict_["batch_size"])
+        elif include_empty:
+            instance.batch_size = 0
+        if "rebalance_enable" in dict_ and dict_["rebalance_enable"] is not None:
+            instance.rebalance_enable = bool(dict_["rebalance_enable"])
+        elif include_empty:
+            instance.rebalance_enable = False
+        if (
+            "ticket_flexing_selection" in dict_
+            and dict_["ticket_flexing_selection"] is not None
+        ):
+            instance.ticket_flexing_selection = str(dict_["ticket_flexing_selection"])
+        elif include_empty:
+            instance.ticket_flexing_selection = ""
         if "alliance" in dict_ and dict_["alliance"] is not None:
             instance.alliance = ModelsAllianceRule.create_from_dict(
                 dict_["alliance"], include_empty=include_empty
             )
         elif include_empty:
             instance.alliance = ModelsAllianceRule()
-        if "batch_size" in dict_ and dict_["batch_size"] is not None:
-            instance.batch_size = int(dict_["batch_size"])
+        if (
+            "alliance_flexing_rule" in dict_
+            and dict_["alliance_flexing_rule"] is not None
+        ):
+            instance.alliance_flexing_rule = [
+                ModelsAllianceFlexingRule.create_from_dict(
+                    i0, include_empty=include_empty
+                )
+                for i0 in dict_["alliance_flexing_rule"]
+            ]
         elif include_empty:
-            instance.batch_size = 0
+            instance.alliance_flexing_rule = []
+        if "bucket_mmr_rule" in dict_ and dict_["bucket_mmr_rule"] is not None:
+            instance.bucket_mmr_rule = ModelsBucketMMRRule.create_from_dict(
+                dict_["bucket_mmr_rule"], include_empty=include_empty
+            )
+        elif include_empty:
+            instance.bucket_mmr_rule = ModelsBucketMMRRule()
         if "flexing_rule" in dict_ and dict_["flexing_rule"] is not None:
             instance.flexing_rule = [
                 ModelsFlexingRule.create_from_dict(i0, include_empty=include_empty)
                 for i0 in dict_["flexing_rule"]
             ]
         elif include_empty:
             instance.flexing_rule = []
@@ -329,76 +353,47 @@
         if "matching_rule" in dict_ and dict_["matching_rule"] is not None:
             instance.matching_rule = [
                 ModelsMatchingRule.create_from_dict(i0, include_empty=include_empty)
                 for i0 in dict_["matching_rule"]
             ]
         elif include_empty:
             instance.matching_rule = []
-        if "rebalance_enable" in dict_ and dict_["rebalance_enable"] is not None:
-            instance.rebalance_enable = bool(dict_["rebalance_enable"])
-        elif include_empty:
-            instance.rebalance_enable = False
         if "sort_ticket" in dict_ and dict_["sort_ticket"] is not None:
             instance.sort_ticket = ModelsSortTicket.create_from_dict(
                 dict_["sort_ticket"], include_empty=include_empty
             )
         elif include_empty:
             instance.sort_ticket = ModelsSortTicket()
         if "sort_tickets" in dict_ and dict_["sort_tickets"] is not None:
             instance.sort_tickets = [
                 ModelsSortTicketRule.create_from_dict(i0, include_empty=include_empty)
                 for i0 in dict_["sort_tickets"]
             ]
         elif include_empty:
             instance.sort_tickets = []
-        if (
-            "ticket_flexing_selection" in dict_
-            and dict_["ticket_flexing_selection"] is not None
-        ):
-            instance.ticket_flexing_selection = str(dict_["ticket_flexing_selection"])
+        if "sub_game_modes" in dict_ and dict_["sub_game_modes"] is not None:
+            instance.sub_game_modes = {
+                str(k0): ModelsSubGameMode.create_from_dict(
+                    v0, include_empty=include_empty
+                )
+                for k0, v0 in dict_["sub_game_modes"].items()
+            }
         elif include_empty:
-            instance.ticket_flexing_selection = Union[str, TicketFlexingSelectionEnum]()
+            instance.sub_game_modes = {}
         if (
             "ticket_flexing_selections" in dict_
             and dict_["ticket_flexing_selections"] is not None
         ):
             instance.ticket_flexing_selections = [
                 ModelsSelectionRule.create_from_dict(i0, include_empty=include_empty)
                 for i0 in dict_["ticket_flexing_selections"]
             ]
         elif include_empty:
             instance.ticket_flexing_selections = []
         if (
-            "alliance_flexing_rule" in dict_
-            and dict_["alliance_flexing_rule"] is not None
-        ):
-            instance.alliance_flexing_rule = [
-                ModelsAllianceFlexingRule.create_from_dict(
-                    i0, include_empty=include_empty
-                )
-                for i0 in dict_["alliance_flexing_rule"]
-            ]
-        elif include_empty:
-            instance.alliance_flexing_rule = []
-        if "bucket_mmr_rule" in dict_ and dict_["bucket_mmr_rule"] is not None:
-            instance.bucket_mmr_rule = ModelsBucketMMRRule.create_from_dict(
-                dict_["bucket_mmr_rule"], include_empty=include_empty
-            )
-        elif include_empty:
-            instance.bucket_mmr_rule = ModelsBucketMMRRule()
-        if "sub_game_modes" in dict_ and dict_["sub_game_modes"] is not None:
-            instance.sub_game_modes = {
-                str(k0): ModelsSubGameMode.create_from_dict(
-                    v0, include_empty=include_empty
-                )
-                for k0, v0 in dict_["sub_game_modes"].items()
-            }
-        elif include_empty:
-            instance.sub_game_modes = {}
-        if (
             "use_newest_ticket_for_flexing" in dict_
             and dict_["use_newest_ticket_for_flexing"] is not None
         ):
             instance.use_newest_ticket_for_flexing = bool(
                 dict_["use_newest_ticket_for_flexing"]
             )
         elif include_empty:
@@ -438,49 +433,43 @@
                 raise ValueError()
         else:
             return cls.create_from_dict(any_, include_empty=include_empty)
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
-            "alliance": "alliance",
             "batch_size": "batch_size",
+            "rebalance_enable": "rebalance_enable",
+            "ticket_flexing_selection": "ticket_flexing_selection",
+            "alliance": "alliance",
+            "alliance_flexing_rule": "alliance_flexing_rule",
+            "bucket_mmr_rule": "bucket_mmr_rule",
             "flexing_rule": "flexing_rule",
             "match_options": "match_options",
             "matching_rule": "matching_rule",
-            "rebalance_enable": "rebalance_enable",
             "sort_ticket": "sort_ticket",
             "sort_tickets": "sort_tickets",
-            "ticket_flexing_selection": "ticket_flexing_selection",
-            "ticket_flexing_selections": "ticket_flexing_selections",
-            "alliance_flexing_rule": "alliance_flexing_rule",
-            "bucket_mmr_rule": "bucket_mmr_rule",
             "sub_game_modes": "sub_game_modes",
+            "ticket_flexing_selections": "ticket_flexing_selections",
             "use_newest_ticket_for_flexing": "use_newest_ticket_for_flexing",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
-            "alliance": True,
             "batch_size": True,
-            "flexing_rule": True,
-            "match_options": True,
-            "matching_rule": True,
             "rebalance_enable": True,
-            "sort_ticket": True,
-            "sort_tickets": True,
             "ticket_flexing_selection": True,
-            "ticket_flexing_selections": True,
+            "alliance": False,
             "alliance_flexing_rule": False,
             "bucket_mmr_rule": False,
+            "flexing_rule": False,
+            "match_options": False,
+            "matching_rule": False,
+            "sort_ticket": False,
+            "sort_tickets": False,
             "sub_game_modes": False,
+            "ticket_flexing_selections": False,
             "use_newest_ticket_for_flexing": False,
         }
 
-    @staticmethod
-    def get_enum_map() -> Dict[str, List[Any]]:
-        return {
-            "ticket_flexing_selection": ["newest", "oldest", "pivot", "random"],
-        }
-
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_rule_set_v1.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_rule_set_v1.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,98 +22,98 @@
 # pylint: disable=too-many-statements
 # pylint: disable=unused-import
 
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Model
-from accelbyte_py_sdk.core import StrEnum
 
 from ..models.models_alliance_flexing_rule import ModelsAllianceFlexingRule
 from ..models.models_alliance_rule_v1 import ModelsAllianceRuleV1
 from ..models.models_bucket_mmr_rule import ModelsBucketMMRRule
 from ..models.models_flexing_rule import ModelsFlexingRule
 from ..models.models_match_option_rule import ModelsMatchOptionRule
 from ..models.models_matching_rule import ModelsMatchingRule
 from ..models.models_selection_rule import ModelsSelectionRule
 from ..models.models_sort_ticket import ModelsSortTicket
 from ..models.models_sort_ticket_rule import ModelsSortTicketRule
 from ..models.models_sub_game_mode import ModelsSubGameMode
 
 
-class TicketFlexingSelectionEnum(StrEnum):
-    NEWEST = "newest"
-    OLDEST = "oldest"
-    PIVOT = "pivot"
-    RANDOM = "random"
-
-
 class ModelsRuleSetV1(Model):
     """Models rule set V1 (models.RuleSetV1)
 
     Properties:
-        alliance: (alliance) REQUIRED ModelsAllianceRuleV1
+        batch_size: (batch_size) REQUIRED int
 
-        alliance_flexing_rule: (alliance_flexing_rule) REQUIRED List[ModelsAllianceFlexingRule]
+        ticket_flexing_selection: (ticket_flexing_selection) REQUIRED str
 
-        batch_size: (batch_size) REQUIRED int
+        alliance: (alliance) OPTIONAL ModelsAllianceRuleV1
 
-        flexing_rules: (flexingRules) REQUIRED List[ModelsFlexingRule]
+        alliance_flexing_rule: (alliance_flexing_rule) OPTIONAL List[ModelsAllianceFlexingRule]
 
-        match_options: (match_options) REQUIRED ModelsMatchOptionRule
+        bucket_mmr_rule: (bucket_mmr_rule) OPTIONAL ModelsBucketMMRRule
 
-        matching_rules: (matchingRules) REQUIRED List[ModelsMatchingRule]
+        flexing_rules: (flexingRules) OPTIONAL List[ModelsFlexingRule]
 
-        sort_ticket: (sort_ticket) REQUIRED ModelsSortTicket
+        match_options: (match_options) OPTIONAL ModelsMatchOptionRule
 
-        sort_tickets: (sort_tickets) REQUIRED List[ModelsSortTicketRule]
+        matching_rules: (matchingRules) OPTIONAL List[ModelsMatchingRule]
 
-        sub_game_modes: (sub_game_modes) REQUIRED Dict[str, ModelsSubGameMode]
+        sort_ticket: (sort_ticket) OPTIONAL ModelsSortTicket
 
-        ticket_flexing_selection: (ticket_flexing_selection) REQUIRED Union[str, TicketFlexingSelectionEnum]
+        sort_tickets: (sort_tickets) OPTIONAL List[ModelsSortTicketRule]
 
-        ticket_flexing_selections: (ticket_flexing_selections) REQUIRED List[ModelsSelectionRule]
+        sub_game_modes: (sub_game_modes) OPTIONAL Dict[str, ModelsSubGameMode]
 
-        bucket_mmr_rule: (bucket_mmr_rule) OPTIONAL ModelsBucketMMRRule
+        ticket_flexing_selections: (ticket_flexing_selections) OPTIONAL List[ModelsSelectionRule]
 
         use_newest_ticket_for_flexing: (use_newest_ticket_for_flexing) OPTIONAL bool
     """
 
     # region fields
 
-    alliance: ModelsAllianceRuleV1  # REQUIRED
-    alliance_flexing_rule: List[ModelsAllianceFlexingRule]  # REQUIRED
     batch_size: int  # REQUIRED
-    flexing_rules: List[ModelsFlexingRule]  # REQUIRED
-    match_options: ModelsMatchOptionRule  # REQUIRED
-    matching_rules: List[ModelsMatchingRule]  # REQUIRED
-    sort_ticket: ModelsSortTicket  # REQUIRED
-    sort_tickets: List[ModelsSortTicketRule]  # REQUIRED
-    sub_game_modes: Dict[str, ModelsSubGameMode]  # REQUIRED
-    ticket_flexing_selection: Union[str, TicketFlexingSelectionEnum]  # REQUIRED
-    ticket_flexing_selections: List[ModelsSelectionRule]  # REQUIRED
+    ticket_flexing_selection: str  # REQUIRED
+    alliance: ModelsAllianceRuleV1  # OPTIONAL
+    alliance_flexing_rule: List[ModelsAllianceFlexingRule]  # OPTIONAL
     bucket_mmr_rule: ModelsBucketMMRRule  # OPTIONAL
+    flexing_rules: List[ModelsFlexingRule]  # OPTIONAL
+    match_options: ModelsMatchOptionRule  # OPTIONAL
+    matching_rules: List[ModelsMatchingRule]  # OPTIONAL
+    sort_ticket: ModelsSortTicket  # OPTIONAL
+    sort_tickets: List[ModelsSortTicketRule]  # OPTIONAL
+    sub_game_modes: Dict[str, ModelsSubGameMode]  # OPTIONAL
+    ticket_flexing_selections: List[ModelsSelectionRule]  # OPTIONAL
     use_newest_ticket_for_flexing: bool  # OPTIONAL
 
     # endregion fields
 
     # region with_x methods
 
+    def with_batch_size(self, value: int) -> ModelsRuleSetV1:
+        self.batch_size = value
+        return self
+
+    def with_ticket_flexing_selection(self, value: str) -> ModelsRuleSetV1:
+        self.ticket_flexing_selection = value
+        return self
+
     def with_alliance(self, value: ModelsAllianceRuleV1) -> ModelsRuleSetV1:
         self.alliance = value
         return self
 
     def with_alliance_flexing_rule(
         self, value: List[ModelsAllianceFlexingRule]
     ) -> ModelsRuleSetV1:
         self.alliance_flexing_rule = value
         return self
 
-    def with_batch_size(self, value: int) -> ModelsRuleSetV1:
-        self.batch_size = value
+    def with_bucket_mmr_rule(self, value: ModelsBucketMMRRule) -> ModelsRuleSetV1:
+        self.bucket_mmr_rule = value
         return self
 
     def with_flexing_rules(self, value: List[ModelsFlexingRule]) -> ModelsRuleSetV1:
         self.flexing_rules = value
         return self
 
     def with_match_options(self, value: ModelsMatchOptionRule) -> ModelsRuleSetV1:
@@ -134,55 +134,55 @@
 
     def with_sub_game_modes(
         self, value: Dict[str, ModelsSubGameMode]
     ) -> ModelsRuleSetV1:
         self.sub_game_modes = value
         return self
 
-    def with_ticket_flexing_selection(
-        self, value: Union[str, TicketFlexingSelectionEnum]
-    ) -> ModelsRuleSetV1:
-        self.ticket_flexing_selection = value
-        return self
-
     def with_ticket_flexing_selections(
         self, value: List[ModelsSelectionRule]
     ) -> ModelsRuleSetV1:
         self.ticket_flexing_selections = value
         return self
 
-    def with_bucket_mmr_rule(self, value: ModelsBucketMMRRule) -> ModelsRuleSetV1:
-        self.bucket_mmr_rule = value
-        return self
-
     def with_use_newest_ticket_for_flexing(self, value: bool) -> ModelsRuleSetV1:
         self.use_newest_ticket_for_flexing = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
+        if hasattr(self, "batch_size"):
+            result["batch_size"] = int(self.batch_size)
+        elif include_empty:
+            result["batch_size"] = 0
+        if hasattr(self, "ticket_flexing_selection"):
+            result["ticket_flexing_selection"] = str(self.ticket_flexing_selection)
+        elif include_empty:
+            result["ticket_flexing_selection"] = ""
         if hasattr(self, "alliance"):
             result["alliance"] = self.alliance.to_dict(include_empty=include_empty)
         elif include_empty:
             result["alliance"] = ModelsAllianceRuleV1()
         if hasattr(self, "alliance_flexing_rule"):
             result["alliance_flexing_rule"] = [
                 i0.to_dict(include_empty=include_empty)
                 for i0 in self.alliance_flexing_rule
             ]
         elif include_empty:
             result["alliance_flexing_rule"] = []
-        if hasattr(self, "batch_size"):
-            result["batch_size"] = int(self.batch_size)
+        if hasattr(self, "bucket_mmr_rule"):
+            result["bucket_mmr_rule"] = self.bucket_mmr_rule.to_dict(
+                include_empty=include_empty
+            )
         elif include_empty:
-            result["batch_size"] = 0
+            result["bucket_mmr_rule"] = ModelsBucketMMRRule()
         if hasattr(self, "flexing_rules"):
             result["flexingRules"] = [
                 i0.to_dict(include_empty=include_empty) for i0 in self.flexing_rules
             ]
         elif include_empty:
             result["flexingRules"] = []
         if hasattr(self, "match_options"):
@@ -212,33 +212,21 @@
         if hasattr(self, "sub_game_modes"):
             result["sub_game_modes"] = {
                 str(k0): v0.to_dict(include_empty=include_empty)
                 for k0, v0 in self.sub_game_modes.items()
             }
         elif include_empty:
             result["sub_game_modes"] = {}
-        if hasattr(self, "ticket_flexing_selection"):
-            result["ticket_flexing_selection"] = str(self.ticket_flexing_selection)
-        elif include_empty:
-            result["ticket_flexing_selection"] = Union[
-                str, TicketFlexingSelectionEnum
-            ]()
         if hasattr(self, "ticket_flexing_selections"):
             result["ticket_flexing_selections"] = [
                 i0.to_dict(include_empty=include_empty)
                 for i0 in self.ticket_flexing_selections
             ]
         elif include_empty:
             result["ticket_flexing_selections"] = []
-        if hasattr(self, "bucket_mmr_rule"):
-            result["bucket_mmr_rule"] = self.bucket_mmr_rule.to_dict(
-                include_empty=include_empty
-            )
-        elif include_empty:
-            result["bucket_mmr_rule"] = ModelsBucketMMRRule()
         if hasattr(self, "use_newest_ticket_for_flexing"):
             result["use_newest_ticket_for_flexing"] = bool(
                 self.use_newest_ticket_for_flexing
             )
         elif include_empty:
             result["use_newest_ticket_for_flexing"] = False
         return result
@@ -246,54 +234,74 @@
     # endregion to methods
 
     # region static methods
 
     @classmethod
     def create(
         cls,
-        alliance: ModelsAllianceRuleV1,
-        alliance_flexing_rule: List[ModelsAllianceFlexingRule],
         batch_size: int,
-        flexing_rules: List[ModelsFlexingRule],
-        match_options: ModelsMatchOptionRule,
-        matching_rules: List[ModelsMatchingRule],
-        sort_ticket: ModelsSortTicket,
-        sort_tickets: List[ModelsSortTicketRule],
-        sub_game_modes: Dict[str, ModelsSubGameMode],
-        ticket_flexing_selection: Union[str, TicketFlexingSelectionEnum],
-        ticket_flexing_selections: List[ModelsSelectionRule],
+        ticket_flexing_selection: str,
+        alliance: Optional[ModelsAllianceRuleV1] = None,
+        alliance_flexing_rule: Optional[List[ModelsAllianceFlexingRule]] = None,
         bucket_mmr_rule: Optional[ModelsBucketMMRRule] = None,
+        flexing_rules: Optional[List[ModelsFlexingRule]] = None,
+        match_options: Optional[ModelsMatchOptionRule] = None,
+        matching_rules: Optional[List[ModelsMatchingRule]] = None,
+        sort_ticket: Optional[ModelsSortTicket] = None,
+        sort_tickets: Optional[List[ModelsSortTicketRule]] = None,
+        sub_game_modes: Optional[Dict[str, ModelsSubGameMode]] = None,
+        ticket_flexing_selections: Optional[List[ModelsSelectionRule]] = None,
         use_newest_ticket_for_flexing: Optional[bool] = None,
         **kwargs,
     ) -> ModelsRuleSetV1:
         instance = cls()
-        instance.alliance = alliance
-        instance.alliance_flexing_rule = alliance_flexing_rule
         instance.batch_size = batch_size
-        instance.flexing_rules = flexing_rules
-        instance.match_options = match_options
-        instance.matching_rules = matching_rules
-        instance.sort_ticket = sort_ticket
-        instance.sort_tickets = sort_tickets
-        instance.sub_game_modes = sub_game_modes
         instance.ticket_flexing_selection = ticket_flexing_selection
-        instance.ticket_flexing_selections = ticket_flexing_selections
+        if alliance is not None:
+            instance.alliance = alliance
+        if alliance_flexing_rule is not None:
+            instance.alliance_flexing_rule = alliance_flexing_rule
         if bucket_mmr_rule is not None:
             instance.bucket_mmr_rule = bucket_mmr_rule
+        if flexing_rules is not None:
+            instance.flexing_rules = flexing_rules
+        if match_options is not None:
+            instance.match_options = match_options
+        if matching_rules is not None:
+            instance.matching_rules = matching_rules
+        if sort_ticket is not None:
+            instance.sort_ticket = sort_ticket
+        if sort_tickets is not None:
+            instance.sort_tickets = sort_tickets
+        if sub_game_modes is not None:
+            instance.sub_game_modes = sub_game_modes
+        if ticket_flexing_selections is not None:
+            instance.ticket_flexing_selections = ticket_flexing_selections
         if use_newest_ticket_for_flexing is not None:
             instance.use_newest_ticket_for_flexing = use_newest_ticket_for_flexing
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
     ) -> ModelsRuleSetV1:
         instance = cls()
         if not dict_:
             return instance
+        if "batch_size" in dict_ and dict_["batch_size"] is not None:
+            instance.batch_size = int(dict_["batch_size"])
+        elif include_empty:
+            instance.batch_size = 0
+        if (
+            "ticket_flexing_selection" in dict_
+            and dict_["ticket_flexing_selection"] is not None
+        ):
+            instance.ticket_flexing_selection = str(dict_["ticket_flexing_selection"])
+        elif include_empty:
+            instance.ticket_flexing_selection = ""
         if "alliance" in dict_ and dict_["alliance"] is not None:
             instance.alliance = ModelsAllianceRuleV1.create_from_dict(
                 dict_["alliance"], include_empty=include_empty
             )
         elif include_empty:
             instance.alliance = ModelsAllianceRuleV1()
         if (
@@ -304,18 +312,20 @@
                 ModelsAllianceFlexingRule.create_from_dict(
                     i0, include_empty=include_empty
                 )
                 for i0 in dict_["alliance_flexing_rule"]
             ]
         elif include_empty:
             instance.alliance_flexing_rule = []
-        if "batch_size" in dict_ and dict_["batch_size"] is not None:
-            instance.batch_size = int(dict_["batch_size"])
+        if "bucket_mmr_rule" in dict_ and dict_["bucket_mmr_rule"] is not None:
+            instance.bucket_mmr_rule = ModelsBucketMMRRule.create_from_dict(
+                dict_["bucket_mmr_rule"], include_empty=include_empty
+            )
         elif include_empty:
-            instance.batch_size = 0
+            instance.bucket_mmr_rule = ModelsBucketMMRRule()
         if "flexingRules" in dict_ and dict_["flexingRules"] is not None:
             instance.flexing_rules = [
                 ModelsFlexingRule.create_from_dict(i0, include_empty=include_empty)
                 for i0 in dict_["flexingRules"]
             ]
         elif include_empty:
             instance.flexing_rules = []
@@ -351,36 +361,23 @@
                     v0, include_empty=include_empty
                 )
                 for k0, v0 in dict_["sub_game_modes"].items()
             }
         elif include_empty:
             instance.sub_game_modes = {}
         if (
-            "ticket_flexing_selection" in dict_
-            and dict_["ticket_flexing_selection"] is not None
-        ):
-            instance.ticket_flexing_selection = str(dict_["ticket_flexing_selection"])
-        elif include_empty:
-            instance.ticket_flexing_selection = Union[str, TicketFlexingSelectionEnum]()
-        if (
             "ticket_flexing_selections" in dict_
             and dict_["ticket_flexing_selections"] is not None
         ):
             instance.ticket_flexing_selections = [
                 ModelsSelectionRule.create_from_dict(i0, include_empty=include_empty)
                 for i0 in dict_["ticket_flexing_selections"]
             ]
         elif include_empty:
             instance.ticket_flexing_selections = []
-        if "bucket_mmr_rule" in dict_ and dict_["bucket_mmr_rule"] is not None:
-            instance.bucket_mmr_rule = ModelsBucketMMRRule.create_from_dict(
-                dict_["bucket_mmr_rule"], include_empty=include_empty
-            )
-        elif include_empty:
-            instance.bucket_mmr_rule = ModelsBucketMMRRule()
         if (
             "use_newest_ticket_for_flexing" in dict_
             and dict_["use_newest_ticket_for_flexing"] is not None
         ):
             instance.use_newest_ticket_for_flexing = bool(
                 dict_["use_newest_ticket_for_flexing"]
             )
@@ -421,47 +418,41 @@
                 raise ValueError()
         else:
             return cls.create_from_dict(any_, include_empty=include_empty)
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
+            "batch_size": "batch_size",
+            "ticket_flexing_selection": "ticket_flexing_selection",
             "alliance": "alliance",
             "alliance_flexing_rule": "alliance_flexing_rule",
-            "batch_size": "batch_size",
+            "bucket_mmr_rule": "bucket_mmr_rule",
             "flexingRules": "flexing_rules",
             "match_options": "match_options",
             "matchingRules": "matching_rules",
             "sort_ticket": "sort_ticket",
             "sort_tickets": "sort_tickets",
             "sub_game_modes": "sub_game_modes",
-            "ticket_flexing_selection": "ticket_flexing_selection",
             "ticket_flexing_selections": "ticket_flexing_selections",
-            "bucket_mmr_rule": "bucket_mmr_rule",
             "use_newest_ticket_for_flexing": "use_newest_ticket_for_flexing",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
-            "alliance": True,
-            "alliance_flexing_rule": True,
             "batch_size": True,
-            "flexingRules": True,
-            "match_options": True,
-            "matchingRules": True,
-            "sort_ticket": True,
-            "sort_tickets": True,
-            "sub_game_modes": True,
             "ticket_flexing_selection": True,
-            "ticket_flexing_selections": True,
+            "alliance": False,
+            "alliance_flexing_rule": False,
             "bucket_mmr_rule": False,
+            "flexingRules": False,
+            "match_options": False,
+            "matchingRules": False,
+            "sort_ticket": False,
+            "sort_tickets": False,
+            "sub_game_modes": False,
+            "ticket_flexing_selections": False,
             "use_newest_ticket_for_flexing": False,
         }
 
-    @staticmethod
-    def get_enum_map() -> Dict[str, List[Any]]:
-        return {
-            "ticket_flexing_selection": ["newest", "oldest", "pivot", "random"],
-        }
-
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_selection_rule.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_selection_rule.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,43 +22,35 @@
 # pylint: disable=too-many-statements
 # pylint: disable=unused-import
 
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Model
-from accelbyte_py_sdk.core import StrEnum
-
-
-class SelectionEnum(StrEnum):
-    NEWEST = "newest"
-    OLDEST = "oldest"
-    PIVOT = "pivot"
-    RANDOM = "random"
 
 
 class ModelsSelectionRule(Model):
     """Models selection rule (models.SelectionRule)
 
     Properties:
-        selection: (selection) REQUIRED Union[str, SelectionEnum]
+        selection: (selection) REQUIRED str
 
         threshold: (threshold) REQUIRED int
     """
 
     # region fields
 
-    selection: Union[str, SelectionEnum]  # REQUIRED
+    selection: str  # REQUIRED
     threshold: int  # REQUIRED
 
     # endregion fields
 
     # region with_x methods
 
-    def with_selection(self, value: Union[str, SelectionEnum]) -> ModelsSelectionRule:
+    def with_selection(self, value: str) -> ModelsSelectionRule:
         self.selection = value
         return self
 
     def with_threshold(self, value: int) -> ModelsSelectionRule:
         self.threshold = value
         return self
 
@@ -67,29 +59,27 @@
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
         if hasattr(self, "selection"):
             result["selection"] = str(self.selection)
         elif include_empty:
-            result["selection"] = Union[str, SelectionEnum]()
+            result["selection"] = ""
         if hasattr(self, "threshold"):
             result["threshold"] = int(self.threshold)
         elif include_empty:
             result["threshold"] = 0
         return result
 
     # endregion to methods
 
     # region static methods
 
     @classmethod
-    def create(
-        cls, selection: Union[str, SelectionEnum], threshold: int, **kwargs
-    ) -> ModelsSelectionRule:
+    def create(cls, selection: str, threshold: int, **kwargs) -> ModelsSelectionRule:
         instance = cls()
         instance.selection = selection
         instance.threshold = threshold
         return instance
 
     @classmethod
     def create_from_dict(
@@ -97,15 +87,15 @@
     ) -> ModelsSelectionRule:
         instance = cls()
         if not dict_:
             return instance
         if "selection" in dict_ and dict_["selection"] is not None:
             instance.selection = str(dict_["selection"])
         elif include_empty:
-            instance.selection = Union[str, SelectionEnum]()
+            instance.selection = ""
         if "threshold" in dict_ and dict_["threshold"] is not None:
             instance.threshold = int(dict_["threshold"])
         elif include_empty:
             instance.threshold = 0
         return instance
 
     @classmethod
@@ -154,14 +144,8 @@
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
             "selection": True,
             "threshold": True,
         }
 
-    @staticmethod
-    def get_enum_map() -> Dict[str, List[Any]]:
-        return {
-            "selection": ["newest", "oldest", "pivot", "random"],
-        }
-
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_sort_ticket.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_sort_ticket_rule.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,171 +22,152 @@
 # pylint: disable=too-many-statements
 # pylint: disable=unused-import
 
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Model
-from accelbyte_py_sdk.core import StrEnum
 
 
-class SearchResultEnum(StrEnum):
-    DISTANCE = "distance"
-    LARGESTPARTYSIZE = "largestPartySize"
-    NONE = "none"
-    OLDESTTICKETAGE = "oldestTicketAge"
-    RANDOM = "random"
-
-
-class TicketQueueEnum(StrEnum):
-    DISTANCE = "distance"
-    LARGESTPARTYSIZE = "largestPartySize"
-    NONE = "none"
-    OLDESTTICKETAGE = "oldestTicketAge"
-    RANDOM = "random"
-
-
-class ModelsSortTicket(Model):
-    """Models sort ticket (models.SortTicket)
+class ModelsSortTicketRule(Model):
+    """Models sort ticket rule (models.SortTicketRule)
 
     Properties:
-        search_result: (search_result) REQUIRED Union[str, SearchResultEnum]
+        search_result: (search_result) REQUIRED str
 
-        ticket_queue: (ticket_queue) REQUIRED Union[str, TicketQueueEnum]
+        threshold: (threshold) REQUIRED int
+
+        ticket_queue: (ticket_queue) REQUIRED str
     """
 
     # region fields
 
-    search_result: Union[str, SearchResultEnum]  # REQUIRED
-    ticket_queue: Union[str, TicketQueueEnum]  # REQUIRED
+    search_result: str  # REQUIRED
+    threshold: int  # REQUIRED
+    ticket_queue: str  # REQUIRED
 
     # endregion fields
 
     # region with_x methods
 
-    def with_search_result(
-        self, value: Union[str, SearchResultEnum]
-    ) -> ModelsSortTicket:
+    def with_search_result(self, value: str) -> ModelsSortTicketRule:
         self.search_result = value
         return self
 
-    def with_ticket_queue(self, value: Union[str, TicketQueueEnum]) -> ModelsSortTicket:
+    def with_threshold(self, value: int) -> ModelsSortTicketRule:
+        self.threshold = value
+        return self
+
+    def with_ticket_queue(self, value: str) -> ModelsSortTicketRule:
         self.ticket_queue = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
         if hasattr(self, "search_result"):
             result["search_result"] = str(self.search_result)
         elif include_empty:
-            result["search_result"] = Union[str, SearchResultEnum]()
+            result["search_result"] = ""
+        if hasattr(self, "threshold"):
+            result["threshold"] = int(self.threshold)
+        elif include_empty:
+            result["threshold"] = 0
         if hasattr(self, "ticket_queue"):
             result["ticket_queue"] = str(self.ticket_queue)
         elif include_empty:
-            result["ticket_queue"] = Union[str, TicketQueueEnum]()
+            result["ticket_queue"] = ""
         return result
 
     # endregion to methods
 
     # region static methods
 
     @classmethod
     def create(
-        cls,
-        search_result: Union[str, SearchResultEnum],
-        ticket_queue: Union[str, TicketQueueEnum],
-        **kwargs,
-    ) -> ModelsSortTicket:
+        cls, search_result: str, threshold: int, ticket_queue: str, **kwargs
+    ) -> ModelsSortTicketRule:
         instance = cls()
         instance.search_result = search_result
+        instance.threshold = threshold
         instance.ticket_queue = ticket_queue
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> ModelsSortTicket:
+    ) -> ModelsSortTicketRule:
         instance = cls()
         if not dict_:
             return instance
         if "search_result" in dict_ and dict_["search_result"] is not None:
             instance.search_result = str(dict_["search_result"])
         elif include_empty:
-            instance.search_result = Union[str, SearchResultEnum]()
+            instance.search_result = ""
+        if "threshold" in dict_ and dict_["threshold"] is not None:
+            instance.threshold = int(dict_["threshold"])
+        elif include_empty:
+            instance.threshold = 0
         if "ticket_queue" in dict_ and dict_["ticket_queue"] is not None:
             instance.ticket_queue = str(dict_["ticket_queue"])
         elif include_empty:
-            instance.ticket_queue = Union[str, TicketQueueEnum]()
+            instance.ticket_queue = ""
         return instance
 
     @classmethod
     def create_many_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> Dict[str, ModelsSortTicket]:
+    ) -> Dict[str, ModelsSortTicketRule]:
         return (
             {k: cls.create_from_dict(v, include_empty=include_empty) for k, v in dict_}
             if dict_
             else {}
         )
 
     @classmethod
     def create_many_from_list(
         cls, list_: list, include_empty: bool = False
-    ) -> List[ModelsSortTicket]:
+    ) -> List[ModelsSortTicketRule]:
         return (
             [cls.create_from_dict(i, include_empty=include_empty) for i in list_]
             if list_
             else []
         )
 
     @classmethod
     def create_from_any(
         cls, any_: any, include_empty: bool = False, many: bool = False
-    ) -> Union[ModelsSortTicket, List[ModelsSortTicket], Dict[Any, ModelsSortTicket]]:
+    ) -> Union[
+        ModelsSortTicketRule,
+        List[ModelsSortTicketRule],
+        Dict[Any, ModelsSortTicketRule],
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
             "search_result": "search_result",
+            "threshold": "threshold",
             "ticket_queue": "ticket_queue",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
             "search_result": True,
+            "threshold": True,
             "ticket_queue": True,
         }
 
-    @staticmethod
-    def get_enum_map() -> Dict[str, List[Any]]:
-        return {
-            "search_result": [
-                "distance",
-                "largestPartySize",
-                "none",
-                "oldestTicketAge",
-                "random",
-            ],
-            "ticket_queue": [
-                "distance",
-                "largestPartySize",
-                "none",
-                "oldestTicketAge",
-                "random",
-            ],
-        }
-
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_sort_ticket_rule.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_update_player_playtime_weight_response.py`

 * *Files 26% similar despite different names*

```diff
@@ -22,196 +22,152 @@
 # pylint: disable=too-many-statements
 # pylint: disable=unused-import
 
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Model
-from accelbyte_py_sdk.core import StrEnum
 
 
-class SearchResultEnum(StrEnum):
-    DISTANCE = "distance"
-    LARGESTPARTYSIZE = "largestPartySize"
-    NONE = "none"
-    OLDESTTICKETAGE = "oldestTicketAge"
-    RANDOM = "random"
-
-
-class TicketQueueEnum(StrEnum):
-    DISTANCE = "distance"
-    LARGESTPARTYSIZE = "largestPartySize"
-    NONE = "none"
-    OLDESTTICKETAGE = "oldestTicketAge"
-    RANDOM = "random"
-
-
-class ModelsSortTicketRule(Model):
-    """Models sort ticket rule (models.SortTicketRule)
+class ModelsUpdatePlayerPlaytimeWeightResponse(Model):
+    """Models update player playtime weight response (models.UpdatePlayerPlaytimeWeightResponse)
 
     Properties:
-        search_result: (search_result) REQUIRED Union[str, SearchResultEnum]
+        playtime: (playtime) REQUIRED str
 
-        threshold: (threshold) REQUIRED int
+        user_id: (userID) REQUIRED str
 
-        ticket_queue: (ticket_queue) REQUIRED Union[str, TicketQueueEnum]
+        weight: (weight) REQUIRED float
     """
 
     # region fields
 
-    search_result: Union[str, SearchResultEnum]  # REQUIRED
-    threshold: int  # REQUIRED
-    ticket_queue: Union[str, TicketQueueEnum]  # REQUIRED
+    playtime: str  # REQUIRED
+    user_id: str  # REQUIRED
+    weight: float  # REQUIRED
 
     # endregion fields
 
     # region with_x methods
 
-    def with_search_result(
-        self, value: Union[str, SearchResultEnum]
-    ) -> ModelsSortTicketRule:
-        self.search_result = value
+    def with_playtime(self, value: str) -> ModelsUpdatePlayerPlaytimeWeightResponse:
+        self.playtime = value
         return self
 
-    def with_threshold(self, value: int) -> ModelsSortTicketRule:
-        self.threshold = value
+    def with_user_id(self, value: str) -> ModelsUpdatePlayerPlaytimeWeightResponse:
+        self.user_id = value
         return self
 
-    def with_ticket_queue(
-        self, value: Union[str, TicketQueueEnum]
-    ) -> ModelsSortTicketRule:
-        self.ticket_queue = value
+    def with_weight(self, value: float) -> ModelsUpdatePlayerPlaytimeWeightResponse:
+        self.weight = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
-        if hasattr(self, "search_result"):
-            result["search_result"] = str(self.search_result)
+        if hasattr(self, "playtime"):
+            result["playtime"] = str(self.playtime)
         elif include_empty:
-            result["search_result"] = Union[str, SearchResultEnum]()
-        if hasattr(self, "threshold"):
-            result["threshold"] = int(self.threshold)
-        elif include_empty:
-            result["threshold"] = 0
-        if hasattr(self, "ticket_queue"):
-            result["ticket_queue"] = str(self.ticket_queue)
+            result["playtime"] = ""
+        if hasattr(self, "user_id"):
+            result["userID"] = str(self.user_id)
+        elif include_empty:
+            result["userID"] = ""
+        if hasattr(self, "weight"):
+            result["weight"] = float(self.weight)
         elif include_empty:
-            result["ticket_queue"] = Union[str, TicketQueueEnum]()
+            result["weight"] = 0.0
         return result
 
     # endregion to methods
 
     # region static methods
 
     @classmethod
     def create(
-        cls,
-        search_result: Union[str, SearchResultEnum],
-        threshold: int,
-        ticket_queue: Union[str, TicketQueueEnum],
-        **kwargs,
-    ) -> ModelsSortTicketRule:
+        cls, playtime: str, user_id: str, weight: float, **kwargs
+    ) -> ModelsUpdatePlayerPlaytimeWeightResponse:
         instance = cls()
-        instance.search_result = search_result
-        instance.threshold = threshold
-        instance.ticket_queue = ticket_queue
+        instance.playtime = playtime
+        instance.user_id = user_id
+        instance.weight = weight
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> ModelsSortTicketRule:
+    ) -> ModelsUpdatePlayerPlaytimeWeightResponse:
         instance = cls()
         if not dict_:
             return instance
-        if "search_result" in dict_ and dict_["search_result"] is not None:
-            instance.search_result = str(dict_["search_result"])
+        if "playtime" in dict_ and dict_["playtime"] is not None:
+            instance.playtime = str(dict_["playtime"])
         elif include_empty:
-            instance.search_result = Union[str, SearchResultEnum]()
-        if "threshold" in dict_ and dict_["threshold"] is not None:
-            instance.threshold = int(dict_["threshold"])
-        elif include_empty:
-            instance.threshold = 0
-        if "ticket_queue" in dict_ and dict_["ticket_queue"] is not None:
-            instance.ticket_queue = str(dict_["ticket_queue"])
+            instance.playtime = ""
+        if "userID" in dict_ and dict_["userID"] is not None:
+            instance.user_id = str(dict_["userID"])
+        elif include_empty:
+            instance.user_id = ""
+        if "weight" in dict_ and dict_["weight"] is not None:
+            instance.weight = float(dict_["weight"])
         elif include_empty:
-            instance.ticket_queue = Union[str, TicketQueueEnum]()
+            instance.weight = 0.0
         return instance
 
     @classmethod
     def create_many_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> Dict[str, ModelsSortTicketRule]:
+    ) -> Dict[str, ModelsUpdatePlayerPlaytimeWeightResponse]:
         return (
             {k: cls.create_from_dict(v, include_empty=include_empty) for k, v in dict_}
             if dict_
             else {}
         )
 
     @classmethod
     def create_many_from_list(
         cls, list_: list, include_empty: bool = False
-    ) -> List[ModelsSortTicketRule]:
+    ) -> List[ModelsUpdatePlayerPlaytimeWeightResponse]:
         return (
             [cls.create_from_dict(i, include_empty=include_empty) for i in list_]
             if list_
             else []
         )
 
     @classmethod
     def create_from_any(
         cls, any_: any, include_empty: bool = False, many: bool = False
     ) -> Union[
-        ModelsSortTicketRule,
-        List[ModelsSortTicketRule],
-        Dict[Any, ModelsSortTicketRule],
+        ModelsUpdatePlayerPlaytimeWeightResponse,
+        List[ModelsUpdatePlayerPlaytimeWeightResponse],
+        Dict[Any, ModelsUpdatePlayerPlaytimeWeightResponse],
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
-            "search_result": "search_result",
-            "threshold": "threshold",
-            "ticket_queue": "ticket_queue",
+            "playtime": "playtime",
+            "userID": "user_id",
+            "weight": "weight",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
-            "search_result": True,
-            "threshold": True,
-            "ticket_queue": True,
-        }
-
-    @staticmethod
-    def get_enum_map() -> Dict[str, List[Any]]:
-        return {
-            "search_result": [
-                "distance",
-                "largestPartySize",
-                "none",
-                "oldestTicketAge",
-                "random",
-            ],
-            "ticket_queue": [
-                "distance",
-                "largestPartySize",
-                "none",
-                "oldestTicketAge",
-                "random",
-            ],
+            "playtime": True,
+            "userID": True,
+            "weight": True,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_stat_resume_response.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_stat_resume_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_sub_game_mode.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_sub_game_mode.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,82 +33,83 @@
 
 class ModelsSubGameMode(Model):
     """Models sub game mode (models.SubGameMode)
 
     Properties:
         alliance: (alliance) REQUIRED ModelsAllianceRule
 
-        alliance_flexing_rule: (alliance_flexing_rule) REQUIRED List[ModelsAllianceFlexingRule]
-
         name: (name) REQUIRED str
+
+        alliance_flexing_rule: (alliance_flexing_rule) OPTIONAL List[ModelsAllianceFlexingRule]
     """
 
     # region fields
 
     alliance: ModelsAllianceRule  # REQUIRED
-    alliance_flexing_rule: List[ModelsAllianceFlexingRule]  # REQUIRED
     name: str  # REQUIRED
+    alliance_flexing_rule: List[ModelsAllianceFlexingRule]  # OPTIONAL
 
     # endregion fields
 
     # region with_x methods
 
     def with_alliance(self, value: ModelsAllianceRule) -> ModelsSubGameMode:
         self.alliance = value
         return self
 
+    def with_name(self, value: str) -> ModelsSubGameMode:
+        self.name = value
+        return self
+
     def with_alliance_flexing_rule(
         self, value: List[ModelsAllianceFlexingRule]
     ) -> ModelsSubGameMode:
         self.alliance_flexing_rule = value
         return self
 
-    def with_name(self, value: str) -> ModelsSubGameMode:
-        self.name = value
-        return self
-
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
         if hasattr(self, "alliance"):
             result["alliance"] = self.alliance.to_dict(include_empty=include_empty)
         elif include_empty:
             result["alliance"] = ModelsAllianceRule()
+        if hasattr(self, "name"):
+            result["name"] = str(self.name)
+        elif include_empty:
+            result["name"] = ""
         if hasattr(self, "alliance_flexing_rule"):
             result["alliance_flexing_rule"] = [
                 i0.to_dict(include_empty=include_empty)
                 for i0 in self.alliance_flexing_rule
             ]
         elif include_empty:
             result["alliance_flexing_rule"] = []
-        if hasattr(self, "name"):
-            result["name"] = str(self.name)
-        elif include_empty:
-            result["name"] = ""
         return result
 
     # endregion to methods
 
     # region static methods
 
     @classmethod
     def create(
         cls,
         alliance: ModelsAllianceRule,
-        alliance_flexing_rule: List[ModelsAllianceFlexingRule],
         name: str,
+        alliance_flexing_rule: Optional[List[ModelsAllianceFlexingRule]] = None,
         **kwargs,
     ) -> ModelsSubGameMode:
         instance = cls()
         instance.alliance = alliance
-        instance.alliance_flexing_rule = alliance_flexing_rule
         instance.name = name
+        if alliance_flexing_rule is not None:
+            instance.alliance_flexing_rule = alliance_flexing_rule
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
     ) -> ModelsSubGameMode:
         instance = cls()
@@ -116,30 +117,30 @@
             return instance
         if "alliance" in dict_ and dict_["alliance"] is not None:
             instance.alliance = ModelsAllianceRule.create_from_dict(
                 dict_["alliance"], include_empty=include_empty
             )
         elif include_empty:
             instance.alliance = ModelsAllianceRule()
+        if "name" in dict_ and dict_["name"] is not None:
+            instance.name = str(dict_["name"])
+        elif include_empty:
+            instance.name = ""
         if (
             "alliance_flexing_rule" in dict_
             and dict_["alliance_flexing_rule"] is not None
         ):
             instance.alliance_flexing_rule = [
                 ModelsAllianceFlexingRule.create_from_dict(
                     i0, include_empty=include_empty
                 )
                 for i0 in dict_["alliance_flexing_rule"]
             ]
         elif include_empty:
             instance.alliance_flexing_rule = []
-        if "name" in dict_ and dict_["name"] is not None:
-            instance.name = str(dict_["name"])
-        elif include_empty:
-            instance.name = ""
         return instance
 
     @classmethod
     def create_many_from_dict(
         cls, dict_: dict, include_empty: bool = False
     ) -> Dict[str, ModelsSubGameMode]:
         return (
@@ -174,20 +175,20 @@
         else:
             return cls.create_from_dict(any_, include_empty=include_empty)
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
             "alliance": "alliance",
-            "alliance_flexing_rule": "alliance_flexing_rule",
             "name": "name",
+            "alliance_flexing_rule": "alliance_flexing_rule",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
             "alliance": True,
-            "alliance_flexing_rule": True,
             "name": True,
+            "alliance_flexing_rule": False,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_ticket_metric_result_record.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_ticket_metric_result_record.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_update_alliance_rule.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_update_alliance_rule.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_update_channel_request.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_update_channel_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_update_play_time_weight_request.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_update_play_time_weight_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_update_player_playtime_weight_response.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/service_get_session_history_search_response.py`

 * *Files 22% similar despite different names*

```diff
@@ -23,151 +23,154 @@
 # pylint: disable=unused-import
 
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Model
 
+from ..models.models_pagination import ModelsPagination
+from ..models.service_get_session_history_search_response_item import (
+    ServiceGetSessionHistorySearchResponseItem,
+)
 
-class ModelsUpdatePlayerPlaytimeWeightResponse(Model):
-    """Models update player playtime weight response (models.UpdatePlayerPlaytimeWeightResponse)
 
-    Properties:
-        playtime: (playtime) REQUIRED str
+class ServiceGetSessionHistorySearchResponse(Model):
+    """Service get session history search response (service.GetSessionHistorySearchResponse)
 
-        user_id: (userID) REQUIRED str
+    Properties:
+        data: (data) REQUIRED List[ServiceGetSessionHistorySearchResponseItem]
 
-        weight: (weight) REQUIRED float
+        pagination: (pagination) REQUIRED ModelsPagination
     """
 
     # region fields
 
-    playtime: str  # REQUIRED
-    user_id: str  # REQUIRED
-    weight: float  # REQUIRED
+    data: List[ServiceGetSessionHistorySearchResponseItem]  # REQUIRED
+    pagination: ModelsPagination  # REQUIRED
 
     # endregion fields
 
     # region with_x methods
 
-    def with_playtime(self, value: str) -> ModelsUpdatePlayerPlaytimeWeightResponse:
-        self.playtime = value
-        return self
-
-    def with_user_id(self, value: str) -> ModelsUpdatePlayerPlaytimeWeightResponse:
-        self.user_id = value
+    def with_data(
+        self, value: List[ServiceGetSessionHistorySearchResponseItem]
+    ) -> ServiceGetSessionHistorySearchResponse:
+        self.data = value
         return self
 
-    def with_weight(self, value: float) -> ModelsUpdatePlayerPlaytimeWeightResponse:
-        self.weight = value
+    def with_pagination(
+        self, value: ModelsPagination
+    ) -> ServiceGetSessionHistorySearchResponse:
+        self.pagination = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
-        if hasattr(self, "playtime"):
-            result["playtime"] = str(self.playtime)
+        if hasattr(self, "data"):
+            result["data"] = [
+                i0.to_dict(include_empty=include_empty) for i0 in self.data
+            ]
+        elif include_empty:
+            result["data"] = []
+        if hasattr(self, "pagination"):
+            result["pagination"] = self.pagination.to_dict(include_empty=include_empty)
         elif include_empty:
-            result["playtime"] = ""
-        if hasattr(self, "user_id"):
-            result["userID"] = str(self.user_id)
-        elif include_empty:
-            result["userID"] = ""
-        if hasattr(self, "weight"):
-            result["weight"] = float(self.weight)
-        elif include_empty:
-            result["weight"] = 0.0
+            result["pagination"] = ModelsPagination()
         return result
 
     # endregion to methods
 
     # region static methods
 
     @classmethod
     def create(
-        cls, playtime: str, user_id: str, weight: float, **kwargs
-    ) -> ModelsUpdatePlayerPlaytimeWeightResponse:
+        cls,
+        data: List[ServiceGetSessionHistorySearchResponseItem],
+        pagination: ModelsPagination,
+        **kwargs,
+    ) -> ServiceGetSessionHistorySearchResponse:
         instance = cls()
-        instance.playtime = playtime
-        instance.user_id = user_id
-        instance.weight = weight
+        instance.data = data
+        instance.pagination = pagination
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> ModelsUpdatePlayerPlaytimeWeightResponse:
+    ) -> ServiceGetSessionHistorySearchResponse:
         instance = cls()
         if not dict_:
             return instance
-        if "playtime" in dict_ and dict_["playtime"] is not None:
-            instance.playtime = str(dict_["playtime"])
-        elif include_empty:
-            instance.playtime = ""
-        if "userID" in dict_ and dict_["userID"] is not None:
-            instance.user_id = str(dict_["userID"])
-        elif include_empty:
-            instance.user_id = ""
-        if "weight" in dict_ and dict_["weight"] is not None:
-            instance.weight = float(dict_["weight"])
+        if "data" in dict_ and dict_["data"] is not None:
+            instance.data = [
+                ServiceGetSessionHistorySearchResponseItem.create_from_dict(
+                    i0, include_empty=include_empty
+                )
+                for i0 in dict_["data"]
+            ]
+        elif include_empty:
+            instance.data = []
+        if "pagination" in dict_ and dict_["pagination"] is not None:
+            instance.pagination = ModelsPagination.create_from_dict(
+                dict_["pagination"], include_empty=include_empty
+            )
         elif include_empty:
-            instance.weight = 0.0
+            instance.pagination = ModelsPagination()
         return instance
 
     @classmethod
     def create_many_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> Dict[str, ModelsUpdatePlayerPlaytimeWeightResponse]:
+    ) -> Dict[str, ServiceGetSessionHistorySearchResponse]:
         return (
             {k: cls.create_from_dict(v, include_empty=include_empty) for k, v in dict_}
             if dict_
             else {}
         )
 
     @classmethod
     def create_many_from_list(
         cls, list_: list, include_empty: bool = False
-    ) -> List[ModelsUpdatePlayerPlaytimeWeightResponse]:
+    ) -> List[ServiceGetSessionHistorySearchResponse]:
         return (
             [cls.create_from_dict(i, include_empty=include_empty) for i in list_]
             if list_
             else []
         )
 
     @classmethod
     def create_from_any(
         cls, any_: any, include_empty: bool = False, many: bool = False
     ) -> Union[
-        ModelsUpdatePlayerPlaytimeWeightResponse,
-        List[ModelsUpdatePlayerPlaytimeWeightResponse],
-        Dict[Any, ModelsUpdatePlayerPlaytimeWeightResponse],
+        ServiceGetSessionHistorySearchResponse,
+        List[ServiceGetSessionHistorySearchResponse],
+        Dict[Any, ServiceGetSessionHistorySearchResponse],
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
-            "playtime": "playtime",
-            "userID": "user_id",
-            "weight": "weight",
+            "data": "data",
+            "pagination": "pagination",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
-            "playtime": True,
-            "userID": True,
-            "weight": True,
+            "data": True,
+            "pagination": True,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_update_ruleset.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_update_ruleset.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 # pylint: disable=too-many-statements
 # pylint: disable=unused-import
 
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Model
-from accelbyte_py_sdk.core import StrEnum
 
 from ..models.models_alliance_flexing_rule import ModelsAllianceFlexingRule
 from ..models.models_bucket_mmr_rule import ModelsBucketMMRRule
 from ..models.models_flexing_rule import ModelsFlexingRule
 from ..models.models_match_option_rule import ModelsMatchOptionRule
 from ..models.models_matching_rule import ModelsMatchingRule
 from ..models.models_selection_rule import ModelsSelectionRule
@@ -38,36 +37,29 @@
 from ..models.models_sort_ticket_rule import ModelsSortTicketRule
 from ..models.models_update_alliance_rule import ModelsUpdateAllianceRule
 from ..models.models_update_ruleset_sub_game_modes import (
     ModelsUpdateRulesetSubGameModes,
 )
 
 
-class TicketFlexingSelectionEnum(StrEnum):
-    NEWEST = "newest"
-    OLDEST = "oldest"
-    PIVOT = "pivot"
-    RANDOM = "random"
-
-
 class ModelsUpdateRuleset(Model):
     """Models update ruleset (models.UpdateRuleset)
 
     Properties:
         alliance: (alliance) REQUIRED ModelsUpdateAllianceRule
 
         alliance_flexing_rule: (alliance_flexing_rule) REQUIRED List[ModelsAllianceFlexingRule]
 
         batch_size: (batch_size) REQUIRED int
 
         sort_ticket: (sort_ticket) REQUIRED ModelsSortTicket
 
         sort_tickets: (sort_tickets) REQUIRED List[ModelsSortTicketRule]
 
-        ticket_flexing_selection: (ticket_flexing_selection) REQUIRED Union[str, TicketFlexingSelectionEnum]
+        ticket_flexing_selection: (ticket_flexing_selection) REQUIRED str
 
         ticket_flexing_selections: (ticket_flexing_selections) REQUIRED List[ModelsSelectionRule]
 
         bucket_mmr_rule: (bucket_mmr_rule) OPTIONAL ModelsBucketMMRRule
 
         flexing_rules: (flexingRules) OPTIONAL List[ModelsFlexingRule]
 
@@ -83,15 +75,15 @@
     # region fields
 
     alliance: ModelsUpdateAllianceRule  # REQUIRED
     alliance_flexing_rule: List[ModelsAllianceFlexingRule]  # REQUIRED
     batch_size: int  # REQUIRED
     sort_ticket: ModelsSortTicket  # REQUIRED
     sort_tickets: List[ModelsSortTicketRule]  # REQUIRED
-    ticket_flexing_selection: Union[str, TicketFlexingSelectionEnum]  # REQUIRED
+    ticket_flexing_selection: str  # REQUIRED
     ticket_flexing_selections: List[ModelsSelectionRule]  # REQUIRED
     bucket_mmr_rule: ModelsBucketMMRRule  # OPTIONAL
     flexing_rules: List[ModelsFlexingRule]  # OPTIONAL
     match_options: ModelsMatchOptionRule  # OPTIONAL
     matching_rules: List[ModelsMatchingRule]  # OPTIONAL
     sub_game_modes: ModelsUpdateRulesetSubGameModes  # OPTIONAL
     use_newest_ticket_for_flexing: bool  # OPTIONAL
@@ -120,17 +112,15 @@
 
     def with_sort_tickets(
         self, value: List[ModelsSortTicketRule]
     ) -> ModelsUpdateRuleset:
         self.sort_tickets = value
         return self
 
-    def with_ticket_flexing_selection(
-        self, value: Union[str, TicketFlexingSelectionEnum]
-    ) -> ModelsUpdateRuleset:
+    def with_ticket_flexing_selection(self, value: str) -> ModelsUpdateRuleset:
         self.ticket_flexing_selection = value
         return self
 
     def with_ticket_flexing_selections(
         self, value: List[ModelsSelectionRule]
     ) -> ModelsUpdateRuleset:
         self.ticket_flexing_selections = value
@@ -196,17 +186,15 @@
                 i0.to_dict(include_empty=include_empty) for i0 in self.sort_tickets
             ]
         elif include_empty:
             result["sort_tickets"] = []
         if hasattr(self, "ticket_flexing_selection"):
             result["ticket_flexing_selection"] = str(self.ticket_flexing_selection)
         elif include_empty:
-            result["ticket_flexing_selection"] = Union[
-                str, TicketFlexingSelectionEnum
-            ]()
+            result["ticket_flexing_selection"] = ""
         if hasattr(self, "ticket_flexing_selections"):
             result["ticket_flexing_selections"] = [
                 i0.to_dict(include_empty=include_empty)
                 for i0 in self.ticket_flexing_selections
             ]
         elif include_empty:
             result["ticket_flexing_selections"] = []
@@ -256,15 +244,15 @@
     def create(
         cls,
         alliance: ModelsUpdateAllianceRule,
         alliance_flexing_rule: List[ModelsAllianceFlexingRule],
         batch_size: int,
         sort_ticket: ModelsSortTicket,
         sort_tickets: List[ModelsSortTicketRule],
-        ticket_flexing_selection: Union[str, TicketFlexingSelectionEnum],
+        ticket_flexing_selection: str,
         ticket_flexing_selections: List[ModelsSelectionRule],
         bucket_mmr_rule: Optional[ModelsBucketMMRRule] = None,
         flexing_rules: Optional[List[ModelsFlexingRule]] = None,
         match_options: Optional[ModelsMatchOptionRule] = None,
         matching_rules: Optional[List[ModelsMatchingRule]] = None,
         sub_game_modes: Optional[ModelsUpdateRulesetSubGameModes] = None,
         use_newest_ticket_for_flexing: Optional[bool] = None,
@@ -336,15 +324,15 @@
             instance.sort_tickets = []
         if (
             "ticket_flexing_selection" in dict_
             and dict_["ticket_flexing_selection"] is not None
         ):
             instance.ticket_flexing_selection = str(dict_["ticket_flexing_selection"])
         elif include_empty:
-            instance.ticket_flexing_selection = Union[str, TicketFlexingSelectionEnum]()
+            instance.ticket_flexing_selection = ""
         if (
             "ticket_flexing_selections" in dict_
             and dict_["ticket_flexing_selections"] is not None
         ):
             instance.ticket_flexing_selections = [
                 ModelsSelectionRule.create_from_dict(i0, include_empty=include_empty)
                 for i0 in dict_["ticket_flexing_selections"]
@@ -462,14 +450,8 @@
             "flexingRules": False,
             "match_options": False,
             "matchingRules": False,
             "sub_game_modes": False,
             "use_newest_ticket_for_flexing": False,
         }
 
-    @staticmethod
-    def get_enum_map() -> Dict[str, List[Any]]:
-        return {
-            "ticket_flexing_selection": ["newest", "oldest", "pivot", "random"],
-        }
-
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/models_update_ruleset_sub_game_modes.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/models_update_ruleset_sub_game_modes.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/response_error.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/response_error.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/response_error_v1.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/response_error_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/service_get_session_history_detailed_response_item.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/service_get_session_history_detailed_response_item.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/service_get_session_history_search_response.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/service_get_session_history_search_response_v2.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,46 +24,46 @@
 
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Model
 
 from ..models.models_pagination import ModelsPagination
-from ..models.service_get_session_history_search_response_item import (
-    ServiceGetSessionHistorySearchResponseItem,
+from ..models.service_get_session_history_search_response_item_v2 import (
+    ServiceGetSessionHistorySearchResponseItemV2,
 )
 
 
-class ServiceGetSessionHistorySearchResponse(Model):
-    """Service get session history search response (service.GetSessionHistorySearchResponse)
+class ServiceGetSessionHistorySearchResponseV2(Model):
+    """Service get session history search response V2 (service.GetSessionHistorySearchResponseV2)
 
     Properties:
-        data: (data) REQUIRED List[ServiceGetSessionHistorySearchResponseItem]
+        data: (data) REQUIRED List[ServiceGetSessionHistorySearchResponseItemV2]
 
         pagination: (pagination) REQUIRED ModelsPagination
     """
 
     # region fields
 
-    data: List[ServiceGetSessionHistorySearchResponseItem]  # REQUIRED
+    data: List[ServiceGetSessionHistorySearchResponseItemV2]  # REQUIRED
     pagination: ModelsPagination  # REQUIRED
 
     # endregion fields
 
     # region with_x methods
 
     def with_data(
-        self, value: List[ServiceGetSessionHistorySearchResponseItem]
-    ) -> ServiceGetSessionHistorySearchResponse:
+        self, value: List[ServiceGetSessionHistorySearchResponseItemV2]
+    ) -> ServiceGetSessionHistorySearchResponseV2:
         self.data = value
         return self
 
     def with_pagination(
         self, value: ModelsPagination
-    ) -> ServiceGetSessionHistorySearchResponse:
+    ) -> ServiceGetSessionHistorySearchResponseV2:
         self.pagination = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
@@ -84,33 +84,33 @@
     # endregion to methods
 
     # region static methods
 
     @classmethod
     def create(
         cls,
-        data: List[ServiceGetSessionHistorySearchResponseItem],
+        data: List[ServiceGetSessionHistorySearchResponseItemV2],
         pagination: ModelsPagination,
         **kwargs,
-    ) -> ServiceGetSessionHistorySearchResponse:
+    ) -> ServiceGetSessionHistorySearchResponseV2:
         instance = cls()
         instance.data = data
         instance.pagination = pagination
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> ServiceGetSessionHistorySearchResponse:
+    ) -> ServiceGetSessionHistorySearchResponseV2:
         instance = cls()
         if not dict_:
             return instance
         if "data" in dict_ and dict_["data"] is not None:
             instance.data = [
-                ServiceGetSessionHistorySearchResponseItem.create_from_dict(
+                ServiceGetSessionHistorySearchResponseItemV2.create_from_dict(
                     i0, include_empty=include_empty
                 )
                 for i0 in dict_["data"]
             ]
         elif include_empty:
             instance.data = []
         if "pagination" in dict_ and dict_["pagination"] is not None:
@@ -120,38 +120,38 @@
         elif include_empty:
             instance.pagination = ModelsPagination()
         return instance
 
     @classmethod
     def create_many_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> Dict[str, ServiceGetSessionHistorySearchResponse]:
+    ) -> Dict[str, ServiceGetSessionHistorySearchResponseV2]:
         return (
             {k: cls.create_from_dict(v, include_empty=include_empty) for k, v in dict_}
             if dict_
             else {}
         )
 
     @classmethod
     def create_many_from_list(
         cls, list_: list, include_empty: bool = False
-    ) -> List[ServiceGetSessionHistorySearchResponse]:
+    ) -> List[ServiceGetSessionHistorySearchResponseV2]:
         return (
             [cls.create_from_dict(i, include_empty=include_empty) for i in list_]
             if list_
             else []
         )
 
     @classmethod
     def create_from_any(
         cls, any_: any, include_empty: bool = False, many: bool = False
     ) -> Union[
-        ServiceGetSessionHistorySearchResponse,
-        List[ServiceGetSessionHistorySearchResponse],
-        Dict[Any, ServiceGetSessionHistorySearchResponse],
+        ServiceGetSessionHistorySearchResponseV2,
+        List[ServiceGetSessionHistorySearchResponseV2],
+        Dict[Any, ServiceGetSessionHistorySearchResponseV2],
     ]:
         if many:
             if isinstance(any_, dict):
                 return cls.create_many_from_dict(any_, include_empty=include_empty)
             elif isinstance(any_, list):
                 return cls.create_many_from_list(any_, include_empty=include_empty)
             else:
```

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/service_get_session_history_search_response_item.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/service_get_session_history_search_response_item.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/models/service_get_session_history_search_response_item_v2.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/models/service_get_session_history_search_response_item_v2.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/__init__.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Matchmaking Service."""
 
-__version__ = "2.30.1"
+__version__ = "2.30.2"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .add_user_into_session_i_3d8cc3 import AddUserIntoSessionInChannel
 from .bulk_get_sessions import BulkGetSessions
```

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/add_user_into_session_i_3d8cc3.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/add_user_into_session_i_3d8cc3.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/bulk_get_sessions.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/bulk_get_sessions.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/create_channel_handler.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/create_channel_handler.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/delete_channel_handler.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/delete_channel_handler.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/delete_session_in_channel.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/delete_session_in_channel.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/delete_user_from_sessio_8c8e34.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/delete_user_from_sessio_8c8e34.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/dequeue_session_handler.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/dequeue_session_handler.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/export_channels.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/export_channels.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/get_all_channels_handler.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/get_all_channels_handler.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/get_all_party_in_all_channel.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/get_all_party_in_all_channel.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/get_all_party_in_channel.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/get_all_party_in_channel.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/get_all_sessions_in_channel.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/get_all_sessions_in_channel.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/get_match_pool_metric.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/get_match_pool_metric.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/get_session_history_detailed.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/get_session_history_detailed.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/get_single_matchmaking_channel.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/get_single_matchmaking_channel.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/get_stat_data.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/get_stat_data.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/import_channels.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/import_channels.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/public_get_all_matchmak_cd6d3e.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/public_get_all_matchmak_cd6d3e.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/public_get_single_match_188a61.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/public_get_single_match_188a61.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/query_session_handler.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/query_session_handler.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/queue_session_handler.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/queue_session_handler.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/rebalance.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/rebalance.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/search_sessions.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/search_sessions.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/search_sessions_v2.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/search_sessions_v2.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/store_match_results.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/store_match_results.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/update_matchmaking_channel.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking/update_matchmaking_channel.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking_operations/__init__.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking_operations/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Matchmaking Service."""
 
-__version__ = "2.30.1"
+__version__ = "2.30.2"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .get_healthcheck_info import GetHealthcheckInfo
 from .handler_v3_healthz import HandlerV3Healthz
```

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking_operations/get_healthcheck_info.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking_operations/get_healthcheck_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking_operations/handler_v3_healthz.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking_operations/handler_v3_healthz.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking_operations/public_get_messages.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking_operations/public_get_messages.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking_operations/version_check_handler.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/matchmaking_operations/version_check_handler.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/mock_matchmaking/__init__.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/mock_matchmaking/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Matchmaking Service."""
 
-__version__ = "2.30.1"
+__version__ = "2.30.2"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .bulk_create_mock_tickets import BulkCreateMockTickets
 from .clean_all_mocks import CleanAllMocks
```

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/mock_matchmaking/bulk_create_mock_tickets.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/mock_matchmaking/bulk_create_mock_tickets.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/mock_matchmaking/clean_all_mocks.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/mock_matchmaking/clean_all_mocks.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/mock_matchmaking/create_mock_tickets.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/mock_matchmaking/create_mock_tickets.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/mock_matchmaking/get_all_mock_matches.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/mock_matchmaking/get_all_mock_matches.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/mock_matchmaking/get_all_mock_tickets.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/mock_matchmaking/get_all_mock_tickets.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/mock_matchmaking/get_mock_matches_by_timestamp.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/mock_matchmaking/get_mock_matches_by_timestamp.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/mock_matchmaking/get_mock_tickets_by_timestamp.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/mock_matchmaking/get_mock_tickets_by_timestamp.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/social_matchmaking/__init__.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/social_matchmaking/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,14 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Matchmaking Service."""
 
-__version__ = "2.30.1"
+__version__ = "2.30.2"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .update_play_time_weight import UpdatePlayTimeWeight
```

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/operations/social_matchmaking/update_play_time_weight.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/operations/social_matchmaking/update_play_time_weight.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/wrappers/__init__.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/wrappers/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: wrapper-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Matchmaking Service."""
 
-__version__ = "2.30.1"
+__version__ = "2.30.2"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from ._matchmaking import add_user_into_session_in_channel
 from ._matchmaking import add_user_into_session_in_channel_async
```

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/wrappers/_matchmaking.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/wrappers/_matchmaking.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/wrappers/_matchmaking_operations.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/wrappers/_matchmaking_operations.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/wrappers/_mock_matchmaking.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/wrappers/_mock_matchmaking.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk/api/matchmaking/wrappers/_social_matchmaking.py` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk/api/matchmaking/wrappers/_social_matchmaking.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk_service_matchmaking.egg-info/PKG-INFO` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk_service_matchmaking.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: accelbyte-py-sdk-service-matchmaking
-Version: 0.8.0
+Version: 0.9.0
 Summary: AccelByte Python SDK - AccelByte Gaming Services Matchmaking Service
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: accelbyte-py-sdk-core
 
 [//]: # (Code generated. DO NOT EDIT!)
 
 # AccelByte Modular Python SDK - Service Module
 
 This is a service module for the [AccelByte Modular Python SDK](https://github.com/AccelByte/accelbyte-python-modular-sdk) package.
 
 ```text
 AccelByte Gaming Services Matchmaking Service
-* Version: 2.30.1
+* Version: 2.30.2
 ```
 
 ## Setup
 
 This SDK requires Python 3.9 to be installed.
 
 ### Install with Pip
```

### Comparing `accelbyte-py-sdk-service-matchmaking-0.8.0/accelbyte_py_sdk_service_matchmaking.egg-info/SOURCES.txt` & `accelbyte-py-sdk-service-matchmaking-0.9.0/accelbyte_py_sdk_service_matchmaking.egg-info/SOURCES.txt`

 * *Files identical despite different names*

