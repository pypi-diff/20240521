# Comparing `tmp/spetlr-5.1.6.tar.gz` & `tmp/spetlr-5.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spetlr-5.1.6.tar", last modified: Wed May 15 08:21:07 2024, max compression
+gzip compressed data, was "spetlr-5.1.9.tar", last modified: Tue May 21 11:40:54 2024, max compression
```

## Comparing `spetlr-5.1.6.tar` & `spetlr-5.1.9.tar`

### file list

```diff
@@ -1,351 +1,351 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:07.630220 spetlr-5.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-15 08:20:58.000000 spetlr-5.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-15 08:20:58.000000 spetlr-5.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8653 2024-05-15 08:21:07.630220 spetlr-5.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6434 2024-05-15 08:20:58.000000 spetlr-5.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-15 08:20:58.000000 spetlr-5.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-05-15 08:21:07.630220 spetlr-5.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 08:20:58.000000 spetlr-5.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:07.586219 spetlr-5.1.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:07.594220 spetlr-5.1.6/src/spetlr/
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/alias.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:07.594220 spetlr-5.1.6/src/spetlr/azure_log_analytics/
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/azure_log_analytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/azure_log_analytics/azure_log_analytics_handle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:07.598219 spetlr-5.1.6/src/spetlr/cache/
--rw-r--r--   0 runner    (1001) docker     (127)     8344 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/cache/CachedLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/cache/CachedLoaderParameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/cache/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:07.598219 spetlr-5.1.6/src/spetlr/config_master/
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/config_master/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:07.598219 spetlr-5.1.6/src/spetlr/configurator/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/configurator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:07.598219 spetlr-5.1.6/src/spetlr/configurator/_cli/
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/configurator/_cli/ConfiguratorCli.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/configurator/_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/configurator/_cli/generate_keys_file.py
--rw-r--r--   0 runner    (1001) docker     (127)    18060 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/configurator/configurator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:07.598219 spetlr-5.1.6/src/spetlr/configurator/sql/
--rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/configurator/sql/StatementBlocks.py
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/configurator/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/configurator/sql/comments.py
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/configurator/sql/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/configurator/sql/db.py
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/configurator/sql/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/configurator/sql/init_sqlparse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/configurator/sql/parse_sql.py
--rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/configurator/sql/substructures.py
--rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/configurator/sql/table.py
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/configurator/sql/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/configurator/sql/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/configurator/sql/view.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:07.598219 spetlr-5.1.6/src/spetlr/cosmos/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/cosmos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6686 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/cosmos/cosmos.py
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/cosmos/cosmos_base_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/cosmos/cosmos_handle.py
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/db_auto.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:07.598219 spetlr-5.1.6/src/spetlr/delta/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/delta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/delta/db_handle.py
--rw-r--r--   0 runner    (1001) docker     (127)    10383 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/delta/delta_handle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:07.602220 spetlr-5.1.6/src/spetlr/deltaspec/
--rw-r--r--   0 runner    (1001) docker     (127)     5554 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/deltaspec/DeltaDatabaseSpec.py
--rw-r--r--   0 runner    (1001) docker     (127)     8772 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/deltaspec/DeltaTableSpec.py
--rw-r--r--   0 runner    (1001) docker     (127)     8455 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/deltaspec/DeltaTableSpecBase.py
--rw-r--r--   0 runner    (1001) docker     (127)    18247 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/deltaspec/DeltaTableSpecDifference.py
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/deltaspec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/deltaspec/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/deltaspec/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:07.602220 spetlr-5.1.6/src/spetlr/eh/
--rw-r--r--   0 runner    (1001) docker     (127)     8005 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/eh/EventHubCapture.py
--rw-r--r--   0 runner    (1001) docker     (127)    10391 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/eh/EventHubCaptureExtractor.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/eh/EventHubJsonPublisher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/eh/EventHubStream.py
--rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/eh/PartitionSpec.py
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/eh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/eh/eh_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:07.602220 spetlr-5.1.6/src/spetlr/entry_points/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/entry_points/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/entry_points/generalized_task_entry_point.py
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/entry_points/task_entry_point.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:07.602220 spetlr-5.1.6/src/spetlr/etl/
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/etl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/etl/extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:07.602220 spetlr-5.1.6/src/spetlr/etl/extractors/
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/etl/extractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/etl/extractors/check_schema_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/etl/extractors/incremental_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/etl/extractors/lazy_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/etl/extractors/lazy_simple_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/etl/extractors/schema_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/etl/extractors/simple_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/etl/extractors/stream_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/etl/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:07.606220 spetlr-5.1.6/src/spetlr/etl/loaders/
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/etl/loaders/DeleteDataLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/etl/loaders/UpsertLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/etl/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/etl/loaders/load_modes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/etl/loaders/scd2_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/etl/loaders/simple_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/etl/loaders/simple_sql_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     5189 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/etl/loaders/stream_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/etl/loaders/upsert_loader_streaming.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:07.606220 spetlr-5.1.6/src/spetlr/etl/log/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/etl/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4844 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/etl/log/log_orchestrator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/etl/log/log_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:07.606220 spetlr-5.1.6/src/spetlr/etl/log/log_transformers/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/etl/log/log_transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/etl/log/log_transformers/count_log_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/etl/log/log_transformers/null_log_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/etl/orchestrator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/etl/transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:07.610220 spetlr-5.1.6/src/spetlr/etl/transformers/
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/etl/transformers/SimpleSqlTransformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/etl/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/etl/transformers/clean_column_names_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/etl/transformers/country_to_alphacode_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/etl/transformers/data_change_capture_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/etl/transformers/dropColumnsTransformer.py
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/etl/transformers/drop_oldest_duplicate_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/etl/transformers/fuzzy_select.py
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/etl/transformers/generate_md5_column_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/etl/transformers/join_dataframes_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/etl/transformers/selectColumnsTransformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/etl/transformers/select_and_cast_columns_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/etl/transformers/simple_dataframe_filter_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/etl/transformers/simple_sql_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/etl/transformers/timezone_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/etl/transformers/union_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/etl/transformers/validfromto_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/etl/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:07.610220 spetlr-5.1.6/src/spetlr/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/exceptions/cli_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/exceptions/configurator_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:07.610220 spetlr-5.1.6/src/spetlr/extractors/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/extractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/extractors/eventhub_stream_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:07.610220 spetlr-5.1.6/src/spetlr/filehandle/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/filehandle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/filehandle/file_handle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:07.610220 spetlr-5.1.6/src/spetlr/formatting/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/formatting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/formatting/git_hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:07.610220 spetlr-5.1.6/src/spetlr/mount/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/mount/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/mount/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:07.610220 spetlr-5.1.6/src/spetlr/orchestrators/
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/orchestrators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:07.610220 spetlr-5.1.6/src/spetlr/orchestrators/eh2bronze/
--rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/orchestrators/eh2bronze/EhToDeltaBronzeOrchestrator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/orchestrators/eh2bronze/EhToDeltaBronzeTransformer.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/orchestrators/eh2bronze/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:07.610220 spetlr-5.1.6/src/spetlr/orchestrators/eh2silver/
--rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/orchestrators/eh2silver/EhToDeltaSilverOrchestrator.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/orchestrators/eh2silver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:07.610220 spetlr-5.1.6/src/spetlr/orchestrators/ehjson2delta/
--rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/orchestrators/ehjson2delta/EhJsonToDeltaExtractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/orchestrators/ehjson2delta/EhJsonToDeltaOrchestrator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/orchestrators/ehjson2delta/EhJsonToDeltaTransformer.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/orchestrators/ehjson2delta/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:07.610220 spetlr-5.1.6/src/spetlr/power_bi/
--rw-r--r--   0 runner    (1001) docker     (127)    50067 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/power_bi/PowerBi.py
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/power_bi/PowerBiClient.py
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/power_bi/PowerBiException.py
--rw-r--r--   0 runner    (1001) docker     (127)    12063 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/power_bi/SparkPandasDataFrame.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/power_bi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:07.610220 spetlr-5.1.6/src/spetlr/reporting/
--rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/reporting/JobReflection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4349 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/reporting/SlackNotifier.py
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/reporting/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:07.614220 spetlr-5.1.6/src/spetlr/schema_manager/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/schema_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5794 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/schema_manager/schema_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     9697 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/schema_manager/spark_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:07.614220 spetlr-5.1.6/src/spetlr/singleton/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/singleton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/singleton/singleton.py
--rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/spark.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:07.614220 spetlr-5.1.6/src/spetlr/sql/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/sql/BaseExecutor.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/sql/CommonBaseServer.py
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/sql/SqlBaseServer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6959 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/sql/SqlExecutor.py
--rw-r--r--   0 runner    (1001) docker     (127)    15267 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/sql/SqlServer.py
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/sql/SqlServerBaseOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/sql/sql_handle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:07.614220 spetlr-5.1.6/src/spetlr/sqlrepr/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/sqlrepr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/sqlrepr/sql_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:07.614220 spetlr-5.1.6/src/spetlr/tables/
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/tables/TableHandle.py
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/tables/ThMaker.py
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/tables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:07.614220 spetlr-5.1.6/src/spetlr/testutils/
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/testutils/CleanupTestDatabases.py
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/testutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/testutils/stop_test_streams.py
--rw-r--r--   0 runner    (1001) docker     (127)    13226 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/transformations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:07.614220 spetlr-5.1.6/src/spetlr/transformers/
--rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/transformers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:07.618220 spetlr-5.1.6/src/spetlr/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/utils/CheckDfMerge.py
--rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/utils/DataframeCreator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/utils/DeleteMismatchedSchemas.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/utils/DropOldestDuplicates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/utils/GetMergeStatement.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/utils/Md5HashColumn.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/utils/MockExtractor.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/utils/MockLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/utils/SelectAndCastColumns.py
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-15 08:20:58.000000 spetlr-5.1.6/src/spetlr/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:07.594220 spetlr-5.1.6/src/spetlr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8653 2024-05-15 08:21:07.000000 spetlr-5.1.6/src/spetlr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11435 2024-05-15 08:21:07.000000 spetlr-5.1.6/src/spetlr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 08:21:07.000000 spetlr-5.1.6/src/spetlr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-15 08:21:07.000000 spetlr-5.1.6/src/spetlr.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 08:21:07.000000 spetlr-5.1.6/src/spetlr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-15 08:21:07.000000 spetlr-5.1.6/src/spetlr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-15 08:21:07.000000 spetlr-5.1.6/src/spetlr.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:07.590220 spetlr-5.1.6/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:07.590220 spetlr-5.1.6/tests/cluster/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:07.618220 spetlr-5.1.6/tests/cluster/azure_log_analytics/
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/cluster/azure_log_analytics/test_azure_log_analytics_handle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:07.618220 spetlr-5.1.6/tests/cluster/cache/
--rw-r--r--   0 runner    (1001) docker     (127)     6039 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/cluster/cache/test_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:07.618220 spetlr-5.1.6/tests/cluster/cosmos/
--rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/cluster/cosmos/test_cosmos.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:07.618220 spetlr-5.1.6/tests/cluster/db/
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/cluster/db/test_db_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:07.618220 spetlr-5.1.6/tests/cluster/delta/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:07.618220 spetlr-5.1.6/tests/cluster/delta/deltaspec/
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/cluster/delta/deltaspec/test_dbspec.py
--rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/cluster/delta/deltaspec/test_tblspec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/cluster/delta/test_cleanup_databases.py
--rw-r--r--   0 runner    (1001) docker     (127)     5675 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/cluster/delta/test_delta_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     8696 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/cluster/delta/test_delta_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     6505 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/cluster/delta/test_filehandle.py
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/cluster/delta/test_sparkexecutor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:07.618220 spetlr-5.1.6/tests/cluster/eh/
--rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/cluster/eh/test_eh_json_orchestrator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4665 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/cluster/eh/test_eh_json_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/cluster/eh/test_eh_saving.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:07.618220 spetlr-5.1.6/tests/cluster/etl/
--rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/cluster/etl/test_checkschemaextractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/cluster/etl/test_delete_data_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/cluster/etl/test_deltaupsert.py
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/cluster/etl/test_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     9721 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/cluster/etl/test_incremental_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4226 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/cluster/etl/test_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/cluster/etl/test_orchestrator_etl_warning.py
--rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/cluster/etl/test_simpleloader_upsert.py
--rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/cluster/etl/test_upsertloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4591 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/cluster/etl/test_upsertloader_streaming.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:07.618220 spetlr-5.1.6/tests/cluster/filehandle/
--rw-r--r--   0 runner    (1001) docker     (127)     5435 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/cluster/filehandle/test_filehandle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:07.618220 spetlr-5.1.6/tests/cluster/loaders/
--rw-r--r--   0 runner    (1001) docker     (127)    26466 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/cluster/loaders/test_scd2_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:07.618220 spetlr-5.1.6/tests/cluster/reporting/
--rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/cluster/reporting/test_slack_reporting.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:07.618220 spetlr-5.1.6/tests/cluster/schema_manager/
--rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/cluster/schema_manager/test_schema_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:07.622220 spetlr-5.1.6/tests/cluster/sql/
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/cluster/sql/test_deliveryexecutor.py
--rw-r--r--   0 runner    (1001) docker     (127)    12751 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/cluster/sql/test_deliverysql.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/cluster/sql/test_deliverysqlspn.py
--rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/cluster/sql/test_simple_sql_etl.py
--rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/cluster/sql/test_sql_streaming.py
--rw-r--r--   0 runner    (1001) docker     (127)     5516 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/cluster/sql/test_sqlhandle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:07.622220 spetlr-5.1.6/tests/cluster/transformations/
--rw-r--r--   0 runner    (1001) docker     (127)     6530 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/cluster/transformations/test_merge_df_into_target.py
--rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/cluster/transformations/test_simple_sql_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/cluster/transformations/test_union_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:07.622220 spetlr-5.1.6/tests/cluster/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/cluster/utils/test_delete_schema_mismatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/cluster/utils/test_spark_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/cluster/utils/test_stop_test_stream.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:07.622220 spetlr-5.1.6/tests/local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:07.622220 spetlr-5.1.6/tests/local/azure_log_analytics/
--rw-r--r--   0 runner    (1001) docker     (127)     4799 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/local/azure_log_analytics/test_azure_log_analytics_handle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:07.622220 spetlr-5.1.6/tests/local/configurator/
--rw-r--r--   0 runner    (1001) docker     (127)     9658 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/local/configurator/test_configurator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/local/configurator/test_configurator_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:07.622220 spetlr-5.1.6/tests/local/delta/
--rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/local/delta/test_DeltaDatabaseSpec.py
--rw-r--r--   0 runner    (1001) docker     (127)    12308 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/local/delta/test_DeltaTableSpec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/local/delta/test_table_name.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:07.622220 spetlr-5.1.6/tests/local/eh/
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/local/eh/test_EventHubCaptureExtractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4618 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/local/eh/test_ehto_bronze_and_silver.py
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/local/eh/test_ehtodeltabronze_orchestrator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/local/eh/test_ehtodeltabronze_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7356 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/local/eh/test_ehtodeltasilver_orchestrator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:07.622220 spetlr-5.1.6/tests/local/entry_points/
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/local/entry_points/test_generalized_entry_points.py
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/local/entry_points/test_task_entry_point.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:07.626220 spetlr-5.1.6/tests/local/etl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:07.626220 spetlr-5.1.6/tests/local/etl/log/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:07.626220 spetlr-5.1.6/tests/local/etl/log/log_transformers/
--rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/local/etl/log/log_transformers/test_count_log_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/local/etl/log/log_transformers/test_null_log_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/local/etl/log/test_log_orchestrator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/local/etl/log/test_log_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/local/etl/test_lazy_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/local/etl/test_orchestrator.py
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/local/etl/test_simple_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)    11196 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/local/etl/test_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:07.626220 spetlr-5.1.6/tests/local/extractors/
--rw-r--r--   0 runner    (1001) docker     (127)     4547 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/local/extractors/test_eventhub_stream_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:07.626220 spetlr-5.1.6/tests/local/filehandle/
--rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/local/filehandle/test_filehandle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:07.626220 spetlr-5.1.6/tests/local/power_bi/
--rw-r--r--   0 runner    (1001) docker     (127)    56683 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/local/power_bi/test_power_bi.py
--rw-r--r--   0 runner    (1001) docker     (127)     5152 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/local/power_bi/test_spark_pandas_dataframe.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:07.626220 spetlr-5.1.6/tests/local/reporting/
--rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/local/reporting/test_slack_reporting.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:07.626220 spetlr-5.1.6/tests/local/repr/
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/local/repr/test_repr_sql_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:07.626220 spetlr-5.1.6/tests/local/schema_manager/
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/local/schema_manager/test_schema_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:07.626220 spetlr-5.1.6/tests/local/sql/
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/local/sql/test_SqlExecutor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:07.626220 spetlr-5.1.6/tests/local/streaming/
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/local/streaming/test_deltahandle_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/local/streaming/test_stream_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/local/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/local/test_get_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/local/test_spark.py
--rw-r--r--   0 runner    (1001) docker     (127)     5543 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/local/test_sqlServer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6193 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/local/test_transformations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:07.630220 spetlr-5.1.6/tests/local/transformers/
--rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/local/transformers/test_clean_column_names_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8391 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/local/transformers/test_concat_df.py
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/local/transformers/test_country_to_alphacode_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4547 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/local/transformers/test_data_change_capture_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/local/transformers/test_drop_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/local/transformers/test_dropoldestduplicates.py
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/local/transformers/test_fuzzy_select.py
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/local/transformers/test_generate_md5_column_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)    13371 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/local/transformers/test_join_dataframes_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/local/transformers/test_select_and_cast_columns_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/local/transformers/test_select_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/local/transformers/test_simple_dataframe_filter_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/local/transformers/test_timezone_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4704 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/local/transformers/test_union_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/local/transformers/test_validfromto_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:07.630220 spetlr-5.1.6/tests/local/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/local/utils/test_cleandatabases.py
--rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/local/utils/test_dataframe_creation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/local/utils/test_dropoldestduplicates.py
--rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/local/utils/test_getmergestatement.py
--rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/local/utils/test_md5_hashcolumn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/local/utils/test_mock_etl.py
--rw-r--r--   0 runner    (1001) docker     (127)     5916 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/local/utils/test_selectandcastcolumns.py
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-15 08:20:58.000000 spetlr-5.1.6/tests/local/utils/test_stop_test_streams.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:40:54.272503 spetlr-5.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-21 11:40:40.000000 spetlr-5.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-21 11:40:40.000000 spetlr-5.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8653 2024-05-21 11:40:54.272503 spetlr-5.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6434 2024-05-21 11:40:40.000000 spetlr-5.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-21 11:40:40.000000 spetlr-5.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-05-21 11:40:54.272503 spetlr-5.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 11:40:40.000000 spetlr-5.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:40:54.220503 spetlr-5.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:40:54.228503 spetlr-5.1.9/src/spetlr/
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/alias.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:40:54.232503 spetlr-5.1.9/src/spetlr/azure_log_analytics/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/azure_log_analytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/azure_log_analytics/azure_log_analytics_handle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:40:54.232503 spetlr-5.1.9/src/spetlr/cache/
+-rw-r--r--   0 runner    (1001) docker     (127)     8344 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/cache/CachedLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/cache/CachedLoaderParameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/cache/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:40:54.232503 spetlr-5.1.9/src/spetlr/config_master/
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/config_master/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:40:54.232503 spetlr-5.1.9/src/spetlr/configurator/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/configurator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:40:54.232503 spetlr-5.1.9/src/spetlr/configurator/_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/configurator/_cli/ConfiguratorCli.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/configurator/_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/configurator/_cli/generate_keys_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18060 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/configurator/configurator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:40:54.236503 spetlr-5.1.9/src/spetlr/configurator/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/configurator/sql/StatementBlocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/configurator/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/configurator/sql/comments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/configurator/sql/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/configurator/sql/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/configurator/sql/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/configurator/sql/init_sqlparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/configurator/sql/parse_sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/configurator/sql/substructures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/configurator/sql/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/configurator/sql/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/configurator/sql/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/configurator/sql/view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:40:54.236503 spetlr-5.1.9/src/spetlr/cosmos/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/cosmos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6686 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/cosmos/cosmos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/cosmos/cosmos_base_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/cosmos/cosmos_handle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/db_auto.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:40:54.236503 spetlr-5.1.9/src/spetlr/delta/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/delta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/delta/db_handle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10383 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/delta/delta_handle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:40:54.236503 spetlr-5.1.9/src/spetlr/deltaspec/
+-rw-r--r--   0 runner    (1001) docker     (127)     5554 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/deltaspec/DeltaDatabaseSpec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8772 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/deltaspec/DeltaTableSpec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8455 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/deltaspec/DeltaTableSpecBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18247 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/deltaspec/DeltaTableSpecDifference.py
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/deltaspec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/deltaspec/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/deltaspec/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:40:54.236503 spetlr-5.1.9/src/spetlr/eh/
+-rw-r--r--   0 runner    (1001) docker     (127)     8005 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/eh/EventHubCapture.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10391 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/eh/EventHubCaptureExtractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/eh/EventHubJsonPublisher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/eh/EventHubStream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/eh/PartitionSpec.py
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/eh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/eh/eh_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:40:54.240503 spetlr-5.1.9/src/spetlr/entry_points/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/entry_points/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/entry_points/generalized_task_entry_point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/entry_points/task_entry_point.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:40:54.240503 spetlr-5.1.9/src/spetlr/etl/
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/etl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/etl/extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:40:54.240503 spetlr-5.1.9/src/spetlr/etl/extractors/
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/etl/extractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/etl/extractors/check_schema_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/etl/extractors/incremental_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/etl/extractors/lazy_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/etl/extractors/lazy_simple_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/etl/extractors/schema_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/etl/extractors/simple_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/etl/extractors/stream_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/etl/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:40:54.244503 spetlr-5.1.9/src/spetlr/etl/loaders/
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/etl/loaders/DeleteDataLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/etl/loaders/UpsertLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/etl/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/etl/loaders/load_modes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/etl/loaders/scd2_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/etl/loaders/simple_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/etl/loaders/simple_sql_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5189 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/etl/loaders/stream_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/etl/loaders/upsert_loader_streaming.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:40:54.244503 spetlr-5.1.9/src/spetlr/etl/log/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/etl/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4844 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/etl/log/log_orchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/etl/log/log_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:40:54.244503 spetlr-5.1.9/src/spetlr/etl/log/log_transformers/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/etl/log/log_transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/etl/log/log_transformers/count_log_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/etl/log/log_transformers/null_log_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/etl/orchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/etl/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:40:54.244503 spetlr-5.1.9/src/spetlr/etl/transformers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/etl/transformers/SimpleSqlTransformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/etl/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/etl/transformers/clean_column_names_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/etl/transformers/country_to_alphacode_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/etl/transformers/data_change_capture_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/etl/transformers/dropColumnsTransformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/etl/transformers/drop_oldest_duplicate_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/etl/transformers/fuzzy_select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/etl/transformers/generate_md5_column_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/etl/transformers/join_dataframes_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/etl/transformers/selectColumnsTransformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/etl/transformers/select_and_cast_columns_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/etl/transformers/simple_dataframe_filter_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/etl/transformers/simple_sql_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/etl/transformers/timezone_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/etl/transformers/union_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/etl/transformers/validfromto_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/etl/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:40:54.248503 spetlr-5.1.9/src/spetlr/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/exceptions/cli_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/exceptions/configurator_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:40:54.248503 spetlr-5.1.9/src/spetlr/extractors/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/extractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/extractors/eventhub_stream_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:40:54.248503 spetlr-5.1.9/src/spetlr/filehandle/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/filehandle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/filehandle/file_handle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:40:54.248503 spetlr-5.1.9/src/spetlr/formatting/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/formatting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/formatting/git_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:40:54.248503 spetlr-5.1.9/src/spetlr/mount/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/mount/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/mount/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:40:54.248503 spetlr-5.1.9/src/spetlr/orchestrators/
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/orchestrators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:40:54.248503 spetlr-5.1.9/src/spetlr/orchestrators/eh2bronze/
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/orchestrators/eh2bronze/EhToDeltaBronzeOrchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/orchestrators/eh2bronze/EhToDeltaBronzeTransformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/orchestrators/eh2bronze/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:40:54.248503 spetlr-5.1.9/src/spetlr/orchestrators/eh2silver/
+-rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/orchestrators/eh2silver/EhToDeltaSilverOrchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/orchestrators/eh2silver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:40:54.248503 spetlr-5.1.9/src/spetlr/orchestrators/ehjson2delta/
+-rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/orchestrators/ehjson2delta/EhJsonToDeltaExtractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/orchestrators/ehjson2delta/EhJsonToDeltaOrchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/orchestrators/ehjson2delta/EhJsonToDeltaTransformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/orchestrators/ehjson2delta/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:40:54.248503 spetlr-5.1.9/src/spetlr/power_bi/
+-rw-r--r--   0 runner    (1001) docker     (127)    50155 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/power_bi/PowerBi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/power_bi/PowerBiClient.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/power_bi/PowerBiException.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12057 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/power_bi/SparkPandasDataFrame.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/power_bi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:40:54.252503 spetlr-5.1.9/src/spetlr/reporting/
+-rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/reporting/JobReflection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4349 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/reporting/SlackNotifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/reporting/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:40:54.252503 spetlr-5.1.9/src/spetlr/schema_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/schema_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5794 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/schema_manager/schema_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9697 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/schema_manager/spark_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:40:54.252503 spetlr-5.1.9/src/spetlr/singleton/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/singleton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/singleton/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/spark.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:40:54.252503 spetlr-5.1.9/src/spetlr/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/sql/BaseExecutor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/sql/CommonBaseServer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/sql/SqlBaseServer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6959 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/sql/SqlExecutor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15267 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/sql/SqlServer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/sql/SqlServerBaseOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/sql/sql_handle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:40:54.252503 spetlr-5.1.9/src/spetlr/sqlrepr/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/sqlrepr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/sqlrepr/sql_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:40:54.252503 spetlr-5.1.9/src/spetlr/tables/
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/tables/TableHandle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/tables/ThMaker.py
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/tables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:40:54.252503 spetlr-5.1.9/src/spetlr/testutils/
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/testutils/CleanupTestDatabases.py
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/testutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/testutils/stop_test_streams.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13226 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/transformations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:40:54.252503 spetlr-5.1.9/src/spetlr/transformers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/transformers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:40:54.256503 spetlr-5.1.9/src/spetlr/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/utils/CheckDfMerge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/utils/DataframeCreator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/utils/DeleteMismatchedSchemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/utils/DropOldestDuplicates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/utils/GetMergeStatement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/utils/Md5HashColumn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/utils/MockExtractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/utils/MockLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/utils/SelectAndCastColumns.py
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-21 11:40:40.000000 spetlr-5.1.9/src/spetlr/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:40:54.232503 spetlr-5.1.9/src/spetlr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8653 2024-05-21 11:40:53.000000 spetlr-5.1.9/src/spetlr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11435 2024-05-21 11:40:54.000000 spetlr-5.1.9/src/spetlr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 11:40:53.000000 spetlr-5.1.9/src/spetlr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-21 11:40:53.000000 spetlr-5.1.9/src/spetlr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 11:40:53.000000 spetlr-5.1.9/src/spetlr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-21 11:40:53.000000 spetlr-5.1.9/src/spetlr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-21 11:40:53.000000 spetlr-5.1.9/src/spetlr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:40:54.224503 spetlr-5.1.9/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:40:54.224503 spetlr-5.1.9/tests/cluster/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:40:54.256503 spetlr-5.1.9/tests/cluster/azure_log_analytics/
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/cluster/azure_log_analytics/test_azure_log_analytics_handle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:40:54.256503 spetlr-5.1.9/tests/cluster/cache/
+-rw-r--r--   0 runner    (1001) docker     (127)     6039 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/cluster/cache/test_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:40:54.256503 spetlr-5.1.9/tests/cluster/cosmos/
+-rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/cluster/cosmos/test_cosmos.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:40:54.256503 spetlr-5.1.9/tests/cluster/db/
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/cluster/db/test_db_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:40:54.256503 spetlr-5.1.9/tests/cluster/delta/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:40:54.256503 spetlr-5.1.9/tests/cluster/delta/deltaspec/
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/cluster/delta/deltaspec/test_dbspec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/cluster/delta/deltaspec/test_tblspec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/cluster/delta/test_cleanup_databases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5675 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/cluster/delta/test_delta_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8696 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/cluster/delta/test_delta_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6505 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/cluster/delta/test_filehandle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/cluster/delta/test_sparkexecutor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:40:54.256503 spetlr-5.1.9/tests/cluster/eh/
+-rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/cluster/eh/test_eh_json_orchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4665 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/cluster/eh/test_eh_json_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/cluster/eh/test_eh_saving.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:40:54.260503 spetlr-5.1.9/tests/cluster/etl/
+-rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/cluster/etl/test_checkschemaextractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/cluster/etl/test_delete_data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/cluster/etl/test_deltaupsert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/cluster/etl/test_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9721 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/cluster/etl/test_incremental_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4226 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/cluster/etl/test_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/cluster/etl/test_orchestrator_etl_warning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/cluster/etl/test_simpleloader_upsert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/cluster/etl/test_upsertloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4591 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/cluster/etl/test_upsertloader_streaming.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:40:54.260503 spetlr-5.1.9/tests/cluster/filehandle/
+-rw-r--r--   0 runner    (1001) docker     (127)     5435 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/cluster/filehandle/test_filehandle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:40:54.260503 spetlr-5.1.9/tests/cluster/loaders/
+-rw-r--r--   0 runner    (1001) docker     (127)    26466 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/cluster/loaders/test_scd2_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:40:54.260503 spetlr-5.1.9/tests/cluster/reporting/
+-rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/cluster/reporting/test_slack_reporting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:40:54.260503 spetlr-5.1.9/tests/cluster/schema_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/cluster/schema_manager/test_schema_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:40:54.260503 spetlr-5.1.9/tests/cluster/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/cluster/sql/test_deliveryexecutor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12751 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/cluster/sql/test_deliverysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/cluster/sql/test_deliverysqlspn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/cluster/sql/test_simple_sql_etl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/cluster/sql/test_sql_streaming.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5516 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/cluster/sql/test_sqlhandle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:40:54.260503 spetlr-5.1.9/tests/cluster/transformations/
+-rw-r--r--   0 runner    (1001) docker     (127)     6530 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/cluster/transformations/test_merge_df_into_target.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/cluster/transformations/test_simple_sql_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/cluster/transformations/test_union_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:40:54.264503 spetlr-5.1.9/tests/cluster/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/cluster/utils/test_delete_schema_mismatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/cluster/utils/test_spark_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/cluster/utils/test_stop_test_stream.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:40:54.264503 spetlr-5.1.9/tests/local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:40:54.264503 spetlr-5.1.9/tests/local/azure_log_analytics/
+-rw-r--r--   0 runner    (1001) docker     (127)     4799 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/local/azure_log_analytics/test_azure_log_analytics_handle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:40:54.264503 spetlr-5.1.9/tests/local/configurator/
+-rw-r--r--   0 runner    (1001) docker     (127)     9658 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/local/configurator/test_configurator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/local/configurator/test_configurator_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:40:54.264503 spetlr-5.1.9/tests/local/delta/
+-rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/local/delta/test_DeltaDatabaseSpec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12308 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/local/delta/test_DeltaTableSpec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/local/delta/test_table_name.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:40:54.264503 spetlr-5.1.9/tests/local/eh/
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/local/eh/test_EventHubCaptureExtractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4618 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/local/eh/test_ehto_bronze_and_silver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/local/eh/test_ehtodeltabronze_orchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/local/eh/test_ehtodeltabronze_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7356 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/local/eh/test_ehtodeltasilver_orchestrator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:40:54.264503 spetlr-5.1.9/tests/local/entry_points/
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/local/entry_points/test_generalized_entry_points.py
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/local/entry_points/test_task_entry_point.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:40:54.264503 spetlr-5.1.9/tests/local/etl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:40:54.268503 spetlr-5.1.9/tests/local/etl/log/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:40:54.268503 spetlr-5.1.9/tests/local/etl/log/log_transformers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/local/etl/log/log_transformers/test_count_log_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/local/etl/log/log_transformers/test_null_log_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/local/etl/log/test_log_orchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/local/etl/log/test_log_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/local/etl/test_lazy_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/local/etl/test_orchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/local/etl/test_simple_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11196 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/local/etl/test_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:40:54.268503 spetlr-5.1.9/tests/local/extractors/
+-rw-r--r--   0 runner    (1001) docker     (127)     4547 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/local/extractors/test_eventhub_stream_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:40:54.268503 spetlr-5.1.9/tests/local/filehandle/
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/local/filehandle/test_filehandle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:40:54.268503 spetlr-5.1.9/tests/local/power_bi/
+-rw-r--r--   0 runner    (1001) docker     (127)    59963 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/local/power_bi/test_power_bi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5152 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/local/power_bi/test_spark_pandas_dataframe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:40:54.268503 spetlr-5.1.9/tests/local/reporting/
+-rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/local/reporting/test_slack_reporting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:40:54.268503 spetlr-5.1.9/tests/local/repr/
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/local/repr/test_repr_sql_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:40:54.268503 spetlr-5.1.9/tests/local/schema_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/local/schema_manager/test_schema_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:40:54.268503 spetlr-5.1.9/tests/local/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/local/sql/test_SqlExecutor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:40:54.268503 spetlr-5.1.9/tests/local/streaming/
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/local/streaming/test_deltahandle_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/local/streaming/test_stream_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/local/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/local/test_get_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/local/test_spark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5543 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/local/test_sqlServer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6193 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/local/test_transformations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:40:54.272503 spetlr-5.1.9/tests/local/transformers/
+-rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/local/transformers/test_clean_column_names_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8391 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/local/transformers/test_concat_df.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/local/transformers/test_country_to_alphacode_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4547 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/local/transformers/test_data_change_capture_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/local/transformers/test_drop_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/local/transformers/test_dropoldestduplicates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/local/transformers/test_fuzzy_select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/local/transformers/test_generate_md5_column_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13371 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/local/transformers/test_join_dataframes_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/local/transformers/test_select_and_cast_columns_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/local/transformers/test_select_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/local/transformers/test_simple_dataframe_filter_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/local/transformers/test_timezone_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4704 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/local/transformers/test_union_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/local/transformers/test_validfromto_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:40:54.272503 spetlr-5.1.9/tests/local/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/local/utils/test_cleandatabases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/local/utils/test_dataframe_creation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/local/utils/test_dropoldestduplicates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/local/utils/test_getmergestatement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/local/utils/test_md5_hashcolumn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/local/utils/test_mock_etl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5916 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/local/utils/test_selectandcastcolumns.py
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-21 11:40:40.000000 spetlr-5.1.9/tests/local/utils/test_stop_test_streams.py
```

### Comparing `spetlr-5.1.6/LICENSE` & `spetlr-5.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/PKG-INFO` & `spetlr-5.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spetlr
-Version: 5.1.6
+Version: 5.1.9
 Summary: A python ETL libRary (SPETLR) for Databricks powered by Apache SPark.
 Home-page: https://github.com/spetlr-org/spetlr
 Author: Spetlr.Org
 Author-email: spetlr.org@gmail.com
 License: UNKNOWN
 Project-URL: Documentation, https://github.com/spetlr-org/spetlr
 Project-URL: Bug Reports, https://github.com/spetlr-org/spetlr/issues
