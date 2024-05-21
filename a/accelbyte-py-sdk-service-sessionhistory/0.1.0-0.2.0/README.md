# Comparing `tmp/accelbyte_py_sdk_service_sessionhistory-0.1.0.tar.gz` & `tmp/accelbyte_py_sdk_service_sessionhistory-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accelbyte_py_sdk_service_sessionhistory-0.1.0.tar", last modified: Tue May  7 06:30:36 2024, max compression
+gzip compressed data, was "accelbyte_py_sdk_service_sessionhistory-0.2.0.tar", last modified: Tue May 21 03:49:53 2024, max compression
```

## Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0.tar` & `accelbyte_py_sdk_service_sessionhistory-0.2.0.tar`

### file list

```diff
@@ -1,135 +1,141 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:30:36.473449 accelbyte_py_sdk_service_sessionhistory-0.1.0/
--rw-r--r--   0 root         (0) root         (0)     1154 2024-05-07 06:30:36.473449 accelbyte_py_sdk_service_sessionhistory-0.1.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      887 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:30:36.461449 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:30:36.461449 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:30:36.465449 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/
--rw-rw-r--   0 root         (0) root         (0)     3899 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:30:36.469449 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/
--rw-rw-r--   0 root         (0) root         (0)     6169 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7391 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_acquiring_ds.py
--rw-rw-r--   0 root         (0) root         (0)     6156 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_acquiring_ds_wait_time.py
--rw-rw-r--   0 root         (0) root         (0)     6223 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_canceled_matchmaking_ticket.py
--rw-rw-r--   0 root         (0) root         (0)     6209 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_created_matchmaking_ticket.py
--rw-rw-r--   0 root         (0) root         (0)     9448 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_event_match_history.py
--rw-rw-r--   0 root         (0) root         (0)     6209 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_expired_matchmaking_ticket.py
--rw-rw-r--   0 root         (0) root         (0)     7142 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_game_session_detail.py
--rw-rw-r--   0 root         (0) root         (0)     5343 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_game_session_detail_query_response.py
--rw-rw-r--   0 root         (0) root         (0)     7145 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_history.py
--rw-rw-r--   0 root         (0) root         (0)     6155 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_match_length_duration.py
--rw-rw-r--   0 root         (0) root         (0)     6096 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_match_matchmaking.py
--rw-rw-r--   0 root         (0) root         (0)     6181 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_match_matchmaking_ticket.py
--rw-rw-r--   0 root         (0) root         (0)    10590 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_matchmaking_detail.py
--rw-rw-r--   0 root         (0) root         (0)     5341 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_matchmaking_detail_query_response.py
--rw-rw-r--   0 root         (0) root         (0)     9860 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_matchmaking_history.py
--rw-rw-r--   0 root         (0) root         (0)     5500 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_pagination.py
--rw-rw-r--   0 root         (0) root         (0)     7199 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_party_detail.py
--rw-rw-r--   0 root         (0) root         (0)     5164 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_party_detail_query_response.py
--rw-rw-r--   0 root         (0) root         (0)     7197 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_party_history.py
--rw-rw-r--   0 root         (0) root         (0)     5347 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_ticket_detail_query_response.py
--rw-rw-r--   0 root         (0) root         (0)    18058 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_ticket_observability_detail.py
--rw-rw-r--   0 root         (0) root         (0)     9318 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_ticket_observability_history.py
--rw-rw-r--   0 root         (0) root         (0)     6049 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_total_active_session.py
--rw-rw-r--   0 root         (0) root         (0)     6859 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_total_player_persession.py
--rw-rw-r--   0 root         (0) root         (0)     4290 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_acquiring_ds_query_response.py
--rw-rw-r--   0 root         (0) root         (0)     4476 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_acquiring_ds_wait_time_query_response.py
--rw-rw-r--   0 root         (0) root         (0)     4591 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_canceled_matchmaking_ticket_query_response.py
--rw-rw-r--   0 root         (0) root         (0)     4573 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_created_matchmaking_ticket_query_response.py
--rw-rw-r--   0 root         (0) root         (0)     4573 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_expired_matchmaking_ticket_query_response.py
--rw-rw-r--   0 root         (0) root         (0)     5320 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_match_histor_query_response.py
--rw-rw-r--   0 root         (0) root         (0)     4474 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_match_length_duration_query_response.py
--rw-rw-r--   0 root         (0) root         (0)     4418 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_match_matchmaking_query_response.py
--rw-rw-r--   0 root         (0) root         (0)     4528 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_match_matchmaking_ticket_query_response.py
--rw-rw-r--   0 root         (0) root         (0)     4428 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_match_pool_pod_tick_match_response.py
--rw-rw-r--   0 root         (0) root         (0)     5458 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_match_pool_pod_tick_query_response.py
--rw-rw-r--   0 root         (0) root         (0)    12957 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_match_pool_pod_tick_result.py
--rw-rw-r--   0 root         (0) root         (0)     4344 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_match_pool_pod_tick_ticket_response.py
--rw-rw-r--   0 root         (0) root         (0)     4365 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_match_pool_query_response.py
--rw-rw-r--   0 root         (0) root         (0)     3875 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_match_pool_result.py
--rw-rw-r--   0 root         (0) root         (0)     6517 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_match_ticket_history.py
--rw-rw-r--   0 root         (0) root         (0)     4495 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_match_ticket_history_query_response.py
--rw-rw-r--   0 root         (0) root         (0)     4379 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_matches_query_response.py
--rw-rw-r--   0 root         (0) root         (0)    11450 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_ticket_matches_result.py
--rw-rw-r--   0 root         (0) root         (0)     5253 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_ticket_query_response.py
--rw-rw-r--   0 root         (0) root         (0)     7827 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_ticket_result.py
--rw-rw-r--   0 root         (0) root         (0)     4456 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_total_active_session_query_response.py
--rw-rw-r--   0 root         (0) root         (0)     4544 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_total_player_persession_avg_query_response.py
--rw-rw-r--   0 root         (0) root         (0)     6169 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/models_alliance_rule.py
--rw-rw-r--   0 root         (0) root         (0)     9433 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/models_backfill_proposal.py
--rw-rw-r--   0 root         (0) root         (0)     8250 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/models_backfill_ticket.py
--rw-rw-r--   0 root         (0) root         (0)     6239 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/models_ds_information.py
--rw-rw-r--   0 root         (0) root         (0)    15892 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/models_game_server.py
--rw-rw-r--   0 root         (0) root         (0)    20141 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/models_game_session.py
--rw-rw-r--   0 root         (0) root         (0)     4982 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/models_game_session_team.py
--rw-rw-r--   0 root         (0) root         (0)     9178 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/models_match.py
--rw-rw-r--   0 root         (0) root         (0)     4293 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/models_matching_ally.py
--rw-rw-r--   0 root         (0) root         (0)     7584 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/models_matching_party.py
--rw-rw-r--   0 root         (0) root         (0)     5107 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/models_matching_rule.py
--rw-rw-r--   0 root         (0) root         (0)    17838 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/models_matchmaking_result.py
--rw-rw-r--   0 root         (0) root         (0)    14610 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/models_party.py
--rw-rw-r--   0 root         (0) root         (0)     4767 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/models_party_member.py
--rw-rw-r--   0 root         (0) root         (0)     4596 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/models_party_members.py
--rw-rw-r--   0 root         (0) root         (0)     4546 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/models_party_team.py
--rw-rw-r--   0 root         (0) root         (0)     6153 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/models_player_data.py
--rw-rw-r--   0 root         (0) root         (0)     5388 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/models_proposed_proposal.py
--rw-rw-r--   0 root         (0) root         (0)    11656 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/models_session_config.py
--rw-rw-r--   0 root         (0) root         (0)    11929 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/models_session_configuration.py
--rw-rw-r--   0 root         (0) root         (0)     4782 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/models_team.py
--rw-rw-r--   0 root         (0) root         (0)    10979 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/models_ticket.py
--rw-rw-r--   0 root         (0) root         (0)    20462 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/models_ticket_data.py
--rw-rw-r--   0 root         (0) root         (0)     4070 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/models_ticket_observability.py
--rw-rw-r--   0 root         (0) root         (0)     4588 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/models_ticket_status.py
--rw-rw-r--   0 root         (0) root         (0)     7310 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/models_user.py
--rw-rw-r--   0 root         (0) root         (0)     6536 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/response_error.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:30:36.469449 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/operations/
--rw-rw-r--   0 root         (0) root         (0)      443 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/operations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:30:36.469449 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/operations/game_session_detail/
--rw-rw-r--   0 root         (0) root         (0)     1081 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/operations/game_session_detail/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7732 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/operations/game_session_detail/admin_get_matchmaking_d_8811e8.py
--rw-rw-r--   0 root         (0) root         (0)     7738 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/operations/game_session_detail/admin_get_matchmaking_d_98288e.py
--rw-rw-r--   0 root         (0) root         (0)    11975 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/operations/game_session_detail/admin_query_game_sessio_2eed0b.py
--rw-rw-r--   0 root         (0) root         (0)    12822 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/operations/game_session_detail/admin_query_matchmaking_detail.py
--rw-rw-r--   0 root         (0) root         (0)    11637 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/operations/game_session_detail/admin_query_party_detail.py
--rw-rw-r--   0 root         (0) root         (0)    14222 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/operations/game_session_detail/admin_query_ticket_detail.py
--rw-rw-r--   0 root         (0) root         (0)     7691 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/operations/game_session_detail/admin_ticket_detail_get_8ac60d.py
--rw-rw-r--   0 root         (0) root         (0)     7790 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/operations/game_session_detail/get_game_session_detail.py
--rw-rw-r--   0 root         (0) root         (0)     7654 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/operations/game_session_detail/get_party_detail.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:30:36.469449 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/operations/operations/
--rw-rw-r--   0 root         (0) root         (0)      587 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/operations/operations/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4437 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/operations/operations/get_healthcheck_info.py
--rw-rw-r--   0 root         (0) root         (0)     4493 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/operations/operations/get_healthcheck_info_v1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:30:36.473449 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/
--rw-rw-r--   0 root         (0) root         (0)     1825 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8740 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_acquiring_ds.py
--rw-rw-r--   0 root         (0) root         (0)     8926 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_acquiring_ds_wait_a2982b.py
--rw-rw-r--   0 root         (0) root         (0)     9610 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_detail_tick_match_d45948.py
--rw-rw-r--   0 root         (0) root         (0)     9606 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_detail_tick_match_f9b8b2.py
--rw-rw-r--   0 root         (0) root         (0)    12741 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_detail_tick_match_pool.py
--rw-rw-r--   0 root         (0) root         (0)     9472 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_match_histories.py
--rw-rw-r--   0 root         (0) root         (0)     8920 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_match_length_dura_0e6d44.py
--rw-rw-r--   0 root         (0) root         (0)     8913 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_match_length_durationp99.py
--rw-rw-r--   0 root         (0) root         (0)     7942 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_match_ticket_histories.py
--rw-rw-r--   0 root         (0) root         (0)     9656 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_total_active_session.py
--rw-rw-r--   0 root         (0) root         (0)     9867 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_total_matchmaking_0ba5f3.py
--rw-rw-r--   0 root         (0) root         (0)     9873 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_total_matchmaking_49d09d.py
--rw-rw-r--   0 root         (0) root         (0)     9855 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_total_matchmaking_73a209.py
--rw-rw-r--   0 root         (0) root         (0)     9855 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_total_matchmaking_adaa30.py
--rw-rw-r--   0 root         (0) root         (0)     9748 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_total_matchmaking_match.py
--rw-rw-r--   0 root         (0) root         (0)     8971 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_total_player_persession.py
--rw-rw-r--   0 root         (0) root         (0)     7757 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_xray_match.py
--rw-rw-r--   0 root         (0) root         (0)     9493 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_xray_match_pool.py
--rw-rw-r--   0 root         (0) root         (0)    11133 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_xray_timeline_by__b9129e.py
--rw-rw-r--   0 root         (0) root         (0)    11087 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_xray_timeline_by_user_id.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:30:36.473449 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/wrappers/
--rw-rw-r--   0 root         (0) root         (0)     4004 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/wrappers/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    32263 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/wrappers/_game_session_detail.py
--rw-rw-r--   0 root         (0) root         (0)     3395 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/wrappers/_operations.py
--rw-rw-r--   0 root         (0) root         (0)    68335 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/wrappers/_x_ray.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:30:36.473449 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk_service_sessionhistory.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1154 2024-05-07 06:30:36.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk_service_sessionhistory.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9504 2024-05-07 06:30:36.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk_service_sessionhistory.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-07 06:30:36.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk_service_sessionhistory.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-07 06:30:36.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk_service_sessionhistory.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-05-07 06:30:36.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk_service_sessionhistory.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)      374 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_sessionhistory-0.1.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-07 06:30:36.473449 accelbyte_py_sdk_service_sessionhistory-0.1.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:49:53.593846 accelbyte_py_sdk_service_sessionhistory-0.2.0/
+-rw-r--r--   0 root         (0) root         (0)     1155 2024-05-21 03:49:53.593846 accelbyte_py_sdk_service_sessionhistory-0.2.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      888 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:49:53.581847 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:49:53.581847 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:49:53.581847 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/
+-rw-rw-r--   0 root         (0) root         (0)     4112 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:49:53.589846 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/
+-rw-rw-r--   0 root         (0) root         (0)     6318 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7391 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_acquiring_ds.py
+-rw-rw-r--   0 root         (0) root         (0)     6156 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_acquiring_ds_wait_time.py
+-rw-rw-r--   0 root         (0) root         (0)     6223 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_canceled_matchmaking_ticket.py
+-rw-rw-r--   0 root         (0) root         (0)     6209 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_created_matchmaking_ticket.py
+-rw-rw-r--   0 root         (0) root         (0)     9448 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_event_match_history.py
+-rw-rw-r--   0 root         (0) root         (0)     6209 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_expired_matchmaking_ticket.py
+-rw-rw-r--   0 root         (0) root         (0)     7142 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_game_session_detail.py
+-rw-rw-r--   0 root         (0) root         (0)     5343 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_game_session_detail_query_response.py
+-rw-rw-r--   0 root         (0) root         (0)     7145 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_history.py
+-rw-rw-r--   0 root         (0) root         (0)     6155 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_match_length_duration.py
+-rw-rw-r--   0 root         (0) root         (0)     6096 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_match_matchmaking.py
+-rw-rw-r--   0 root         (0) root         (0)     6181 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_match_matchmaking_ticket.py
+-rw-rw-r--   0 root         (0) root         (0)    10590 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_matchmaking_detail.py
+-rw-rw-r--   0 root         (0) root         (0)     5341 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_matchmaking_detail_query_response.py
+-rw-rw-r--   0 root         (0) root         (0)     9860 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_matchmaking_history.py
+-rw-rw-r--   0 root         (0) root         (0)     5500 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_pagination.py
+-rw-rw-r--   0 root         (0) root         (0)     7199 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_party_detail.py
+-rw-rw-r--   0 root         (0) root         (0)     5164 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_party_detail_query_response.py
+-rw-rw-r--   0 root         (0) root         (0)     7197 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_party_history.py
+-rw-rw-r--   0 root         (0) root         (0)     5347 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_ticket_detail_query_response.py
+-rw-rw-r--   0 root         (0) root         (0)    18058 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_ticket_observability_detail.py
+-rw-rw-r--   0 root         (0) root         (0)     9318 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_ticket_observability_history.py
+-rw-rw-r--   0 root         (0) root         (0)     6049 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_total_active_session.py
+-rw-rw-r--   0 root         (0) root         (0)     6859 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_total_player_persession.py
+-rw-rw-r--   0 root         (0) root         (0)     4290 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_acquiring_ds_query_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4476 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_acquiring_ds_wait_time_query_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4591 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_canceled_matchmaking_ticket_query_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4573 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_created_matchmaking_ticket_query_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4573 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_expired_matchmaking_ticket_query_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5320 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_match_histor_query_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4474 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_match_length_duration_query_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4418 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_match_matchmaking_query_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4528 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_match_matchmaking_ticket_query_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4428 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_match_pool_pod_tick_match_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5458 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_match_pool_pod_tick_query_response.py
+-rw-rw-r--   0 root         (0) root         (0)    12957 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_match_pool_pod_tick_result.py
+-rw-rw-r--   0 root         (0) root         (0)     4344 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_match_pool_pod_tick_ticket_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4365 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_match_pool_query_response.py
+-rw-rw-r--   0 root         (0) root         (0)     3875 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_match_pool_result.py
+-rw-rw-r--   0 root         (0) root         (0)     6517 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_match_ticket_history.py
+-rw-rw-r--   0 root         (0) root         (0)     4495 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_match_ticket_history_query_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4379 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_matches_query_response.py
+-rw-rw-r--   0 root         (0) root         (0)    11450 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_ticket_matches_result.py
+-rw-rw-r--   0 root         (0) root         (0)     5253 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_ticket_query_response.py
+-rw-rw-r--   0 root         (0) root         (0)     7827 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_ticket_result.py
+-rw-rw-r--   0 root         (0) root         (0)     4456 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_total_active_session_query_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4544 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_total_player_persession_avg_query_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4553 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/logconfig_configuration.py
+-rw-rw-r--   0 root         (0) root         (0)     6169 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/models_alliance_rule.py
+-rw-rw-r--   0 root         (0) root         (0)     9433 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/models_backfill_proposal.py
+-rw-rw-r--   0 root         (0) root         (0)     8250 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/models_backfill_ticket.py
+-rw-rw-r--   0 root         (0) root         (0)     6239 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/models_ds_information.py
+-rw-rw-r--   0 root         (0) root         (0)    15892 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/models_game_server.py
+-rw-rw-r--   0 root         (0) root         (0)    20141 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/models_game_session.py
+-rw-rw-r--   0 root         (0) root         (0)     4982 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/models_game_session_team.py
+-rw-rw-r--   0 root         (0) root         (0)     9178 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/models_match.py
+-rw-rw-r--   0 root         (0) root         (0)     4293 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/models_matching_ally.py
+-rw-rw-r--   0 root         (0) root         (0)     7584 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/models_matching_party.py
+-rw-rw-r--   0 root         (0) root         (0)     5107 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/models_matching_rule.py
+-rw-rw-r--   0 root         (0) root         (0)    17838 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/models_matchmaking_result.py
+-rw-rw-r--   0 root         (0) root         (0)    14610 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/models_party.py
+-rw-rw-r--   0 root         (0) root         (0)     4767 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/models_party_member.py
+-rw-rw-r--   0 root         (0) root         (0)     4596 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/models_party_members.py
+-rw-rw-r--   0 root         (0) root         (0)     4546 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/models_party_team.py
+-rw-rw-r--   0 root         (0) root         (0)     6153 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/models_player_data.py
+-rw-rw-r--   0 root         (0) root         (0)     5388 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/models_proposed_proposal.py
+-rw-rw-r--   0 root         (0) root         (0)    11656 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/models_session_config.py
+-rw-rw-r--   0 root         (0) root         (0)    11929 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/models_session_configuration.py
+-rw-rw-r--   0 root         (0) root         (0)     4782 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/models_team.py
+-rw-rw-r--   0 root         (0) root         (0)    10979 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/models_ticket.py
+-rw-rw-r--   0 root         (0) root         (0)    20462 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/models_ticket_data.py
+-rw-rw-r--   0 root         (0) root         (0)     4070 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/models_ticket_observability.py
+-rw-rw-r--   0 root         (0) root         (0)     4588 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/models_ticket_status.py
+-rw-rw-r--   0 root         (0) root         (0)     7310 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/models_user.py
+-rw-rw-r--   0 root         (0) root         (0)     6536 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/response_error.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:49:53.589846 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/operations/
+-rw-rw-r--   0 root         (0) root         (0)      444 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/operations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:49:53.589846 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/operations/config/
+-rw-rw-r--   0 root         (0) root         (0)      598 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/operations/config/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     5204 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/operations/config/admin_get_log_config.py
+-rw-rw-r--   0 root         (0) root         (0)     6344 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/operations/config/admin_patch_update_log_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:49:53.589846 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/operations/game_session_detail/
+-rw-rw-r--   0 root         (0) root         (0)     1082 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/operations/game_session_detail/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7732 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/operations/game_session_detail/admin_get_matchmaking_d_8811e8.py
+-rw-rw-r--   0 root         (0) root         (0)     7738 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/operations/game_session_detail/admin_get_matchmaking_d_98288e.py
+-rw-rw-r--   0 root         (0) root         (0)    11975 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/operations/game_session_detail/admin_query_game_sessio_2eed0b.py
+-rw-rw-r--   0 root         (0) root         (0)    12822 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/operations/game_session_detail/admin_query_matchmaking_detail.py
+-rw-rw-r--   0 root         (0) root         (0)    11637 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/operations/game_session_detail/admin_query_party_detail.py
+-rw-rw-r--   0 root         (0) root         (0)    14222 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/operations/game_session_detail/admin_query_ticket_detail.py
+-rw-rw-r--   0 root         (0) root         (0)     7691 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/operations/game_session_detail/admin_ticket_detail_get_8ac60d.py
+-rw-rw-r--   0 root         (0) root         (0)     7790 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/operations/game_session_detail/get_game_session_detail.py
+-rw-rw-r--   0 root         (0) root         (0)     7654 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/operations/game_session_detail/get_party_detail.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:49:53.589846 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/operations/operations/
+-rw-rw-r--   0 root         (0) root         (0)      588 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/operations/operations/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4473 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/operations/operations/get_healthcheck_info.py
+-rw-rw-r--   0 root         (0) root         (0)     4529 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/operations/operations/get_healthcheck_info_v1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:49:53.593846 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/
+-rw-rw-r--   0 root         (0) root         (0)     1826 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8740 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_acquiring_ds.py
+-rw-rw-r--   0 root         (0) root         (0)     8926 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_acquiring_ds_wait_a2982b.py
+-rw-rw-r--   0 root         (0) root         (0)     9610 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_detail_tick_match_d45948.py
+-rw-rw-r--   0 root         (0) root         (0)     9606 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_detail_tick_match_f9b8b2.py
+-rw-rw-r--   0 root         (0) root         (0)    12741 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_detail_tick_match_pool.py
+-rw-rw-r--   0 root         (0) root         (0)     9472 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_match_histories.py
+-rw-rw-r--   0 root         (0) root         (0)     8920 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_match_length_dura_0e6d44.py
+-rw-rw-r--   0 root         (0) root         (0)     8913 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_match_length_durationp99.py
+-rw-rw-r--   0 root         (0) root         (0)     7942 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_match_ticket_histories.py
+-rw-rw-r--   0 root         (0) root         (0)     9656 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_total_active_session.py
+-rw-rw-r--   0 root         (0) root         (0)     9867 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_total_matchmaking_0ba5f3.py
+-rw-rw-r--   0 root         (0) root         (0)     9873 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_total_matchmaking_49d09d.py
+-rw-rw-r--   0 root         (0) root         (0)     9855 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_total_matchmaking_73a209.py
+-rw-rw-r--   0 root         (0) root         (0)     9855 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_total_matchmaking_adaa30.py
+-rw-rw-r--   0 root         (0) root         (0)     9748 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_total_matchmaking_match.py
+-rw-rw-r--   0 root         (0) root         (0)     8971 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_total_player_persession.py
+-rw-rw-r--   0 root         (0) root         (0)     7757 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_xray_match.py
+-rw-rw-r--   0 root         (0) root         (0)     9493 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_xray_match_pool.py
+-rw-rw-r--   0 root         (0) root         (0)    11133 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_xray_timeline_by__b9129e.py
+-rw-rw-r--   0 root         (0) root         (0)    11087 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_xray_timeline_by_user_id.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:49:53.593846 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/wrappers/
+-rw-rw-r--   0 root         (0) root         (0)     4204 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/wrappers/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4730 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/wrappers/_config.py
+-rw-rw-r--   0 root         (0) root         (0)    32263 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/wrappers/_game_session_detail.py
+-rw-rw-r--   0 root         (0) root         (0)     3467 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/wrappers/_operations.py
+-rw-rw-r--   0 root         (0) root         (0)    68335 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/wrappers/_x_ray.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:49:53.593846 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk_service_sessionhistory.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1155 2024-05-21 03:49:53.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk_service_sessionhistory.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9861 2024-05-21 03:49:53.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk_service_sessionhistory.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 03:49:53.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk_service_sessionhistory.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-21 03:49:53.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk_service_sessionhistory.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-05-21 03:49:53.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk_service_sessionhistory.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)      374 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_sessionhistory-0.2.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-21 03:49:53.593846 accelbyte_py_sdk_service_sessionhistory-0.2.0/setup.cfg
```

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/PKG-INFO` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: accelbyte-py-sdk-service-sessionhistory
-Version: 0.1.0
+Version: 0.2.0
 Summary: AccelByte Python SDK - AccelByte Gaming Services Session History Service
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: accelbyte-py-sdk-core
 
 [//]: # (Code generated. DO NOT EDIT!)
 
 # AccelByte Modular Python SDK - Service Module
 
 This is a service module for the [AccelByte Modular Python SDK](https://github.com/AccelByte/accelbyte-python-modular-sdk) package.
 
 ```text
 AccelByte Gaming Services Session History Service
