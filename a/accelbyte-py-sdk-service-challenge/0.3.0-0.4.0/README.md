# Comparing `tmp/accelbyte_py_sdk_service_challenge-0.3.0.tar.gz` & `tmp/accelbyte_py_sdk_service_challenge-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accelbyte_py_sdk_service_challenge-0.3.0.tar", last modified: Tue May  7 06:26:10 2024, max compression
+gzip compressed data, was "accelbyte_py_sdk_service_challenge-0.4.0.tar", last modified: Tue May 21 03:45:22 2024, max compression
```

## Comparing `accelbyte_py_sdk_service_challenge-0.3.0.tar` & `accelbyte_py_sdk_service_challenge-0.4.0.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:26:10.792635 accelbyte_py_sdk_service_challenge-0.3.0/
--rw-r--r--   0 root         (0) root         (0)     1132 2024-05-07 06:26:10.792635 accelbyte_py_sdk_service_challenge-0.3.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      876 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:26:10.788635 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:26:10.788635 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:26:10.788635 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/
--rw-rw-r--   0 root         (0) root         (0)     2538 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:26:10.792635 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/
--rw-rw-r--   0 root         (0) root         (0)     3643 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4474 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/iam_error_response.py
--rw-rw-r--   0 root         (0) root         (0)    14602 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_challenge_response.py
--rw-rw-r--   0 root         (0) root         (0)     3930 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_claim_user_rewards_req.py
--rw-rw-r--   0 root         (0) root         (0)    12603 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_create_challenge_request.py
--rw-rw-r--   0 root         (0) root         (0)     9703 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_create_goal_request.py
--rw-rw-r--   0 root         (0) root         (0)     4090 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_evaluate_player_progression_request.py
--rw-rw-r--   0 root         (0) root         (0)     4928 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_get_goals_response.py
--rw-rw-r--   0 root         (0) root         (0)     7676 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_goal_meta.py
--rw-rw-r--   0 root         (0) root         (0)     4458 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_goal_order.py
--rw-rw-r--   0 root         (0) root         (0)     9022 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_goal_progression_response.py
--rw-rw-r--   0 root         (0) root         (0)    12214 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_goal_response.py
--rw-rw-r--   0 root         (0) root         (0)     5051 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_goal_schedule.py
--rw-rw-r--   0 root         (0) root         (0)     5037 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_list_challenge_response.py
--rw-rw-r--   0 root         (0) root         (0)     4928 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_list_periods_response.py
--rw-rw-r--   0 root         (0) root         (0)     4999 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_list_user_rewards_response.py
--rw-rw-r--   0 root         (0) root         (0)     5424 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_pagination.py
--rw-rw-r--   0 root         (0) root         (0)     6987 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_predicate.py
--rw-rw-r--   0 root         (0) root         (0)     5094 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_requirement.py
--rw-rw-r--   0 root         (0) root         (0)     8409 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_requirement_progression_response.py
--rw-rw-r--   0 root         (0) root         (0)     5814 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_reward.py
--rw-rw-r--   0 root         (0) root         (0)     8061 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_schedule.py
--rw-rw-r--   0 root         (0) root         (0)     8956 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_update_goal_request.py
--rw-rw-r--   0 root         (0) root         (0)     6179 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_user_progression_response.py
--rw-rw-r--   0 root         (0) root         (0)     7227 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_user_progression_response_meta.py
--rw-rw-r--   0 root         (0) root         (0)    10051 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_user_reward.py
--rw-rw-r--   0 root         (0) root         (0)     4882 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/models_period.py
--rw-rw-r--   0 root         (0) root         (0)    12345 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/models_update_challenge_request.py
--rw-rw-r--   0 root         (0) root         (0)     6530 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/response_error.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:26:10.792635 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/
--rw-rw-r--   0 root         (0) root         (0)      437 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:26:10.792635 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/challenge_configuration/
--rw-rw-r--   0 root         (0) root         (0)     1007 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/challenge_configuration/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     9908 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/challenge_configuration/admin_create_challenge.py
--rw-rw-r--   0 root         (0) root         (0)     7934 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/challenge_configuration/admin_delete_challenge.py
--rw-rw-r--   0 root         (0) root         (0)     8127 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/challenge_configuration/admin_delete_tied_challenge.py
--rw-rw-r--   0 root         (0) root         (0)     7880 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/challenge_configuration/admin_get_challenge.py
--rw-rw-r--   0 root         (0) root         (0)    10423 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/challenge_configuration/admin_get_challenges.py
--rw-rw-r--   0 root         (0) root         (0)     9633 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/challenge_configuration/admin_get_periods.py
--rw-rw-r--   0 root         (0) root         (0)     8086 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/challenge_configuration/admin_randomize_challenge.py
--rw-rw-r--   0 root         (0) root         (0)     9591 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/challenge_configuration/admin_update_challenge.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:26:10.792635 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/challenge_list/
--rw-rw-r--   0 root         (0) root         (0)      651 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/challenge_list/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    10360 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/challenge_list/get_challenges.py
--rw-rw-r--   0 root         (0) root         (0)    10394 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/challenge_list/public_get_scheduled_goals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:26:10.792635 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/challenge_progression/
--rw-rw-r--   0 root         (0) root         (0)      648 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/challenge_progression/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8134 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/challenge_progression/admin_evaluate_progress.py
--rw-rw-r--   0 root         (0) root         (0)     6681 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/challenge_progression/evaluate_my_progress.py
--rw-rw-r--   0 root         (0) root         (0)    11538 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/challenge_progression/public_get_user_progression.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:26:10.792635 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/goal_configuration/
--rw-rw-r--   0 root         (0) root         (0)      697 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/goal_configuration/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    10497 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/goal_configuration/admin_create_goal.py
--rw-rw-r--   0 root         (0) root         (0)     8128 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/goal_configuration/admin_delete_goal.py
--rw-rw-r--   0 root         (0) root         (0)     8460 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/goal_configuration/admin_get_goal.py
--rw-rw-r--   0 root         (0) root         (0)    10383 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/goal_configuration/admin_get_goals.py
--rw-rw-r--   0 root         (0) root         (0)    10047 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/goal_configuration/admin_update_goals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:26:10.792635 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/player_reward/
--rw-rw-r--   0 root         (0) root         (0)      826 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/player_reward/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    11215 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/player_reward/admin_get_user_rewards.py
--rw-rw-r--   0 root         (0) root         (0)     8164 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/player_reward/public_claim_user_rewards.py
--rw-rw-r--   0 root         (0) root         (0)    10457 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/player_reward/public_get_user_rewards.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:26:10.792635 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/wrappers/
--rw-rw-r--   0 root         (0) root         (0)     2948 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/wrappers/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    32811 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/wrappers/_challenge_configuration.py
--rw-rw-r--   0 root         (0) root         (0)     8446 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/wrappers/_challenge_list.py
--rw-rw-r--   0 root         (0) root         (0)    11292 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/wrappers/_challenge_progression.py
--rw-rw-r--   0 root         (0) root         (0)    21624 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/wrappers/_goal_configuration.py
--rw-rw-r--   0 root         (0) root         (0)    12063 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/wrappers/_player_reward.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:26:10.792635 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk_service_challenge.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1132 2024-05-07 06:26:10.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk_service_challenge.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4849 2024-05-07 06:26:10.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk_service_challenge.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-07 06:26:10.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk_service_challenge.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-07 06:26:10.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk_service_challenge.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-05-07 06:26:10.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk_service_challenge.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)      363 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-07 06:26:10.792635 accelbyte_py_sdk_service_challenge-0.3.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:45:22.417191 accelbyte_py_sdk_service_challenge-0.4.0/
+-rw-r--r--   0 root         (0) root         (0)     1132 2024-05-21 03:45:22.417191 accelbyte_py_sdk_service_challenge-0.4.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      876 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_challenge-0.4.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:45:22.409191 accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:45:22.409191 accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:45:22.409191 accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/
+-rw-rw-r--   0 root         (0) root         (0)     2538 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:45:22.413191 accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/models/
+-rw-rw-r--   0 root         (0) root         (0)     3643 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/models/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4474 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/models/iam_error_response.py
+-rw-rw-r--   0 root         (0) root         (0)    14602 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/models/model_challenge_response.py
+-rw-rw-r--   0 root         (0) root         (0)     3930 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/models/model_claim_user_rewards_req.py
+-rw-rw-r--   0 root         (0) root         (0)    12603 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/models/model_create_challenge_request.py
+-rw-rw-r--   0 root         (0) root         (0)     9703 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/models/model_create_goal_request.py
+-rw-rw-r--   0 root         (0) root         (0)     4090 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/models/model_evaluate_player_progression_request.py
+-rw-rw-r--   0 root         (0) root         (0)     5843 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/models/model_get_goals_response.py
+-rw-rw-r--   0 root         (0) root         (0)     7676 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/models/model_goal_meta.py
+-rw-rw-r--   0 root         (0) root         (0)     4458 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/models/model_goal_order.py
+-rw-rw-r--   0 root         (0) root         (0)     9022 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/models/model_goal_progression_response.py
+-rw-rw-r--   0 root         (0) root         (0)    12214 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/models/model_goal_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5051 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/models/model_goal_schedule.py
+-rw-rw-r--   0 root         (0) root         (0)     5037 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/models/model_list_challenge_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4928 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/models/model_list_periods_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4999 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/models/model_list_user_rewards_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5424 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/models/model_pagination.py
+-rw-rw-r--   0 root         (0) root         (0)     7916 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/models/model_predicate.py
+-rw-rw-r--   0 root         (0) root         (0)     5094 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/models/model_requirement.py
+-rw-rw-r--   0 root         (0) root         (0)     9221 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/models/model_requirement_progression_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5814 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/models/model_reward.py
+-rw-rw-r--   0 root         (0) root         (0)     8061 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/models/model_schedule.py
+-rw-rw-r--   0 root         (0) root         (0)     8956 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/models/model_update_goal_request.py
+-rw-rw-r--   0 root         (0) root         (0)     6179 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/models/model_user_progression_response.py
+-rw-rw-r--   0 root         (0) root         (0)     7227 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/models/model_user_progression_response_meta.py
+-rw-rw-r--   0 root         (0) root         (0)    10051 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/models/model_user_reward.py
+-rw-rw-r--   0 root         (0) root         (0)     4882 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/models/models_period.py
+-rw-rw-r--   0 root         (0) root         (0)    12345 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/models/models_update_challenge_request.py
+-rw-rw-r--   0 root         (0) root         (0)     6530 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/models/response_error.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:45:22.413191 accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/operations/
+-rw-rw-r--   0 root         (0) root         (0)      437 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/operations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:45:22.413191 accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/operations/challenge_configuration/
+-rw-rw-r--   0 root         (0) root         (0)     1007 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/operations/challenge_configuration/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    10149 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/operations/challenge_configuration/admin_create_challenge.py
+-rw-rw-r--   0 root         (0) root         (0)     7934 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/operations/challenge_configuration/admin_delete_challenge.py
+-rw-rw-r--   0 root         (0) root         (0)     8127 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/operations/challenge_configuration/admin_delete_tied_challenge.py
+-rw-rw-r--   0 root         (0) root         (0)     7880 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/operations/challenge_configuration/admin_get_challenge.py
+-rw-rw-r--   0 root         (0) root         (0)    10423 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/operations/challenge_configuration/admin_get_challenges.py
+-rw-rw-r--   0 root         (0) root         (0)     9633 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/operations/challenge_configuration/admin_get_periods.py
+-rw-rw-r--   0 root         (0) root         (0)     8086 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/operations/challenge_configuration/admin_randomize_challenge.py
+-rw-rw-r--   0 root         (0) root         (0)     9832 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/operations/challenge_configuration/admin_update_challenge.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:45:22.413191 accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/operations/challenge_list/
+-rw-rw-r--   0 root         (0) root         (0)      651 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/operations/challenge_list/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    10360 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/operations/challenge_list/get_challenges.py
+-rw-rw-r--   0 root         (0) root         (0)    10601 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/operations/challenge_list/public_get_scheduled_goals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:45:22.413191 accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/operations/challenge_progression/
+-rw-rw-r--   0 root         (0) root         (0)      648 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/operations/challenge_progression/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8134 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/operations/challenge_progression/admin_evaluate_progress.py
+-rw-rw-r--   0 root         (0) root         (0)     6681 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/operations/challenge_progression/evaluate_my_progress.py
+-rw-rw-r--   0 root         (0) root         (0)    11538 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/operations/challenge_progression/public_get_user_progression.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:45:22.413191 accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/operations/goal_configuration/
+-rw-rw-r--   0 root         (0) root         (0)      697 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/operations/goal_configuration/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    10497 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/operations/goal_configuration/admin_create_goal.py
+-rw-rw-r--   0 root         (0) root         (0)     8128 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/operations/goal_configuration/admin_delete_goal.py
+-rw-rw-r--   0 root         (0) root         (0)     8460 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/operations/goal_configuration/admin_get_goal.py
+-rw-rw-r--   0 root         (0) root         (0)    10383 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/operations/goal_configuration/admin_get_goals.py
+-rw-rw-r--   0 root         (0) root         (0)    10288 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/operations/goal_configuration/admin_update_goals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:45:22.413191 accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/operations/player_reward/
+-rw-rw-r--   0 root         (0) root         (0)      826 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/operations/player_reward/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    11215 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/operations/player_reward/admin_get_user_rewards.py
+-rw-rw-r--   0 root         (0) root         (0)     8164 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/operations/player_reward/public_claim_user_rewards.py
+-rw-rw-r--   0 root         (0) root         (0)    10457 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/operations/player_reward/public_get_user_rewards.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:45:22.413191 accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/wrappers/
+-rw-rw-r--   0 root         (0) root         (0)     2948 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/wrappers/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    33115 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/wrappers/_challenge_configuration.py
+-rw-rw-r--   0 root         (0) root         (0)     8564 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/wrappers/_challenge_list.py
+-rw-rw-r--   0 root         (0) root         (0)    11292 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/wrappers/_challenge_progression.py
+-rw-rw-r--   0 root         (0) root         (0)    21776 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/wrappers/_goal_configuration.py
+-rw-rw-r--   0 root         (0) root         (0)    12063 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/wrappers/_player_reward.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 03:45:22.413191 accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk_service_challenge.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1132 2024-05-21 03:45:22.000000 accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk_service_challenge.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4849 2024-05-21 03:45:22.000000 accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk_service_challenge.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 03:45:22.000000 accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk_service_challenge.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-21 03:45:22.000000 accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk_service_challenge.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-05-21 03:45:22.000000 accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk_service_challenge.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)      363 2024-05-21 03:44:14.000000 accelbyte_py_sdk_service_challenge-0.4.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-21 03:45:22.417191 accelbyte_py_sdk_service_challenge-0.4.0/setup.cfg
```

### Comparing `accelbyte_py_sdk_service_challenge-0.3.0/PKG-INFO` & `accelbyte_py_sdk_service_challenge-0.4.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: accelbyte-py-sdk-service-challenge
-Version: 0.3.0
+Version: 0.4.0
 Summary: AccelByte Python SDK - AccelByte Gaming Services Challenge Service
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: accelbyte-py-sdk-core
 
 [//]: # (Code generated. DO NOT EDIT!)
```

### Comparing `accelbyte_py_sdk_service_challenge-0.3.0/README.md` & `accelbyte_py_sdk_service_challenge-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/__init__.py` & `accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/__init__.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/__init__.py` & `accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/models/__init__.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/iam_error_response.py` & `accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/models/iam_error_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_challenge_response.py` & `accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/models/model_challenge_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_claim_user_rewards_req.py` & `accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/models/model_claim_user_rewards_req.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_create_challenge_request.py` & `accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/models/model_create_challenge_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_create_goal_request.py` & `accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/models/model_create_goal_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_evaluate_player_progression_request.py` & `accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/models/model_evaluate_player_progression_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_get_goals_response.py` & `accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/models/model_list_user_rewards_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,41 +23,41 @@
 # pylint: disable=unused-import
 
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Model
 
-from ..models.model_goal_response import ModelGoalResponse
 from ..models.model_pagination import ModelPagination
+from ..models.model_user_reward import ModelUserReward
 
 
-class ModelGetGoalsResponse(Model):
-    """Model get goals response (model.GetGoalsResponse)
+class ModelListUserRewardsResponse(Model):
+    """Model list user rewards response (model.ListUserRewardsResponse)
 
     Properties:
-        data: (data) REQUIRED List[ModelGoalResponse]
+        data: (data) REQUIRED List[ModelUserReward]
 
         paging: (paging) REQUIRED ModelPagination
     """
 
     # region fields
 
-    data: List[ModelGoalResponse]  # REQUIRED
+    data: List[ModelUserReward]  # REQUIRED
     paging: ModelPagination  # REQUIRED
 
     # endregion fields
 
     # region with_x methods
 
-    def with_data(self, value: List[ModelGoalResponse]) -> ModelGetGoalsResponse:
+    def with_data(self, value: List[ModelUserReward]) -> ModelListUserRewardsResponse:
         self.data = value
         return self
 
-    def with_paging(self, value: ModelPagination) -> ModelGetGoalsResponse:
+    def with_paging(self, value: ModelPagination) -> ModelListUserRewardsResponse:
         self.paging = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
@@ -77,31 +77,31 @@
 
     # endregion to methods
 
     # region static methods
 
     @classmethod
     def create(
-        cls, data: List[ModelGoalResponse], paging: ModelPagination, **kwargs
-    ) -> ModelGetGoalsResponse:
+        cls, data: List[ModelUserReward], paging: ModelPagination, **kwargs
+    ) -> ModelListUserRewardsResponse:
         instance = cls()
         instance.data = data
         instance.paging = paging
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> ModelGetGoalsResponse:
+    ) -> ModelListUserRewardsResponse:
         instance = cls()
         if not dict_:
             return instance
         if "data" in dict_ and dict_["data"] is not None:
             instance.data = [
-                ModelGoalResponse.create_from_dict(i0, include_empty=include_empty)
+                ModelUserReward.create_from_dict(i0, include_empty=include_empty)
                 for i0 in dict_["data"]
             ]
         elif include_empty:
             instance.data = []
         if "paging" in dict_ and dict_["paging"] is not None:
             instance.paging = ModelPagination.create_from_dict(
                 dict_["paging"], include_empty=include_empty
@@ -109,38 +109,38 @@
         elif include_empty:
             instance.paging = ModelPagination()
         return instance
 
     @classmethod
     def create_many_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> Dict[str, ModelGetGoalsResponse]:
+    ) -> Dict[str, ModelListUserRewardsResponse]:
         return (
             {k: cls.create_from_dict(v, include_empty=include_empty) for k, v in dict_}
             if dict_
             else {}
         )
 
     @classmethod
     def create_many_from_list(
         cls, list_: list, include_empty: bool = False
-    ) -> List[ModelGetGoalsResponse]:
+    ) -> List[ModelListUserRewardsResponse]:
         return (
             [cls.create_from_dict(i, include_empty=include_empty) for i in list_]
             if list_
             else []
         )
 
     @classmethod
     def create_from_any(
         cls, any_: any, include_empty: bool = False, many: bool = False
     ) -> Union[
-        ModelGetGoalsResponse,
-        List[ModelGetGoalsResponse],
-        Dict[Any, ModelGetGoalsResponse],
+        ModelListUserRewardsResponse,
+        List[ModelListUserRewardsResponse],
+        Dict[Any, ModelListUserRewardsResponse],
     ]:
         if many:
             if isinstance(any_, dict):
                 return cls.create_many_from_dict(any_, include_empty=include_empty)
             elif isinstance(any_, list):
                 return cls.create_many_from_list(any_, include_empty=include_empty)
             else:
```

### Comparing `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_goal_meta.py` & `accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/models/model_goal_meta.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_goal_order.py` & `accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/models/model_goal_order.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_goal_progression_response.py` & `accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/models/model_goal_progression_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_goal_response.py` & `accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/models/model_goal_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_goal_schedule.py` & `accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/models/model_goal_schedule.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_list_challenge_response.py` & `accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/models/model_list_challenge_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_list_periods_response.py` & `accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/models/model_list_periods_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_list_user_rewards_response.py` & `accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/models/model_pagination.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,143 +23,165 @@
 # pylint: disable=unused-import
 
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Model
 
-from ..models.model_pagination import ModelPagination
-from ..models.model_user_reward import ModelUserReward
 
-
-class ModelListUserRewardsResponse(Model):
-    """Model list user rewards response (model.ListUserRewardsResponse)
+class ModelPagination(Model):
+    """Model pagination (model.Pagination)
 
     Properties:
-        data: (data) REQUIRED List[ModelUserReward]
+        first: (first) REQUIRED str
+
+        last: (last) REQUIRED str
 
-        paging: (paging) REQUIRED ModelPagination
+        next_: (next) REQUIRED str
+
+        previous: (previous) REQUIRED str
     """
 
     # region fields
 
-    data: List[ModelUserReward]  # REQUIRED
-    paging: ModelPagination  # REQUIRED
+    first: str  # REQUIRED
+    last: str  # REQUIRED
+    next_: str  # REQUIRED
+    previous: str  # REQUIRED
 
     # endregion fields
 
     # region with_x methods
 
-    def with_data(self, value: List[ModelUserReward]) -> ModelListUserRewardsResponse:
-        self.data = value
+    def with_first(self, value: str) -> ModelPagination:
+        self.first = value
+        return self
+
+    def with_last(self, value: str) -> ModelPagination:
+        self.last = value
+        return self
+
+    def with_next(self, value: str) -> ModelPagination:
+        self.next_ = value
         return self
 
-    def with_paging(self, value: ModelPagination) -> ModelListUserRewardsResponse:
-        self.paging = value
+    def with_previous(self, value: str) -> ModelPagination:
+        self.previous = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
-        if hasattr(self, "data"):
-            result["data"] = [
-                i0.to_dict(include_empty=include_empty) for i0 in self.data
-            ]
-        elif include_empty:
-            result["data"] = []
-        if hasattr(self, "paging"):
-            result["paging"] = self.paging.to_dict(include_empty=include_empty)
+        if hasattr(self, "first"):
+            result["first"] = str(self.first)
         elif include_empty:
-            result["paging"] = ModelPagination()
+            result["first"] = ""
+        if hasattr(self, "last"):
+            result["last"] = str(self.last)
+        elif include_empty:
+            result["last"] = ""
+        if hasattr(self, "next_"):
+            result["next"] = str(self.next_)
+        elif include_empty:
+            result["next"] = ""
+        if hasattr(self, "previous"):
+            result["previous"] = str(self.previous)
+        elif include_empty:
+            result["previous"] = ""
         return result
 
     # endregion to methods
 
     # region static methods
 
     @classmethod
     def create(
-        cls, data: List[ModelUserReward], paging: ModelPagination, **kwargs
-    ) -> ModelListUserRewardsResponse:
+        cls, first: str, last: str, next_: str, previous: str, **kwargs
+    ) -> ModelPagination:
         instance = cls()
