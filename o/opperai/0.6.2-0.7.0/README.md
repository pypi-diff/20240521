# Comparing `tmp/opperai-0.6.2.tar.gz` & `tmp/opperai-0.7.0.tar.gz`

## Comparing `opperai-0.6.2.tar` & `opperai-0.7.0.tar`

### file list

```diff
@@ -1,97 +1,100 @@
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 opperai-0.6.2/pytest.ini
--rw-r--r--   0        0        0     5424 2020-02-02 00:00:00.000000 opperai-0.6.2/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 opperai-0.6.2/src/opperai/__init__.py
--rw-r--r--   0        0        0     3069 2020-02-02 00:00:00.000000 opperai-0.6.2/src/opperai/_client.py
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 opperai-0.6.2/src/opperai/core/_http_clients.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opperai-0.6.2/src/opperai/core/functions/__init__.py
--rw-r--r--   0        0        0    14112 2020-02-02 00:00:00.000000 opperai-0.6.2/src/opperai/core/functions/_async_functions.py
--rw-r--r--   0        0        0    15365 2020-02-02 00:00:00.000000 opperai-0.6.2/src/opperai/core/functions/_functions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opperai-0.6.2/src/opperai/core/indexes/__init__.py
--rw-r--r--   0        0        0    12400 2020-02-02 00:00:00.000000 opperai-0.6.2/src/opperai/core/indexes/_async_indexes.py
--rw-r--r--   0        0        0    12203 2020-02-02 00:00:00.000000 opperai-0.6.2/src/opperai/core/indexes/_indexes.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 opperai-0.6.2/src/opperai/core/spans/__init__.py
--rw-r--r--   0        0        0     9236 2020-02-02 00:00:00.000000 opperai-0.6.2/src/opperai/core/spans/_async_spans.py
--rw-r--r--   0        0        0     5424 2020-02-02 00:00:00.000000 opperai-0.6.2/src/opperai/core/spans/_decorator.py
--rw-r--r--   0        0        0     8749 2020-02-02 00:00:00.000000 opperai-0.6.2/src/opperai/core/spans/_spans.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 opperai-0.6.2/src/opperai/core/utils/__init__.py
--rw-r--r--   0        0        0     6561 2020-02-02 00:00:00.000000 opperai-0.6.2/src/opperai/functions/async_functions.py
--rw-r--r--   0        0        0     5939 2020-02-02 00:00:00.000000 opperai-0.6.2/src/opperai/functions/functions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opperai-0.6.2/src/opperai/functions/decorator/__init__.py
--rw-r--r--   0        0        0     7879 2020-02-02 00:00:00.000000 opperai-0.6.2/src/opperai/functions/decorator/_decorator.py
--rw-r--r--   0        0        0     3457 2020-02-02 00:00:00.000000 opperai-0.6.2/src/opperai/functions/decorator/_schemas.py
--rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 opperai-0.6.2/src/opperai/indexes/async_indexes.py
--rw-r--r--   0        0        0     2470 2020-02-02 00:00:00.000000 opperai-0.6.2/src/opperai/indexes/indexes.py
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 opperai-0.6.2/src/opperai/spans/async_spans.py
--rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 opperai-0.6.2/src/opperai/spans/spans.py
--rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 opperai-0.6.2/src/opperai/types/__init__.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 opperai-0.6.2/src/opperai/types/exceptions.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 opperai-0.6.2/src/opperai/types/indexes.py
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 opperai-0.6.2/src/opperai/types/spans.py
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 opperai-0.6.2/src/opperai/types/validators.py
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 opperai-0.6.2/tests/conftest.py
--rw-r--r--   0        0        0    10822 2020-02-02 00:00:00.000000 opperai-0.6.2/tests/test_async_functions.py
--rw-r--r--   0        0        0     4358 2020-02-02 00:00:00.000000 opperai-0.6.2/tests/test_async_indexes.py
--rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 opperai-0.6.2/tests/test_async_spans.py
--rw-r--r--   0        0        0     9435 2020-02-02 00:00:00.000000 opperai-0.6.2/tests/test_fn_decorator.py
--rw-r--r--   0        0        0     9957 2020-02-02 00:00:00.000000 opperai-0.6.2/tests/test_functions.py
--rw-r--r--   0        0        0     3632 2020-02-02 00:00:00.000000 opperai-0.6.2/tests/test_indexes.py
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 opperai-0.6.2/tests/test_trace_decorator.py
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 opperai-0.6.2/tests/test_types.py
--rw-r--r--   0        0        0   173874 2020-02-02 00:00:00.000000 opperai-0.6.2/tests/fixtures/images/fossil.jpg
--rw-r--r--   0        0        0     5673 2020-02-02 00:00:00.000000 opperai-0.6.2/tests/fixtures/images/letters.png
--rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 opperai-0.6.2/tests/fixtures/vcr_cassettes/test_async_functions/test_async_chat.yaml
--rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 opperai-0.6.2/tests/fixtures/vcr_cassettes/test_async_functions/test_async_chat_stream.yaml
--rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 opperai-0.6.2/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function.yaml
--rw-r--r--   0        0        0     4023 2020-02-02 00:00:00.000000 opperai-0.6.2/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function_with_cache.yaml
--rw-r--r--   0        0        0     5369 2020-02-02 00:00:00.000000 opperai-0.6.2/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function_with_cache_flush.yaml
--rw-r--r--   0        0        0     2593 2020-02-02 00:00:00.000000 opperai-0.6.2/tests/fixtures/vcr_cassettes/test_async_functions/test_delete_function.yaml
--rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 opperai-0.6.2/tests/fixtures/vcr_cassettes/test_async_functions/test_failed_structured_generation.yaml
--rw-r--r--   0        0        0     3899 2020-02-02 00:00:00.000000 opperai-0.6.2/tests/fixtures/vcr_cassettes/test_async_functions/test_get.yaml
--rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 opperai-0.6.2/tests/fixtures/vcr_cassettes/test_async_functions/test_get_by_id.yaml
--rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 opperai-0.6.2/tests/fixtures/vcr_cassettes/test_async_functions/test_get_by_path.yaml
--rw-r--r--   0        0        0   236306 2020-02-02 00:00:00.000000 opperai-0.6.2/tests/fixtures/vcr_cassettes/test_async_functions/test_image_file.yaml
--rw-r--r--   0        0        0     4535 2020-02-02 00:00:00.000000 opperai-0.6.2/tests/fixtures/vcr_cassettes/test_async_functions/test_image_url.yaml
--rw-r--r--   0        0        0     3452 2020-02-02 00:00:00.000000 opperai-0.6.2/tests/fixtures/vcr_cassettes/test_async_functions/test_update_function.yaml
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 opperai-0.6.2/tests/fixtures/vcr_cassettes/test_async_indexes/test_create_index.yaml
--rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 opperai-0.6.2/tests/fixtures/vcr_cassettes/test_async_indexes/test_delete_index.yaml
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 opperai-0.6.2/tests/fixtures/vcr_cassettes/test_async_indexes/test_get_by_id.yaml
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 opperai-0.6.2/tests/fixtures/vcr_cassettes/test_async_indexes/test_get_by_name.yaml
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 opperai-0.6.2/tests/fixtures/vcr_cassettes/test_async_indexes/test_index_document.yaml
--rw-r--r--   0        0        0     3977 2020-02-02 00:00:00.000000 opperai-0.6.2/tests/fixtures/vcr_cassettes/test_async_indexes/test_list_indexes.yaml
--rw-r--r--   0        0        0     2532 2020-02-02 00:00:00.000000 opperai-0.6.2/tests/fixtures/vcr_cassettes/test_async_indexes/test_retrieve_document.yaml
--rw-r--r--   0        0        0     2588 2020-02-02 00:00:00.000000 opperai-0.6.2/tests/fixtures/vcr_cassettes/test_async_indexes/test_retrieve_filters.yaml
--rw-r--r--   0        0        0     3528 2020-02-02 00:00:00.000000 opperai-0.6.2/tests/fixtures/vcr_cassettes/test_async_spans/test_async_crud.yaml
--rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 opperai-0.6.2/tests/fixtures/vcr_cassettes/test_async_spans/test_save_metric.yaml
--rw-r--r--   0        0        0     4892 2020-02-02 00:00:00.000000 opperai-0.6.2/tests/fixtures/vcr_cassettes/test_fn_decorator/test_fn_decorator.yaml
--rw-r--r--   0        0        0     4874 2020-02-02 00:00:00.000000 opperai-0.6.2/tests/fixtures/vcr_cassettes/test_fn_decorator/test_fn_decorator_async.yaml
--rw-r--r--   0        0        0    11474 2020-02-02 00:00:00.000000 opperai-0.6.2/tests/fixtures/vcr_cassettes/test_fn_decorator/test_fn_decorator_image.yaml
--rw-r--r--   0        0        0    11474 2020-02-02 00:00:00.000000 opperai-0.6.2/tests/fixtures/vcr_cassettes/test_fn_decorator/test_fn_decorator_image_async.yaml
--rw-r--r--   0        0        0     3861 2020-02-02 00:00:00.000000 opperai-0.6.2/tests/fixtures/vcr_cassettes/test_fn_decorator/test_fn_decorator_on_method.yaml
--rw-r--r--   0        0        0     3861 2020-02-02 00:00:00.000000 opperai-0.6.2/tests/fixtures/vcr_cassettes/test_fn_decorator/test_fn_decorator_on_method_async.yaml
--rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 opperai-0.6.2/tests/fixtures/vcr_cassettes/test_functions/test_chat.yaml
--rw-r--r--   0        0        0     4010 2020-02-02 00:00:00.000000 opperai-0.6.2/tests/fixtures/vcr_cassettes/test_functions/test_chat_stream.yaml
--rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 opperai-0.6.2/tests/fixtures/vcr_cassettes/test_functions/test_create_function.yaml
--rw-r--r--   0        0        0     3993 2020-02-02 00:00:00.000000 opperai-0.6.2/tests/fixtures/vcr_cassettes/test_functions/test_create_function_with_cache.yaml
--rw-r--r--   0        0        0     5343 2020-02-02 00:00:00.000000 opperai-0.6.2/tests/fixtures/vcr_cassettes/test_functions/test_create_function_with_cache_flush.yaml
--rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 opperai-0.6.2/tests/fixtures/vcr_cassettes/test_functions/test_delete_function_by_id.yaml
--rw-r--r--   0        0        0     2703 2020-02-02 00:00:00.000000 opperai-0.6.2/tests/fixtures/vcr_cassettes/test_functions/test_delete_function_by_path.yaml
--rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 opperai-0.6.2/tests/fixtures/vcr_cassettes/test_functions/test_failed_structured_generation.yaml
--rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 opperai-0.6.2/tests/fixtures/vcr_cassettes/test_functions/test_get_by_id.yaml
--rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 opperai-0.6.2/tests/fixtures/vcr_cassettes/test_functions/test_get_by_path.yaml
--rw-r--r--   0        0        0   237017 2020-02-02 00:00:00.000000 opperai-0.6.2/tests/fixtures/vcr_cassettes/test_functions/test_image_file.yaml
--rw-r--r--   0        0        0     4451 2020-02-02 00:00:00.000000 opperai-0.6.2/tests/fixtures/vcr_cassettes/test_functions/test_image_url.yaml
--rw-r--r--   0        0        0     5892 2020-02-02 00:00:00.000000 opperai-0.6.2/tests/fixtures/vcr_cassettes/test_functions/test_update_function.yaml
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 opperai-0.6.2/tests/fixtures/vcr_cassettes/test_indexes/test_create_index.yaml
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 opperai-0.6.2/tests/fixtures/vcr_cassettes/test_indexes/test_delete_index.yaml
--rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 opperai-0.6.2/tests/fixtures/vcr_cassettes/test_indexes/test_get_by_id.yaml
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 opperai-0.6.2/tests/fixtures/vcr_cassettes/test_indexes/test_get_by_name.yaml
--rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 opperai-0.6.2/tests/fixtures/vcr_cassettes/test_indexes/test_index_document.yaml
--rw-r--r--   0        0        0     3970 2020-02-02 00:00:00.000000 opperai-0.6.2/tests/fixtures/vcr_cassettes/test_indexes/test_list_indexes.yaml
--rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 opperai-0.6.2/tests/fixtures/vcr_cassettes/test_indexes/test_retrieve_document.yaml
--rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 opperai-0.6.2/tests/fixtures/vcr_cassettes/test_indexes/test_retrieve_filters.yaml
--rw-r--r--   0        0        0     3528 2020-02-02 00:00:00.000000 opperai-0.6.2/tests/fixtures/vcr_cassettes/test_spans/test_crud.yaml
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 opperai-0.6.2/.gitignore
--rw-r--r--   0        0        0    11335 2020-02-02 00:00:00.000000 opperai-0.6.2/LICENSE
--rw-r--r--   0        0        0     4382 2020-02-02 00:00:00.000000 opperai-0.6.2/README.md
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 opperai-0.6.2/pyproject.toml
--rw-r--r--   0        0        0     5148 2020-02-02 00:00:00.000000 opperai-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 opperai-0.7.0/pytest.ini
+-rw-r--r--   0        0        0     5424 2020-02-02 00:00:00.000000 opperai-0.7.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 opperai-0.7.0/src/opperai/__init__.py
+-rw-r--r--   0        0        0     2636 2020-02-02 00:00:00.000000 opperai-0.7.0/src/opperai/_client.py
+-rw-r--r--   0        0        0     3633 2020-02-02 00:00:00.000000 opperai-0.7.0/src/opperai/core/_http_clients.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opperai-0.7.0/src/opperai/core/functions/__init__.py
+-rw-r--r--   0        0        0    13815 2020-02-02 00:00:00.000000 opperai-0.7.0/src/opperai/core/functions/_async_functions.py
+-rw-r--r--   0        0        0    15068 2020-02-02 00:00:00.000000 opperai-0.7.0/src/opperai/core/functions/_functions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opperai-0.7.0/src/opperai/core/indexes/__init__.py
+-rw-r--r--   0        0        0    12417 2020-02-02 00:00:00.000000 opperai-0.7.0/src/opperai/core/indexes/_async_indexes.py
+-rw-r--r--   0        0        0    12203 2020-02-02 00:00:00.000000 opperai-0.7.0/src/opperai/core/indexes/_indexes.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 opperai-0.7.0/src/opperai/core/spans/__init__.py
+-rw-r--r--   0        0        0     9236 2020-02-02 00:00:00.000000 opperai-0.7.0/src/opperai/core/spans/_async_spans.py
+-rw-r--r--   0        0        0     5424 2020-02-02 00:00:00.000000 opperai-0.7.0/src/opperai/core/spans/_decorator.py
+-rw-r--r--   0        0        0     8749 2020-02-02 00:00:00.000000 opperai-0.7.0/src/opperai/core/spans/_spans.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 opperai-0.7.0/src/opperai/core/utils/__init__.py
+-rw-r--r--   0        0        0     6566 2020-02-02 00:00:00.000000 opperai-0.7.0/src/opperai/functions/async_functions.py
+-rw-r--r--   0        0        0     5939 2020-02-02 00:00:00.000000 opperai-0.7.0/src/opperai/functions/functions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opperai-0.7.0/src/opperai/functions/decorator/__init__.py
+-rw-r--r--   0        0        0     7879 2020-02-02 00:00:00.000000 opperai-0.7.0/src/opperai/functions/decorator/_decorator.py
+-rw-r--r--   0        0        0     3457 2020-02-02 00:00:00.000000 opperai-0.7.0/src/opperai/functions/decorator/_schemas.py
+-rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 opperai-0.7.0/src/opperai/indexes/async_indexes.py
+-rw-r--r--   0        0        0     2470 2020-02-02 00:00:00.000000 opperai-0.7.0/src/opperai/indexes/indexes.py
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 opperai-0.7.0/src/opperai/spans/async_spans.py
+-rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 opperai-0.7.0/src/opperai/spans/spans.py
+-rw-r--r--   0        0        0     4168 2020-02-02 00:00:00.000000 opperai-0.7.0/src/opperai/types/__init__.py
+-rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 opperai-0.7.0/src/opperai/types/exceptions.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 opperai-0.7.0/src/opperai/types/indexes.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 opperai-0.7.0/src/opperai/types/spans.py
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 opperai-0.7.0/src/opperai/types/validators.py
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 opperai-0.7.0/tests/conftest.py
+-rw-r--r--   0        0        0    10847 2020-02-02 00:00:00.000000 opperai-0.7.0/tests/test_async_functions.py
+-rw-r--r--   0        0        0     4358 2020-02-02 00:00:00.000000 opperai-0.7.0/tests/test_async_indexes.py
+-rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 opperai-0.7.0/tests/test_async_spans.py
+-rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 opperai-0.7.0/tests/test_client.py
+-rw-r--r--   0        0        0     9489 2020-02-02 00:00:00.000000 opperai-0.7.0/tests/test_fn_decorator.py
+-rw-r--r--   0        0        0     9957 2020-02-02 00:00:00.000000 opperai-0.7.0/tests/test_functions.py
+-rw-r--r--   0        0        0     3632 2020-02-02 00:00:00.000000 opperai-0.7.0/tests/test_indexes.py
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 opperai-0.7.0/tests/test_trace_decorator.py
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 opperai-0.7.0/tests/test_types.py
+-rw-r--r--   0        0        0   173874 2020-02-02 00:00:00.000000 opperai-0.7.0/tests/fixtures/images/fossil.jpg
+-rw-r--r--   0        0        0   199592 2020-02-02 00:00:00.000000 opperai-0.7.0/tests/fixtures/images/fossil.png
+-rw-r--r--   0        0        0     5673 2020-02-02 00:00:00.000000 opperai-0.7.0/tests/fixtures/images/letters.png
+-rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 opperai-0.7.0/tests/fixtures/vcr_cassettes/test_async_functions/test_async_chat.yaml
+-rw-r--r--   0        0        0     3157 2020-02-02 00:00:00.000000 opperai-0.7.0/tests/fixtures/vcr_cassettes/test_async_functions/test_async_chat_stream.yaml
+-rw-r--r--   0        0        0     2225 2020-02-02 00:00:00.000000 opperai-0.7.0/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function.yaml
+-rw-r--r--   0        0        0     4090 2020-02-02 00:00:00.000000 opperai-0.7.0/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function_with_cache.yaml
+-rw-r--r--   0        0        0     5195 2020-02-02 00:00:00.000000 opperai-0.7.0/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function_with_cache_flush.yaml
+-rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 opperai-0.7.0/tests/fixtures/vcr_cassettes/test_async_functions/test_delete_function.yaml
+-rw-r--r--   0        0        0     5641 2020-02-02 00:00:00.000000 opperai-0.7.0/tests/fixtures/vcr_cassettes/test_async_functions/test_failed_structured_generation.yaml
+-rw-r--r--   0        0        0     3974 2020-02-02 00:00:00.000000 opperai-0.7.0/tests/fixtures/vcr_cassettes/test_async_functions/test_get.yaml
+-rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 opperai-0.7.0/tests/fixtures/vcr_cassettes/test_async_functions/test_get_by_id.yaml
+-rw-r--r--   0        0        0     3124 2020-02-02 00:00:00.000000 opperai-0.7.0/tests/fixtures/vcr_cassettes/test_async_functions/test_get_by_path.yaml
+-rw-r--r--   0        0        0   236349 2020-02-02 00:00:00.000000 opperai-0.7.0/tests/fixtures/vcr_cassettes/test_async_functions/test_image_file.yaml
+-rw-r--r--   0        0        0     4822 2020-02-02 00:00:00.000000 opperai-0.7.0/tests/fixtures/vcr_cassettes/test_async_functions/test_image_url.yaml
+-rw-r--r--   0        0        0     3519 2020-02-02 00:00:00.000000 opperai-0.7.0/tests/fixtures/vcr_cassettes/test_async_functions/test_update_function.yaml
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 opperai-0.7.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_create_index.yaml
+-rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 opperai-0.7.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_delete_index.yaml
+-rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 opperai-0.7.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_get_by_id.yaml
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 opperai-0.7.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_get_by_name.yaml
+-rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 opperai-0.7.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_index_document.yaml
+-rw-r--r--   0        0        0     3970 2020-02-02 00:00:00.000000 opperai-0.7.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_list_indexes.yaml
+-rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 opperai-0.7.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_retrieve_document.yaml
+-rw-r--r--   0        0        0     2582 2020-02-02 00:00:00.000000 opperai-0.7.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_retrieve_filters.yaml
+-rw-r--r--   0        0        0     3528 2020-02-02 00:00:00.000000 opperai-0.7.0/tests/fixtures/vcr_cassettes/test_async_spans/test_async_crud.yaml
+-rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 opperai-0.7.0/tests/fixtures/vcr_cassettes/test_async_spans/test_save_metric.yaml
+-rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 opperai-0.7.0/tests/fixtures/vcr_cassettes/test_client/test_async_client_raises_timeout_error.yaml
+-rw-r--r--   0        0        0     2345 2020-02-02 00:00:00.000000 opperai-0.7.0/tests/fixtures/vcr_cassettes/test_client/test_client_raises_timeout_error.yaml
+-rw-r--r--   0        0        0     4862 2020-02-02 00:00:00.000000 opperai-0.7.0/tests/fixtures/vcr_cassettes/test_fn_decorator/test_fn_decorator.yaml
+-rw-r--r--   0        0        0     4862 2020-02-02 00:00:00.000000 opperai-0.7.0/tests/fixtures/vcr_cassettes/test_fn_decorator/test_fn_decorator_async.yaml
+-rw-r--r--   0        0        0   270241 2020-02-02 00:00:00.000000 opperai-0.7.0/tests/fixtures/vcr_cassettes/test_fn_decorator/test_fn_decorator_image.yaml
+-rw-r--r--   0        0        0    11470 2020-02-02 00:00:00.000000 opperai-0.7.0/tests/fixtures/vcr_cassettes/test_fn_decorator/test_fn_decorator_image_async.yaml
+-rw-r--r--   0        0        0     3857 2020-02-02 00:00:00.000000 opperai-0.7.0/tests/fixtures/vcr_cassettes/test_fn_decorator/test_fn_decorator_on_method.yaml
+-rw-r--r--   0        0        0     3857 2020-02-02 00:00:00.000000 opperai-0.7.0/tests/fixtures/vcr_cassettes/test_fn_decorator/test_fn_decorator_on_method_async.yaml
+-rw-r--r--   0        0        0     3818 2020-02-02 00:00:00.000000 opperai-0.7.0/tests/fixtures/vcr_cassettes/test_functions/test_chat.yaml
+-rw-r--r--   0        0        0     4069 2020-02-02 00:00:00.000000 opperai-0.7.0/tests/fixtures/vcr_cassettes/test_functions/test_chat_stream.yaml
+-rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 opperai-0.7.0/tests/fixtures/vcr_cassettes/test_functions/test_create_function.yaml
+-rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 opperai-0.7.0/tests/fixtures/vcr_cassettes/test_functions/test_create_function_with_cache.yaml
+-rw-r--r--   0        0        0     5368 2020-02-02 00:00:00.000000 opperai-0.7.0/tests/fixtures/vcr_cassettes/test_functions/test_create_function_with_cache_flush.yaml
+-rw-r--r--   0        0        0     2761 2020-02-02 00:00:00.000000 opperai-0.7.0/tests/fixtures/vcr_cassettes/test_functions/test_delete_function_by_id.yaml
+-rw-r--r--   0        0        0     2853 2020-02-02 00:00:00.000000 opperai-0.7.0/tests/fixtures/vcr_cassettes/test_functions/test_delete_function_by_path.yaml
+-rw-r--r--   0        0        0     3918 2020-02-02 00:00:00.000000 opperai-0.7.0/tests/fixtures/vcr_cassettes/test_functions/test_failed_structured_generation.yaml
+-rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 opperai-0.7.0/tests/fixtures/vcr_cassettes/test_functions/test_get_by_id.yaml
+-rw-r--r--   0        0        0     3124 2020-02-02 00:00:00.000000 opperai-0.7.0/tests/fixtures/vcr_cassettes/test_functions/test_get_by_path.yaml
+-rw-r--r--   0        0        0   236495 2020-02-02 00:00:00.000000 opperai-0.7.0/tests/fixtures/vcr_cassettes/test_functions/test_image_file.yaml
+-rw-r--r--   0        0        0     4694 2020-02-02 00:00:00.000000 opperai-0.7.0/tests/fixtures/vcr_cassettes/test_functions/test_image_url.yaml
+-rw-r--r--   0        0        0     5417 2020-02-02 00:00:00.000000 opperai-0.7.0/tests/fixtures/vcr_cassettes/test_functions/test_update_function.yaml
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 opperai-0.7.0/tests/fixtures/vcr_cassettes/test_indexes/test_create_index.yaml
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 opperai-0.7.0/tests/fixtures/vcr_cassettes/test_indexes/test_delete_index.yaml
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 opperai-0.7.0/tests/fixtures/vcr_cassettes/test_indexes/test_get_by_id.yaml
+-rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 opperai-0.7.0/tests/fixtures/vcr_cassettes/test_indexes/test_get_by_name.yaml
+-rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 opperai-0.7.0/tests/fixtures/vcr_cassettes/test_indexes/test_index_document.yaml
+-rw-r--r--   0        0        0     3977 2020-02-02 00:00:00.000000 opperai-0.7.0/tests/fixtures/vcr_cassettes/test_indexes/test_list_indexes.yaml
+-rw-r--r--   0        0        0     2530 2020-02-02 00:00:00.000000 opperai-0.7.0/tests/fixtures/vcr_cassettes/test_indexes/test_retrieve_document.yaml
+-rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 opperai-0.7.0/tests/fixtures/vcr_cassettes/test_indexes/test_retrieve_filters.yaml
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 opperai-0.7.0/.gitignore
+-rw-r--r--   0        0        0    11335 2020-02-02 00:00:00.000000 opperai-0.7.0/LICENSE
+-rw-r--r--   0        0        0     4382 2020-02-02 00:00:00.000000 opperai-0.7.0/README.md
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 opperai-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     5148 2020-02-02 00:00:00.000000 opperai-0.7.0/PKG-INFO
```

### Comparing `opperai-0.6.2/.github/workflows/publish.yml` & `opperai-0.7.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `opperai-0.6.2/src/opperai/__init__.py` & `opperai-0.7.0/src/opperai/__init__.py`

 * *Files identical despite different names*

### Comparing `opperai-0.6.2/src/opperai/core/functions/_async_functions.py` & `opperai-0.7.0/src/opperai/core/functions/_async_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from opperai.types import (
     ChatPayload,
     Function,
     FunctionResponse,
     StreamingChunk,
     validate_id_xor_path,
 )
-from opperai.types.exceptions import APIError, RateLimitError, StructuredGenerationError
+from opperai.types.exceptions import APIError
 
 
 class AsyncFunctions:
     def __init__(self, http_client: _async_http_client, default_model: str = None):
         self.http_client = http_client
         self.default_model = default_model
 
@@ -295,21 +295,17 @@
             "POST",
             f"/v1/chat/{function_path}",
             json={**serialized_data, **kwargs},
         )
 
         if response.status_code == HTTPStatus.OK:
             return FunctionResponse.model_validate(response.json())
-        elif response.status_code == HTTPStatus.TOO_MANY_REQUESTS:
-            raise RateLimitError("Rate limit error: please retry in a few seconds")
-        elif response.status_code == HTTPStatus.BAD_REQUEST:
-            raise StructuredGenerationError(response.text)
 
         raise APIError(
-            f"Failed to run function {function_path} with status {response.status_code}"
+            f"Failed to run function {function_path} with status {response.status_code}: {response.text}"
         )
 
     async def _chat_stream(
         self, function_path, data: ChatPayload, **kwargs
     ) -> Generator[StreamingChunk, None, None]:
         gen = self.http_client.stream(
             "POST",
```

### Comparing `opperai-0.6.2/src/opperai/core/functions/_functions.py` & `opperai-0.7.0/src/opperai/core/functions/_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from opperai.types import (
     ChatPayload,
     Function,
     FunctionResponse,
     StreamingChunk,
     validate_id_xor_path,
 )
-from opperai.types.exceptions import APIError, RateLimitError, StructuredGenerationError
+from opperai.types.exceptions import APIError
 
 
 class Functions:
     def __init__(self, http_client: _http_client, default_model: str = None):
         self.http_client = http_client
         self.default_model = default_model
 
@@ -325,21 +325,17 @@
             "POST",
             f"/v1/chat/{function_path}",
             json={**serialized_data, **kwargs},
         )
 
         if response.status_code == HTTPStatus.OK:
             return FunctionResponse.model_validate(response.json())