-* Version: 1.9.4
+* Version: 1.10.1
 ```
 
 ## Setup
 
 This SDK requires Python 3.9 to be installed.
 
 ### Install with Pip
```

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/README.md` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # AccelByte Modular Python SDK - Service Module
 
 This is a service module for the [AccelByte Modular Python SDK](https://github.com/AccelByte/accelbyte-python-modular-sdk) package.
 
 ```text
 AccelByte Gaming Services Session History Service
-* Version: 1.9.4
+* Version: 1.10.1
 ```
 
 ## Setup
 
 This SDK requires Python 3.9 to be installed.
 
 ### Install with Pip
```

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/__init__.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,20 +4,26 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: service-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Session History Service."""
 
-__version__ = "1.9.4"
+__version__ = "1.10.1"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
+# config
+from .wrappers import admin_get_log_config
+from .wrappers import admin_get_log_config_async
+from .wrappers import admin_patch_update_log_config
+from .wrappers import admin_patch_update_log_config_async
+
 # game_session_detail
 from .wrappers import admin_get_matchmaking_detail_by_session_id
 from .wrappers import admin_get_matchmaking_detail_by_session_id_async
 from .wrappers import admin_get_matchmaking_detail_by_ticket_id
 from .wrappers import admin_get_matchmaking_detail_by_ticket_id_async
 from .wrappers import admin_query_game_session_detail
 from .wrappers import admin_query_game_session_detail_async
```

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/__init__.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: model-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Session History Service."""
 