-        instance.data = data
-        instance.paging = paging
+        instance.first = first
+        instance.last = last
+        instance.next_ = next_
+        instance.previous = previous
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> ModelListUserRewardsResponse:
+    ) -> ModelPagination:
         instance = cls()
         if not dict_:
             return instance
-        if "data" in dict_ and dict_["data"] is not None:
-            instance.data = [
-                ModelUserReward.create_from_dict(i0, include_empty=include_empty)
-                for i0 in dict_["data"]
-            ]
-        elif include_empty:
-            instance.data = []
-        if "paging" in dict_ and dict_["paging"] is not None:
-            instance.paging = ModelPagination.create_from_dict(
-                dict_["paging"], include_empty=include_empty
-            )
+        if "first" in dict_ and dict_["first"] is not None:
+            instance.first = str(dict_["first"])
+        elif include_empty:
+            instance.first = ""
+        if "last" in dict_ and dict_["last"] is not None:
+            instance.last = str(dict_["last"])
+        elif include_empty:
+            instance.last = ""
+        if "next" in dict_ and dict_["next"] is not None:
+            instance.next_ = str(dict_["next"])
+        elif include_empty:
+            instance.next_ = ""
+        if "previous" in dict_ and dict_["previous"] is not None:
+            instance.previous = str(dict_["previous"])
         elif include_empty:
