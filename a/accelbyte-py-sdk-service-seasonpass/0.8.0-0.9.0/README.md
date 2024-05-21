# Comparing `tmp/accelbyte-py-sdk-service-seasonpass-0.8.0.tar.gz` & `tmp/accelbyte-py-sdk-service-seasonpass-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accelbyte-py-sdk-service-seasonpass-0.8.0.tar", last modified: Tue Feb 27 05:41:42 2024, max compression
+gzip compressed data, was "accelbyte-py-sdk-service-seasonpass-0.9.0.tar", last modified: Wed Mar 13 06:14:23 2024, max compression
```

## Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0.tar` & `accelbyte-py-sdk-service-seasonpass-0.9.0.tar`

### file list

```diff
@@ -1,124 +1,124 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:41:42.579944 accelbyte-py-sdk-service-seasonpass-0.8.0/
--rw-r--r--   0 root         (0) root         (0)     1137 2024-02-27 05:41:42.579944 accelbyte-py-sdk-service-seasonpass-0.8.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      879 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:41:42.567945 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:41:42.567945 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:41:42.567945 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/
--rw-rw-r--   0 root         (0) root         (0)     4304 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:41:42.571945 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/
--rw-rw-r--   0 root         (0) root         (0)     3332 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3968 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/bulk_user_progression_request.py
--rw-rw-r--   0 root         (0) root         (0)     5036 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/claimable_rewards.py
--rw-rw-r--   0 root         (0) root         (0)    17655 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/claimable_user_season_info.py
--rw-rw-r--   0 root         (0) root         (0)     6324 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/error_entity.py
--rw-rw-r--   0 root         (0) root         (0)     5585 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/excess_strategy.py
--rw-rw-r--   0 root         (0) root         (0)     8726 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/exp_grant_history_info.py
--rw-rw-r--   0 root         (0) root         (0)     5755 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/exp_grant_history_paging_sliced_result.py
--rw-rw-r--   0 root         (0) root         (0)     7302 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/field_validation_error.py
--rw-rw-r--   0 root         (0) root         (0)     9606 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/full_season_info.py
--rw-rw-r--   0 root         (0) root         (0)     6864 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/image.py
--rw-rw-r--   0 root         (0) root         (0)    12208 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/list_season_info.py
--rw-rw-r--   0 root         (0) root         (0)     5026 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/list_season_info_paging_sliced_result.py
--rw-rw-r--   0 root         (0) root         (0)     9499 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/list_user_season_info.py
--rw-rw-r--   0 root         (0) root         (0)     5788 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/list_user_season_info_paging_sliced_result.py
--rw-rw-r--   0 root         (0) root         (0)     4412 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/localization.py
--rw-rw-r--   0 root         (0) root         (0)    11559 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/localized_pass_info.py
--rw-rw-r--   0 root         (0) root         (0)    17248 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/localized_season_info.py
--rw-rw-r--   0 root         (0) root         (0)     3570 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/ownership.py
--rw-rw-r--   0 root         (0) root         (0)     4268 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/paging.py
--rw-rw-r--   0 root         (0) root         (0)     7844 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/pass_create.py
--rw-rw-r--   0 root         (0) root         (0)    11150 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/pass_info.py
--rw-rw-r--   0 root         (0) root         (0)     7460 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/pass_update.py
--rw-rw-r--   0 root         (0) root         (0)     3696 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/reason_tags_result.py
--rw-rw-r--   0 root         (0) root         (0)     7676 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/reward_create.py
--rw-rw-r--   0 root         (0) root         (0)     4457 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/reward_currency.py
--rw-rw-r--   0 root         (0) root         (0)    11825 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/reward_info.py
--rw-rw-r--   0 root         (0) root         (0)     7972 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/reward_update.py
--rw-rw-r--   0 root         (0) root         (0)     4812 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/season_clone_request.py
--rw-rw-r--   0 root         (0) root         (0)    11838 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/season_create.py
--rw-rw-r--   0 root         (0) root         (0)    17474 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/season_info.py
--rw-rw-r--   0 root         (0) root         (0)     9452 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/season_summary.py
--rw-rw-r--   0 root         (0) root         (0)    12238 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/season_update.py
--rw-rw-r--   0 root         (0) root         (0)     5202 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/tier.py
--rw-rw-r--   0 root         (0) root         (0)     5189 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/tier_create.py
--rw-rw-r--   0 root         (0) root         (0)     4703 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/tier_input.py
--rw-rw-r--   0 root         (0) root         (0)     5488 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/tier_paging_sliced_result.py
--rw-rw-r--   0 root         (0) root         (0)     3707 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/tier_reorder.py
--rw-rw-r--   0 root         (0) root         (0)     5357 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/user_exp_grant.py
--rw-rw-r--   0 root         (0) root         (0)     4567 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/user_pass_grant.py
--rw-rw-r--   0 root         (0) root         (0)     5474 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/user_purchasable.py
--rw-rw-r--   0 root         (0) root         (0)     5109 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/user_reward_claim.py
--rw-rw-r--   0 root         (0) root         (0)    12836 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/user_season_summary.py
--rw-rw-r--   0 root         (0) root         (0)     5426 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/user_tier_grant.py
--rw-rw-r--   0 root         (0) root         (0)     5630 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/validation_error_entity.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:41:42.575945 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/
--rw-rw-r--   0 root         (0) root         (0)      439 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:41:42.575945 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/export/
--rw-rw-r--   0 root         (0) root         (0)      512 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/export/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5678 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/export/export_season.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:41:42.575945 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/pass_/
--rw-rw-r--   0 root         (0) root         (0)      691 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/pass_/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     9231 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/pass_/create_pass.py
--rw-rw-r--   0 root         (0) root         (0)     7981 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/pass_/delete_pass.py
--rw-rw-r--   0 root         (0) root         (0)     7738 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/pass_/get_pass.py
--rw-rw-r--   0 root         (0) root         (0)     8093 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/pass_/grant_user_pass.py
--rw-rw-r--   0 root         (0) root         (0)     7064 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/pass_/query_passes.py
--rw-rw-r--   0 root         (0) root         (0)     9946 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/pass_/update_pass.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:41:42.575945 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/reward/
--rw-rw-r--   0 root         (0) root         (0)      797 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/reward/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     9386 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/reward/create_reward.py
--rw-rw-r--   0 root         (0) root         (0)     8097 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/reward/delete_reward.py
--rw-rw-r--   0 root         (0) root         (0)     7776 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/reward/get_reward.py
--rw-rw-r--   0 root         (0) root         (0)     7339 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/reward/public_bulk_claim_user_rewards.py
--rw-rw-r--   0 root         (0) root         (0)     8788 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/reward/public_claim_user_reward.py
--rw-rw-r--   0 root         (0) root         (0)     7866 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/reward/query_rewards.py
--rw-rw-r--   0 root         (0) root         (0)    10072 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/reward/update_reward.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:41:42.575945 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/season/
--rw-rw-r--   0 root         (0) root         (0)     1863 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/season/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7739 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/season/bulk_get_user_season_pr_a15d63.py
--rw-rw-r--   0 root         (0) root         (0)     8704 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/season/check_season_purchasable.py
--rw-rw-r--   0 root         (0) root         (0)     8615 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/season/clone_season.py
--rw-rw-r--   0 root         (0) root         (0)     8218 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/season/create_season.py
--rw-rw-r--   0 root         (0) root         (0)     7194 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/season/delete_season.py
--rw-rw-r--   0 root         (0) root         (0)     8190 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/season/exists_any_pass_by_pass_codes.py
--rw-rw-r--   0 root         (0) root         (0)     6180 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/season/get_current_season.py
--rw-rw-r--   0 root         (0) root         (0)     7319 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/season/get_current_user_season_eed4c8.py
--rw-rw-r--   0 root         (0) root         (0)     7120 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/season/get_full_season.py
--rw-rw-r--   0 root         (0) root         (0)     7026 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/season/get_season.py
--rw-rw-r--   0 root         (0) root         (0)     8751 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/season/get_user_participated_seasons.py
--rw-rw-r--   0 root         (0) root         (0)     7902 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/season/get_user_season.py
--rw-rw-r--   0 root         (0) root         (0)     7124 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/season/public_get_current_season.py
--rw-rw-r--   0 root         (0) root         (0)     7385 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/season/public_get_current_user_season.py
--rw-rw-r--   0 root         (0) root         (0)     7934 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/season/public_get_user_season.py
--rw-rw-r--   0 root         (0) root         (0)     8891 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/season/publish_season.py
--rw-rw-r--   0 root         (0) root         (0)     9165 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/season/query_seasons.py
--rw-rw-r--   0 root         (0) root         (0)     7985 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/season/query_user_exp_grant_hi_12346c.py
--rw-rw-r--   0 root         (0) root         (0)    13220 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/season/query_user_exp_grant_history.py
--rw-rw-r--   0 root         (0) root         (0)     6748 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/season/reset_user_season.py
--rw-rw-r--   0 root         (0) root         (0)     8334 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/season/retire_season.py
--rw-rw-r--   0 root         (0) root         (0)     8393 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/season/unpublish_season.py
--rw-rw-r--   0 root         (0) root         (0)     9411 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/season/update_season.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:41:42.579944 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/tier/
--rw-rw-r--   0 root         (0) root         (0)      738 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/tier/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8880 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/tier/create_tier.py
--rw-rw-r--   0 root         (0) root         (0)     7826 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/tier/delete_tier.py
--rw-rw-r--   0 root         (0) root         (0)     8023 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/tier/grant_user_exp.py
--rw-rw-r--   0 root         (0) root         (0)     8326 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/tier/grant_user_tier.py
--rw-rw-r--   0 root         (0) root         (0)     8800 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/tier/query_tiers.py
--rw-rw-r--   0 root         (0) root         (0)     9442 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/tier/reorder_tier.py
--rw-rw-r--   0 root         (0) root         (0)     9540 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/tier/update_tier.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:41:42.579944 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/wrappers/
--rw-rw-r--   0 root         (0) root         (0)     4134 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/wrappers/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3299 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/wrappers/_export.py
--rw-rw-r--   0 root         (0) root         (0)    22664 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/wrappers/_pass_.py
--rw-rw-r--   0 root         (0) root         (0)    27251 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/wrappers/_reward.py
--rw-rw-r--   0 root         (0) root         (0)    82939 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/wrappers/_season.py
--rw-rw-r--   0 root         (0) root         (0)    26579 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/wrappers/_tier.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:41:42.579944 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk_service_seasonpass.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1137 2024-02-27 05:41:42.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk_service_seasonpass.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6812 2024-02-27 05:41:42.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk_service_seasonpass.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-27 05:41:42.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk_service_seasonpass.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       22 2024-02-27 05:41:42.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk_service_seasonpass.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-02-27 05:41:42.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk_service_seasonpass.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)      365 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-seasonpass-0.8.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-27 05:41:42.579944 accelbyte-py-sdk-service-seasonpass-0.8.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:14:23.328674 accelbyte-py-sdk-service-seasonpass-0.9.0/
+-rw-r--r--   0 root         (0) root         (0)     1137 2024-03-13 06:14:23.328674 accelbyte-py-sdk-service-seasonpass-0.9.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      879 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:14:23.316674 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:14:23.320674 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:14:23.320674 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/
+-rw-rw-r--   0 root         (0) root         (0)     4304 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:14:23.324674 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/
+-rw-rw-r--   0 root         (0) root         (0)     3332 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3968 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/bulk_user_progression_request.py
+-rw-rw-r--   0 root         (0) root         (0)     5036 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/claimable_rewards.py
+-rw-rw-r--   0 root         (0) root         (0)    17655 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/claimable_user_season_info.py
+-rw-rw-r--   0 root         (0) root         (0)     6324 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/error_entity.py
+-rw-rw-r--   0 root         (0) root         (0)     5585 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/excess_strategy.py
+-rw-rw-r--   0 root         (0) root         (0)     8726 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/exp_grant_history_info.py
+-rw-rw-r--   0 root         (0) root         (0)     5755 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/exp_grant_history_paging_sliced_result.py
+-rw-rw-r--   0 root         (0) root         (0)     7302 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/field_validation_error.py
+-rw-rw-r--   0 root         (0) root         (0)     9606 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/full_season_info.py
+-rw-rw-r--   0 root         (0) root         (0)     6864 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/image.py
+-rw-rw-r--   0 root         (0) root         (0)    12208 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/list_season_info.py
+-rw-rw-r--   0 root         (0) root         (0)     5026 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/list_season_info_paging_sliced_result.py
+-rw-rw-r--   0 root         (0) root         (0)     9499 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/list_user_season_info.py
+-rw-rw-r--   0 root         (0) root         (0)     5788 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/list_user_season_info_paging_sliced_result.py
+-rw-rw-r--   0 root         (0) root         (0)     4412 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/localization.py
+-rw-rw-r--   0 root         (0) root         (0)    11559 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/localized_pass_info.py
+-rw-rw-r--   0 root         (0) root         (0)    17248 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/localized_season_info.py
+-rw-rw-r--   0 root         (0) root         (0)     3570 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/ownership.py
+-rw-rw-r--   0 root         (0) root         (0)     4268 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/paging.py
+-rw-rw-r--   0 root         (0) root         (0)     7844 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/pass_create.py
+-rw-rw-r--   0 root         (0) root         (0)    11150 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/pass_info.py
+-rw-rw-r--   0 root         (0) root         (0)     7460 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/pass_update.py
+-rw-rw-r--   0 root         (0) root         (0)     3696 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/reason_tags_result.py
+-rw-rw-r--   0 root         (0) root         (0)     7676 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/reward_create.py
+-rw-rw-r--   0 root         (0) root         (0)     4457 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/reward_currency.py
+-rw-rw-r--   0 root         (0) root         (0)    11825 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/reward_info.py
+-rw-rw-r--   0 root         (0) root         (0)     7972 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/reward_update.py
+-rw-rw-r--   0 root         (0) root         (0)     4812 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/season_clone_request.py
+-rw-rw-r--   0 root         (0) root         (0)    11838 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/season_create.py
+-rw-rw-r--   0 root         (0) root         (0)    17474 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/season_info.py
+-rw-rw-r--   0 root         (0) root         (0)     9452 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/season_summary.py
+-rw-rw-r--   0 root         (0) root         (0)    12238 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/season_update.py
+-rw-rw-r--   0 root         (0) root         (0)     5202 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/tier.py
+-rw-rw-r--   0 root         (0) root         (0)     5189 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/tier_create.py
+-rw-rw-r--   0 root         (0) root         (0)     4703 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/tier_input.py
+-rw-rw-r--   0 root         (0) root         (0)     5488 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/tier_paging_sliced_result.py
+-rw-rw-r--   0 root         (0) root         (0)     3707 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/tier_reorder.py
+-rw-rw-r--   0 root         (0) root         (0)     5357 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/user_exp_grant.py
+-rw-rw-r--   0 root         (0) root         (0)     4567 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/user_pass_grant.py
+-rw-rw-r--   0 root         (0) root         (0)     5474 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/user_purchasable.py
+-rw-rw-r--   0 root         (0) root         (0)     5109 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/user_reward_claim.py
+-rw-rw-r--   0 root         (0) root         (0)    12836 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/user_season_summary.py
+-rw-rw-r--   0 root         (0) root         (0)     5426 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/user_tier_grant.py
+-rw-rw-r--   0 root         (0) root         (0)     5630 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/validation_error_entity.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:14:23.324674 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/
+-rw-rw-r--   0 root         (0) root         (0)      439 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:14:23.324674 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/export/
+-rw-rw-r--   0 root         (0) root         (0)      512 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/export/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     5678 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/export/export_season.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:14:23.324674 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/pass_/
+-rw-rw-r--   0 root         (0) root         (0)      691 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/pass_/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     9231 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/pass_/create_pass.py
+-rw-rw-r--   0 root         (0) root         (0)     7981 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/pass_/delete_pass.py
+-rw-rw-r--   0 root         (0) root         (0)     7738 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/pass_/get_pass.py
+-rw-rw-r--   0 root         (0) root         (0)     8093 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/pass_/grant_user_pass.py
+-rw-rw-r--   0 root         (0) root         (0)     7064 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/pass_/query_passes.py
+-rw-rw-r--   0 root         (0) root         (0)     9946 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/pass_/update_pass.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:14:23.324674 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/reward/
+-rw-rw-r--   0 root         (0) root         (0)      797 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/reward/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     9386 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/reward/create_reward.py
+-rw-rw-r--   0 root         (0) root         (0)     8097 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/reward/delete_reward.py
+-rw-rw-r--   0 root         (0) root         (0)     7776 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/reward/get_reward.py
+-rw-rw-r--   0 root         (0) root         (0)     7339 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/reward/public_bulk_claim_user_rewards.py
+-rw-rw-r--   0 root         (0) root         (0)     8788 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/reward/public_claim_user_reward.py
+-rw-rw-r--   0 root         (0) root         (0)     7866 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/reward/query_rewards.py
+-rw-rw-r--   0 root         (0) root         (0)    10072 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/reward/update_reward.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:14:23.328674 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/season/
+-rw-rw-r--   0 root         (0) root         (0)     1863 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/season/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7739 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/season/bulk_get_user_season_pr_a15d63.py
+-rw-rw-r--   0 root         (0) root         (0)     8704 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/season/check_season_purchasable.py
+-rw-rw-r--   0 root         (0) root         (0)     8615 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/season/clone_season.py
+-rw-rw-r--   0 root         (0) root         (0)     8218 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/season/create_season.py
+-rw-rw-r--   0 root         (0) root         (0)     7194 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/season/delete_season.py
+-rw-rw-r--   0 root         (0) root         (0)     8190 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/season/exists_any_pass_by_pass_codes.py
+-rw-rw-r--   0 root         (0) root         (0)     6180 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/season/get_current_season.py
+-rw-rw-r--   0 root         (0) root         (0)     7319 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/season/get_current_user_season_eed4c8.py
+-rw-rw-r--   0 root         (0) root         (0)     7120 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/season/get_full_season.py
+-rw-rw-r--   0 root         (0) root         (0)     7026 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/season/get_season.py
+-rw-rw-r--   0 root         (0) root         (0)     8751 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/season/get_user_participated_seasons.py
+-rw-rw-r--   0 root         (0) root         (0)     7902 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/season/get_user_season.py
+-rw-rw-r--   0 root         (0) root         (0)     7124 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/season/public_get_current_season.py
+-rw-rw-r--   0 root         (0) root         (0)     7385 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/season/public_get_current_user_season.py
+-rw-rw-r--   0 root         (0) root         (0)     7934 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/season/public_get_user_season.py
+-rw-rw-r--   0 root         (0) root         (0)     8891 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/season/publish_season.py
+-rw-rw-r--   0 root         (0) root         (0)     9165 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/season/query_seasons.py
+-rw-rw-r--   0 root         (0) root         (0)     7985 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/season/query_user_exp_grant_hi_12346c.py
+-rw-rw-r--   0 root         (0) root         (0)    13220 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/season/query_user_exp_grant_history.py
+-rw-rw-r--   0 root         (0) root         (0)     6748 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/season/reset_user_season.py
+-rw-rw-r--   0 root         (0) root         (0)     8334 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/season/retire_season.py
+-rw-rw-r--   0 root         (0) root         (0)     8393 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/season/unpublish_season.py
+-rw-rw-r--   0 root         (0) root         (0)     9411 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/season/update_season.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:14:23.328674 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/tier/
+-rw-rw-r--   0 root         (0) root         (0)      738 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/tier/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8880 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/tier/create_tier.py
+-rw-rw-r--   0 root         (0) root         (0)     7826 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/tier/delete_tier.py
+-rw-rw-r--   0 root         (0) root         (0)     8023 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/tier/grant_user_exp.py
+-rw-rw-r--   0 root         (0) root         (0)     8326 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/tier/grant_user_tier.py
+-rw-rw-r--   0 root         (0) root         (0)     8800 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/tier/query_tiers.py
+-rw-rw-r--   0 root         (0) root         (0)     9442 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/tier/reorder_tier.py
+-rw-rw-r--   0 root         (0) root         (0)     9540 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/tier/update_tier.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:14:23.328674 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/wrappers/
+-rw-rw-r--   0 root         (0) root         (0)     4134 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/wrappers/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3299 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/wrappers/_export.py
+-rw-rw-r--   0 root         (0) root         (0)    22664 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/wrappers/_pass_.py
+-rw-rw-r--   0 root         (0) root         (0)    27251 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/wrappers/_reward.py
+-rw-rw-r--   0 root         (0) root         (0)    82939 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/wrappers/_season.py
+-rw-rw-r--   0 root         (0) root         (0)    26579 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/wrappers/_tier.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:14:23.328674 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk_service_seasonpass.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1137 2024-03-13 06:14:23.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk_service_seasonpass.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6812 2024-03-13 06:14:23.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk_service_seasonpass.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-03-13 06:14:23.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk_service_seasonpass.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-03-13 06:14:23.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk_service_seasonpass.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-03-13 06:14:23.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk_service_seasonpass.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)      365 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-seasonpass-0.9.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-03-13 06:14:23.328674 accelbyte-py-sdk-service-seasonpass-0.9.0/setup.cfg
```

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/PKG-INFO` & `accelbyte-py-sdk-service-seasonpass-0.9.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: accelbyte-py-sdk-service-seasonpass
-Version: 0.8.0
+Version: 0.9.0
 Summary: AccelByte Python SDK - AccelByte Gaming Services Seasonpass Service
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: accelbyte-py-sdk-core
 
 [//]: # (Code generated. DO NOT EDIT!)
 
 # AccelByte Modular Python SDK - Service Module
 
 This is a service module for the [AccelByte Modular Python SDK](https://github.com/AccelByte/accelbyte-python-modular-sdk) package.
 
 ```text
 AccelByte Gaming Services Seasonpass Service
-* Version: 1.21.2
+* Version: 1.21.3
 ```
 
 ## Setup
 
 This SDK requires Python 3.9 to be installed.
 
 ### Install with Pip
```

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/README.md` & `accelbyte-py-sdk-service-seasonpass-0.9.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # AccelByte Modular Python SDK - Service Module
 
 This is a service module for the [AccelByte Modular Python SDK](https://github.com/AccelByte/accelbyte-python-modular-sdk) package.
 
 ```text
 AccelByte Gaming Services Seasonpass Service
-* Version: 1.21.2
+* Version: 1.21.3
 ```
 
 ## Setup
 
 This SDK requires Python 3.9 to be installed.
 
 ### Install with Pip
```

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/__init__.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: service-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Seasonpass Service."""
 
-__version__ = "1.21.2"
+__version__ = "1.21.3"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 # export
 from .wrappers import export_season
```

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/__init__.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: model-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Seasonpass Service."""
 
-__version__ = "1.21.2"
+__version__ = "1.21.3"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .bulk_user_progression_request import BulkUserProgressionRequest
 from .claimable_rewards import ClaimableRewards
```

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/bulk_user_progression_request.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/bulk_user_progression_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/claimable_rewards.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/claimable_rewards.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/claimable_user_season_info.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/claimable_user_season_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/error_entity.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/error_entity.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/excess_strategy.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/excess_strategy.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/exp_grant_history_info.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/exp_grant_history_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/exp_grant_history_paging_sliced_result.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/exp_grant_history_paging_sliced_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/field_validation_error.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/field_validation_error.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/full_season_info.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/full_season_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/image.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/image.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/list_season_info.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/list_season_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/list_season_info_paging_sliced_result.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/list_season_info_paging_sliced_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/list_user_season_info.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/list_user_season_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/list_user_season_info_paging_sliced_result.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/list_user_season_info_paging_sliced_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/localization.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/localization.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/localized_pass_info.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/localized_pass_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/localized_season_info.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/localized_season_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/ownership.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/ownership.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/paging.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/paging.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/pass_create.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/pass_create.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/pass_info.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/pass_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/pass_update.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/pass_update.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/reason_tags_result.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/reason_tags_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/reward_create.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/reward_create.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/reward_currency.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/reward_currency.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/reward_info.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/reward_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/reward_update.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/reward_update.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/season_clone_request.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/season_clone_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/season_create.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/season_create.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/season_info.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/season_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/season_summary.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/season_summary.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/season_update.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/season_update.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/tier.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/tier.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/tier_create.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/tier_create.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/tier_input.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/tier_input.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/tier_paging_sliced_result.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/tier_paging_sliced_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/tier_reorder.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/tier_reorder.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/user_exp_grant.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/user_exp_grant.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/user_pass_grant.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/user_pass_grant.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/user_purchasable.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/user_purchasable.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/user_reward_claim.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/user_reward_claim.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/user_season_summary.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/user_season_summary.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/user_tier_grant.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/user_tier_grant.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/models/validation_error_entity.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/models/validation_error_entity.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/export/__init__.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/export/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,14 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Seasonpass Service."""
 
-__version__ = "1.21.2"
+__version__ = "1.21.3"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .export_season import ExportSeason
```

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/export/export_season.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/export/export_season.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/pass_/__init__.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/pass_/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Seasonpass Service."""
 
-__version__ = "1.21.2"
+__version__ = "1.21.3"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .create_pass import CreatePass
 from .delete_pass import DeletePass
```

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/pass_/create_pass.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/pass_/create_pass.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/pass_/delete_pass.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/pass_/delete_pass.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/pass_/get_pass.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/pass_/get_pass.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/pass_/grant_user_pass.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/pass_/grant_user_pass.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/pass_/query_passes.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/pass_/query_passes.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/pass_/update_pass.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/pass_/update_pass.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/reward/__init__.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/reward/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Seasonpass Service."""
 
-__version__ = "1.21.2"
+__version__ = "1.21.3"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .create_reward import CreateReward
 from .delete_reward import DeleteReward
```

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/reward/create_reward.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/reward/create_reward.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/reward/delete_reward.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/reward/delete_reward.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/reward/get_reward.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/reward/get_reward.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/reward/public_bulk_claim_user_rewards.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/reward/public_bulk_claim_user_rewards.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/reward/public_claim_user_reward.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/reward/public_claim_user_reward.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/reward/query_rewards.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/reward/query_rewards.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/reward/update_reward.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/reward/update_reward.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/season/__init__.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/season/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Seasonpass Service."""
 
-__version__ = "1.21.2"
+__version__ = "1.21.3"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .bulk_get_user_season_pr_a15d63 import BulkGetUserSeasonProgression
 from .check_season_purchasable import CheckSeasonPurchasable
```

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/season/bulk_get_user_season_pr_a15d63.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/season/bulk_get_user_season_pr_a15d63.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/season/check_season_purchasable.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/season/check_season_purchasable.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/season/clone_season.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/season/clone_season.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/season/create_season.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/season/create_season.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/season/delete_season.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/season/delete_season.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/season/exists_any_pass_by_pass_codes.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/season/exists_any_pass_by_pass_codes.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/season/get_current_season.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/season/get_current_season.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/season/get_current_user_season_eed4c8.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/season/get_current_user_season_eed4c8.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/season/get_full_season.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/season/get_full_season.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/season/get_season.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/season/get_season.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/season/get_user_participated_seasons.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/season/get_user_participated_seasons.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/season/get_user_season.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/season/get_user_season.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/season/public_get_current_season.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/season/public_get_current_season.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/season/public_get_current_user_season.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/season/public_get_current_user_season.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/season/public_get_user_season.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/season/public_get_user_season.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/season/publish_season.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/season/publish_season.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/season/query_seasons.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/season/query_seasons.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/season/query_user_exp_grant_hi_12346c.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/season/query_user_exp_grant_hi_12346c.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/season/query_user_exp_grant_history.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/season/query_user_exp_grant_history.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/season/reset_user_season.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/season/reset_user_season.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/season/retire_season.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/season/retire_season.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/season/unpublish_season.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/season/unpublish_season.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/season/update_season.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/season/update_season.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/tier/__init__.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/tier/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Seasonpass Service."""
 
-__version__ = "1.21.2"
+__version__ = "1.21.3"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .create_tier import CreateTier
 from .delete_tier import DeleteTier
```

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/tier/create_tier.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/tier/create_tier.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/tier/delete_tier.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/tier/delete_tier.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/tier/grant_user_exp.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/tier/grant_user_exp.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/tier/grant_user_tier.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/tier/grant_user_tier.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/tier/query_tiers.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/tier/query_tiers.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/tier/reorder_tier.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/tier/reorder_tier.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/operations/tier/update_tier.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/operations/tier/update_tier.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/wrappers/__init__.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/wrappers/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: wrapper-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Seasonpass Service."""
 
-__version__ = "1.21.2"
+__version__ = "1.21.3"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from ._export import export_season
 from ._export import export_season_async
```

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/wrappers/_export.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/wrappers/_export.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/wrappers/_pass_.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/wrappers/_pass_.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/wrappers/_reward.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/wrappers/_reward.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/wrappers/_season.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/wrappers/_season.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk/api/seasonpass/wrappers/_tier.py` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk/api/seasonpass/wrappers/_tier.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk_service_seasonpass.egg-info/PKG-INFO` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk_service_seasonpass.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: accelbyte-py-sdk-service-seasonpass
-Version: 0.8.0
+Version: 0.9.0
 Summary: AccelByte Python SDK - AccelByte Gaming Services Seasonpass Service
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: accelbyte-py-sdk-core
 
 [//]: # (Code generated. DO NOT EDIT!)
 
 # AccelByte Modular Python SDK - Service Module
 
 This is a service module for the [AccelByte Modular Python SDK](https://github.com/AccelByte/accelbyte-python-modular-sdk) package.
 
 ```text
 AccelByte Gaming Services Seasonpass Service
-* Version: 1.21.2
+* Version: 1.21.3
 ```
 
 ## Setup
 
 This SDK requires Python 3.9 to be installed.
 
 ### Install with Pip
```

### Comparing `accelbyte-py-sdk-service-seasonpass-0.8.0/accelbyte_py_sdk_service_seasonpass.egg-info/SOURCES.txt` & `accelbyte-py-sdk-service-seasonpass-0.9.0/accelbyte_py_sdk_service_seasonpass.egg-info/SOURCES.txt`

 * *Files identical despite different names*

