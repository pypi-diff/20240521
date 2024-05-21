# Comparing `tmp/vantage_sdk-0.8.0.tar.gz` & `tmp/vantage_sdk-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vantage_sdk-0.8.0.tar", max compression
+gzip compressed data, was "vantage_sdk-0.8.1.tar", max compression
```

## Comparing `vantage_sdk-0.8.0.tar` & `vantage_sdk-0.8.1.tar`

### file list

```diff
@@ -1,77 +1,81 @@
--rw-r--r--   0        0        0    11357 2024-01-22 15:20:18.752197 vantage_sdk-0.8.0/LICENSE
--rw-r--r--   0        0        0     3974 2024-05-14 15:00:04.643283 vantage_sdk-0.8.0/README.md
--rw-r--r--   0        0        0     2924 2024-05-14 15:00:04.643589 vantage_sdk-0.8.0/pyproject.toml
--rw-r--r--   0        0        0       41 2024-01-22 15:20:18.753683 vantage_sdk-0.8.0/tests/__init__.py
--rw-r--r--   0        0        0    70399 2024-04-25 01:26:48.217409 vantage_sdk-0.8.0/tests/data/documents.jsonl
--rw-r--r--   0        0        0     2971 2024-04-25 01:26:48.217491 vantage_sdk-0.8.0/tests/data/hello_world.parquet
--rw-r--r--   0        0        0      777 2024-04-25 01:26:48.217595 vantage_sdk-0.8.0/tests/integration_tests/.env-example
--rw-r--r--   0        0        0        0 2024-01-26 19:13:09.644916 vantage_sdk-0.8.0/tests/integration_tests/__init__.py
--rw-r--r--   0        0        0    10571 2024-05-14 15:00:04.643899 vantage_sdk-0.8.0/tests/integration_tests/conftest.py
--rw-r--r--   0        0        0     3027 2024-04-25 01:26:48.217838 vantage_sdk-0.8.0/tests/integration_tests/test_account.py
--rw-r--r--   0        0        0    10983 2024-04-25 01:26:48.217894 vantage_sdk-0.8.0/tests/integration_tests/test_api_keys.py
--rw-r--r--   0        0        0    12709 2024-05-14 15:00:04.644178 vantage_sdk-0.8.0/tests/integration_tests/test_collection.py
--rw-r--r--   0        0        0     4219 2024-05-14 15:00:04.644424 vantage_sdk-0.8.0/tests/integration_tests/test_documents.py
--rw-r--r--   0        0        0     9132 2024-04-25 01:26:48.218158 vantage_sdk-0.8.0/tests/integration_tests/test_search.py
--rw-r--r--   0        0        0      671 2024-05-14 15:00:04.644679 vantage_sdk-0.8.0/vantage_sdk/__init__.py
--rw-r--r--   0        0        0    66114 2024-05-14 15:00:04.645142 vantage_sdk-0.8.0/vantage_sdk/client.py
--rw-r--r--   0        0        0      239 2024-05-14 15:00:04.645361 vantage_sdk-0.8.0/vantage_sdk/config.py
--rw-r--r--   0        0        0       43 2024-04-25 01:26:48.218648 vantage_sdk-0.8.0/vantage_sdk/core/__init__.py
--rw-r--r--   0        0        0     6471 2024-04-25 01:26:48.218733 vantage_sdk-0.8.0/vantage_sdk/core/base.py
--rw-r--r--   0        0        0     1628 2024-04-25 01:26:48.218805 vantage_sdk-0.8.0/vantage_sdk/core/exceptions.py
--rw-r--r--   0        0        0     4268 2024-05-14 15:00:04.645589 vantage_sdk-0.8.0/vantage_sdk/core/http/__init__.py
--rw-r--r--   0        0        0      515 2024-04-25 01:26:48.219014 vantage_sdk-0.8.0/vantage_sdk/core/http/api/__init__.py
--rw-r--r--   0        0        0    22934 2024-04-25 01:26:48.219174 vantage_sdk-0.8.0/vantage_sdk/core/http/api/account_management_api.py
--rw-r--r--   0        0        0    75134 2024-05-14 15:00:04.645955 vantage_sdk-0.8.0/vantage_sdk/core/http/api/collection_management_api.py
--rw-r--r--   0        0        0    15180 2024-04-25 01:26:48.219450 vantage_sdk-0.8.0/vantage_sdk/core/http/api/documents_api.py
--rw-r--r--   0        0        0    57753 2024-05-14 15:00:04.646292 vantage_sdk-0.8.0/vantage_sdk/core/http/api/external_api_keys_api.py
--rw-r--r--   0        0        0    54428 2024-04-25 01:26:48.219739 vantage_sdk-0.8.0/vantage_sdk/core/http/api/search_api.py
--rw-r--r--   0        0        0    22624 2024-05-14 15:00:04.646500 vantage_sdk-0.8.0/vantage_sdk/core/http/api/vantage_api_keys_api.py
--rw-r--r--   0        0        0    24948 2024-04-25 01:26:48.219980 vantage_sdk-0.8.0/vantage_sdk/core/http/api_client.py
--rw-r--r--   0        0        0      678 2024-04-25 01:26:48.220043 vantage_sdk-0.8.0/vantage_sdk/core/http/api_response.py
--rw-r--r--   0        0        0    15524 2024-04-25 01:26:48.220150 vantage_sdk-0.8.0/vantage_sdk/core/http/configuration.py
--rw-r--r--   0        0        0     6369 2024-04-25 01:26:48.220244 vantage_sdk-0.8.0/vantage_sdk/core/http/exceptions.py
--rw-r--r--   0        0        0     3384 2024-05-14 15:00:04.646724 vantage_sdk-0.8.0/vantage_sdk/core/http/models/__init__.py
--rw-r--r--   0        0        0     2951 2024-04-25 01:26:48.220414 vantage_sdk-0.8.0/vantage_sdk/core/http/models/account.py
--rw-r--r--   0        0        0     2735 2024-04-25 01:26:48.220567 vantage_sdk-0.8.0/vantage_sdk/core/http/models/account_modifiable.py
--rw-r--r--   0        0        0     2812 2024-04-25 01:26:48.220678 vantage_sdk-0.8.0/vantage_sdk/core/http/models/account_read_only.py
--rw-r--r--   0        0        0     7946 2024-05-14 15:00:04.646949 vantage_sdk-0.8.0/vantage_sdk/core/http/models/collection.py
--rw-r--r--   0        0        0     4615 2024-04-25 01:26:48.220877 vantage_sdk-0.8.0/vantage_sdk/core/http/models/collection_immutable.py
--rw-r--r--   0        0        0     4445 2024-05-14 15:00:04.647162 vantage_sdk-0.8.0/vantage_sdk/core/http/models/collection_modifiable.py
--rw-r--r--   0        0        0     4316 2024-04-25 01:26:48.221041 vantage_sdk-0.8.0/vantage_sdk/core/http/models/collection_read_only.py
--rw-r--r--   0        0        0     3698 2024-04-25 01:26:48.221096 vantage_sdk-0.8.0/vantage_sdk/core/http/models/collection_upload_url.py
--rw-r--r--   0        0        0     6297 2024-05-14 15:00:04.647434 vantage_sdk-0.8.0/vantage_sdk/core/http/models/create_collection_request.py
--rw-r--r--   0        0        0     2962 2024-04-25 01:26:48.221270 vantage_sdk-0.8.0/vantage_sdk/core/http/models/document_batch.py
--rw-r--r--   0        0        0     5971 2024-04-25 01:26:48.221347 vantage_sdk-0.8.0/vantage_sdk/core/http/models/embedding_search_query.py
--rw-r--r--   0        0        0     4350 2024-04-25 01:26:48.221399 vantage_sdk-0.8.0/vantage_sdk/core/http/models/external_api_key.py
--rw-r--r--   0        0        0     3383 2024-04-25 01:26:48.221449 vantage_sdk-0.8.0/vantage_sdk/core/http/models/external_api_key_modifiable.py
--rw-r--r--   0        0        0     3673 2024-04-25 01:26:48.221506 vantage_sdk-0.8.0/vantage_sdk/core/http/models/external_api_key_read_only.py
--rw-r--r--   0        0        0     5819 2024-04-25 01:26:48.221570 vantage_sdk-0.8.0/vantage_sdk/core/http/models/global_search_properties.py
--rw-r--r--   0        0        0     3146 2024-04-25 01:26:48.221626 vantage_sdk-0.8.0/vantage_sdk/core/http/models/global_search_properties_collection.py
--rw-r--r--   0        0        0     4596 2024-04-25 01:26:48.221687 vantage_sdk-0.8.0/vantage_sdk/core/http/models/global_search_properties_field_value_weighting.py
--rw-r--r--   0        0        0     2809 2024-04-25 01:26:48.221743 vantage_sdk-0.8.0/vantage_sdk/core/http/models/global_search_properties_filter.py
--rw-r--r--   0        0        0     2859 2024-04-25 01:26:48.221799 vantage_sdk-0.8.0/vantage_sdk/core/http/models/global_search_properties_pagination.py
--rw-r--r--   0        0        0     3657 2024-04-25 01:26:48.221873 vantage_sdk-0.8.0/vantage_sdk/core/http/models/global_search_properties_sort.py
--rw-r--r--   0        0        0     3282 2024-04-25 01:26:48.221935 vantage_sdk-0.8.0/vantage_sdk/core/http/models/ml_these.py
--rw-r--r--   0        0        0     3326 2024-04-25 01:26:48.221996 vantage_sdk-0.8.0/vantage_sdk/core/http/models/ml_these_these_inner.py
--rw-r--r--   0        0        0     6474 2024-04-25 01:26:48.222076 vantage_sdk-0.8.0/vantage_sdk/core/http/models/more_like_these_query.py
--rw-r--r--   0        0        0     5932 2024-04-25 01:26:48.222130 vantage_sdk-0.8.0/vantage_sdk/core/http/models/more_like_this_query.py
--rw-r--r--   0        0        0     3721 2024-04-25 01:26:48.222195 vantage_sdk-0.8.0/vantage_sdk/core/http/models/search_result.py
--rw-r--r--   0        0        0     2870 2024-04-25 01:26:48.222242 vantage_sdk-0.8.0/vantage_sdk/core/http/models/search_result_results_inner.py
--rw-r--r--   0        0        0     3445 2024-05-14 15:00:04.647571 vantage_sdk-0.8.0/vantage_sdk/core/http/models/secondary_external_account.py
--rw-r--r--   0        0        0     5912 2024-04-25 01:26:48.222361 vantage_sdk-0.8.0/vantage_sdk/core/http/models/semantic_search_query.py
--rw-r--r--   0        0        0     4093 2024-04-25 01:26:48.222442 vantage_sdk-0.8.0/vantage_sdk/core/http/models/vantage_api_key.py
--rw-r--r--   0        0        0     3003 2024-04-25 01:26:48.222499 vantage_sdk-0.8.0/vantage_sdk/core/http/models/weighted_field_values.py
--rw-r--r--   0        0        0        0 2024-04-25 01:26:48.222520 vantage_sdk-0.8.0/vantage_sdk/core/http/py.typed
--rw-r--r--   0        0        0    10169 2024-04-25 01:26:48.222607 vantage_sdk-0.8.0/vantage_sdk/core/http/rest.py
--rw-r--r--   0        0        0       95 2024-04-25 01:26:48.222695 vantage_sdk-0.8.0/vantage_sdk/core/management/__init__.py
--rw-r--r--   0        0        0     1727 2024-04-25 01:26:48.222760 vantage_sdk-0.8.0/vantage_sdk/core/management/management.py
--rw-r--r--   0        0        0       79 2024-04-25 01:26:48.222849 vantage_sdk-0.8.0/vantage_sdk/core/search/__init__.py
--rw-r--r--   0        0        0      232 2024-04-25 01:26:48.222901 vantage_sdk-0.8.0/vantage_sdk/core/search/search.py
--rw-r--r--   0        0        0      559 2024-04-25 01:26:48.222952 vantage_sdk-0.8.0/vantage_sdk/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-25 01:26:48.223004 vantage_sdk-0.8.0/vantage_sdk/model/__init__.py
--rw-r--r--   0        0        0      187 2024-04-25 01:26:48.223071 vantage_sdk-0.8.0/vantage_sdk/model/account.py
--rw-r--r--   0        0        0     2563 2024-05-14 15:00:04.647772 vantage_sdk-0.8.0/vantage_sdk/model/collection.py
--rw-r--r--   0        0        0     1670 2024-05-14 15:00:04.647963 vantage_sdk-0.8.0/vantage_sdk/model/document.py
--rw-r--r--   0        0        0      910 2024-05-14 15:00:04.648235 vantage_sdk-0.8.0/vantage_sdk/model/keys.py
--rw-r--r--   0        0        0     1193 2024-04-25 01:26:48.223288 vantage_sdk-0.8.0/vantage_sdk/model/search.py
--rw-r--r--   0        0        0     6018 1970-01-01 00:00:00.000000 vantage_sdk-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-01-22 15:20:18.752197 vantage_sdk-0.8.1/LICENSE
+-rw-r--r--   0        0        0     3974 2024-05-14 15:00:04.643283 vantage_sdk-0.8.1/README.md
+-rw-r--r--   0        0        0     2551 2024-05-21 16:24:37.163466 vantage_sdk-0.8.1/docs/api.md
+-rw-r--r--   0        0        0        9 2024-05-21 16:24:37.163636 vantage_sdk-0.8.1/docs/index.md
+-rw-r--r--   0        0        0        9 2024-05-21 16:24:37.163767 vantage_sdk-0.8.1/docs/installation.md
+-rw-r--r--   0        0        0        9 2024-05-21 16:24:37.163900 vantage_sdk-0.8.1/docs/usage.md
+-rw-r--r--   0        0        0     3017 2024-05-21 16:24:37.166299 vantage_sdk-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0       41 2024-01-22 15:20:18.753683 vantage_sdk-0.8.1/tests/__init__.py
+-rw-r--r--   0        0        0    70399 2024-04-25 01:26:48.217409 vantage_sdk-0.8.1/tests/data/documents.jsonl
+-rw-r--r--   0        0        0     2971 2024-04-25 01:26:48.217491 vantage_sdk-0.8.1/tests/data/hello_world.parquet
+-rw-r--r--   0        0        0      777 2024-04-25 01:26:48.217595 vantage_sdk-0.8.1/tests/integration_tests/.env-example
+-rw-r--r--   0        0        0        0 2024-01-26 19:13:09.644916 vantage_sdk-0.8.1/tests/integration_tests/__init__.py
+-rw-r--r--   0        0        0    10571 2024-05-14 15:00:04.643899 vantage_sdk-0.8.1/tests/integration_tests/conftest.py
+-rw-r--r--   0        0        0     3027 2024-04-25 01:26:48.217838 vantage_sdk-0.8.1/tests/integration_tests/test_account.py
+-rw-r--r--   0        0        0    10983 2024-04-25 01:26:48.217894 vantage_sdk-0.8.1/tests/integration_tests/test_api_keys.py
+-rw-r--r--   0        0        0    12709 2024-05-14 15:00:04.644178 vantage_sdk-0.8.1/tests/integration_tests/test_collection.py
+-rw-r--r--   0        0        0     4219 2024-05-14 15:00:04.644424 vantage_sdk-0.8.1/tests/integration_tests/test_documents.py
+-rw-r--r--   0        0        0     9132 2024-04-25 01:26:48.218158 vantage_sdk-0.8.1/tests/integration_tests/test_search.py
+-rw-r--r--   0        0        0      671 2024-05-21 16:24:37.166553 vantage_sdk-0.8.1/vantage_sdk/__init__.py
+-rw-r--r--   0        0        0    66145 2024-05-21 16:24:37.167025 vantage_sdk-0.8.1/vantage_sdk/client.py
+-rw-r--r--   0        0        0      239 2024-05-14 15:00:04.645361 vantage_sdk-0.8.1/vantage_sdk/config.py
+-rw-r--r--   0        0        0       43 2024-04-25 01:26:48.218648 vantage_sdk-0.8.1/vantage_sdk/core/__init__.py
+-rw-r--r--   0        0        0     6471 2024-04-25 01:26:48.218733 vantage_sdk-0.8.1/vantage_sdk/core/base.py
+-rw-r--r--   0        0        0     1628 2024-04-25 01:26:48.218805 vantage_sdk-0.8.1/vantage_sdk/core/exceptions.py
+-rw-r--r--   0        0        0     4268 2024-05-14 15:00:04.645589 vantage_sdk-0.8.1/vantage_sdk/core/http/__init__.py
+-rw-r--r--   0        0        0      515 2024-04-25 01:26:48.219014 vantage_sdk-0.8.1/vantage_sdk/core/http/api/__init__.py
+-rw-r--r--   0        0        0    22934 2024-04-25 01:26:48.219174 vantage_sdk-0.8.1/vantage_sdk/core/http/api/account_management_api.py
+-rw-r--r--   0        0        0    75134 2024-05-14 15:00:04.645955 vantage_sdk-0.8.1/vantage_sdk/core/http/api/collection_management_api.py
+-rw-r--r--   0        0        0    15180 2024-04-25 01:26:48.219450 vantage_sdk-0.8.1/vantage_sdk/core/http/api/documents_api.py
+-rw-r--r--   0        0        0    57753 2024-05-14 15:00:04.646292 vantage_sdk-0.8.1/vantage_sdk/core/http/api/external_api_keys_api.py
+-rw-r--r--   0        0        0    54428 2024-04-25 01:26:48.219739 vantage_sdk-0.8.1/vantage_sdk/core/http/api/search_api.py
+-rw-r--r--   0        0        0    22624 2024-05-14 15:00:04.646500 vantage_sdk-0.8.1/vantage_sdk/core/http/api/vantage_api_keys_api.py
+-rw-r--r--   0        0        0    24948 2024-04-25 01:26:48.219980 vantage_sdk-0.8.1/vantage_sdk/core/http/api_client.py
+-rw-r--r--   0        0        0      678 2024-04-25 01:26:48.220043 vantage_sdk-0.8.1/vantage_sdk/core/http/api_response.py
+-rw-r--r--   0        0        0    15524 2024-04-25 01:26:48.220150 vantage_sdk-0.8.1/vantage_sdk/core/http/configuration.py
+-rw-r--r--   0        0        0     6369 2024-04-25 01:26:48.220244 vantage_sdk-0.8.1/vantage_sdk/core/http/exceptions.py
+-rw-r--r--   0        0        0     3384 2024-05-14 15:00:04.646724 vantage_sdk-0.8.1/vantage_sdk/core/http/models/__init__.py
+-rw-r--r--   0        0        0     2951 2024-04-25 01:26:48.220414 vantage_sdk-0.8.1/vantage_sdk/core/http/models/account.py
+-rw-r--r--   0        0        0     2735 2024-04-25 01:26:48.220567 vantage_sdk-0.8.1/vantage_sdk/core/http/models/account_modifiable.py
+-rw-r--r--   0        0        0     2812 2024-04-25 01:26:48.220678 vantage_sdk-0.8.1/vantage_sdk/core/http/models/account_read_only.py
+-rw-r--r--   0        0        0     7946 2024-05-14 15:00:04.646949 vantage_sdk-0.8.1/vantage_sdk/core/http/models/collection.py
+-rw-r--r--   0        0        0     4615 2024-04-25 01:26:48.220877 vantage_sdk-0.8.1/vantage_sdk/core/http/models/collection_immutable.py
+-rw-r--r--   0        0        0     4445 2024-05-14 15:00:04.647162 vantage_sdk-0.8.1/vantage_sdk/core/http/models/collection_modifiable.py
+-rw-r--r--   0        0        0     4316 2024-04-25 01:26:48.221041 vantage_sdk-0.8.1/vantage_sdk/core/http/models/collection_read_only.py
+-rw-r--r--   0        0        0     3698 2024-04-25 01:26:48.221096 vantage_sdk-0.8.1/vantage_sdk/core/http/models/collection_upload_url.py
+-rw-r--r--   0        0        0     6297 2024-05-14 15:00:04.647434 vantage_sdk-0.8.1/vantage_sdk/core/http/models/create_collection_request.py
+-rw-r--r--   0        0        0     2962 2024-04-25 01:26:48.221270 vantage_sdk-0.8.1/vantage_sdk/core/http/models/document_batch.py
+-rw-r--r--   0        0        0     5971 2024-04-25 01:26:48.221347 vantage_sdk-0.8.1/vantage_sdk/core/http/models/embedding_search_query.py
+-rw-r--r--   0        0        0     4350 2024-04-25 01:26:48.221399 vantage_sdk-0.8.1/vantage_sdk/core/http/models/external_api_key.py
+-rw-r--r--   0        0        0     3383 2024-04-25 01:26:48.221449 vantage_sdk-0.8.1/vantage_sdk/core/http/models/external_api_key_modifiable.py
+-rw-r--r--   0        0        0     3673 2024-04-25 01:26:48.221506 vantage_sdk-0.8.1/vantage_sdk/core/http/models/external_api_key_read_only.py
+-rw-r--r--   0        0        0     5819 2024-04-25 01:26:48.221570 vantage_sdk-0.8.1/vantage_sdk/core/http/models/global_search_properties.py
+-rw-r--r--   0        0        0     3146 2024-04-25 01:26:48.221626 vantage_sdk-0.8.1/vantage_sdk/core/http/models/global_search_properties_collection.py
+-rw-r--r--   0        0        0     4596 2024-04-25 01:26:48.221687 vantage_sdk-0.8.1/vantage_sdk/core/http/models/global_search_properties_field_value_weighting.py
+-rw-r--r--   0        0        0     2809 2024-04-25 01:26:48.221743 vantage_sdk-0.8.1/vantage_sdk/core/http/models/global_search_properties_filter.py
+-rw-r--r--   0        0        0     2859 2024-04-25 01:26:48.221799 vantage_sdk-0.8.1/vantage_sdk/core/http/models/global_search_properties_pagination.py
+-rw-r--r--   0        0        0     3657 2024-04-25 01:26:48.221873 vantage_sdk-0.8.1/vantage_sdk/core/http/models/global_search_properties_sort.py
+-rw-r--r--   0        0        0     3282 2024-04-25 01:26:48.221935 vantage_sdk-0.8.1/vantage_sdk/core/http/models/ml_these.py
+-rw-r--r--   0        0        0     3326 2024-04-25 01:26:48.221996 vantage_sdk-0.8.1/vantage_sdk/core/http/models/ml_these_these_inner.py
+-rw-r--r--   0        0        0     6474 2024-04-25 01:26:48.222076 vantage_sdk-0.8.1/vantage_sdk/core/http/models/more_like_these_query.py
+-rw-r--r--   0        0        0     5932 2024-04-25 01:26:48.222130 vantage_sdk-0.8.1/vantage_sdk/core/http/models/more_like_this_query.py
+-rw-r--r--   0        0        0     3721 2024-04-25 01:26:48.222195 vantage_sdk-0.8.1/vantage_sdk/core/http/models/search_result.py
+-rw-r--r--   0        0        0     2870 2024-04-25 01:26:48.222242 vantage_sdk-0.8.1/vantage_sdk/core/http/models/search_result_results_inner.py
+-rw-r--r--   0        0        0     3445 2024-05-14 15:00:04.647571 vantage_sdk-0.8.1/vantage_sdk/core/http/models/secondary_external_account.py
+-rw-r--r--   0        0        0     5912 2024-04-25 01:26:48.222361 vantage_sdk-0.8.1/vantage_sdk/core/http/models/semantic_search_query.py
+-rw-r--r--   0        0        0     4093 2024-04-25 01:26:48.222442 vantage_sdk-0.8.1/vantage_sdk/core/http/models/vantage_api_key.py
+-rw-r--r--   0        0        0     3003 2024-04-25 01:26:48.222499 vantage_sdk-0.8.1/vantage_sdk/core/http/models/weighted_field_values.py
+-rw-r--r--   0        0        0        0 2024-04-25 01:26:48.222520 vantage_sdk-0.8.1/vantage_sdk/core/http/py.typed
+-rw-r--r--   0        0        0    10169 2024-04-25 01:26:48.222607 vantage_sdk-0.8.1/vantage_sdk/core/http/rest.py
+-rw-r--r--   0        0        0       95 2024-04-25 01:26:48.222695 vantage_sdk-0.8.1/vantage_sdk/core/management/__init__.py
+-rw-r--r--   0        0        0     1727 2024-04-25 01:26:48.222760 vantage_sdk-0.8.1/vantage_sdk/core/management/management.py
+-rw-r--r--   0        0        0       79 2024-04-25 01:26:48.222849 vantage_sdk-0.8.1/vantage_sdk/core/search/__init__.py
+-rw-r--r--   0        0        0      232 2024-04-25 01:26:48.222901 vantage_sdk-0.8.1/vantage_sdk/core/search/search.py
+-rw-r--r--   0        0        0      559 2024-04-25 01:26:48.222952 vantage_sdk-0.8.1/vantage_sdk/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-25 01:26:48.223004 vantage_sdk-0.8.1/vantage_sdk/model/__init__.py
+-rw-r--r--   0        0        0      187 2024-04-25 01:26:48.223071 vantage_sdk-0.8.1/vantage_sdk/model/account.py
+-rw-r--r--   0        0        0     2563 2024-05-14 15:00:04.647772 vantage_sdk-0.8.1/vantage_sdk/model/collection.py
+-rw-r--r--   0        0        0     1670 2024-05-14 15:00:04.647963 vantage_sdk-0.8.1/vantage_sdk/model/document.py
+-rw-r--r--   0        0        0      910 2024-05-14 15:00:04.648235 vantage_sdk-0.8.1/vantage_sdk/model/keys.py
+-rw-r--r--   0        0        0     1193 2024-04-25 01:26:48.223288 vantage_sdk-0.8.1/vantage_sdk/model/search.py
+-rw-r--r--   0        0        0     6150 1970-01-01 00:00:00.000000 vantage_sdk-0.8.1/PKG-INFO
```

### Comparing `vantage_sdk-0.8.0/LICENSE` & `vantage_sdk-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.0/README.md` & `vantage_sdk-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.0/pyproject.toml` & `vantage_sdk-0.8.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "vantage-sdk"
-version = "0.8.0"
+version = "0.8.1"
 description = "Vantage Python SDK."
 authors = ["Vantage <none@vantage.com>"]
 readme = "README.md"
 repository = "https://github.com/VantageDiscovery/vantage-sdk-python"
 documentation = "https://docs.vantagediscovery.com/docs/concepts"
 classifiers=[
     'Programming Language :: Python :: 3.10',
@@ -17,15 +17,15 @@
 
 include = [
     { path = "examples", format = "sdist" },
     { path = "docs", format = "sdist" },
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.10,<3.12"
+python = ">=3.10"
 pydantic = ">=2"
 black  = { version = "^23.0", optional = true}
 isort  = { version = "^5.8.0", optional = true}
 flake8  = { version = "^5.0.1", optional = true}
 requests = ">=2, <3"
 urllib3 = ">=2, <3"
 python-dateutil = ">=2, <3"
@@ -38,20 +38,22 @@
 tox  = { version = "^4.0.0", optional = true}
 virtualenv  = { version = "^20.2.2", optional = true}
 pip  = { version = "*", optional = true}
 twine  = { version = "^4.0.2", optional = true}
 pre-commit = {version = "^3.3.0", optional = true}
 toml = {version = "^0.10.2", optional = true}
 bump2version = {version = "^1.0.1", optional = true}
-mkdocs = {version = "^1.5.3", optional = true}
-mkdocs-material = {version = "^9.5.3", optional = true}
-mkdocs-include-markdown-plugin = {version = "^4.0.0", optional = true}
+mkdocs = {version = "^1.6.0", optional = true}
+mkdocs-material = {version = "^9.5.23", optional = true}
+mkdocs-include-markdown-plugin = {version = "^6.0.6", optional = true}
 python-dotenv = ">=1.0.1"
 bumpver = {version = ">=2023.1129"}
 pip-tools = {version = ">=7.3.0"}
+mkdocstrings = {version = ">=0.25.1", extras = ["python"]}
+griffe-fieldz = {version = ">= 0.1.2"}
 
 [tool.poetry.extras]
 test = [
     "pytest",
     "black",
     "isort",
     "mypy",
@@ -114,15 +116,15 @@
     "D107"
 ]
 
 [tool.mypy]
 exclude = "vantage_sdk/core/http"
 
 [bumpver]
-current_version = "0.8.0"
+current_version = "0.8.1"
 version_pattern = "MAJOR.MINOR.PATCH"
 
 [bumpver.file_patterns]
 "pyproject.toml" = [
     'version = "{version}"',
 ]
 "vantage_sdk/__init__.py" = [
```

### Comparing `vantage_sdk-0.8.0/tests/data/documents.jsonl` & `vantage_sdk-0.8.1/tests/data/documents.jsonl`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.0/tests/data/hello_world.parquet` & `vantage_sdk-0.8.1/tests/data/hello_world.parquet`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.0/tests/integration_tests/.env-example` & `vantage_sdk-0.8.1/tests/integration_tests/.env-example`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.0/tests/integration_tests/conftest.py` & `vantage_sdk-0.8.1/tests/integration_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.0/tests/integration_tests/test_account.py` & `vantage_sdk-0.8.1/tests/integration_tests/test_account.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.0/tests/integration_tests/test_api_keys.py` & `vantage_sdk-0.8.1/tests/integration_tests/test_api_keys.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.0/tests/integration_tests/test_collection.py` & `vantage_sdk-0.8.1/tests/integration_tests/test_collection.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.0/tests/integration_tests/test_documents.py` & `vantage_sdk-0.8.1/tests/integration_tests/test_documents.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.0/tests/integration_tests/test_search.py` & `vantage_sdk-0.8.1/tests/integration_tests/test_search.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.0/vantage_sdk/__init__.py` & `vantage_sdk-0.8.1/vantage_sdk/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     SearchResult,
     SearchResultItem,
 )
 
 
 __author__ = """Vantage"""
 __email__ = 'none@vantage.com'
-__version__ = '0.8.0'
+__version__ = '0.8.1'
 __all__ = [
     "VantageClient",
     "Collection",
     "CollectionUploadURL",
     "Account",
     "VantageAPIKey",
     "ExternalAPIKey",
```

### Comparing `vantage_sdk-0.8.0/vantage_sdk/client.py` & `vantage_sdk-0.8.1/vantage_sdk/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -327,14 +327,16 @@
             Defaults to None.
 
         Returns
         -------
         Account
             An updated Account object reflecting the changes made.
 
+        Notes
+        --------
         Visit our [documentation](https://docs.vantagediscovery.com/docs/management-api) for more details and examples.
         """
 
         account_modifiable = AccountModifiable(account_name=account_name)
 
         result = self.management_api.account_api.update_account(
             account_id=account_id or self.account_id,
```

### Comparing `vantage_sdk-0.8.0/vantage_sdk/core/base.py` & `vantage_sdk-0.8.1/vantage_sdk/core/base.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.0/vantage_sdk/core/exceptions.py` & `vantage_sdk-0.8.1/vantage_sdk/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.0/vantage_sdk/core/http/__init__.py` & `vantage_sdk-0.8.1/vantage_sdk/core/http/__init__.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.0/vantage_sdk/core/http/api/__init__.py` & `vantage_sdk-0.8.1/vantage_sdk/core/http/api/__init__.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.0/vantage_sdk/core/http/api/account_management_api.py` & `vantage_sdk-0.8.1/vantage_sdk/core/http/api/account_management_api.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.0/vantage_sdk/core/http/api/collection_management_api.py` & `vantage_sdk-0.8.1/vantage_sdk/core/http/api/collection_management_api.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.0/vantage_sdk/core/http/api/documents_api.py` & `vantage_sdk-0.8.1/vantage_sdk/core/http/api/documents_api.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.0/vantage_sdk/core/http/api/external_api_keys_api.py` & `vantage_sdk-0.8.1/vantage_sdk/core/http/api/external_api_keys_api.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.0/vantage_sdk/core/http/api/search_api.py` & `vantage_sdk-0.8.1/vantage_sdk/core/http/api/search_api.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.0/vantage_sdk/core/http/api/vantage_api_keys_api.py` & `vantage_sdk-0.8.1/vantage_sdk/core/http/api/vantage_api_keys_api.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.0/vantage_sdk/core/http/api_client.py` & `vantage_sdk-0.8.1/vantage_sdk/core/http/api_client.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.0/vantage_sdk/core/http/api_response.py` & `vantage_sdk-0.8.1/vantage_sdk/core/http/api_response.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.0/vantage_sdk/core/http/configuration.py` & `vantage_sdk-0.8.1/vantage_sdk/core/http/configuration.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.0/vantage_sdk/core/http/exceptions.py` & `vantage_sdk-0.8.1/vantage_sdk/core/http/exceptions.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.0/vantage_sdk/core/http/models/__init__.py` & `vantage_sdk-0.8.1/vantage_sdk/core/http/models/__init__.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.0/vantage_sdk/core/http/models/account.py` & `vantage_sdk-0.8.1/vantage_sdk/core/http/models/account.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.0/vantage_sdk/core/http/models/account_modifiable.py` & `vantage_sdk-0.8.1/vantage_sdk/core/http/models/account_modifiable.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.0/vantage_sdk/core/http/models/account_read_only.py` & `vantage_sdk-0.8.1/vantage_sdk/core/http/models/account_read_only.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.0/vantage_sdk/core/http/models/collection.py` & `vantage_sdk-0.8.1/vantage_sdk/core/http/models/collection.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.0/vantage_sdk/core/http/models/collection_immutable.py` & `vantage_sdk-0.8.1/vantage_sdk/core/http/models/collection_immutable.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.0/vantage_sdk/core/http/models/collection_modifiable.py` & `vantage_sdk-0.8.1/vantage_sdk/core/http/models/collection_modifiable.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.0/vantage_sdk/core/http/models/collection_read_only.py` & `vantage_sdk-0.8.1/vantage_sdk/core/http/models/collection_read_only.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.0/vantage_sdk/core/http/models/collection_upload_url.py` & `vantage_sdk-0.8.1/vantage_sdk/core/http/models/collection_upload_url.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.0/vantage_sdk/core/http/models/create_collection_request.py` & `vantage_sdk-0.8.1/vantage_sdk/core/http/models/create_collection_request.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.0/vantage_sdk/core/http/models/document_batch.py` & `vantage_sdk-0.8.1/vantage_sdk/core/http/models/document_batch.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.0/vantage_sdk/core/http/models/embedding_search_query.py` & `vantage_sdk-0.8.1/vantage_sdk/core/http/models/embedding_search_query.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.0/vantage_sdk/core/http/models/external_api_key.py` & `vantage_sdk-0.8.1/vantage_sdk/core/http/models/external_api_key.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.0/vantage_sdk/core/http/models/external_api_key_modifiable.py` & `vantage_sdk-0.8.1/vantage_sdk/core/http/models/external_api_key_modifiable.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.0/vantage_sdk/core/http/models/external_api_key_read_only.py` & `vantage_sdk-0.8.1/vantage_sdk/core/http/models/external_api_key_read_only.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.0/vantage_sdk/core/http/models/global_search_properties.py` & `vantage_sdk-0.8.1/vantage_sdk/core/http/models/global_search_properties.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.0/vantage_sdk/core/http/models/global_search_properties_collection.py` & `vantage_sdk-0.8.1/vantage_sdk/core/http/models/global_search_properties_collection.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.0/vantage_sdk/core/http/models/global_search_properties_field_value_weighting.py` & `vantage_sdk-0.8.1/vantage_sdk/core/http/models/global_search_properties_field_value_weighting.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.0/vantage_sdk/core/http/models/global_search_properties_filter.py` & `vantage_sdk-0.8.1/vantage_sdk/core/http/models/global_search_properties_filter.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.0/vantage_sdk/core/http/models/global_search_properties_pagination.py` & `vantage_sdk-0.8.1/vantage_sdk/core/http/models/global_search_properties_pagination.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.0/vantage_sdk/core/http/models/global_search_properties_sort.py` & `vantage_sdk-0.8.1/vantage_sdk/core/http/models/global_search_properties_sort.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.0/vantage_sdk/core/http/models/ml_these.py` & `vantage_sdk-0.8.1/vantage_sdk/core/http/models/ml_these.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.0/vantage_sdk/core/http/models/ml_these_these_inner.py` & `vantage_sdk-0.8.1/vantage_sdk/core/http/models/ml_these_these_inner.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.0/vantage_sdk/core/http/models/more_like_these_query.py` & `vantage_sdk-0.8.1/vantage_sdk/core/http/models/more_like_these_query.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.0/vantage_sdk/core/http/models/more_like_this_query.py` & `vantage_sdk-0.8.1/vantage_sdk/core/http/models/more_like_this_query.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.0/vantage_sdk/core/http/models/search_result.py` & `vantage_sdk-0.8.1/vantage_sdk/core/http/models/search_result.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.0/vantage_sdk/core/http/models/search_result_results_inner.py` & `vantage_sdk-0.8.1/vantage_sdk/core/http/models/search_result_results_inner.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.0/vantage_sdk/core/http/models/secondary_external_account.py` & `vantage_sdk-0.8.1/vantage_sdk/core/http/models/secondary_external_account.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.0/vantage_sdk/core/http/models/semantic_search_query.py` & `vantage_sdk-0.8.1/vantage_sdk/core/http/models/semantic_search_query.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.0/vantage_sdk/core/http/models/vantage_api_key.py` & `vantage_sdk-0.8.1/vantage_sdk/core/http/models/vantage_api_key.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.0/vantage_sdk/core/http/models/weighted_field_values.py` & `vantage_sdk-0.8.1/vantage_sdk/core/http/models/weighted_field_values.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.0/vantage_sdk/core/http/rest.py` & `vantage_sdk-0.8.1/vantage_sdk/core/http/rest.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.0/vantage_sdk/core/management/management.py` & `vantage_sdk-0.8.1/vantage_sdk/core/management/management.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.0/vantage_sdk/exceptions.py` & `vantage_sdk-0.8.1/vantage_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.0/vantage_sdk/model/collection.py` & `vantage_sdk-0.8.1/vantage_sdk/model/collection.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.0/vantage_sdk/model/document.py` & `vantage_sdk-0.8.1/vantage_sdk/model/document.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.0/vantage_sdk/model/keys.py` & `vantage_sdk-0.8.1/vantage_sdk/model/keys.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.0/vantage_sdk/model/search.py` & `vantage_sdk-0.8.1/vantage_sdk/model/search.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.0/PKG-INFO` & `vantage_sdk-0.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 Metadata-Version: 2.1
 Name: vantage-sdk
-Version: 0.8.0
+Version: 0.8.1
 Summary: Vantage Python SDK.
 Home-page: https://github.com/VantageDiscovery/vantage-sdk-python
 Author: Vantage
 Author-email: none@vantage.com
-Requires-Python: >=3.10,<3.12
+Requires-Python: >=3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: dev
 Provides-Extra: doc
 Provides-Extra: test
 Requires-Dist: black (>=23.0,<24.0) ; extra == "test"
 Requires-Dist: bump2version (>=1.0.1,<2.0.0) ; extra == "dev"
 Requires-Dist: bumpver (>=2023.1129) ; extra == "dev"
 Requires-Dist: flake8 (>=5.0.1,<6.0.0) ; extra == "test"
 Requires-Dist: flake8-docstrings (>=1.6.0,<2.0.0) ; extra == "test"
 Requires-Dist: flake8-pyproject (>=1.2.3,<2.0.0) ; extra == "test"
+Requires-Dist: griffe-fieldz (>=0.1.2)
 Requires-Dist: isort (>=5.8.0,<6.0.0) ; extra == "test"
-Requires-Dist: mkdocs (>=1.5.3,<2.0.0) ; extra == "doc"
-Requires-Dist: mkdocs-include-markdown-plugin (>=4.0.0,<5.0.0) ; extra == "doc"
-Requires-Dist: mkdocs-material (>=9.5.3,<10.0.0) ; extra == "doc"
+Requires-Dist: mkdocs (>=1.6.0,<2.0.0) ; extra == "doc"
+Requires-Dist: mkdocs-include-markdown-plugin (>=6.0.6,<7.0.0) ; extra == "doc"
+Requires-Dist: mkdocs-material (>=9.5.23,<10.0.0) ; extra == "doc"
+Requires-Dist: mkdocstrings[python] (>=0.25.1)
 Requires-Dist: mypy (>=1.5,<2.0) ; extra == "test"
 Requires-Dist: pip ; extra == "dev"
 Requires-Dist: pip-tools (>=7.3.0) ; extra == "dev"
 Requires-Dist: pre-commit (>=3.3.0,<4.0.0) ; extra == "dev"
 Requires-Dist: pydantic (>=2)
 Requires-Dist: pytest (>=7.2.0,<8.0.0) ; extra == "test"
 Requires-Dist: pytest-cov (>=4.0.0,<5.0.0) ; extra == "test"
```