-            instance.paging = ModelPagination()
+            instance.previous = ""
         return instance
 
     @classmethod
     def create_many_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> Dict[str, ModelListUserRewardsResponse]:
+    ) -> Dict[str, ModelPagination]:
         return (
             {k: cls.create_from_dict(v, include_empty=include_empty) for k, v in dict_}
             if dict_
             else {}
         )
 
     @classmethod
     def create_many_from_list(
         cls, list_: list, include_empty: bool = False
-    ) -> List[ModelListUserRewardsResponse]:
+    ) -> List[ModelPagination]:
         return (
             [cls.create_from_dict(i, include_empty=include_empty) for i in list_]
             if list_
             else []
         )
 
     @classmethod
     def create_from_any(
         cls, any_: any, include_empty: bool = False, many: bool = False
-    ) -> Union[
-        ModelListUserRewardsResponse,
-        List[ModelListUserRewardsResponse],
-        Dict[Any, ModelListUserRewardsResponse],
-    ]:
+    ) -> Union[ModelPagination, List[ModelPagination], Dict[Any, ModelPagination]]:
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
-            "data": "data",
-            "paging": "paging",
+            "first": "first",
+            "last": "last",
+            "next": "next_",
+            "previous": "previous",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
-            "data": True,
-            "paging": True,
+            "first": True,
+            "last": True,
+            "next": True,
+            "previous": True,
         }
 
     # endregion static methods
```

### Comparing `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_pagination.py` & `accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/models/model_reward.py`

 * *Files 15% similar despite different names*

```diff
@@ -22,166 +22,181 @@
 # pylint: disable=too-many-statements
 # pylint: disable=unused-import
 
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Model
+from accelbyte_py_sdk.core import StrEnum
 
 
-class ModelPagination(Model):
-    """Model pagination (model.Pagination)
+class TypeEnum(StrEnum):
+    ENTITLEMENT = "ENTITLEMENT"
+    STATISTIC = "STATISTIC"
+
+
+class ModelReward(Model):
+    """Model reward (model.Reward)
 
     Properties:
-        first: (first) REQUIRED str
+        item_id: (itemId) REQUIRED str
 
-        last: (last) REQUIRED str
+        item_name: (itemName) REQUIRED str
 
-        next_: (next) REQUIRED str
+        qty: (qty) REQUIRED float
 