-__version__ = "1.9.4"
+__version__ = "1.10.1"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .apimodels_acquiring_ds import ApimodelsAcquiringDS
 from .apimodels_acquiring_ds_wait_time import ApimodelsAcquiringDsWaitTime
@@ -95,14 +95,16 @@
 from .apimodels_x_ray_ticket_result import ApimodelsXRayTicketResult
 from .apimodels_x_ray_total_active_session_query_response import (
     ApimodelsXRayTotalActiveSessionQueryResponse,
 )
 from .apimodels_x_ray_total_player_persession_avg_query_response import (
     ApimodelsXRayTotalPlayerPersessionAVGQueryResponse,
 )
+from .logconfig_configuration import LogconfigConfiguration
+from .logconfig_configuration import LogLevelEnum as LogconfigConfigurationLogLevelEnum
 from .models_alliance_rule import ModelsAllianceRule
 from .models_backfill_proposal import ModelsBackfillProposal
 from .models_backfill_ticket import ModelsBackfillTicket
 from .models_ds_information import ModelsDSInformation
 from .models_game_server import ModelsGameServer
 from .models_game_session import ModelsGameSession
 from .models_game_session_team import ModelsGameSessionTeam
```

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_acquiring_ds.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_acquiring_ds.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_acquiring_ds_wait_time.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_acquiring_ds_wait_time.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_canceled_matchmaking_ticket.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_canceled_matchmaking_ticket.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_created_matchmaking_ticket.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_created_matchmaking_ticket.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_event_match_history.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_event_match_history.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_expired_matchmaking_ticket.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_expired_matchmaking_ticket.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_game_session_detail.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_game_session_detail.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_game_session_detail_query_response.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_game_session_detail_query_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_history.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_history.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_match_length_duration.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_match_length_duration.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_match_matchmaking.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_match_matchmaking.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_match_matchmaking_ticket.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_match_matchmaking_ticket.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_matchmaking_detail.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_matchmaking_detail.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_matchmaking_detail_query_response.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_matchmaking_detail_query_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_matchmaking_history.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_matchmaking_history.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_pagination.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_pagination.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_party_detail.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_party_detail.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_party_detail_query_response.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_party_detail_query_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_party_history.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_party_history.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_ticket_detail_query_response.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_ticket_detail_query_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_ticket_observability_detail.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_ticket_observability_detail.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_ticket_observability_history.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_ticket_observability_history.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_total_active_session.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_total_active_session.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_total_player_persession.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_total_player_persession.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_acquiring_ds_query_response.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_acquiring_ds_query_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_acquiring_ds_wait_time_query_response.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_acquiring_ds_wait_time_query_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_canceled_matchmaking_ticket_query_response.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_canceled_matchmaking_ticket_query_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_created_matchmaking_ticket_query_response.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_created_matchmaking_ticket_query_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_expired_matchmaking_ticket_query_response.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_expired_matchmaking_ticket_query_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_match_histor_query_response.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_match_histor_query_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_match_length_duration_query_response.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_match_length_duration_query_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_match_matchmaking_query_response.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_match_matchmaking_query_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_match_matchmaking_ticket_query_response.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_match_matchmaking_ticket_query_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_match_pool_pod_tick_match_response.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_match_pool_pod_tick_match_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_match_pool_pod_tick_query_response.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_match_pool_pod_tick_query_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_match_pool_pod_tick_result.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_match_pool_pod_tick_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_match_pool_pod_tick_ticket_response.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_match_pool_pod_tick_ticket_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_match_pool_query_response.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_match_pool_query_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_match_pool_result.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_match_pool_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_match_ticket_history.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_match_ticket_history.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_match_ticket_history_query_response.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_match_ticket_history_query_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_matches_query_response.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_matches_query_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_ticket_matches_result.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_ticket_matches_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_ticket_query_response.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_ticket_query_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_ticket_result.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_ticket_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_total_active_session_query_response.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_total_active_session_query_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_total_player_persession_avg_query_response.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_total_player_persession_avg_query_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/models_alliance_rule.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/models_alliance_rule.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/models_backfill_proposal.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/models_backfill_proposal.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/models_backfill_ticket.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/models_backfill_ticket.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/models_ds_information.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/models_ds_information.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/models_game_server.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/models_game_server.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/models_game_session.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/models_game_session.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/models_game_session_team.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/models_game_session_team.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/models_match.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/models_match.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/models_matching_ally.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/models_matching_ally.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/models_matching_party.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/models_matching_party.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/models_matching_rule.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/models_matching_rule.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/models_matchmaking_result.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/models_matchmaking_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/models_party.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/models_party.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/models_party_member.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/models_party_member.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/models_party_members.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/models_party_members.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/models_party_team.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/models_party_team.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/models_player_data.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/models_player_data.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/models_proposed_proposal.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/models_proposed_proposal.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/models_session_config.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/models_session_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/models_session_configuration.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/models_session_configuration.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/models_team.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/models_team.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/models_ticket.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/models_ticket.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/models_ticket_data.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/models_ticket_data.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/models_ticket_observability.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/models_ticket_observability.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/models_ticket_status.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/models_ticket_status.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/models_user.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/models_user.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/models/response_error.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/models/response_error.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/operations/game_session_detail/__init__.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/operations/game_session_detail/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Session History Service."""
 
-__version__ = "1.9.4"
+__version__ = "1.10.1"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .admin_get_matchmaking_d_98288e import AdminGetMatchmakingDetailBySessionID
 from .admin_get_matchmaking_d_8811e8 import AdminGetMatchmakingDetailByTicketID
```

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/operations/game_session_detail/admin_get_matchmaking_d_8811e8.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/operations/game_session_detail/admin_get_matchmaking_d_8811e8.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/operations/game_session_detail/admin_get_matchmaking_d_98288e.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/operations/game_session_detail/admin_get_matchmaking_d_98288e.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/operations/game_session_detail/admin_query_game_sessio_2eed0b.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/operations/game_session_detail/admin_query_game_sessio_2eed0b.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/operations/game_session_detail/admin_query_matchmaking_detail.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/operations/game_session_detail/admin_query_matchmaking_detail.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/operations/game_session_detail/admin_query_party_detail.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/operations/game_session_detail/admin_query_party_detail.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/operations/game_session_detail/admin_query_ticket_detail.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/operations/game_session_detail/admin_query_ticket_detail.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/operations/game_session_detail/admin_ticket_detail_get_8ac60d.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/operations/game_session_detail/admin_ticket_detail_get_8ac60d.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/operations/game_session_detail/get_game_session_detail.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/operations/game_session_detail/get_game_session_detail.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/operations/game_session_detail/get_party_detail.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/operations/game_session_detail/get_party_detail.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/operations/operations/__init__.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/operations/operations/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Session History Service."""
 
-__version__ = "1.9.4"
+__version__ = "1.10.1"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .get_healthcheck_info import GetHealthcheckInfo
 from .get_healthcheck_info_v1 import GetHealthcheckInfoV1
```

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/operations/operations/get_healthcheck_info.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/operations/operations/get_healthcheck_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,30 +39,30 @@
 
         method: GET
 
         tags: []
 
         consumes: []
 
-        produces: []
+        produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
     Responses:
         200: OK - (OK)
     """
 
     # region fields
 
     _url: str = "/healthz"
     _path: str = "/healthz"
     _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = []
-    _produces: List[str] = []
+    _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
     service_name: Optional[str] = "sessionhistory"
 
     # endregion fields
```

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/operations/operations/get_healthcheck_info_v1.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/operations/operations/get_healthcheck_info_v1.py`

 * *Files 7% similar despite different names*

```diff
@@ -39,30 +39,30 @@
 
         method: GET
 
         tags: []
 
         consumes: []
 
-        produces: []
+        produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
     Responses:
         200: OK - (OK)
     """
 
     # region fields
 
     _url: str = "/sessionhistory/healthz"
     _path: str = "/sessionhistory/healthz"
     _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = []
-    _produces: List[str] = []
+    _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
     service_name: Optional[str] = "sessionhistory"
 
     # endregion fields
```

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/__init__.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Session History Service."""
 
-__version__ = "1.9.4"
+__version__ = "1.10.1"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .query_acquiring_ds import QueryAcquiringDS
 from .query_acquiring_ds_wait_a2982b import QueryAcquiringDSWaitTimeAvg
```

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_acquiring_ds.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_acquiring_ds.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_acquiring_ds_wait_a2982b.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_acquiring_ds_wait_a2982b.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_detail_tick_match_d45948.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_detail_tick_match_d45948.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_detail_tick_match_f9b8b2.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_detail_tick_match_f9b8b2.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_detail_tick_match_pool.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_detail_tick_match_pool.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_match_histories.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_match_histories.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_match_length_dura_0e6d44.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_match_length_dura_0e6d44.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_match_length_durationp99.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_match_length_durationp99.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_match_ticket_histories.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_match_ticket_histories.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_total_active_session.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_total_active_session.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_total_matchmaking_0ba5f3.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_total_matchmaking_0ba5f3.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_total_matchmaking_49d09d.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_total_matchmaking_49d09d.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_total_matchmaking_73a209.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_total_matchmaking_73a209.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_total_matchmaking_adaa30.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_total_matchmaking_adaa30.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_total_matchmaking_match.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_total_matchmaking_match.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_total_player_persession.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_total_player_persession.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_xray_match.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_xray_match.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_xray_match_pool.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_xray_match_pool.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_xray_timeline_by__b9129e.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_xray_timeline_by__b9129e.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_xray_timeline_by_user_id.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_xray_timeline_by_user_id.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/wrappers/__init__.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/wrappers/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,20 +4,25 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: wrapper-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Session History Service."""
 