```

### Comparing `spetlr-5.1.6/README.md` & `spetlr-5.1.9/README.md`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/setup.cfg` & `spetlr-5.1.9/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -27,52 +27,30 @@
 python_requires = >=3.8
 zip_safe = False
 include_package_data = True
 package_dir = 
 	=src
 packages = find:
 install_requires = 
-	azure-core==1.30.0
-	azure-cosmos==4.5.1
-	cachetools==5.3.3
-	certifi==2024.2.2
-	cffi==1.16.0
-	charset-normalizer==3.3.2
-	cryptography==42.0.5
-	databricks-sdk==0.20.0
-	Deprecated==1.2.14
-	google-auth==2.28.1
-	h3==3.7.6
-	idna==3.6
-	importlib-metadata==7.0.1
-	importlib-resources==5.13.0
-	more-itertools==10.2.0
-	msal==1.27.0
-	numpy==1.24.0
-	pandas==2.0.3
-	pyasn1==0.5.1
-	pyasn1-modules==0.3.0
-	pycountry==23.12.11
-	pycparser==2.21
-	PyJWT==2.8.0
-	pyodbc==5.1.0
-	python-dateutil==2.8.2
-	pytz==2024.1
-	PyYAML==6.0.1
-	requests==2.31.0
-	rsa==4.9
-	setuptools==49.2.1
-	six==1.16.0
-	sqlparse==0.4.4
+	pyyaml
+	sqlparse>=0.4.4
+	Deprecated
+	pyodbc
+	importlib-metadata
+	azure-cosmos
 	timezonefinder==6.0.2
-	typing_extensions==4.10.0
-	tzdata==2024.1
-	urllib3==1.26.16
-	wrapt==1.16.0
-	zipp==3.17.0
+	more_itertools
+	pycountry
+	databricks-sdk
+	numpy<=1.24;python_version<="3.8"
+	numpy;python_version>"3.8"
+	urllib3==1.26.16;python_version<="3.8" # follows numpy
+	urllib3;python_version>"3.8" # follows numpy
+	msal
+	pandas
 
 [options.packages.find]
 where = src
 
 [options.entry_points]
 console_scripts = 
 	python3 = spetlr.alias:python3
```