-        previous: (previous) REQUIRED str
+        type_: (type) REQUIRED Union[str, TypeEnum]
     """
 
     # region fields
 
-    first: str  # REQUIRED
-    last: str  # REQUIRED
-    next_: str  # REQUIRED
-    previous: str  # REQUIRED
+    item_id: str  # REQUIRED
+    item_name: str  # REQUIRED
+    qty: float  # REQUIRED
+    type_: Union[str, TypeEnum]  # REQUIRED
 
     # endregion fields
 
     # region with_x methods
 
-    def with_first(self, value: str) -> ModelPagination:
-        self.first = value
+    def with_item_id(self, value: str) -> ModelReward:
+        self.item_id = value
         return self
 
-    def with_last(self, value: str) -> ModelPagination:
-        self.last = value
+    def with_item_name(self, value: str) -> ModelReward:
+        self.item_name = value
         return self
 
-    def with_next(self, value: str) -> ModelPagination:
-        self.next_ = value
+    def with_qty(self, value: float) -> ModelReward:
+        self.qty = value
         return self
 
-    def with_previous(self, value: str) -> ModelPagination:
-        self.previous = value
+    def with_type(self, value: Union[str, TypeEnum]) -> ModelReward:
+        self.type_ = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
-        if hasattr(self, "first"):
-            result["first"] = str(self.first)
+        if hasattr(self, "item_id"):
+            result["itemId"] = str(self.item_id)
         elif include_empty:
-            result["first"] = ""
-        if hasattr(self, "last"):
-            result["last"] = str(self.last)
-        elif include_empty:
-            result["last"] = ""
-        if hasattr(self, "next_"):
-            result["next"] = str(self.next_)
-        elif include_empty:
-            result["next"] = ""
-        if hasattr(self, "previous"):
-            result["previous"] = str(self.previous)
+            result["itemId"] = ""
+        if hasattr(self, "item_name"):
+            result["itemName"] = str(self.item_name)
+        elif include_empty:
+            result["itemName"] = ""
+        if hasattr(self, "qty"):
+            result["qty"] = float(self.qty)
+        elif include_empty:
+            result["qty"] = 0.0
+        if hasattr(self, "type_"):
+            result["type"] = str(self.type_)
         elif include_empty:
-            result["previous"] = ""
+            result["type"] = Union[str, TypeEnum]()
         return result
 
     # endregion to methods
 
     # region static methods
 
     @classmethod
     def create(
-        cls, first: str, last: str, next_: str, previous: str, **kwargs
-    ) -> ModelPagination:
+        cls,
+        item_id: str,
+        item_name: str,
+        qty: float,
+        type_: Union[str, TypeEnum],
+        **kwargs,
+    ) -> ModelReward:
         instance = cls()
-        instance.first = first
-        instance.last = last
-        instance.next_ = next_
-        instance.previous = previous
+        instance.item_id = item_id
+        instance.item_name = item_name
+        instance.qty = qty
+        instance.type_ = type_
         return instance
 
     @classmethod
-    def create_from_dict(
-        cls, dict_: dict, include_empty: bool = False
-    ) -> ModelPagination:
+    def create_from_dict(cls, dict_: dict, include_empty: bool = False) -> ModelReward:
         instance = cls()
         if not dict_:
             return instance
-        if "first" in dict_ and dict_["first"] is not None:
-            instance.first = str(dict_["first"])
+        if "itemId" in dict_ and dict_["itemId"] is not None:
+            instance.item_id = str(dict_["itemId"])
         elif include_empty:
-            instance.first = ""
-        if "last" in dict_ and dict_["last"] is not None:
-            instance.last = str(dict_["last"])
-        elif include_empty:
-            instance.last = ""
-        if "next" in dict_ and dict_["next"] is not None:
-            instance.next_ = str(dict_["next"])
-        elif include_empty:
-            instance.next_ = ""
-        if "previous" in dict_ and dict_["previous"] is not None:
-            instance.previous = str(dict_["previous"])
+            instance.item_id = ""
+        if "itemName" in dict_ and dict_["itemName"] is not None:
+            instance.item_name = str(dict_["itemName"])
+        elif include_empty:
+            instance.item_name = ""
+        if "qty" in dict_ and dict_["qty"] is not None:
+            instance.qty = float(dict_["qty"])
+        elif include_empty:
+            instance.qty = 0.0
+        if "type" in dict_ and dict_["type"] is not None:
+            instance.type_ = str(dict_["type"])
         elif include_empty:
-            instance.previous = ""
+            instance.type_ = Union[str, TypeEnum]()
         return instance
 
     @classmethod
     def create_many_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> Dict[str, ModelPagination]:
+    ) -> Dict[str, ModelReward]:
         return (
             {k: cls.create_from_dict(v, include_empty=include_empty) for k, v in dict_}
             if dict_
             else {}
         )
 
     @classmethod
     def create_many_from_list(
         cls, list_: list, include_empty: bool = False
-    ) -> List[ModelPagination]:
+    ) -> List[ModelReward]:
         return (
             [cls.create_from_dict(i, include_empty=include_empty) for i in list_]
             if list_
             else []
         )
 
     @classmethod
     def create_from_any(
         cls, any_: any, include_empty: bool = False, many: bool = False
-    ) -> Union[ModelPagination, List[ModelPagination], Dict[Any, ModelPagination]]:
+    ) -> Union[ModelReward, List[ModelReward], Dict[Any, ModelReward]]:
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
-            "first": "first",
-            "last": "last",
-            "next": "next_",
-            "previous": "previous",
+            "itemId": "item_id",
+            "itemName": "item_name",
+            "qty": "qty",
+            "type": "type_",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
-            "first": True,
-            "last": True,
-            "next": True,
-            "previous": True,
+            "itemId": True,
+            "itemName": True,
+            "qty": True,
+            "type": True,
+        }
+
+    @staticmethod
+    def get_enum_map() -> Dict[str, List[Any]]:
+        return {
+            "type": ["ENTITLEMENT", "STATISTIC"],
         }
 
     # endregion static methods
```

### Comparing `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_predicate.py` & `accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/models/model_predicate.py`

 * *Files 13% similar despite different names*

```diff
@@ -36,36 +36,40 @@
     LESS_THAN = "LESS_THAN"
     LESS_THAN_EQUAL = "LESS_THAN_EQUAL"
 
 
 class ParameterTypeEnum(StrEnum):
     ACHIEVEMENT = "ACHIEVEMENT"
     STATISTIC = "STATISTIC"
+    STATISTIC_CYCLE = "STATISTIC_CYCLE"
     USERACCOUNT = "USERACCOUNT"
 
 
 class ModelPredicate(Model):
     """Model predicate (model.Predicate)
 
     Properties:
         matcher: (matcher) REQUIRED Union[str, MatcherEnum]
 
         parameter_name: (parameterName) REQUIRED str
 
         parameter_type: (parameterType) REQUIRED Union[str, ParameterTypeEnum]
 
         target_value: (targetValue) REQUIRED float
+
+        stat_cycle_id: (statCycleId) OPTIONAL str
     """
 
     # region fields
 
     matcher: Union[str, MatcherEnum]  # REQUIRED
     parameter_name: str  # REQUIRED
     parameter_type: Union[str, ParameterTypeEnum]  # REQUIRED
     target_value: float  # REQUIRED
+    stat_cycle_id: str  # OPTIONAL
 
     # endregion fields
 
     # region with_x methods
 
     def with_matcher(self, value: Union[str, MatcherEnum]) -> ModelPredicate:
         self.matcher = value
@@ -81,14 +85,18 @@
         self.parameter_type = value
         return self
 
     def with_target_value(self, value: float) -> ModelPredicate:
         self.target_value = value
         return self
 
+    def with_stat_cycle_id(self, value: str) -> ModelPredicate:
+        self.stat_cycle_id = value
+        return self
+
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
         if hasattr(self, "matcher"):
@@ -103,34 +111,41 @@
             result["parameterType"] = str(self.parameter_type)
         elif include_empty:
             result["parameterType"] = Union[str, ParameterTypeEnum]()
         if hasattr(self, "target_value"):
             result["targetValue"] = float(self.target_value)
         elif include_empty:
             result["targetValue"] = 0.0
+        if hasattr(self, "stat_cycle_id"):
+            result["statCycleId"] = str(self.stat_cycle_id)
+        elif include_empty:
+            result["statCycleId"] = ""
         return result
 
     # endregion to methods
 
     # region static methods
 
     @classmethod
     def create(
         cls,
         matcher: Union[str, MatcherEnum],
         parameter_name: str,
         parameter_type: Union[str, ParameterTypeEnum],
         target_value: float,
+        stat_cycle_id: Optional[str] = None,
         **kwargs,
     ) -> ModelPredicate:
         instance = cls()
         instance.matcher = matcher
         instance.parameter_name = parameter_name
         instance.parameter_type = parameter_type
         instance.target_value = target_value
+        if stat_cycle_id is not None:
+            instance.stat_cycle_id = stat_cycle_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
     ) -> ModelPredicate:
         instance = cls()
@@ -148,14 +163,18 @@
             instance.parameter_type = str(dict_["parameterType"])
         elif include_empty:
             instance.parameter_type = Union[str, ParameterTypeEnum]()
         if "targetValue" in dict_ and dict_["targetValue"] is not None:
             instance.target_value = float(dict_["targetValue"])
         elif include_empty:
             instance.target_value = 0.0
+        if "statCycleId" in dict_ and dict_["statCycleId"] is not None:
+            instance.stat_cycle_id = str(dict_["statCycleId"])
+        elif include_empty:
+            instance.stat_cycle_id = ""
         return instance
 
     @classmethod
     def create_many_from_dict(
         cls, dict_: dict, include_empty: bool = False
     ) -> Dict[str, ModelPredicate]:
         return (
@@ -191,32 +210,39 @@
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
             "matcher": "matcher",
             "parameterName": "parameter_name",
             "parameterType": "parameter_type",
             "targetValue": "target_value",
+            "statCycleId": "stat_cycle_id",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
             "matcher": True,
             "parameterName": True,
             "parameterType": True,
             "targetValue": True,
+            "statCycleId": False,
         }
 
     @staticmethod
     def get_enum_map() -> Dict[str, List[Any]]:
         return {
             "matcher": [
                 "EQUAL",
                 "GREATER_THAN",
                 "GREATER_THAN_EQUAL",
                 "LESS_THAN",
                 "LESS_THAN_EQUAL",
             ],
-            "parameterType": ["ACHIEVEMENT", "STATISTIC", "USERACCOUNT"],
+            "parameterType": [
+                "ACHIEVEMENT",
+                "STATISTIC",
+                "STATISTIC_CYCLE",
+                "USERACCOUNT",
+            ],
         }
 
     # endregion static methods
```

### Comparing `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_requirement.py` & `accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/models/model_requirement.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_requirement_progression_response.py` & `accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/models/model_requirement_progression_response.py`

 * *Files 19% similar despite different names*

```diff
@@ -41,25 +41,28 @@
         parameter_name: (parameterName) REQUIRED str
 
         parameter_type: (parameterType) REQUIRED str
 
         target_value: (targetValue) REQUIRED float
 
         completed_at: (completedAt) OPTIONAL str
+
+        stat_cycle_id: (statCycleId) OPTIONAL str
     """
 
     # region fields
 
     current_value: float  # REQUIRED
     id_: str  # REQUIRED
     matcher: str  # REQUIRED
     parameter_name: str  # REQUIRED
     parameter_type: str  # REQUIRED
     target_value: float  # REQUIRED
     completed_at: str  # OPTIONAL
