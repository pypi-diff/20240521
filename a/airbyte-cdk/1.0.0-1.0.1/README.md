# Comparing `tmp/airbyte_cdk-1.0.0.tar.gz` & `tmp/airbyte_cdk-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_cdk-1.0.0.tar", max compression
+gzip compressed data, was "airbyte_cdk-1.0.1.tar", max compression
```

## Comparing `airbyte_cdk-1.0.0.tar` & `airbyte_cdk-1.0.1.tar`

### file list

```diff
@@ -1,288 +1,288 @@
--rw-r--r--   0        0        0     1051 2024-05-20 14:22:43.199579 airbyte_cdk-1.0.0/LICENSE.txt
--rw-r--r--   0        0        0     9977 2024-05-20 14:22:43.199579 airbyte_cdk-1.0.0/README.md
--rw-r--r--   0        0        0     9536 2024-05-20 14:22:43.199579 airbyte_cdk-1.0.0/airbyte_cdk/__init__.py
--rw-r--r--   0        0        0     3610 2024-05-20 14:22:43.199579 airbyte_cdk-1.0.0/airbyte_cdk/config_observation.py
--rw-r--r--   0        0        0     4067 2024-05-20 14:22:43.199579 airbyte_cdk-1.0.0/airbyte_cdk/connector.py
--rw-r--r--   0        0        0     1665 2024-05-20 14:22:43.199579 airbyte_cdk-1.0.0/airbyte_cdk/connector_builder/README.md
--rw-r--r--   0        0        0       61 2024-05-20 14:22:43.199579 airbyte_cdk-1.0.0/airbyte_cdk/connector_builder/__init__.py
--rw-r--r--   0        0        0     3958 2024-05-20 14:22:43.199579 airbyte_cdk-1.0.0/airbyte_cdk/connector_builder/connector_builder_handler.py
--rw-r--r--   0        0        0     3365 2024-05-20 14:22:43.199579 airbyte_cdk-1.0.0/airbyte_cdk/connector_builder/main.py
--rw-r--r--   0        0        0    17120 2024-05-20 14:22:43.199579 airbyte_cdk-1.0.0/airbyte_cdk/connector_builder/message_grouper.py
--rw-r--r--   0        0        0     1420 2024-05-20 14:22:43.199579 airbyte_cdk-1.0.0/airbyte_cdk/connector_builder/models.py
--rw-r--r--   0        0        0      126 2024-05-20 14:22:43.199579 airbyte_cdk-1.0.0/airbyte_cdk/destinations/__init__.py
--rw-r--r--   0        0        0     5420 2024-05-20 14:22:43.199579 airbyte_cdk-1.0.0/airbyte_cdk/destinations/destination.py
--rw-r--r--   0        0        0     2115 2024-05-20 14:22:43.199579 airbyte_cdk-1.0.0/airbyte_cdk/destinations/vector_db_based/README.md
--rw-r--r--   0        0        0     1006 2024-05-20 14:22:43.199579 airbyte_cdk-1.0.0/airbyte_cdk/destinations/vector_db_based/__init__.py
--rw-r--r--   0        0        0    12324 2024-05-20 14:22:43.199579 airbyte_cdk-1.0.0/airbyte_cdk/destinations/vector_db_based/config.py
--rw-r--r--   0        0        0     9081 2024-05-20 14:22:43.199579 airbyte_cdk-1.0.0/airbyte_cdk/destinations/vector_db_based/document_processor.py
--rw-r--r--   0        0        0    11443 2024-05-20 14:22:43.203579 airbyte_cdk-1.0.0/airbyte_cdk/destinations/vector_db_based/embedder.py
--rw-r--r--   0        0        0     3243 2024-05-20 14:22:43.203579 airbyte_cdk-1.0.0/airbyte_cdk/destinations/vector_db_based/indexer.py
--rw-r--r--   0        0        0     1807 2024-05-20 14:22:43.203579 airbyte_cdk-1.0.0/airbyte_cdk/destinations/vector_db_based/test_utils.py
--rw-r--r--   0        0        0     1073 2024-05-20 14:22:43.203579 airbyte_cdk-1.0.0/airbyte_cdk/destinations/vector_db_based/utils.py
--rw-r--r--   0        0        0     4394 2024-05-20 14:22:43.203579 airbyte_cdk-1.0.0/airbyte_cdk/destinations/vector_db_based/writer.py
--rw-r--r--   0        0        0    14978 2024-05-20 14:22:43.203579 airbyte_cdk-1.0.0/airbyte_cdk/entrypoint.py
--rw-r--r--   0        0        0     1930 2024-05-20 14:22:43.203579 airbyte_cdk-1.0.0/airbyte_cdk/exception_handler.py
--rw-r--r--   0        0        0     3186 2024-05-20 14:22:43.203579 airbyte_cdk-1.0.0/airbyte_cdk/logger.py
--rw-r--r--   0        0        0     1708 2024-05-20 14:22:43.203579 airbyte_cdk-1.0.0/airbyte_cdk/models/__init__.py
--rw-r--r--   0        0        0      100 2024-05-20 14:22:43.203579 airbyte_cdk-1.0.0/airbyte_cdk/models/airbyte_protocol.py
--rw-r--r--   0        0        0      117 2024-05-20 14:22:43.203579 airbyte_cdk-1.0.0/airbyte_cdk/models/well_known_types.py
--rw-r--r--   0        0        0        0 2024-05-20 14:22:43.203579 airbyte_cdk-1.0.0/airbyte_cdk/py.typed
--rw-r--r--   0        0        0     1141 2024-05-20 14:22:43.203579 airbyte_cdk-1.0.0/airbyte_cdk/sources/__init__.py
--rw-r--r--   0        0        0    14428 2024-05-20 14:22:43.203579 airbyte_cdk-1.0.0/airbyte_cdk/sources/abstract_source.py
--rw-r--r--   0        0        0       61 2024-05-20 14:22:43.203579 airbyte_cdk-1.0.0/airbyte_cdk/sources/concurrent_source/__init__.py
--rw-r--r--   0        0        0    11976 2024-05-20 14:22:43.203579 airbyte_cdk-1.0.0/airbyte_cdk/sources/concurrent_source/concurrent_read_processor.py
--rw-r--r--   0        0        0     8750 2024-05-20 14:22:43.203579 airbyte_cdk-1.0.0/airbyte_cdk/sources/concurrent_source/concurrent_source.py
--rw-r--r--   0        0        0     3691 2024-05-20 14:22:43.203579 airbyte_cdk-1.0.0/airbyte_cdk/sources/concurrent_source/concurrent_source_adapter.py
--rw-r--r--   0        0        0      696 2024-05-20 14:22:43.203579 airbyte_cdk-1.0.0/airbyte_cdk/sources/concurrent_source/partition_generation_completed_sentinel.py
--rw-r--r--   0        0        0      764 2024-05-20 14:22:43.203579 airbyte_cdk-1.0.0/airbyte_cdk/sources/concurrent_source/stream_thread_exception.py
--rw-r--r--   0        0        0     5076 2024-05-20 14:22:43.203579 airbyte_cdk-1.0.0/airbyte_cdk/sources/concurrent_source/thread_pool_manager.py
--rw-r--r--   0        0        0      856 2024-05-20 14:22:43.203579 airbyte_cdk-1.0.0/airbyte_cdk/sources/config.py
--rw-r--r--   0        0        0     9903 2024-05-20 14:22:43.203579 airbyte_cdk-1.0.0/airbyte_cdk/sources/connector_state_manager.py
--rw-r--r--   0        0        0       61 2024-05-20 14:22:43.203579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/__init__.py
--rw-r--r--   0        0        0      294 2024-05-20 14:22:43.203579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/auth/__init__.py
--rw-r--r--   0        0        0     1090 2024-05-20 14:22:43.203579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/auth/declarative_authenticator.py
--rw-r--r--   0        0        0     8007 2024-05-20 14:22:43.203579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/auth/jwt.py
--rw-r--r--   0        0        0     8272 2024-05-20 14:22:43.203579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/auth/oauth.py
--rw-r--r--   0        0        0     1347 2024-05-20 14:22:43.203579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/auth/selective_authenticator.py
--rw-r--r--   0        0        0    11032 2024-05-20 14:22:43.203579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/auth/token.py
--rw-r--r--   0        0        0     2887 2024-05-20 14:22:43.203579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/auth/token_provider.py
--rw-r--r--   0        0        0      274 2024-05-20 14:22:43.203579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/checks/__init__.py
--rw-r--r--   0        0        0     2154 2024-05-20 14:22:43.203579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/checks/check_stream.py
--rw-r--r--   0        0        0     1368 2024-05-20 14:22:43.203579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/checks/connection_checker.py
--rw-r--r--   0        0        0      177 2024-05-20 14:22:43.203579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/datetime/__init__.py
--rw-r--r--   0        0        0     2369 2024-05-20 14:22:43.203579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/datetime/datetime_parser.py
--rw-r--r--   0        0        0     5187 2024-05-20 14:22:43.203579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/datetime/min_max_datetime.py
--rw-r--r--   0        0        0    97462 2024-05-20 14:22:43.203579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/declarative_component_schema.yaml
--rw-r--r--   0        0        0     1517 2024-05-20 14:22:43.203579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/declarative_source.py
--rw-r--r--   0        0        0     7495 2024-05-20 14:22:43.203579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/declarative_stream.py
--rw-r--r--   0        0        0      247 2024-05-20 14:22:43.203579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/decoders/__init__.py
--rw-r--r--   0        0        0      639 2024-05-20 14:22:43.203579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/decoders/decoder.py
--rw-r--r--   0        0        0      637 2024-05-20 14:22:43.203579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/decoders/json_decoder.py
--rw-r--r--   0        0        0      176 2024-05-20 14:22:43.203579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/exceptions.py
--rw-r--r--   0        0        0      478 2024-05-20 14:22:43.203579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/extractors/__init__.py
--rw-r--r--   0        0        0     2990 2024-05-20 14:22:43.203579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/extractors/dpath_extractor.py
--rw-r--r--   0        0        0     1213 2024-05-20 14:22:43.203579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/extractors/http_selector.py
--rw-r--r--   0        0        0      691 2024-05-20 14:22:43.203579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/extractors/record_extractor.py
--rw-r--r--   0        0        0     1421 2024-05-20 14:22:43.203579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/extractors/record_filter.py
--rw-r--r--   0        0        0     4671 2024-05-20 14:22:43.203579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/extractors/record_selector.py
--rw-r--r--   0        0        0      459 2024-05-20 14:22:43.203579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/incremental/__init__.py
--rw-r--r--   0        0        0    18380 2024-05-20 14:22:43.203579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/incremental/datetime_based_cursor.py
--rw-r--r--   0        0        0      536 2024-05-20 14:22:43.203579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/incremental/declarative_cursor.py
--rw-r--r--   0        0        0    12286 2024-05-20 14:22:43.203579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/incremental/per_partition_cursor.py
--rw-r--r--   0        0        0      437 2024-05-20 14:22:43.203579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/interpolation/__init__.py
--rw-r--r--   0        0        0     3331 2024-05-20 14:22:43.203579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/interpolation/filters.py
--rw-r--r--   0        0        0     1844 2024-05-20 14:22:43.203579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/interpolation/interpolated_boolean.py
--rw-r--r--   0        0        0     2018 2024-05-20 14:22:43.203579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/interpolation/interpolated_mapping.py
--rw-r--r--   0        0        0     1791 2024-05-20 14:22:43.203579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/interpolation/interpolated_nested_mapping.py
--rw-r--r--   0        0        0     2443 2024-05-20 14:22:43.203579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/interpolation/interpolated_string.py
--rw-r--r--   0        0        0      934 2024-05-20 14:22:43.203579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/interpolation/interpolation.py
--rw-r--r--   0        0        0     5367 2024-05-20 14:22:43.203579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/interpolation/jinja.py
--rw-r--r--   0        0        0     3556 2024-05-20 14:22:43.203579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/interpolation/macros.py
--rw-r--r--   0        0        0    12253 2024-05-20 14:22:43.207579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/manifest_declarative_source.py
--rw-r--r--   0        0        0        0 2024-05-20 14:22:43.207579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/migrations/__init__.py
--rw-r--r--   0        0        0     3729 2024-05-20 14:22:43.207579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/migrations/legacy_to_per_partition_state_migration.py
--rw-r--r--   0        0        0      794 2024-05-20 14:22:43.207579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/migrations/state_migration.py
--rw-r--r--   0        0        0       93 2024-05-20 14:22:43.207579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/models/__init__.py
--rw-r--r--   0        0        0    65245 2024-05-20 14:22:43.207579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/models/declarative_component_schema.py
--rw-r--r--   0        0        0       61 2024-05-20 14:22:43.207579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/parsers/__init__.py
--rw-r--r--   0        0        0     6204 2024-05-20 14:22:43.207579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/parsers/class_types_registry.py
--rw-r--r--   0        0        0      553 2024-05-20 14:22:43.207579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/parsers/custom_exceptions.py
--rw-r--r--   0        0        0     3801 2024-05-20 14:22:43.207579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/parsers/default_implementation_registry.py
--rw-r--r--   0        0        0     8287 2024-05-20 14:22:43.207579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/parsers/manifest_component_transformer.py
--rw-r--r--   0        0        0     6728 2024-05-20 14:22:43.207579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/parsers/manifest_reference_resolver.py
--rw-r--r--   0        0        0    63618 2024-05-20 14:22:43.207579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/parsers/model_to_component_factory.py
--rw-r--r--   0        0        0      476 2024-05-20 14:22:43.207579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/partition_routers/__init__.py
--rw-r--r--   0        0        0     4312 2024-05-20 14:22:43.207579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/partition_routers/list_partition_router.py
--rw-r--r--   0        0        0     1599 2024-05-20 14:22:43.207579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/partition_routers/single_partition_router.py
--rw-r--r--   0        0        0     7952 2024-05-20 14:22:43.207579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/partition_routers/substream_partition_router.py
--rw-r--r--   0        0        0      364 2024-05-20 14:22:43.207579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/requesters/__init__.py
--rw-r--r--   0        0        0      717 2024-05-20 14:22:43.207579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/requesters/error_handlers/__init__.py
--rw-r--r--   0        0        0      875 2024-05-20 14:22:43.207579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/requesters/error_handlers/backoff_strategies/__init__.py
--rw-r--r--   0        0        0     1571 2024-05-20 14:22:43.207579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/requesters/error_handlers/backoff_strategies/constant_backoff_strategy.py
--rw-r--r--   0        0        0     1366 2024-05-20 14:22:43.207579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/requesters/error_handlers/backoff_strategies/exponential_backoff_strategy.py
--rw-r--r--   0        0        0     1156 2024-05-20 14:22:43.207579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/requesters/error_handlers/backoff_strategies/header_helper.py
--rw-r--r--   0        0        0     1816 2024-05-20 14:22:43.207579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/requesters/error_handlers/backoff_strategies/wait_time_from_header_backoff_strategy.py
--rw-r--r--   0        0        0     2803 2024-05-20 14:22:43.207579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/requesters/error_handlers/backoff_strategies/wait_until_time_from_header_backoff_strategy.py
--rw-r--r--   0        0        0      697 2024-05-20 14:22:43.207579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/requesters/error_handlers/backoff_strategy.py
--rw-r--r--   0        0        0     2476 2024-05-20 14:22:43.207579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/requesters/error_handlers/composite_error_handler.py
--rw-r--r--   0        0        0     6041 2024-05-20 14:22:43.207579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/requesters/error_handlers/default_error_handler.py
--rw-r--r--   0        0        0     1141 2024-05-20 14:22:43.207579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/requesters/error_handlers/error_handler.py
--rw-r--r--   0        0        0     4979 2024-05-20 14:22:43.207579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/requesters/error_handlers/http_response_filter.py
--rw-r--r--   0        0        0      405 2024-05-20 14:22:43.207579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/requesters/error_handlers/response_action.py
--rw-r--r--   0        0        0     2656 2024-05-20 14:22:43.207579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/requesters/error_handlers/response_status.py
--rw-r--r--   0        0        0    27968 2024-05-20 14:22:43.207579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/requesters/http_requester.py
--rw-r--r--   0        0        0      599 2024-05-20 14:22:43.207579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/requesters/paginators/__init__.py
--rw-r--r--   0        0        0    10305 2024-05-20 14:22:43.207579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/requesters/paginators/default_paginator.py
--rw-r--r--   0        0        0     1877 2024-05-20 14:22:43.207579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/requesters/paginators/no_pagination.py
--rw-r--r--   0        0        0     1927 2024-05-20 14:22:43.207579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/requesters/paginators/paginator.py
--rw-r--r--   0        0        0      740 2024-05-20 14:22:43.207579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/requesters/paginators/strategies/__init__.py
--rw-r--r--   0        0        0     3445 2024-05-20 14:22:43.207579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/requesters/paginators/strategies/cursor_pagination_strategy.py
--rw-r--r--   0        0        0     2887 2024-05-20 14:22:43.207579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/requesters/paginators/strategies/offset_increment.py
--rw-r--r--   0        0        0     2152 2024-05-20 14:22:43.207579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/requesters/paginators/strategies/page_increment.py
--rw-r--r--   0        0        0     1240 2024-05-20 14:22:43.207579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/requesters/paginators/strategies/pagination_strategy.py
--rw-r--r--   0        0        0     1967 2024-05-20 14:22:43.207579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/requesters/paginators/strategies/stop_condition.py
--rw-r--r--   0        0        0     1055 2024-05-20 14:22:43.207579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/requesters/request_option.py
--rw-r--r--   0        0        0      410 2024-05-20 14:22:43.207579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/requesters/request_options/__init__.py
--rw-r--r--   0        0        0     2275 2024-05-20 14:22:43.207579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/requesters/request_options/interpolated_nested_request_input_provider.py
--rw-r--r--   0        0        0     2883 2024-05-20 14:22:43.207579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/requesters/request_options/interpolated_request_input_provider.py
--rw-r--r--   0        0        0     4995 2024-05-20 14:22:43.207579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/requesters/request_options/interpolated_request_options_provider.py
--rw-r--r--   0        0        0     2590 2024-05-20 14:22:43.207579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/requesters/request_options/request_options_provider.py
--rw-r--r--   0        0        0      299 2024-05-20 14:22:43.207579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/requesters/request_path.py
--rw-r--r--   0        0        0     5539 2024-05-20 14:22:43.207579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/requesters/requester.py
--rw-r--r--   0        0        0      339 2024-05-20 14:22:43.207579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/retrievers/__init__.py
--rw-r--r--   0        0        0     1741 2024-05-20 14:22:43.207579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/retrievers/retriever.py
--rw-r--r--   0        0        0    19727 2024-05-20 14:22:43.207579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/retrievers/simple_retriever.py
--rw-r--r--   0        0        0      517 2024-05-20 14:22:43.207579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/schema/__init__.py
--rw-r--r--   0        0        0     1790 2024-05-20 14:22:43.207579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/schema/default_schema_loader.py
--rw-r--r--   0        0        0      464 2024-05-20 14:22:43.207579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/schema/inline_schema_loader.py
--rw-r--r--   0        0        0     4150 2024-05-20 14:22:43.207579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/schema/json_file_schema_loader.py
--rw-r--r--   0        0        0      379 2024-05-20 14:22:43.207579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/schema/schema_loader.py
--rw-r--r--   0        0        0      141 2024-05-20 14:22:43.207579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/spec/__init__.py
--rw-r--r--   0        0        0     1786 2024-05-20 14:22:43.207579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/spec/spec.py
--rw-r--r--   0        0        0      328 2024-05-20 14:22:43.207579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/stream_slicers/__init__.py
--rw-r--r--   0        0        0     4721 2024-05-20 14:22:43.207579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/stream_slicers/cartesian_product_stream_slicer.py
--rw-r--r--   0        0        0      856 2024-05-20 14:22:43.207579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/stream_slicers/stream_slicer.py
--rw-r--r--   0        0        0      919 2024-05-20 14:22:43.211579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/transformations/__init__.py
--rw-r--r--   0        0        0     4884 2024-05-20 14:22:43.211579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/transformations/add_fields.py
--rw-r--r--   0        0        0     2725 2024-05-20 14:22:43.211579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/transformations/remove_fields.py
--rw-r--r--   0        0        0     1123 2024-05-20 14:22:43.211579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/transformations/transformation.py
--rw-r--r--   0        0        0      749 2024-05-20 14:22:43.211579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/types.py
--rw-r--r--   0        0        0     1879 2024-05-20 14:22:43.211579 airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/yaml_declarative_source.py
--rw-r--r--   0        0        0       61 2024-05-20 14:22:43.211579 airbyte_cdk-1.0.0/airbyte_cdk/sources/embedded/__init__.py
--rw-r--r--   0        0        0     2264 2024-05-20 14:22:43.211579 airbyte_cdk-1.0.0/airbyte_cdk/sources/embedded/base_integration.py
--rw-r--r--   0        0        0     1571 2024-05-20 14:22:43.211579 airbyte_cdk-1.0.0/airbyte_cdk/sources/embedded/catalog.py
--rw-r--r--   0        0        0     1390 2024-05-20 14:22:43.211579 airbyte_cdk-1.0.0/airbyte_cdk/sources/embedded/runner.py
--rw-r--r--   0        0        0      744 2024-05-20 14:22:43.211579 airbyte_cdk-1.0.0/airbyte_cdk/sources/embedded/tools.py
--rw-r--r--   0        0        0    11085 2024-05-20 14:22:43.211579 airbyte_cdk-1.0.0/airbyte_cdk/sources/file_based/README.md
--rw-r--r--   0        0        0      868 2024-05-20 14:22:43.211579 airbyte_cdk-1.0.0/airbyte_cdk/sources/file_based/__init__.py
--rw-r--r--   0        0        0      371 2024-05-20 14:22:43.211579 airbyte_cdk-1.0.0/airbyte_cdk/sources/file_based/availability_strategy/__init__.py
--rw-r--r--   0        0        0     2137 2024-05-20 14:22:43.211579 airbyte_cdk-1.0.0/airbyte_cdk/sources/file_based/availability_strategy/abstract_file_based_availability_strategy.py
--rw-r--r--   0        0        0     5289 2024-05-20 14:22:43.211579 airbyte_cdk-1.0.0/airbyte_cdk/sources/file_based/availability_strategy/default_file_based_availability_strategy.py
--rw-r--r--   0        0        0        0 2024-05-20 14:22:43.211579 airbyte_cdk-1.0.0/airbyte_cdk/sources/file_based/config/__init__.py
--rw-r--r--   0        0        0     4956 2024-05-20 14:22:43.211579 airbyte_cdk-1.0.0/airbyte_cdk/sources/file_based/config/abstract_file_based_spec.py
--rw-r--r--   0        0        0      712 2024-05-20 14:22:43.211579 airbyte_cdk-1.0.0/airbyte_cdk/sources/file_based/config/avro_format.py
--rw-r--r--   0        0        0     7804 2024-05-20 14:22:43.211579 airbyte_cdk-1.0.0/airbyte_cdk/sources/file_based/config/csv_format.py
--rw-r--r--   0        0        0     4229 2024-05-20 14:22:43.211579 airbyte_cdk-1.0.0/airbyte_cdk/sources/file_based/config/file_based_stream_config.py
--rw-r--r--   0        0        0      374 2024-05-20 14:22:43.211579 airbyte_cdk-1.0.0/airbyte_cdk/sources/file_based/config/jsonl_format.py
--rw-r--r--   0        0        0      737 2024-05-20 14:22:43.211579 airbyte_cdk-1.0.0/airbyte_cdk/sources/file_based/config/parquet_format.py
--rw-r--r--   0        0        0     3513 2024-05-20 14:22:43.211579 airbyte_cdk-1.0.0/airbyte_cdk/sources/file_based/config/unstructured_format.py
--rw-r--r--   0        0        0      283 2024-05-20 14:22:43.211579 airbyte_cdk-1.0.0/airbyte_cdk/sources/file_based/discovery_policy/__init__.py
--rw-r--r--   0        0        0      621 2024-05-20 14:22:43.211579 airbyte_cdk-1.0.0/airbyte_cdk/sources/file_based/discovery_policy/abstract_discovery_policy.py
--rw-r--r--   0        0        0      939 2024-05-20 14:22:43.211579 airbyte_cdk-1.0.0/airbyte_cdk/sources/file_based/discovery_policy/default_discovery_policy.py
--rw-r--r--   0        0        0     5613 2024-05-20 14:22:43.211579 airbyte_cdk-1.0.0/airbyte_cdk/sources/file_based/exceptions.py
--rw-r--r--   0        0        0    13784 2024-05-20 14:22:43.211579 airbyte_cdk-1.0.0/airbyte_cdk/sources/file_based/file_based_source.py
--rw-r--r--   0        0        0     3749 2024-05-20 14:22:43.211579 airbyte_cdk-1.0.0/airbyte_cdk/sources/file_based/file_based_stream_reader.py
--rw-r--r--   0        0        0     1017 2024-05-20 14:22:43.211579 airbyte_cdk-1.0.0/airbyte_cdk/sources/file_based/file_types/__init__.py
--rw-r--r--   0        0        0     9167 2024-05-20 14:22:43.211579 airbyte_cdk-1.0.0/airbyte_cdk/sources/file_based/file_types/avro_parser.py
--rw-r--r--   0        0        0    19461 2024-05-20 14:22:43.211579 airbyte_cdk-1.0.0/airbyte_cdk/sources/file_based/file_types/csv_parser.py
--rw-r--r--   0        0        0     2819 2024-05-20 14:22:43.211579 airbyte_cdk-1.0.0/airbyte_cdk/sources/file_based/file_types/file_type_parser.py
--rw-r--r--   0        0        0     5666 2024-05-20 14:22:43.211579 airbyte_cdk-1.0.0/airbyte_cdk/sources/file_based/file_types/jsonl_parser.py
--rw-r--r--   0        0        0     9998 2024-05-20 14:22:43.211579 airbyte_cdk-1.0.0/airbyte_cdk/sources/file_based/file_types/parquet_parser.py
--rw-r--r--   0        0        0    16736 2024-05-20 14:22:43.211579 airbyte_cdk-1.0.0/airbyte_cdk/sources/file_based/file_types/unstructured_parser.py
--rw-r--r--   0        0        0      312 2024-05-20 14:22:43.211579 airbyte_cdk-1.0.0/airbyte_cdk/sources/file_based/remote_file.py
--rw-r--r--   0        0        0     9291 2024-05-20 14:22:43.211579 airbyte_cdk-1.0.0/airbyte_cdk/sources/file_based/schema_helpers.py
--rw-r--r--   0        0        0      527 2024-05-20 14:22:43.211579 airbyte_cdk-1.0.0/airbyte_cdk/sources/file_based/schema_validation_policies/__init__.py
--rw-r--r--   0        0        0      604 2024-05-20 14:22:43.211579 airbyte_cdk-1.0.0/airbyte_cdk/sources/file_based/schema_validation_policies/abstract_schema_validation_policy.py
--rw-r--r--   0        0        0     1643 2024-05-20 14:22:43.211579 airbyte_cdk-1.0.0/airbyte_cdk/sources/file_based/schema_validation_policies/default_schema_validation_policies.py
--rw-r--r--   0        0        0      265 2024-05-20 14:22:43.211579 airbyte_cdk-1.0.0/airbyte_cdk/sources/file_based/stream/__init__.py
--rw-r--r--   0        0        0     6557 2024-05-20 14:22:43.211579 airbyte_cdk-1.0.0/airbyte_cdk/sources/file_based/stream/abstract_file_based_stream.py
--rw-r--r--   0        0        0        0 2024-05-20 14:22:43.211579 airbyte_cdk-1.0.0/airbyte_cdk/sources/file_based/stream/concurrent/__init__.py
--rw-r--r--   0        0        0    12818 2024-05-20 14:22:43.211579 airbyte_cdk-1.0.0/airbyte_cdk/sources/file_based/stream/concurrent/adapters.py
--rw-r--r--   0        0        0      329 2024-05-20 14:22:43.211579 airbyte_cdk-1.0.0/airbyte_cdk/sources/file_based/stream/concurrent/cursor/__init__.py
--rw-r--r--   0        0        0     1961 2024-05-20 14:22:43.211579 airbyte_cdk-1.0.0/airbyte_cdk/sources/file_based/stream/concurrent/cursor/abstract_concurrent_file_based_cursor.py
--rw-r--r--   0        0        0    14331 2024-05-20 14:22:43.211579 airbyte_cdk-1.0.0/airbyte_cdk/sources/file_based/stream/concurrent/cursor/file_based_concurrent_cursor.py
--rw-r--r--   0        0        0     3150 2024-05-20 14:22:43.211579 airbyte_cdk-1.0.0/airbyte_cdk/sources/file_based/stream/concurrent/cursor/file_based_final_state_cursor.py
--rw-r--r--   0        0        0      191 2024-05-20 14:22:43.211579 airbyte_cdk-1.0.0/airbyte_cdk/sources/file_based/stream/cursor/__init__.py
--rw-r--r--   0        0        0     1920 2024-05-20 14:22:43.211579 airbyte_cdk-1.0.0/airbyte_cdk/sources/file_based/stream/cursor/abstract_file_based_cursor.py
--rw-r--r--   0        0        0     6815 2024-05-20 14:22:43.211579 airbyte_cdk-1.0.0/airbyte_cdk/sources/file_based/stream/cursor/default_file_based_cursor.py
--rw-r--r--   0        0        0    13113 2024-05-20 14:22:43.211579 airbyte_cdk-1.0.0/airbyte_cdk/sources/file_based/stream/default_file_based_stream.py
--rw-r--r--   0        0        0      218 2024-05-20 14:22:43.211579 airbyte_cdk-1.0.0/airbyte_cdk/sources/file_based/types.py
--rw-r--r--   0        0        0      730 2024-05-20 14:22:43.211579 airbyte_cdk-1.0.0/airbyte_cdk/sources/http_config.py
--rw-r--r--   0        0        0     1437 2024-05-20 14:22:43.211579 airbyte_cdk-1.0.0/airbyte_cdk/sources/http_logger.py
--rw-r--r--   0        0        0      372 2024-05-20 14:22:43.211579 airbyte_cdk-1.0.0/airbyte_cdk/sources/message/__init__.py
--rw-r--r--   0        0        0     4583 2024-05-20 14:22:43.211579 airbyte_cdk-1.0.0/airbyte_cdk/sources/message/repository.py
--rw-r--r--   0        0        0     4412 2024-05-20 14:22:43.211579 airbyte_cdk-1.0.0/airbyte_cdk/sources/source.py
--rw-r--r--   0        0        0      256 2024-05-20 14:22:43.211579 airbyte_cdk-1.0.0/airbyte_cdk/sources/streams/__init__.py
--rw-r--r--   0        0        0     1007 2024-05-20 14:22:43.211579 airbyte_cdk-1.0.0/airbyte_cdk/sources/streams/availability_strategy.py
--rw-r--r--   0        0        0    20555 2024-05-20 14:22:43.211579 airbyte_cdk-1.0.0/airbyte_cdk/sources/streams/call_rate.py
--rw-r--r--   0        0        0      408 2024-05-20 14:22:43.211579 airbyte_cdk-1.0.0/airbyte_cdk/sources/streams/checkpoint/__init__.py
--rw-r--r--   0        0        0     4893 2024-05-20 14:22:43.211579 airbyte_cdk-1.0.0/airbyte_cdk/sources/streams/checkpoint/checkpoint_reader.py
--rw-r--r--   0        0        0     2946 2024-05-20 14:22:43.211579 airbyte_cdk-1.0.0/airbyte_cdk/sources/streams/checkpoint/cursor.py
--rw-r--r--   0        0        0     1070 2024-05-20 14:22:43.211579 airbyte_cdk-1.0.0/airbyte_cdk/sources/streams/concurrent/README.md
--rw-r--r--   0        0        0       61 2024-05-20 14:22:43.215579 airbyte_cdk-1.0.0/airbyte_cdk/sources/streams/concurrent/__init__.py
--rw-r--r--   0        0        0     3792 2024-05-20 14:22:43.215579 airbyte_cdk-1.0.0/airbyte_cdk/sources/streams/concurrent/abstract_stream.py
--rw-r--r--   0        0        0     1358 2024-05-20 14:22:43.215579 airbyte_cdk-1.0.0/airbyte_cdk/sources/streams/concurrent/abstract_stream_facade.py
--rw-r--r--   0        0        0    16279 2024-05-20 14:22:43.215579 airbyte_cdk-1.0.0/airbyte_cdk/sources/streams/concurrent/adapters.py
--rw-r--r--   0        0        0     2013 2024-05-20 14:22:43.215579 airbyte_cdk-1.0.0/airbyte_cdk/sources/streams/concurrent/availability_strategy.py
--rw-r--r--   0        0        0    15155 2024-05-20 14:22:43.215579 airbyte_cdk-1.0.0/airbyte_cdk/sources/streams/concurrent/cursor.py
--rw-r--r--   0        0        0     3059 2024-05-20 14:22:43.215579 airbyte_cdk-1.0.0/airbyte_cdk/sources/streams/concurrent/default_stream.py
--rw-r--r--   0        0        0      468 2024-05-20 14:22:43.215579 airbyte_cdk-1.0.0/airbyte_cdk/sources/streams/concurrent/exceptions.py
--rw-r--r--   0        0        0     1290 2024-05-20 14:22:43.215579 airbyte_cdk-1.0.0/airbyte_cdk/sources/streams/concurrent/helpers.py
--rw-r--r--   0        0        0     3315 2024-05-20 14:22:43.215579 airbyte_cdk-1.0.0/airbyte_cdk/sources/streams/concurrent/partition_enqueuer.py
--rw-r--r--   0        0        0     1747 2024-05-20 14:22:43.215579 airbyte_cdk-1.0.0/airbyte_cdk/sources/streams/concurrent/partition_reader.py
--rw-r--r--   0        0        0       61 2024-05-20 14:22:43.215579 airbyte_cdk-1.0.0/airbyte_cdk/sources/streams/concurrent/partitions/__init__.py
--rw-r--r--   0        0        0     1795 2024-05-20 14:22:43.215579 airbyte_cdk-1.0.0/airbyte_cdk/sources/streams/concurrent/partitions/partition.py
--rw-r--r--   0        0        0      441 2024-05-20 14:22:43.215579 airbyte_cdk-1.0.0/airbyte_cdk/sources/streams/concurrent/partitions/partition_generator.py
--rw-r--r--   0        0        0      600 2024-05-20 14:22:43.215579 airbyte_cdk-1.0.0/airbyte_cdk/sources/streams/concurrent/partitions/record.py
--rw-r--r--   0        0        0     1182 2024-05-20 14:22:43.215579 airbyte_cdk-1.0.0/airbyte_cdk/sources/streams/concurrent/partitions/types.py
--rw-r--r--   0        0        0        0 2024-05-20 14:22:43.215579 airbyte_cdk-1.0.0/airbyte_cdk/sources/streams/concurrent/state_converters/__init__.py
--rw-r--r--   0        0        0     5539 2024-05-20 14:22:43.215579 airbyte_cdk-1.0.0/airbyte_cdk/sources/streams/concurrent/state_converters/abstract_stream_state_converter.py
--rw-r--r--   0        0        0     5504 2024-05-20 14:22:43.215579 airbyte_cdk-1.0.0/airbyte_cdk/sources/streams/concurrent/state_converters/datetime_stream_state_converter.py
--rw-r--r--   0        0        0    22387 2024-05-20 14:22:43.215579 airbyte_cdk-1.0.0/airbyte_cdk/sources/streams/core.py
--rw-r--r--   0        0        0      311 2024-05-20 14:22:43.215579 airbyte_cdk-1.0.0/airbyte_cdk/sources/streams/http/__init__.py
--rw-r--r--   0        0        0     6884 2024-05-20 14:22:43.215579 airbyte_cdk-1.0.0/airbyte_cdk/sources/streams/http/availability_strategy.py
--rw-r--r--   0        0        0      665 2024-05-20 14:22:43.215579 airbyte_cdk-1.0.0/airbyte_cdk/sources/streams/http/error_handlers/__init__.py
--rw-r--r--   0        0        0      826 2024-05-20 14:22:43.215579 airbyte_cdk-1.0.0/airbyte_cdk/sources/streams/http/error_handlers/backoff_strategy.py
--rw-r--r--   0        0        0      991 2024-05-20 14:22:43.215579 airbyte_cdk-1.0.0/airbyte_cdk/sources/streams/http/error_handlers/default_backoff_strategy.py
--rw-r--r--   0        0        0      781 2024-05-20 14:22:43.215579 airbyte_cdk-1.0.0/airbyte_cdk/sources/streams/http/error_handlers/error_handler.py
--rw-r--r--   0        0        0      456 2024-05-20 14:22:43.215579 airbyte_cdk-1.0.0/airbyte_cdk/sources/streams/http/error_handlers/error_message_parser.py
--rw-r--r--   0        0        0     6172 2024-05-20 14:22:43.215579 airbyte_cdk-1.0.0/airbyte_cdk/sources/streams/http/error_handlers/http_status_error_handler.py
--rw-r--r--   0        0        0     1491 2024-05-20 14:22:43.215579 airbyte_cdk-1.0.0/airbyte_cdk/sources/streams/http/error_handlers/json_error_message_parser.py
--rw-r--r--   0        0        0      476 2024-05-20 14:22:43.215579 airbyte_cdk-1.0.0/airbyte_cdk/sources/streams/http/error_handlers/response_models.py
--rw-r--r--   0        0        0     1743 2024-05-20 14:22:43.215579 airbyte_cdk-1.0.0/airbyte_cdk/sources/streams/http/exceptions.py
--rw-r--r--   0        0        0    24016 2024-05-20 14:22:43.215579 airbyte_cdk-1.0.0/airbyte_cdk/sources/streams/http/http.py
--rw-r--r--   0        0        0    11292 2024-05-20 14:22:43.215579 airbyte_cdk-1.0.0/airbyte_cdk/sources/streams/http/http_client.py
--rw-r--r--   0        0        0     5258 2024-05-20 14:22:43.215579 airbyte_cdk-1.0.0/airbyte_cdk/sources/streams/http/rate_limiting.py
--rw-r--r--   0        0        0      413 2024-05-20 14:22:43.215579 airbyte_cdk-1.0.0/airbyte_cdk/sources/streams/http/requests_native_auth/__init__.py
--rw-r--r--   0        0        0    10125 2024-05-20 14:22:43.215579 airbyte_cdk-1.0.0/airbyte_cdk/sources/streams/http/requests_native_auth/abstract_oauth.py
--rw-r--r--   0        0        0      961 2024-05-20 14:22:43.215579 airbyte_cdk-1.0.0/airbyte_cdk/sources/streams/http/requests_native_auth/abstract_token.py
--rw-r--r--   0        0        0    13381 2024-05-20 14:22:43.215579 airbyte_cdk-1.0.0/airbyte_cdk/sources/streams/http/requests_native_auth/oauth.py
--rw-r--r--   0        0        0     2456 2024-05-20 14:22:43.215579 airbyte_cdk-1.0.0/airbyte_cdk/sources/streams/http/requests_native_auth/token.py
--rw-r--r--   0        0        0       61 2024-05-20 14:22:43.215579 airbyte_cdk-1.0.0/airbyte_cdk/sources/streams/utils/__init__.py
--rw-r--r--   0        0        0     1645 2024-05-20 14:22:43.215579 airbyte_cdk-1.0.0/airbyte_cdk/sources/streams/utils/stream_helper.py
--rw-r--r--   0        0        0     3588 2024-05-20 14:22:43.215579 airbyte_cdk-1.0.0/airbyte_cdk/sources/types.py
--rw-r--r--   0        0        0      118 2024-05-20 14:22:43.215579 airbyte_cdk-1.0.0/airbyte_cdk/sources/utils/__init__.py
--rw-r--r--   0        0        0      256 2024-05-20 14:22:43.215579 airbyte_cdk-1.0.0/airbyte_cdk/sources/utils/casing.py
--rw-r--r--   0        0        0      714 2024-05-20 14:22:43.215579 airbyte_cdk-1.0.0/airbyte_cdk/sources/utils/catalog_helpers.py
--rw-r--r--   0        0        0     1711 2024-05-20 14:22:43.215579 airbyte_cdk-1.0.0/airbyte_cdk/sources/utils/record_helper.py
--rw-r--r--   0        0        0     8483 2024-05-20 14:22:43.215579 airbyte_cdk-1.0.0/airbyte_cdk/sources/utils/schema_helpers.py
--rw-r--r--   0        0        0     3151 2024-05-20 14:22:43.215579 airbyte_cdk-1.0.0/airbyte_cdk/sources/utils/schema_models.py
--rw-r--r--   0        0        0     1731 2024-05-20 14:22:43.215579 airbyte_cdk-1.0.0/airbyte_cdk/sources/utils/slice_logger.py
--rw-r--r--   0        0        0     9493 2024-05-20 14:22:43.215579 airbyte_cdk-1.0.0/airbyte_cdk/sources/utils/transform.py
--rw-r--r--   0        0        0      175 2024-05-20 14:22:43.215579 airbyte_cdk-1.0.0/airbyte_cdk/sources/utils/types.py
--rw-r--r--   0        0        0      199 2024-05-20 14:22:43.215579 airbyte_cdk-1.0.0/airbyte_cdk/test/__init__.py
--rw-r--r--   0        0        0     2691 2024-05-20 14:22:43.215579 airbyte_cdk-1.0.0/airbyte_cdk/test/catalog_builder.py
--rw-r--r--   0        0        0     7399 2024-05-20 14:22:43.215579 airbyte_cdk-1.0.0/airbyte_cdk/test/entrypoint_wrapper.py
--rw-r--r--   0        0        0      322 2024-05-20 14:22:43.215579 airbyte_cdk-1.0.0/airbyte_cdk/test/mock_http/__init__.py
--rw-r--r--   0        0        0     1240 2024-05-20 14:22:43.215579 airbyte_cdk-1.0.0/airbyte_cdk/test/mock_http/matcher.py
--rw-r--r--   0        0        0     6412 2024-05-20 14:22:43.215579 airbyte_cdk-1.0.0/airbyte_cdk/test/mock_http/mocker.py
--rw-r--r--   0        0        0     3687 2024-05-20 14:22:43.215579 airbyte_cdk-1.0.0/airbyte_cdk/test/mock_http/request.py
--rw-r--r--   0        0        0      588 2024-05-20 14:22:43.215579 airbyte_cdk-1.0.0/airbyte_cdk/test/mock_http/response.py
--rw-r--r--   0        0        0     7789 2024-05-20 14:22:43.215579 airbyte_cdk-1.0.0/airbyte_cdk/test/mock_http/response_builder.py
--rw-r--r--   0        0        0      609 2024-05-20 14:22:43.215579 airbyte_cdk-1.0.0/airbyte_cdk/test/state_builder.py
--rw-r--r--   0        0        0      294 2024-05-20 14:22:43.215579 airbyte_cdk-1.0.0/airbyte_cdk/utils/__init__.py
--rw-r--r--   0        0        0     3079 2024-05-20 14:22:43.215579 airbyte_cdk-1.0.0/airbyte_cdk/utils/airbyte_secrets_utils.py
--rw-r--r--   0        0        0      598 2024-05-20 14:22:43.215579 airbyte_cdk-1.0.0/airbyte_cdk/utils/analytics_message.py
--rw-r--r--   0        0        0      108 2024-05-20 14:22:43.215579 airbyte_cdk-1.0.0/airbyte_cdk/utils/constants.py
--rw-r--r--   0        0        0     3954 2024-05-20 14:22:43.215579 airbyte_cdk-1.0.0/airbyte_cdk/utils/datetime_format_inferrer.py
--rw-r--r--   0        0        0     2377 2024-05-20 14:22:43.215579 airbyte_cdk-1.0.0/airbyte_cdk/utils/event_timing.py
--rw-r--r--   0        0        0      574 2024-05-20 14:22:43.215579 airbyte_cdk-1.0.0/airbyte_cdk/utils/is_cloud_environment.py
--rw-r--r--   0        0        0     1729 2024-05-20 14:22:43.215579 airbyte_cdk-1.0.0/airbyte_cdk/utils/mapping_helpers.py
--rw-r--r--   0        0        0      953 2024-05-20 14:22:43.215579 airbyte_cdk-1.0.0/airbyte_cdk/utils/message_utils.py
--rw-r--r--   0        0        0     1180 2024-05-20 14:22:43.215579 airbyte_cdk-1.0.0/airbyte_cdk/utils/oneof_option_config.py
--rw-r--r--   0        0        0     8622 2024-05-20 14:22:43.215579 airbyte_cdk-1.0.0/airbyte_cdk/utils/schema_inferrer.py
--rw-r--r--   0        0        0      741 2024-05-20 14:22:43.215579 airbyte_cdk-1.0.0/airbyte_cdk/utils/spec_schema_transformations.py
--rw-r--r--   0        0        0      971 2024-05-20 14:22:43.215579 airbyte_cdk-1.0.0/airbyte_cdk/utils/stream_status_utils.py
--rw-r--r--   0        0        0     5245 2024-05-20 14:22:43.215579 airbyte_cdk-1.0.0/airbyte_cdk/utils/traced_exception.py
--rw-r--r--   0        0        0     4084 2024-05-20 14:22:43.219579 airbyte_cdk-1.0.0/pyproject.toml
--rw-r--r--   0        0        0    12797 1970-01-01 00:00:00.000000 airbyte_cdk-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1051 2024-05-21 12:14:18.401344 airbyte_cdk-1.0.1/LICENSE.txt
+-rw-r--r--   0        0        0     9977 2024-05-21 12:14:18.401344 airbyte_cdk-1.0.1/README.md
+-rw-r--r--   0        0        0     9536 2024-05-21 12:14:18.401344 airbyte_cdk-1.0.1/airbyte_cdk/__init__.py
+-rw-r--r--   0        0        0     3610 2024-05-21 12:14:18.401344 airbyte_cdk-1.0.1/airbyte_cdk/config_observation.py
+-rw-r--r--   0        0        0     4067 2024-05-21 12:14:18.401344 airbyte_cdk-1.0.1/airbyte_cdk/connector.py
+-rw-r--r--   0        0        0     1665 2024-05-21 12:14:18.401344 airbyte_cdk-1.0.1/airbyte_cdk/connector_builder/README.md
+-rw-r--r--   0        0        0       61 2024-05-21 12:14:18.401344 airbyte_cdk-1.0.1/airbyte_cdk/connector_builder/__init__.py
+-rw-r--r--   0        0        0     3958 2024-05-21 12:14:18.401344 airbyte_cdk-1.0.1/airbyte_cdk/connector_builder/connector_builder_handler.py
+-rw-r--r--   0        0        0     3365 2024-05-21 12:14:18.401344 airbyte_cdk-1.0.1/airbyte_cdk/connector_builder/main.py
+-rw-r--r--   0        0        0    17120 2024-05-21 12:14:18.401344 airbyte_cdk-1.0.1/airbyte_cdk/connector_builder/message_grouper.py
+-rw-r--r--   0        0        0     1420 2024-05-21 12:14:18.401344 airbyte_cdk-1.0.1/airbyte_cdk/connector_builder/models.py
+-rw-r--r--   0        0        0      126 2024-05-21 12:14:18.401344 airbyte_cdk-1.0.1/airbyte_cdk/destinations/__init__.py
+-rw-r--r--   0        0        0     5420 2024-05-21 12:14:18.401344 airbyte_cdk-1.0.1/airbyte_cdk/destinations/destination.py
+-rw-r--r--   0        0        0     2115 2024-05-21 12:14:18.401344 airbyte_cdk-1.0.1/airbyte_cdk/destinations/vector_db_based/README.md
+-rw-r--r--   0        0        0     1006 2024-05-21 12:14:18.401344 airbyte_cdk-1.0.1/airbyte_cdk/destinations/vector_db_based/__init__.py
+-rw-r--r--   0        0        0    12324 2024-05-21 12:14:18.401344 airbyte_cdk-1.0.1/airbyte_cdk/destinations/vector_db_based/config.py
+-rw-r--r--   0        0        0     9081 2024-05-21 12:14:18.401344 airbyte_cdk-1.0.1/airbyte_cdk/destinations/vector_db_based/document_processor.py
+-rw-r--r--   0        0        0    11443 2024-05-21 12:14:18.401344 airbyte_cdk-1.0.1/airbyte_cdk/destinations/vector_db_based/embedder.py
+-rw-r--r--   0        0        0     3243 2024-05-21 12:14:18.401344 airbyte_cdk-1.0.1/airbyte_cdk/destinations/vector_db_based/indexer.py
+-rw-r--r--   0        0        0     1807 2024-05-21 12:14:18.401344 airbyte_cdk-1.0.1/airbyte_cdk/destinations/vector_db_based/test_utils.py
+-rw-r--r--   0        0        0     1073 2024-05-21 12:14:18.401344 airbyte_cdk-1.0.1/airbyte_cdk/destinations/vector_db_based/utils.py
+-rw-r--r--   0        0        0     4394 2024-05-21 12:14:18.401344 airbyte_cdk-1.0.1/airbyte_cdk/destinations/vector_db_based/writer.py
+-rw-r--r--   0        0        0    14978 2024-05-21 12:14:18.401344 airbyte_cdk-1.0.1/airbyte_cdk/entrypoint.py
+-rw-r--r--   0        0        0     1930 2024-05-21 12:14:18.401344 airbyte_cdk-1.0.1/airbyte_cdk/exception_handler.py
+-rw-r--r--   0        0        0     3186 2024-05-21 12:14:18.401344 airbyte_cdk-1.0.1/airbyte_cdk/logger.py
+-rw-r--r--   0        0        0     1708 2024-05-21 12:14:18.401344 airbyte_cdk-1.0.1/airbyte_cdk/models/__init__.py
+-rw-r--r--   0        0        0      100 2024-05-21 12:14:18.401344 airbyte_cdk-1.0.1/airbyte_cdk/models/airbyte_protocol.py
+-rw-r--r--   0        0        0      117 2024-05-21 12:14:18.401344 airbyte_cdk-1.0.1/airbyte_cdk/models/well_known_types.py
+-rw-r--r--   0        0        0        0 2024-05-21 12:14:18.401344 airbyte_cdk-1.0.1/airbyte_cdk/py.typed
+-rw-r--r--   0        0        0     1141 2024-05-21 12:14:18.401344 airbyte_cdk-1.0.1/airbyte_cdk/sources/__init__.py
+-rw-r--r--   0        0        0    14428 2024-05-21 12:14:18.401344 airbyte_cdk-1.0.1/airbyte_cdk/sources/abstract_source.py
+-rw-r--r--   0        0        0       61 2024-05-21 12:14:18.401344 airbyte_cdk-1.0.1/airbyte_cdk/sources/concurrent_source/__init__.py
+-rw-r--r--   0        0        0    11976 2024-05-21 12:14:18.401344 airbyte_cdk-1.0.1/airbyte_cdk/sources/concurrent_source/concurrent_read_processor.py
+-rw-r--r--   0        0        0     8750 2024-05-21 12:14:18.401344 airbyte_cdk-1.0.1/airbyte_cdk/sources/concurrent_source/concurrent_source.py
+-rw-r--r--   0        0        0     3691 2024-05-21 12:14:18.401344 airbyte_cdk-1.0.1/airbyte_cdk/sources/concurrent_source/concurrent_source_adapter.py
+-rw-r--r--   0        0        0      696 2024-05-21 12:14:18.401344 airbyte_cdk-1.0.1/airbyte_cdk/sources/concurrent_source/partition_generation_completed_sentinel.py
+-rw-r--r--   0        0        0      764 2024-05-21 12:14:18.401344 airbyte_cdk-1.0.1/airbyte_cdk/sources/concurrent_source/stream_thread_exception.py
+-rw-r--r--   0        0        0     5076 2024-05-21 12:14:18.401344 airbyte_cdk-1.0.1/airbyte_cdk/sources/concurrent_source/thread_pool_manager.py
+-rw-r--r--   0        0        0      856 2024-05-21 12:14:18.401344 airbyte_cdk-1.0.1/airbyte_cdk/sources/config.py
+-rw-r--r--   0        0        0     9903 2024-05-21 12:14:18.405344 airbyte_cdk-1.0.1/airbyte_cdk/sources/connector_state_manager.py
+-rw-r--r--   0        0        0       61 2024-05-21 12:14:18.405344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/__init__.py
+-rw-r--r--   0        0        0      294 2024-05-21 12:14:18.405344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/auth/__init__.py
+-rw-r--r--   0        0        0     1090 2024-05-21 12:14:18.405344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/auth/declarative_authenticator.py
+-rw-r--r--   0        0        0     8007 2024-05-21 12:14:18.405344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/auth/jwt.py
+-rw-r--r--   0        0        0     8272 2024-05-21 12:14:18.405344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/auth/oauth.py
+-rw-r--r--   0        0        0     1347 2024-05-21 12:14:18.405344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/auth/selective_authenticator.py
+-rw-r--r--   0        0        0    11032 2024-05-21 12:14:18.405344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/auth/token.py
+-rw-r--r--   0        0        0     2887 2024-05-21 12:14:18.405344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/auth/token_provider.py
+-rw-r--r--   0        0        0      274 2024-05-21 12:14:18.405344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/checks/__init__.py
+-rw-r--r--   0        0        0     2154 2024-05-21 12:14:18.405344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/checks/check_stream.py
+-rw-r--r--   0        0        0     1368 2024-05-21 12:14:18.405344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/checks/connection_checker.py
+-rw-r--r--   0        0        0      177 2024-05-21 12:14:18.405344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/datetime/__init__.py
+-rw-r--r--   0        0        0     2369 2024-05-21 12:14:18.405344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/datetime/datetime_parser.py
+-rw-r--r--   0        0        0     5187 2024-05-21 12:14:18.405344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/datetime/min_max_datetime.py
+-rw-r--r--   0        0        0    97462 2024-05-21 12:14:18.405344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/declarative_component_schema.yaml
+-rw-r--r--   0        0        0     1517 2024-05-21 12:14:18.405344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/declarative_source.py
+-rw-r--r--   0        0        0     7495 2024-05-21 12:14:18.405344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/declarative_stream.py
+-rw-r--r--   0        0        0      247 2024-05-21 12:14:18.405344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/decoders/__init__.py
+-rw-r--r--   0        0        0      639 2024-05-21 12:14:18.405344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/decoders/decoder.py
+-rw-r--r--   0        0        0      637 2024-05-21 12:14:18.405344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/decoders/json_decoder.py
+-rw-r--r--   0        0        0      176 2024-05-21 12:14:18.405344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/exceptions.py
+-rw-r--r--   0        0        0      478 2024-05-21 12:14:18.405344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/extractors/__init__.py
+-rw-r--r--   0        0        0     2990 2024-05-21 12:14:18.405344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/extractors/dpath_extractor.py
+-rw-r--r--   0        0        0     1213 2024-05-21 12:14:18.405344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/extractors/http_selector.py
+-rw-r--r--   0        0        0      691 2024-05-21 12:14:18.405344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/extractors/record_extractor.py
+-rw-r--r--   0        0        0     1421 2024-05-21 12:14:18.405344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/extractors/record_filter.py
+-rw-r--r--   0        0        0     4671 2024-05-21 12:14:18.405344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/extractors/record_selector.py
+-rw-r--r--   0        0        0      459 2024-05-21 12:14:18.405344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/incremental/__init__.py
+-rw-r--r--   0        0        0    18380 2024-05-21 12:14:18.405344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/incremental/datetime_based_cursor.py
+-rw-r--r--   0        0        0      536 2024-05-21 12:14:18.405344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/incremental/declarative_cursor.py
+-rw-r--r--   0        0        0    12286 2024-05-21 12:14:18.405344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/incremental/per_partition_cursor.py
+-rw-r--r--   0        0        0      437 2024-05-21 12:14:18.405344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/interpolation/__init__.py
+-rw-r--r--   0        0        0     3331 2024-05-21 12:14:18.405344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/interpolation/filters.py
+-rw-r--r--   0        0        0     1844 2024-05-21 12:14:18.405344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/interpolation/interpolated_boolean.py
+-rw-r--r--   0        0        0     2018 2024-05-21 12:14:18.405344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/interpolation/interpolated_mapping.py
+-rw-r--r--   0        0        0     1791 2024-05-21 12:14:18.405344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/interpolation/interpolated_nested_mapping.py
+-rw-r--r--   0        0        0     2443 2024-05-21 12:14:18.405344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/interpolation/interpolated_string.py
+-rw-r--r--   0        0        0      934 2024-05-21 12:14:18.405344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/interpolation/interpolation.py
+-rw-r--r--   0        0        0     5367 2024-05-21 12:14:18.405344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/interpolation/jinja.py
+-rw-r--r--   0        0        0     3556 2024-05-21 12:14:18.405344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/interpolation/macros.py
+-rw-r--r--   0        0        0    12253 2024-05-21 12:14:18.405344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/manifest_declarative_source.py
+-rw-r--r--   0        0        0        0 2024-05-21 12:14:18.405344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/migrations/__init__.py
+-rw-r--r--   0        0        0     3729 2024-05-21 12:14:18.405344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/migrations/legacy_to_per_partition_state_migration.py
+-rw-r--r--   0        0        0      794 2024-05-21 12:14:18.405344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/migrations/state_migration.py
+-rw-r--r--   0        0        0       93 2024-05-21 12:14:18.405344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/models/__init__.py
+-rw-r--r--   0        0        0    65245 2024-05-21 12:14:18.405344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/models/declarative_component_schema.py
+-rw-r--r--   0        0        0       61 2024-05-21 12:14:18.405344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/parsers/__init__.py
+-rw-r--r--   0        0        0     6204 2024-05-21 12:14:18.405344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/parsers/class_types_registry.py
+-rw-r--r--   0        0        0      553 2024-05-21 12:14:18.405344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/parsers/custom_exceptions.py
+-rw-r--r--   0        0        0     3801 2024-05-21 12:14:18.405344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/parsers/default_implementation_registry.py
+-rw-r--r--   0        0        0     8287 2024-05-21 12:14:18.405344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/parsers/manifest_component_transformer.py
+-rw-r--r--   0        0        0     6728 2024-05-21 12:14:18.405344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/parsers/manifest_reference_resolver.py
+-rw-r--r--   0        0        0    63618 2024-05-21 12:14:18.405344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/parsers/model_to_component_factory.py
+-rw-r--r--   0        0        0      476 2024-05-21 12:14:18.405344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/partition_routers/__init__.py
+-rw-r--r--   0        0        0     4312 2024-05-21 12:14:18.405344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/partition_routers/list_partition_router.py
+-rw-r--r--   0        0        0     1599 2024-05-21 12:14:18.405344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/partition_routers/single_partition_router.py
+-rw-r--r--   0        0        0     7952 2024-05-21 12:14:18.405344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/partition_routers/substream_partition_router.py
+-rw-r--r--   0        0        0      364 2024-05-21 12:14:18.405344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/requesters/__init__.py
+-rw-r--r--   0        0        0      717 2024-05-21 12:14:18.409344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/requesters/error_handlers/__init__.py
+-rw-r--r--   0        0        0      875 2024-05-21 12:14:18.409344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/requesters/error_handlers/backoff_strategies/__init__.py
+-rw-r--r--   0        0        0     1571 2024-05-21 12:14:18.409344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/requesters/error_handlers/backoff_strategies/constant_backoff_strategy.py
+-rw-r--r--   0        0        0     1366 2024-05-21 12:14:18.409344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/requesters/error_handlers/backoff_strategies/exponential_backoff_strategy.py
+-rw-r--r--   0        0        0     1156 2024-05-21 12:14:18.409344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/requesters/error_handlers/backoff_strategies/header_helper.py
+-rw-r--r--   0        0        0     1816 2024-05-21 12:14:18.409344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/requesters/error_handlers/backoff_strategies/wait_time_from_header_backoff_strategy.py
+-rw-r--r--   0        0        0     2803 2024-05-21 12:14:18.409344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/requesters/error_handlers/backoff_strategies/wait_until_time_from_header_backoff_strategy.py
+-rw-r--r--   0        0        0      697 2024-05-21 12:14:18.409344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/requesters/error_handlers/backoff_strategy.py
+-rw-r--r--   0        0        0     2476 2024-05-21 12:14:18.409344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/requesters/error_handlers/composite_error_handler.py
+-rw-r--r--   0        0        0     6041 2024-05-21 12:14:18.409344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/requesters/error_handlers/default_error_handler.py
+-rw-r--r--   0        0        0     1141 2024-05-21 12:14:18.409344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/requesters/error_handlers/error_handler.py
+-rw-r--r--   0        0        0     4979 2024-05-21 12:14:18.409344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/requesters/error_handlers/http_response_filter.py
+-rw-r--r--   0        0        0      405 2024-05-21 12:14:18.409344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/requesters/error_handlers/response_action.py
+-rw-r--r--   0        0        0     2656 2024-05-21 12:14:18.409344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/requesters/error_handlers/response_status.py
+-rw-r--r--   0        0        0    27968 2024-05-21 12:14:18.409344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/requesters/http_requester.py
+-rw-r--r--   0        0        0      599 2024-05-21 12:14:18.409344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/requesters/paginators/__init__.py
+-rw-r--r--   0        0        0    10305 2024-05-21 12:14:18.409344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/requesters/paginators/default_paginator.py
+-rw-r--r--   0        0        0     1877 2024-05-21 12:14:18.409344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/requesters/paginators/no_pagination.py
+-rw-r--r--   0        0        0     1927 2024-05-21 12:14:18.409344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/requesters/paginators/paginator.py
+-rw-r--r--   0        0        0      740 2024-05-21 12:14:18.409344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/requesters/paginators/strategies/__init__.py
+-rw-r--r--   0        0        0     3445 2024-05-21 12:14:18.409344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/requesters/paginators/strategies/cursor_pagination_strategy.py
+-rw-r--r--   0        0        0     2887 2024-05-21 12:14:18.409344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/requesters/paginators/strategies/offset_increment.py
+-rw-r--r--   0        0        0     2152 2024-05-21 12:14:18.409344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/requesters/paginators/strategies/page_increment.py
+-rw-r--r--   0        0        0     1240 2024-05-21 12:14:18.409344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/requesters/paginators/strategies/pagination_strategy.py
+-rw-r--r--   0        0        0     1967 2024-05-21 12:14:18.409344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/requesters/paginators/strategies/stop_condition.py
+-rw-r--r--   0        0        0     1055 2024-05-21 12:14:18.409344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/requesters/request_option.py
+-rw-r--r--   0        0        0      410 2024-05-21 12:14:18.409344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/requesters/request_options/__init__.py
+-rw-r--r--   0        0        0     2275 2024-05-21 12:14:18.409344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/requesters/request_options/interpolated_nested_request_input_provider.py
+-rw-r--r--   0        0        0     2883 2024-05-21 12:14:18.409344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/requesters/request_options/interpolated_request_input_provider.py
+-rw-r--r--   0        0        0     4995 2024-05-21 12:14:18.409344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/requesters/request_options/interpolated_request_options_provider.py
+-rw-r--r--   0        0        0     2590 2024-05-21 12:14:18.409344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/requesters/request_options/request_options_provider.py
+-rw-r--r--   0        0        0      299 2024-05-21 12:14:18.409344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/requesters/request_path.py
+-rw-r--r--   0        0        0     5539 2024-05-21 12:14:18.409344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/requesters/requester.py
+-rw-r--r--   0        0        0      339 2024-05-21 12:14:18.409344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/retrievers/__init__.py
+-rw-r--r--   0        0        0     1741 2024-05-21 12:14:18.409344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/retrievers/retriever.py
+-rw-r--r--   0        0        0    19727 2024-05-21 12:14:18.409344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/retrievers/simple_retriever.py
+-rw-r--r--   0        0        0      517 2024-05-21 12:14:18.409344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/schema/__init__.py
+-rw-r--r--   0        0        0     1790 2024-05-21 12:14:18.409344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/schema/default_schema_loader.py
+-rw-r--r--   0        0        0      464 2024-05-21 12:14:18.409344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/schema/inline_schema_loader.py
+-rw-r--r--   0        0        0     4150 2024-05-21 12:14:18.409344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/schema/json_file_schema_loader.py
+-rw-r--r--   0        0        0      379 2024-05-21 12:14:18.409344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/schema/schema_loader.py
+-rw-r--r--   0        0        0      141 2024-05-21 12:14:18.409344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/spec/__init__.py
+-rw-r--r--   0        0        0     1786 2024-05-21 12:14:18.409344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/spec/spec.py
+-rw-r--r--   0        0        0      328 2024-05-21 12:14:18.409344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/stream_slicers/__init__.py
+-rw-r--r--   0        0        0     4721 2024-05-21 12:14:18.409344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/stream_slicers/cartesian_product_stream_slicer.py
+-rw-r--r--   0        0        0      856 2024-05-21 12:14:18.409344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/stream_slicers/stream_slicer.py
+-rw-r--r--   0        0        0      919 2024-05-21 12:14:18.409344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/transformations/__init__.py
+-rw-r--r--   0        0        0     4884 2024-05-21 12:14:18.409344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/transformations/add_fields.py
+-rw-r--r--   0        0        0     2725 2024-05-21 12:14:18.409344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/transformations/remove_fields.py
+-rw-r--r--   0        0        0     1123 2024-05-21 12:14:18.409344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/transformations/transformation.py
+-rw-r--r--   0        0        0      749 2024-05-21 12:14:18.409344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/types.py
+-rw-r--r--   0        0        0     1879 2024-05-21 12:14:18.409344 airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/yaml_declarative_source.py
+-rw-r--r--   0        0        0       61 2024-05-21 12:14:18.409344 airbyte_cdk-1.0.1/airbyte_cdk/sources/embedded/__init__.py
+-rw-r--r--   0        0        0     2264 2024-05-21 12:14:18.409344 airbyte_cdk-1.0.1/airbyte_cdk/sources/embedded/base_integration.py
+-rw-r--r--   0        0        0     1571 2024-05-21 12:14:18.409344 airbyte_cdk-1.0.1/airbyte_cdk/sources/embedded/catalog.py
+-rw-r--r--   0        0        0     1390 2024-05-21 12:14:18.409344 airbyte_cdk-1.0.1/airbyte_cdk/sources/embedded/runner.py
+-rw-r--r--   0        0        0      744 2024-05-21 12:14:18.409344 airbyte_cdk-1.0.1/airbyte_cdk/sources/embedded/tools.py
+-rw-r--r--   0        0        0    11085 2024-05-21 12:14:18.409344 airbyte_cdk-1.0.1/airbyte_cdk/sources/file_based/README.md
+-rw-r--r--   0        0        0      868 2024-05-21 12:14:18.409344 airbyte_cdk-1.0.1/airbyte_cdk/sources/file_based/__init__.py
+-rw-r--r--   0        0        0      371 2024-05-21 12:14:18.409344 airbyte_cdk-1.0.1/airbyte_cdk/sources/file_based/availability_strategy/__init__.py
+-rw-r--r--   0        0        0     2137 2024-05-21 12:14:18.409344 airbyte_cdk-1.0.1/airbyte_cdk/sources/file_based/availability_strategy/abstract_file_based_availability_strategy.py
+-rw-r--r--   0        0        0     5289 2024-05-21 12:14:18.409344 airbyte_cdk-1.0.1/airbyte_cdk/sources/file_based/availability_strategy/default_file_based_availability_strategy.py
+-rw-r--r--   0        0        0        0 2024-05-21 12:14:18.409344 airbyte_cdk-1.0.1/airbyte_cdk/sources/file_based/config/__init__.py
+-rw-r--r--   0        0        0     4956 2024-05-21 12:14:18.409344 airbyte_cdk-1.0.1/airbyte_cdk/sources/file_based/config/abstract_file_based_spec.py
+-rw-r--r--   0        0        0      712 2024-05-21 12:14:18.409344 airbyte_cdk-1.0.1/airbyte_cdk/sources/file_based/config/avro_format.py
+-rw-r--r--   0        0        0     7804 2024-05-21 12:14:18.409344 airbyte_cdk-1.0.1/airbyte_cdk/sources/file_based/config/csv_format.py
+-rw-r--r--   0        0        0     4229 2024-05-21 12:14:18.409344 airbyte_cdk-1.0.1/airbyte_cdk/sources/file_based/config/file_based_stream_config.py
+-rw-r--r--   0        0        0      374 2024-05-21 12:14:18.409344 airbyte_cdk-1.0.1/airbyte_cdk/sources/file_based/config/jsonl_format.py
+-rw-r--r--   0        0        0      737 2024-05-21 12:14:18.409344 airbyte_cdk-1.0.1/airbyte_cdk/sources/file_based/config/parquet_format.py
+-rw-r--r--   0        0        0     3513 2024-05-21 12:14:18.409344 airbyte_cdk-1.0.1/airbyte_cdk/sources/file_based/config/unstructured_format.py
+-rw-r--r--   0        0        0      283 2024-05-21 12:14:18.409344 airbyte_cdk-1.0.1/airbyte_cdk/sources/file_based/discovery_policy/__init__.py
+-rw-r--r--   0        0        0      621 2024-05-21 12:14:18.409344 airbyte_cdk-1.0.1/airbyte_cdk/sources/file_based/discovery_policy/abstract_discovery_policy.py
+-rw-r--r--   0        0        0      939 2024-05-21 12:14:18.409344 airbyte_cdk-1.0.1/airbyte_cdk/sources/file_based/discovery_policy/default_discovery_policy.py
+-rw-r--r--   0        0        0     5613 2024-05-21 12:14:18.413344 airbyte_cdk-1.0.1/airbyte_cdk/sources/file_based/exceptions.py
+-rw-r--r--   0        0        0    13784 2024-05-21 12:14:18.413344 airbyte_cdk-1.0.1/airbyte_cdk/sources/file_based/file_based_source.py
+-rw-r--r--   0        0        0     3749 2024-05-21 12:14:18.413344 airbyte_cdk-1.0.1/airbyte_cdk/sources/file_based/file_based_stream_reader.py
+-rw-r--r--   0        0        0     1017 2024-05-21 12:14:18.413344 airbyte_cdk-1.0.1/airbyte_cdk/sources/file_based/file_types/__init__.py
+-rw-r--r--   0        0        0     9167 2024-05-21 12:14:18.413344 airbyte_cdk-1.0.1/airbyte_cdk/sources/file_based/file_types/avro_parser.py
+-rw-r--r--   0        0        0    19461 2024-05-21 12:14:18.413344 airbyte_cdk-1.0.1/airbyte_cdk/sources/file_based/file_types/csv_parser.py
+-rw-r--r--   0        0        0     2819 2024-05-21 12:14:18.413344 airbyte_cdk-1.0.1/airbyte_cdk/sources/file_based/file_types/file_type_parser.py
+-rw-r--r--   0        0        0     5666 2024-05-21 12:14:18.413344 airbyte_cdk-1.0.1/airbyte_cdk/sources/file_based/file_types/jsonl_parser.py
+-rw-r--r--   0        0        0     9998 2024-05-21 12:14:18.413344 airbyte_cdk-1.0.1/airbyte_cdk/sources/file_based/file_types/parquet_parser.py
+-rw-r--r--   0        0        0    16736 2024-05-21 12:14:18.413344 airbyte_cdk-1.0.1/airbyte_cdk/sources/file_based/file_types/unstructured_parser.py
+-rw-r--r--   0        0        0      312 2024-05-21 12:14:18.413344 airbyte_cdk-1.0.1/airbyte_cdk/sources/file_based/remote_file.py
+-rw-r--r--   0        0        0     9291 2024-05-21 12:14:18.413344 airbyte_cdk-1.0.1/airbyte_cdk/sources/file_based/schema_helpers.py
+-rw-r--r--   0        0        0      527 2024-05-21 12:14:18.413344 airbyte_cdk-1.0.1/airbyte_cdk/sources/file_based/schema_validation_policies/__init__.py
+-rw-r--r--   0        0        0      604 2024-05-21 12:14:18.413344 airbyte_cdk-1.0.1/airbyte_cdk/sources/file_based/schema_validation_policies/abstract_schema_validation_policy.py
+-rw-r--r--   0        0        0     1643 2024-05-21 12:14:18.413344 airbyte_cdk-1.0.1/airbyte_cdk/sources/file_based/schema_validation_policies/default_schema_validation_policies.py
+-rw-r--r--   0        0        0      265 2024-05-21 12:14:18.413344 airbyte_cdk-1.0.1/airbyte_cdk/sources/file_based/stream/__init__.py
+-rw-r--r--   0        0        0     6557 2024-05-21 12:14:18.413344 airbyte_cdk-1.0.1/airbyte_cdk/sources/file_based/stream/abstract_file_based_stream.py
+-rw-r--r--   0        0        0        0 2024-05-21 12:14:18.413344 airbyte_cdk-1.0.1/airbyte_cdk/sources/file_based/stream/concurrent/__init__.py
+-rw-r--r--   0        0        0    12818 2024-05-21 12:14:18.413344 airbyte_cdk-1.0.1/airbyte_cdk/sources/file_based/stream/concurrent/adapters.py
+-rw-r--r--   0        0        0      329 2024-05-21 12:14:18.413344 airbyte_cdk-1.0.1/airbyte_cdk/sources/file_based/stream/concurrent/cursor/__init__.py
+-rw-r--r--   0        0        0     1961 2024-05-21 12:14:18.413344 airbyte_cdk-1.0.1/airbyte_cdk/sources/file_based/stream/concurrent/cursor/abstract_concurrent_file_based_cursor.py
+-rw-r--r--   0        0        0    14331 2024-05-21 12:14:18.413344 airbyte_cdk-1.0.1/airbyte_cdk/sources/file_based/stream/concurrent/cursor/file_based_concurrent_cursor.py
+-rw-r--r--   0        0        0     3150 2024-05-21 12:14:18.413344 airbyte_cdk-1.0.1/airbyte_cdk/sources/file_based/stream/concurrent/cursor/file_based_final_state_cursor.py
+-rw-r--r--   0        0        0      191 2024-05-21 12:14:18.413344 airbyte_cdk-1.0.1/airbyte_cdk/sources/file_based/stream/cursor/__init__.py
+-rw-r--r--   0        0        0     1920 2024-05-21 12:14:18.413344 airbyte_cdk-1.0.1/airbyte_cdk/sources/file_based/stream/cursor/abstract_file_based_cursor.py
+-rw-r--r--   0        0        0     6815 2024-05-21 12:14:18.413344 airbyte_cdk-1.0.1/airbyte_cdk/sources/file_based/stream/cursor/default_file_based_cursor.py
+-rw-r--r--   0        0        0    13143 2024-05-21 12:14:18.413344 airbyte_cdk-1.0.1/airbyte_cdk/sources/file_based/stream/default_file_based_stream.py
+-rw-r--r--   0        0        0      218 2024-05-21 12:14:18.413344 airbyte_cdk-1.0.1/airbyte_cdk/sources/file_based/types.py
+-rw-r--r--   0        0        0      730 2024-05-21 12:14:18.413344 airbyte_cdk-1.0.1/airbyte_cdk/sources/http_config.py
+-rw-r--r--   0        0        0     1437 2024-05-21 12:14:18.413344 airbyte_cdk-1.0.1/airbyte_cdk/sources/http_logger.py
+-rw-r--r--   0        0        0      372 2024-05-21 12:14:18.413344 airbyte_cdk-1.0.1/airbyte_cdk/sources/message/__init__.py
+-rw-r--r--   0        0        0     4583 2024-05-21 12:14:18.413344 airbyte_cdk-1.0.1/airbyte_cdk/sources/message/repository.py
+-rw-r--r--   0        0        0     4412 2024-05-21 12:14:18.413344 airbyte_cdk-1.0.1/airbyte_cdk/sources/source.py
+-rw-r--r--   0        0        0      256 2024-05-21 12:14:18.413344 airbyte_cdk-1.0.1/airbyte_cdk/sources/streams/__init__.py
+-rw-r--r--   0        0        0     1007 2024-05-21 12:14:18.413344 airbyte_cdk-1.0.1/airbyte_cdk/sources/streams/availability_strategy.py
+-rw-r--r--   0        0        0    20555 2024-05-21 12:14:18.413344 airbyte_cdk-1.0.1/airbyte_cdk/sources/streams/call_rate.py
+-rw-r--r--   0        0        0      408 2024-05-21 12:14:18.413344 airbyte_cdk-1.0.1/airbyte_cdk/sources/streams/checkpoint/__init__.py
+-rw-r--r--   0        0        0     4893 2024-05-21 12:14:18.413344 airbyte_cdk-1.0.1/airbyte_cdk/sources/streams/checkpoint/checkpoint_reader.py
+-rw-r--r--   0        0        0     2946 2024-05-21 12:14:18.413344 airbyte_cdk-1.0.1/airbyte_cdk/sources/streams/checkpoint/cursor.py
+-rw-r--r--   0        0        0     1070 2024-05-21 12:14:18.413344 airbyte_cdk-1.0.1/airbyte_cdk/sources/streams/concurrent/README.md
+-rw-r--r--   0        0        0       61 2024-05-21 12:14:18.413344 airbyte_cdk-1.0.1/airbyte_cdk/sources/streams/concurrent/__init__.py
+-rw-r--r--   0        0        0     3792 2024-05-21 12:14:18.413344 airbyte_cdk-1.0.1/airbyte_cdk/sources/streams/concurrent/abstract_stream.py
+-rw-r--r--   0        0        0     1358 2024-05-21 12:14:18.413344 airbyte_cdk-1.0.1/airbyte_cdk/sources/streams/concurrent/abstract_stream_facade.py
+-rw-r--r--   0        0        0    16279 2024-05-21 12:14:18.413344 airbyte_cdk-1.0.1/airbyte_cdk/sources/streams/concurrent/adapters.py
+-rw-r--r--   0        0        0     2013 2024-05-21 12:14:18.413344 airbyte_cdk-1.0.1/airbyte_cdk/sources/streams/concurrent/availability_strategy.py
+-rw-r--r--   0        0        0    15155 2024-05-21 12:14:18.413344 airbyte_cdk-1.0.1/airbyte_cdk/sources/streams/concurrent/cursor.py
+-rw-r--r--   0        0        0     3059 2024-05-21 12:14:18.413344 airbyte_cdk-1.0.1/airbyte_cdk/sources/streams/concurrent/default_stream.py
+-rw-r--r--   0        0        0      468 2024-05-21 12:14:18.413344 airbyte_cdk-1.0.1/airbyte_cdk/sources/streams/concurrent/exceptions.py
+-rw-r--r--   0        0        0     1290 2024-05-21 12:14:18.413344 airbyte_cdk-1.0.1/airbyte_cdk/sources/streams/concurrent/helpers.py
+-rw-r--r--   0        0        0     3315 2024-05-21 12:14:18.413344 airbyte_cdk-1.0.1/airbyte_cdk/sources/streams/concurrent/partition_enqueuer.py
+-rw-r--r--   0        0        0     1747 2024-05-21 12:14:18.413344 airbyte_cdk-1.0.1/airbyte_cdk/sources/streams/concurrent/partition_reader.py
+-rw-r--r--   0        0        0       61 2024-05-21 12:14:18.413344 airbyte_cdk-1.0.1/airbyte_cdk/sources/streams/concurrent/partitions/__init__.py
+-rw-r--r--   0        0        0     1795 2024-05-21 12:14:18.413344 airbyte_cdk-1.0.1/airbyte_cdk/sources/streams/concurrent/partitions/partition.py
+-rw-r--r--   0        0        0      441 2024-05-21 12:14:18.413344 airbyte_cdk-1.0.1/airbyte_cdk/sources/streams/concurrent/partitions/partition_generator.py
+-rw-r--r--   0        0        0      600 2024-05-21 12:14:18.413344 airbyte_cdk-1.0.1/airbyte_cdk/sources/streams/concurrent/partitions/record.py
+-rw-r--r--   0        0        0     1182 2024-05-21 12:14:18.413344 airbyte_cdk-1.0.1/airbyte_cdk/sources/streams/concurrent/partitions/types.py
+-rw-r--r--   0        0        0        0 2024-05-21 12:14:18.413344 airbyte_cdk-1.0.1/airbyte_cdk/sources/streams/concurrent/state_converters/__init__.py
+-rw-r--r--   0        0        0     5539 2024-05-21 12:14:18.413344 airbyte_cdk-1.0.1/airbyte_cdk/sources/streams/concurrent/state_converters/abstract_stream_state_converter.py
+-rw-r--r--   0        0        0     5504 2024-05-21 12:14:18.413344 airbyte_cdk-1.0.1/airbyte_cdk/sources/streams/concurrent/state_converters/datetime_stream_state_converter.py
+-rw-r--r--   0        0        0    22387 2024-05-21 12:14:18.413344 airbyte_cdk-1.0.1/airbyte_cdk/sources/streams/core.py
+-rw-r--r--   0        0        0      311 2024-05-21 12:14:18.413344 airbyte_cdk-1.0.1/airbyte_cdk/sources/streams/http/__init__.py
+-rw-r--r--   0        0        0     6884 2024-05-21 12:14:18.413344 airbyte_cdk-1.0.1/airbyte_cdk/sources/streams/http/availability_strategy.py
+-rw-r--r--   0        0        0      665 2024-05-21 12:14:18.413344 airbyte_cdk-1.0.1/airbyte_cdk/sources/streams/http/error_handlers/__init__.py
+-rw-r--r--   0        0        0      826 2024-05-21 12:14:18.413344 airbyte_cdk-1.0.1/airbyte_cdk/sources/streams/http/error_handlers/backoff_strategy.py
+-rw-r--r--   0        0        0      991 2024-05-21 12:14:18.413344 airbyte_cdk-1.0.1/airbyte_cdk/sources/streams/http/error_handlers/default_backoff_strategy.py
+-rw-r--r--   0        0        0      781 2024-05-21 12:14:18.413344 airbyte_cdk-1.0.1/airbyte_cdk/sources/streams/http/error_handlers/error_handler.py
+-rw-r--r--   0        0        0      456 2024-05-21 12:14:18.413344 airbyte_cdk-1.0.1/airbyte_cdk/sources/streams/http/error_handlers/error_message_parser.py
+-rw-r--r--   0        0        0     6172 2024-05-21 12:14:18.413344 airbyte_cdk-1.0.1/airbyte_cdk/sources/streams/http/error_handlers/http_status_error_handler.py
+-rw-r--r--   0        0        0     1491 2024-05-21 12:14:18.413344 airbyte_cdk-1.0.1/airbyte_cdk/sources/streams/http/error_handlers/json_error_message_parser.py
+-rw-r--r--   0        0        0      476 2024-05-21 12:14:18.413344 airbyte_cdk-1.0.1/airbyte_cdk/sources/streams/http/error_handlers/response_models.py
+-rw-r--r--   0        0        0     1743 2024-05-21 12:14:18.413344 airbyte_cdk-1.0.1/airbyte_cdk/sources/streams/http/exceptions.py
+-rw-r--r--   0        0        0    24016 2024-05-21 12:14:18.417344 airbyte_cdk-1.0.1/airbyte_cdk/sources/streams/http/http.py
+-rw-r--r--   0        0        0    11292 2024-05-21 12:14:18.417344 airbyte_cdk-1.0.1/airbyte_cdk/sources/streams/http/http_client.py
+-rw-r--r--   0        0        0     5258 2024-05-21 12:14:18.417344 airbyte_cdk-1.0.1/airbyte_cdk/sources/streams/http/rate_limiting.py
+-rw-r--r--   0        0        0      413 2024-05-21 12:14:18.417344 airbyte_cdk-1.0.1/airbyte_cdk/sources/streams/http/requests_native_auth/__init__.py
+-rw-r--r--   0        0        0    10125 2024-05-21 12:14:18.417344 airbyte_cdk-1.0.1/airbyte_cdk/sources/streams/http/requests_native_auth/abstract_oauth.py
+-rw-r--r--   0        0        0      961 2024-05-21 12:14:18.417344 airbyte_cdk-1.0.1/airbyte_cdk/sources/streams/http/requests_native_auth/abstract_token.py
+-rw-r--r--   0        0        0    13381 2024-05-21 12:14:18.417344 airbyte_cdk-1.0.1/airbyte_cdk/sources/streams/http/requests_native_auth/oauth.py
+-rw-r--r--   0        0        0     2456 2024-05-21 12:14:18.417344 airbyte_cdk-1.0.1/airbyte_cdk/sources/streams/http/requests_native_auth/token.py
+-rw-r--r--   0        0        0       61 2024-05-21 12:14:18.417344 airbyte_cdk-1.0.1/airbyte_cdk/sources/streams/utils/__init__.py
+-rw-r--r--   0        0        0     1645 2024-05-21 12:14:18.417344 airbyte_cdk-1.0.1/airbyte_cdk/sources/streams/utils/stream_helper.py
+-rw-r--r--   0        0        0     3588 2024-05-21 12:14:18.417344 airbyte_cdk-1.0.1/airbyte_cdk/sources/types.py
+-rw-r--r--   0        0        0      118 2024-05-21 12:14:18.417344 airbyte_cdk-1.0.1/airbyte_cdk/sources/utils/__init__.py
+-rw-r--r--   0        0        0      256 2024-05-21 12:14:18.417344 airbyte_cdk-1.0.1/airbyte_cdk/sources/utils/casing.py
+-rw-r--r--   0        0        0      714 2024-05-21 12:14:18.417344 airbyte_cdk-1.0.1/airbyte_cdk/sources/utils/catalog_helpers.py
+-rw-r--r--   0        0        0     1711 2024-05-21 12:14:18.417344 airbyte_cdk-1.0.1/airbyte_cdk/sources/utils/record_helper.py
+-rw-r--r--   0        0        0     8483 2024-05-21 12:14:18.417344 airbyte_cdk-1.0.1/airbyte_cdk/sources/utils/schema_helpers.py
+-rw-r--r--   0        0        0     3151 2024-05-21 12:14:18.417344 airbyte_cdk-1.0.1/airbyte_cdk/sources/utils/schema_models.py
+-rw-r--r--   0        0        0     1731 2024-05-21 12:14:18.417344 airbyte_cdk-1.0.1/airbyte_cdk/sources/utils/slice_logger.py
+-rw-r--r--   0        0        0     9493 2024-05-21 12:14:18.417344 airbyte_cdk-1.0.1/airbyte_cdk/sources/utils/transform.py
+-rw-r--r--   0        0        0      175 2024-05-21 12:14:18.417344 airbyte_cdk-1.0.1/airbyte_cdk/sources/utils/types.py
+-rw-r--r--   0        0        0      199 2024-05-21 12:14:18.417344 airbyte_cdk-1.0.1/airbyte_cdk/test/__init__.py
+-rw-r--r--   0        0        0     2691 2024-05-21 12:14:18.417344 airbyte_cdk-1.0.1/airbyte_cdk/test/catalog_builder.py
+-rw-r--r--   0        0        0     7399 2024-05-21 12:14:18.417344 airbyte_cdk-1.0.1/airbyte_cdk/test/entrypoint_wrapper.py
+-rw-r--r--   0        0        0      322 2024-05-21 12:14:18.417344 airbyte_cdk-1.0.1/airbyte_cdk/test/mock_http/__init__.py
+-rw-r--r--   0        0        0     1240 2024-05-21 12:14:18.417344 airbyte_cdk-1.0.1/airbyte_cdk/test/mock_http/matcher.py
+-rw-r--r--   0        0        0     6412 2024-05-21 12:14:18.417344 airbyte_cdk-1.0.1/airbyte_cdk/test/mock_http/mocker.py
+-rw-r--r--   0        0        0     3687 2024-05-21 12:14:18.417344 airbyte_cdk-1.0.1/airbyte_cdk/test/mock_http/request.py
+-rw-r--r--   0        0        0      588 2024-05-21 12:14:18.417344 airbyte_cdk-1.0.1/airbyte_cdk/test/mock_http/response.py
+-rw-r--r--   0        0        0     7789 2024-05-21 12:14:18.417344 airbyte_cdk-1.0.1/airbyte_cdk/test/mock_http/response_builder.py
+-rw-r--r--   0        0        0      609 2024-05-21 12:14:18.417344 airbyte_cdk-1.0.1/airbyte_cdk/test/state_builder.py
+-rw-r--r--   0        0        0      294 2024-05-21 12:14:18.417344 airbyte_cdk-1.0.1/airbyte_cdk/utils/__init__.py
+-rw-r--r--   0        0        0     3079 2024-05-21 12:14:18.417344 airbyte_cdk-1.0.1/airbyte_cdk/utils/airbyte_secrets_utils.py
+-rw-r--r--   0        0        0      598 2024-05-21 12:14:18.417344 airbyte_cdk-1.0.1/airbyte_cdk/utils/analytics_message.py
+-rw-r--r--   0        0        0      108 2024-05-21 12:14:18.417344 airbyte_cdk-1.0.1/airbyte_cdk/utils/constants.py
+-rw-r--r--   0        0        0     3954 2024-05-21 12:14:18.417344 airbyte_cdk-1.0.1/airbyte_cdk/utils/datetime_format_inferrer.py
+-rw-r--r--   0        0        0     2377 2024-05-21 12:14:18.417344 airbyte_cdk-1.0.1/airbyte_cdk/utils/event_timing.py
+-rw-r--r--   0        0        0      574 2024-05-21 12:14:18.417344 airbyte_cdk-1.0.1/airbyte_cdk/utils/is_cloud_environment.py
+-rw-r--r--   0        0        0     1729 2024-05-21 12:14:18.417344 airbyte_cdk-1.0.1/airbyte_cdk/utils/mapping_helpers.py
+-rw-r--r--   0        0        0      953 2024-05-21 12:14:18.417344 airbyte_cdk-1.0.1/airbyte_cdk/utils/message_utils.py
+-rw-r--r--   0        0        0     1180 2024-05-21 12:14:18.417344 airbyte_cdk-1.0.1/airbyte_cdk/utils/oneof_option_config.py
+-rw-r--r--   0        0        0     8622 2024-05-21 12:14:18.417344 airbyte_cdk-1.0.1/airbyte_cdk/utils/schema_inferrer.py
+-rw-r--r--   0        0        0      741 2024-05-21 12:14:18.417344 airbyte_cdk-1.0.1/airbyte_cdk/utils/spec_schema_transformations.py
+-rw-r--r--   0        0        0      971 2024-05-21 12:14:18.417344 airbyte_cdk-1.0.1/airbyte_cdk/utils/stream_status_utils.py
+-rw-r--r--   0        0        0     5245 2024-05-21 12:14:18.417344 airbyte_cdk-1.0.1/airbyte_cdk/utils/traced_exception.py
+-rw-r--r--   0        0        0     4084 2024-05-21 12:14:18.421344 airbyte_cdk-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0    12797 1970-01-01 00:00:00.000000 airbyte_cdk-1.0.1/PKG-INFO
```

### Comparing `airbyte_cdk-1.0.0/LICENSE.txt` & `airbyte_cdk-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/README.md` & `airbyte_cdk-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/__init__.py` & `airbyte_cdk-1.0.1/airbyte_cdk/__init__.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/config_observation.py` & `airbyte_cdk-1.0.1/airbyte_cdk/config_observation.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/connector.py` & `airbyte_cdk-1.0.1/airbyte_cdk/connector.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/connector_builder/README.md` & `airbyte_cdk-1.0.1/airbyte_cdk/connector_builder/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/connector_builder/connector_builder_handler.py` & `airbyte_cdk-1.0.1/airbyte_cdk/connector_builder/connector_builder_handler.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/connector_builder/main.py` & `airbyte_cdk-1.0.1/airbyte_cdk/connector_builder/main.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/connector_builder/message_grouper.py` & `airbyte_cdk-1.0.1/airbyte_cdk/connector_builder/message_grouper.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/connector_builder/models.py` & `airbyte_cdk-1.0.1/airbyte_cdk/connector_builder/models.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/destinations/destination.py` & `airbyte_cdk-1.0.1/airbyte_cdk/destinations/destination.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/destinations/vector_db_based/README.md` & `airbyte_cdk-1.0.1/airbyte_cdk/destinations/vector_db_based/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/destinations/vector_db_based/__init__.py` & `airbyte_cdk-1.0.1/airbyte_cdk/destinations/vector_db_based/__init__.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/destinations/vector_db_based/config.py` & `airbyte_cdk-1.0.1/airbyte_cdk/destinations/vector_db_based/config.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/destinations/vector_db_based/document_processor.py` & `airbyte_cdk-1.0.1/airbyte_cdk/destinations/vector_db_based/document_processor.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/destinations/vector_db_based/embedder.py` & `airbyte_cdk-1.0.1/airbyte_cdk/destinations/vector_db_based/embedder.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/destinations/vector_db_based/indexer.py` & `airbyte_cdk-1.0.1/airbyte_cdk/destinations/vector_db_based/indexer.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/destinations/vector_db_based/test_utils.py` & `airbyte_cdk-1.0.1/airbyte_cdk/destinations/vector_db_based/test_utils.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/destinations/vector_db_based/utils.py` & `airbyte_cdk-1.0.1/airbyte_cdk/destinations/vector_db_based/utils.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/destinations/vector_db_based/writer.py` & `airbyte_cdk-1.0.1/airbyte_cdk/destinations/vector_db_based/writer.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/entrypoint.py` & `airbyte_cdk-1.0.1/airbyte_cdk/entrypoint.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/exception_handler.py` & `airbyte_cdk-1.0.1/airbyte_cdk/exception_handler.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/logger.py` & `airbyte_cdk-1.0.1/airbyte_cdk/logger.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/models/__init__.py` & `airbyte_cdk-1.0.1/airbyte_cdk/models/__init__.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/__init__.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/__init__.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/abstract_source.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/abstract_source.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/concurrent_source/concurrent_read_processor.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/concurrent_source/concurrent_read_processor.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/concurrent_source/concurrent_source.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/concurrent_source/concurrent_source.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/concurrent_source/concurrent_source_adapter.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/concurrent_source/concurrent_source_adapter.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/concurrent_source/partition_generation_completed_sentinel.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/concurrent_source/partition_generation_completed_sentinel.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/concurrent_source/stream_thread_exception.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/concurrent_source/stream_thread_exception.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/concurrent_source/thread_pool_manager.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/concurrent_source/thread_pool_manager.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/config.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/config.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/connector_state_manager.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/connector_state_manager.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/auth/declarative_authenticator.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/auth/declarative_authenticator.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/auth/jwt.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/auth/jwt.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/auth/oauth.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/auth/oauth.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/auth/selective_authenticator.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/auth/selective_authenticator.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/auth/token.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/auth/token.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/auth/token_provider.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/auth/token_provider.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/checks/check_stream.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/checks/check_stream.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/checks/connection_checker.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/checks/connection_checker.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/datetime/datetime_parser.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/datetime/datetime_parser.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/datetime/min_max_datetime.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/datetime/min_max_datetime.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/declarative_component_schema.yaml` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/declarative_component_schema.yaml`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/declarative_source.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/declarative_source.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/declarative_stream.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/declarative_stream.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/decoders/decoder.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/decoders/decoder.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/decoders/json_decoder.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/decoders/json_decoder.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/extractors/dpath_extractor.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/extractors/dpath_extractor.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/extractors/http_selector.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/extractors/http_selector.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/extractors/record_extractor.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/extractors/record_extractor.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/extractors/record_filter.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/extractors/record_filter.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/extractors/record_selector.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/extractors/record_selector.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/incremental/datetime_based_cursor.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/incremental/datetime_based_cursor.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/incremental/declarative_cursor.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/incremental/declarative_cursor.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/incremental/per_partition_cursor.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/incremental/per_partition_cursor.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/interpolation/filters.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/interpolation/filters.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/interpolation/interpolated_boolean.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/interpolation/interpolated_boolean.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/interpolation/interpolated_mapping.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/interpolation/interpolated_mapping.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/interpolation/interpolated_nested_mapping.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/interpolation/interpolated_nested_mapping.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/interpolation/interpolated_string.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/interpolation/interpolated_string.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/interpolation/interpolation.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/interpolation/interpolation.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/interpolation/jinja.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/interpolation/jinja.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/interpolation/macros.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/interpolation/macros.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/manifest_declarative_source.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/manifest_declarative_source.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/migrations/legacy_to_per_partition_state_migration.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/migrations/legacy_to_per_partition_state_migration.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/migrations/state_migration.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/migrations/state_migration.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/models/declarative_component_schema.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/models/declarative_component_schema.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/parsers/class_types_registry.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/parsers/class_types_registry.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/parsers/custom_exceptions.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/parsers/custom_exceptions.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/parsers/default_implementation_registry.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/parsers/default_implementation_registry.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/parsers/manifest_component_transformer.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/parsers/manifest_component_transformer.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/parsers/manifest_reference_resolver.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/parsers/manifest_reference_resolver.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/parsers/model_to_component_factory.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/parsers/model_to_component_factory.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/partition_routers/list_partition_router.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/partition_routers/list_partition_router.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/partition_routers/single_partition_router.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/partition_routers/single_partition_router.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/partition_routers/substream_partition_router.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/partition_routers/substream_partition_router.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/requesters/error_handlers/__init__.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/requesters/error_handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/requesters/error_handlers/backoff_strategies/__init__.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/requesters/error_handlers/backoff_strategies/__init__.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/requesters/error_handlers/backoff_strategies/constant_backoff_strategy.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/requesters/error_handlers/backoff_strategies/constant_backoff_strategy.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/requesters/error_handlers/backoff_strategies/exponential_backoff_strategy.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/requesters/error_handlers/backoff_strategies/exponential_backoff_strategy.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/requesters/error_handlers/backoff_strategies/header_helper.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/requesters/error_handlers/backoff_strategies/header_helper.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/requesters/error_handlers/backoff_strategies/wait_time_from_header_backoff_strategy.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/requesters/error_handlers/backoff_strategies/wait_time_from_header_backoff_strategy.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/requesters/error_handlers/backoff_strategies/wait_until_time_from_header_backoff_strategy.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/requesters/error_handlers/backoff_strategies/wait_until_time_from_header_backoff_strategy.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/requesters/error_handlers/backoff_strategy.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/requesters/error_handlers/backoff_strategy.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/requesters/error_handlers/composite_error_handler.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/requesters/error_handlers/composite_error_handler.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/requesters/error_handlers/default_error_handler.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/requesters/error_handlers/default_error_handler.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/requesters/error_handlers/error_handler.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/requesters/error_handlers/error_handler.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/requesters/error_handlers/http_response_filter.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/requesters/error_handlers/http_response_filter.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/requesters/error_handlers/response_status.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/requesters/error_handlers/response_status.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/requesters/http_requester.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/requesters/http_requester.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/requesters/paginators/__init__.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/requesters/paginators/__init__.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/requesters/paginators/default_paginator.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/requesters/paginators/default_paginator.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/requesters/paginators/no_pagination.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/requesters/paginators/no_pagination.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/requesters/paginators/paginator.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/requesters/paginators/paginator.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/requesters/paginators/strategies/__init__.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/requesters/paginators/strategies/__init__.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/requesters/paginators/strategies/cursor_pagination_strategy.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/requesters/paginators/strategies/cursor_pagination_strategy.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/requesters/paginators/strategies/offset_increment.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/requesters/paginators/strategies/offset_increment.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/requesters/paginators/strategies/page_increment.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/requesters/paginators/strategies/page_increment.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/requesters/paginators/strategies/pagination_strategy.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/requesters/paginators/strategies/pagination_strategy.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/requesters/paginators/strategies/stop_condition.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/requesters/paginators/strategies/stop_condition.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/requesters/request_option.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/requesters/request_option.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/requesters/request_options/interpolated_nested_request_input_provider.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/requesters/request_options/interpolated_nested_request_input_provider.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/requesters/request_options/interpolated_request_input_provider.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/requesters/request_options/interpolated_request_input_provider.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/requesters/request_options/interpolated_request_options_provider.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/requesters/request_options/interpolated_request_options_provider.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/requesters/request_options/request_options_provider.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/requesters/request_options/request_options_provider.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/requesters/requester.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/requesters/requester.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/retrievers/retriever.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/retrievers/retriever.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/retrievers/simple_retriever.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/retrievers/simple_retriever.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/schema/__init__.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/schema/default_schema_loader.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/schema/default_schema_loader.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/schema/json_file_schema_loader.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/schema/json_file_schema_loader.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/spec/spec.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/spec/spec.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/stream_slicers/cartesian_product_stream_slicer.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/stream_slicers/cartesian_product_stream_slicer.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/stream_slicers/stream_slicer.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/stream_slicers/stream_slicer.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/transformations/__init__.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/transformations/add_fields.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/transformations/add_fields.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/transformations/remove_fields.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/transformations/remove_fields.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/transformations/transformation.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/transformations/transformation.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/types.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/types.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/declarative/yaml_declarative_source.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/declarative/yaml_declarative_source.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/embedded/base_integration.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/embedded/base_integration.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/embedded/catalog.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/embedded/catalog.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/embedded/runner.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/embedded/runner.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/embedded/tools.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/embedded/tools.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/file_based/README.md` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/file_based/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/file_based/__init__.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/file_based/__init__.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/file_based/availability_strategy/abstract_file_based_availability_strategy.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/file_based/availability_strategy/abstract_file_based_availability_strategy.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/file_based/availability_strategy/default_file_based_availability_strategy.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/file_based/availability_strategy/default_file_based_availability_strategy.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/file_based/config/abstract_file_based_spec.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/file_based/config/abstract_file_based_spec.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/file_based/config/avro_format.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/file_based/config/avro_format.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/file_based/config/csv_format.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/file_based/config/csv_format.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/file_based/config/file_based_stream_config.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/file_based/config/file_based_stream_config.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/file_based/config/parquet_format.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/file_based/config/parquet_format.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/file_based/config/unstructured_format.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/file_based/config/unstructured_format.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/file_based/discovery_policy/abstract_discovery_policy.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/file_based/discovery_policy/abstract_discovery_policy.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/file_based/discovery_policy/default_discovery_policy.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/file_based/discovery_policy/default_discovery_policy.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/file_based/exceptions.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/file_based/exceptions.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/file_based/file_based_source.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/file_based/file_based_source.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/file_based/file_based_stream_reader.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/file_based/file_based_stream_reader.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/file_based/file_types/__init__.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/file_based/file_types/__init__.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/file_based/file_types/avro_parser.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/file_based/file_types/avro_parser.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/file_based/file_types/csv_parser.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/file_based/file_types/csv_parser.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/file_based/file_types/file_type_parser.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/file_based/file_types/file_type_parser.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/file_based/file_types/jsonl_parser.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/file_based/file_types/jsonl_parser.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/file_based/file_types/parquet_parser.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/file_based/file_types/parquet_parser.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/file_based/file_types/unstructured_parser.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/file_based/file_types/unstructured_parser.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/file_based/schema_helpers.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/file_based/schema_helpers.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/file_based/schema_validation_policies/__init__.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/file_based/schema_validation_policies/__init__.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/file_based/schema_validation_policies/abstract_schema_validation_policy.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/file_based/schema_validation_policies/abstract_schema_validation_policy.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/file_based/schema_validation_policies/default_schema_validation_policies.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/file_based/schema_validation_policies/default_schema_validation_policies.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/file_based/stream/abstract_file_based_stream.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/file_based/stream/abstract_file_based_stream.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/file_based/stream/concurrent/adapters.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/file_based/stream/concurrent/adapters.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/file_based/stream/concurrent/cursor/abstract_concurrent_file_based_cursor.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/file_based/stream/concurrent/cursor/abstract_concurrent_file_based_cursor.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/file_based/stream/concurrent/cursor/file_based_concurrent_cursor.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/file_based/stream/concurrent/cursor/file_based_concurrent_cursor.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/file_based/stream/concurrent/cursor/file_based_final_state_cursor.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/file_based/stream/concurrent/cursor/file_based_final_state_cursor.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/file_based/stream/cursor/abstract_file_based_cursor.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/file_based/stream/cursor/abstract_file_based_cursor.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/file_based/stream/cursor/default_file_based_cursor.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/file_based/stream/cursor/default_file_based_cursor.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/file_based/stream/default_file_based_stream.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/file_based/stream/default_file_based_stream.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 from airbyte_cdk.models import AirbyteLogMessage, AirbyteMessage, FailureType, Level
 from airbyte_cdk.models import Type as MessageType
 from airbyte_cdk.sources.file_based.config.file_based_stream_config import PrimaryKeyType
 from airbyte_cdk.sources.file_based.exceptions import (
     FileBasedSourceError,
     InvalidSchemaError,
     MissingSchemaError,
-    NoFilesMatchingError,
     RecordParseError,
     SchemaInferenceError,
     StopSyncPerValidationPolicy,
 )
 from airbyte_cdk.sources.file_based.remote_file import RemoteFile
 from airbyte_cdk.sources.file_based.schema_helpers import SchemaType, merge_schemas, schemaless_schema
 from airbyte_cdk.sources.file_based.stream import AbstractFileBasedStream
@@ -168,15 +167,15 @@
     def get_json_schema(self) -> JsonSchema:
         extra_fields = {
             self.ab_last_mod_col: {"type": "string"},
             self.ab_file_name_col: {"type": "string"},
         }
         try:
             schema = self._get_raw_json_schema()
-        except (InvalidSchemaError, NoFilesMatchingError) as config_exception:
+        except InvalidSchemaError as config_exception:
             self.logger.exception(FileBasedSourceError.SCHEMA_INFERENCE_ERROR.value, exc_info=config_exception)
             raise AirbyteTracedException(
                 internal_message="Please check the logged errors for more information.",
                 message=FileBasedSourceError.SCHEMA_INFERENCE_ERROR.value,
                 exception=AirbyteTracedException(exception=config_exception),
                 failure_type=FailureType.config_error,
             )
@@ -191,15 +190,16 @@
         elif self.config.schemaless:
             return schemaless_schema
         else:
             files = self.list_files()
             total_n_files = len(files)
 
             if total_n_files == 0:
-                raise NoFilesMatchingError(FileBasedSourceError.EMPTY_STREAM, stream=self.name)
+                self.logger.warning(msg=f"No files were identified in the stream {self.name}. Setting default schema for the stream.")
+                return schemaless_schema
 
             max_n_files_for_schema_inference = self._discovery_policy.get_max_n_files_for_schema_inference(self.get_parser())
             if total_n_files > max_n_files_for_schema_inference:
                 # Use the most recent files for schema inference, so we pick up schema changes during discovery.
                 files = sorted(files, key=lambda x: x.last_modified, reverse=True)[:max_n_files_for_schema_inference]
                 self.logger.warn(
                     msg=f"Refusing to infer schema for all {total_n_files} files; using {max_n_files_for_schema_inference} files."
```

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/http_config.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/http_config.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/http_logger.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/http_logger.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/message/repository.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/message/repository.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/source.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/source.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/streams/availability_strategy.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/streams/availability_strategy.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/streams/call_rate.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/streams/call_rate.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/streams/checkpoint/checkpoint_reader.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/streams/checkpoint/checkpoint_reader.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/streams/checkpoint/cursor.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/streams/checkpoint/cursor.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/streams/concurrent/README.md` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/streams/concurrent/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/streams/concurrent/abstract_stream.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/streams/concurrent/abstract_stream.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/streams/concurrent/abstract_stream_facade.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/streams/concurrent/abstract_stream_facade.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/streams/concurrent/adapters.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/streams/concurrent/adapters.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/streams/concurrent/availability_strategy.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/streams/concurrent/availability_strategy.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/streams/concurrent/cursor.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/streams/concurrent/cursor.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/streams/concurrent/default_stream.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/streams/concurrent/default_stream.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/streams/concurrent/helpers.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/streams/concurrent/helpers.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/streams/concurrent/partition_enqueuer.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/streams/concurrent/partition_enqueuer.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/streams/concurrent/partition_reader.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/streams/concurrent/partition_reader.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/streams/concurrent/partitions/partition.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/streams/concurrent/partitions/partition.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/streams/concurrent/partitions/record.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/streams/concurrent/partitions/record.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/streams/concurrent/partitions/types.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/streams/concurrent/partitions/types.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/streams/concurrent/state_converters/abstract_stream_state_converter.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/streams/concurrent/state_converters/abstract_stream_state_converter.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/streams/concurrent/state_converters/datetime_stream_state_converter.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/streams/concurrent/state_converters/datetime_stream_state_converter.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/streams/core.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/streams/core.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/streams/http/availability_strategy.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/streams/http/availability_strategy.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/streams/http/error_handlers/__init__.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/streams/http/error_handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/streams/http/error_handlers/backoff_strategy.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/streams/http/error_handlers/backoff_strategy.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/streams/http/error_handlers/default_backoff_strategy.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/streams/http/error_handlers/default_backoff_strategy.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/streams/http/error_handlers/error_handler.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/streams/http/error_handlers/error_handler.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/streams/http/error_handlers/http_status_error_handler.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/streams/http/error_handlers/http_status_error_handler.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/streams/http/error_handlers/json_error_message_parser.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/streams/http/error_handlers/json_error_message_parser.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/streams/http/exceptions.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/streams/http/exceptions.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/streams/http/http.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/streams/http/http.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/streams/http/http_client.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/streams/http/http_client.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/streams/http/rate_limiting.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/streams/http/rate_limiting.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/streams/http/requests_native_auth/abstract_oauth.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/streams/http/requests_native_auth/abstract_oauth.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/streams/http/requests_native_auth/abstract_token.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/streams/http/requests_native_auth/abstract_token.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/streams/http/requests_native_auth/oauth.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/streams/http/requests_native_auth/oauth.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/streams/http/requests_native_auth/token.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/streams/http/requests_native_auth/token.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/streams/utils/stream_helper.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/streams/utils/stream_helper.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/types.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/types.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/utils/catalog_helpers.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/utils/catalog_helpers.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/utils/record_helper.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/utils/record_helper.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/utils/schema_helpers.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/utils/schema_helpers.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/utils/schema_models.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/utils/schema_models.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/utils/slice_logger.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/utils/slice_logger.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/sources/utils/transform.py` & `airbyte_cdk-1.0.1/airbyte_cdk/sources/utils/transform.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/test/catalog_builder.py` & `airbyte_cdk-1.0.1/airbyte_cdk/test/catalog_builder.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/test/entrypoint_wrapper.py` & `airbyte_cdk-1.0.1/airbyte_cdk/test/entrypoint_wrapper.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/test/mock_http/matcher.py` & `airbyte_cdk-1.0.1/airbyte_cdk/test/mock_http/matcher.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/test/mock_http/mocker.py` & `airbyte_cdk-1.0.1/airbyte_cdk/test/mock_http/mocker.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/test/mock_http/request.py` & `airbyte_cdk-1.0.1/airbyte_cdk/test/mock_http/request.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/test/mock_http/response.py` & `airbyte_cdk-1.0.1/airbyte_cdk/test/mock_http/response.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/test/mock_http/response_builder.py` & `airbyte_cdk-1.0.1/airbyte_cdk/test/mock_http/response_builder.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/test/state_builder.py` & `airbyte_cdk-1.0.1/airbyte_cdk/test/state_builder.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/utils/airbyte_secrets_utils.py` & `airbyte_cdk-1.0.1/airbyte_cdk/utils/airbyte_secrets_utils.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/utils/analytics_message.py` & `airbyte_cdk-1.0.1/airbyte_cdk/utils/analytics_message.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/utils/datetime_format_inferrer.py` & `airbyte_cdk-1.0.1/airbyte_cdk/utils/datetime_format_inferrer.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/utils/event_timing.py` & `airbyte_cdk-1.0.1/airbyte_cdk/utils/event_timing.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/utils/is_cloud_environment.py` & `airbyte_cdk-1.0.1/airbyte_cdk/utils/is_cloud_environment.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/utils/mapping_helpers.py` & `airbyte_cdk-1.0.1/airbyte_cdk/utils/mapping_helpers.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/utils/message_utils.py` & `airbyte_cdk-1.0.1/airbyte_cdk/utils/message_utils.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/utils/oneof_option_config.py` & `airbyte_cdk-1.0.1/airbyte_cdk/utils/oneof_option_config.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/utils/schema_inferrer.py` & `airbyte_cdk-1.0.1/airbyte_cdk/utils/schema_inferrer.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/utils/spec_schema_transformations.py` & `airbyte_cdk-1.0.1/airbyte_cdk/utils/spec_schema_transformations.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/utils/stream_status_utils.py` & `airbyte_cdk-1.0.1/airbyte_cdk/utils/stream_status_utils.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/airbyte_cdk/utils/traced_exception.py` & `airbyte_cdk-1.0.1/airbyte_cdk/utils/traced_exception.py`

 * *Files identical despite different names*

### Comparing `airbyte_cdk-1.0.0/pyproject.toml` & `airbyte_cdk-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "airbyte-cdk"
-version = "1.0.0"
+version = "1.0.1"
 description = "A framework for writing Airbyte Connectors."
 authors = ["Airbyte <contact@airbyte.io>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/airbytehq/airbyte"
 repository = "https://github.com/airbytehq/airbyte"
 documentation = "https://docs.airbyte.io/"
```

### Comparing `airbyte_cdk-1.0.0/PKG-INFO` & `airbyte_cdk-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-cdk
-Version: 1.0.0
+Version: 1.0.1
 Summary: A framework for writing Airbyte Connectors.
 Home-page: https://github.com/airbytehq/airbyte
 License: MIT
 Keywords: airbyte,connector-development-kit,cdk
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<4.0
```