### Comparing `spetlr-5.1.6/src/spetlr/azure_log_analytics/azure_log_analytics_handle.py` & `spetlr-5.1.9/src/spetlr/azure_log_analytics/azure_log_analytics_handle.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/cache/CachedLoader.py` & `spetlr-5.1.9/src/spetlr/cache/CachedLoader.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/cache/CachedLoaderParameters.py` & `spetlr-5.1.9/src/spetlr/cache/CachedLoaderParameters.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/configurator/_cli/ConfiguratorCli.py` & `spetlr-5.1.9/src/spetlr/configurator/_cli/ConfiguratorCli.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/configurator/_cli/generate_keys_file.py` & `spetlr-5.1.9/src/spetlr/configurator/_cli/generate_keys_file.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/configurator/configurator.py` & `spetlr-5.1.9/src/spetlr/configurator/configurator.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/configurator/sql/StatementBlocks.py` & `spetlr-5.1.9/src/spetlr/configurator/sql/StatementBlocks.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/configurator/sql/comments.py` & `spetlr-5.1.9/src/spetlr/configurator/sql/comments.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/configurator/sql/create.py` & `spetlr-5.1.9/src/spetlr/configurator/sql/create.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/configurator/sql/db.py` & `spetlr-5.1.9/src/spetlr/configurator/sql/db.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/configurator/sql/init_sqlparse.py` & `spetlr-5.1.9/src/spetlr/configurator/sql/init_sqlparse.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/configurator/sql/parse_sql.py` & `spetlr-5.1.9/src/spetlr/configurator/sql/parse_sql.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/configurator/sql/substructures.py` & `spetlr-5.1.9/src/spetlr/configurator/sql/substructures.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/configurator/sql/table.py` & `spetlr-5.1.9/src/spetlr/configurator/sql/table.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/configurator/sql/view.py` & `spetlr-5.1.9/src/spetlr/configurator/sql/view.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/cosmos/cosmos.py` & `spetlr-5.1.9/src/spetlr/cosmos/cosmos.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/cosmos/cosmos_base_server.py` & `spetlr-5.1.9/src/spetlr/cosmos/cosmos_base_server.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/cosmos/cosmos_handle.py` & `spetlr-5.1.9/src/spetlr/cosmos/cosmos_handle.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/db_auto.py` & `spetlr-5.1.9/src/spetlr/db_auto.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/delta/db_handle.py` & `spetlr-5.1.9/src/spetlr/delta/db_handle.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/delta/delta_handle.py` & `spetlr-5.1.9/src/spetlr/delta/delta_handle.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/deltaspec/DeltaDatabaseSpec.py` & `spetlr-5.1.9/src/spetlr/deltaspec/DeltaDatabaseSpec.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/deltaspec/DeltaTableSpec.py` & `spetlr-5.1.9/src/spetlr/deltaspec/DeltaTableSpec.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/deltaspec/DeltaTableSpecBase.py` & `spetlr-5.1.9/src/spetlr/deltaspec/DeltaTableSpecBase.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/deltaspec/DeltaTableSpecDifference.py` & `spetlr-5.1.9/src/spetlr/deltaspec/DeltaTableSpecDifference.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/deltaspec/__init__.py` & `spetlr-5.1.9/src/spetlr/deltaspec/__init__.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/deltaspec/exceptions.py` & `spetlr-5.1.9/src/spetlr/deltaspec/exceptions.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/deltaspec/helpers.py` & `spetlr-5.1.9/src/spetlr/deltaspec/helpers.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/eh/EventHubCapture.py` & `spetlr-5.1.9/src/spetlr/eh/EventHubCapture.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/eh/EventHubCaptureExtractor.py` & `spetlr-5.1.9/src/spetlr/eh/EventHubCaptureExtractor.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/eh/EventHubJsonPublisher.py` & `spetlr-5.1.9/src/spetlr/eh/EventHubJsonPublisher.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/eh/EventHubStream.py` & `spetlr-5.1.9/src/spetlr/eh/EventHubStream.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/eh/PartitionSpec.py` & `spetlr-5.1.9/src/spetlr/eh/PartitionSpec.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/entry_points/generalized_task_entry_point.py` & `spetlr-5.1.9/src/spetlr/entry_points/generalized_task_entry_point.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/entry_points/task_entry_point.py` & `spetlr-5.1.9/src/spetlr/entry_points/task_entry_point.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/etl/extractor.py` & `spetlr-5.1.9/src/spetlr/etl/extractor.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/etl/extractors/__init__.py` & `spetlr-5.1.9/src/spetlr/etl/extractors/__init__.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/etl/extractors/check_schema_extractor.py` & `spetlr-5.1.9/src/spetlr/etl/extractors/check_schema_extractor.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/etl/extractors/incremental_extractor.py` & `spetlr-5.1.9/src/spetlr/etl/extractors/incremental_extractor.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/etl/extractors/lazy_extractor.py` & `spetlr-5.1.9/src/spetlr/etl/extractors/lazy_extractor.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/etl/extractors/lazy_simple_extractor.py` & `spetlr-5.1.9/src/spetlr/etl/extractors/lazy_simple_extractor.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/etl/extractors/schema_extractor.py` & `spetlr-5.1.9/src/spetlr/etl/extractors/schema_extractor.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/etl/loader.py` & `spetlr-5.1.9/src/spetlr/etl/loader.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/etl/loaders/DeleteDataLoader.py` & `spetlr-5.1.9/src/spetlr/etl/loaders/DeleteDataLoader.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/etl/loaders/UpsertLoader.py` & `spetlr-5.1.9/src/spetlr/etl/loaders/UpsertLoader.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/etl/loaders/scd2_loader.py` & `spetlr-5.1.9/src/spetlr/etl/loaders/scd2_loader.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/etl/loaders/simple_loader.py` & `spetlr-5.1.9/src/spetlr/etl/loaders/simple_loader.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/etl/loaders/stream_loader.py` & `spetlr-5.1.9/src/spetlr/etl/loaders/stream_loader.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/etl/loaders/upsert_loader_streaming.py` & `spetlr-5.1.9/src/spetlr/etl/loaders/upsert_loader_streaming.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/etl/log/log_orchestrator.py` & `spetlr-5.1.9/src/spetlr/etl/log/log_orchestrator.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/etl/log/log_transformer.py` & `spetlr-5.1.9/src/spetlr/etl/log/log_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/etl/log/log_transformers/count_log_transformer.py` & `spetlr-5.1.9/src/spetlr/etl/log/log_transformers/count_log_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/etl/log/log_transformers/null_log_transformer.py` & `spetlr-5.1.9/src/spetlr/etl/log/log_transformers/null_log_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/etl/orchestrator.py` & `spetlr-5.1.9/src/spetlr/etl/orchestrator.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/etl/transformer.py` & `spetlr-5.1.9/src/spetlr/etl/transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/etl/transformers/SimpleSqlTransformer.py` & `spetlr-5.1.9/src/spetlr/etl/transformers/SimpleSqlTransformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/etl/transformers/__init__.py` & `spetlr-5.1.9/src/spetlr/etl/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/etl/transformers/clean_column_names_transformer.py` & `spetlr-5.1.9/src/spetlr/etl/transformers/clean_column_names_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/etl/transformers/country_to_alphacode_transformer.py` & `spetlr-5.1.9/src/spetlr/etl/transformers/country_to_alphacode_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/etl/transformers/data_change_capture_transformer.py` & `spetlr-5.1.9/src/spetlr/etl/transformers/data_change_capture_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/etl/transformers/dropColumnsTransformer.py` & `spetlr-5.1.9/src/spetlr/etl/transformers/dropColumnsTransformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/etl/transformers/drop_oldest_duplicate_transformer.py` & `spetlr-5.1.9/src/spetlr/etl/transformers/drop_oldest_duplicate_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/etl/transformers/fuzzy_select.py` & `spetlr-5.1.9/src/spetlr/etl/transformers/fuzzy_select.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/etl/transformers/generate_md5_column_transformer.py` & `spetlr-5.1.9/src/spetlr/etl/transformers/generate_md5_column_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/etl/transformers/join_dataframes_transformer.py` & `spetlr-5.1.9/src/spetlr/etl/transformers/join_dataframes_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/etl/transformers/selectColumnsTransformer.py` & `spetlr-5.1.9/src/spetlr/etl/transformers/selectColumnsTransformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/etl/transformers/select_and_cast_columns_transformer.py` & `spetlr-5.1.9/src/spetlr/etl/transformers/select_and_cast_columns_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/etl/transformers/simple_dataframe_filter_transformer.py` & `spetlr-5.1.9/src/spetlr/etl/transformers/simple_dataframe_filter_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/etl/transformers/simple_sql_transformer.py` & `spetlr-5.1.9/src/spetlr/etl/transformers/simple_sql_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/etl/transformers/timezone_transformer.py` & `spetlr-5.1.9/src/spetlr/etl/transformers/timezone_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/etl/transformers/union_transformer.py` & `spetlr-5.1.9/src/spetlr/etl/transformers/union_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/etl/transformers/validfromto_transformer.py` & `spetlr-5.1.9/src/spetlr/etl/transformers/validfromto_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/exceptions/__init__.py` & `spetlr-5.1.9/src/spetlr/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/extractors/eventhub_stream_extractor.py` & `spetlr-5.1.9/src/spetlr/extractors/eventhub_stream_extractor.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/filehandle/file_handle.py` & `spetlr-5.1.9/src/spetlr/filehandle/file_handle.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/formatting/git_hooks.py` & `spetlr-5.1.9/src/spetlr/formatting/git_hooks.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/functions.py` & `spetlr-5.1.9/src/spetlr/functions.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/mount/main.py` & `spetlr-5.1.9/src/spetlr/mount/main.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/orchestrators/eh2bronze/EhToDeltaBronzeOrchestrator.py` & `spetlr-5.1.9/src/spetlr/orchestrators/eh2bronze/EhToDeltaBronzeOrchestrator.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/orchestrators/eh2bronze/EhToDeltaBronzeTransformer.py` & `spetlr-5.1.9/src/spetlr/orchestrators/eh2bronze/EhToDeltaBronzeTransformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/orchestrators/eh2silver/EhToDeltaSilverOrchestrator.py` & `spetlr-5.1.9/src/spetlr/orchestrators/eh2silver/EhToDeltaSilverOrchestrator.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/orchestrators/ehjson2delta/EhJsonToDeltaExtractor.py` & `spetlr-5.1.9/src/spetlr/orchestrators/ehjson2delta/EhJsonToDeltaExtractor.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/orchestrators/ehjson2delta/EhJsonToDeltaOrchestrator.py` & `spetlr-5.1.9/src/spetlr/orchestrators/ehjson2delta/EhJsonToDeltaOrchestrator.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/orchestrators/ehjson2delta/EhJsonToDeltaTransformer.py` & `spetlr-5.1.9/src/spetlr/orchestrators/ehjson2delta/EhJsonToDeltaTransformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/power_bi/PowerBi.py` & `spetlr-5.1.9/src/spetlr/power_bi/PowerBi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import time
 from datetime import datetime, timedelta