+    stat_cycle_id: str  # OPTIONAL
 
     # endregion fields
 
     # region with_x methods
 
     def with_current_value(self, value: float) -> ModelRequirementProgressionResponse:
         self.current_value = value
@@ -85,14 +88,18 @@
         self.target_value = value
         return self
 
     def with_completed_at(self, value: str) -> ModelRequirementProgressionResponse:
         self.completed_at = value
         return self
 
+    def with_stat_cycle_id(self, value: str) -> ModelRequirementProgressionResponse:
+        self.stat_cycle_id = value
+        return self
+
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
         if hasattr(self, "current_value"):
@@ -119,14 +126,18 @@
             result["targetValue"] = float(self.target_value)
         elif include_empty:
             result["targetValue"] = 0.0
         if hasattr(self, "completed_at"):
             result["completedAt"] = str(self.completed_at)
         elif include_empty:
             result["completedAt"] = ""
+        if hasattr(self, "stat_cycle_id"):
+            result["statCycleId"] = str(self.stat_cycle_id)
+        elif include_empty:
+            result["statCycleId"] = ""
         return result
 
     # endregion to methods
 
     # region static methods
 
     @classmethod
@@ -135,25 +146,28 @@
         current_value: float,
         id_: str,
         matcher: str,
         parameter_name: str,
         parameter_type: str,
         target_value: float,
         completed_at: Optional[str] = None,
+        stat_cycle_id: Optional[str] = None,
         **kwargs,
     ) -> ModelRequirementProgressionResponse:
         instance = cls()
         instance.current_value = current_value
         instance.id_ = id_
         instance.matcher = matcher
         instance.parameter_name = parameter_name
         instance.parameter_type = parameter_type
         instance.target_value = target_value
         if completed_at is not None:
             instance.completed_at = completed_at
+        if stat_cycle_id is not None:
+            instance.stat_cycle_id = stat_cycle_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
     ) -> ModelRequirementProgressionResponse:
         instance = cls()
@@ -183,14 +197,18 @@
             instance.target_value = float(dict_["targetValue"])
         elif include_empty:
             instance.target_value = 0.0
         if "completedAt" in dict_ and dict_["completedAt"] is not None:
             instance.completed_at = str(dict_["completedAt"])
         elif include_empty:
             instance.completed_at = ""
+        if "statCycleId" in dict_ and dict_["statCycleId"] is not None:
+            instance.stat_cycle_id = str(dict_["statCycleId"])
+        elif include_empty:
+            instance.stat_cycle_id = ""
         return instance
 
     @classmethod
     def create_many_from_dict(
         cls, dict_: dict, include_empty: bool = False
     ) -> Dict[str, ModelRequirementProgressionResponse]:
         return (
@@ -233,22 +251,24 @@
             "currentValue": "current_value",
             "id": "id_",
             "matcher": "matcher",
             "parameterName": "parameter_name",
             "parameterType": "parameter_type",
             "targetValue": "target_value",
             "completedAt": "completed_at",
+            "statCycleId": "stat_cycle_id",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
             "currentValue": True,
             "id": True,
             "matcher": True,
             "parameterName": True,
             "parameterType": True,
             "targetValue": True,
             "completedAt": False,
+            "statCycleId": False,
         }
 
     # endregion static methods
```

### Comparing `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_reward.py` & `accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/models/response_error.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,181 +22,194 @@
 # pylint: disable=too-many-statements
 # pylint: disable=unused-import
 
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Model
-from accelbyte_py_sdk.core import StrEnum
 
 
-class TypeEnum(StrEnum):
-    ENTITLEMENT = "ENTITLEMENT"
-    STATISTIC = "STATISTIC"
-
-
-class ModelReward(Model):
-    """Model reward (model.Reward)
+class ResponseError(Model):
+    """Response error (response.Error)
 
     Properties:
-        item_id: (itemId) REQUIRED str
+        attributes: (attributes) REQUIRED Dict[str, str]
+
+        error_code: (errorCode) REQUIRED int
 
-        item_name: (itemName) REQUIRED str
+        error_message: (errorMessage) REQUIRED str
 
-        qty: (qty) REQUIRED float
+        message: (message) REQUIRED str
 