-__version__ = "1.9.4"
+__version__ = "1.10.1"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
+from ._config import admin_get_log_config
+from ._config import admin_get_log_config_async
+from ._config import admin_patch_update_log_config
+from ._config import admin_patch_update_log_config_async
+
 from ._game_session_detail import admin_get_matchmaking_detail_by_session_id
 from ._game_session_detail import admin_get_matchmaking_detail_by_session_id_async
 from ._game_session_detail import admin_get_matchmaking_detail_by_ticket_id
 from ._game_session_detail import admin_get_matchmaking_detail_by_ticket_id_async
 from ._game_session_detail import admin_query_game_session_detail
 from ._game_session_detail import admin_query_game_session_detail_async
 from ._game_session_detail import admin_query_matchmaking_detail
```

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/wrappers/_game_session_detail.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/wrappers/_game_session_detail.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/wrappers/_operations.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/wrappers/_operations.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
         method: GET
 
         tags: []
 
         consumes: []
 
-        produces: []
+        produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
     Responses:
         200: OK - (OK)
     """
     request = GetHealthcheckInfo.create()
@@ -73,15 +73,15 @@
 
         method: GET
 
         tags: []
 
         consumes: []
 
-        produces: []
+        produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
     Responses:
         200: OK - (OK)
     """
     request = GetHealthcheckInfo.create()
@@ -102,15 +102,15 @@
 
         method: GET
 
         tags: []
 
         consumes: []
 
-        produces: []
+        produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
     Responses:
         200: OK - (OK)
     """
     request = GetHealthcheckInfoV1.create()
@@ -129,15 +129,15 @@
 
         method: GET
 
         tags: []
 
         consumes: []
 
-        produces: []
+        produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
     Responses:
         200: OK - (OK)
     """
     request = GetHealthcheckInfoV1.create()
```

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk/api/sessionhistory/wrappers/_x_ray.py` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk/api/sessionhistory/wrappers/_x_ray.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk_service_sessionhistory.egg-info/PKG-INFO` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk_service_sessionhistory.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: accelbyte-py-sdk-service-sessionhistory
-Version: 0.1.0
+Version: 0.2.0
 Summary: AccelByte Python SDK - AccelByte Gaming Services Session History Service
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: accelbyte-py-sdk-core
 
 [//]: # (Code generated. DO NOT EDIT!)
 
 # AccelByte Modular Python SDK - Service Module
 
 This is a service module for the [AccelByte Modular Python SDK](https://github.com/AccelByte/accelbyte-python-modular-sdk) package.
 
 ```text
 AccelByte Gaming Services Session History Service
-* Version: 1.9.4
+* Version: 1.10.1
 ```
 
 ## Setup
 
 This SDK requires Python 3.9 to be installed.
 
 ### Install with Pip
```

### Comparing `accelbyte_py_sdk_service_sessionhistory-0.1.0/accelbyte_py_sdk_service_sessionhistory.egg-info/SOURCES.txt` & `accelbyte_py_sdk_service_sessionhistory-0.2.0/accelbyte_py_sdk_service_sessionhistory.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_match_ticket_history_query_response.py
 accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_matches_query_response.py
 accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_ticket_matches_result.py
 accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_ticket_query_response.py
 accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_ticket_result.py
 accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_total_active_session_query_response.py
 accelbyte_py_sdk/api/sessionhistory/models/apimodels_x_ray_total_player_persession_avg_query_response.py
+accelbyte_py_sdk/api/sessionhistory/models/logconfig_configuration.py
 accelbyte_py_sdk/api/sessionhistory/models/models_alliance_rule.py
 accelbyte_py_sdk/api/sessionhistory/models/models_backfill_proposal.py
 accelbyte_py_sdk/api/sessionhistory/models/models_backfill_ticket.py
 accelbyte_py_sdk/api/sessionhistory/models/models_ds_information.py
 accelbyte_py_sdk/api/sessionhistory/models/models_game_server.py
 accelbyte_py_sdk/api/sessionhistory/models/models_game_session.py
 accelbyte_py_sdk/api/sessionhistory/models/models_game_session_team.py
@@ -73,14 +74,17 @@
 accelbyte_py_sdk/api/sessionhistory/models/models_ticket.py
 accelbyte_py_sdk/api/sessionhistory/models/models_ticket_data.py
 accelbyte_py_sdk/api/sessionhistory/models/models_ticket_observability.py
 accelbyte_py_sdk/api/sessionhistory/models/models_ticket_status.py
 accelbyte_py_sdk/api/sessionhistory/models/models_user.py
 accelbyte_py_sdk/api/sessionhistory/models/response_error.py
 accelbyte_py_sdk/api/sessionhistory/operations/__init__.py
+accelbyte_py_sdk/api/sessionhistory/operations/config/__init__.py
+accelbyte_py_sdk/api/sessionhistory/operations/config/admin_get_log_config.py
+accelbyte_py_sdk/api/sessionhistory/operations/config/admin_patch_update_log_config.py
 accelbyte_py_sdk/api/sessionhistory/operations/game_session_detail/__init__.py
 accelbyte_py_sdk/api/sessionhistory/operations/game_session_detail/admin_get_matchmaking_d_8811e8.py
 accelbyte_py_sdk/api/sessionhistory/operations/game_session_detail/admin_get_matchmaking_d_98288e.py
 accelbyte_py_sdk/api/sessionhistory/operations/game_session_detail/admin_query_game_sessio_2eed0b.py
 accelbyte_py_sdk/api/sessionhistory/operations/game_session_detail/admin_query_matchmaking_detail.py
 accelbyte_py_sdk/api/sessionhistory/operations/game_session_detail/admin_query_party_detail.py
 accelbyte_py_sdk/api/sessionhistory/operations/game_session_detail/admin_query_ticket_detail.py
@@ -108,14 +112,15 @@
 accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_total_matchmaking_match.py
 accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_total_player_persession.py
 accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_xray_match.py
 accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_xray_match_pool.py
 accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_xray_timeline_by__b9129e.py
 accelbyte_py_sdk/api/sessionhistory/operations/x_ray/query_xray_timeline_by_user_id.py
 accelbyte_py_sdk/api/sessionhistory/wrappers/__init__.py
+accelbyte_py_sdk/api/sessionhistory/wrappers/_config.py
 accelbyte_py_sdk/api/sessionhistory/wrappers/_game_session_detail.py
 accelbyte_py_sdk/api/sessionhistory/wrappers/_operations.py
 accelbyte_py_sdk/api/sessionhistory/wrappers/_x_ray.py
 accelbyte_py_sdk_service_sessionhistory.egg-info/PKG-INFO
 accelbyte_py_sdk_service_sessionhistory.egg-info/SOURCES.txt
 accelbyte_py_sdk_service_sessionhistory.egg-info/dependency_links.txt
 accelbyte_py_sdk_service_sessionhistory.egg-info/requires.txt
```