-from typing import Callable, Dict, List, Tuple, Union
+from typing import Callable, Dict, List, Optional, Tuple
 
 import msal
 import pandas as pd
 import requests
 from pyspark.sql import DataFrame
 from pytz import utc
 
@@ -226,15 +226,15 @@
 
         self.api_header = {
             "Content-Type": "application/json",
             "Authorization": f"Bearer {access_token}",
         }
         return True
 
-    def _get_workspaces(self) -> Union[SparkPandasDataFrame, None]:
+    def _get_workspaces(self) -> Optional[SparkPandasDataFrame]:
         """
         Returns the list of available PowerBI workspaces.
 
         :return: data frame with workspaces if succeeded,
             or None if failed (when ignore_errors==True)
         :rtype: SparkPandas data frame
         :raises PowerBiException: if failed and ignore_errors==False
@@ -261,15 +261,15 @@
                 ],
                 indexing_columns="id",
                 sorting_columns="name",
             )
         self._raise_base_api_error("Failed to fetch workspaces!", api_call)
         return None
 
-    def _get_datasets(self, workspace_id: str) -> Union[SparkPandasDataFrame, None]:
+    def _get_datasets(self, workspace_id: str) -> Optional[SparkPandasDataFrame]:
         """
         Returns the list of available PowerBI datasets.
 
         :param str workspace_id: the id of the workspace to fetch
         :return: data frame with datasets if succeeded,
             or None if failed (when ignore_errors==True)
         :rtype: SparkPandas data frame