-        type_: (type) REQUIRED Union[str, TypeEnum]
+        name: (name) REQUIRED str
     """
 
     # region fields
 
-    item_id: str  # REQUIRED
-    item_name: str  # REQUIRED
-    qty: float  # REQUIRED
-    type_: Union[str, TypeEnum]  # REQUIRED
+    attributes: Dict[str, str]  # REQUIRED
+    error_code: int  # REQUIRED
+    error_message: str  # REQUIRED
+    message: str  # REQUIRED
+    name: str  # REQUIRED
 
     # endregion fields
 
     # region with_x methods
 
-    def with_item_id(self, value: str) -> ModelReward:
-        self.item_id = value
+    def with_attributes(self, value: Dict[str, str]) -> ResponseError:
+        self.attributes = value
         return self
 
-    def with_item_name(self, value: str) -> ModelReward:
-        self.item_name = value
+    def with_error_code(self, value: int) -> ResponseError:
+        self.error_code = value
         return self
 
-    def with_qty(self, value: float) -> ModelReward:
-        self.qty = value
+    def with_error_message(self, value: str) -> ResponseError:
+        self.error_message = value
         return self
 
-    def with_type(self, value: Union[str, TypeEnum]) -> ModelReward:
-        self.type_ = value
+    def with_message(self, value: str) -> ResponseError:
+        self.message = value
+        return self
+
+    def with_name(self, value: str) -> ResponseError:
+        self.name = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
-        if hasattr(self, "item_id"):
-            result["itemId"] = str(self.item_id)
-        elif include_empty:
-            result["itemId"] = ""
-        if hasattr(self, "item_name"):
-            result["itemName"] = str(self.item_name)
-        elif include_empty:
-            result["itemName"] = ""
-        if hasattr(self, "qty"):
-            result["qty"] = float(self.qty)
-        elif include_empty:
-            result["qty"] = 0.0
-        if hasattr(self, "type_"):
-            result["type"] = str(self.type_)
+        if hasattr(self, "attributes"):
+            result["attributes"] = {
+                str(k0): str(v0) for k0, v0 in self.attributes.items()
+            }
+        elif include_empty:
+            result["attributes"] = {}
+        if hasattr(self, "error_code"):
+            result["errorCode"] = int(self.error_code)
+        elif include_empty:
+            result["errorCode"] = 0
+        if hasattr(self, "error_message"):
+            result["errorMessage"] = str(self.error_message)
+        elif include_empty:
+            result["errorMessage"] = ""
+        if hasattr(self, "message"):
+            result["message"] = str(self.message)
+        elif include_empty:
+            result["message"] = ""
+        if hasattr(self, "name"):
+            result["name"] = str(self.name)
         elif include_empty:
-            result["type"] = Union[str, TypeEnum]()
+            result["name"] = ""
         return result
 
     # endregion to methods
 
     # region static methods
 
     @classmethod
     def create(
         cls,
-        item_id: str,
-        item_name: str,
-        qty: float,
-        type_: Union[str, TypeEnum],
+        attributes: Dict[str, str],
+        error_code: int,
+        error_message: str,
+        message: str,
+        name: str,
         **kwargs,
-    ) -> ModelReward:
+    ) -> ResponseError:
         instance = cls()
-        instance.item_id = item_id
-        instance.item_name = item_name
-        instance.qty = qty
-        instance.type_ = type_
+        instance.attributes = attributes
+        instance.error_code = error_code
+        instance.error_message = error_message
+        instance.message = message
+        instance.name = name
         return instance
 
     @classmethod
-    def create_from_dict(cls, dict_: dict, include_empty: bool = False) -> ModelReward:
+    def create_from_dict(
+        cls, dict_: dict, include_empty: bool = False
+    ) -> ResponseError:
         instance = cls()
         if not dict_:
             return instance
-        if "itemId" in dict_ and dict_["itemId"] is not None:
-            instance.item_id = str(dict_["itemId"])
-        elif include_empty:
-            instance.item_id = ""
-        if "itemName" in dict_ and dict_["itemName"] is not None:
-            instance.item_name = str(dict_["itemName"])
-        elif include_empty:
-            instance.item_name = ""
-        if "qty" in dict_ and dict_["qty"] is not None:
-            instance.qty = float(dict_["qty"])
-        elif include_empty:
-            instance.qty = 0.0
-        if "type" in dict_ and dict_["type"] is not None:
-            instance.type_ = str(dict_["type"])
+        if "attributes" in dict_ and dict_["attributes"] is not None:
+            instance.attributes = {
+                str(k0): str(v0) for k0, v0 in dict_["attributes"].items()
+            }
+        elif include_empty:
+            instance.attributes = {}
+        if "errorCode" in dict_ and dict_["errorCode"] is not None:
+            instance.error_code = int(dict_["errorCode"])
+        elif include_empty:
+            instance.error_code = 0
+        if "errorMessage" in dict_ and dict_["errorMessage"] is not None:
+            instance.error_message = str(dict_["errorMessage"])
+        elif include_empty:
+            instance.error_message = ""
+        if "message" in dict_ and dict_["message"] is not None:
+            instance.message = str(dict_["message"])
+        elif include_empty:
+            instance.message = ""
+        if "name" in dict_ and dict_["name"] is not None:
+            instance.name = str(dict_["name"])
         elif include_empty:
-            instance.type_ = Union[str, TypeEnum]()
+            instance.name = ""
         return instance
 
     @classmethod
     def create_many_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> Dict[str, ModelReward]:
+    ) -> Dict[str, ResponseError]:
         return (
             {k: cls.create_from_dict(v, include_empty=include_empty) for k, v in dict_}
             if dict_
             else {}
         )
 
     @classmethod
     def create_many_from_list(
         cls, list_: list, include_empty: bool = False
-    ) -> List[ModelReward]:
+    ) -> List[ResponseError]:
         return (
             [cls.create_from_dict(i, include_empty=include_empty) for i in list_]
             if list_
             else []
         )
 
     @classmethod
     def create_from_any(
         cls, any_: any, include_empty: bool = False, many: bool = False
-    ) -> Union[ModelReward, List[ModelReward], Dict[Any, ModelReward]]:
+    ) -> Union[ResponseError, List[ResponseError], Dict[Any, ResponseError]]:
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
-            "itemId": "item_id",
-            "itemName": "item_name",
-            "qty": "qty",
-            "type": "type_",
+            "attributes": "attributes",
+            "errorCode": "error_code",
+            "errorMessage": "error_message",
+            "message": "message",
+            "name": "name",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
-            "itemId": True,
-            "itemName": True,
-            "qty": True,
-            "type": True,
-        }
-
-    @staticmethod
-    def get_enum_map() -> Dict[str, List[Any]]:
-        return {
-            "type": ["ENTITLEMENT", "STATISTIC"],
+            "attributes": True,
+            "errorCode": True,
+            "errorMessage": True,
+            "message": True,
+            "name": True,
         }
 
     # endregion static methods
```

### Comparing `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_schedule.py` & `accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/models/model_schedule.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_update_goal_request.py` & `accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/models/model_update_goal_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_user_progression_response.py` & `accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/models/model_user_progression_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_user_progression_response_meta.py` & `accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/models/model_user_progression_response_meta.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_user_reward.py` & `accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/models/model_user_reward.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/models_period.py` & `accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/models/models_period.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/models_update_challenge_request.py` & `accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/models/models_update_challenge_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/response_error.py` & `accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/models/model_get_goals_response.py`

 * *Files 25% similar despite different names*

```diff
@@ -23,193 +23,168 @@
 # pylint: disable=unused-import
 
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Model
 
+from ..models.model_challenge_response import ModelChallengeResponse
+from ..models.model_goal_response import ModelGoalResponse
+from ..models.model_pagination import ModelPagination
 
-class ResponseError(Model):
-    """Response error (response.Error)
 
-    Properties:
-        attributes: (attributes) REQUIRED Dict[str, str]
-
-        error_code: (errorCode) REQUIRED int
+class ModelGetGoalsResponse(Model):
+    """Model get goals response (model.GetGoalsResponse)
 
-        error_message: (errorMessage) REQUIRED str
+    Properties:
+        data: (data) REQUIRED List[ModelGoalResponse]
 
-        message: (message) REQUIRED str
+        meta: (meta) REQUIRED ModelChallengeResponse
 
-        name: (name) REQUIRED str
+        paging: (paging) REQUIRED ModelPagination
     """
 
     # region fields
 
-    attributes: Dict[str, str]  # REQUIRED
-    error_code: int  # REQUIRED
-    error_message: str  # REQUIRED
-    message: str  # REQUIRED
-    name: str  # REQUIRED
+    data: List[ModelGoalResponse]  # REQUIRED
+    meta: ModelChallengeResponse  # REQUIRED
+    paging: ModelPagination  # REQUIRED
 
     # endregion fields
 
     # region with_x methods
 
-    def with_attributes(self, value: Dict[str, str]) -> ResponseError:
-        self.attributes = value
-        return self
-
-    def with_error_code(self, value: int) -> ResponseError:
-        self.error_code = value
-        return self
-
-    def with_error_message(self, value: str) -> ResponseError:
-        self.error_message = value
+    def with_data(self, value: List[ModelGoalResponse]) -> ModelGetGoalsResponse:
+        self.data = value
         return self
 
-    def with_message(self, value: str) -> ResponseError:
-        self.message = value
+    def with_meta(self, value: ModelChallengeResponse) -> ModelGetGoalsResponse:
+        self.meta = value
         return self
 
-    def with_name(self, value: str) -> ResponseError:
-        self.name = value
+    def with_paging(self, value: ModelPagination) -> ModelGetGoalsResponse:
+        self.paging = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
-        if hasattr(self, "attributes"):
-            result["attributes"] = {
-                str(k0): str(v0) for k0, v0 in self.attributes.items()
-            }
-        elif include_empty:
-            result["attributes"] = {}
-        if hasattr(self, "error_code"):
-            result["errorCode"] = int(self.error_code)
-        elif include_empty:
-            result["errorCode"] = 0
-        if hasattr(self, "error_message"):
-            result["errorMessage"] = str(self.error_message)
-        elif include_empty:
-            result["errorMessage"] = ""
-        if hasattr(self, "message"):
-            result["message"] = str(self.message)
-        elif include_empty:
-            result["message"] = ""
-        if hasattr(self, "name"):
-            result["name"] = str(self.name)
+        if hasattr(self, "data"):
+            result["data"] = [
+                i0.to_dict(include_empty=include_empty) for i0 in self.data
+            ]
+        elif include_empty:
+            result["data"] = []
+        if hasattr(self, "meta"):
+            result["meta"] = self.meta.to_dict(include_empty=include_empty)
+        elif include_empty:
+            result["meta"] = ModelChallengeResponse()
+        if hasattr(self, "paging"):
+            result["paging"] = self.paging.to_dict(include_empty=include_empty)
         elif include_empty:
-            result["name"] = ""
+            result["paging"] = ModelPagination()
         return result
 
     # endregion to methods
 
     # region static methods
 
     @classmethod
     def create(
         cls,
-        attributes: Dict[str, str],
-        error_code: int,
-        error_message: str,
-        message: str,
-        name: str,
+        data: List[ModelGoalResponse],
+        meta: ModelChallengeResponse,
+        paging: ModelPagination,
         **kwargs,
-    ) -> ResponseError:
+    ) -> ModelGetGoalsResponse:
         instance = cls()
-        instance.attributes = attributes
-        instance.error_code = error_code
-        instance.error_message = error_message
-        instance.message = message
-        instance.name = name
+        instance.data = data
+        instance.meta = meta
+        instance.paging = paging
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> ResponseError:
+    ) -> ModelGetGoalsResponse:
         instance = cls()
         if not dict_:
             return instance