-        elif response.status_code == HTTPStatus.TOO_MANY_REQUESTS:
-            raise RateLimitError("Rate limit error: please retry in a few seconds")
-        elif response.status_code == HTTPStatus.BAD_REQUEST:
-            raise StructuredGenerationError(response.text)
 
         raise APIError(
-            f"Failed to run function {function_path} with status {response.status_code}"
+            f"Failed to run function {function_path} with status {response.status_code}: {response.text}"
         )
 
     def _chat_stream(
         self, function_path, data: ChatPayload, **kwargs
     ) -> Iterator[StreamingChunk]:
         gen = self.http_client.stream(
             "POST",
```

### Comparing `opperai-0.6.2/src/opperai/core/indexes/_async_indexes.py` & `opperai-0.7.0/src/opperai/core/indexes/_async_indexes.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from opperai.types.exceptions import APIError
 from opperai.types.indexes import (
     Document,
     Filter,
     Index,
     RetrievalResponse,
 )
+
 from ._indexes import RetrieveQuery
 
 
 class AsyncIndexes:
     def __init__(self, http_client: _async_http_client):
         self.http_client = http_client
 
@@ -46,15 +47,17 @@
         if response.status_code != 200:
             raise APIError(f"Failed to create index with status {response.status_code}")
         return Index.model_validate(response.json())
 
     async def delete(self, id: int) -> bool:
         """Delete an index
 
-        This method sends a DELETE request to the OpperAI service to remove an index specified by its unique identifier. If the index does not exist, it returns False. If the deletion is successful, it returns True. If there's an issue with the request, it raises an APIError.
+        This method sends a DELETE request to the OpperAI service to remove an index specified by
+        its unique identifier. If the index does not exist, it returns False. If the deletion is
+        successful, it returns True. If there's an issue with the request, it raises an APIError.
 
         Args:
             id (int): The unique identifier of the index to be deleted.
 
         Returns:
             bool: True if the index was successfully deleted, False if the index does not exist.
```

### Comparing `opperai-0.6.2/src/opperai/core/indexes/_indexes.py` & `opperai-0.7.0/src/opperai/core/indexes/_indexes.py`

 * *Files identical despite different names*

### Comparing `opperai-0.6.2/src/opperai/core/spans/_async_spans.py` & `opperai-0.7.0/src/opperai/core/spans/_async_spans.py`

 * *Files identical despite different names*

### Comparing `opperai-0.6.2/src/opperai/core/spans/_decorator.py` & `opperai-0.7.0/src/opperai/core/spans/_decorator.py`

 * *Files identical despite different names*

### Comparing `opperai-0.6.2/src/opperai/core/spans/_spans.py` & `opperai-0.7.0/src/opperai/core/spans/_spans.py`

 * *Files identical despite different names*

### Comparing `opperai-0.6.2/src/opperai/core/utils/__init__.py` & `opperai-0.7.0/src/opperai/core/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `opperai-0.6.2/src/opperai/functions/async_functions.py` & `opperai-0.7.0/src/opperai/functions/async_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
             client = AsyncClient()
         self._client = client
         self.stream = stream
 
     async def initialize(self):
         self.stream = await self.stream
         try:
-            first_chunk = await anext(self.stream)
+            first_chunk = await self.stream.__anext__()
             self._span_id = (
                 first_chunk.span_id if first_chunk.span_id is not None else None
             )
             self._context = (
                 first_chunk.context if first_chunk.context is not None else []
             )
         except StopAsyncIteration:
```

### Comparing `opperai-0.6.2/src/opperai/functions/functions.py` & `opperai-0.7.0/src/opperai/functions/functions.py`

 * *Files identical despite different names*

### Comparing `opperai-0.6.2/src/opperai/functions/decorator/_decorator.py` & `opperai-0.7.0/src/opperai/functions/decorator/_decorator.py`

 * *Files identical despite different names*

### Comparing `opperai-0.6.2/src/opperai/functions/decorator/_schemas.py` & `opperai-0.7.0/src/opperai/functions/decorator/_schemas.py`

 * *Files identical despite different names*

### Comparing `opperai-0.6.2/src/opperai/indexes/async_indexes.py` & `opperai-0.7.0/src/opperai/indexes/async_indexes.py`

 * *Files identical despite different names*

### Comparing `opperai-0.6.2/src/opperai/indexes/indexes.py` & `opperai-0.7.0/src/opperai/indexes/indexes.py`

 * *Files identical despite different names*

### Comparing `opperai-0.6.2/src/opperai/spans/async_spans.py` & `opperai-0.7.0/src/opperai/spans/async_spans.py`

 * *Files identical despite different names*

### Comparing `opperai-0.6.2/src/opperai/spans/spans.py` & `opperai-0.7.0/src/opperai/spans/spans.py`

 * *Files identical despite different names*

### Comparing `opperai-0.6.2/src/opperai/types/__init__.py` & `opperai-0.7.0/src/opperai/types/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # ruff: noqa: F401
+
 import base64
+from pathlib import Path
 from typing import Any, Dict, List, Optional, Union
 from uuid import UUID
 
-from pydantic import BaseModel, ConfigDict, Field, computed_field
+from pydantic import BaseModel, ConfigDict, Field, FilePath, computed_field
 
 from .indexes import Document, Filter, RetrievalResponse
 from .spans import SpanMetric
 from .validators import validate_id_xor_path
 
 
 class TextMessageContent(BaseModel):
@@ -16,29 +18,30 @@
 
 
 class ImageMessageUrl(BaseModel):
     url: str
 
 
 class ImageMessageFile(BaseModel):
-    path: str = Field(exclude=True)
+    path: FilePath = Field(exclude=True)
 
     @computed_field
     @property
     def url(self) -> str:
-        if self.path.endswith(".png"):
-            with open(self.path, "rb") as image_file:
+        path = self.path.as_posix()
+        if path.endswith(".png"):
+            with open(path, "rb") as image_file:
                 base64_image = base64.b64encode(image_file.read()).decode("utf-8")
             return f"data:image/png;base64,{base64_image}"
-        elif self.path.endswith(".jpg"):
-            with open(self.path, "rb") as image_file:
+        elif path.endswith(".jpg"):
+            with open(path, "rb") as image_file:
                 base64_image = base64.b64encode(image_file.read()).decode("utf-8")
             return f"data:image/jpeg;base64,{base64_image}"
-        elif self.path.endswith(".jpeg"):
-            with open(self.path, "rb") as image_file:
+        elif path.endswith(".jpeg"):
+            with open(path, "rb") as image_file:
                 base64_image = base64.b64encode(image_file.read()).decode("utf-8")
             return f"data:image/jpeg;base64,{base64_image}"
         else:
             raise ValueError(
                 "File type not supported. Supported types: .png, .jpg, .jpeg"
             )
 
@@ -127,7 +130,17 @@
     instructions: str
     model: Optional[str] = None
     index_ids: Optional[List[int]] = []
     use_semantic_search: Optional[bool] = None
     few_shot: Optional[bool] = None
     few_shot_count: Optional[int] = None
     cache_configuration: Optional[CacheConfiguration] = None
+
+
+class Error(BaseModel):
+    type: str
+    message: str
+    detail: Any
+
+
+class Errors(BaseModel):
+    errors: List[Error]
```

### Comparing `opperai-0.6.2/src/opperai/types/indexes.py` & `opperai-0.7.0/src/opperai/types/indexes.py`

 * *Files identical despite different names*

### Comparing `opperai-0.6.2/src/opperai/types/spans.py` & `opperai-0.7.0/src/opperai/types/spans.py`

 * *Files identical despite different names*

### Comparing `opperai-0.6.2/src/opperai/types/validators.py` & `opperai-0.7.0/src/opperai/types/validators.py`

 * *Files identical despite different names*

### Comparing `opperai-0.6.2/tests/conftest.py` & `opperai-0.7.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `opperai-0.6.2/tests/test_async_functions.py` & `opperai-0.7.0/tests/test_async_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -263,15 +263,15 @@
 @pytest.mark.asyncio(scope="module")
 async def test_failed_structured_generation(aclient: AsyncClient, vcr_cassette):
     async with _function(
         Function(
             model="mistral/mistral-tiny-eu",
             path="test/sdk/test_failed_structured_generation",
             description="test structured generation exception",
-            instructions="You translate the incoming text to french",
+            instructions="You translate the incoming text to french returned as markdown ```",
             out_schema={
                 "type": "object",
                 "properties": {
                     "universityName": {"type": "string"},
                     "location": {"type": "string"},
                     "departments": {
                         "type": "array",
```

### Comparing `opperai-0.6.2/tests/test_async_indexes.py` & `opperai-0.7.0/tests/test_async_indexes.py`

 * *Files identical despite different names*

### Comparing `opperai-0.6.2/tests/test_async_spans.py` & `opperai-0.7.0/tests/test_async_spans.py`

 * *Files identical despite different names*

### Comparing `opperai-0.6.2/tests/test_fn_decorator.py` & `opperai-0.7.0/tests/test_fn_decorator.py`

 * *Files 7% similar despite different names*

```diff
@@ -42,29 +42,29 @@
     assert "hello" in res.lower()
 
     res, _ = await test.test_method.call("Hello")
     assert "hello" in res.lower()
 
 
 def test_fn_decorator_image(client: Client, vcr_cassette):
-    class Word(BaseModel):
-        letters: List[str]
+    class ImageDescription(BaseModel):
+        description: str
 
     @fn(client=client, model="openai/gpt-4o")
-    def extract_letters(
+    def describe_image(
         image: ImageContent,
-    ) -> Word:
-        """given an image extract the word it represents"""
+    ) -> ImageDescription:
+        """given an image describe what it is"""
 
-    word = extract_letters(
-        ImageContent.from_path("tests/fixtures/images/letters.png"),
+    description = describe_image(
+        ImageContent.from_path("tests/fixtures/images/fossil.png"),
     )
-    print(word)
+    print(description)
 
-    assert [x.lower() for x in word.letters] == ["l", "e", "t", "t", "e", "r"]
+    assert "fossil" in description.description.lower()
 
 
 @pytest.mark.asyncio(scope="module")
 async def test_fn_decorator_image_async(aclient: AsyncClient, vcr_cassette):
     class Word(BaseModel):
         letters: List[str]
 
@@ -248,18 +248,18 @@
 
 
 def test_convert_func_to_json_with_image():
     def f(image: ImageContent, text: str) -> str:
         pass
 
     input, media = convert_function_call_to_json(
-        f, ImageContent.from_path("path"), "Hello"
+        f, ImageContent.from_path("tests/fixtures/images/fossil.png"), "Hello"
     )
     assert input == {"text": "Hello"}
-    assert media == [ImageContent.from_path("path")]
+    assert media == [ImageContent.from_path("tests/fixtures/images/fossil.png")]
 
 
 class ToyModel(BaseModel):
     name: str
 
 
 class ChildModel(BaseModel):
```

### Comparing `opperai-0.6.2/tests/test_functions.py` & `opperai-0.7.0/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `opperai-0.6.2/tests/test_indexes.py` & `opperai-0.7.0/tests/test_indexes.py`

 * *Files identical despite different names*

### Comparing `opperai-0.6.2/tests/test_trace_decorator.py` & `opperai-0.7.0/tests/test_trace_decorator.py`

 * *Files identical despite different names*

### Comparing `opperai-0.6.2/tests/test_types.py` & `opperai-0.7.0/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `opperai-0.6.2/tests/fixtures/images/fossil.jpg` & `opperai-0.7.0/tests/fixtures/images/fossil.jpg`

 * *Files identical despite different names*

### Comparing `opperai-0.6.2/tests/fixtures/images/letters.png` & `opperai-0.7.0/tests/fixtures/images/letters.png`

 * *Files identical despite different names*

### Comparing `opperai-0.6.2/tests/fixtures/vcr_cassettes/test_async_functions/test_async_chat.yaml` & `opperai-0.7.0/tests/fixtures/vcr_cassettes/test_async_functions/test_async_chat.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -6,22 +6,23 @@
       - '*/*'
       connection:
       - keep-alive
     method: GET
     uri: http://localhost:8000/v1/functions/by_path/test/sdk/test_async_chat
   response:
     body:
-      string: '{"detail":"Function not found"}'
+      string: '{"errors":[{"type":"HTTPException","message":"Function not found","detail":"Function
+        not found"}]}'
     headers:
       content-length:
-      - '31'
+      - '98'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 10:52:28 GMT
+      - Tue, 21 May 2024 10:10:02 GMT
       server:
       - uvicorn
     status:
       code: 404
       message: Not Found
 - request:
     body: '{"id": null, "path": "test/sdk/test_async_chat", "description": "Translate
@@ -37,24 +38,23 @@
       - '299'
       content-type:
       - application/json
     method: POST
     uri: http://localhost:8000/v1/functions
   response:
     body:
-      string: '{"id":71,"path":"test/sdk/test_async_chat","description":"Translate
-        to French","input_schema":null,"out_schema":null,"instructions":"Translate
-        to French","few_shot":false,"few_shot_count":2,"dataset_uuid":"05a07dc3-f0a2-4a31-8283-b85ad16b8653","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
+      string: '{"path":"test/sdk/test_async_chat","instructions":"Translate to French","id":33,"description":"Translate
+        to French","input_schema":null,"out_schema":null,"few_shot":false,"few_shot_count":2,"dataset_uuid":"ebc1ad13-460f-4351-88e7-021375408546","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
     headers:
       content-length:
       - '400'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 10:52:28 GMT
+      - Tue, 21 May 2024 10:10:02 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: '{"parent_span_uuid": null, "messages": [{"role": "user", "content": "hello"}]}'
@@ -67,43 +67,43 @@
       - '78'
       content-type:
       - application/json
     method: POST
     uri: http://localhost:8000/v1/chat/test/sdk/test_async_chat
   response:
     body:
-      string: '{"span_id":"7099623e-78b8-450d-887c-2028f018caed","message":"Bonjour","json_payload":null,"error":null,"context":null,"cached":false}'
+      string: '{"span_id":"3010807e-b28a-4840-a9cc-828b8b9924a8","message":"Bonjour","json_payload":null,"context":null,"cached":false}'
     headers:
       content-length:
-      - '133'
+      - '120'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 10:52:28 GMT
+      - Tue, 21 May 2024 10:10:02 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
     method: DELETE
-    uri: http://localhost:8000/v1/functions/71
+    uri: http://localhost:8000/v1/functions/33
   response:
     body:
       string: ''
     headers:
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 10:52:29 GMT
+      - Tue, 21 May 2024 10:10:03 GMT
       server:
       - uvicorn
     status:
       code: 204
       message: No Content
 version: 1
```

### Comparing `opperai-0.6.2/tests/fixtures/vcr_cassettes/test_async_functions/test_async_chat_stream.yaml` & `opperai-0.7.0/tests/fixtures/vcr_cassettes/test_async_functions/test_async_chat_stream.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -6,22 +6,23 @@
       - '*/*'
       connection:
       - keep-alive
     method: GET
     uri: http://localhost:8000/v1/functions/by_path/test/sdk/test_async_chat_stream
   response:
     body:
-      string: '{"detail":"Function not found"}'
+      string: '{"errors":[{"type":"HTTPException","message":"Function not found","detail":"Function
+        not found"}]}'
     headers:
       content-length:
-      - '31'
+      - '98'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 10:52:29 GMT
+      - Tue, 21 May 2024 10:10:03 GMT
       server:
       - uvicorn
     status:
       code: 404
       message: Not Found
 - request:
     body: '{"id": null, "path": "test/sdk/test_async_chat_stream", "description":
@@ -37,24 +38,23 @@
       - '306'
       content-type:
       - application/json
     method: POST
     uri: http://localhost:8000/v1/functions
   response:
     body:
-      string: '{"id":72,"path":"test/sdk/test_async_chat_stream","description":"Translate
-        to French","input_schema":null,"out_schema":null,"instructions":"Translate
-        to French","few_shot":false,"few_shot_count":2,"dataset_uuid":"c3d10f2b-3760-4cba-bf6d-60a4f011d093","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
+      string: '{"path":"test/sdk/test_async_chat_stream","instructions":"Translate
+        to French","id":34,"description":"Translate to French","input_schema":null,"out_schema":null,"few_shot":false,"few_shot_count":2,"dataset_uuid":"39480448-fe2c-4f18-a2f7-ce71c686467e","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
     headers:
       content-length:
       - '407'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 10:52:29 GMT
+      - Tue, 21 May 2024 10:10:03 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: '{"parent_span_uuid": null, "messages": [{"role": "user", "content": "hello"}]}'
@@ -69,27 +69,27 @@
       - '78'
       content-type:
       - application/json
     method: POST
     uri: http://localhost:8000/v1/chat/test/sdk/test_async_chat_stream?stream=True
   response:
     body:
-      string: "data: {\"span_id\": \"29fdf592-9b0b-4f20-b30e-0fcc972c12f5\"}\r\n\r\ndata:
+      string: "data: {\"span_id\": \"47f354e1-263d-4e37-9639-f5db39190653\"}\r\n\r\ndata:
         {\"delta\": \"Bonjour\"}\r\n\r\n"
     headers:
       Transfer-Encoding:
       - chunked
       cache-control:
       - no-cache
       connection:
       - keep-alive
       content-type:
       - text/event-stream; charset=utf-8
       date:
-      - Thu, 02 May 2024 10:52:29 GMT
+      - Tue, 21 May 2024 10:10:03 GMT
       server:
       - uvicorn
       x-accel-buffering:
       - 'no'
     status:
       code: 200
       message: OK
@@ -97,22 +97,22 @@
     body: ''
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
     method: DELETE
-    uri: http://localhost:8000/v1/functions/72
+    uri: http://localhost:8000/v1/functions/34
   response:
     body:
       string: ''
     headers:
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 10:52:29 GMT
+      - Tue, 21 May 2024 10:10:03 GMT
       server:
       - uvicorn
     status:
       code: 204
       message: No Content
 version: 1
```

### Comparing `opperai-0.6.2/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function.yaml` & `opperai-0.7.0/tests/fixtures/vcr_cassettes/test_functions/test_delete_function_by_id.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -3,32 +3,33 @@
     body: ''
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
     method: GET
-    uri: http://localhost:8000/v1/functions/by_path/test/sdk/test_create_function_async
+    uri: http://localhost:8000/v1/functions/by_path/test/sdk/test_delete_function_by_id
   response:
     body:
-      string: '{"detail":"Function not found"}'
+      string: '{"errors":[{"type":"HTTPException","message":"Function not found","detail":"Function
+        not found"}]}'
     headers:
       content-length:
-      - '31'
+      - '98'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 10:52:28 GMT
+      - Tue, 21 May 2024 10:10:21 GMT
       server:
       - uvicorn
     status:
       code: 404
       message: Not Found
 - request:
-    body: '{"id": null, "path": "test/sdk/test_create_function_async", "description":
+    body: '{"id": null, "path": "test/sdk/test_delete_function_by_id", "description":
       "Test function", "input_schema": null, "out_schema": null, "instructions": "Do
       something", "model": null, "index_ids": [], "use_semantic_search": null, "few_shot":
       null, "few_shot_count": null, "cache_configuration": null}'
     headers:
       accept:
       - '*/*'
       connection:
@@ -37,44 +38,69 @@
       - '297'
       content-type:
       - application/json
     method: POST
     uri: http://localhost:8000/v1/functions
   response:
     body:
-      string: '{"id":65,"path":"test/sdk/test_create_function_async","description":"Test
-        function","input_schema":null,"out_schema":null,"instructions":"Do something","few_shot":false,"few_shot_count":2,"dataset_uuid":"b10c086d-6e04-4517-b577-8387939018d8","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
+      string: '{"path":"test/sdk/test_delete_function_by_id","instructions":"Do something","id":42,"description":"Test
+        function","input_schema":null,"out_schema":null,"few_shot":false,"few_shot_count":2,"dataset_uuid":"b787b478-20e7-4051-a4e7-bc88ec424121","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
     headers:
       content-length:
       - '398'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 10:52:28 GMT
+      - Tue, 21 May 2024 10:10:21 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
     method: DELETE
-    uri: http://localhost:8000/v1/functions/65
+    uri: http://localhost:8000/v1/functions/42
   response:
     body:
       string: ''
     headers:
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 10:52:28 GMT
+      - Tue, 21 May 2024 10:10:21 GMT
       server:
       - uvicorn
     status:
       code: 204
       message: No Content
+- request:
+    body: ''
+    headers:
+      accept:
+      - '*/*'
+      connection:
+      - keep-alive
+    method: GET
+    uri: http://localhost:8000/v1/functions/42
+  response:
+    body:
+      string: '{"errors":[{"type":"HTTPException","message":"Function not found","detail":"Function
+        not found"}]}'
+    headers:
+      content-length:
+      - '98'
+      content-type:
+      - application/json
+      date:
+      - Tue, 21 May 2024 10:10:21 GMT
+      server:
+      - uvicorn
+    status:
+      code: 404
+      message: Not Found
 version: 1
```

### Comparing `opperai-0.6.2/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function_with_cache.yaml` & `opperai-0.7.0/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function_with_cache.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,23 @@
       - '*/*'
       connection:
       - keep-alive
     method: GET
     uri: http://localhost:8000/v1/functions/by_path/test/sdk/test_create_function_with_cache_async
   response:
     body:
-      string: '{"detail":"Function not found"}'
+      string: '{"errors":[{"type":"HTTPException","message":"Function not found","detail":"Function
+        not found"}]}'
     headers:
       content-length:
-      - '31'
+      - '98'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 10:52:29 GMT
+      - Tue, 21 May 2024 10:10:03 GMT
       server:
       - uvicorn
     status:
       code: 404
       message: Not Found
 - request:
     body: '{"id": null, "path": "test/sdk/test_create_function_with_cache_async",
@@ -38,23 +39,23 @@
       - '395'
       content-type:
       - application/json
     method: POST
     uri: http://localhost:8000/v1/functions
   response:
     body:
-      string: '{"id":73,"path":"test/sdk/test_create_function_with_cache_async","description":"Test
-        function","input_schema":null,"out_schema":null,"instructions":"Do something","few_shot":false,"few_shot_count":2,"dataset_uuid":"8628e6fd-7519-4f50-9298-3f8da3db4f33","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
+      string: '{"path":"test/sdk/test_create_function_with_cache_async","instructions":"Do
+        something","id":35,"description":"Test function","input_schema":null,"out_schema":null,"few_shot":false,"few_shot_count":2,"dataset_uuid":"f2b18845-412e-41e5-949e-f72cd2679bc7","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
     headers:
       content-length:
       - '409'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 10:52:29 GMT
+      - Tue, 21 May 2024 10:10:03 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: '{"parent_span_uuid": null, "messages": [{"role": "user", "content": "hello"}]}'
@@ -67,24 +68,24 @@
       - '78'
       content-type:
       - application/json
     method: POST
     uri: http://localhost:8000/v1/chat/test/sdk/test_create_function_with_cache_async
   response:
     body:
-      string: '{"span_id":"1fc4ce18-b522-4015-bbb3-a84a39c79af4","message":"Hello!
+      string: '{"span_id":"b68eb0cb-96ed-4897-8909-81eeb8f710a9","message":"Hello!
         How can I assist you today? If you have any questions or need information
-        on a topic, feel free to ask.","json_payload":null,"error":null,"context":null,"cached":false}'
+        on a specific topic, feel free to ask.","json_payload":null,"context":null,"cached":false}'
     headers:
       content-length:
-      - '236'
+      - '232'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 10:52:30 GMT
+      - Tue, 21 May 2024 10:10:03 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: '{"parent_span_uuid": null, "messages": [{"role": "user", "content": "hello"}]}'
@@ -97,45 +98,45 @@
       - '78'
       content-type:
       - application/json
     method: POST
     uri: http://localhost:8000/v1/chat/test/sdk/test_create_function_with_cache_async
   response:
     body:
-      string: '{"span_id":"9688cdc4-261e-4fe1-8df1-0a2282dd3186","message":"Hello!
+      string: '{"span_id":"7a4baddc-7c53-4be7-9a8e-f28c1afa8e81","message":"Hello!
         How can I assist you today? If you have any questions or need information
-        on a topic, feel free to ask.","json_payload":null,"error":null,"context":null,"cached":true}'
+        on a specific topic, feel free to ask.","json_payload":null,"context":null,"cached":true}'
     headers:
       content-length:
-      - '235'
+      - '231'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 10:52:32 GMT
+      - Tue, 21 May 2024 10:10:07 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
     method: DELETE
-    uri: http://localhost:8000/v1/functions/73
+    uri: http://localhost:8000/v1/functions/35
   response:
     body:
       string: ''
     headers:
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 10:52:32 GMT
+      - Tue, 21 May 2024 10:10:07 GMT
       server:
       - uvicorn
     status:
       code: 204
       message: No Content
 version: 1
```

### Comparing `opperai-0.6.2/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function_with_cache_flush.yaml` & `opperai-0.7.0/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function_with_cache_flush.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,23 @@
       - '*/*'
       connection:
       - keep-alive
     method: GET
     uri: http://localhost:8000/v1/functions/by_path/test/sdk/test_create_function_with_cache_async_flush
   response:
     body:
-      string: '{"detail":"Function not found"}'
+      string: '{"errors":[{"type":"HTTPException","message":"Function not found","detail":"Function
+        not found"}]}'
     headers:
       content-length:
-      - '31'
+      - '98'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 10:52:32 GMT
+      - Tue, 21 May 2024 10:10:08 GMT
       server:
       - uvicorn
     status:
       code: 404
       message: Not Found
 - request:
     body: '{"id": null, "path": "test/sdk/test_create_function_with_cache_async_flush",
@@ -38,23 +39,23 @@
       - '401'
       content-type:
       - application/json
     method: POST
     uri: http://localhost:8000/v1/functions
   response:
     body:
-      string: '{"id":74,"path":"test/sdk/test_create_function_with_cache_async_flush","description":"Test
-        function","input_schema":null,"out_schema":null,"instructions":"Do something","few_shot":false,"few_shot_count":2,"dataset_uuid":"f755d0c0-8430-4052-8072-00a160c38fa8","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
+      string: '{"path":"test/sdk/test_create_function_with_cache_async_flush","instructions":"Do
+        something","id":36,"description":"Test function","input_schema":null,"out_schema":null,"few_shot":false,"few_shot_count":2,"dataset_uuid":"fd95b9e9-c1e7-44f4-865f-9a8b7445973d","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
     headers:
       content-length:
       - '415'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 10:52:32 GMT
+      - Tue, 21 May 2024 10:10:08 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: '{"parent_span_uuid": null, "messages": [{"role": "user", "content": "hello"}]}'
@@ -67,24 +68,23 @@
       - '78'
       content-type:
       - application/json
     method: POST
     uri: http://localhost:8000/v1/chat/test/sdk/test_create_function_with_cache_async_flush
   response:
     body:
-      string: '{"span_id":"08b7c1c3-b5bb-4304-97b7-2722aef33a1b","message":"Hello!
-        How can I assist you today? If you have any questions or need information
-        on a particular topic, feel free to ask.","json_payload":null,"error":null,"context":null,"cached":false}'
+      string: '{"span_id":"5ae75ab3-58d3-47ae-a329-c668987ab2ac","message":"Hello!
+        How can I assist you today?","json_payload":null,"context":null,"cached":false}'
     headers:
       content-length:
-      - '247'
+      - '147'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 10:52:32 GMT
+      - Tue, 21 May 2024 10:10:08 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: '{"parent_span_uuid": null, "messages": [{"role": "user", "content": "hello"}]}'
@@ -97,46 +97,45 @@
       - '78'
       content-type:
       - application/json
     method: POST
     uri: http://localhost:8000/v1/chat/test/sdk/test_create_function_with_cache_async_flush
   response:
     body:
-      string: '{"span_id":"d95bbcac-602b-49af-aaef-47002e271e28","message":"Hello!
-        How can I assist you today? If you have any questions or need information
-        on a particular topic, feel free to ask.","json_payload":null,"error":null,"context":null,"cached":true}'
+      string: '{"span_id":"b7e9e90e-064d-47f0-be27-db2b02c38f76","message":"Hello!
+        How can I assist you today?","json_payload":null,"context":null,"cached":true}'
     headers:
       content-length:
-      - '246'
+      - '146'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 10:52:34 GMT
+      - Tue, 21 May 2024 10:10:09 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
     method: DELETE
-    uri: http://localhost:8000/v1/functions/74/cache
+    uri: http://localhost:8000/v1/functions/36/cache
   response:
     body:
       string: ''
     headers:
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 10:52:34 GMT
+      - Tue, 21 May 2024 10:10:09 GMT
       server:
       - uvicorn
     status:
       code: 204
       message: No Content
 - request:
     body: '{"parent_span_uuid": null, "messages": [{"role": "user", "content": "hello"}]}'
@@ -149,45 +148,45 @@
       - '78'
       content-type:
       - application/json
     method: POST
     uri: http://localhost:8000/v1/chat/test/sdk/test_create_function_with_cache_async_flush
   response:
     body:
-      string: '{"span_id":"0041a12d-1433-4d75-988d-03e346f715b4","message":"Hello!
-        How can I assist you today? If you have any questions or need information
-        on a specific topic, feel free to ask.","json_payload":null,"error":null,"context":null,"cached":false}'
+      string: '{"span_id":"45543e05-daef-424d-b5bd-4870ae7da454","message":"Hello!
+        How can I assist you today? If you have any questions or need information,
+        feel free to ask.","json_payload":null,"context":null,"cached":false}'
     headers:
       content-length:
-      - '245'
+      - '212'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 10:52:34 GMT
+      - Tue, 21 May 2024 10:10:09 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
     method: DELETE
-    uri: http://localhost:8000/v1/functions/74
+    uri: http://localhost:8000/v1/functions/36
   response:
     body:
       string: ''
     headers:
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 10:52:36 GMT
+      - Tue, 21 May 2024 10:10:12 GMT
       server:
       - uvicorn
     status:
       code: 204
       message: No Content
 version: 1
```

### Comparing `opperai-0.6.2/tests/fixtures/vcr_cassettes/test_async_functions/test_delete_function.yaml` & `opperai-0.7.0/tests/fixtures/vcr_cassettes/test_async_functions/test_delete_function.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,23 @@
       - '*/*'
       connection:
       - keep-alive
     method: GET
     uri: http://localhost:8000/v1/functions/by_path/test/sdk/test_delete_function
   response:
     body:
-      string: '{"detail":"Function not found"}'
+      string: '{"errors":[{"type":"HTTPException","message":"Function not found","detail":"Function
+        not found"}]}'
     headers:
       content-length:
-      - '31'
+      - '98'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 10:52:28 GMT
+      - Tue, 21 May 2024 10:09:44 GMT
       server:
       - uvicorn
     status:
       code: 404
       message: Not Found
 - request:
     body: '{"id": null, "path": "test/sdk/test_delete_function", "description": "Test
@@ -37,68 +38,69 @@
       - '291'
       content-type:
       - application/json
     method: POST
     uri: http://localhost:8000/v1/functions
   response:
     body:
-      string: '{"id":70,"path":"test/sdk/test_delete_function","description":"Test
-        function","input_schema":null,"out_schema":null,"instructions":"Do something","few_shot":false,"few_shot_count":2,"dataset_uuid":"a40bf43d-a236-4b34-9095-9a4e73330f65","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
+      string: '{"path":"test/sdk/test_delete_function","instructions":"Do something","id":30,"description":"Test
+        function","input_schema":null,"out_schema":null,"few_shot":false,"few_shot_count":2,"dataset_uuid":"7a43dc5c-fd22-4c6d-bed4-efe966e6f163","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
     headers:
       content-length:
       - '392'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 10:52:28 GMT
+      - Tue, 21 May 2024 10:09:44 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
     method: DELETE
-    uri: http://localhost:8000/v1/functions/70
+    uri: http://localhost:8000/v1/functions/30
   response:
     body:
       string: ''
     headers:
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 10:52:28 GMT
+      - Tue, 21 May 2024 10:09:44 GMT
       server:
       - uvicorn
     status:
       code: 204
       message: No Content
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
     method: GET
-    uri: http://localhost:8000/v1/functions/70
+    uri: http://localhost:8000/v1/functions/30
   response:
     body:
-      string: '{"detail":"Function not found"}'
+      string: '{"errors":[{"type":"HTTPException","message":"Function not found","detail":"Function
+        not found"}]}'
     headers:
       content-length:
-      - '31'
+      - '98'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 10:52:28 GMT
+      - Tue, 21 May 2024 10:09:44 GMT
       server:
       - uvicorn
     status:
       code: 404
       message: Not Found
 version: 1
```

### Comparing `opperai-0.6.2/tests/fixtures/vcr_cassettes/test_async_functions/test_failed_structured_generation.yaml` & `opperai-0.7.0/tests/fixtures/vcr_cassettes/test_functions/test_failed_structured_generation.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -6,22 +6,23 @@
       - '*/*'
       connection:
       - keep-alive
     method: GET
     uri: http://localhost:8000/v1/functions/by_path/test/sdk/test_failed_structured_generation
   response:
     body:
-      string: '{"detail":"Function not found"}'
+      string: '{"errors":[{"type":"HTTPException","message":"Function not found","detail":"Function
+        not found"}]}'
     headers:
       content-length:
-      - '31'
+      - '98'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 10:46:24 GMT
+      - Tue, 21 May 2024 10:10:51 GMT
       server:
       - uvicorn
     status:
       code: 404
       message: Not Found
 - request:
     body: '{"id": null, "path": "test/sdk/test_failed_structured_generation", "description":
@@ -45,24 +46,24 @@
       - '985'
       content-type:
       - application/json
     method: POST
     uri: http://localhost:8000/v1/functions
   response:
     body:
-      string: '{"id":64,"path":"test/sdk/test_failed_structured_generation","description":"test
-        structured generation exception","input_schema":null,"out_schema":null,"instructions":"You
-        translate the incoming text to french","few_shot":false,"few_shot_count":2,"dataset_uuid":"ab9dbbaf-e647-4b5b-a69c-e3e768e2f11d","use_semantic_search":false,"model":"mistral/mistral-tiny-eu","language_model_id":4,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
+      string: '{"path":"test/sdk/test_failed_structured_generation","instructions":"You
+        translate the incoming text to french","id":50,"description":"test structured
+        generation exception","input_schema":null,"out_schema":null,"few_shot":false,"few_shot_count":2,"dataset_uuid":"b90e7886-2ed7-4a24-8798-e0d494f8b891","use_semantic_search":false,"model":"mistral/mistral-tiny-eu","language_model_id":4,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
     headers:
       content-length:
       - '467'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 10:46:24 GMT
+      - Tue, 21 May 2024 10:10:51 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: '{"parent_span_uuid": null, "messages": [{"role": "user", "content": "hello"}]}'
@@ -75,44 +76,45 @@
       - '78'
       content-type:
       - application/json
     method: POST
     uri: http://localhost:8000/v1/chat/test/sdk/test_failed_structured_generation
   response:
     body:
-      string: '{"detail":"Structured generation failed, could not generate response
-        matching the schema."}'
+      string: '{"errors":[{"type":"StructuredGenerationError","message":"Structured
+        generation failed, could not generate response matching the schema.","detail":"Structured
+        generation failed, could not generate response matching the schema."}]}'
     headers:
       content-length:
-      - '91'
+      - '230'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 10:46:24 GMT
+      - Tue, 21 May 2024 10:10:51 GMT
       server:
       - uvicorn
     status:
       code: 400
       message: Bad Request
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
     method: DELETE
-    uri: http://localhost:8000/v1/functions/64
+    uri: http://localhost:8000/v1/functions/50
   response:
     body:
       string: ''
     headers:
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 10:46:45 GMT
+      - Tue, 21 May 2024 10:10:57 GMT
       server:
       - uvicorn
     status:
       code: 204
       message: No Content
 version: 1
```

### Comparing `opperai-0.6.2/tests/fixtures/vcr_cassettes/test_async_functions/test_get.yaml` & `opperai-0.7.0/tests/fixtures/vcr_cassettes/test_async_functions/test_get.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -6,22 +6,23 @@
       - '*/*'
       connection:
       - keep-alive
     method: GET
     uri: http://localhost:8000/v1/functions/by_path/test/sdk/test_get
   response:
     body:
-      string: '{"detail":"Function not found"}'
+      string: '{"errors":[{"type":"HTTPException","message":"Function not found","detail":"Function
+        not found"}]}'
     headers:
       content-length:
-      - '31'
+      - '98'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 10:52:28 GMT
+      - Tue, 21 May 2024 10:09:44 GMT
       server:
       - uvicorn
     status:
       code: 404
       message: Not Found
 - request:
     body: '{"id": null, "path": "test/sdk/test_get", "description": "Test function",
@@ -37,48 +38,48 @@
       - '279'
       content-type:
       - application/json
     method: POST
     uri: http://localhost:8000/v1/functions
   response:
     body:
-      string: '{"id":68,"path":"test/sdk/test_get","description":"Test function","input_schema":null,"out_schema":null,"instructions":"Do
-        something","few_shot":false,"few_shot_count":2,"dataset_uuid":"0499d814-14f6-46cc-afd3-f8405b14c4d0","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
+      string: '{"path":"test/sdk/test_get","instructions":"Do something","id":28,"description":"Test
+        function","input_schema":null,"out_schema":null,"few_shot":false,"few_shot_count":2,"dataset_uuid":"bd611b17-b68e-4e33-80de-21cfe5456e8c","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
     headers:
       content-length:
       - '380'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 10:52:28 GMT
+      - Tue, 21 May 2024 10:09:44 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
     method: GET
-    uri: http://localhost:8000/v1/functions/68
+    uri: http://localhost:8000/v1/functions/28
   response:
     body:
-      string: '{"id":68,"path":"test/sdk/test_get","description":"Test function","input_schema":null,"out_schema":null,"instructions":"Do
-        something","few_shot":false,"few_shot_count":2,"dataset_uuid":"0499d814-14f6-46cc-afd3-f8405b14c4d0","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":{"exact_match_cache_ttl":0,"semantic_cache_threshold":0.95,"semantic_cache_ttl":0}}'
+      string: '{"path":"test/sdk/test_get","instructions":"Do something","id":28,"description":"Test
+        function","input_schema":null,"out_schema":null,"few_shot":false,"few_shot_count":2,"dataset_uuid":"bd611b17-b68e-4e33-80de-21cfe5456e8c","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":{"exact_match_cache_ttl":0,"semantic_cache_threshold":0.95,"semantic_cache_ttl":0}}'
     headers:
       content-length:
       - '458'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 10:52:28 GMT
+      - Tue, 21 May 2024 10:09:44 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
@@ -87,44 +88,44 @@
       - '*/*'
       connection:
       - keep-alive
     method: GET
     uri: http://localhost:8000/v1/functions/by_path/test/sdk/test_get
   response:
     body:
-      string: '{"id":68,"path":"test/sdk/test_get","description":"Test function","input_schema":null,"out_schema":null,"instructions":"Do
-        something","few_shot":false,"few_shot_count":2,"dataset_uuid":"0499d814-14f6-46cc-afd3-f8405b14c4d0","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":{"exact_match_cache_ttl":0,"semantic_cache_threshold":0.95,"semantic_cache_ttl":0}}'
+      string: '{"path":"test/sdk/test_get","instructions":"Do something","id":28,"description":"Test
+        function","input_schema":null,"out_schema":null,"few_shot":false,"few_shot_count":2,"dataset_uuid":"bd611b17-b68e-4e33-80de-21cfe5456e8c","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":{"exact_match_cache_ttl":0,"semantic_cache_threshold":0.95,"semantic_cache_ttl":0}}'
     headers:
       content-length:
       - '458'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 10:52:28 GMT
+      - Tue, 21 May 2024 10:09:44 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
     method: DELETE
-    uri: http://localhost:8000/v1/functions/68
+    uri: http://localhost:8000/v1/functions/28
   response:
     body:
       string: ''
     headers:
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 10:52:28 GMT
+      - Tue, 21 May 2024 10:09:44 GMT
       server:
       - uvicorn
     status:
       code: 204
       message: No Content
 version: 1
```

### Comparing `opperai-0.6.2/tests/fixtures/vcr_cassettes/test_async_functions/test_get_by_id.yaml` & `opperai-0.7.0/tests/fixtures/vcr_cassettes/test_functions/test_get_by_id.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -6,22 +6,23 @@
       - '*/*'
       connection:
       - keep-alive
     method: GET
     uri: http://localhost:8000/v1/functions/by_path/test/sdk/test_get_by_id
   response:
     body:
-      string: '{"detail":"Function not found"}'
+      string: '{"errors":[{"type":"HTTPException","message":"Function not found","detail":"Function
+        not found"}]}'
     headers:
       content-length:
-      - '31'
+      - '98'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 10:52:28 GMT
+      - Tue, 21 May 2024 10:10:21 GMT
       server:
       - uvicorn
     status:
       code: 404
       message: Not Found
 - request:
     body: '{"id": null, "path": "test/sdk/test_get_by_id", "description": "Test function",
@@ -37,69 +38,69 @@
       - '285'
       content-type:
       - application/json
     method: POST
     uri: http://localhost:8000/v1/functions
   response:
     body:
-      string: '{"id":66,"path":"test/sdk/test_get_by_id","description":"Test function","input_schema":null,"out_schema":null,"instructions":"Do
-        something","few_shot":false,"few_shot_count":2,"dataset_uuid":"50969b89-33ce-4a1b-9676-1667695aa78e","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
+      string: '{"path":"test/sdk/test_get_by_id","instructions":"Do something","id":39,"description":"Test
+        function","input_schema":null,"out_schema":null,"few_shot":false,"few_shot_count":2,"dataset_uuid":"a8ef26c8-1ae9-4042-86e1-a639c13c7aa1","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
     headers:
       content-length:
       - '386'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 10:52:28 GMT
+      - Tue, 21 May 2024 10:10:21 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
     method: GET
-    uri: http://localhost:8000/v1/functions/66
+    uri: http://localhost:8000/v1/functions/39
   response:
     body:
-      string: '{"id":66,"path":"test/sdk/test_get_by_id","description":"Test function","input_schema":null,"out_schema":null,"instructions":"Do
-        something","few_shot":false,"few_shot_count":2,"dataset_uuid":"50969b89-33ce-4a1b-9676-1667695aa78e","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":{"exact_match_cache_ttl":0,"semantic_cache_threshold":0.95,"semantic_cache_ttl":0}}'
+      string: '{"path":"test/sdk/test_get_by_id","instructions":"Do something","id":39,"description":"Test
+        function","input_schema":null,"out_schema":null,"few_shot":false,"few_shot_count":2,"dataset_uuid":"a8ef26c8-1ae9-4042-86e1-a639c13c7aa1","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":{"exact_match_cache_ttl":0,"semantic_cache_threshold":0.95,"semantic_cache_ttl":0}}'
     headers:
       content-length:
       - '464'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 10:52:28 GMT
+      - Tue, 21 May 2024 10:10:21 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
     method: DELETE
-    uri: http://localhost:8000/v1/functions/66
+    uri: http://localhost:8000/v1/functions/39
   response:
     body:
       string: ''
     headers:
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 10:52:28 GMT
+      - Tue, 21 May 2024 10:10:21 GMT
       server:
       - uvicorn
     status:
       code: 204
       message: No Content
 version: 1
```

### Comparing `opperai-0.6.2/tests/fixtures/vcr_cassettes/test_async_functions/test_get_by_path.yaml` & `opperai-0.7.0/tests/fixtures/vcr_cassettes/test_functions/test_delete_function_by_path.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -3,103 +3,104 @@
     body: ''
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
     method: GET
-    uri: http://localhost:8000/v1/functions/by_path/test/sdk/test_get_by_path
+    uri: http://localhost:8000/v1/functions/by_path/test/sdk/test_delete_function_by_path
   response:
     body:
-      string: '{"detail":"Function not found"}'
+      string: '{"errors":[{"type":"HTTPException","message":"Function not found","detail":"Function
+        not found"}]}'
     headers:
       content-length:
-      - '31'
+      - '98'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 10:52:28 GMT
+      - Tue, 21 May 2024 10:10:21 GMT
       server:
       - uvicorn
     status:
       code: 404
       message: Not Found
 - request:
-    body: '{"id": null, "path": "test/sdk/test_get_by_path", "description": "Test
-      function", "input_schema": null, "out_schema": null, "instructions": "Do something",
-      "model": null, "index_ids": [], "use_semantic_search": null, "few_shot": null,
-      "few_shot_count": null, "cache_configuration": null}'
+    body: '{"id": null, "path": "test/sdk/test_delete_function_by_path", "description":
+      "Test function", "input_schema": null, "out_schema": null, "instructions": "Do
+      something", "model": null, "index_ids": [], "use_semantic_search": null, "few_shot":
+      null, "few_shot_count": null, "cache_configuration": null}'
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
       content-length:
-      - '287'
+      - '299'
       content-type:
       - application/json
     method: POST
     uri: http://localhost:8000/v1/functions
   response:
     body:
-      string: '{"id":67,"path":"test/sdk/test_get_by_path","description":"Test function","input_schema":null,"out_schema":null,"instructions":"Do
-        something","few_shot":false,"few_shot_count":2,"dataset_uuid":"4e22a996-0444-41b2-8921-3aaaf20f0af8","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
+      string: '{"path":"test/sdk/test_delete_function_by_path","instructions":"Do
+        something","id":43,"description":"Test function","input_schema":null,"out_schema":null,"few_shot":false,"few_shot_count":2,"dataset_uuid":"dbbab2e1-6a23-49e8-9486-4452155ef9e1","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
     headers:
       content-length:
-      - '388'
+      - '400'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 10:52:28 GMT
+      - Tue, 21 May 2024 10:10:21 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
-    method: GET
-    uri: http://localhost:8000/v1/functions/by_path/test/sdk/test_get_by_path
+    method: DELETE
+    uri: http://localhost:8000/v1/functions/by_path/test/sdk/test_delete_function_by_path
   response:
     body:
-      string: '{"id":67,"path":"test/sdk/test_get_by_path","description":"Test function","input_schema":null,"out_schema":null,"instructions":"Do
-        something","few_shot":false,"few_shot_count":2,"dataset_uuid":"4e22a996-0444-41b2-8921-3aaaf20f0af8","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":{"exact_match_cache_ttl":0,"semantic_cache_threshold":0.95,"semantic_cache_ttl":0}}'
+      string: ''
     headers:
-      content-length:
-      - '466'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 10:52:28 GMT
+      - Tue, 21 May 2024 10:10:21 GMT
       server:
       - uvicorn
     status:
-      code: 200
-      message: OK
+      code: 204
+      message: No Content
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
-    method: DELETE
-    uri: http://localhost:8000/v1/functions/67
+    method: GET
+    uri: http://localhost:8000/v1/functions/by_path/test/sdk/test_delete_function_by_path
   response:
     body:
-      string: ''
+      string: '{"errors":[{"type":"HTTPException","message":"Function not found","detail":"Function
+        not found"}]}'
     headers:
+      content-length:
+      - '98'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 10:52:28 GMT
+      - Tue, 21 May 2024 10:10:21 GMT
       server:
       - uvicorn
     status:
-      code: 204
-      message: No Content
+      code: 404
+      message: Not Found
 version: 1
```

### Comparing `opperai-0.6.2/tests/fixtures/vcr_cassettes/test_async_functions/test_image_file.yaml` & `opperai-0.7.0/tests/fixtures/vcr_cassettes/test_async_functions/test_image_file.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,23 @@
       - '*/*'
       connection:
       - keep-alive
     method: GET
     uri: http://localhost:8000/v1/functions/by_path/test/sdk/test_image
   response:
     body:
-      string: '{"detail":"Function not found"}'
+      string: '{"errors":[{"type":"HTTPException","message":"Function not found","detail":"Function
+        not found"}]}'
     headers:
       content-length:
-      - '31'
+      - '98'
       content-type:
       - application/json
       date:
-      - Mon, 13 May 2024 11:25:05 GMT
+      - Tue, 21 May 2024 10:09:52 GMT
       server:
       - uvicorn
     status:
       code: 404
       message: Not Found
 - request:
     body: '{"id": null, "path": "test/sdk/test_image", "description": null, "input_schema":
@@ -37,46 +38,46 @@
       - '291'
       content-type:
       - application/json
     method: POST
     uri: http://localhost:8000/v1/functions
   response:
     body:
-      string: '{"path":"test/sdk/test_image","instructions":"describe the image","id":183,"description":null,"input_schema":null,"out_schema":null,"few_shot":false,"few_shot_count":2,"dataset_uuid":"1fc8e34c-6132-4a51-842f-e7c248cd9412","use_semantic_search":false,"model":"openai/gpt4-turbo","language_model_id":1,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
+      string: '{"path":"test/sdk/test_image","instructions":"describe the image","id":32,"description":null,"input_schema":null,"out_schema":null,"few_shot":false,"few_shot_count":2,"dataset_uuid":"ae8b0e84-9aab-4b34-835f-0fc14e9682c9","use_semantic_search":false,"model":"openai/gpt4-turbo","language_model_id":1,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
     headers:
       content-length:
-      - '382'
+      - '381'
       content-type:
       - application/json
       date:
-      - Mon, 13 May 2024 11:25:05 GMT
+      - Tue, 21 May 2024 10:09:52 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
     method: GET
-    uri: http://localhost:8000/v1/functions/183
+    uri: http://localhost:8000/v1/functions/32
   response:
     body:
-      string: '{"path":"test/sdk/test_image","instructions":"describe the image","id":183,"description":null,"input_schema":null,"out_schema":null,"few_shot":false,"few_shot_count":2,"dataset_uuid":"1fc8e34c-6132-4a51-842f-e7c248cd9412","use_semantic_search":false,"model":"openai/gpt4-turbo","language_model_id":1,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":{"exact_match_cache_ttl":0,"semantic_cache_threshold":0.95,"semantic_cache_ttl":0}}'
+      string: '{"path":"test/sdk/test_image","instructions":"describe the image","id":32,"description":null,"input_schema":null,"out_schema":null,"few_shot":false,"few_shot_count":2,"dataset_uuid":"ae8b0e84-9aab-4b34-835f-0fc14e9682c9","use_semantic_search":false,"model":"openai/gpt4-turbo","language_model_id":1,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":{"exact_match_cache_ttl":0,"semantic_cache_threshold":0.95,"semantic_cache_ttl":0}}'
     headers:
       content-length:
-      - '460'
+      - '459'
       content-type:
       - application/json
       date:
-      - Mon, 13 May 2024 11:25:05 GMT
+      - Tue, 21 May 2024 10:09:52 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: '{"parent_span_uuid": null, "messages": [{"role": "user", "content": [{"type":
@@ -90,52 +91,51 @@
       - '231975'
       content-type:
       - application/json
     method: POST
     uri: http://localhost:8000/v1/chat/test/sdk/test_image
   response:
     body:
-      string: '{"span_id":"ae4ff934-9926-4f17-b9d0-24b73d494347","message":"The image
-        shows an ancient fossil of an animal, impressively preserved and displayed
-        on a flat surface. The skeleton appears to be that of a small, prehistoric
-        reptile or mammal-like reptile, embedded in a craggy, light-colored stone
-        matrix that contrasts with the darker color of the bones. The animal''s head,
-        with its distinct eye socket, and elongated body are clear. The skeletal structure
-        suggests it has a well-defined rib cage and limbs, indicating it possibly
-        moved actively during its lifetime. This fossil provides a valuable glimpse
-        into the anatomy and possible lifestyle of creatures from remote geological
-        periods.","json_payload":null,"context":null,"cached":false}'
+      string: '{"span_id":"d2157133-c047-45cb-9645-1c7980011402","message":"The image
+        shows a fossil embedded in a stone slab. The fossil appears to be that of
+        a small, reptilian creature, possibly a dinosaur or a similar prehistoric
+        animal. It is prominently displayed in a good state of preservation with clear
+        visibility of the skeletal structure, including the skull, vertebral column,
+        ribs, and limbs. The fossil is well-articulated, suggesting it was buried
+        quickly or in a low-energy environment that preserved its original arrangement.
+        Its presentation is museum-like, with the slab laid flat and illuminated,
+        likely to highlight details for educational or exhibition purposes.","json_payload":null,"context":null,"cached":false}'
     headers:
       content-length:
-      - '741'
+      - '722'
       content-type:
       - application/json
       date:
-      - Mon, 13 May 2024 11:25:05 GMT
+      - Tue, 21 May 2024 10:09:52 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
     method: DELETE
-    uri: http://localhost:8000/v1/functions/183
+    uri: http://localhost:8000/v1/functions/32
   response:
     body:
       string: ''
     headers:
       content-type:
       - application/json
       date:
-      - Mon, 13 May 2024 11:25:18 GMT
+      - Tue, 21 May 2024 10:10:02 GMT
       server:
       - uvicorn
     status:
       code: 204
       message: No Content
 version: 1
```

### Comparing `opperai-0.6.2/tests/fixtures/vcr_cassettes/test_async_functions/test_image_url.yaml` & `opperai-0.7.0/tests/fixtures/vcr_cassettes/test_functions/test_image_url.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -6,22 +6,23 @@
       - '*/*'
       connection:
       - keep-alive
     method: GET
     uri: http://localhost:8000/v1/functions/by_path/test/sdk/test_image
   response:
     body:
-      string: '{"detail":"Function not found"}'
+      string: '{"errors":[{"type":"HTTPException","message":"Function not found","detail":"Function
+        not found"}]}'
     headers:
       content-length:
-      - '31'
+      - '98'
       content-type:
       - application/json
       date:
-      - Mon, 13 May 2024 11:24:37 GMT
+      - Tue, 21 May 2024 10:10:21 GMT
       server:
       - uvicorn
     status:
       code: 404
       message: Not Found
 - request:
     body: '{"id": null, "path": "test/sdk/test_image", "description": null, "input_schema":
@@ -37,46 +38,46 @@
       - '291'
       content-type:
       - application/json
     method: POST
     uri: http://localhost:8000/v1/functions
   response:
     body:
-      string: '{"path":"test/sdk/test_image","instructions":"describe the image","id":182,"description":null,"input_schema":null,"out_schema":null,"few_shot":false,"few_shot_count":2,"dataset_uuid":"91475eb6-b617-4160-92c6-253282b24961","use_semantic_search":false,"model":"openai/gpt4-turbo","language_model_id":1,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
+      string: '{"path":"test/sdk/test_image","instructions":"describe the image","id":44,"description":null,"input_schema":null,"out_schema":null,"few_shot":false,"few_shot_count":2,"dataset_uuid":"6db40da6-c469-4c3b-bb65-fcd752a431fb","use_semantic_search":false,"model":"openai/gpt4-turbo","language_model_id":1,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
     headers:
       content-length:
-      - '382'
+      - '381'
       content-type:
       - application/json
       date:
-      - Mon, 13 May 2024 11:24:37 GMT
+      - Tue, 21 May 2024 10:10:21 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
     method: GET
-    uri: http://localhost:8000/v1/functions/182
+    uri: http://localhost:8000/v1/functions/44
   response:
     body:
-      string: '{"path":"test/sdk/test_image","instructions":"describe the image","id":182,"description":null,"input_schema":null,"out_schema":null,"few_shot":false,"few_shot_count":2,"dataset_uuid":"91475eb6-b617-4160-92c6-253282b24961","use_semantic_search":false,"model":"openai/gpt4-turbo","language_model_id":1,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":{"exact_match_cache_ttl":0,"semantic_cache_threshold":0.95,"semantic_cache_ttl":0}}'
+      string: '{"path":"test/sdk/test_image","instructions":"describe the image","id":44,"description":null,"input_schema":null,"out_schema":null,"few_shot":false,"few_shot_count":2,"dataset_uuid":"6db40da6-c469-4c3b-bb65-fcd752a431fb","use_semantic_search":false,"model":"openai/gpt4-turbo","language_model_id":1,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":{"exact_match_cache_ttl":0,"semantic_cache_threshold":0.95,"semantic_cache_ttl":0}}'
     headers:
       content-length:
-      - '460'
+      - '459'
       content-type:
       - application/json
       date:
-      - Mon, 13 May 2024 11:24:37 GMT
+      - Tue, 21 May 2024 10:10:21 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: '{"parent_span_uuid": null, "messages": [{"role": "user", "content": [{"type":
@@ -90,51 +91,52 @@
       - '251'
       content-type:
       - application/json
     method: POST
     uri: http://localhost:8000/v1/chat/test/sdk/test_image
   response:
     body:
-      string: '{"span_id":"8dcb500e-e2b6-4c31-8aba-bba667130742","message":"This image
-        displays a fossil embedded in a rock slab, which appears to be from a small
-        dinosaur or reptile. The fossil includes a well-preserved skeleton with a
-        clear outline of the skull, vertebrae, ribs, limbs, and tail. The rock matrix
-        surrounding the fossil is relatively smooth and light-colored, highlighting
-        the darker tones of the bones. This specimen is excellently preserved, showing
-        intricate details of the bone structure, which can be very helpful for scientific
-        study and educational purposes. The lighting and the dark background enhance
-        the visibility of the fossil''s details.","json_payload":null,"context":null,"cached":false}'
+      string: '{"span_id":"9b17ef15-368e-446d-b9ea-a338423bc54f","message":"The image
+        displays a fossil of a prehistoric reptile, possibly a dinosaur or similar
+        creature, embedded in a stone slab. The fossil is remarkably well-preserved,
+        showing intricate details. The skeleton is largely intact with a clearly recognizable
+        skull, spine, ribs, and limbs. The texture of the stone contrasts with the
+        darker coloration of the fossilized remains, emphasizing the form and structure
+        of the creature. The backdrop is a simple black, which highlights the fossil
+        and the subtleties of its preservation on the slab. This type of specimen
+        is essential for paleontological studies, offering insights into the anatomy
+        and possible lifestyle of extinct species.","json_payload":null,"context":null,"cached":false}'
     headers:
       content-length:
-      - '705'
+      - '786'
       content-type:
       - application/json
       date:
-      - Mon, 13 May 2024 11:24:37 GMT
+      - Tue, 21 May 2024 10:10:21 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
     method: DELETE
-    uri: http://localhost:8000/v1/functions/182
+    uri: http://localhost:8000/v1/functions/44
   response:
     body:
       string: ''
     headers:
       content-type:
       - application/json
       date:
-      - Mon, 13 May 2024 11:25:05 GMT
+      - Tue, 21 May 2024 10:10:30 GMT
       server:
       - uvicorn
     status:
       code: 204
       message: No Content
 version: 1
```

### Comparing `opperai-0.6.2/tests/fixtures/vcr_cassettes/test_async_functions/test_update_function.yaml` & `opperai-0.7.0/tests/fixtures/vcr_cassettes/test_async_functions/test_update_function.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,23 @@
       - '*/*'
       connection:
       - keep-alive
     method: GET
     uri: http://localhost:8000/v1/functions/by_path/test/sdk/test_update_function
   response:
     body:
-      string: '{"detail":"Function not found"}'
+      string: '{"errors":[{"type":"HTTPException","message":"Function not found","detail":"Function
+        not found"}]}'
     headers:
       content-length:
-      - '31'
+      - '98'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 10:52:28 GMT
+      - Tue, 21 May 2024 10:09:44 GMT
       server:
       - uvicorn
     status:
       code: 404
       message: Not Found
 - request:
     body: '{"id": null, "path": "test/sdk/test_update_function", "description": "Test
@@ -37,77 +38,76 @@
       - '291'
       content-type:
       - application/json
     method: POST
     uri: http://localhost:8000/v1/functions
   response:
     body:
-      string: '{"id":69,"path":"test/sdk/test_update_function","description":"Test
-        function","input_schema":null,"out_schema":null,"instructions":"Do something","few_shot":false,"few_shot_count":2,"dataset_uuid":"dd72b71a-ca0d-45bc-bf60-29651f5fffcf","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
+      string: '{"path":"test/sdk/test_update_function","instructions":"Do something","id":29,"description":"Test
+        function","input_schema":null,"out_schema":null,"few_shot":false,"few_shot_count":2,"dataset_uuid":"9da46a32-c839-4d04-b9e3-63f32cb5260e","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
     headers:
       content-length:
       - '392'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 10:52:28 GMT
+      - Tue, 21 May 2024 10:09:44 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
-    body: '{"id": 69, "path": "test/sdk/test_update_function", "description": "Test
+    body: '{"id": 29, "path": "test/sdk/test_update_function", "description": "Test
       function", "input_schema": null, "out_schema": null, "instructions": "Do something
       else", "model": "azure/gpt4-eu", "index_ids": [], "use_semantic_search": false,
       "few_shot": false, "few_shot_count": 2, "cache_configuration": null}'
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
       content-length:
       - '304'
       content-type:
       - application/json
     method: PATCH
-    uri: http://localhost:8000/v1/functions/69
+    uri: http://localhost:8000/v1/functions/29
   response:
     body:
-      string: '{"id":69,"path":"test/sdk/test_update_function","description":"Test
-        function","input_schema":null,"out_schema":null,"instructions":"Do something
-        else","few_shot":false,"few_shot_count":2,"dataset_uuid":"dd72b71a-ca0d-45bc-bf60-29651f5fffcf","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":2,"cache_configuration":{"exact_match_cache_ttl":0,"semantic_cache_threshold":0.95,"semantic_cache_ttl":0}}'
+      string: '{"path":"test/sdk/test_update_function","instructions":"Do something
+        else","id":29,"description":"Test function","input_schema":null,"out_schema":null,"few_shot":false,"few_shot_count":2,"dataset_uuid":"9da46a32-c839-4d04-b9e3-63f32cb5260e","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":2,"cache_configuration":{"exact_match_cache_ttl":0,"semantic_cache_threshold":0.95,"semantic_cache_ttl":0}}'
     headers:
       content-length:
       - '475'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 10:52:28 GMT
+      - Tue, 21 May 2024 10:09:44 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
     method: DELETE
-    uri: http://localhost:8000/v1/functions/69
+    uri: http://localhost:8000/v1/functions/29
   response:
     body:
       string: ''
     headers:
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 10:52:28 GMT
+      - Tue, 21 May 2024 10:09:44 GMT
       server:
       - uvicorn
     status:
       code: 204
       message: No Content
 version: 1
```

### Comparing `opperai-0.6.2/tests/fixtures/vcr_cassettes/test_async_indexes/test_create_index.yaml` & `opperai-0.7.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_create_index.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -10,45 +10,45 @@
       - '29'
       content-type:
       - application/json
     method: POST
     uri: http://localhost:8000/v1/indexes
   response:
     body:
-      string: '{"id":22,"name":"test_create_index","files":[],"created_at":"2024-05-02T10:54:43.324416Z"}'
+      string: '{"id":1,"name":"test_create_index","files":[],"created_at":"2024-05-21T09:54:22.806557Z"}'
     headers:
       content-length:
-      - '90'
+      - '89'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 10:54:42 GMT
+      - Tue, 21 May 2024 09:54:22 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
     method: DELETE
-    uri: http://localhost:8000/v1/indexes/22
+    uri: http://localhost:8000/v1/indexes/1
   response:
     body:
       string: 'true'
     headers:
       content-length:
       - '4'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 10:54:42 GMT
+      - Tue, 21 May 2024 09:54:22 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `opperai-0.6.2/tests/fixtures/vcr_cassettes/test_async_indexes/test_delete_index.yaml` & `opperai-0.7.0/tests/fixtures/vcr_cassettes/test_indexes/test_get_by_id.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -1,102 +1,78 @@
 interactions:
 - request:
-    body: '{"name": "test_delete_index"}'
+    body: '{"name": "test_get_by_id"}'
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
       content-length:
-      - '29'
+      - '26'
       content-type:
       - application/json
     method: POST
     uri: http://localhost:8000/v1/indexes
   response:
     body:
-      string: '{"id":23,"name":"test_delete_index","files":[],"created_at":"2024-05-02T10:54:43.383662Z"}'
+      string: '{"id":12,"name":"test_get_by_id","files":[],"created_at":"2024-05-21T10:10:58.713906Z"}'
     headers:
       content-length:
-      - '90'
+      - '87'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 10:54:43 GMT
+      - Tue, 21 May 2024 10:10:58 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
-    method: DELETE
-    uri: http://localhost:8000/v1/indexes/23
+    method: GET
+    uri: http://localhost:8000/v1/indexes/12
   response:
     body:
-      string: 'true'
+      string: '{"id":12,"name":"test_get_by_id","files":[],"created_at":"2024-05-21T10:10:58.713906Z"}'
     headers:
       content-length:
-      - '4'
+      - '87'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 10:54:43 GMT
+      - Tue, 21 May 2024 10:10:58 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
-    method: GET
-    uri: http://localhost:8000/v1/indexes/23
-  response:
-    body:
-      string: '{"detail":"Index not found"}'
-    headers:
-      content-length:
-      - '28'
-      content-type:
-      - application/json
-      date:
-      - Thu, 02 May 2024 10:54:43 GMT
-      server:
-      - uvicorn
-    status:
-      code: 404
-      message: Not Found
-- request:
-    body: ''
-    headers:
-      accept:
-      - '*/*'
-      connection:
-      - keep-alive
     method: DELETE
-    uri: http://localhost:8000/v1/indexes/23
+    uri: http://localhost:8000/v1/indexes/12
   response:
     body:
-      string: '{"detail":"Index not found"}'
+      string: 'true'
     headers:
       content-length:
-      - '28'
+      - '4'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 10:54:43 GMT
+      - Tue, 21 May 2024 10:10:58 GMT
       server:
       - uvicorn
     status:
-      code: 404
-      message: Not Found
+      code: 200
+      message: OK
 version: 1
```

### Comparing `opperai-0.6.2/tests/fixtures/vcr_cassettes/test_async_indexes/test_get_by_id.yaml` & `opperai-0.7.0/tests/fixtures/vcr_cassettes/test_indexes/test_index_document.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,78 +1,83 @@
 interactions:
 - request:
-    body: '{"name": "test_get_by_id"}'
+    body: '{"name": "test_index_document"}'
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
       content-length:
-      - '26'
+      - '31'
       content-type:
       - application/json
     method: POST
     uri: http://localhost:8000/v1/indexes
   response:
     body:
-      string: '{"id":24,"name":"test_get_by_id","files":[],"created_at":"2024-05-02T10:54:43.425668Z"}'
+      string: '{"id":16,"name":"test_index_document","files":[],"created_at":"2024-05-21T10:10:58.938484Z"}'
     headers:
       content-length:
-      - '87'
+      - '92'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 10:54:43 GMT
+      - Tue, 21 May 2024 10:10:58 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
-    body: ''
+    body: '{"id": null, "uuid": null, "key": null, "content": "Hello", "metadata":
+      {"source": "test"}}'
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
-    method: GET
-    uri: http://localhost:8000/v1/indexes/24
+      content-length:
+      - '91'
+      content-type:
+      - application/json
+    method: POST
+    uri: http://localhost:8000/v1/indexes/16/index
   response:
     body:
-      string: '{"id":24,"name":"test_get_by_id","files":[],"created_at":"2024-05-02T10:54:43.425668Z"}'
+      string: '{"id":4,"uuid":"92de1367-4e21-4e27-9573-a5863229aa15","key":"92de1367-4e21-4e27-9573-a5863229aa15"}'
     headers:
       content-length:
-      - '87'
+      - '99'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 10:54:43 GMT
+      - Tue, 21 May 2024 10:10:58 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
     method: DELETE
-    uri: http://localhost:8000/v1/indexes/24
+    uri: http://localhost:8000/v1/indexes/16
   response:
     body:
       string: 'true'
     headers:
       content-length:
       - '4'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 10:54:43 GMT
+      - Tue, 21 May 2024 10:10:58 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `opperai-0.6.2/tests/fixtures/vcr_cassettes/test_async_indexes/test_get_by_name.yaml` & `opperai-0.7.0/tests/fixtures/vcr_cassettes/test_indexes/test_get_by_name.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -10,22 +10,22 @@
       - '28'
       content-type:
       - application/json
     method: POST
     uri: http://localhost:8000/v1/indexes
   response:
     body:
-      string: '{"id":25,"name":"test_get_by_name","files":[],"created_at":"2024-05-02T10:54:43.459696Z"}'
+      string: '{"id":13,"name":"test_get_by_name","files":[],"created_at":"2024-05-21T10:10:58.756581Z"}'
     headers:
       content-length:
       - '89'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 10:54:43 GMT
+      - Tue, 21 May 2024 10:10:58 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
@@ -34,46 +34,46 @@
       - '*/*'
       connection:
       - keep-alive
     method: GET
     uri: http://localhost:8000/v1/indexes
   response:
     body:
-      string: '[{"id":25,"org_id":1,"org_name":null,"name":"test_get_by_name","created_by":"Mattias
-        Lundell","created_at":"2024-05-02T10:54:43.459696Z","updated_at":"2024-05-02T10:54:43.459696Z","count":0}]'
+      string: '[{"id":13,"org_id":1,"org_name":null,"name":"test_get_by_name","created_by":"Mattias
+        Lundell","created_at":"2024-05-21T10:10:58.756581Z","updated_at":"2024-05-21T10:10:58.756581Z","count":0}]'
     headers:
       content-length:
       - '191'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 10:54:43 GMT
+      - Tue, 21 May 2024 10:10:58 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
     method: DELETE
-    uri: http://localhost:8000/v1/indexes/25
+    uri: http://localhost:8000/v1/indexes/13
   response:
     body:
       string: 'true'
     headers:
       content-length:
       - '4'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 10:54:43 GMT
+      - Tue, 21 May 2024 10:10:58 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `opperai-0.6.2/tests/fixtures/vcr_cassettes/test_async_indexes/test_index_document.yaml` & `opperai-0.7.0/tests/fixtures/vcr_cassettes/test_indexes/test_delete_index.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,83 +1,79 @@
 interactions:
 - request:
-    body: '{"name": "test_index_document"}'
+    body: '{"name": "test_delete_index"}'
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
       content-length:
-      - '31'
+      - '29'
       content-type:
       - application/json
     method: POST
     uri: http://localhost:8000/v1/indexes
   response:
     body:
-      string: '{"id":28,"name":"test_index_document","files":[],"created_at":"2024-05-02T10:54:43.552742Z"}'
+      string: '{"id":11,"name":"test_delete_index","files":[],"created_at":"2024-05-21T10:10:58.634013Z"}'
     headers:
       content-length:
-      - '92'
+      - '90'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 10:54:43 GMT
+      - Tue, 21 May 2024 10:10:58 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
-    body: '{"id": null, "uuid": null, "key": null, "content": "Hello", "metadata":
-      {"source": "test"}}'
+    body: ''
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
-      content-length:
-      - '91'
-      content-type:
-      - application/json
-    method: POST
-    uri: http://localhost:8000/v1/indexes/28/index
+    method: DELETE
+    uri: http://localhost:8000/v1/indexes/11
   response:
     body:
-      string: '{"id":12,"uuid":"a36fd9f3-051f-4bb0-b2bb-d85ed56f44a3","key":"a36fd9f3-051f-4bb0-b2bb-d85ed56f44a3"}'
+      string: 'true'
     headers:
       content-length:
-      - '100'
+      - '4'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 10:54:43 GMT
+      - Tue, 21 May 2024 10:10:58 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
-    method: DELETE
-    uri: http://localhost:8000/v1/indexes/28
+    method: GET
+    uri: http://localhost:8000/v1/indexes/11
   response:
     body:
-      string: 'true'
+      string: '{"errors":[{"type":"HTTPException","message":"Index not found","detail":"Index
+        not found"}]}'
     headers:
       content-length:
-      - '4'
+      - '92'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 10:54:43 GMT
+      - Tue, 21 May 2024 10:10:58 GMT
       server:
       - uvicorn
     status:
-      code: 200
-      message: OK
+      code: 404
+      message: Not Found
 version: 1
```

### Comparing `opperai-0.6.2/tests/fixtures/vcr_cassettes/test_async_indexes/test_list_indexes.yaml` & `opperai-0.7.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_list_indexes.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -13,15 +13,15 @@
       string: '[]'
     headers:
       content-length:
       - '2'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 10:54:43 GMT
+      - Tue, 21 May 2024 09:54:22 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: '{"name": "test_list_indexes"}'
@@ -34,22 +34,22 @@
       - '29'
       content-type:
       - application/json
     method: POST
     uri: http://localhost:8000/v1/indexes
   response:
     body:
-      string: '{"id":26,"name":"test_list_indexes","files":[],"created_at":"2024-05-02T10:54:43.494792Z"}'
+      string: '{"id":5,"name":"test_list_indexes","files":[],"created_at":"2024-05-21T09:54:23.021698Z"}'
     headers:
       content-length:
-      - '90'
+      - '89'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 10:54:43 GMT
+      - Tue, 21 May 2024 09:54:22 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
@@ -58,23 +58,23 @@
       - '*/*'
       connection:
       - keep-alive
     method: GET
     uri: http://localhost:8000/v1/indexes
   response:
     body:
-      string: '[{"id":26,"org_id":1,"org_name":null,"name":"test_list_indexes","created_by":"Mattias
-        Lundell","created_at":"2024-05-02T10:54:43.494792Z","updated_at":"2024-05-02T10:54:43.494792Z","count":0}]'
+      string: '[{"id":5,"org_id":1,"org_name":null,"name":"test_list_indexes","created_by":"Mattias
+        Lundell","created_at":"2024-05-21T09:54:23.021698Z","updated_at":"2024-05-21T09:54:23.021698Z","count":0}]'
     headers:
       content-length:
-      - '192'
+      - '191'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 10:54:43 GMT
+      - Tue, 21 May 2024 09:54:22 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: '{"name": "test_list_indexes_2"}'
@@ -87,22 +87,22 @@
       - '31'
       content-type:
       - application/json
     method: POST
     uri: http://localhost:8000/v1/indexes
   response:
     body:
-      string: '{"id":27,"name":"test_list_indexes_2","files":[],"created_at":"2024-05-02T10:54:43.512887Z"}'
+      string: '{"id":6,"name":"test_list_indexes_2","files":[],"created_at":"2024-05-21T09:54:23.052666Z"}'
     headers:
       content-length:
-      - '92'
+      - '91'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 10:54:43 GMT
+      - Tue, 21 May 2024 09:54:22 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
@@ -111,71 +111,71 @@
       - '*/*'
       connection:
       - keep-alive
     method: GET
     uri: http://localhost:8000/v1/indexes
   response:
     body:
-      string: '[{"id":26,"org_id":1,"org_name":null,"name":"test_list_indexes","created_by":"Mattias
-        Lundell","created_at":"2024-05-02T10:54:43.494792Z","updated_at":"2024-05-02T10:54:43.494792Z","count":0},{"id":27,"org_id":1,"org_name":null,"name":"test_list_indexes_2","created_by":"Mattias
-        Lundell","created_at":"2024-05-02T10:54:43.512887Z","updated_at":"2024-05-02T10:54:43.512887Z","count":0}]'
+      string: '[{"id":5,"org_id":1,"org_name":null,"name":"test_list_indexes","created_by":"Mattias
+        Lundell","created_at":"2024-05-21T09:54:23.021698Z","updated_at":"2024-05-21T09:54:23.021698Z","count":0},{"id":6,"org_id":1,"org_name":null,"name":"test_list_indexes_2","created_by":"Mattias
+        Lundell","created_at":"2024-05-21T09:54:23.052666Z","updated_at":"2024-05-21T09:54:23.052666Z","count":0}]'
     headers:
       content-length:
-      - '385'
+      - '383'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 10:54:43 GMT
+      - Tue, 21 May 2024 09:54:22 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
     method: DELETE
-    uri: http://localhost:8000/v1/indexes/27
+    uri: http://localhost:8000/v1/indexes/6
   response:
     body:
       string: 'true'
     headers:
       content-length:
       - '4'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 10:54:43 GMT
+      - Tue, 21 May 2024 09:54:22 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
     method: DELETE
-    uri: http://localhost:8000/v1/indexes/26
+    uri: http://localhost:8000/v1/indexes/5
   response:
     body:
       string: 'true'
     headers:
       content-length:
       - '4'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 10:54:43 GMT
+      - Tue, 21 May 2024 09:54:22 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `opperai-0.6.2/tests/fixtures/vcr_cassettes/test_async_indexes/test_retrieve_document.yaml` & `opperai-0.7.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_retrieve_filters.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,111 +1,112 @@
 interactions:
 - request:
-    body: '{"name": "test_retrieve_document"}'
+    body: '{"name": "test_retrieve_filters"}'
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
       content-length:
-      - '34'
+      - '33'
       content-type:
       - application/json
     method: POST
     uri: http://localhost:8000/v1/indexes
   response:
     body:
-      string: '{"id":29,"name":"test_retrieve_document","files":[],"created_at":"2024-05-02T10:54:43.991266Z"}'
+      string: '{"id":9,"name":"test_retrieve_filters","files":[],"created_at":"2024-05-21T09:54:24.437878Z"}'
     headers:
       content-length:
-      - '95'
+      - '93'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 10:54:43 GMT
+      - Tue, 21 May 2024 09:54:23 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
-    body: '{"id": null, "uuid": null, "key": null, "content": "Hello", "metadata":
+    body: '{"id": null, "uuid": null, "key": null, "content": "Bonjour", "metadata":
       {"source": "test"}}'
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
       content-length:
-      - '91'
+      - '93'
       content-type:
       - application/json
     method: POST
-    uri: http://localhost:8000/v1/indexes/29/index
+    uri: http://localhost:8000/v1/indexes/9/index
   response:
     body:
-      string: '{"id":13,"uuid":"ae40747e-b6a3-4649-ab53-d59cf77b3828","key":"ae40747e-b6a3-4649-ab53-d59cf77b3828"}'
+      string: '{"id":3,"uuid":"1f15dfff-cbcf-403f-b0e3-111303582bf4","key":"1f15dfff-cbcf-403f-b0e3-111303582bf4"}'
     headers:
       content-length:
-      - '100'
+      - '99'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 10:54:43 GMT
+      - Tue, 21 May 2024 09:54:24 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
-    body: '{"q": "Hello", "k": 1, "filters": null}'
+    body: '{"q": "test", "k": 1, "filters": [{"key": "source", "operation": "=", "value":
+      "test"}]}'
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
       content-length:
-      - '39'
+      - '88'
       content-type:
       - application/json
     method: POST
-    uri: http://localhost:8000/v1/indexes/29/query
+    uri: http://localhost:8000/v1/indexes/9/query
   response:
     body:
-      string: '[{"uuid":"fc3499e7-a601-4256-9a84-ecf7b8cc7458","content":"Hello","metadata":{"source":"test"},"document_id":null,"score":29.458036422729492,"source_uuids":["fc3499e7-a601-4256-9a84-ecf7b8cc7458"]}]'
+      string: '[{"uuid":"49be6c1a-7ad2-4c1a-b75e-a1d3d6642b22","content":"Bonjour","metadata":{"source":"test"},"document_id":null,"score":4.736573219299316,"source_uuids":["49be6c1a-7ad2-4c1a-b75e-a1d3d6642b22"]}]'
     headers:
       content-length:
-      - '198'
+      - '199'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 10:54:43 GMT
+      - Tue, 21 May 2024 09:54:24 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
     method: DELETE
-    uri: http://localhost:8000/v1/indexes/29
+    uri: http://localhost:8000/v1/indexes/9
   response:
     body:
       string: 'true'
     headers:
       content-length:
       - '4'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 10:54:43 GMT
+      - Tue, 21 May 2024 09:54:24 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `opperai-0.6.2/tests/fixtures/vcr_cassettes/test_async_indexes/test_retrieve_filters.yaml` & `opperai-0.7.0/tests/fixtures/vcr_cassettes/test_indexes/test_retrieve_document.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,112 +1,111 @@
 interactions:
 - request:
-    body: '{"name": "test_retrieve_filters"}'
+    body: '{"name": "test_retrieve_document"}'
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
       content-length:
-      - '33'
+      - '34'
       content-type:
       - application/json
     method: POST
     uri: http://localhost:8000/v1/indexes
   response:
     body:
-      string: '{"id":30,"name":"test_retrieve_filters","files":[],"created_at":"2024-05-02T10:54:44.462991Z"}'
+      string: '{"id":17,"name":"test_retrieve_document","files":[],"created_at":"2024-05-21T10:10:59.242625Z"}'
     headers:
       content-length:
-      - '94'
+      - '95'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 10:54:44 GMT
+      - Tue, 21 May 2024 10:10:58 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
-    body: '{"id": null, "uuid": null, "key": null, "content": "Bonjour", "metadata":
+    body: '{"id": null, "uuid": null, "key": null, "content": "Hello", "metadata":
       {"source": "test"}}'
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
       content-length:
-      - '93'
+      - '91'
       content-type:
       - application/json
     method: POST
-    uri: http://localhost:8000/v1/indexes/30/index
+    uri: http://localhost:8000/v1/indexes/17/index
   response:
     body:
-      string: '{"id":14,"uuid":"a8008a30-6a5e-4ab4-8ad0-eee61bc32eaa","key":"a8008a30-6a5e-4ab4-8ad0-eee61bc32eaa"}'
+      string: '{"id":5,"uuid":"ba1d3d58-032d-4e15-9bad-5ae7d2e292de","key":"ba1d3d58-032d-4e15-9bad-5ae7d2e292de"}'
     headers:
       content-length:
-      - '100'
+      - '99'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 10:54:44 GMT
+      - Tue, 21 May 2024 10:10:58 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
-    body: '{"q": "test", "k": 1, "filters": [{"key": "source", "operation": "=", "value":
-      "test"}]}'
+    body: '{"q": "Hello", "k": 1, "filters": null}'
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
       content-length:
-      - '88'
+      - '39'
       content-type:
       - application/json
     method: POST
-    uri: http://localhost:8000/v1/indexes/30/query
+    uri: http://localhost:8000/v1/indexes/17/query
   response:
     body:
-      string: '[{"uuid":"366fdf32-fba0-453c-ae3e-e3b6ce29289d","content":"Bonjour","metadata":{"source":"test"},"document_id":null,"score":4.736573219299316,"source_uuids":["366fdf32-fba0-453c-ae3e-e3b6ce29289d"]}]'
+      string: '[{"uuid":"17e7a097-53d7-4941-b47c-4d28cce727b4","content":"Hello","metadata":{"source":"test"},"document_id":null,"score":29.458036422729492,"source_uuids":["17e7a097-53d7-4941-b47c-4d28cce727b4"]}]'
     headers:
       content-length:
-      - '199'
+      - '198'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 10:54:44 GMT
+      - Tue, 21 May 2024 10:10:58 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
     method: DELETE
-    uri: http://localhost:8000/v1/indexes/30
+    uri: http://localhost:8000/v1/indexes/17
   response:
     body:
       string: 'true'
     headers:
       content-length:
       - '4'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 10:54:44 GMT
+      - Tue, 21 May 2024 10:10:59 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `opperai-0.6.2/tests/fixtures/vcr_cassettes/test_async_spans/test_async_crud.yaml` & `opperai-0.7.0/tests/fixtures/vcr_cassettes/test_async_spans/test_async_crud.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -16,15 +16,15 @@
       string: '{"uuid":"bcf1b3b4-0b3b-4b3b-8b3b-0b3b4b3b4112"}'
     headers:
       content-length:
       - '47'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 10:52:26 GMT
+      - Tue, 21 May 2024 09:54:24 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: '{"uuid": "cfc1c3c4-0c3c-4c3c-8c3c-0c3c4c31cc12", "project": "project",
@@ -44,15 +44,15 @@
       string: '{"uuid":"cfc1c3c4-0c3c-4c3c-8c3c-0c3c4c31cc12"}'
     headers:
       content-length:
       - '47'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 10:52:26 GMT
+      - Tue, 21 May 2024 09:54:24 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: '{"uuid": "cfc1c3c4-0c3c-4c3c-8c3c-0c3c4c31cc12", "output": "output", "end_time":
@@ -71,15 +71,15 @@
       string: '{"uuid":"cfc1c3c4-0c3c-4c3c-8c3c-0c3c4c31cc12"}'
     headers:
       content-length:
       - '47'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 10:52:26 GMT
+      - Tue, 21 May 2024 09:54:24 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: '{"uuid": "bcf1b3b4-0b3b-4b3b-8b3b-0b3b4b3b4112", "output": "output", "end_time":
@@ -98,15 +98,15 @@
       string: '{"uuid":"bcf1b3b4-0b3b-4b3b-8b3b-0b3b4b3b4112"}'
     headers:
       content-length:
       - '47'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 10:52:26 GMT
+      - Tue, 21 May 2024 09:54:24 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
@@ -120,15 +120,15 @@
   response:
     body:
       string: ''
     headers:
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 10:52:26 GMT
+      - Tue, 21 May 2024 09:54:24 GMT
       server:
       - uvicorn
     status:
       code: 204
       message: No Content
 - request:
     body: ''
@@ -142,14 +142,14 @@
   response:
     body:
       string: ''
     headers:
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 10:52:26 GMT
+      - Tue, 21 May 2024 09:54:24 GMT
       server:
       - uvicorn
     status:
       code: 204
       message: No Content
 version: 1
```

### Comparing `opperai-0.6.2/tests/fixtures/vcr_cassettes/test_async_spans/test_save_metric.yaml` & `opperai-0.7.0/tests/fixtures/vcr_cassettes/test_async_spans/test_save_metric.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -16,15 +16,15 @@
       string: '{"uuid":"bcf1b3b4-0b3b-4b3b-8b3b-0b3b4b3b4133"}'
     headers:
       content-length:
       - '47'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 13:23:01 GMT
+      - Tue, 21 May 2024 09:54:24 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: '{"dimension": "dim", "value": 0.5, "comment": "comment"}'
@@ -37,22 +37,22 @@
       - '56'
       content-type:
       - application/json
     method: POST
     uri: http://localhost:8000/v1/spans/bcf1b3b4-0b3b-4b3b-8b3b-0b3b4b3b4133/metrics
   response:
     body:
-      string: '{"id":"0bf87615-d886-405b-a696-e10e9eacf787","span_id":"bcf1b3b4-0b3b-4b3b-8b3b-0b3b4b3b4133","dimension":"dim","value":null,"comment":"comment","updated_at":null,"created_at":"2024-05-02T13:23:02.650064Z"}'
+      string: '{"id":"65f56389-75bd-44fc-b6b3-0ad7f08dcc55","span_id":"bcf1b3b4-0b3b-4b3b-8b3b-0b3b4b3b4133","dimension":"dim","value":0.5,"comment":"comment","updated_at":null,"created_at":"2024-05-21T09:54:25.297498Z"}'
     headers:
       content-length:
-      - '206'
+      - '205'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 13:23:01 GMT
+      - Tue, 21 May 2024 09:54:24 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
@@ -66,14 +66,14 @@
   response:
     body:
       string: ''
     headers:
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 13:23:01 GMT
+      - Tue, 21 May 2024 09:54:24 GMT
       server:
       - uvicorn
     status:
       code: 204
       message: No Content
 version: 1
```

### Comparing `opperai-0.6.2/tests/fixtures/vcr_cassettes/test_fn_decorator/test_fn_decorator.yaml` & `opperai-0.7.0/tests/fixtures/vcr_cassettes/test_fn_decorator/test_fn_decorator.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -7,57 +7,57 @@
       connection:
       - keep-alive
     method: GET
     uri: http://localhost:8000/v1/functions/by_path/translate
   response:
     body:
       string: '{"path":"translate","instructions":"Operation: translate\n\nOperation
-        description: Translate text to a target language.","id":82,"description":"Translate
-        text to a target language.","input_schema":null,"out_schema":{"type":"string","$defs":{}},"few_shot":false,"few_shot_count":2,"dataset_uuid":"0331a79c-e4f6-44c3-8176-56d908caaf43","use_semantic_search":false,"model":"openai/gpt3.5-turbo","language_model_id":2,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":{"exact_match_cache_ttl":0,"semantic_cache_threshold":0.95,"semantic_cache_ttl":0}}'
+        description: Translate text to a target language.","id":37,"description":"Translate
+        text to a target language.","input_schema":null,"out_schema":{"type":"string","$defs":{}},"few_shot":false,"few_shot_count":2,"dataset_uuid":"c5018772-4b37-4020-9dd0-878d2b1b749e","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":{"exact_match_cache_ttl":0,"semantic_cache_threshold":0.95,"semantic_cache_ttl":0}}'
     headers:
       content-length:
-      - '574'
+      - '568'
       content-type:
       - application/json
       date:
-      - Tue, 14 May 2024 19:47:08 GMT
+      - Tue, 21 May 2024 10:22:15 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
-    body: '{"id": 82, "path": "translate", "description": "Translate text to a target
+    body: '{"id": 37, "path": "translate", "description": "Translate text to a target
       language.", "input_schema": null, "out_schema": {"type": "string", "$defs":
       {}}, "instructions": "Operation: translate\n\nOperation description: Translate
       text to a target language.", "model": null, "index_ids": [], "use_semantic_search":
       null, "few_shot": false, "few_shot_count": null, "cache_configuration": null}'
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
       content-length:
       - '391'
       content-type:
       - application/json
     method: PATCH
-    uri: http://localhost:8000/v1/functions/82
+    uri: http://localhost:8000/v1/functions/37
   response:
     body:
       string: '{"path":"translate","instructions":"Operation: translate\n\nOperation
-        description: Translate text to a target language.","id":82,"description":"Translate
-        text to a target language.","input_schema":null,"out_schema":{"type":"string","$defs":{}},"few_shot":false,"few_shot_count":2,"dataset_uuid":"0331a79c-e4f6-44c3-8176-56d908caaf43","use_semantic_search":false,"model":"openai/gpt3.5-turbo","language_model_id":2,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":{"exact_match_cache_ttl":0,"semantic_cache_threshold":0.95,"semantic_cache_ttl":0}}'
+        description: Translate text to a target language.","id":37,"description":"Translate
+        text to a target language.","input_schema":null,"out_schema":{"type":"string","$defs":{}},"few_shot":false,"few_shot_count":2,"dataset_uuid":"c5018772-4b37-4020-9dd0-878d2b1b749e","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":{"exact_match_cache_ttl":0,"semantic_cache_threshold":0.95,"semantic_cache_ttl":0}}'
     headers:
       content-length:
-      - '574'
+      - '568'
       content-type:
       - application/json
       date:
-      - Tue, 14 May 2024 19:47:08 GMT
+      - Tue, 21 May 2024 10:22:15 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: '{"parent_span_uuid": null, "messages": [{"role": "user", "content": "{\"text\":
@@ -71,22 +71,22 @@
       - '123'
       content-type:
       - application/json
     method: POST
     uri: http://localhost:8000/v1/chat/translate
   response:
     body:
-      string: '{"span_id":"e0ce9a90-60a1-4545-bb3a-cabf0d8cead2","message":null,"json_payload":"Hola","context":null,"cached":false}'
+      string: '{"span_id":"12165659-17b4-4125-8504-bfc4d6957111","message":null,"json_payload":"Hola","context":null,"cached":false}'
     headers:
       content-length:
       - '117'
       content-type:
       - application/json
       date:
-      - Tue, 14 May 2024 19:47:08 GMT
+      - Tue, 21 May 2024 10:22:15 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: '{"parent_span_uuid": null, "messages": [{"role": "user", "content": "{\"text\":
@@ -100,22 +100,22 @@
       - '123'
       content-type:
       - application/json
     method: POST
     uri: http://localhost:8000/v1/chat/translate
   response:
     body:
-      string: "{\"span_id\":\"60281093-905d-4e50-b0bc-710259ca24c0\",\"message\":null,\"json_payload\":\"\xA1Hola\",\"context\":null,\"cached\":false}"
+      string: '{"span_id":"78879150-0123-44a2-84ae-0d6a83d52114","message":null,"json_payload":"Hola","context":null,"cached":false}'
     headers:
       content-length:
-      - '119'
+      - '117'
       content-type:
       - application/json
       date:
-      - Tue, 14 May 2024 19:47:09 GMT
+      - Tue, 21 May 2024 10:22:17 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: '{"dimension": "metric", "value": 1.0, "comment": null}'
@@ -125,24 +125,24 @@
       connection:
       - keep-alive
       content-length:
       - '54'
       content-type:
       - application/json
     method: POST
-    uri: http://localhost:8000/v1/spans/60281093-905d-4e50-b0bc-710259ca24c0/metrics
+    uri: http://localhost:8000/v1/spans/78879150-0123-44a2-84ae-0d6a83d52114/metrics
   response:
     body:
-      string: '{"id":"4d172cb9-295e-4456-b560-c8c7e5401b23","span_id":"60281093-905d-4e50-b0bc-710259ca24c0","dimension":"metric","value":1.0,"comment":null,"updated_at":null,"created_at":"2024-05-14T19:47:10.979159Z"}'
+      string: '{"id":"9dd86986-0b0d-48ac-af69-d4407751c603","span_id":"78879150-0123-44a2-84ae-0d6a83d52114","dimension":"metric","value":1.0,"comment":null,"updated_at":null,"created_at":"2024-05-21T10:22:21.597089Z"}'
     headers:
       content-length:
       - '203'
       content-type:
       - application/json
       date:
-      - Tue, 14 May 2024 19:47:10 GMT
+      - Tue, 21 May 2024 10:22:21 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `opperai-0.6.2/tests/fixtures/vcr_cassettes/test_fn_decorator/test_fn_decorator_async.yaml` & `opperai-0.7.0/tests/fixtures/vcr_cassettes/test_fn_decorator/test_fn_decorator_async.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -7,57 +7,57 @@
       connection:
       - keep-alive
     method: GET
     uri: http://localhost:8000/v1/functions/by_path/translate
   response:
     body:
       string: '{"path":"translate","instructions":"Operation: translate\n\nOperation
-        description: Translate text to a target language.","id":82,"description":"Translate
-        text to a target language.","input_schema":null,"out_schema":{"type":"string","$defs":{}},"few_shot":false,"few_shot_count":2,"dataset_uuid":"0331a79c-e4f6-44c3-8176-56d908caaf43","use_semantic_search":false,"model":"openai/gpt3.5-turbo","language_model_id":2,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":{"exact_match_cache_ttl":0,"semantic_cache_threshold":0.95,"semantic_cache_ttl":0}}'
+        description: Translate text to a target language.","id":37,"description":"Translate
+        text to a target language.","input_schema":null,"out_schema":{"type":"string","$defs":{}},"few_shot":false,"few_shot_count":2,"dataset_uuid":"c5018772-4b37-4020-9dd0-878d2b1b749e","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":{"exact_match_cache_ttl":0,"semantic_cache_threshold":0.95,"semantic_cache_ttl":0}}'
     headers:
       content-length:
-      - '574'
+      - '568'
       content-type:
       - application/json
       date:
-      - Tue, 14 May 2024 19:47:15 GMT
+      - Tue, 21 May 2024 10:25:50 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
-    body: '{"id": 82, "path": "translate", "description": "Translate text to a target
+    body: '{"id": 37, "path": "translate", "description": "Translate text to a target
       language.", "input_schema": null, "out_schema": {"type": "string", "$defs":
       {}}, "instructions": "Operation: translate\n\nOperation description: Translate
       text to a target language.", "model": null, "index_ids": [], "use_semantic_search":
       null, "few_shot": false, "few_shot_count": null, "cache_configuration": null}'
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
       content-length:
       - '391'
       content-type:
       - application/json
     method: PATCH
-    uri: http://localhost:8000/v1/functions/82
+    uri: http://localhost:8000/v1/functions/37
   response:
     body:
       string: '{"path":"translate","instructions":"Operation: translate\n\nOperation
-        description: Translate text to a target language.","id":82,"description":"Translate
-        text to a target language.","input_schema":null,"out_schema":{"type":"string","$defs":{}},"few_shot":false,"few_shot_count":2,"dataset_uuid":"0331a79c-e4f6-44c3-8176-56d908caaf43","use_semantic_search":false,"model":"openai/gpt3.5-turbo","language_model_id":2,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":{"exact_match_cache_ttl":0,"semantic_cache_threshold":0.95,"semantic_cache_ttl":0}}'
+        description: Translate text to a target language.","id":37,"description":"Translate
+        text to a target language.","input_schema":null,"out_schema":{"type":"string","$defs":{}},"few_shot":false,"few_shot_count":2,"dataset_uuid":"c5018772-4b37-4020-9dd0-878d2b1b749e","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":{"exact_match_cache_ttl":0,"semantic_cache_threshold":0.95,"semantic_cache_ttl":0}}'
     headers:
       content-length:
-      - '574'
+      - '568'
       content-type:
       - application/json
       date:
-      - Tue, 14 May 2024 19:47:15 GMT
+      - Tue, 21 May 2024 10:25:50 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: '{"parent_span_uuid": null, "messages": [{"role": "user", "content": "{\"text\":
@@ -71,22 +71,22 @@
       - '123'
       content-type:
       - application/json
     method: POST
     uri: http://localhost:8000/v1/chat/translate
   response:
     body:
-      string: '{"span_id":"5702b249-1f6f-40c6-be52-ed97ce1d21f0","message":null,"json_payload":"Hola","context":null,"cached":false}'
+      string: '{"span_id":"3a635532-fd37-4ab3-966f-aa9ad8f90e9f","message":null,"json_payload":"Hola","context":null,"cached":false}'
     headers:
       content-length:
       - '117'
       content-type:
       - application/json
       date:
-      - Tue, 14 May 2024 19:47:15 GMT
+      - Tue, 21 May 2024 10:25:50 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: '{"parent_span_uuid": null, "messages": [{"role": "user", "content": "{\"text\":
@@ -100,22 +100,22 @@
       - '123'
       content-type:
       - application/json
     method: POST
     uri: http://localhost:8000/v1/chat/translate
   response:
     body:
-      string: '{"span_id":"1b820c2e-c858-4420-9676-4c9c8a78fab8","message":null,"json_payload":"Hola","context":null,"cached":false}'
+      string: '{"span_id":"cb4dd1bd-c912-454c-b454-f4da7efc274d","message":null,"json_payload":"Hola","context":null,"cached":false}'
     headers:
       content-length:
       - '117'
       content-type:
       - application/json
       date:
-      - Tue, 14 May 2024 19:47:15 GMT
+      - Tue, 21 May 2024 10:25:51 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: '{"dimension": "metric", "value": 1.0, "comment": null}'
@@ -125,24 +125,24 @@
       connection:
       - keep-alive
       content-length:
       - '54'
       content-type:
       - application/json
     method: POST
-    uri: http://localhost:8000/v1/spans/1b820c2e-c858-4420-9676-4c9c8a78fab8/metrics
+    uri: http://localhost:8000/v1/spans/cb4dd1bd-c912-454c-b454-f4da7efc274d/metrics
   response:
     body:
-      string: '{"id":"6ca2cbce-2a0b-4d3e-8169-f7511614ca26","span_id":"1b820c2e-c858-4420-9676-4c9c8a78fab8","dimension":"metric","value":1.0,"comment":null,"updated_at":null,"created_at":"2024-05-14T19:47:17.653381Z"}'
+      string: '{"id":"db309fae-d80f-4f5a-9a8b-d30f5137fb64","span_id":"cb4dd1bd-c912-454c-b454-f4da7efc274d","dimension":"metric","value":1.0,"comment":null,"updated_at":null,"created_at":"2024-05-21T10:25:53.108679Z"}'
     headers:
       content-length:
       - '203'
       content-type:
       - application/json
       date:
-      - Tue, 14 May 2024 19:47:16 GMT
+      - Tue, 21 May 2024 10:25:52 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `opperai-0.6.2/tests/fixtures/vcr_cassettes/test_fn_decorator/test_fn_decorator_image.yaml` & `opperai-0.7.0/tests/fixtures/vcr_cassettes/test_fn_decorator/test_fn_decorator_image_async.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -7,59 +7,59 @@
       connection:
       - keep-alive
     method: GET
     uri: http://localhost:8000/v1/functions/by_path/extract_letters
   response:
     body:
       string: '{"path":"extract_letters","instructions":"Operation: extract_letters\n\nOperation
-        description: given an image extract the word it represents","id":190,"description":"given
-        an image extract the word it represents","input_schema":null,"out_schema":{"properties":{"letters":{"items":{"type":"string"},"title":"Letters","type":"array"}},"required":["letters"],"title":"Word","type":"object","$defs":{}},"few_shot":false,"few_shot_count":2,"dataset_uuid":"7eb2250e-88fd-495a-bb60-d8c10f54b4e4","use_semantic_search":false,"model":"openai/gpt-4o","language_model_id":20,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":{"exact_match_cache_ttl":0,"semantic_cache_threshold":0.95,"semantic_cache_ttl":0}}'
+        description: given an image extract the word it represents","id":24,"description":"given
+        an image extract the word it represents","input_schema":null,"out_schema":{"properties":{"letters":{"items":{"type":"string"},"title":"Letters","type":"array"}},"required":["letters"],"title":"Word","type":"object","$defs":{}},"few_shot":false,"few_shot_count":2,"dataset_uuid":"f3f7d90e-5a26-4143-9289-2cbfa7d3c2e8","use_semantic_search":false,"model":"openai/gpt-4o","language_model_id":20,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":{"exact_match_cache_ttl":0,"semantic_cache_threshold":0.95,"semantic_cache_ttl":0}}'
     headers:
       content-length:
-      - '724'
+      - '723'
       content-type:
       - application/json
       date:
-      - Tue, 14 May 2024 19:46:20 GMT
+      - Tue, 21 May 2024 10:25:48 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
-    body: '{"id": 190, "path": "extract_letters", "description": "given an image extract
+    body: '{"id": 24, "path": "extract_letters", "description": "given an image extract
       the word it represents", "input_schema": null, "out_schema": {"properties":
       {"letters": {"items": {"type": "string"}, "title": "Letters", "type": "array"}},
       "required": ["letters"], "title": "Word", "type": "object", "$defs": {}}, "instructions":
       "Operation: extract_letters\n\nOperation description: given an image extract
       the word it represents", "model": "openai/gpt-4o", "index_ids": [], "use_semantic_search":
       null, "few_shot": false, "few_shot_count": null, "cache_configuration": null}'
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
       content-length:
-      - '570'
+      - '569'
       content-type:
       - application/json
     method: PATCH
-    uri: http://localhost:8000/v1/functions/190
+    uri: http://localhost:8000/v1/functions/24
   response:
     body:
       string: '{"path":"extract_letters","instructions":"Operation: extract_letters\n\nOperation
-        description: given an image extract the word it represents","id":190,"description":"given
-        an image extract the word it represents","input_schema":null,"out_schema":{"properties":{"letters":{"items":{"type":"string"},"title":"Letters","type":"array"}},"required":["letters"],"title":"Word","type":"object","$defs":{}},"few_shot":false,"few_shot_count":2,"dataset_uuid":"7eb2250e-88fd-495a-bb60-d8c10f54b4e4","use_semantic_search":false,"model":"openai/gpt-4o","language_model_id":20,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":{"exact_match_cache_ttl":0,"semantic_cache_threshold":0.95,"semantic_cache_ttl":0}}'
+        description: given an image extract the word it represents","id":24,"description":"given
+        an image extract the word it represents","input_schema":null,"out_schema":{"properties":{"letters":{"items":{"type":"string"},"title":"Letters","type":"array"}},"required":["letters"],"title":"Word","type":"object","$defs":{}},"few_shot":false,"few_shot_count":2,"dataset_uuid":"f3f7d90e-5a26-4143-9289-2cbfa7d3c2e8","use_semantic_search":false,"model":"openai/gpt-4o","language_model_id":20,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":{"exact_match_cache_ttl":0,"semantic_cache_threshold":0.95,"semantic_cache_ttl":0}}'
     headers:
       content-length:
-      - '724'
+      - '723'
       content-type:
       - application/json
       date:
-      - Tue, 14 May 2024 19:46:20 GMT
+      - Tue, 21 May 2024 10:25:48 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: '{"parent_span_uuid": null, "messages": [{"role": "user", "content": "{}"},
@@ -73,21 +73,21 @@
       - '7741'
       content-type:
       - application/json
     method: POST
     uri: http://localhost:8000/v1/chat/extract_letters
   response:
     body:
-      string: '{"span_id":"4278fcef-952b-4330-9984-e36179bae733","message":null,"json_payload":{"letters":["L","E","T","T","E","R"]},"context":null,"cached":false}'
+      string: '{"span_id":"a720f126-4ecc-47f8-acc9-1a46f38f8ef1","message":null,"json_payload":{"letters":["L","E","T","T","E","R"]},"context":null,"cached":false}'
     headers:
       content-length:
       - '148'
       content-type:
       - application/json
       date:
-      - Tue, 14 May 2024 19:46:20 GMT
+      - Tue, 21 May 2024 10:25:48 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `opperai-0.6.2/tests/fixtures/vcr_cassettes/test_fn_decorator/test_fn_decorator_on_method.yaml` & `opperai-0.7.0/tests/fixtures/vcr_cassettes/test_fn_decorator/test_fn_decorator_on_method.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -7,55 +7,55 @@
       connection:
       - keep-alive
     method: GET
     uri: http://localhost:8000/v1/functions/by_path/test_method
   response:
     body:
       string: '{"path":"test_method","instructions":"Operation: test_method\n\nOperation
-        description: say hello","id":199,"description":"say hello","input_schema":null,"out_schema":{"type":"string","$defs":{}},"few_shot":false,"few_shot_count":2,"dataset_uuid":"63ef2190-c132-424b-9266-e1051642e78e","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":{"exact_match_cache_ttl":0,"semantic_cache_threshold":0.95,"semantic_cache_ttl":0}}'
+        description: say hello","id":23,"description":"say hello","input_schema":null,"out_schema":{"type":"string","$defs":{}},"few_shot":false,"few_shot_count":2,"dataset_uuid":"22ca6525-a4c3-476f-be85-e65a1ec49976","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":{"exact_match_cache_ttl":0,"semantic_cache_threshold":0.95,"semantic_cache_ttl":0}}'
     headers:
       content-length:
-      - '519'
+      - '518'
       content-type:
       - application/json
       date:
-      - Thu, 16 May 2024 11:48:57 GMT
+      - Tue, 21 May 2024 10:22:07 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
-    body: '{"id": 199, "path": "test_method", "description": "say hello", "input_schema":
+    body: '{"id": 23, "path": "test_method", "description": "say hello", "input_schema":
       null, "out_schema": {"type": "string", "$defs": {}}, "instructions": "Operation:
       test_method\n\nOperation description: say hello", "model": null, "index_ids":
       [], "use_semantic_search": null, "few_shot": false, "few_shot_count": null,
       "cache_configuration": null}'
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
       content-length:
-      - '342'
+      - '341'
       content-type:
       - application/json
     method: PATCH
-    uri: http://localhost:8000/v1/functions/199
+    uri: http://localhost:8000/v1/functions/23
   response:
     body:
       string: '{"path":"test_method","instructions":"Operation: test_method\n\nOperation
-        description: say hello","id":199,"description":"say hello","input_schema":null,"out_schema":{"type":"string","$defs":{}},"few_shot":false,"few_shot_count":2,"dataset_uuid":"63ef2190-c132-424b-9266-e1051642e78e","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":{"exact_match_cache_ttl":0,"semantic_cache_threshold":0.95,"semantic_cache_ttl":0}}'
+        description: say hello","id":23,"description":"say hello","input_schema":null,"out_schema":{"type":"string","$defs":{}},"few_shot":false,"few_shot_count":2,"dataset_uuid":"22ca6525-a4c3-476f-be85-e65a1ec49976","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":{"exact_match_cache_ttl":0,"semantic_cache_threshold":0.95,"semantic_cache_ttl":0}}'
     headers:
       content-length:
-      - '519'
+      - '518'
       content-type:
       - application/json
       date:
-      - Thu, 16 May 2024 11:48:57 GMT
+      - Tue, 21 May 2024 10:22:07 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: '{"parent_span_uuid": null, "messages": [{"role": "user", "content": "{\"self\":
@@ -69,22 +69,22 @@
       - '106'
       content-type:
       - application/json
     method: POST
     uri: http://localhost:8000/v1/chat/test_method
   response:
     body:
-      string: '{"span_id":"a3af19bb-d67c-4eb4-972c-d26cc0e5fc8b","message":null,"json_payload":"Hello","context":null,"cached":false}'
+      string: '{"span_id":"19f39b2f-71ff-4fae-80c3-7317ceb119f8","message":null,"json_payload":"Hello","context":null,"cached":false}'
     headers:
       content-length:
       - '118'
       content-type:
       - application/json
       date:
-      - Thu, 16 May 2024 11:48:57 GMT
+      - Tue, 21 May 2024 10:22:07 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: '{"parent_span_uuid": null, "messages": [{"role": "user", "content": "{\"self\":
@@ -98,21 +98,21 @@
       - '94'
       content-type:
       - application/json
     method: POST
     uri: http://localhost:8000/v1/chat/test_method
   response:
     body:
-      string: '{"span_id":"920bf660-afc9-49df-8d43-9c9717cb5ee9","message":null,"json_payload":"Hello","context":null,"cached":false}'
+      string: '{"span_id":"913638f8-b968-4bcf-862f-c686c965d42d","message":null,"json_payload":"Hello","context":null,"cached":false}'
     headers:
       content-length:
       - '118'
       content-type:
       - application/json
       date:
-      - Thu, 16 May 2024 11:48:58 GMT
+      - Tue, 21 May 2024 10:22:08 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `opperai-0.6.2/tests/fixtures/vcr_cassettes/test_fn_decorator/test_fn_decorator_on_method_async.yaml` & `opperai-0.7.0/tests/fixtures/vcr_cassettes/test_fn_decorator/test_fn_decorator_on_method_async.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -7,55 +7,55 @@
       connection:
       - keep-alive
     method: GET
     uri: http://localhost:8000/v1/functions/by_path/test_method
   response:
     body:
       string: '{"path":"test_method","instructions":"Operation: test_method\n\nOperation
-        description: say hello","id":199,"description":"say hello","input_schema":null,"out_schema":{"type":"string","$defs":{}},"few_shot":false,"few_shot_count":2,"dataset_uuid":"63ef2190-c132-424b-9266-e1051642e78e","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":{"exact_match_cache_ttl":0,"semantic_cache_threshold":0.95,"semantic_cache_ttl":0}}'
+        description: say hello","id":23,"description":"say hello","input_schema":null,"out_schema":{"type":"string","$defs":{}},"few_shot":false,"few_shot_count":2,"dataset_uuid":"22ca6525-a4c3-476f-be85-e65a1ec49976","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":{"exact_match_cache_ttl":0,"semantic_cache_threshold":0.95,"semantic_cache_ttl":0}}'
     headers:
       content-length:
-      - '519'
+      - '518'
       content-type:
       - application/json
       date:
-      - Thu, 16 May 2024 11:49:32 GMT
+      - Tue, 21 May 2024 10:22:10 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
-    body: '{"id": 199, "path": "test_method", "description": "say hello", "input_schema":
+    body: '{"id": 23, "path": "test_method", "description": "say hello", "input_schema":
       null, "out_schema": {"type": "string", "$defs": {}}, "instructions": "Operation:
       test_method\n\nOperation description: say hello", "model": null, "index_ids":
       [], "use_semantic_search": null, "few_shot": false, "few_shot_count": null,
       "cache_configuration": null}'
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
       content-length:
-      - '342'
+      - '341'
       content-type:
       - application/json
     method: PATCH
-    uri: http://localhost:8000/v1/functions/199
+    uri: http://localhost:8000/v1/functions/23
   response:
     body:
       string: '{"path":"test_method","instructions":"Operation: test_method\n\nOperation
-        description: say hello","id":199,"description":"say hello","input_schema":null,"out_schema":{"type":"string","$defs":{}},"few_shot":false,"few_shot_count":2,"dataset_uuid":"63ef2190-c132-424b-9266-e1051642e78e","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":{"exact_match_cache_ttl":0,"semantic_cache_threshold":0.95,"semantic_cache_ttl":0}}'
+        description: say hello","id":23,"description":"say hello","input_schema":null,"out_schema":{"type":"string","$defs":{}},"few_shot":false,"few_shot_count":2,"dataset_uuid":"22ca6525-a4c3-476f-be85-e65a1ec49976","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":{"exact_match_cache_ttl":0,"semantic_cache_threshold":0.95,"semantic_cache_ttl":0}}'
     headers:
       content-length:
-      - '519'
+      - '518'
       content-type:
       - application/json
       date:
-      - Thu, 16 May 2024 11:49:32 GMT
+      - Tue, 21 May 2024 10:22:10 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: '{"parent_span_uuid": null, "messages": [{"role": "user", "content": "{\"self\":
@@ -69,22 +69,22 @@
       - '106'
       content-type:
       - application/json
     method: POST
     uri: http://localhost:8000/v1/chat/test_method
   response:
     body:
-      string: '{"span_id":"86fcc8f5-dcf6-4df3-910f-f82625e88662","message":null,"json_payload":"Hello","context":null,"cached":false}'
+      string: '{"span_id":"073ef049-92fa-4d51-9d1c-62fcc103fe3a","message":null,"json_payload":"Hello","context":null,"cached":false}'
     headers:
       content-length:
       - '118'
       content-type:
       - application/json
       date:
-      - Thu, 16 May 2024 11:49:32 GMT
+      - Tue, 21 May 2024 10:22:10 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: '{"parent_span_uuid": null, "messages": [{"role": "user", "content": "{\"self\":
@@ -98,21 +98,21 @@
       - '94'
       content-type:
       - application/json
     method: POST
     uri: http://localhost:8000/v1/chat/test_method
   response:
     body:
-      string: '{"span_id":"57a964f0-a233-455e-85a7-5b47c7842f97","message":null,"json_payload":"Hello","context":null,"cached":false}'
+      string: '{"span_id":"c9082651-6777-46d2-bf3b-dd20aa4fba49","message":null,"json_payload":"Hello","context":null,"cached":false}'
     headers:
       content-length:
       - '118'
       content-type:
       - application/json
       date:
-      - Thu, 16 May 2024 11:49:34 GMT
+      - Tue, 21 May 2024 10:22:11 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `opperai-0.6.2/tests/fixtures/vcr_cassettes/test_functions/test_chat.yaml` & `opperai-0.7.0/tests/fixtures/vcr_cassettes/test_functions/test_chat_stream.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -3,131 +3,141 @@
     body: ''
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
     method: GET
-    uri: http://localhost:8000/v1/functions/by_path/test/sdk/test_chat
+    uri: http://localhost:8000/v1/functions/by_path/test/sdk/test_sync_chat_stream
   response:
     body:
-      string: '{"detail":"Function not found"}'
+      string: '{"errors":[{"type":"HTTPException","message":"Function not found","detail":"Function
+        not found"}]}'
     headers:
       content-length:
-      - '31'
+      - '98'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 09:17:37 GMT
+      - Tue, 21 May 2024 10:10:39 GMT
       server:
       - uvicorn
     status:
       code: 404
       message: Not Found
 - request:
-    body: '{"id": null, "path": "test/sdk/test_chat", "description": "Translate to
-      French", "input_schema": null, "out_schema": null, "instructions": "Translate
+    body: '{"id": null, "path": "test/sdk/test_sync_chat_stream", "description": "Translate
+      to French", "input_schema": null, "out_schema": null, "instructions": "Translate
       to French", "model": null, "index_ids": [], "use_semantic_search": null, "few_shot":
       null, "few_shot_count": null, "cache_configuration": null}'
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
       content-length:
-      - '293'
+      - '305'
       content-type:
       - application/json
     method: POST
     uri: http://localhost:8000/v1/functions
   response:
     body:
-      string: '{"id":26,"path":"test/sdk/test_chat","description":"Translate to French","input_schema":null,"out_schema":null,"instructions":"Translate
-        to French","few_shot":false,"few_shot_count":2,"dataset_uuid":"6b3d0427-baac-4be2-ad81-6b15bfbec58a","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
+      string: '{"path":"test/sdk/test_sync_chat_stream","instructions":"Translate
+        to French","id":47,"description":"Translate to French","input_schema":null,"out_schema":null,"few_shot":false,"few_shot_count":2,"dataset_uuid":"c057fd90-aa65-4779-88fd-7ef07079e98e","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
     headers:
       content-length:
-      - '394'
+      - '406'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 09:17:37 GMT
+      - Tue, 21 May 2024 10:10:39 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
     method: GET
-    uri: http://localhost:8000/v1/functions/26
+    uri: http://localhost:8000/v1/functions/47
   response:
     body:
-      string: '{"id":26,"path":"test/sdk/test_chat","description":"Translate to French","input_schema":null,"out_schema":null,"instructions":"Translate
-        to French","few_shot":false,"few_shot_count":2,"dataset_uuid":"6b3d0427-baac-4be2-ad81-6b15bfbec58a","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":{"exact_match_cache_ttl":0,"semantic_cache_threshold":0.95,"semantic_cache_ttl":0}}'
+      string: '{"path":"test/sdk/test_sync_chat_stream","instructions":"Translate
+        to French","id":47,"description":"Translate to French","input_schema":null,"out_schema":null,"few_shot":false,"few_shot_count":2,"dataset_uuid":"c057fd90-aa65-4779-88fd-7ef07079e98e","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":{"exact_match_cache_ttl":0,"semantic_cache_threshold":0.95,"semantic_cache_ttl":0}}'
     headers:
       content-length:
-      - '472'
+      - '484'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 09:17:37 GMT
+      - Tue, 21 May 2024 10:10:41 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: '{"parent_span_uuid": null, "messages": [{"role": "user", "content": "hello"}]}'
     headers:
       accept:
-      - '*/*'
+      - text/event-stream
+      cache-control:
+      - no-store
       connection:
       - keep-alive
       content-length:
       - '78'
       content-type:
       - application/json
     method: POST
-    uri: http://localhost:8000/v1/chat/test/sdk/test_chat
+    uri: http://localhost:8000/v1/chat/test/sdk/test_sync_chat_stream?stream=True
   response:
     body:
-      string: '{"span_id":"41f52b87-85c1-4495-a89a-a4b24d983f33","message":"Bonjour","json_payload":null,"error":null,"context":null,"cached":false}'
+      string: "data: {\"span_id\": \"31130663-5b65-4e30-9f7d-e15f8877d0ff\"}\r\n\r\ndata:
+        {\"delta\": \"Bonjour\"}\r\n\r\n"
     headers:
-      content-length:
-      - '133'
+      Transfer-Encoding:
+      - chunked
+      cache-control:
+      - no-cache
+      connection:
+      - keep-alive
       content-type:
-      - application/json
+      - text/event-stream; charset=utf-8
       date:
-      - Thu, 02 May 2024 09:17:37 GMT
+      - Tue, 21 May 2024 10:10:41 GMT
       server:
       - uvicorn
+      x-accel-buffering:
+      - 'no'
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
     method: DELETE
-    uri: http://localhost:8000/v1/functions/26
+    uri: http://localhost:8000/v1/functions/47
   response:
     body:
       string: ''
     headers:
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 09:17:38 GMT
+      - Tue, 21 May 2024 10:10:41 GMT
       server:
       - uvicorn
     status:
       code: 204
       message: No Content
 version: 1
```

### Comparing `opperai-0.6.2/tests/fixtures/vcr_cassettes/test_functions/test_chat_stream.yaml` & `opperai-0.7.0/tests/fixtures/vcr_cassettes/test_functions/test_create_function_with_cache.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -3,142 +3,138 @@
     body: ''
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
     method: GET
-    uri: http://localhost:8000/v1/functions/by_path/test/sdk/test_sync_chat_stream
+    uri: http://localhost:8000/v1/functions/by_path/test/sdk/test_create_function_with_cache
   response:
     body:
-      string: '{"detail":"Function not found"}'
+      string: '{"errors":[{"type":"HTTPException","message":"Function not found","detail":"Function
+        not found"}]}'
     headers:
       content-length:
-      - '31'
+      - '98'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 09:17:38 GMT
+      - Tue, 21 May 2024 10:10:41 GMT
       server:
       - uvicorn
     status:
       code: 404
       message: Not Found
 - request:
-    body: '{"id": null, "path": "test/sdk/test_sync_chat_stream", "description": "Translate
-      to French", "input_schema": null, "out_schema": null, "instructions": "Translate
-      to French", "model": null, "index_ids": [], "use_semantic_search": null, "few_shot":
-      null, "few_shot_count": null, "cache_configuration": null}'
+    body: '{"id": null, "path": "test/sdk/test_create_function_with_cache", "description":
+      "Test function", "input_schema": null, "out_schema": null, "instructions": "Do
+      something", "model": null, "index_ids": [], "use_semantic_search": null, "few_shot":
+      null, "few_shot_count": null, "cache_configuration": {"exact_match_cache_ttl":
+      10, "semantic_cache_threshold": null, "semantic_cache_ttl": null}}'
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
       content-length:
-      - '305'
+      - '389'
       content-type:
       - application/json
     method: POST
     uri: http://localhost:8000/v1/functions
   response:
     body:
-      string: '{"id":27,"path":"test/sdk/test_sync_chat_stream","description":"Translate
-        to French","input_schema":null,"out_schema":null,"instructions":"Translate
-        to French","few_shot":false,"few_shot_count":2,"dataset_uuid":"1f6ce832-10cd-4541-b338-3c0f02996a49","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
+      string: '{"path":"test/sdk/test_create_function_with_cache","instructions":"Do
+        something","id":48,"description":"Test function","input_schema":null,"out_schema":null,"few_shot":false,"few_shot_count":2,"dataset_uuid":"0b2e6263-47e2-4069-9fb6-0af1f3b40491","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
     headers:
       content-length:
-      - '406'
+      - '403'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 09:17:38 GMT
+      - Tue, 21 May 2024 10:10:41 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
-    body: ''
+    body: '{"parent_span_uuid": null, "messages": [{"role": "user", "content": "hello"}]}'
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
-    method: GET
-    uri: http://localhost:8000/v1/functions/27
+      content-length:
+      - '78'
+      content-type:
+      - application/json
+    method: POST
+    uri: http://localhost:8000/v1/chat/test/sdk/test_create_function_with_cache
   response:
     body:
-      string: '{"id":27,"path":"test/sdk/test_sync_chat_stream","description":"Translate
-        to French","input_schema":null,"out_schema":null,"instructions":"Translate
-        to French","few_shot":false,"few_shot_count":2,"dataset_uuid":"1f6ce832-10cd-4541-b338-3c0f02996a49","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":{"exact_match_cache_ttl":0,"semantic_cache_threshold":0.95,"semantic_cache_ttl":0}}'
+      string: '{"span_id":"9684c8ab-54db-4a35-919c-edcc6bd7f835","message":"Hello
+        there! How can I assist you today?","json_payload":null,"context":null,"cached":false}'
     headers:
       content-length:
-      - '484'
+      - '153'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 09:17:38 GMT
+      - Tue, 21 May 2024 10:10:41 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: '{"parent_span_uuid": null, "messages": [{"role": "user", "content": "hello"}]}'
     headers:
       accept:
-      - text/event-stream
-      cache-control:
-      - no-store
+      - '*/*'
       connection:
       - keep-alive
       content-length:
       - '78'
       content-type:
       - application/json
     method: POST
-    uri: http://localhost:8000/v1/chat/test/sdk/test_sync_chat_stream?stream=True
+    uri: http://localhost:8000/v1/chat/test/sdk/test_create_function_with_cache
   response:
     body:
-      string: "data: {\"span_id\": \"0199c47d-b130-4346-a06c-bbdce9e53e18\"}\r\n\r\ndata:
-        {\"delta\": \"Bonjour\"}\r\n\r\n"
+      string: '{"span_id":"58b6730f-7b06-465e-8448-ca30f8ab8cbd","message":"Hello
+        there! How can I assist you today?","json_payload":null,"context":null,"cached":true}'
     headers:
-      Transfer-Encoding:
-      - chunked
-      cache-control:
-      - no-cache
-      connection:
-      - keep-alive
+      content-length:
+      - '152'
       content-type:
-      - text/event-stream; charset=utf-8
+      - application/json
       date:
-      - Thu, 02 May 2024 09:17:38 GMT
+      - Tue, 21 May 2024 10:10:42 GMT
       server:
       - uvicorn
-      x-accel-buffering:
-      - 'no'
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
     method: DELETE
-    uri: http://localhost:8000/v1/functions/27
+    uri: http://localhost:8000/v1/functions/48
   response:
     body:
       string: ''
     headers:
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 09:17:39 GMT
+      - Tue, 21 May 2024 10:10:42 GMT
       server:
       - uvicorn
     status:
       code: 204
       message: No Content
 version: 1
```

### Comparing `opperai-0.6.2/tests/fixtures/vcr_cassettes/test_functions/test_create_function.yaml` & `opperai-0.7.0/tests/fixtures/vcr_cassettes/test_client/test_client_raises_timeout_error.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -3,78 +3,81 @@
     body: ''
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
     method: GET
-    uri: http://localhost:8000/v1/functions/by_path/test/sdk/test_create_function
+    uri: http://localhost:8000/v1/functions/by_path/test_client_raises_timeout_error
   response:
     body:
-      string: '{"detail":"Function not found"}'
+      string: '{"errors":[{"type":"HTTPException","message":"Function not found","detail":"Function
+        not found"}]}'
     headers:
       content-length:
-      - '31'
+      - '98'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 09:22:31 GMT
+      - Tue, 21 May 2024 09:54:24 GMT
       server:
       - uvicorn
     status:
       code: 404
       message: Not Found
 - request:
-    body: '{"id": null, "path": "test/sdk/test_create_function", "description": "Test
-      function", "input_schema": null, "out_schema": null, "instructions": "Do something",
-      "model": null, "index_ids": [], "use_semantic_search": null, "few_shot": null,
-      "few_shot_count": null, "cache_configuration": null}'
+    body: ''
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
-      content-length:
-      - '291'
-      content-type:
-      - application/json
-    method: POST
-    uri: http://localhost:8000/v1/functions
+    method: GET
+    uri: http://localhost:8000/v1/functions/by_path/test_client_raises_timeout_error
   response:
     body:
-      string: '{"id":56,"path":"test/sdk/test_create_function","description":"Test
-        function","input_schema":null,"out_schema":null,"instructions":"Do something","few_shot":false,"few_shot_count":2,"dataset_uuid":"a1663bee-f874-4031-895f-2faae028c8e5","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
+      string: '{"errors":[{"type":"HTTPException","message":"Function not found","detail":"Function
+        not found"}]}'
     headers:
       content-length:
-      - '392'
+      - '98'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 09:22:31 GMT
+      - Tue, 21 May 2024 09:54:24 GMT
       server:
       - uvicorn
     status:
-      code: 200
-      message: OK
+      code: 404
+      message: Not Found
 - request:
-    body: ''
+    body: '{"id": null, "path": "test_client_raises_timeout_error", "description":
+      null, "input_schema": null, "out_schema": null, "instructions": "test", "model":
+      null, "index_ids": [], "use_semantic_search": null, "few_shot": null, "few_shot_count":
+      null, "cache_configuration": null}'
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
-    method: DELETE
-    uri: http://localhost:8000/v1/functions/56
+      content-length:
+      - '275'
+      content-type:
+      - application/json
+    method: POST
+    uri: http://localhost:8000/v1/functions
   response:
     body:
-      string: ''
+      string: '{"path":"test_client_raises_timeout_error","instructions":"test","id":22,"description":null,"input_schema":null,"out_schema":null,"few_shot":false,"few_shot_count":2,"dataset_uuid":"f69ad070-aed2-478e-b690-d409923b4953","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
     headers:
+      content-length:
+      - '376'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 09:22:31 GMT
+      - Tue, 21 May 2024 09:54:24 GMT
       server:
       - uvicorn
     status:
-      code: 204
-      message: No Content
+      code: 200
+      message: OK
 version: 1
```

### Comparing `opperai-0.6.2/tests/fixtures/vcr_cassettes/test_functions/test_create_function_with_cache.yaml` & `opperai-0.7.0/tests/fixtures/vcr_cassettes/test_functions/test_create_function_with_cache_flush.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -3,58 +3,59 @@
     body: ''
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
     method: GET
-    uri: http://localhost:8000/v1/functions/by_path/test/sdk/test_create_function_with_cache
+    uri: http://localhost:8000/v1/functions/by_path/test/sdk/test_create_function_with_cache_sync_flush
   response:
     body:
-      string: '{"detail":"Function not found"}'
+      string: '{"errors":[{"type":"HTTPException","message":"Function not found","detail":"Function
+        not found"}]}'
     headers:
       content-length:
-      - '31'
+      - '98'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 09:17:39 GMT
+      - Tue, 21 May 2024 10:10:42 GMT
       server:
       - uvicorn
     status:
       code: 404
       message: Not Found
 - request:
-    body: '{"id": null, "path": "test/sdk/test_create_function_with_cache", "description":
-      "Test function", "input_schema": null, "out_schema": null, "instructions": "Do
-      something", "model": null, "index_ids": [], "use_semantic_search": null, "few_shot":
-      null, "few_shot_count": null, "cache_configuration": {"exact_match_cache_ttl":
+    body: '{"id": null, "path": "test/sdk/test_create_function_with_cache_sync_flush",
+      "description": "Test function", "input_schema": null, "out_schema": null, "instructions":
+      "Do something", "model": null, "index_ids": [], "use_semantic_search": null,
+      "few_shot": null, "few_shot_count": null, "cache_configuration": {"exact_match_cache_ttl":
       10, "semantic_cache_threshold": null, "semantic_cache_ttl": null}}'
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
       content-length:
-      - '389'
+      - '400'
       content-type:
       - application/json
     method: POST
     uri: http://localhost:8000/v1/functions
   response:
     body:
-      string: '{"id":28,"path":"test/sdk/test_create_function_with_cache","description":"Test
-        function","input_schema":null,"out_schema":null,"instructions":"Do something","few_shot":false,"few_shot_count":2,"dataset_uuid":"0ddeb3de-617d-4442-afc5-e51c05c833af","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
+      string: '{"path":"test/sdk/test_create_function_with_cache_sync_flush","instructions":"Do
+        something","id":49,"description":"Test function","input_schema":null,"out_schema":null,"few_shot":false,"few_shot_count":2,"dataset_uuid":"93e94b58-83c7-4442-9df0-7818b582189e","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
     headers:
       content-length:
-      - '403'
+      - '414'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 09:17:39 GMT
+      - Tue, 21 May 2024 10:10:42 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: '{"parent_span_uuid": null, "messages": [{"role": "user", "content": "hello"}]}'
@@ -64,27 +65,27 @@
       connection:
       - keep-alive
       content-length:
       - '78'
       content-type:
       - application/json
     method: POST
-    uri: http://localhost:8000/v1/chat/test/sdk/test_create_function_with_cache
+    uri: http://localhost:8000/v1/chat/test/sdk/test_create_function_with_cache_sync_flush
   response:
     body:
-      string: '{"span_id":"ca79b63e-76d3-4962-91bb-83d4e6de549b","message":"Hello!
+      string: '{"span_id":"67fdd8b5-be07-46b7-9368-40b35e68e9aa","message":"Hello!
         How can I assist you today? If you have any questions or need information
-        on a topic, feel free to ask.","json_payload":null,"error":null,"context":null,"cached":false}'
+        on a topic, feel free to ask.","json_payload":null,"context":null,"cached":false}'
     headers:
       content-length:
-      - '236'
+      - '223'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 09:17:39 GMT
+      - Tue, 21 May 2024 10:10:42 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: '{"parent_span_uuid": null, "messages": [{"role": "user", "content": "hello"}]}'
@@ -94,48 +95,100 @@
       connection:
       - keep-alive
       content-length:
       - '78'
       content-type:
       - application/json
     method: POST
-    uri: http://localhost:8000/v1/chat/test/sdk/test_create_function_with_cache
+    uri: http://localhost:8000/v1/chat/test/sdk/test_create_function_with_cache_sync_flush
   response:
     body:
-      string: '{"span_id":"0794f09f-22e3-4a1a-8ebf-ad03922d636f","message":"Hello!
+      string: '{"span_id":"12cfc647-d90f-49cb-9769-89de32335a7f","message":"Hello!
         How can I assist you today? If you have any questions or need information
-        on a topic, feel free to ask.","json_payload":null,"error":null,"context":null,"cached":true}'
+        on a topic, feel free to ask.","json_payload":null,"context":null,"cached":true}'
     headers:
       content-length:
-      - '235'
+      - '222'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 09:17:41 GMT
+      - Tue, 21 May 2024 10:10:48 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
     method: DELETE
-    uri: http://localhost:8000/v1/functions/28
+    uri: http://localhost:8000/v1/functions/49/cache
   response:
     body:
       string: ''
     headers:
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 09:17:42 GMT
+      - Tue, 21 May 2024 10:10:48 GMT
+      server:
+      - uvicorn
+    status:
+      code: 204
+      message: No Content
+- request:
+    body: '{"parent_span_uuid": null, "messages": [{"role": "user", "content": "hello"}]}'
+    headers:
+      accept:
+      - '*/*'
+      connection:
+      - keep-alive
+      content-length:
+      - '78'
+      content-type:
+      - application/json
+    method: POST
+    uri: http://localhost:8000/v1/chat/test/sdk/test_create_function_with_cache_sync_flush
+  response:
+    body:
+      string: '{"span_id":"ec4b7fd2-52b3-4778-a812-a42b8aa34bfe","message":"Hello!
+        How can I assist you today? If you have any questions or need information
+        on a topic, feel free to ask.","json_payload":null,"context":null,"cached":false}'
+    headers:
+      content-length:
+      - '223'
+      content-type:
+      - application/json
+      date:
+      - Tue, 21 May 2024 10:10:48 GMT
+      server:
+      - uvicorn
+    status:
+      code: 200
+      message: OK
+- request:
+    body: ''
+    headers:
+      accept:
+      - '*/*'
+      connection:
+      - keep-alive
+    method: DELETE
+    uri: http://localhost:8000/v1/functions/49
+  response:
+    body:
+      string: ''
+    headers:
+      content-type:
+      - application/json
+      date:
+      - Tue, 21 May 2024 10:10:51 GMT
       server:
       - uvicorn
     status:
       code: 204
       message: No Content
 version: 1
```

### Comparing `opperai-0.6.2/tests/fixtures/vcr_cassettes/test_functions/test_delete_function_by_id.yaml` & `opperai-0.7.0/tests/fixtures/vcr_cassettes/test_async_functions/test_get_by_path.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -3,102 +3,104 @@
     body: ''
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
     method: GET
-    uri: http://localhost:8000/v1/functions/by_path/test/sdk/test_delete_function_by_id
+    uri: http://localhost:8000/v1/functions/by_path/test/sdk/test_get_by_path
   response:
     body:
-      string: '{"detail":"Function not found"}'
+      string: '{"errors":[{"type":"HTTPException","message":"Function not found","detail":"Function
+        not found"}]}'
     headers:
       content-length:
-      - '31'
+      - '98'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 09:17:37 GMT
+      - Tue, 21 May 2024 10:09:44 GMT
       server:
       - uvicorn
     status:
       code: 404
       message: Not Found
 - request:
-    body: '{"id": null, "path": "test/sdk/test_delete_function_by_id", "description":
-      "Test function", "input_schema": null, "out_schema": null, "instructions": "Do
-      something", "model": null, "index_ids": [], "use_semantic_search": null, "few_shot":
-      null, "few_shot_count": null, "cache_configuration": null}'
+    body: '{"id": null, "path": "test/sdk/test_get_by_path", "description": "Test
+      function", "input_schema": null, "out_schema": null, "instructions": "Do something",
+      "model": null, "index_ids": [], "use_semantic_search": null, "few_shot": null,
+      "few_shot_count": null, "cache_configuration": null}'
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
       content-length:
-      - '297'
+      - '287'
       content-type:
       - application/json
     method: POST
     uri: http://localhost:8000/v1/functions
   response:
     body:
-      string: '{"id":24,"path":"test/sdk/test_delete_function_by_id","description":"Test
-        function","input_schema":null,"out_schema":null,"instructions":"Do something","few_shot":false,"few_shot_count":2,"dataset_uuid":"55891e4f-91f2-48ef-a423-9f5dcb9fa61b","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
+      string: '{"path":"test/sdk/test_get_by_path","instructions":"Do something","id":27,"description":"Test
+        function","input_schema":null,"out_schema":null,"few_shot":false,"few_shot_count":2,"dataset_uuid":"8a923aaf-fb90-46dc-a099-09b56ae92e56","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
     headers:
       content-length:
-      - '398'
+      - '388'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 09:17:37 GMT
+      - Tue, 21 May 2024 10:09:44 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
-    method: DELETE
-    uri: http://localhost:8000/v1/functions/24
+    method: GET
+    uri: http://localhost:8000/v1/functions/by_path/test/sdk/test_get_by_path
   response:
     body:
-      string: ''
+      string: '{"path":"test/sdk/test_get_by_path","instructions":"Do something","id":27,"description":"Test
+        function","input_schema":null,"out_schema":null,"few_shot":false,"few_shot_count":2,"dataset_uuid":"8a923aaf-fb90-46dc-a099-09b56ae92e56","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":{"exact_match_cache_ttl":0,"semantic_cache_threshold":0.95,"semantic_cache_ttl":0}}'
     headers:
+      content-length:
+      - '466'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 09:17:37 GMT
+      - Tue, 21 May 2024 10:09:44 GMT
       server:
       - uvicorn
     status:
-      code: 204
-      message: No Content
+      code: 200
+      message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
-    method: GET
-    uri: http://localhost:8000/v1/functions/24
+    method: DELETE
+    uri: http://localhost:8000/v1/functions/27
   response:
     body:
-      string: '{"detail":"Function not found"}'
+      string: ''
     headers:
-      content-length:
-      - '31'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 09:17:37 GMT
+      - Tue, 21 May 2024 10:09:44 GMT
       server:
       - uvicorn
     status:
-      code: 404
-      message: Not Found
+      code: 204
+      message: No Content
 version: 1
```

### Comparing `opperai-0.6.2/tests/fixtures/vcr_cassettes/test_functions/test_delete_function_by_path.yaml` & `opperai-0.7.0/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -3,102 +3,79 @@
     body: ''
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
     method: GET
-    uri: http://localhost:8000/v1/functions/by_path/test/sdk/test_delete_function_by_path
+    uri: http://localhost:8000/v1/functions/by_path/test/sdk/test_create_function_async
   response:
     body:
-      string: '{"detail":"Function not found"}'
+      string: '{"errors":[{"type":"HTTPException","message":"Function not found","detail":"Function
+        not found"}]}'
     headers:
       content-length:
-      - '31'
+      - '98'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 09:17:37 GMT
+      - Tue, 21 May 2024 10:09:44 GMT
       server:
       - uvicorn
     status:
       code: 404
       message: Not Found
 - request:
-    body: '{"id": null, "path": "test/sdk/test_delete_function_by_path", "description":
+    body: '{"id": null, "path": "test/sdk/test_create_function_async", "description":
       "Test function", "input_schema": null, "out_schema": null, "instructions": "Do
       something", "model": null, "index_ids": [], "use_semantic_search": null, "few_shot":
       null, "few_shot_count": null, "cache_configuration": null}'
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
       content-length:
-      - '299'
+      - '297'
       content-type:
       - application/json
     method: POST
     uri: http://localhost:8000/v1/functions
   response:
     body:
-      string: '{"id":25,"path":"test/sdk/test_delete_function_by_path","description":"Test
-        function","input_schema":null,"out_schema":null,"instructions":"Do something","few_shot":false,"few_shot_count":2,"dataset_uuid":"6df5d044-11cb-4b46-8505-2e6dd439978d","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
+      string: '{"path":"test/sdk/test_create_function_async","instructions":"Do something","id":25,"description":"Test
+        function","input_schema":null,"out_schema":null,"few_shot":false,"few_shot_count":2,"dataset_uuid":"9ea0935f-594f-400c-8192-fb9c20c1a006","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
     headers:
       content-length:
-      - '400'
+      - '398'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 09:17:37 GMT
+      - Tue, 21 May 2024 10:09:44 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
     method: DELETE
-    uri: http://localhost:8000/v1/functions/by_path/test/sdk/test_delete_function_by_path
+    uri: http://localhost:8000/v1/functions/25
   response:
     body:
       string: ''
     headers:
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 09:17:37 GMT
+      - Tue, 21 May 2024 10:09:44 GMT
       server:
       - uvicorn
     status:
       code: 204
       message: No Content
-- request:
-    body: ''
-    headers:
-      accept:
-      - '*/*'
-      connection:
-      - keep-alive
-    method: GET
-    uri: http://localhost:8000/v1/functions/by_path/test/sdk/test_delete_function_by_path
-  response:
-    body:
-      string: '{"detail":"Function not found"}'
-    headers:
-      content-length:
-      - '31'
-      content-type:
-      - application/json
-      date:
-      - Thu, 02 May 2024 09:17:37 GMT
-      server:
-      - uvicorn
-    status:
-      code: 404
-      message: Not Found
 version: 1
```

### Comparing `opperai-0.6.2/tests/fixtures/vcr_cassettes/test_functions/test_failed_structured_generation.yaml` & `opperai-0.7.0/tests/fixtures/vcr_cassettes/test_functions/test_chat.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -3,66 +3,83 @@
     body: ''
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
     method: GET
-    uri: http://localhost:8000/v1/functions/by_path/test/sdk/test_failed_structured_generation
+    uri: http://localhost:8000/v1/functions/by_path/test/sdk/test_chat
   response:
     body:
-      string: '{"detail":"Function not found"}'
+      string: '{"errors":[{"type":"HTTPException","message":"Function not found","detail":"Function
+        not found"}]}'
     headers:
       content-length:
-      - '31'
+      - '98'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 09:17:50 GMT
+      - Tue, 21 May 2024 10:10:39 GMT
       server:
       - uvicorn
     status:
       code: 404
       message: Not Found
 - request:
-    body: '{"id": null, "path": "test/sdk/test_failed_structured_generation", "description":
-      "test structured generation exception", "input_schema": null, "out_schema":
-      {"type": "object", "properties": {"universityName": {"type": "string"}, "location":
-      {"type": "string"}, "departments": {"type": "array", "items": {"type": "object",
-      "properties": {"departmentName": {"type": "string"}, "head": {"type": "string"},
-      "courses": {"type": "array", "items": {"type": "object", "properties": {"courseId":
-      {"type": "string"}, "courseName": {"type": "string"}, "credits": {"type": "integer",
-      "minimum": 1, "maximum": 10}}, "required": ["courseId", "courseName", "credits"]}}},
-      "required": ["departmentName", "head", "courses"]}}}, "required": ["universityName",
-      "location", "departments"]}, "instructions": "You translate the incoming text
-      to french", "model": "mistral/mistral-tiny-eu", "index_ids": [], "use_semantic_search":
-      null, "few_shot": null, "few_shot_count": null, "cache_configuration": null}'
+    body: '{"id": null, "path": "test/sdk/test_chat", "description": "Translate to
+      French", "input_schema": null, "out_schema": null, "instructions": "Translate
+      to French", "model": null, "index_ids": [], "use_semantic_search": null, "few_shot":
+      null, "few_shot_count": null, "cache_configuration": null}'
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
       content-length:
-      - '985'
+      - '293'
       content-type:
       - application/json
     method: POST
     uri: http://localhost:8000/v1/functions
   response:
     body:
-      string: '{"id":30,"path":"test/sdk/test_failed_structured_generation","description":"test
-        structured generation exception","input_schema":null,"out_schema":null,"instructions":"You
-        translate the incoming text to french","few_shot":false,"few_shot_count":2,"dataset_uuid":"b6e23402-8fcf-49d0-9a30-3ada2f0b5742","use_semantic_search":false,"model":"mistral/mistral-tiny-eu","language_model_id":4,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
+      string: '{"path":"test/sdk/test_chat","instructions":"Translate to French","id":46,"description":"Translate
+        to French","input_schema":null,"out_schema":null,"few_shot":false,"few_shot_count":2,"dataset_uuid":"d81febd9-34f2-44a9-a3a0-f7631c972abb","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
     headers:
       content-length:
-      - '467'
+      - '394'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 09:17:50 GMT
+      - Tue, 21 May 2024 10:10:39 GMT
+      server:
+      - uvicorn
+    status:
+      code: 200
+      message: OK
+- request:
+    body: ''
+    headers:
+      accept:
+      - '*/*'
+      connection:
+      - keep-alive
+    method: GET
+    uri: http://localhost:8000/v1/functions/46
+  response:
+    body:
+      string: '{"path":"test/sdk/test_chat","instructions":"Translate to French","id":46,"description":"Translate
+        to French","input_schema":null,"out_schema":null,"few_shot":false,"few_shot_count":2,"dataset_uuid":"d81febd9-34f2-44a9-a3a0-f7631c972abb","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":{"exact_match_cache_ttl":0,"semantic_cache_threshold":0.95,"semantic_cache_ttl":0}}'
+    headers:
+      content-length:
+      - '472'
+      content-type:
+      - application/json
+      date:
+      - Tue, 21 May 2024 10:10:39 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: '{"parent_span_uuid": null, "messages": [{"role": "user", "content": "hello"}]}'
@@ -72,47 +89,46 @@
       connection:
       - keep-alive
       content-length:
       - '78'
       content-type:
       - application/json
     method: POST
-    uri: http://localhost:8000/v1/chat/test/sdk/test_failed_structured_generation
+    uri: http://localhost:8000/v1/chat/test/sdk/test_chat
   response:
     body:
-      string: '{"detail":"Structured generation failed, could not generate response
-        matching the schema."}'
+      string: '{"span_id":"49139fdf-9296-4583-937a-e60a78e6a86d","message":"Bonjour","json_payload":null,"context":null,"cached":false}'
     headers:
       content-length:
-      - '91'
+      - '120'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 09:17:50 GMT
+      - Tue, 21 May 2024 10:10:39 GMT
       server:
       - uvicorn
     status:
-      code: 400
-      message: Bad Request
+      code: 200
+      message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
     method: DELETE
-    uri: http://localhost:8000/v1/functions/30
+    uri: http://localhost:8000/v1/functions/46
   response:
     body:
       string: ''
     headers:
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 09:18:06 GMT
+      - Tue, 21 May 2024 10:10:39 GMT
       server:
       - uvicorn
     status:
       code: 204
       message: No Content
 version: 1
```

### Comparing `opperai-0.6.2/tests/fixtures/vcr_cassettes/test_functions/test_get_by_id.yaml` & `opperai-0.7.0/tests/fixtures/vcr_cassettes/test_functions/test_get_by_path.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -3,103 +3,104 @@
     body: ''
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
     method: GET
-    uri: http://localhost:8000/v1/functions/by_path/test/sdk/test_get_by_id
+    uri: http://localhost:8000/v1/functions/by_path/test/sdk/test_get_by_path
   response:
     body:
-      string: '{"detail":"Function not found"}'
+      string: '{"errors":[{"type":"HTTPException","message":"Function not found","detail":"Function
+        not found"}]}'
     headers:
       content-length:
-      - '31'
+      - '98'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 09:22:31 GMT
+      - Tue, 21 May 2024 10:10:21 GMT
       server:
       - uvicorn
     status:
       code: 404
       message: Not Found
 - request:
-    body: '{"id": null, "path": "test/sdk/test_get_by_id", "description": "Test function",
-      "input_schema": null, "out_schema": null, "instructions": "Do something", "model":
-      null, "index_ids": [], "use_semantic_search": null, "few_shot": null, "few_shot_count":
-      null, "cache_configuration": null}'
+    body: '{"id": null, "path": "test/sdk/test_get_by_path", "description": "Test
+      function", "input_schema": null, "out_schema": null, "instructions": "Do something",
+      "model": null, "index_ids": [], "use_semantic_search": null, "few_shot": null,
+      "few_shot_count": null, "cache_configuration": null}'
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
       content-length:
-      - '285'
+      - '287'
       content-type:
       - application/json
     method: POST
     uri: http://localhost:8000/v1/functions
   response:
     body:
-      string: '{"id":57,"path":"test/sdk/test_get_by_id","description":"Test function","input_schema":null,"out_schema":null,"instructions":"Do
-        something","few_shot":false,"few_shot_count":2,"dataset_uuid":"7ce0a1d8-d7bb-4323-8703-95974c257844","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
+      string: '{"path":"test/sdk/test_get_by_path","instructions":"Do something","id":40,"description":"Test
+        function","input_schema":null,"out_schema":null,"few_shot":false,"few_shot_count":2,"dataset_uuid":"a000b500-ea57-459a-a21f-e647b4fbbeee","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
     headers:
       content-length:
-      - '386'
+      - '388'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 09:22:31 GMT
+      - Tue, 21 May 2024 10:10:21 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
     method: GET
-    uri: http://localhost:8000/v1/functions/57
+    uri: http://localhost:8000/v1/functions/by_path/test/sdk/test_get_by_path
   response:
     body:
-      string: '{"id":57,"path":"test/sdk/test_get_by_id","description":"Test function","input_schema":null,"out_schema":null,"instructions":"Do
-        something","few_shot":false,"few_shot_count":2,"dataset_uuid":"7ce0a1d8-d7bb-4323-8703-95974c257844","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":{"exact_match_cache_ttl":0,"semantic_cache_threshold":0.95,"semantic_cache_ttl":0}}'
+      string: '{"path":"test/sdk/test_get_by_path","instructions":"Do something","id":40,"description":"Test
+        function","input_schema":null,"out_schema":null,"few_shot":false,"few_shot_count":2,"dataset_uuid":"a000b500-ea57-459a-a21f-e647b4fbbeee","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":{"exact_match_cache_ttl":0,"semantic_cache_threshold":0.95,"semantic_cache_ttl":0}}'
     headers:
       content-length:
-      - '464'
+      - '466'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 09:22:31 GMT
+      - Tue, 21 May 2024 10:10:21 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
     method: DELETE
-    uri: http://localhost:8000/v1/functions/57
+    uri: http://localhost:8000/v1/functions/40
   response:
     body:
       string: ''
     headers:
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 09:22:31 GMT
+      - Tue, 21 May 2024 10:10:21 GMT
       server:
       - uvicorn
     status:
       code: 204
       message: No Content
 version: 1
```

### Comparing `opperai-0.6.2/tests/fixtures/vcr_cassettes/test_functions/test_get_by_path.yaml` & `opperai-0.7.0/tests/fixtures/vcr_cassettes/test_async_functions/test_get_by_id.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -3,103 +3,104 @@
     body: ''
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
     method: GET
-    uri: http://localhost:8000/v1/functions/by_path/test/sdk/test_get_by_path
+    uri: http://localhost:8000/v1/functions/by_path/test/sdk/test_get_by_id
   response:
     body:
-      string: '{"detail":"Function not found"}'
+      string: '{"errors":[{"type":"HTTPException","message":"Function not found","detail":"Function
+        not found"}]}'
     headers:
       content-length:
-      - '31'
+      - '98'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 09:22:31 GMT
+      - Tue, 21 May 2024 10:09:44 GMT
       server:
       - uvicorn
     status:
       code: 404
       message: Not Found
 - request:
-    body: '{"id": null, "path": "test/sdk/test_get_by_path", "description": "Test
-      function", "input_schema": null, "out_schema": null, "instructions": "Do something",
-      "model": null, "index_ids": [], "use_semantic_search": null, "few_shot": null,
-      "few_shot_count": null, "cache_configuration": null}'
+    body: '{"id": null, "path": "test/sdk/test_get_by_id", "description": "Test function",
+      "input_schema": null, "out_schema": null, "instructions": "Do something", "model":
+      null, "index_ids": [], "use_semantic_search": null, "few_shot": null, "few_shot_count":
+      null, "cache_configuration": null}'
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
       content-length:
-      - '287'
+      - '285'
       content-type:
       - application/json
     method: POST
     uri: http://localhost:8000/v1/functions
   response:
     body:
-      string: '{"id":58,"path":"test/sdk/test_get_by_path","description":"Test function","input_schema":null,"out_schema":null,"instructions":"Do
-        something","few_shot":false,"few_shot_count":2,"dataset_uuid":"02d0f301-270e-4014-be08-c3cfc2017d18","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
+      string: '{"path":"test/sdk/test_get_by_id","instructions":"Do something","id":26,"description":"Test
+        function","input_schema":null,"out_schema":null,"few_shot":false,"few_shot_count":2,"dataset_uuid":"a2104338-bb3c-4da8-aff0-8c4c1b58f568","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
     headers:
       content-length:
-      - '388'
+      - '386'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 09:22:31 GMT
+      - Tue, 21 May 2024 10:09:44 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
     method: GET
-    uri: http://localhost:8000/v1/functions/by_path/test/sdk/test_get_by_path
+    uri: http://localhost:8000/v1/functions/26
   response:
     body:
-      string: '{"id":58,"path":"test/sdk/test_get_by_path","description":"Test function","input_schema":null,"out_schema":null,"instructions":"Do
-        something","few_shot":false,"few_shot_count":2,"dataset_uuid":"02d0f301-270e-4014-be08-c3cfc2017d18","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":{"exact_match_cache_ttl":0,"semantic_cache_threshold":0.95,"semantic_cache_ttl":0}}'
+      string: '{"path":"test/sdk/test_get_by_id","instructions":"Do something","id":26,"description":"Test
+        function","input_schema":null,"out_schema":null,"few_shot":false,"few_shot_count":2,"dataset_uuid":"a2104338-bb3c-4da8-aff0-8c4c1b58f568","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":{"exact_match_cache_ttl":0,"semantic_cache_threshold":0.95,"semantic_cache_ttl":0}}'
     headers:
       content-length:
-      - '466'
+      - '464'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 09:22:31 GMT
+      - Tue, 21 May 2024 10:09:44 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
     method: DELETE
-    uri: http://localhost:8000/v1/functions/58
+    uri: http://localhost:8000/v1/functions/26
   response:
     body:
       string: ''
     headers:
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 09:22:31 GMT
+      - Tue, 21 May 2024 10:09:44 GMT
       server:
       - uvicorn
     status:
       code: 204
       message: No Content
 version: 1
```

### Comparing `opperai-0.6.2/tests/fixtures/vcr_cassettes/test_functions/test_image_file.yaml` & `opperai-0.7.0/tests/fixtures/vcr_cassettes/test_functions/test_image_file.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -6,77 +6,78 @@
       - '*/*'
       connection:
       - keep-alive
     method: GET
     uri: http://localhost:8000/v1/functions/by_path/test/sdk/test_image
   response:
     body:
-      string: '{"path":"test/sdk/test_image","instructions":"describe the image","id":180,"description":null,"input_schema":null,"out_schema":null,"few_shot":false,"few_shot_count":2,"dataset_uuid":"346eb784-74f0-4fe1-935e-d67545d92e5b","use_semantic_search":false,"model":"openai/gpt4-turbo","language_model_id":1,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":{"exact_match_cache_ttl":0,"semantic_cache_threshold":0.95,"semantic_cache_ttl":0}}'
+      string: '{"errors":[{"type":"HTTPException","message":"Function not found","detail":"Function
+        not found"}]}'
     headers:
       content-length:
-      - '460'
+      - '98'
       content-type:
       - application/json
       date:
-      - Mon, 13 May 2024 11:22:46 GMT
+      - Tue, 21 May 2024 10:10:30 GMT
       server:
       - uvicorn
     status:
-      code: 200
-      message: OK
+      code: 404
+      message: Not Found
 - request:
-    body: '{"id": 180, "path": "test/sdk/test_image", "description": null, "input_schema":
+    body: '{"id": null, "path": "test/sdk/test_image", "description": null, "input_schema":
       null, "out_schema": null, "instructions": "describe the image", "model": "openai/gpt4-turbo",
       "index_ids": [], "use_semantic_search": null, "few_shot": null, "few_shot_count":
       null, "cache_configuration": null}'
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
       content-length:
-      - '290'
+      - '291'
       content-type:
       - application/json
-    method: PATCH
-    uri: http://localhost:8000/v1/functions/180
+    method: POST
+    uri: http://localhost:8000/v1/functions
   response:
     body:
-      string: '{"path":"test/sdk/test_image","instructions":"describe the image","id":180,"description":null,"input_schema":null,"out_schema":null,"few_shot":false,"few_shot_count":2,"dataset_uuid":"346eb784-74f0-4fe1-935e-d67545d92e5b","use_semantic_search":false,"model":"openai/gpt4-turbo","language_model_id":1,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":{"exact_match_cache_ttl":0,"semantic_cache_threshold":0.95,"semantic_cache_ttl":0}}'
+      string: '{"path":"test/sdk/test_image","instructions":"describe the image","id":45,"description":null,"input_schema":null,"out_schema":null,"few_shot":false,"few_shot_count":2,"dataset_uuid":"3213d9ff-ddce-44e5-81f9-2998c96eb452","use_semantic_search":false,"model":"openai/gpt4-turbo","language_model_id":1,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
     headers:
       content-length:
-      - '460'
+      - '381'
       content-type:
       - application/json
       date:
-      - Mon, 13 May 2024 11:22:46 GMT
+      - Tue, 21 May 2024 10:10:30 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
     method: GET
-    uri: http://localhost:8000/v1/functions/180
+    uri: http://localhost:8000/v1/functions/45
   response:
     body:
-      string: '{"path":"test/sdk/test_image","instructions":"describe the image","id":180,"description":null,"input_schema":null,"out_schema":null,"few_shot":false,"few_shot_count":2,"dataset_uuid":"346eb784-74f0-4fe1-935e-d67545d92e5b","use_semantic_search":false,"model":"openai/gpt4-turbo","language_model_id":1,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":{"exact_match_cache_ttl":0,"semantic_cache_threshold":0.95,"semantic_cache_ttl":0}}'
+      string: '{"path":"test/sdk/test_image","instructions":"describe the image","id":45,"description":null,"input_schema":null,"out_schema":null,"few_shot":false,"few_shot_count":2,"dataset_uuid":"3213d9ff-ddce-44e5-81f9-2998c96eb452","use_semantic_search":false,"model":"openai/gpt4-turbo","language_model_id":1,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":{"exact_match_cache_ttl":0,"semantic_cache_threshold":0.95,"semantic_cache_ttl":0}}'
     headers:
       content-length:
-      - '460'
+      - '459'
       content-type:
       - application/json
       date:
-      - Mon, 13 May 2024 11:22:46 GMT
+      - Tue, 21 May 2024 10:10:30 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: '{"parent_span_uuid": null, "messages": [{"role": "user", "content": [{"type":
@@ -90,54 +91,53 @@
       - '231975'
       content-type:
       - application/json
     method: POST
     uri: http://localhost:8000/v1/chat/test/sdk/test_image
   response:
     body:
-      string: "{\"span_id\":\"31aa7d03-f570-4387-bdf2-6e91c578007b\",\"message\":\"This
-        is an image of a fossil, displayed on a flat, roughly oval piece of stone.
-        The fossil appears to be that of a small, lizard-like creature, possibly a
-        young dinosaur or another prehistoric reptile, embedded within the rock. The
-        skeleton is well-preserved, showcasing a detailed skull with visible eye sockets,
-        a row of fine teeth, and a clearly defined vertebrae. The ribs, limbs, and
-        tail bones are also visible, giving a complete view of the creature\u2019s
-        body structure. The rock itself has a sandy color and the fossil is accentuated
-        with a darker, metallic hue which enhances its visibility and details against
-        the pale background. This specimen is likely displayed under artificial lighting
-        in a museum or similar setting, which highlights the contours and textures
-        of the fossil and the rock.\",\"json_payload\":null,\"context\":null,\"cached\":false}"
+      string: '{"span_id":"f833633e-dc92-485e-9a6f-7dc9da3e0320","message":"This image
+        shows a fossilized skeleton displayed on a rocky matrix. The skeleton appears
+        to belong to a reptilian or amphibious creature, judging by the structure
+        of its skull, spine, and limb configuration. The skull is large with visible
+        eye sockets, and the body follows with a clearly defined rib cage and vertebrae
+        leading to a slender tail. The limbs are positioned closely to the body, with
+        bones of legs and possible digits discernible near the edges. The overall
+        presentation and preservation suggest that this fossil is well-maintained
+        and possibly displayed in a museum or educational setting. The lighting highlights
+        the details of the fossil, enhancing its three-dimensional appearance against
+        the contrasting dark background.","json_payload":null,"context":null,"cached":false}'
     headers:
       content-length:
-      - '915'
+      - '852'
       content-type:
       - application/json
       date:
-      - Mon, 13 May 2024 11:22:46 GMT
+      - Tue, 21 May 2024 10:10:30 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
     method: DELETE
-    uri: http://localhost:8000/v1/functions/180
+    uri: http://localhost:8000/v1/functions/45
   response:
     body:
       string: ''
     headers:
       content-type:
       - application/json
       date:
-      - Mon, 13 May 2024 11:23:07 GMT
+      - Tue, 21 May 2024 10:10:39 GMT
       server:
       - uvicorn
     status:
       code: 204
       message: No Content
 version: 1
```

### Comparing `opperai-0.6.2/tests/fixtures/vcr_cassettes/test_functions/test_image_url.yaml` & `opperai-0.7.0/tests/fixtures/vcr_cassettes/test_async_functions/test_image_url.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -6,22 +6,23 @@
       - '*/*'
       connection:
       - keep-alive
     method: GET
     uri: http://localhost:8000/v1/functions/by_path/test/sdk/test_image
   response:
     body:
-      string: '{"detail":"Function not found"}'
+      string: '{"errors":[{"type":"HTTPException","message":"Function not found","detail":"Function
+        not found"}]}'
     headers:
       content-length:
-      - '31'
+      - '98'
       content-type:
       - application/json
       date:
-      - Mon, 13 May 2024 11:23:17 GMT
+      - Tue, 21 May 2024 10:09:44 GMT
       server:
       - uvicorn
     status:
       code: 404
       message: Not Found
 - request:
     body: '{"id": null, "path": "test/sdk/test_image", "description": null, "input_schema":
@@ -37,46 +38,46 @@
       - '291'
       content-type:
       - application/json
     method: POST
     uri: http://localhost:8000/v1/functions
   response:
     body:
-      string: '{"path":"test/sdk/test_image","instructions":"describe the image","id":181,"description":null,"input_schema":null,"out_schema":null,"few_shot":false,"few_shot_count":2,"dataset_uuid":"35a44240-ad9d-4151-8476-8b7b54f53ba5","use_semantic_search":false,"model":"openai/gpt4-turbo","language_model_id":1,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
+      string: '{"path":"test/sdk/test_image","instructions":"describe the image","id":31,"description":null,"input_schema":null,"out_schema":null,"few_shot":false,"few_shot_count":2,"dataset_uuid":"d3fdeb37-9dc4-4e05-a090-904016c00727","use_semantic_search":false,"model":"openai/gpt4-turbo","language_model_id":1,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
     headers:
       content-length:
-      - '382'
+      - '381'
       content-type:
       - application/json
       date:
-      - Mon, 13 May 2024 11:23:17 GMT
+      - Tue, 21 May 2024 10:09:44 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
     method: GET
-    uri: http://localhost:8000/v1/functions/181
+    uri: http://localhost:8000/v1/functions/31
   response:
     body:
-      string: '{"path":"test/sdk/test_image","instructions":"describe the image","id":181,"description":null,"input_schema":null,"out_schema":null,"few_shot":false,"few_shot_count":2,"dataset_uuid":"35a44240-ad9d-4151-8476-8b7b54f53ba5","use_semantic_search":false,"model":"openai/gpt4-turbo","language_model_id":1,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":{"exact_match_cache_ttl":0,"semantic_cache_threshold":0.95,"semantic_cache_ttl":0}}'
+      string: '{"path":"test/sdk/test_image","instructions":"describe the image","id":31,"description":null,"input_schema":null,"out_schema":null,"few_shot":false,"few_shot_count":2,"dataset_uuid":"d3fdeb37-9dc4-4e05-a090-904016c00727","use_semantic_search":false,"model":"openai/gpt4-turbo","language_model_id":1,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":{"exact_match_cache_ttl":0,"semantic_cache_threshold":0.95,"semantic_cache_ttl":0}}'
     headers:
       content-length:
-      - '460'
+      - '459'
       content-type:
       - application/json
       date:
-      - Mon, 13 May 2024 11:23:17 GMT
+      - Tue, 21 May 2024 10:09:44 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: '{"parent_span_uuid": null, "messages": [{"role": "user", "content": [{"type":
@@ -90,50 +91,54 @@
       - '251'
       content-type:
       - application/json
     method: POST
     uri: http://localhost:8000/v1/chat/test/sdk/test_image
   response:
     body:
-      string: '{"span_id":"9f365d67-a09e-4faa-a859-5eccf58714e0","message":"This image
-        features a fossilized skeleton of a prehistoric creature, showcased on a sediment
-        rock slab. The bones are well-preserved and arranged in a nearly complete
-        skeletal form, including the skull, spine, ribs, legs, and tail. The fossil
-        is displayed against a dark backdrop, highlighting the intricate details and
-        contrast against the lighter color of the sediment. It appears to be an exhibit
-        possibly within a museum setting, aimed at educating visitors about ancient
-        wildlife and paleontological discoveries.","json_payload":null,"context":null,"cached":false}'
+      string: '{"span_id":"96558adf-59a6-4322-9ba8-6fa10fa268b1","message":"This image
+        features a fossil embedded in a flat stone slab, displayed under lighting
+        that highlights its details. The fossil appears to be that of a small reptilian
+        or lizard-like creature, possibly from a prehistoric era. You can clearly
+        see the skeletal structure, including the skull, spine, ribs, and limbs, which
+        are well-preserved and distinct. The texture of the stone slab is rough and
+        slightly uneven, providing a natural contrast to the dark fossil remains.
+        This kind of preservation suggests that the creature might have been rapidly
+        covered by sediment, aiding in the excellent preservation of its skeletal
+        features. Such fossils are crucial for scientific studies as they provide
+        valuable insights into the anatomy and evolutionary history of the species
+        they belonged to.","json_payload":null,"context":null,"cached":false}'
     headers:
       content-length:
-      - '630'
+      - '898'
       content-type:
       - application/json
       date:
-      - Mon, 13 May 2024 11:23:17 GMT
+      - Tue, 21 May 2024 10:09:44 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
     method: DELETE
-    uri: http://localhost:8000/v1/functions/181
+    uri: http://localhost:8000/v1/functions/31
   response:
     body:
       string: ''
     headers:
       content-type:
       - application/json
       date:
-      - Mon, 13 May 2024 11:23:30 GMT
+      - Tue, 21 May 2024 10:09:52 GMT
       server:
       - uvicorn
     status:
       code: 204
       message: No Content
 version: 1
```

### Comparing `opperai-0.6.2/tests/fixtures/vcr_cassettes/test_functions/test_update_function.yaml` & `opperai-0.7.0/tests/fixtures/vcr_cassettes/test_functions/test_update_function.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -6,162 +6,159 @@
       - '*/*'
       connection:
       - keep-alive
     method: GET
     uri: http://localhost:8000/v1/functions/by_path/test/sdk/test_update_function
   response:
     body:
-      string: '{"id":23,"path":"test/sdk/test_update_function","description":"Test
-        function","input_schema":null,"out_schema":null,"instructions":"Do something
-        else","few_shot":false,"few_shot_count":2,"dataset_uuid":"22a1b039-cf65-441a-81b4-6306625067b9","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":2,"cache_configuration":{"exact_match_cache_ttl":0,"semantic_cache_threshold":0.95,"semantic_cache_ttl":0}}'
+      string: '{"errors":[{"type":"HTTPException","message":"Function not found","detail":"Function
+        not found"}]}'
     headers:
       content-length:
-      - '475'
+      - '98'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 09:17:37 GMT
+      - Tue, 21 May 2024 10:10:21 GMT
       server:
       - uvicorn
     status:
-      code: 200
-      message: OK
+      code: 404
+      message: Not Found
 - request:
-    body: '{"id": 23, "path": "test/sdk/test_update_function", "description": "Test
+    body: '{"id": null, "path": "test/sdk/test_update_function", "description": "Test
       function", "input_schema": null, "out_schema": null, "instructions": "Do something",
       "model": null, "index_ids": [], "use_semantic_search": null, "few_shot": null,
       "few_shot_count": null, "cache_configuration": null}'
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
       content-length:
-      - '289'
+      - '291'
       content-type:
       - application/json
-    method: PATCH
-    uri: http://localhost:8000/v1/functions/23
+    method: POST
+    uri: http://localhost:8000/v1/functions
   response:
     body:
-      string: '{"id":23,"path":"test/sdk/test_update_function","description":"Test
-        function","input_schema":null,"out_schema":null,"instructions":"Do something","few_shot":false,"few_shot_count":2,"dataset_uuid":"22a1b039-cf65-441a-81b4-6306625067b9","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":3,"cache_configuration":{"exact_match_cache_ttl":0,"semantic_cache_threshold":0.95,"semantic_cache_ttl":0}}'
+      string: '{"path":"test/sdk/test_update_function","instructions":"Do something","id":41,"description":"Test
+        function","input_schema":null,"out_schema":null,"few_shot":false,"few_shot_count":2,"dataset_uuid":"8f6ebb23-fd84-4733-901c-5dc90f9bba01","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
     headers:
       content-length:
-      - '470'
+      - '392'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 09:17:37 GMT
+      - Tue, 21 May 2024 10:10:21 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
     method: GET
-    uri: http://localhost:8000/v1/functions/23
+    uri: http://localhost:8000/v1/functions/41
   response:
     body:
-      string: '{"id":23,"path":"test/sdk/test_update_function","description":"Test
-        function","input_schema":null,"out_schema":null,"instructions":"Do something","few_shot":false,"few_shot_count":2,"dataset_uuid":"22a1b039-cf65-441a-81b4-6306625067b9","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":3,"cache_configuration":{"exact_match_cache_ttl":0,"semantic_cache_threshold":0.95,"semantic_cache_ttl":0}}'
+      string: '{"path":"test/sdk/test_update_function","instructions":"Do something","id":41,"description":"Test
+        function","input_schema":null,"out_schema":null,"few_shot":false,"few_shot_count":2,"dataset_uuid":"8f6ebb23-fd84-4733-901c-5dc90f9bba01","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":{"exact_match_cache_ttl":0,"semantic_cache_threshold":0.95,"semantic_cache_ttl":0}}'
     headers:
       content-length:
       - '470'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 09:17:37 GMT
+      - Tue, 21 May 2024 10:10:21 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
-    body: '{"id": 23, "path": "test/sdk/test_update_function", "description": "Test
+    body: '{"id": 41, "path": "test/sdk/test_update_function", "description": "Test
       function", "input_schema": null, "out_schema": null, "instructions": "Do something
       else", "model": "azure/gpt4-eu", "index_ids": [], "use_semantic_search": false,
       "few_shot": false, "few_shot_count": 2, "cache_configuration": {"exact_match_cache_ttl":
       0, "semantic_cache_threshold": 0.95, "semantic_cache_ttl": 0}}'
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
       content-length:
       - '387'
       content-type:
       - application/json
     method: PATCH
-    uri: http://localhost:8000/v1/functions/23
+    uri: http://localhost:8000/v1/functions/41
   response:
     body:
-      string: '{"id":23,"path":"test/sdk/test_update_function","description":"Test
-        function","input_schema":null,"out_schema":null,"instructions":"Do something
-        else","few_shot":false,"few_shot_count":2,"dataset_uuid":"22a1b039-cf65-441a-81b4-6306625067b9","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":4,"cache_configuration":{"exact_match_cache_ttl":0,"semantic_cache_threshold":0.95,"semantic_cache_ttl":0}}'
+      string: '{"path":"test/sdk/test_update_function","instructions":"Do something
+        else","id":41,"description":"Test function","input_schema":null,"out_schema":null,"few_shot":false,"few_shot_count":2,"dataset_uuid":"8f6ebb23-fd84-4733-901c-5dc90f9bba01","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":2,"cache_configuration":{"exact_match_cache_ttl":0,"semantic_cache_threshold":0.95,"semantic_cache_ttl":0}}'
     headers:
       content-length:
       - '475'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 09:17:37 GMT
+      - Tue, 21 May 2024 10:10:21 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
     method: GET
-    uri: http://localhost:8000/v1/functions/23
+    uri: http://localhost:8000/v1/functions/41
   response:
     body:
-      string: '{"id":23,"path":"test/sdk/test_update_function","description":"Test
-        function","input_schema":null,"out_schema":null,"instructions":"Do something
-        else","few_shot":false,"few_shot_count":2,"dataset_uuid":"22a1b039-cf65-441a-81b4-6306625067b9","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":4,"cache_configuration":{"exact_match_cache_ttl":0,"semantic_cache_threshold":0.95,"semantic_cache_ttl":0}}'
+      string: '{"path":"test/sdk/test_update_function","instructions":"Do something
+        else","id":41,"description":"Test function","input_schema":null,"out_schema":null,"few_shot":false,"few_shot_count":2,"dataset_uuid":"8f6ebb23-fd84-4733-901c-5dc90f9bba01","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":2,"cache_configuration":{"exact_match_cache_ttl":0,"semantic_cache_threshold":0.95,"semantic_cache_ttl":0}}'
     headers:
       content-length:
       - '475'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 09:17:37 GMT
+      - Tue, 21 May 2024 10:10:21 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
     method: DELETE
-    uri: http://localhost:8000/v1/functions/23
+    uri: http://localhost:8000/v1/functions/41
   response:
     body:
       string: ''
     headers:
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 09:17:37 GMT
+      - Tue, 21 May 2024 10:10:21 GMT
       server:
       - uvicorn
     status:
       code: 204
       message: No Content
 version: 1
```

### Comparing `opperai-0.6.2/tests/fixtures/vcr_cassettes/test_indexes/test_create_index.yaml` & `opperai-0.7.0/tests/fixtures/vcr_cassettes/test_indexes/test_create_index.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -10,45 +10,45 @@
       - '29'
       content-type:
       - application/json
     method: POST
     uri: http://localhost:8000/v1/indexes
   response:
     body:
-      string: '{"id":2,"name":"test_create_index","files":[],"created_at":"2024-05-02T09:18:07.238445Z"}'
+      string: '{"id":10,"name":"test_create_index","files":[],"created_at":"2024-05-21T10:10:58.565581Z"}'
     headers:
       content-length:
-      - '89'
+      - '90'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 09:18:07 GMT
+      - Tue, 21 May 2024 10:10:58 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
     method: DELETE
-    uri: http://localhost:8000/v1/indexes/2
+    uri: http://localhost:8000/v1/indexes/10
   response:
     body:
       string: 'true'
     headers:
       content-length:
       - '4'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 09:18:07 GMT
+      - Tue, 21 May 2024 10:10:58 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `opperai-0.6.2/tests/fixtures/vcr_cassettes/test_indexes/test_delete_index.yaml` & `opperai-0.7.0/tests/fixtures/vcr_cassettes/test_functions/test_create_function.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -1,78 +1,81 @@
 interactions:
 - request:
-    body: '{"name": "test_delete_index"}'
+    body: ''
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
-      content-length:
-      - '29'
-      content-type:
-      - application/json
-    method: POST
-    uri: http://localhost:8000/v1/indexes
+    method: GET
+    uri: http://localhost:8000/v1/functions/by_path/test/sdk/test_create_function
   response:
     body:
-      string: '{"id":3,"name":"test_delete_index","files":[],"created_at":"2024-05-02T09:18:07.294338Z"}'
+      string: '{"errors":[{"type":"HTTPException","message":"Function not found","detail":"Function
+        not found"}]}'
     headers:
       content-length:
-      - '89'
+      - '98'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 09:18:07 GMT
+      - Tue, 21 May 2024 10:10:21 GMT
       server:
       - uvicorn
     status:
-      code: 200
-      message: OK
+      code: 404
+      message: Not Found
 - request:
-    body: ''
+    body: '{"id": null, "path": "test/sdk/test_create_function", "description": "Test
+      function", "input_schema": null, "out_schema": null, "instructions": "Do something",
+      "model": null, "index_ids": [], "use_semantic_search": null, "few_shot": null,
+      "few_shot_count": null, "cache_configuration": null}'
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
-    method: DELETE
-    uri: http://localhost:8000/v1/indexes/3
+      content-length:
+      - '291'
+      content-type:
+      - application/json
+    method: POST
+    uri: http://localhost:8000/v1/functions
   response:
     body:
-      string: 'true'
+      string: '{"path":"test/sdk/test_create_function","instructions":"Do something","id":38,"description":"Test
+        function","input_schema":null,"out_schema":null,"few_shot":false,"few_shot_count":2,"dataset_uuid":"bb3849c1-80af-458f-8e45-19cfc4d1d24c","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":null}'
     headers:
       content-length:
-      - '4'
+      - '392'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 09:18:07 GMT
+      - Tue, 21 May 2024 10:10:21 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
-    method: GET
-    uri: http://localhost:8000/v1/indexes/3
+    method: DELETE
+    uri: http://localhost:8000/v1/functions/38
   response:
     body:
-      string: '{"detail":"Index not found"}'
+      string: ''
     headers:
-      content-length:
-      - '28'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 09:18:07 GMT
+      - Tue, 21 May 2024 10:10:21 GMT
       server:
       - uvicorn
     status:
-      code: 404
-      message: Not Found
+      code: 204
+      message: No Content
 version: 1
```

### Comparing `opperai-0.6.2/tests/fixtures/vcr_cassettes/test_indexes/test_get_by_id.yaml` & `opperai-0.7.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_get_by_id.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -10,69 +10,69 @@
       - '26'
       content-type:
       - application/json
     method: POST
     uri: http://localhost:8000/v1/indexes
   response:
     body:
-      string: '{"id":4,"name":"test_get_by_id","files":[],"created_at":"2024-05-02T09:18:07.341181Z"}'
+      string: '{"id":3,"name":"test_get_by_id","files":[],"created_at":"2024-05-21T09:54:22.932563Z"}'
     headers:
       content-length:
       - '86'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 09:18:07 GMT
+      - Tue, 21 May 2024 09:54:22 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
     method: GET
-    uri: http://localhost:8000/v1/indexes/4
+    uri: http://localhost:8000/v1/indexes/3
   response:
     body:
-      string: '{"id":4,"name":"test_get_by_id","files":[],"created_at":"2024-05-02T09:18:07.341181Z"}'
+      string: '{"id":3,"name":"test_get_by_id","files":[],"created_at":"2024-05-21T09:54:22.932563Z"}'
     headers:
       content-length:
       - '86'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 09:18:07 GMT
+      - Tue, 21 May 2024 09:54:22 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
     method: DELETE
-    uri: http://localhost:8000/v1/indexes/4
+    uri: http://localhost:8000/v1/indexes/3
   response:
     body:
       string: 'true'
     headers:
       content-length:
       - '4'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 09:18:07 GMT
+      - Tue, 21 May 2024 09:54:22 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `opperai-0.6.2/tests/fixtures/vcr_cassettes/test_indexes/test_get_by_name.yaml` & `opperai-0.7.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_delete_index.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,79 +1,104 @@
 interactions:
 - request:
-    body: '{"name": "test_get_by_name"}'
+    body: '{"name": "test_delete_index"}'
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
       content-length:
-      - '28'
+      - '29'
       content-type:
       - application/json
     method: POST
     uri: http://localhost:8000/v1/indexes
   response:
     body:
-      string: '{"id":5,"name":"test_get_by_name","files":[],"created_at":"2024-05-02T09:18:07.379419Z"}'
+      string: '{"id":2,"name":"test_delete_index","files":[],"created_at":"2024-05-21T09:54:22.872090Z"}'
     headers:
       content-length:
-      - '88'
+      - '89'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 09:18:07 GMT
+      - Tue, 21 May 2024 09:54:22 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
-    method: GET
-    uri: http://localhost:8000/v1/indexes
+    method: DELETE
+    uri: http://localhost:8000/v1/indexes/2
   response:
     body:
-      string: '[{"id":5,"org_id":1,"org_name":null,"name":"test_get_by_name","created_by":"Mattias
-        Lundell","created_at":"2024-05-02T09:18:07.379419Z","updated_at":"2024-05-02T09:18:07.379419Z","count":0}]'
+      string: 'true'
     headers:
       content-length:
-      - '190'
+      - '4'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 09:18:07 GMT
+      - Tue, 21 May 2024 09:54:22 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
+    method: GET
+    uri: http://localhost:8000/v1/indexes/2
+  response:
+    body:
+      string: '{"errors":[{"type":"HTTPException","message":"Index not found","detail":"Index
+        not found"}]}'
+    headers:
+      content-length:
+      - '92'
+      content-type:
+      - application/json
+      date:
+      - Tue, 21 May 2024 09:54:22 GMT
+      server:
+      - uvicorn
+    status:
+      code: 404
+      message: Not Found
+- request:
+    body: ''
+    headers:
+      accept:
+      - '*/*'
+      connection:
+      - keep-alive
     method: DELETE
-    uri: http://localhost:8000/v1/indexes/5
+    uri: http://localhost:8000/v1/indexes/2
   response:
     body:
-      string: 'true'
+      string: '{"errors":[{"type":"HTTPException","message":"Index not found","detail":"Index
+        not found"}]}'
     headers:
       content-length:
-      - '4'
+      - '92'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 09:18:07 GMT
+      - Tue, 21 May 2024 09:54:22 GMT
       server:
       - uvicorn
     status:
-      code: 200
-      message: OK
+      code: 404
+      message: Not Found
 version: 1
```

### Comparing `opperai-0.6.2/tests/fixtures/vcr_cassettes/test_indexes/test_index_document.yaml` & `opperai-0.7.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_index_document.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -10,22 +10,22 @@
       - '31'
       content-type:
       - application/json
     method: POST
     uri: http://localhost:8000/v1/indexes
   response:
     body:
-      string: '{"id":8,"name":"test_index_document","files":[],"created_at":"2024-05-02T09:18:07.509002Z"}'
+      string: '{"id":7,"name":"test_index_document","files":[],"created_at":"2024-05-21T09:54:23.104059Z"}'
     headers:
       content-length:
       - '91'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 09:18:07 GMT
+      - Tue, 21 May 2024 09:54:22 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: '{"id": null, "uuid": null, "key": null, "content": "Hello", "metadata":
@@ -36,48 +36,48 @@
       connection:
       - keep-alive
       content-length:
       - '91'
       content-type:
       - application/json
     method: POST
-    uri: http://localhost:8000/v1/indexes/8/index
+    uri: http://localhost:8000/v1/indexes/7/index
   response:
     body:
-      string: '{"id":6,"uuid":"5b1ffc8c-d713-48a4-a3a5-2d6cfe8fc571","key":"5b1ffc8c-d713-48a4-a3a5-2d6cfe8fc571"}'
+      string: '{"id":1,"uuid":"dfe5d0db-d1d5-4643-9cdf-6cd7fe2a7e6d","key":"dfe5d0db-d1d5-4643-9cdf-6cd7fe2a7e6d"}'
     headers:
       content-length:
       - '99'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 09:18:07 GMT
+      - Tue, 21 May 2024 09:54:22 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
     method: DELETE
-    uri: http://localhost:8000/v1/indexes/8
+    uri: http://localhost:8000/v1/indexes/7
   response:
     body:
       string: 'true'
     headers:
       content-length:
       - '4'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 09:18:07 GMT
+      - Tue, 21 May 2024 09:54:22 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `opperai-0.6.2/tests/fixtures/vcr_cassettes/test_indexes/test_list_indexes.yaml` & `opperai-0.7.0/tests/fixtures/vcr_cassettes/test_indexes/test_list_indexes.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -13,15 +13,15 @@
       string: '[]'
     headers:
       content-length:
       - '2'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 09:18:07 GMT
+      - Tue, 21 May 2024 10:10:58 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: '{"name": "test_list_indexes"}'
@@ -34,22 +34,22 @@
       - '29'
       content-type:
       - application/json
     method: POST
     uri: http://localhost:8000/v1/indexes
   response:
     body:
-      string: '{"id":6,"name":"test_list_indexes","files":[],"created_at":"2024-05-02T09:18:07.426246Z"}'
+      string: '{"id":14,"name":"test_list_indexes","files":[],"created_at":"2024-05-21T10:10:58.827744Z"}'
     headers:
       content-length:
-      - '89'
+      - '90'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 09:18:07 GMT
+      - Tue, 21 May 2024 10:10:58 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
@@ -58,23 +58,23 @@
       - '*/*'
       connection:
       - keep-alive
     method: GET
     uri: http://localhost:8000/v1/indexes
   response:
     body:
-      string: '[{"id":6,"org_id":1,"org_name":null,"name":"test_list_indexes","created_by":"Mattias
-        Lundell","created_at":"2024-05-02T09:18:07.426246Z","updated_at":"2024-05-02T09:18:07.426246Z","count":0}]'
+      string: '[{"id":14,"org_id":1,"org_name":null,"name":"test_list_indexes","created_by":"Mattias
+        Lundell","created_at":"2024-05-21T10:10:58.827744Z","updated_at":"2024-05-21T10:10:58.827744Z","count":0}]'
     headers:
       content-length:
-      - '191'
+      - '192'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 09:18:07 GMT
+      - Tue, 21 May 2024 10:10:58 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: '{"name": "test_list_indexes_2"}'
@@ -87,22 +87,22 @@
       - '31'
       content-type:
       - application/json
     method: POST
     uri: http://localhost:8000/v1/indexes
   response:
     body:
-      string: '{"id":7,"name":"test_list_indexes_2","files":[],"created_at":"2024-05-02T09:18:07.459416Z"}'
+      string: '{"id":15,"name":"test_list_indexes_2","files":[],"created_at":"2024-05-21T10:10:58.862139Z"}'
     headers:
       content-length:
-      - '91'
+      - '92'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 09:18:07 GMT
+      - Tue, 21 May 2024 10:10:58 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
@@ -111,71 +111,71 @@
       - '*/*'
       connection:
       - keep-alive
     method: GET
     uri: http://localhost:8000/v1/indexes
   response:
     body:
-      string: '[{"id":6,"org_id":1,"org_name":null,"name":"test_list_indexes","created_by":"Mattias
-        Lundell","created_at":"2024-05-02T09:18:07.426246Z","updated_at":"2024-05-02T09:18:07.426246Z","count":0},{"id":7,"org_id":1,"org_name":null,"name":"test_list_indexes_2","created_by":"Mattias
-        Lundell","created_at":"2024-05-02T09:18:07.459416Z","updated_at":"2024-05-02T09:18:07.459416Z","count":0}]'
+      string: '[{"id":14,"org_id":1,"org_name":null,"name":"test_list_indexes","created_by":"Mattias
+        Lundell","created_at":"2024-05-21T10:10:58.827744Z","updated_at":"2024-05-21T10:10:58.827744Z","count":0},{"id":15,"org_id":1,"org_name":null,"name":"test_list_indexes_2","created_by":"Mattias
+        Lundell","created_at":"2024-05-21T10:10:58.862139Z","updated_at":"2024-05-21T10:10:58.862139Z","count":0}]'
     headers:
       content-length:
-      - '383'
+      - '385'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 09:18:07 GMT
+      - Tue, 21 May 2024 10:10:58 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
     method: DELETE
-    uri: http://localhost:8000/v1/indexes/7
+    uri: http://localhost:8000/v1/indexes/15
   response:
     body:
       string: 'true'
     headers:
       content-length:
       - '4'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 09:18:07 GMT
+      - Tue, 21 May 2024 10:10:58 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
     method: DELETE
-    uri: http://localhost:8000/v1/indexes/6
+    uri: http://localhost:8000/v1/indexes/14
   response:
     body:
       string: 'true'
     headers:
       content-length:
       - '4'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 09:18:07 GMT
+      - Tue, 21 May 2024 10:10:58 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `opperai-0.6.2/tests/fixtures/vcr_cassettes/test_indexes/test_retrieve_document.yaml` & `opperai-0.7.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_get_by_name.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,111 +1,79 @@
 interactions:
 - request:
-    body: '{"name": "test_retrieve_document"}'
+    body: '{"name": "test_get_by_name"}'
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
       content-length:
-      - '34'
+      - '28'
       content-type:
       - application/json
     method: POST
     uri: http://localhost:8000/v1/indexes
   response:
     body:
-      string: '{"id":9,"name":"test_retrieve_document","files":[],"created_at":"2024-05-02T09:18:07.817552Z"}'
+      string: '{"id":4,"name":"test_get_by_name","files":[],"created_at":"2024-05-21T09:54:22.973636Z"}'
     headers:
       content-length:
-      - '94'
+      - '88'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 09:18:07 GMT
+      - Tue, 21 May 2024 09:54:22 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
-    body: '{"id": null, "uuid": null, "key": null, "content": "Hello", "metadata":
-      {"source": "test"}}'
-    headers:
-      accept:
-      - '*/*'
-      connection:
-      - keep-alive
-      content-length:
-      - '91'
-      content-type:
-      - application/json
-    method: POST
-    uri: http://localhost:8000/v1/indexes/9/index
-  response:
-    body:
-      string: '{"id":7,"uuid":"4c7e92b0-950a-402e-8152-959b4b8bae86","key":"4c7e92b0-950a-402e-8152-959b4b8bae86"}'
-    headers:
-      content-length:
-      - '99'
-      content-type:
-      - application/json
-      date:
-      - Thu, 02 May 2024 09:18:07 GMT
-      server:
-      - uvicorn
-    status:
-      code: 200
-      message: OK
-- request:
-    body: '{"q": "Hello", "k": 1, "filters": null}'
+    body: ''
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
-      content-length:
-      - '39'
-      content-type:
-      - application/json
-    method: POST
-    uri: http://localhost:8000/v1/indexes/9/query
+    method: GET
+    uri: http://localhost:8000/v1/indexes
   response:
     body:
-      string: '[{"uuid":"b6542583-f101-4af0-bde6-5a6f9cb54793","content":"Hello","metadata":{"source":"test"},"document_id":null,"score":29.458036422729492,"source_uuids":["b6542583-f101-4af0-bde6-5a6f9cb54793"]}]'
+      string: '[{"id":4,"org_id":1,"org_name":null,"name":"test_get_by_name","created_by":"Mattias
+        Lundell","created_at":"2024-05-21T09:54:22.973636Z","updated_at":"2024-05-21T09:54:22.973636Z","count":0}]'
     headers:
       content-length:
-      - '198'
+      - '190'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 09:18:07 GMT
+      - Tue, 21 May 2024 09:54:22 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
     method: DELETE
-    uri: http://localhost:8000/v1/indexes/9
+    uri: http://localhost:8000/v1/indexes/4
   response:
     body:
       string: 'true'
     headers:
       content-length:
       - '4'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 09:18:08 GMT
+      - Tue, 21 May 2024 09:54:22 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `opperai-0.6.2/tests/fixtures/vcr_cassettes/test_indexes/test_retrieve_filters.yaml` & `opperai-0.7.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_retrieve_document.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -1,112 +1,111 @@
 interactions:
 - request:
-    body: '{"name": "test_retrieve_filters"}'
+    body: '{"name": "test_retrieve_document"}'
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
       content-length:
-      - '33'
+      - '34'
       content-type:
       - application/json
     method: POST
     uri: http://localhost:8000/v1/indexes
   response:
     body:
-      string: '{"id":10,"name":"test_retrieve_filters","files":[],"created_at":"2024-05-02T09:18:08.481814Z"}'
+      string: '{"id":8,"name":"test_retrieve_document","files":[],"created_at":"2024-05-21T09:54:23.440315Z"}'
     headers:
       content-length:
       - '94'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 09:18:08 GMT
+      - Tue, 21 May 2024 09:54:23 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
-    body: '{"id": null, "uuid": null, "key": null, "content": "Bonjour", "metadata":
+    body: '{"id": null, "uuid": null, "key": null, "content": "Hello", "metadata":
       {"source": "test"}}'
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
       content-length:
-      - '93'
+      - '91'
       content-type:
       - application/json
     method: POST
-    uri: http://localhost:8000/v1/indexes/10/index
+    uri: http://localhost:8000/v1/indexes/8/index
   response:
     body:
-      string: '{"id":8,"uuid":"1ed107f4-29d9-40de-8b3a-550a61efe1d4","key":"1ed107f4-29d9-40de-8b3a-550a61efe1d4"}'
+      string: '{"id":2,"uuid":"6ab00281-a041-4e54-94db-14f0dbc545e5","key":"6ab00281-a041-4e54-94db-14f0dbc545e5"}'
     headers:
       content-length:
       - '99'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 09:18:08 GMT
+      - Tue, 21 May 2024 09:54:23 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
-    body: '{"q": "test", "k": 1, "filters": [{"key": "source", "operation": "=", "value":
-      "test"}]}'
+    body: '{"q": "Hello", "k": 1, "filters": null}'
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
       content-length:
-      - '88'
+      - '39'
       content-type:
       - application/json
     method: POST
-    uri: http://localhost:8000/v1/indexes/10/query
+    uri: http://localhost:8000/v1/indexes/8/query
   response:
     body:
-      string: '[{"uuid":"9c9adf6d-f446-4cb2-b701-602b211f9491","content":"Bonjour","metadata":{"source":"test"},"document_id":null,"score":4.736573219299316,"source_uuids":["9c9adf6d-f446-4cb2-b701-602b211f9491"]}]'
+      string: '[{"uuid":"a0b8f3cd-a4a2-4eea-84f2-5b86d7e9f971","content":"Hello","metadata":{"source":"test"},"document_id":null,"score":29.458036422729492,"source_uuids":["a0b8f3cd-a4a2-4eea-84f2-5b86d7e9f971"]}]'
     headers:
       content-length:
-      - '199'
+      - '198'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 09:18:08 GMT
+      - Tue, 21 May 2024 09:54:23 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: ''
     headers:
       accept:
       - '*/*'
       connection:
       - keep-alive
     method: DELETE
-    uri: http://localhost:8000/v1/indexes/10
+    uri: http://localhost:8000/v1/indexes/8
   response:
     body:
       string: 'true'
     headers:
       content-length:
       - '4'
       content-type:
       - application/json
       date:
-      - Thu, 02 May 2024 09:18:08 GMT
+      - Tue, 21 May 2024 09:54:23 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `opperai-0.6.2/LICENSE` & `opperai-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `opperai-0.6.2/README.md` & `opperai-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `opperai-0.6.2/pyproject.toml` & `opperai-0.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "opperai"
-version = "0.6.2"
+version = "0.7.0"
 description = "Opper Python client"
 authors = [
   {name = "Opper", email = "opper@opper.ai"},
 ]
 
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `opperai-0.6.2/PKG-INFO` & `opperai-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: opperai
-Version: 0.6.2
+Version: 0.7.0
 Summary: Opper Python client
 Project-URL: Homepage, https://opper.ai
 Project-URL: Documentation, https://docs.opper.ai
 Project-URL: Platform, https://platform.opper.ai
 Author-email: Opper <opper@opper.ai>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
```