@@ -309,15 +309,15 @@
         return None
 
     def _get_refresh_history(
         self,
         workspace_id: str,
         dataset_id: str,
         ignore_unauthorized: bool = False,
-    ) -> Union[SparkPandasDataFrame, None]:
+    ) -> Optional[SparkPandasDataFrame]:
         """
         Returns the PowerBI dataset refresh history for the specified dataset.
 
         :param str workspace_id: the id of the workspace
         :param str dataset_id: the id of the dataset
         :param bool ignore_unauthorized: return None on HTTP 401 Unauthorized
         :return: data frame with the refresh history if succeeded,
@@ -363,15 +363,15 @@
 
     def _get_refresh_history_details(
         self,
         workspace_id: str,
         dataset_id: str,
         request_id: str,
         ignore_unauthorized: bool = False,
-    ) -> Union[SparkPandasDataFrame, None]:
+    ) -> Optional[SparkPandasDataFrame]:
         """
         Returns the PowerBI dataset refresh history details for the specified refresh.
 
         :param str workspace_id: the id of the workspace
         :param str dataset_id: the id of the dataset
         :param str request_id: the id of the refresh request
         :param bool ignore_unauthorized: return None on HTTP 401 Unauthorized
@@ -409,15 +409,15 @@
         return None
 
     def _get_partition_tables(
         self,
         workspace_id: str,
         dataset_id: str,
         ignore_unauthorized: bool = False,
-    ) -> Union[SparkPandasDataFrame, None]:
+    ) -> Optional[SparkPandasDataFrame]:
         """
         Returns the PowerBI dataset partition info with table names
         and their refresh times.
 
         :param str workspace_id: the id of the workspace
         :param str dataset_id: the id of the dataset
         :param bool ignore_unauthorized: return None on HTTP 401 Unauthorized
@@ -605,15 +605,15 @@
 
         return True
 
     def _connect_and_get_workspaces(
         self,
         *,
         skip_read_only: bool = False,
-    ) -> Union[List[Tuple[str, str]], None]:
+    ) -> Optional[List[Tuple[str, str]]]:
         """
         Connects or reconnects to the PowerBI API and returns a list of
         workspace id's and names.
 
         :param bool skip_read_only: True to exclude read-only workspaces.
         :rtype: SparkPandas data frame
         :raises PowerBiException: if failed and ignore_errors==False
@@ -640,15 +640,15 @@
             workspace_list = [
                 (df.WorkspaceId, df.WorkspaceName)
                 for _, df in workspaces.get_pandas_df().iterrows()
                 if not (skip_read_only and df.IsReadOnly)
             ]
         return workspace_list
 
-    def _combine_datasets(self) -> Union[SparkPandasDataFrame, None]:
+    def _combine_datasets(self) -> Optional[SparkPandasDataFrame]:
         """
         Returns a list of PowerBI datasets for a single workspace or
         combined lists for datasets from all workspaces.
 
         :return: data frame with PowerBI datasets if succeeded,
             or None if failed (when ignore_errors==True)
         :rtype: SparkPandas data frame
@@ -669,20 +669,20 @@
             suffix_columns = [("WorkspaceId", workspace_id, "string")]
             result = datasets.append(result, prefix_columns, suffix_columns)
 
         return result
 
     def _combine_dataframes(
         self,
-        function: Callable[[str, str, bool], Union[SparkPandasDataFrame, None]],
+        function: Callable[[str, str, bool], Optional[SparkPandasDataFrame]],
         *,
         skip_read_only: bool = False,
         skip_not_refreshable: bool = False,
         skip_effective_identity: bool = False,
-    ) -> Union[SparkPandasDataFrame, None]:
+    ) -> Optional[SparkPandasDataFrame]:
         """
         Returns a single data frame loaded from PowerBI, or the same
         combined data frame fetched from all workspaces and datasets.
 
         :param callable function: The function that returns the data frame
         :param bool skip_read_only: True to exclude read-only workspaces.
         :param bool skip_not_refreshable: True to exclude PowerBI datasets
@@ -855,18 +855,19 @@
                             self.last_status = "Failed"
                             self.last_exception = df.ErrorMessage.iloc[0]
                             self.table_name = df.TableName.iloc[0]
                             return True
                         else:
                             df = tables.get_pandas_df()
                             df = df[df.TableName.isin(self.table_names)]
-                            column = "RefreshTime" + tables.time_column_suffix
-                            idx = df[column].idxmin()
-                            self.table_name = df.TableName.loc[idx]
-                            refresh_time = df[column].loc[idx]
+                            if not df.empty:
+                                column = "RefreshTime" + tables.time_column_suffix
+                                idx = df[column].idxmin()
+                                self.table_name = df.TableName.loc[idx]
+                                refresh_time = df[column].loc[idx]
 
                 self.last_refresh_utc = history.get_utc_time(refresh_time)
                 self.last_refresh_str = history.get_local_time_str(refresh_time)
 
         return True
 
     def _verify_last_refresh(self) -> bool:
@@ -931,15 +932,15 @@
             self._raise_error(
                 f"Unknown refresh status: {self.last_status}! {self.last_exception}"
             )
         return False
 
     def _get_refresh_argument_json(
         self, with_wait: bool
-    ) -> Union[Dict[str, object], None]:
+    ) -> Optional[Dict[str, object]]:
         """
         Returns the HTTP body of the PowerBI refresh API call
         containing table names to refresh or other parameters if necessary.
 
         :param bool with_wait: True if we need to wait for the refresh to finish.
         :rtype: JSON object or None
         """
@@ -987,14 +988,15 @@
                 f"/datasets/{self.dataset_id}/refreshes"
             )
             api_call = requests.post(
                 url=api_url, headers=self.api_header, json=post_body
             )
             if api_call.status_code == 202:
                 print("A new refresh has been successfully triggered.")
+                self.last_status = "Unknown"
                 return True
             else:
                 self._raise_api_error(
                     "Failed to trigger a refresh!",
                     api_call,
                     post_body=str(post_body),
                     workspace_id=self.workspace_id,
@@ -1078,17 +1080,19 @@
         :return: True if succeeded or False if failed (when ignore_errors==True)
         :rtype: bool
         :raises PowerBiException: if failed and ignore_errors==False
         """
 
         retries = self.number_of_retries
         start_time = time.time()
-        if not (self._get_last_refresh() and self._trigger_new_refresh()):
+        if not self._get_last_refresh():
+            return False
+        restart = self.last_status == "Unknown" and self.is_enhanced
+        if not self._trigger_new_refresh():
             return False
-        restart = self.is_enhanced
 
         while True:
             elapsed_seconds = int(time.time() - start_time)
             if elapsed_seconds >= self.timeout_in_seconds:
                 print("Timeout!")
                 break
             wait_seconds = self._get_seconds_to_wait(elapsed_seconds)
@@ -1100,15 +1104,14 @@
 
             if (self.last_status == "Failed" and retries > 0) or (
                 self.last_status == "Completed" and restart
             ):
                 if not restart:
                     retries = retries - 1
                 restart = False
-                self.last_status = "Unknown"
                 if not self._trigger_new_refresh():
                     return False
                 continue
 
             if self.last_status != "Unknown":
                 break
 
@@ -1124,15 +1127,15 @@
 
         history = self._combine_dataframes(
             self._get_refresh_history, skip_read_only=True, skip_not_refreshable=True
         )
         if history is not None:
             history.show("Refresh history:", "The refresh history is empty.")
 
-    def get_history(self) -> Union[DataFrame, None]:
+    def get_history(self) -> Optional[DataFrame]:
         """
         Returns the refresh history of a PowerBI dataset in a Spark data frame.
 
         :return: the data frame with the refresh history if succeeded,
             or None if failed (when ignore_errors==True)
         :rtype: Spark data frame
         :raises PowerBiException: if failed and ignore_errors==False
@@ -1151,15 +1154,15 @@
         :raises PowerBiException: if failed and ignore_errors==False
         """
 
         details = self._combine_refresh_history_details()
         if details is not None:
             details.show("Refresh history details:", "The refresh history is empty.")
 
-    def get_history_details(self) -> Union[DataFrame, None]:
+    def get_history_details(self) -> Optional[DataFrame]:
         """
         Returns refresh history details of a PowerBI dataset in a Spark data frame.
 
         :return: the data frame with the refresh history details if succeeded,
             or None if failed (when ignore_errors==True)
         :rtype: Spark data frame
         :raises PowerBiException: if failed and ignore_errors==False
@@ -1178,15 +1181,15 @@
 
         tables = self._combine_dataframes(
             self._get_partition_tables, skip_effective_identity=True
         )
         if tables is not None:
             tables.show("Dataset tables:", "No dataset tables found.")
 
-    def get_tables(self) -> Union[DataFrame, None]:
+    def get_tables(self) -> Optional[DataFrame]:
         """
         Returns the tables of a PowerBI dataset as a Spark data frame.
 
         :return: the data frame with the partition tables if succeeded,
             or None if failed (when ignore_errors==True)
         :rtype: Spark data frame
         :raises PowerBiException: if failed and ignore_errors==False
@@ -1206,15 +1209,15 @@
         """
 
         if self._get_access_token():
             workspaces = self._get_workspaces()
             if workspaces is not None:
                 workspaces.show("Workspaces:", "No workspaces found.")
 
-    def get_workspaces(self) -> Union[DataFrame, None]:
+    def get_workspaces(self) -> Optional[DataFrame]:
         """
         Returns the available workspaces as a Spark data frame.
 
         :return: the data frame with the workspaces if succeeded,
             or None if failed (when ignore_errors==True)
         :rtype: Spark data frame
         :raises PowerBiException: if failed and ignore_errors==False
@@ -1233,15 +1236,15 @@
         :raises PowerBiException: if failed and ignore_errors==False
         """
 
         datasets = self._combine_datasets()
         if datasets is not None:
             datasets.show("Datasets:", "No datasets found.")
 
-    def get_datasets(self) -> Union[DataFrame, None]:
+    def get_datasets(self) -> Optional[DataFrame]:
         """
         Returns the available datasets as a Spark data frame.
 
         :return: the data frame with the datasets if succeeded,
             or None if failed (when ignore_errors==True)
         :rtype: Spark data frame
         :raises PowerBiException: if failed and ignore_errors==False
```

### Comparing `spetlr-5.1.6/src/spetlr/power_bi/SparkPandasDataFrame.py` & `spetlr-5.1.9/src/spetlr/power_bi/SparkPandasDataFrame.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from datetime import datetime
-from typing import Callable, Dict, List, Tuple, Union
+from typing import Callable, Dict, List, Optional, Tuple, Union
 
 import numpy as np
 import pandas as pd
 from dateutil.parser import parse
 from pandas.core.generic import NDFrameT
 from pyspark.sql import DataFrame
 from pytz import timezone, utc
@@ -24,16 +24,16 @@
     }
 
     def __init__(
         self,
         json: Union[Dict, List],
         schema: List[Tuple[Union[str, Callable[[pd.DataFrame], NDFrameT]], str, str]],
         *,
-        indexing_columns: Union[int, List[int], str, List[str], None] = None,
-        sorting_columns: Union[int, List[int], str, List[str], None] = None,
+        indexing_columns: Optional[Union[int, List[int], str, List[str]]] = None,
+        sorting_columns: Optional[Union[int, List[int], str, List[str]]] = None,
         ascending: bool = True,
         local_timezone_name: str = None,
     ):
         """
         Provides a class for loading a JSON into Pandas, and for converting
         between Pandas and Spark.
 
@@ -149,15 +149,15 @@
         if not result or (
             isinstance(identifiers, list) and len(result) != len(identifiers)
         ):
             raise PowerBiException(f"{identifiers} column(s) not found in the schema")
         return result if len(result) > 1 else result[0]
 
     @staticmethod
-    def _parse_time(text: str) -> Union[datetime, None]:
+    def _parse_time(text: str) -> Optional[datetime]:
         """
         Parses an ISO 8601 time text and converts it to datetime.
         The result is a timezone-unaware UTC datetime regardless of input.
 
         :param str text: an ISO 8601 time text or None
         :return: timezone-unaware UTC datetime or None
         :rtype: datetime
@@ -170,16 +170,16 @@
             time = utc.localize(time)
         else:
             time = time.astimezone(utc)
         return time.replace(microsecond=0, tzinfo=None)
 
     @staticmethod
     def _localize_time(
-        time: Union[datetime, None], local_timezone_name: str
-    ) -> Union[datetime, None]:
+        time: Optional[datetime], local_timezone_name: str
+    ) -> Optional[datetime]:
         """
         Converts a timezone-unaware UTC datetime to a timezone-unaware local datetime.
 
         :param datetime time: timezone-unaware UTC datetime or None
         :return: timezone-unaware local datetime or None
         :rtype: datetime
         """
@@ -187,25 +187,25 @@
         if time is None or time != time:
             return None
         if time.tzinfo is None or time.tzinfo.utcoffset(time) is None:
             time = utc.localize(time)
         time = time.astimezone(timezone(local_timezone_name))
         return time.replace(tzinfo=None)
 
-    def get_pandas_df(self) -> Union[pd.DataFrame, None]:
+    def get_pandas_df(self) -> Optional[pd.DataFrame]:
         """
         Returns the data frame as a Pandas data frame.
 
         :return: Pandas data frame
         :rtype: Pandas data frame
         """
 
         return self.df
 
-    def get_spark_df(self) -> Union[DataFrame, None]:
+    def get_spark_df(self) -> Optional[DataFrame]:
         """
         Returns the data frame as a Spark data frame.
 
         :return: Spark data frame
         :rtype: Spark data frame
         """
 
@@ -219,15 +219,15 @@
             return Spark.get().createDataFrame(df)
 
     def show(
         self,
         message: str,
         when_empty: str,
         *,
-        filter_columns: Union[List[Tuple[str, str]], None] = None,
+        filter_columns: Optional[List[Tuple[str, str]]] = None,
     ) -> None:
         """
         Displays the Pandas data frame.
 
         :param str message: The message to show when the data frame is not empty.
         :param str when_empty: The message to show when the data frame is empty.
            Note: Pandas fails when showing empty data frames.
@@ -242,29 +242,29 @@
             print(message)
             df = self.df
             if filter_columns:
                 df = df.rename(columns=dict(filter_columns))
                 df = df[[column[1] for column in filter_columns]]
             df.display()
 
-    def get_local_time_str(self, time: datetime) -> Union[str, None]:
+    def get_local_time_str(self, time: datetime) -> Optional[str]:
         """
         Returns the specified time as a local timestamp converted to text.
 
         :param datetime time: the time to convert from
         :return: text of a timezone-aware local datetime or None
         :rtype: str
         """
 
         time_description_suffix = " (UTC)" if self.is_utc else " (local time)"
         if time is not None:
             return time.strftime("%Y-%m-%d %H:%M") + time_description_suffix
         return None
 
-    def get_utc_time(self, time: datetime) -> Union[datetime, None]:
+    def get_utc_time(self, time: datetime) -> Optional[datetime]:
         """
         Returns the specified time as an UTC timestamp.
 
         :param datetime time: the time to convert from
         :return: a timezone-aware UTC datetime or None
         :rtype: datetime
         """
```

### Comparing `spetlr-5.1.6/src/spetlr/reporting/JobReflection.py` & `spetlr-5.1.9/src/spetlr/reporting/JobReflection.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/reporting/SlackNotifier.py` & `spetlr-5.1.9/src/spetlr/reporting/SlackNotifier.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/schema_manager/schema_manager.py` & `spetlr-5.1.9/src/spetlr/schema_manager/schema_manager.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/schema_manager/spark_schema.py` & `spetlr-5.1.9/src/spetlr/schema_manager/spark_schema.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/spark.py` & `spetlr-5.1.9/src/spetlr/spark.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/sql/CommonBaseServer.py` & `spetlr-5.1.9/src/spetlr/sql/CommonBaseServer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/sql/SqlBaseServer.py` & `spetlr-5.1.9/src/spetlr/sql/SqlBaseServer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/sql/SqlExecutor.py` & `spetlr-5.1.9/src/spetlr/sql/SqlExecutor.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/sql/SqlServer.py` & `spetlr-5.1.9/src/spetlr/sql/SqlServer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/sql/sql_handle.py` & `spetlr-5.1.9/src/spetlr/sql/sql_handle.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/sqlrepr/sql_types.py` & `spetlr-5.1.9/src/spetlr/sqlrepr/sql_types.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/tables/TableHandle.py` & `spetlr-5.1.9/src/spetlr/tables/TableHandle.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/testutils/CleanupTestDatabases.py` & `spetlr-5.1.9/src/spetlr/testutils/CleanupTestDatabases.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/testutils/stop_test_streams.py` & `spetlr-5.1.9/src/spetlr/testutils/stop_test_streams.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/transformations.py` & `spetlr-5.1.9/src/spetlr/transformations.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/transformers/__init__.py` & `spetlr-5.1.9/src/spetlr/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/utils/CheckDfMerge.py` & `spetlr-5.1.9/src/spetlr/utils/CheckDfMerge.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/utils/DataframeCreator.py` & `spetlr-5.1.9/src/spetlr/utils/DataframeCreator.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/utils/DeleteMismatchedSchemas.py` & `spetlr-5.1.9/src/spetlr/utils/DeleteMismatchedSchemas.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/utils/DropOldestDuplicates.py` & `spetlr-5.1.9/src/spetlr/utils/DropOldestDuplicates.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/utils/GetMergeStatement.py` & `spetlr-5.1.9/src/spetlr/utils/GetMergeStatement.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/utils/Md5HashColumn.py` & `spetlr-5.1.9/src/spetlr/utils/Md5HashColumn.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/utils/MockLoader.py` & `spetlr-5.1.9/src/spetlr/utils/MockLoader.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/utils/SelectAndCastColumns.py` & `spetlr-5.1.9/src/spetlr/utils/SelectAndCastColumns.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr/utils/__init__.py` & `spetlr-5.1.9/src/spetlr/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/src/spetlr.egg-info/PKG-INFO` & `spetlr-5.1.9/src/spetlr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spetlr
-Version: 5.1.6
+Version: 5.1.9
 Summary: A python ETL libRary (SPETLR) for Databricks powered by Apache SPark.
 Home-page: https://github.com/spetlr-org/spetlr
 Author: Spetlr.Org
 Author-email: spetlr.org@gmail.com
 License: UNKNOWN
 Project-URL: Documentation, https://github.com/spetlr-org/spetlr
 Project-URL: Bug Reports, https://github.com/spetlr-org/spetlr/issues
```

### Comparing `spetlr-5.1.6/src/spetlr.egg-info/SOURCES.txt` & `spetlr-5.1.9/src/spetlr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/cluster/azure_log_analytics/test_azure_log_analytics_handle.py` & `spetlr-5.1.9/tests/cluster/azure_log_analytics/test_azure_log_analytics_handle.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/cluster/cache/test_cache.py` & `spetlr-5.1.9/tests/cluster/cache/test_cache.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/cluster/cosmos/test_cosmos.py` & `spetlr-5.1.9/tests/cluster/cosmos/test_cosmos.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/cluster/delta/deltaspec/test_dbspec.py` & `spetlr-5.1.9/tests/cluster/delta/deltaspec/test_dbspec.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/cluster/delta/deltaspec/test_tblspec.py` & `spetlr-5.1.9/tests/cluster/delta/deltaspec/test_tblspec.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/cluster/delta/test_cleanup_databases.py` & `spetlr-5.1.9/tests/cluster/delta/test_cleanup_databases.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/cluster/delta/test_delta_class.py` & `spetlr-5.1.9/tests/cluster/delta/test_delta_class.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/cluster/delta/test_delta_stream.py` & `spetlr-5.1.9/tests/cluster/delta/test_delta_stream.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/cluster/delta/test_filehandle.py` & `spetlr-5.1.9/tests/cluster/delta/test_filehandle.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/cluster/delta/test_sparkexecutor.py` & `spetlr-5.1.9/tests/cluster/delta/test_sparkexecutor.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/cluster/eh/test_eh_json_orchestrator.py` & `spetlr-5.1.9/tests/cluster/eh/test_eh_json_orchestrator.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/cluster/eh/test_eh_json_transformer.py` & `spetlr-5.1.9/tests/cluster/eh/test_eh_json_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/cluster/eh/test_eh_saving.py` & `spetlr-5.1.9/tests/cluster/eh/test_eh_saving.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/cluster/etl/test_checkschemaextractor.py` & `spetlr-5.1.9/tests/cluster/etl/test_checkschemaextractor.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/cluster/etl/test_delete_data_loader.py` & `spetlr-5.1.9/tests/cluster/etl/test_delete_data_loader.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/cluster/etl/test_deltaupsert.py` & `spetlr-5.1.9/tests/cluster/etl/test_deltaupsert.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/cluster/etl/test_extractor.py` & `spetlr-5.1.9/tests/cluster/etl/test_extractor.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/cluster/etl/test_incremental_extractor.py` & `spetlr-5.1.9/tests/cluster/etl/test_incremental_extractor.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/cluster/etl/test_loader.py` & `spetlr-5.1.9/tests/cluster/etl/test_loader.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/cluster/etl/test_orchestrator_etl_warning.py` & `spetlr-5.1.9/tests/cluster/etl/test_orchestrator_etl_warning.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/cluster/etl/test_simpleloader_upsert.py` & `spetlr-5.1.9/tests/cluster/etl/test_simpleloader_upsert.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/cluster/etl/test_upsertloader.py` & `spetlr-5.1.9/tests/cluster/etl/test_upsertloader.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/cluster/etl/test_upsertloader_streaming.py` & `spetlr-5.1.9/tests/cluster/etl/test_upsertloader_streaming.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/cluster/filehandle/test_filehandle.py` & `spetlr-5.1.9/tests/cluster/filehandle/test_filehandle.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/cluster/loaders/test_scd2_loader.py` & `spetlr-5.1.9/tests/cluster/loaders/test_scd2_loader.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/cluster/reporting/test_slack_reporting.py` & `spetlr-5.1.9/tests/cluster/reporting/test_slack_reporting.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/cluster/schema_manager/test_schema_manager.py` & `spetlr-5.1.9/tests/cluster/schema_manager/test_schema_manager.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/cluster/sql/test_deliveryexecutor.py` & `spetlr-5.1.9/tests/cluster/sql/test_deliveryexecutor.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/cluster/sql/test_deliverysql.py` & `spetlr-5.1.9/tests/cluster/sql/test_deliverysql.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/cluster/sql/test_simple_sql_etl.py` & `spetlr-5.1.9/tests/cluster/sql/test_simple_sql_etl.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/cluster/sql/test_sql_streaming.py` & `spetlr-5.1.9/tests/cluster/sql/test_sql_streaming.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/cluster/sql/test_sqlhandle.py` & `spetlr-5.1.9/tests/cluster/sql/test_sqlhandle.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/cluster/transformations/test_merge_df_into_target.py` & `spetlr-5.1.9/tests/cluster/transformations/test_merge_df_into_target.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/cluster/transformations/test_simple_sql_transformer.py` & `spetlr-5.1.9/tests/cluster/transformations/test_simple_sql_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/cluster/transformations/test_union_transformer.py` & `spetlr-5.1.9/tests/cluster/transformations/test_union_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/cluster/utils/test_delete_schema_mismatch.py` & `spetlr-5.1.9/tests/cluster/utils/test_delete_schema_mismatch.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/cluster/utils/test_spark_version.py` & `spetlr-5.1.9/tests/cluster/utils/test_spark_version.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/cluster/utils/test_stop_test_stream.py` & `spetlr-5.1.9/tests/cluster/utils/test_stop_test_stream.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/local/azure_log_analytics/test_azure_log_analytics_handle.py` & `spetlr-5.1.9/tests/local/azure_log_analytics/test_azure_log_analytics_handle.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/local/configurator/test_configurator.py` & `spetlr-5.1.9/tests/local/configurator/test_configurator.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/local/configurator/test_configurator_cli.py` & `spetlr-5.1.9/tests/local/configurator/test_configurator_cli.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/local/delta/test_DeltaDatabaseSpec.py` & `spetlr-5.1.9/tests/local/delta/test_DeltaDatabaseSpec.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/local/delta/test_DeltaTableSpec.py` & `spetlr-5.1.9/tests/local/delta/test_DeltaTableSpec.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/local/delta/test_table_name.py` & `spetlr-5.1.9/tests/local/delta/test_table_name.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/local/eh/test_EventHubCaptureExtractor.py` & `spetlr-5.1.9/tests/local/eh/test_EventHubCaptureExtractor.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/local/eh/test_ehto_bronze_and_silver.py` & `spetlr-5.1.9/tests/local/eh/test_ehto_bronze_and_silver.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/local/eh/test_ehtodeltabronze_orchestrator.py` & `spetlr-5.1.9/tests/local/eh/test_ehtodeltabronze_orchestrator.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/local/eh/test_ehtodeltabronze_transformer.py` & `spetlr-5.1.9/tests/local/eh/test_ehtodeltabronze_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/local/eh/test_ehtodeltasilver_orchestrator.py` & `spetlr-5.1.9/tests/local/eh/test_ehtodeltasilver_orchestrator.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/local/entry_points/test_generalized_entry_points.py` & `spetlr-5.1.9/tests/local/entry_points/test_generalized_entry_points.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/local/etl/log/log_transformers/test_count_log_transformer.py` & `spetlr-5.1.9/tests/local/etl/log/log_transformers/test_count_log_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/local/etl/log/log_transformers/test_null_log_transformer.py` & `spetlr-5.1.9/tests/local/etl/log/log_transformers/test_null_log_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/local/etl/log/test_log_orchestrator.py` & `spetlr-5.1.9/tests/local/etl/log/test_log_orchestrator.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/local/etl/log/test_log_transformer.py` & `spetlr-5.1.9/tests/local/etl/log/test_log_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/local/etl/test_lazy_extractor.py` & `spetlr-5.1.9/tests/local/etl/test_lazy_extractor.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/local/etl/test_transformer.py` & `spetlr-5.1.9/tests/local/etl/test_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/local/extractors/test_eventhub_stream_extractor.py` & `spetlr-5.1.9/tests/local/extractors/test_eventhub_stream_extractor.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/local/filehandle/test_filehandle.py` & `spetlr-5.1.9/tests/local/filehandle/test_filehandle.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/local/power_bi/test_power_bi.py` & `spetlr-5.1.9/tests/local/power_bi/test_power_bi.py`

 * *Files 5% similar despite different names*

```diff
@@ -1387,15 +1387,15 @@
         # Assert
         self.assertEqual(expected_result, result)
 
     @patch("requests.post")
     def test_refresh_no_restart_no_tables_success(self, mock_post):
         # Arrange
         mock_response = Mock()
-        mock_response.status_code = 401
+        mock_response.status_code = 501  # not called, so the error is irrelevant!
         mock_response.text = "error"
         mock_post.return_value = mock_response
 
         sut = PowerBi(
             PowerBiClient(),
             workspace_id="614850c2-3a5c-4d2d-bcaa-d3f20f32a2e0",
             dataset_id="b1f0a07e-e348-402c-a2b2-11f3e31181ce",
@@ -1419,24 +1419,24 @@
             else:
                 raise ValueError("Called too many times")
             return True
 
         sut._get_last_refresh = get_last_refresh
 
         # Act
-        sut.refresh()
+        sut.refresh()  # No exception!
 
         # Assert
-        # No exception!
+        self.assertFalse(mock_post.called)
 
     @patch("requests.post")
-    def test_refresh_restart_no_tables_failure(self, mock_post):
+    def test_refresh_restart_no_tables_timeout(self, mock_post):
         # Arrange
         mock_response = Mock()
-        mock_response.status_code = 202
+        mock_response.status_code = 202  # called only when restart triggered!
         mock_post.return_value = mock_response
 
         sut = PowerBi(
             PowerBiClient(),
             workspace_id="614850c2-3a5c-4d2d-bcaa-d3f20f32a2e0",
             dataset_id="b1f0a07e-e348-402c-a2b2-11f3e31181ce",
             timeout_in_seconds=1,
@@ -1450,34 +1450,35 @@
             sut.table_name = None
             sut.last_refresh_str = None
             sut.is_enhanced = True
             counter += 1
             if counter == 1:
                 sut.last_status = "Unknown"
             elif counter == 2:
-                sut.last_status = "Completed"
+                sut.last_status = "Completed"  # one restart, then timeout!
                 sut.last_refresh_utc = datetime(2024, 5, 14, 9, 17, tzinfo=utc)
             else:
                 raise ValueError("Called too many times")
             return True
 
         sut._get_last_refresh = get_last_refresh
 
         # Act
         with self.assertRaises(PowerBiException) as context:
             sut.refresh()
 
         # Assert
+        self.assertEqual(1, mock_post.call_count)
         self.assertIn("still in progress", str(context.exception))
 
     @patch("requests.post")
     def test_refresh_no_restart_with_tables_success(self, mock_post):
         # Arrange
         mock_response = Mock()
-        mock_response.status_code = 401
+        mock_response.status_code = 401  # not called, so the error is irrelevant!
         mock_response.text = "error"
         mock_post.return_value = mock_response
 
         sut = PowerBi(
             PowerBiClient(),
             workspace_id="614850c2-3a5c-4d2d-bcaa-d3f20f32a2e0",
             dataset_id="b1f0a07e-e348-402c-a2b2-11f3e31181ce",
@@ -1499,24 +1500,24 @@
             else:
                 raise ValueError("Called too many times")
             return True
 
         sut._get_last_refresh = get_last_refresh
 
         # Act
-        sut.refresh()
+        sut.refresh()  # No exception!
 
         # Assert
-        # No exception!
+        self.assertFalse(mock_post.called)
 
     @patch("requests.post")
-    def test_refresh_restart_with_tables_failure(self, mock_post):
+    def test_refresh_restart_with_tables_timeout(self, mock_post):
         # Arrange
         mock_response = Mock()
-        mock_response.status_code = 202
+        mock_response.status_code = 202  # called only whe restart triggered!
         mock_post.return_value = mock_response
 
         sut = PowerBi(
             PowerBiClient(),
             workspace_id="614850c2-3a5c-4d2d-bcaa-d3f20f32a2e0",
             dataset_id="b1f0a07e-e348-402c-a2b2-11f3e31181ce",
             table_names=["Invoices", "Customers"],
@@ -1531,21 +1532,106 @@
             sut.table_name = None
             sut.last_refresh_str = None
             sut.is_enhanced = True
             counter += 1
             if counter == 1:
                 sut.last_status = "Unknown"
             elif counter == 2:
-                sut.last_status = "Completed"
+                sut.last_status = "Completed"  # one restart, then timeout!
+                sut.last_refresh_utc = datetime(2024, 5, 14, 9, 17, tzinfo=utc)
+            else:
+                raise ValueError("Called too many times")
+            return True
+
+        sut._get_last_refresh = get_last_refresh
+
+        # Act
+        with self.assertRaises(PowerBiException) as context:
+            sut.refresh()
+
+        # Assert
+        self.assertEqual(1, mock_post.call_count)
+        self.assertIn("still in progress", str(context.exception))
+
+    @patch("requests.post")
+    def test_refresh_with_retry_timeout(self, mock_post):
+        # Arrange
+        mock_response = Mock()
+        mock_response.status_code = 202  # called twice, in the beginning and on retry!
+        mock_post.return_value = mock_response
+
+        sut = PowerBi(
+            PowerBiClient(),
+            workspace_id="614850c2-3a5c-4d2d-bcaa-d3f20f32a2e0",
+            dataset_id="b1f0a07e-e348-402c-a2b2-11f3e31181ce",
+            timeout_in_seconds=1,
+            number_of_retries=1,
+        )
+        sut.powerbi_url = "test/"
+        counter = 0
+
+        def get_last_refresh():
+            nonlocal sut, counter
+            sut.table_name = None
+            sut.last_refresh_str = None
+            sut.is_enhanced = True
+            counter += 1
+            if counter == 1:
+                sut.last_status = "Completed"  # refresh triggered
                 sut.last_refresh_utc = datetime(2024, 5, 14, 9, 17, tzinfo=utc)
+            elif counter == 2:
+                sut.last_status = "Failed"  # refresh triggered again, but then timeout!
             else:
                 raise ValueError("Called too many times")
             return True
 
         sut._get_last_refresh = get_last_refresh
 
         # Act
         with self.assertRaises(PowerBiException) as context:
             sut.refresh()
 
         # Assert
+        self.assertEqual(2, mock_post.call_count)
         self.assertIn("still in progress", str(context.exception))
+
+    @patch("requests.post")
+    def test_refresh_not_retry_failure(self, mock_post):
+        # Arrange
+        mock_response = Mock()
+        mock_response.status_code = 202  # called only in the beginning!
+        mock_post.return_value = mock_response
+
+        sut = PowerBi(
+            PowerBiClient(),
+            workspace_id="614850c2-3a5c-4d2d-bcaa-d3f20f32a2e0",
+            dataset_id="b1f0a07e-e348-402c-a2b2-11f3e31181ce",
+            timeout_in_seconds=1,
+            number_of_retries=0,
+        )
+        sut.powerbi_url = "test/"
+        counter = 0
+
+        def get_last_refresh():
+            nonlocal sut, counter
+            sut.table_name = None
+            sut.last_refresh_str = None
+            sut.is_enhanced = True
+            counter += 1
+            if counter == 1:
+                sut.last_status = "Completed"
+                sut.last_refresh_utc = datetime(2024, 5, 14, 9, 17, tzinfo=utc)
+            elif counter == 2:
+                sut.last_status = "Failed"  # the reason of the exception!
+            else:
+                raise ValueError("Called too many times")
+            return True
+
+        sut._get_last_refresh = get_last_refresh
+
+        # Act
+        with self.assertRaises(PowerBiException) as context:
+            sut.refresh()
+
+        # Assert
+        self.assertEqual(1, mock_post.call_count)
+        self.assertIn("Last refresh failed", str(context.exception))
```

### Comparing `spetlr-5.1.6/tests/local/power_bi/test_spark_pandas_dataframe.py` & `spetlr-5.1.9/tests/local/power_bi/test_spark_pandas_dataframe.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/local/reporting/test_slack_reporting.py` & `spetlr-5.1.9/tests/local/reporting/test_slack_reporting.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/local/repr/test_repr_sql_types.py` & `spetlr-5.1.9/tests/local/repr/test_repr_sql_types.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/local/schema_manager/test_schema_manager.py` & `spetlr-5.1.9/tests/local/schema_manager/test_schema_manager.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/local/sql/test_SqlExecutor.py` & `spetlr-5.1.9/tests/local/sql/test_SqlExecutor.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/local/streaming/test_stream_loader.py` & `spetlr-5.1.9/tests/local/streaming/test_stream_loader.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/local/test_functions.py` & `spetlr-5.1.9/tests/local/test_functions.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/local/test_get_schema.py` & `spetlr-5.1.9/tests/local/test_get_schema.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/local/test_sqlServer.py` & `spetlr-5.1.9/tests/local/test_sqlServer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/local/test_transformations.py` & `spetlr-5.1.9/tests/local/test_transformations.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/local/transformers/test_clean_column_names_transformer.py` & `spetlr-5.1.9/tests/local/transformers/test_clean_column_names_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/local/transformers/test_concat_df.py` & `spetlr-5.1.9/tests/local/transformers/test_concat_df.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/local/transformers/test_country_to_alphacode_transformer.py` & `spetlr-5.1.9/tests/local/transformers/test_country_to_alphacode_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/local/transformers/test_data_change_capture_transformer.py` & `spetlr-5.1.9/tests/local/transformers/test_data_change_capture_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/local/transformers/test_drop_columns.py` & `spetlr-5.1.9/tests/local/transformers/test_drop_columns.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/local/transformers/test_dropoldestduplicates.py` & `spetlr-5.1.9/tests/local/transformers/test_dropoldestduplicates.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/local/transformers/test_fuzzy_select.py` & `spetlr-5.1.9/tests/local/transformers/test_fuzzy_select.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/local/transformers/test_generate_md5_column_transformer.py` & `spetlr-5.1.9/tests/local/transformers/test_generate_md5_column_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/local/transformers/test_join_dataframes_transformer.py` & `spetlr-5.1.9/tests/local/transformers/test_join_dataframes_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/local/transformers/test_select_and_cast_columns_transformer.py` & `spetlr-5.1.9/tests/local/transformers/test_select_and_cast_columns_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/local/transformers/test_select_columns.py` & `spetlr-5.1.9/tests/local/transformers/test_select_columns.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/local/transformers/test_simple_dataframe_filter_transformer.py` & `spetlr-5.1.9/tests/local/transformers/test_simple_dataframe_filter_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/local/transformers/test_timezone_transformer.py` & `spetlr-5.1.9/tests/local/transformers/test_timezone_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/local/transformers/test_union_transformer.py` & `spetlr-5.1.9/tests/local/transformers/test_union_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/local/transformers/test_validfromto_transformer.py` & `spetlr-5.1.9/tests/local/transformers/test_validfromto_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/local/utils/test_dataframe_creation.py` & `spetlr-5.1.9/tests/local/utils/test_dataframe_creation.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/local/utils/test_dropoldestduplicates.py` & `spetlr-5.1.9/tests/local/utils/test_dropoldestduplicates.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/local/utils/test_getmergestatement.py` & `spetlr-5.1.9/tests/local/utils/test_getmergestatement.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/local/utils/test_md5_hashcolumn.py` & `spetlr-5.1.9/tests/local/utils/test_md5_hashcolumn.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/local/utils/test_mock_etl.py` & `spetlr-5.1.9/tests/local/utils/test_mock_etl.py`

 * *Files identical despite different names*

### Comparing `spetlr-5.1.6/tests/local/utils/test_selectandcastcolumns.py` & `spetlr-5.1.9/tests/local/utils/test_selectandcastcolumns.py`

 * *Files identical despite different names*