-        if "attributes" in dict_ and dict_["attributes"] is not None:
-            instance.attributes = {
-                str(k0): str(v0) for k0, v0 in dict_["attributes"].items()
-            }
-        elif include_empty:
-            instance.attributes = {}
-        if "errorCode" in dict_ and dict_["errorCode"] is not None:
-            instance.error_code = int(dict_["errorCode"])
-        elif include_empty:
-            instance.error_code = 0
-        if "errorMessage" in dict_ and dict_["errorMessage"] is not None:
-            instance.error_message = str(dict_["errorMessage"])
-        elif include_empty:
-            instance.error_message = ""
-        if "message" in dict_ and dict_["message"] is not None:
-            instance.message = str(dict_["message"])
-        elif include_empty:
-            instance.message = ""
-        if "name" in dict_ and dict_["name"] is not None:
-            instance.name = str(dict_["name"])
+        if "data" in dict_ and dict_["data"] is not None:
+            instance.data = [
+                ModelGoalResponse.create_from_dict(i0, include_empty=include_empty)
+                for i0 in dict_["data"]
+            ]
+        elif include_empty:
+            instance.data = []
+        if "meta" in dict_ and dict_["meta"] is not None:
+            instance.meta = ModelChallengeResponse.create_from_dict(
+                dict_["meta"], include_empty=include_empty
+            )
+        elif include_empty:
+            instance.meta = ModelChallengeResponse()
+        if "paging" in dict_ and dict_["paging"] is not None:
+            instance.paging = ModelPagination.create_from_dict(
+                dict_["paging"], include_empty=include_empty
+            )
         elif include_empty:
-            instance.name = ""
+            instance.paging = ModelPagination()
         return instance
 
     @classmethod
     def create_many_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> Dict[str, ResponseError]:
+    ) -> Dict[str, ModelGetGoalsResponse]:
         return (
             {k: cls.create_from_dict(v, include_empty=include_empty) for k, v in dict_}
             if dict_
             else {}
         )
 
     @classmethod
     def create_many_from_list(
         cls, list_: list, include_empty: bool = False
-    ) -> List[ResponseError]:
+    ) -> List[ModelGetGoalsResponse]:
         return (
             [cls.create_from_dict(i, include_empty=include_empty) for i in list_]
             if list_
             else []
         )
 
     @classmethod
     def create_from_any(
         cls, any_: any, include_empty: bool = False, many: bool = False
-    ) -> Union[ResponseError, List[ResponseError], Dict[Any, ResponseError]]:
+    ) -> Union[
+        ModelGetGoalsResponse,
+        List[ModelGetGoalsResponse],
+        Dict[Any, ModelGetGoalsResponse],
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
-            "attributes": "attributes",
-            "errorCode": "error_code",
-            "errorMessage": "error_message",
-            "message": "message",
-            "name": "name",
+            "data": "data",
+            "meta": "meta",
+            "paging": "paging",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
-            "attributes": True,
-            "errorCode": True,
-            "errorMessage": True,
-            "message": True,
-            "name": True,
+            "data": True,
+            "meta": True,
+            "paging": True,
         }
 
     # endregion static methods
```

### Comparing `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/challenge_configuration/__init__.py` & `accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/operations/challenge_configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/challenge_configuration/admin_create_challenge.py` & `accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/operations/challenge_configuration/admin_create_challenge.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,14 +76,16 @@
         body: (body) REQUIRED ModelCreateChallengeRequest in body
 
         namespace: (namespace) REQUIRED str in path
 
     Responses:
         201: Created - ModelChallengeResponse (Created)
 
+        400: Bad Request - ResponseError (20018: bad request: {{message}})
+
         401: Unauthorized - IamErrorResponse (20001: unauthorized access)
 
         403: Forbidden - IamErrorResponse (20013: insufficient permission)
 
         409: Conflict - ResponseError (99002: duplicate key error: {{message}})
 
         422: Unprocessable Entity - ResponseError (99003: challenge validation error: {{message}})
@@ -211,14 +213,16 @@
         Union[None, ModelChallengeResponse],
         Union[None, HttpResponse, IamErrorResponse, ResponseError],
     ]:
         """Parse the given response.
 
         201: Created - ModelChallengeResponse (Created)
 
+        400: Bad Request - ResponseError (20018: bad request: {{message}})
+
         401: Unauthorized - IamErrorResponse (20001: unauthorized access)
 
         403: Forbidden - IamErrorResponse (20013: insufficient permission)
 
         409: Conflict - ResponseError (99002: duplicate key error: {{message}})
 
         422: Unprocessable Entity - ResponseError (99003: challenge validation error: {{message}})
@@ -236,14 +240,16 @@
         )
         if error is not None:
             return None, None if error.is_no_content() else error
         code, content_type, content = pre_processed_response
 
         if code == 201:
             return ModelChallengeResponse.create_from_dict(content), None
+        if code == 400:
+            return None, ResponseError.create_from_dict(content)
         if code == 401:
             return None, IamErrorResponse.create_from_dict(content)
         if code == 403:
             return None, IamErrorResponse.create_from_dict(content)
         if code == 409:
             return None, ResponseError.create_from_dict(content)
         if code == 422:
```

### Comparing `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/challenge_configuration/admin_delete_challenge.py` & `accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/operations/challenge_configuration/admin_delete_challenge.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/challenge_configuration/admin_delete_tied_challenge.py` & `accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/operations/challenge_configuration/admin_delete_tied_challenge.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/challenge_configuration/admin_get_challenge.py` & `accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/operations/challenge_configuration/admin_get_challenge.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/challenge_configuration/admin_get_challenges.py` & `accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/operations/challenge_configuration/admin_get_challenges.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/challenge_configuration/admin_get_periods.py` & `accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/operations/challenge_configuration/admin_get_periods.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/challenge_configuration/admin_randomize_challenge.py` & `accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/operations/challenge_configuration/admin_randomize_challenge.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/challenge_configuration/admin_update_challenge.py` & `accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/operations/challenge_configuration/admin_update_challenge.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,14 +71,16 @@
         challenge_code: (challengeCode) REQUIRED str in path
 
         namespace: (namespace) REQUIRED str in path
 
     Responses:
         200: OK - ModelChallengeResponse (OK)
 
+        400: Bad Request - ResponseError (20018: bad request: {{message}})
+
         401: Unauthorized - ResponseError (Unauthorized)
 
         403: Forbidden - ResponseError (Forbidden)
 
         404: Not Found - ResponseError (Not Found)
 
         422: Unprocessable Entity - ResponseError (Unprocessable Entity)
@@ -216,14 +218,16 @@
     ) -> Tuple[
         Union[None, ModelChallengeResponse], Union[None, HttpResponse, ResponseError]
     ]:
         """Parse the given response.
 
         200: OK - ModelChallengeResponse (OK)
 
+        400: Bad Request - ResponseError (20018: bad request: {{message}})
+
         401: Unauthorized - ResponseError (Unauthorized)
 
         403: Forbidden - ResponseError (Forbidden)
 
         404: Not Found - ResponseError (Not Found)
 
         422: Unprocessable Entity - ResponseError (Unprocessable Entity)
@@ -241,14 +245,16 @@
         )
         if error is not None:
             return None, None if error.is_no_content() else error
         code, content_type, content = pre_processed_response
 
         if code == 200:
             return ModelChallengeResponse.create_from_dict(content), None
+        if code == 400:
+            return None, ResponseError.create_from_dict(content)
         if code == 401:
             return None, ResponseError.create_from_dict(content)
         if code == 403:
             return None, ResponseError.create_from_dict(content)
         if code == 404:
             return None, ResponseError.create_from_dict(content)
         if code == 422:
```

### Comparing `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/challenge_list/__init__.py` & `accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/operations/challenge_list/__init__.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/challenge_list/get_challenges.py` & `accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/operations/challenge_list/get_challenges.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/challenge_list/public_get_scheduled_goals.py` & `accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/operations/challenge_list/public_get_scheduled_goals.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,14 +68,16 @@
     Responses:
         200: OK - ModelGetGoalsResponse (OK)
 
         401: Unauthorized - IamErrorResponse (20001: unauthorized access)
 
         403: Forbidden - IamErrorResponse (20013: insufficient permission)
 
+        404: Not Found - ResponseError (20029: not found)
+
         500: Internal Server Error - ResponseError (20000: internal server error: {{message}})
     """
 
     # region fields
 
     _url: str = (
         "/challenge/v1/public/namespaces/{namespace}/challenges/{challengeCode}/goals"
@@ -237,14 +239,16 @@
 
         200: OK - ModelGetGoalsResponse (OK)
 
         401: Unauthorized - IamErrorResponse (20001: unauthorized access)
 
         403: Forbidden - IamErrorResponse (20013: insufficient permission)
 
+        404: Not Found - ResponseError (20029: not found)
+
         500: Internal Server Error - ResponseError (20000: internal server error: {{message}})
 
         ---: HttpResponse (Undocumented Response)
 
         ---: HttpResponse (Unexpected Content-Type Error)
 
         ---: HttpResponse (Unhandled Error)
@@ -258,14 +262,16 @@
 
         if code == 200:
             return ModelGetGoalsResponse.create_from_dict(content), None
         if code == 401:
             return None, IamErrorResponse.create_from_dict(content)
         if code == 403:
             return None, IamErrorResponse.create_from_dict(content)
+        if code == 404:
+            return None, ResponseError.create_from_dict(content)
         if code == 500:
             return None, ResponseError.create_from_dict(content)
 
         return self.handle_undocumented_response(
             code=code, content_type=content_type, content=content
         )
```

### Comparing `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/challenge_progression/__init__.py` & `accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/operations/challenge_progression/__init__.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/challenge_progression/admin_evaluate_progress.py` & `accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/operations/challenge_progression/admin_evaluate_progress.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/challenge_progression/evaluate_my_progress.py` & `accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/operations/challenge_progression/evaluate_my_progress.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/challenge_progression/public_get_user_progression.py` & `accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/operations/challenge_progression/public_get_user_progression.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/goal_configuration/__init__.py` & `accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/operations/goal_configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/goal_configuration/admin_create_goal.py` & `accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/operations/goal_configuration/admin_create_goal.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/goal_configuration/admin_delete_goal.py` & `accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/operations/goal_configuration/admin_delete_goal.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/goal_configuration/admin_get_goal.py` & `accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/operations/goal_configuration/admin_get_goal.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/goal_configuration/admin_get_goals.py` & `accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/operations/goal_configuration/admin_get_goals.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/goal_configuration/admin_update_goals.py` & `accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/operations/goal_configuration/admin_update_goals.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,14 +72,16 @@
         code: (code) REQUIRED str in path
 
         namespace: (namespace) REQUIRED str in path
 
     Responses:
         200: OK - ModelGoalResponse (OK)
 
+        400: Bad Request - ResponseError (20018: bad request: {{message}})
+
         404: Not Found - ResponseError (Not Found)
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
@@ -222,14 +224,16 @@
     ) -> Tuple[
         Union[None, ModelGoalResponse], Union[None, HttpResponse, ResponseError]
     ]:
         """Parse the given response.
 
         200: OK - ModelGoalResponse (OK)
 
+        400: Bad Request - ResponseError (20018: bad request: {{message}})
+
         404: Not Found - ResponseError (Not Found)
 
         500: Internal Server Error - ResponseError (Internal Server Error)
 
         ---: HttpResponse (Undocumented Response)
 
         ---: HttpResponse (Unexpected Content-Type Error)
@@ -241,14 +245,16 @@
         )
         if error is not None:
             return None, None if error.is_no_content() else error
         code, content_type, content = pre_processed_response
 
         if code == 200:
             return ModelGoalResponse.create_from_dict(content), None
+        if code == 400:
+            return None, ResponseError.create_from_dict(content)
         if code == 404:
             return None, ResponseError.create_from_dict(content)
         if code == 500:
             return None, ResponseError.create_from_dict(content)
 
         return self.handle_undocumented_response(
             code=code, content_type=content_type, content=content
```

### Comparing `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/player_reward/__init__.py` & `accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/operations/player_reward/__init__.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/player_reward/admin_get_user_rewards.py` & `accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/operations/player_reward/admin_get_user_rewards.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/player_reward/public_claim_user_rewards.py` & `accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/operations/player_reward/public_claim_user_rewards.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/player_reward/public_get_user_rewards.py` & `accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/operations/player_reward/public_get_user_rewards.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/wrappers/__init__.py` & `accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/wrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/wrappers/_challenge_configuration.py` & `accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/wrappers/_challenge_configuration.py`

 * *Files 4% similar despite different names*

```diff
@@ -114,14 +114,16 @@
         body: (body) REQUIRED ModelCreateChallengeRequest in body
 
         namespace: (namespace) REQUIRED str in path
 
     Responses:
         201: Created - ModelChallengeResponse (Created)
 
+        400: Bad Request - ResponseError (20018: bad request: {{message}})
+
         401: Unauthorized - IamErrorResponse (20001: unauthorized access)
 
         403: Forbidden - IamErrorResponse (20013: insufficient permission)
 
         409: Conflict - ResponseError (99002: duplicate key error: {{message}})
 
         422: Unprocessable Entity - ResponseError (99003: challenge validation error: {{message}})
@@ -186,14 +188,16 @@
         body: (body) REQUIRED ModelCreateChallengeRequest in body
 
         namespace: (namespace) REQUIRED str in path
 
     Responses:
         201: Created - ModelChallengeResponse (Created)
 
+        400: Bad Request - ResponseError (20018: bad request: {{message}})
+
         401: Unauthorized - IamErrorResponse (20001: unauthorized access)
 
         403: Forbidden - IamErrorResponse (20013: insufficient permission)
 
         409: Conflict - ResponseError (99002: duplicate key error: {{message}})
 
         422: Unprocessable Entity - ResponseError (99003: challenge validation error: {{message}})
@@ -955,14 +959,16 @@
         challenge_code: (challengeCode) REQUIRED str in path
 
         namespace: (namespace) REQUIRED str in path
 
     Responses:
         200: OK - ModelChallengeResponse (OK)
 
+        400: Bad Request - ResponseError (20018: bad request: {{message}})
+
         401: Unauthorized - ResponseError (Unauthorized)
 
         403: Forbidden - ResponseError (Forbidden)
 
         404: Not Found - ResponseError (Not Found)
 
         422: Unprocessable Entity - ResponseError (Unprocessable Entity)
@@ -1025,14 +1031,16 @@
         challenge_code: (challengeCode) REQUIRED str in path
 
         namespace: (namespace) REQUIRED str in path
 
     Responses:
         200: OK - ModelChallengeResponse (OK)
 
+        400: Bad Request - ResponseError (20018: bad request: {{message}})
+
         401: Unauthorized - ResponseError (Unauthorized)
 
         403: Forbidden - ResponseError (Forbidden)
 
         404: Not Found - ResponseError (Not Found)
 
         422: Unprocessable Entity - ResponseError (Unprocessable Entity)
```

### Comparing `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/wrappers/_challenge_list.py` & `accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/wrappers/_challenge_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -212,14 +212,16 @@
     Responses:
         200: OK - ModelGetGoalsResponse (OK)
 
         401: Unauthorized - IamErrorResponse (20001: unauthorized access)
 
         403: Forbidden - IamErrorResponse (20013: insufficient permission)
 
+        404: Not Found - ResponseError (20029: not found)
+
         500: Internal Server Error - ResponseError (20000: internal server error: {{message}})
     """
     if namespace is None:
         namespace, error = get_services_namespace()
         if error:
             return None, error
     request = PublicGetScheduledGoals.create(
@@ -275,14 +277,16 @@
     Responses:
         200: OK - ModelGetGoalsResponse (OK)
 
         401: Unauthorized - IamErrorResponse (20001: unauthorized access)
 
         403: Forbidden - IamErrorResponse (20013: insufficient permission)
 
+        404: Not Found - ResponseError (20029: not found)
+
         500: Internal Server Error - ResponseError (20000: internal server error: {{message}})
     """
     if namespace is None:
         namespace, error = get_services_namespace()
         if error:
             return None, error
     request = PublicGetScheduledGoals.create(
```

### Comparing `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/wrappers/_challenge_progression.py` & `accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/wrappers/_challenge_progression.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/wrappers/_goal_configuration.py` & `accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/wrappers/_goal_configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -595,14 +595,16 @@
         code: (code) REQUIRED str in path
 
         namespace: (namespace) REQUIRED str in path
 
     Responses:
         200: OK - ModelGoalResponse (OK)
 
+        400: Bad Request - ResponseError (20018: bad request: {{message}})
+
         404: Not Found - ResponseError (Not Found)
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
     if namespace is None:
         namespace, error = get_services_namespace()
         if error:
@@ -662,14 +664,16 @@
         code: (code) REQUIRED str in path
 
         namespace: (namespace) REQUIRED str in path
 
     Responses:
         200: OK - ModelGoalResponse (OK)
 
+        400: Bad Request - ResponseError (20018: bad request: {{message}})
+
         404: Not Found - ResponseError (Not Found)
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
     if namespace is None:
         namespace, error = get_services_namespace()
         if error:
```

### Comparing `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/wrappers/_player_reward.py` & `accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk/api/challenge/wrappers/_player_reward.py`

 * *Files identical despite different names*

### Comparing `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk_service_challenge.egg-info/PKG-INFO` & `accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk_service_challenge.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: accelbyte-py-sdk-service-challenge
-Version: 0.3.0
+Version: 0.4.0
 Summary: AccelByte Python SDK - AccelByte Gaming Services Challenge Service
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: accelbyte-py-sdk-core
 
 [//]: # (Code generated. DO NOT EDIT!)
```

### Comparing `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk_service_challenge.egg-info/SOURCES.txt` & `accelbyte_py_sdk_service_challenge-0.4.0/accelbyte_py_sdk_service_challenge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

