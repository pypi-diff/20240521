# Comparing `tmp/mleko-4.1.0.tar.gz` & `tmp/mleko-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mleko-4.1.0.tar", max compression
+gzip compressed data, was "mleko-4.2.0.tar", max compression
```

## Comparing `mleko-4.1.0.tar` & `mleko-4.2.0.tar`

### file list

```diff
@@ -1,87 +1,87 @@
--rw-r--r--   0        0        0    10947 2024-05-18 16:27:42.343222 mleko-4.1.0/LICENSE
--rw-r--r--   0        0        0     5019 2024-05-18 16:27:42.343222 mleko-4.1.0/README.md
--rw-r--r--   0        0        0     1976 2024-05-18 16:28:13.179034 mleko-4.1.0/mleko/__init__.py
--rw-r--r--   0        0        0      585 2024-05-18 16:27:42.343222 mleko-4.1.0/mleko/cache/__init__.py
--rw-r--r--   0        0        0    16986 2024-05-18 16:27:42.343222 mleko-4.1.0/mleko/cache/cache_mixin.py
--rw-r--r--   0        0        0     1560 2024-05-18 16:27:42.343222 mleko-4.1.0/mleko/cache/fingerprinters/__init__.py
--rw-r--r--   0        0        0     1168 2024-05-18 16:27:42.343222 mleko-4.1.0/mleko/cache/fingerprinters/base_fingerprinter.py
--rw-r--r--   0        0        0     1012 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/cache/fingerprinters/callable_source_fingerprinter.py
--rw-r--r--   0        0        0     2989 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/cache/fingerprinters/csv_fingerprinter.py
--rw-r--r--   0        0        0     1248 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/cache/fingerprinters/json_fingerprinter.py
--rw-r--r--   0        0        0     5578 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/cache/fingerprinters/optuna_pruner_fingerprinter.py
--rw-r--r--   0        0        0    14262 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/cache/fingerprinters/optuna_sampler_fingerprinter.py
--rw-r--r--   0        0        0     1219 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/cache/fingerprinters/vaex_fingerprinter.py
--rw-r--r--   0        0        0     1832 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/cache/handlers/__init__.py
--rw-r--r--   0        0        0      650 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/cache/handlers/base_cache_handler.py
--rw-r--r--   0        0        0     1102 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/cache/handlers/joblib_cache_handler.py
--rw-r--r--   0        0        0     1251 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/cache/handlers/json_cache_handler.py
--rw-r--r--   0        0        0     1196 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/cache/handlers/pickle_cache_handler.py
--rw-r--r--   0        0        0     1207 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/cache/handlers/string_cache_handler.py
--rw-r--r--   0        0        0     1954 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/cache/handlers/vaex_cache_handler.py
--rw-r--r--   0        0        0     8312 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/cache/lru_cache_mixin.py
--rw-r--r--   0        0        0      805 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/dataset/__init__.py
--rw-r--r--   0        0        0      492 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/dataset/convert/__init__.py
--rw-r--r--   0        0        0     1613 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/dataset/convert/base_converter.py
--rw-r--r--   0        0        0    15248 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/dataset/convert/csv_to_vaex_converter.py
--rw-r--r--   0        0        0     6592 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/dataset/data_schema.py
--rw-r--r--   0        0        0      774 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/dataset/export/__init__.py
--rw-r--r--   0        0        0      900 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/dataset/export/base_exporter.py
--rw-r--r--   0        0        0     8725 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/dataset/export/local_exporter.py
--rw-r--r--   0        0        0     8191 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/dataset/export/s3_exporter.py
--rw-r--r--   0        0        0     1614 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/dataset/feature_select/__init__.py
--rw-r--r--   0        0        0    11612 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/dataset/feature_select/base_feature_selector.py
--rw-r--r--   0        0        0     7661 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/dataset/feature_select/composite_feature_selector.py
--rw-r--r--   0        0        0     5156 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/dataset/feature_select/invariance_feature_selector.py
--rw-r--r--   0        0        0     5439 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/dataset/feature_select/missing_rate_feature_selector.py
--rw-r--r--   0        0        0     7257 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/dataset/feature_select/pearson_correlation_feature_selector.py
--rw-r--r--   0        0        0     5803 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/dataset/feature_select/variance_feature_selector.py
--rw-r--r--   0        0        0      569 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/dataset/filter/__init__.py
--rw-r--r--   0        0        0     1615 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/dataset/filter/base_filter.py
--rw-r--r--   0        0        0     3927 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/dataset/filter/expression_filter.py
--rw-r--r--   0        0        0     7160 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/dataset/filter/imblearn_resampling_filter.py
--rw-r--r--   0        0        0      878 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/dataset/ingest/__init__.py
--rw-r--r--   0        0        0     2747 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/dataset/ingest/base_ingester.py
--rw-r--r--   0        0        0    20020 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/dataset/ingest/kaggle_ingester.py
--rw-r--r--   0        0        0    11181 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/dataset/ingest/s3_ingester.py
--rw-r--r--   0        0        0      680 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/dataset/split/__init__.py
--rw-r--r--   0        0        0     1501 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/dataset/split/base_splitter.py
--rw-r--r--   0        0        0     4254 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/dataset/split/expression_splitter.py
--rw-r--r--   0        0        0     7029 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/dataset/split/random_splitter.py
--rw-r--r--   0        0        0     1797 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/dataset/transform/__init__.py
--rw-r--r--   0        0        0     9362 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/dataset/transform/base_transformer.py
--rw-r--r--   0        0        0     6882 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/dataset/transform/composite_transformer.py
--rw-r--r--   0        0        0     4701 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/dataset/transform/expression_transformer.py
--rw-r--r--   0        0        0     4743 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/dataset/transform/frequency_encoder_transformer.py
--rw-r--r--   0        0        0    11533 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/dataset/transform/label_encoder_transformer.py
--rw-r--r--   0        0        0     3744 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/dataset/transform/max_abs_scaler_transformer.py
--rw-r--r--   0        0        0     4150 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/dataset/transform/min_max_scaler_transformer.py
--rw-r--r--   0        0        0      388 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/model/__init__.py
--rw-r--r--   0        0        0    18964 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/model/base_model.py
--rw-r--r--   0        0        0    10756 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/model/lgbm_model.py
--rw-r--r--   0        0        0      413 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/model/tune/__init__.py
--rw-r--r--   0        0        0     3785 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/model/tune/base_tuner.py
--rw-r--r--   0        0        0    17012 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/model/tune/optuna_tuner.py
--rw-r--r--   0        0        0      645 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/pipeline/__init__.py
--rw-r--r--   0        0        0     1382 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/pipeline/data_container.py
--rw-r--r--   0        0        0     4658 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/pipeline/pipeline.py
--rw-r--r--   0        0        0     9807 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/pipeline/pipeline_step.py
--rw-r--r--   0        0        0      928 2024-05-18 16:27:42.351222 mleko-4.1.0/mleko/pipeline/steps/__init__.py
--rw-r--r--   0        0        0     3931 2024-05-18 16:27:42.351222 mleko-4.1.0/mleko/pipeline/steps/convert_step.py
--rw-r--r--   0        0        0     3312 2024-05-18 16:27:42.351222 mleko-4.1.0/mleko/pipeline/steps/export_step.py
--rw-r--r--   0        0        0     6310 2024-05-18 16:27:42.351222 mleko-4.1.0/mleko/pipeline/steps/feature_select_step.py
--rw-r--r--   0        0        0     3115 2024-05-18 16:27:42.351222 mleko-4.1.0/mleko/pipeline/steps/filter_step.py
--rw-r--r--   0        0        0     2858 2024-05-18 16:27:42.351222 mleko-4.1.0/mleko/pipeline/steps/ingest_step.py
--rw-r--r--   0        0        0     8139 2024-05-18 16:27:42.351222 mleko-4.1.0/mleko/pipeline/steps/model_step.py
--rw-r--r--   0        0        0     3002 2024-05-18 16:27:42.351222 mleko-4.1.0/mleko/pipeline/steps/split_step.py
--rw-r--r--   0        0        0     5933 2024-05-18 16:27:42.351222 mleko-4.1.0/mleko/pipeline/steps/transform_step.py
--rw-r--r--   0        0        0     3551 2024-05-18 16:27:42.351222 mleko-4.1.0/mleko/pipeline/steps/tune_step.py
--rw-r--r--   0        0        0        0 2024-05-18 16:27:42.351222 mleko-4.1.0/mleko/py.typed
--rw-r--r--   0        0        0      977 2024-05-18 16:27:42.351222 mleko-4.1.0/mleko/utils/__init__.py
--rw-r--r--   0        0        0     9753 2024-05-18 16:27:42.351222 mleko-4.1.0/mleko/utils/custom_logger.py
--rw-r--r--   0        0        0     3431 2024-05-18 16:27:42.351222 mleko-4.1.0/mleko/utils/decorators.py
--rw-r--r--   0        0        0     4724 2024-05-18 16:27:42.351222 mleko-4.1.0/mleko/utils/file_helpers.py
--rw-r--r--   0        0        0    11820 2024-05-18 16:27:42.351222 mleko-4.1.0/mleko/utils/s3_helpers.py
--rw-r--r--   0        0        0     1414 2024-05-18 16:27:42.351222 mleko-4.1.0/mleko/utils/tqdm_helpers.py
--rw-r--r--   0        0        0     3641 2024-05-18 16:27:42.351222 mleko-4.1.0/mleko/utils/vaex_helpers.py
--rw-r--r--   0        0        0     2608 2024-05-18 16:28:13.179034 mleko-4.1.0/pyproject.toml
--rw-r--r--   0        0        0     6323 1970-01-01 00:00:00.000000 mleko-4.1.0/PKG-INFO
+-rw-r--r--   0        0        0    10947 2024-05-21 14:17:05.188627 mleko-4.2.0/LICENSE
+-rw-r--r--   0        0        0     5019 2024-05-21 14:17:05.188627 mleko-4.2.0/README.md
+-rw-r--r--   0        0        0     1976 2024-05-21 14:17:32.708827 mleko-4.2.0/mleko/__init__.py
+-rw-r--r--   0        0        0      585 2024-05-21 14:17:05.192627 mleko-4.2.0/mleko/cache/__init__.py
+-rw-r--r--   0        0        0    16986 2024-05-21 14:17:05.192627 mleko-4.2.0/mleko/cache/cache_mixin.py
+-rw-r--r--   0        0        0     1560 2024-05-21 14:17:05.192627 mleko-4.2.0/mleko/cache/fingerprinters/__init__.py
+-rw-r--r--   0        0        0     1168 2024-05-21 14:17:05.192627 mleko-4.2.0/mleko/cache/fingerprinters/base_fingerprinter.py
+-rw-r--r--   0        0        0     1012 2024-05-21 14:17:05.192627 mleko-4.2.0/mleko/cache/fingerprinters/callable_source_fingerprinter.py
+-rw-r--r--   0        0        0     2989 2024-05-21 14:17:05.192627 mleko-4.2.0/mleko/cache/fingerprinters/csv_fingerprinter.py
+-rw-r--r--   0        0        0     1248 2024-05-21 14:17:05.192627 mleko-4.2.0/mleko/cache/fingerprinters/json_fingerprinter.py
+-rw-r--r--   0        0        0     5578 2024-05-21 14:17:05.192627 mleko-4.2.0/mleko/cache/fingerprinters/optuna_pruner_fingerprinter.py
+-rw-r--r--   0        0        0    14262 2024-05-21 14:17:05.192627 mleko-4.2.0/mleko/cache/fingerprinters/optuna_sampler_fingerprinter.py
+-rw-r--r--   0        0        0     1219 2024-05-21 14:17:05.192627 mleko-4.2.0/mleko/cache/fingerprinters/vaex_fingerprinter.py
+-rw-r--r--   0        0        0     1832 2024-05-21 14:17:05.192627 mleko-4.2.0/mleko/cache/handlers/__init__.py
+-rw-r--r--   0        0        0      650 2024-05-21 14:17:05.192627 mleko-4.2.0/mleko/cache/handlers/base_cache_handler.py
+-rw-r--r--   0        0        0     1102 2024-05-21 14:17:05.192627 mleko-4.2.0/mleko/cache/handlers/joblib_cache_handler.py
+-rw-r--r--   0        0        0     1251 2024-05-21 14:17:05.192627 mleko-4.2.0/mleko/cache/handlers/json_cache_handler.py
+-rw-r--r--   0        0        0     1196 2024-05-21 14:17:05.192627 mleko-4.2.0/mleko/cache/handlers/pickle_cache_handler.py
+-rw-r--r--   0        0        0     1207 2024-05-21 14:17:05.192627 mleko-4.2.0/mleko/cache/handlers/string_cache_handler.py
+-rw-r--r--   0        0        0     1954 2024-05-21 14:17:05.192627 mleko-4.2.0/mleko/cache/handlers/vaex_cache_handler.py
+-rw-r--r--   0        0        0     8312 2024-05-21 14:17:05.192627 mleko-4.2.0/mleko/cache/lru_cache_mixin.py
+-rw-r--r--   0        0        0      805 2024-05-21 14:17:05.192627 mleko-4.2.0/mleko/dataset/__init__.py
+-rw-r--r--   0        0        0      492 2024-05-21 14:17:05.192627 mleko-4.2.0/mleko/dataset/convert/__init__.py
+-rw-r--r--   0        0        0     1613 2024-05-21 14:17:05.192627 mleko-4.2.0/mleko/dataset/convert/base_converter.py
+-rw-r--r--   0        0        0    15248 2024-05-21 14:17:05.192627 mleko-4.2.0/mleko/dataset/convert/csv_to_vaex_converter.py
+-rw-r--r--   0        0        0     6592 2024-05-21 14:17:05.192627 mleko-4.2.0/mleko/dataset/data_schema.py
+-rw-r--r--   0        0        0      774 2024-05-21 14:17:05.192627 mleko-4.2.0/mleko/dataset/export/__init__.py
+-rw-r--r--   0        0        0      900 2024-05-21 14:17:05.192627 mleko-4.2.0/mleko/dataset/export/base_exporter.py
+-rw-r--r--   0        0        0     8725 2024-05-21 14:17:05.192627 mleko-4.2.0/mleko/dataset/export/local_exporter.py
+-rw-r--r--   0        0        0     8191 2024-05-21 14:17:05.192627 mleko-4.2.0/mleko/dataset/export/s3_exporter.py
+-rw-r--r--   0        0        0     1614 2024-05-21 14:17:05.192627 mleko-4.2.0/mleko/dataset/feature_select/__init__.py
+-rw-r--r--   0        0        0    11612 2024-05-21 14:17:05.192627 mleko-4.2.0/mleko/dataset/feature_select/base_feature_selector.py
+-rw-r--r--   0        0        0     7661 2024-05-21 14:17:05.192627 mleko-4.2.0/mleko/dataset/feature_select/composite_feature_selector.py
+-rw-r--r--   0        0        0     5156 2024-05-21 14:17:05.192627 mleko-4.2.0/mleko/dataset/feature_select/invariance_feature_selector.py
+-rw-r--r--   0        0        0     5439 2024-05-21 14:17:05.192627 mleko-4.2.0/mleko/dataset/feature_select/missing_rate_feature_selector.py
+-rw-r--r--   0        0        0     7257 2024-05-21 14:17:05.192627 mleko-4.2.0/mleko/dataset/feature_select/pearson_correlation_feature_selector.py
+-rw-r--r--   0        0        0     5803 2024-05-21 14:17:05.192627 mleko-4.2.0/mleko/dataset/feature_select/variance_feature_selector.py
+-rw-r--r--   0        0        0      569 2024-05-21 14:17:05.192627 mleko-4.2.0/mleko/dataset/filter/__init__.py
+-rw-r--r--   0        0        0     1615 2024-05-21 14:17:05.192627 mleko-4.2.0/mleko/dataset/filter/base_filter.py
+-rw-r--r--   0        0        0     3927 2024-05-21 14:17:05.192627 mleko-4.2.0/mleko/dataset/filter/expression_filter.py
+-rw-r--r--   0        0        0     7160 2024-05-21 14:17:05.192627 mleko-4.2.0/mleko/dataset/filter/imblearn_resampling_filter.py
+-rw-r--r--   0        0        0      878 2024-05-21 14:17:05.192627 mleko-4.2.0/mleko/dataset/ingest/__init__.py
+-rw-r--r--   0        0        0     2747 2024-05-21 14:17:05.196627 mleko-4.2.0/mleko/dataset/ingest/base_ingester.py
+-rw-r--r--   0        0        0    20020 2024-05-21 14:17:05.196627 mleko-4.2.0/mleko/dataset/ingest/kaggle_ingester.py
+-rw-r--r--   0        0        0    11181 2024-05-21 14:17:05.196627 mleko-4.2.0/mleko/dataset/ingest/s3_ingester.py
+-rw-r--r--   0        0        0      680 2024-05-21 14:17:05.196627 mleko-4.2.0/mleko/dataset/split/__init__.py
+-rw-r--r--   0        0        0     1501 2024-05-21 14:17:05.196627 mleko-4.2.0/mleko/dataset/split/base_splitter.py
+-rw-r--r--   0        0        0     4254 2024-05-21 14:17:05.196627 mleko-4.2.0/mleko/dataset/split/expression_splitter.py
+-rw-r--r--   0        0        0     7029 2024-05-21 14:17:05.196627 mleko-4.2.0/mleko/dataset/split/random_splitter.py
+-rw-r--r--   0        0        0     1797 2024-05-21 14:17:05.196627 mleko-4.2.0/mleko/dataset/transform/__init__.py
+-rw-r--r--   0        0        0     9362 2024-05-21 14:17:05.196627 mleko-4.2.0/mleko/dataset/transform/base_transformer.py
+-rw-r--r--   0        0        0     6882 2024-05-21 14:17:05.196627 mleko-4.2.0/mleko/dataset/transform/composite_transformer.py
+-rw-r--r--   0        0        0     5359 2024-05-21 14:17:05.196627 mleko-4.2.0/mleko/dataset/transform/expression_transformer.py
+-rw-r--r--   0        0        0     4743 2024-05-21 14:17:05.196627 mleko-4.2.0/mleko/dataset/transform/frequency_encoder_transformer.py
+-rw-r--r--   0        0        0    11533 2024-05-21 14:17:05.196627 mleko-4.2.0/mleko/dataset/transform/label_encoder_transformer.py
+-rw-r--r--   0        0        0     3744 2024-05-21 14:17:05.196627 mleko-4.2.0/mleko/dataset/transform/max_abs_scaler_transformer.py
+-rw-r--r--   0        0        0     4150 2024-05-21 14:17:05.196627 mleko-4.2.0/mleko/dataset/transform/min_max_scaler_transformer.py
+-rw-r--r--   0        0        0      388 2024-05-21 14:17:05.196627 mleko-4.2.0/mleko/model/__init__.py
+-rw-r--r--   0        0        0    18964 2024-05-21 14:17:05.196627 mleko-4.2.0/mleko/model/base_model.py
+-rw-r--r--   0        0        0    10756 2024-05-21 14:17:05.196627 mleko-4.2.0/mleko/model/lgbm_model.py
+-rw-r--r--   0        0        0      413 2024-05-21 14:17:05.196627 mleko-4.2.0/mleko/model/tune/__init__.py
+-rw-r--r--   0        0        0     3785 2024-05-21 14:17:05.196627 mleko-4.2.0/mleko/model/tune/base_tuner.py
+-rw-r--r--   0        0        0    17012 2024-05-21 14:17:05.196627 mleko-4.2.0/mleko/model/tune/optuna_tuner.py
+-rw-r--r--   0        0        0      645 2024-05-21 14:17:05.196627 mleko-4.2.0/mleko/pipeline/__init__.py
+-rw-r--r--   0        0        0     1382 2024-05-21 14:17:05.196627 mleko-4.2.0/mleko/pipeline/data_container.py
+-rw-r--r--   0        0        0     4658 2024-05-21 14:17:05.196627 mleko-4.2.0/mleko/pipeline/pipeline.py
+-rw-r--r--   0        0        0     9807 2024-05-21 14:17:05.196627 mleko-4.2.0/mleko/pipeline/pipeline_step.py
+-rw-r--r--   0        0        0      928 2024-05-21 14:17:05.196627 mleko-4.2.0/mleko/pipeline/steps/__init__.py
+-rw-r--r--   0        0        0     3931 2024-05-21 14:17:05.196627 mleko-4.2.0/mleko/pipeline/steps/convert_step.py
+-rw-r--r--   0        0        0     3312 2024-05-21 14:17:05.196627 mleko-4.2.0/mleko/pipeline/steps/export_step.py
+-rw-r--r--   0        0        0     6310 2024-05-21 14:17:05.196627 mleko-4.2.0/mleko/pipeline/steps/feature_select_step.py
+-rw-r--r--   0        0        0     3115 2024-05-21 14:17:05.196627 mleko-4.2.0/mleko/pipeline/steps/filter_step.py
+-rw-r--r--   0        0        0     2858 2024-05-21 14:17:05.196627 mleko-4.2.0/mleko/pipeline/steps/ingest_step.py
+-rw-r--r--   0        0        0     8139 2024-05-21 14:17:05.196627 mleko-4.2.0/mleko/pipeline/steps/model_step.py
+-rw-r--r--   0        0        0     3002 2024-05-21 14:17:05.196627 mleko-4.2.0/mleko/pipeline/steps/split_step.py
+-rw-r--r--   0        0        0     5933 2024-05-21 14:17:05.196627 mleko-4.2.0/mleko/pipeline/steps/transform_step.py
+-rw-r--r--   0        0        0     3551 2024-05-21 14:17:05.196627 mleko-4.2.0/mleko/pipeline/steps/tune_step.py
+-rw-r--r--   0        0        0        0 2024-05-21 14:17:05.196627 mleko-4.2.0/mleko/py.typed
+-rw-r--r--   0        0        0      977 2024-05-21 14:17:05.196627 mleko-4.2.0/mleko/utils/__init__.py
+-rw-r--r--   0        0        0     9753 2024-05-21 14:17:05.196627 mleko-4.2.0/mleko/utils/custom_logger.py
+-rw-r--r--   0        0        0     3431 2024-05-21 14:17:05.196627 mleko-4.2.0/mleko/utils/decorators.py
+-rw-r--r--   0        0        0     4724 2024-05-21 14:17:05.196627 mleko-4.2.0/mleko/utils/file_helpers.py
+-rw-r--r--   0        0        0    11820 2024-05-21 14:17:05.196627 mleko-4.2.0/mleko/utils/s3_helpers.py
+-rw-r--r--   0        0        0     1414 2024-05-21 14:17:05.196627 mleko-4.2.0/mleko/utils/tqdm_helpers.py
+-rw-r--r--   0        0        0     3641 2024-05-21 14:17:05.196627 mleko-4.2.0/mleko/utils/vaex_helpers.py
+-rw-r--r--   0        0        0     2608 2024-05-21 14:17:32.708827 mleko-4.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6323 1970-01-01 00:00:00.000000 mleko-4.2.0/PKG-INFO
```

### Comparing `mleko-4.1.0/LICENSE` & `mleko-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mleko-4.1.0/README.md` & `mleko-4.2.0/README.md`

 * *Files identical despite different names*

### Comparing `mleko-4.1.0/mleko/__init__.py` & `mleko-4.2.0/mleko/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,8 +31,8 @@
 By integrating these features, `mleko` serves as a comprehensive toolkit for machine learning
 practitioners looking to build robust models efficiently.
 """
 
 from __future__ import annotations
 
 
-__version__ = "4.1.0"
+__version__ = "4.2.0"
```

### Comparing `mleko-4.1.0/mleko/cache/__init__.py` & `mleko-4.2.0/mleko/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-4.1.0/mleko/cache/cache_mixin.py` & `mleko-4.2.0/mleko/cache/cache_mixin.py`

 * *Files identical despite different names*

### Comparing `mleko-4.1.0/mleko/cache/fingerprinters/__init__.py` & `mleko-4.2.0/mleko/cache/fingerprinters/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-4.1.0/mleko/cache/fingerprinters/base_fingerprinter.py` & `mleko-4.2.0/mleko/cache/fingerprinters/base_fingerprinter.py`

 * *Files identical despite different names*

### Comparing `mleko-4.1.0/mleko/cache/fingerprinters/callable_source_fingerprinter.py` & `mleko-4.2.0/mleko/cache/fingerprinters/callable_source_fingerprinter.py`

 * *Files identical despite different names*

### Comparing `mleko-4.1.0/mleko/cache/fingerprinters/csv_fingerprinter.py` & `mleko-4.2.0/mleko/cache/fingerprinters/csv_fingerprinter.py`

 * *Files identical despite different names*

### Comparing `mleko-4.1.0/mleko/cache/fingerprinters/json_fingerprinter.py` & `mleko-4.2.0/mleko/cache/fingerprinters/json_fingerprinter.py`

 * *Files identical despite different names*

### Comparing `mleko-4.1.0/mleko/cache/fingerprinters/optuna_pruner_fingerprinter.py` & `mleko-4.2.0/mleko/cache/fingerprinters/optuna_pruner_fingerprinter.py`

 * *Files identical despite different names*

### Comparing `mleko-4.1.0/mleko/cache/fingerprinters/optuna_sampler_fingerprinter.py` & `mleko-4.2.0/mleko/cache/fingerprinters/optuna_sampler_fingerprinter.py`

 * *Files identical despite different names*

### Comparing `mleko-4.1.0/mleko/cache/fingerprinters/vaex_fingerprinter.py` & `mleko-4.2.0/mleko/cache/fingerprinters/vaex_fingerprinter.py`

 * *Files identical despite different names*

### Comparing `mleko-4.1.0/mleko/cache/handlers/__init__.py` & `mleko-4.2.0/mleko/cache/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-4.1.0/mleko/cache/handlers/base_cache_handler.py` & `mleko-4.2.0/mleko/cache/handlers/base_cache_handler.py`

 * *Files identical despite different names*

### Comparing `mleko-4.1.0/mleko/cache/handlers/joblib_cache_handler.py` & `mleko-4.2.0/mleko/cache/handlers/joblib_cache_handler.py`

 * *Files identical despite different names*

### Comparing `mleko-4.1.0/mleko/cache/handlers/json_cache_handler.py` & `mleko-4.2.0/mleko/cache/handlers/json_cache_handler.py`

 * *Files identical despite different names*

### Comparing `mleko-4.1.0/mleko/cache/handlers/pickle_cache_handler.py` & `mleko-4.2.0/mleko/cache/handlers/pickle_cache_handler.py`

 * *Files identical despite different names*

### Comparing `mleko-4.1.0/mleko/cache/handlers/string_cache_handler.py` & `mleko-4.2.0/mleko/cache/handlers/string_cache_handler.py`

 * *Files identical despite different names*

### Comparing `mleko-4.1.0/mleko/cache/handlers/vaex_cache_handler.py` & `mleko-4.2.0/mleko/cache/handlers/vaex_cache_handler.py`

 * *Files identical despite different names*

### Comparing `mleko-4.1.0/mleko/cache/lru_cache_mixin.py` & `mleko-4.2.0/mleko/cache/lru_cache_mixin.py`

 * *Files identical despite different names*

### Comparing `mleko-4.1.0/mleko/dataset/__init__.py` & `mleko-4.2.0/mleko/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-4.1.0/mleko/dataset/convert/base_converter.py` & `mleko-4.2.0/mleko/dataset/convert/base_converter.py`

 * *Files identical despite different names*

### Comparing `mleko-4.1.0/mleko/dataset/convert/csv_to_vaex_converter.py` & `mleko-4.2.0/mleko/dataset/convert/csv_to_vaex_converter.py`

 * *Files identical despite different names*

### Comparing `mleko-4.1.0/mleko/dataset/data_schema.py` & `mleko-4.2.0/mleko/dataset/data_schema.py`

 * *Files identical despite different names*

### Comparing `mleko-4.1.0/mleko/dataset/export/__init__.py` & `mleko-4.2.0/mleko/dataset/export/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-4.1.0/mleko/dataset/export/base_exporter.py` & `mleko-4.2.0/mleko/dataset/export/base_exporter.py`

 * *Files identical despite different names*

### Comparing `mleko-4.1.0/mleko/dataset/export/local_exporter.py` & `mleko-4.2.0/mleko/dataset/export/local_exporter.py`

 * *Files identical despite different names*

### Comparing `mleko-4.1.0/mleko/dataset/export/s3_exporter.py` & `mleko-4.2.0/mleko/dataset/export/s3_exporter.py`

 * *Files identical despite different names*

### Comparing `mleko-4.1.0/mleko/dataset/feature_select/__init__.py` & `mleko-4.2.0/mleko/dataset/feature_select/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-4.1.0/mleko/dataset/feature_select/base_feature_selector.py` & `mleko-4.2.0/mleko/dataset/feature_select/base_feature_selector.py`

 * *Files identical despite different names*

### Comparing `mleko-4.1.0/mleko/dataset/feature_select/composite_feature_selector.py` & `mleko-4.2.0/mleko/dataset/feature_select/composite_feature_selector.py`

 * *Files identical despite different names*

### Comparing `mleko-4.1.0/mleko/dataset/feature_select/invariance_feature_selector.py` & `mleko-4.2.0/mleko/dataset/feature_select/invariance_feature_selector.py`

 * *Files identical despite different names*

### Comparing `mleko-4.1.0/mleko/dataset/feature_select/missing_rate_feature_selector.py` & `mleko-4.2.0/mleko/dataset/feature_select/missing_rate_feature_selector.py`

 * *Files identical despite different names*

### Comparing `mleko-4.1.0/mleko/dataset/feature_select/pearson_correlation_feature_selector.py` & `mleko-4.2.0/mleko/dataset/feature_select/pearson_correlation_feature_selector.py`

 * *Files identical despite different names*

### Comparing `mleko-4.1.0/mleko/dataset/feature_select/variance_feature_selector.py` & `mleko-4.2.0/mleko/dataset/feature_select/variance_feature_selector.py`

 * *Files identical despite different names*

### Comparing `mleko-4.1.0/mleko/dataset/filter/__init__.py` & `mleko-4.2.0/mleko/dataset/filter/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-4.1.0/mleko/dataset/filter/base_filter.py` & `mleko-4.2.0/mleko/dataset/filter/base_filter.py`

 * *Files identical despite different names*

### Comparing `mleko-4.1.0/mleko/dataset/filter/expression_filter.py` & `mleko-4.2.0/mleko/dataset/filter/expression_filter.py`

 * *Files identical despite different names*

### Comparing `mleko-4.1.0/mleko/dataset/filter/imblearn_resampling_filter.py` & `mleko-4.2.0/mleko/dataset/filter/imblearn_resampling_filter.py`

 * *Files identical despite different names*

### Comparing `mleko-4.1.0/mleko/dataset/ingest/__init__.py` & `mleko-4.2.0/mleko/dataset/ingest/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-4.1.0/mleko/dataset/ingest/base_ingester.py` & `mleko-4.2.0/mleko/dataset/ingest/base_ingester.py`

 * *Files identical despite different names*

### Comparing `mleko-4.1.0/mleko/dataset/ingest/kaggle_ingester.py` & `mleko-4.2.0/mleko/dataset/ingest/kaggle_ingester.py`

 * *Files identical despite different names*

### Comparing `mleko-4.1.0/mleko/dataset/ingest/s3_ingester.py` & `mleko-4.2.0/mleko/dataset/ingest/s3_ingester.py`

 * *Files identical despite different names*

### Comparing `mleko-4.1.0/mleko/dataset/split/__init__.py` & `mleko-4.2.0/mleko/dataset/split/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-4.1.0/mleko/dataset/split/base_splitter.py` & `mleko-4.2.0/mleko/dataset/split/base_splitter.py`

 * *Files identical despite different names*

### Comparing `mleko-4.1.0/mleko/dataset/split/expression_splitter.py` & `mleko-4.2.0/mleko/dataset/split/expression_splitter.py`

 * *Files identical despite different names*

### Comparing `mleko-4.1.0/mleko/dataset/split/random_splitter.py` & `mleko-4.2.0/mleko/dataset/split/random_splitter.py`

 * *Files identical despite different names*

### Comparing `mleko-4.1.0/mleko/dataset/transform/__init__.py` & `mleko-4.2.0/mleko/dataset/transform/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-4.1.0/mleko/dataset/transform/base_transformer.py` & `mleko-4.2.0/mleko/dataset/transform/base_transformer.py`

 * *Files identical despite different names*

### Comparing `mleko-4.1.0/mleko/dataset/transform/composite_transformer.py` & `mleko-4.2.0/mleko/dataset/transform/composite_transformer.py`

 * *Files identical despite different names*

### Comparing `mleko-4.1.0/mleko/dataset/transform/expression_transformer.py` & `mleko-4.2.0/mleko/dataset/transform/expression_transformer.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,60 +2,75 @@
 
 from __future__ import annotations
 
 from pathlib import Path
 from typing import Hashable
 
 import vaex
+from typing_extensions import TypedDict
 
 from mleko.cache.fingerprinters.json_fingerprinter import JsonFingerprinter
 from mleko.dataset.data_schema import DataSchema, DataType
 from mleko.utils import CustomLogger, auto_repr, get_column
 
 from .base_transformer import BaseTransformer
 
 
 logger = CustomLogger()
 """A module-level logger for the module."""
 
 
+class ExpressionTransformerConfig(TypedDict):
+    """A type alias for the configuration of the expression transformer."""
+
+    expression: str
+    """The `vaex` expression used to create the new feature."""
+
+    type: DataType
+    """The data type of the new feature."""
+
+    is_meta: bool
+    """A boolean indicating if the new feature is a metadata feature."""
+
+
 class ExpressionTransformer(BaseTransformer):
     """Creates new features using `vaex` expressions."""
 
     @auto_repr
     def __init__(
         self,
-        expressions: dict[str, tuple[str, DataType, bool]],
+        expressions: dict[str, ExpressionTransformerConfig],
         cache_directory: str | Path = "data/expression-transformer",
         cache_size: int = 1,
     ) -> None:
         """Initializes the transformer with the specified expressions.
 
         The expressions are a dictionary where the key is the name of the new feature and the value is a tuple
         containing the expression, the data type and a boolean indicating if the feaature is a metadata feature.
         The expression must be a valid `vaex` expression that can be evaluated on the DataFrame.
 
         Note:
             To translate a `vaex` vectorized statement to a valid `vaex` expression, use the `.expression` attribute.
             For example, the expression of `df["a"] + df["b"]` can be extracted using `(df["a"] + df["b"]).expression`.
 
         Args:
-            expressions: A dictionary where the key is the name of the new feature and the value is a tuple containing
-                the expression, the data type and a boolean indicating if the feature is a metadata feature. In
+            expressions: A dictionary where the key is the name of the new feature and the value is a dictionary
+                containing the expression, the data type and a boolean indicating if the feaature is a metadata feature.
+                The expression must be a valid `vaex` expression that can be evaluated on the DataFrame.
             cache_directory: The directory where the cache will be stored locally.
             cache_size: The maximum number of cache entries to keep in the cache.
 
         Examples:
             >>> from mleko.dataset.data_schema import DataSchema
             >>> from mleko.dataset.transform import ExpressionTransformer
             >>> transformer = ExpressionTransformer(
             ...     expressions={
-            ...         "sum": ("a + b", "numerical", False),
-            ...         "product": ("a * b", "numerical", False),
-            ...         "both_positive": ("(a > 0) & (b > 0)", "boolean", True),
+            ...         "sum": {"expression": "a + b", "type": "numerical", "is_meta": False},
+            ...         "product": {"expression": "a * b", "type": "numerical", "is_meta": False},
+            ...         "both_positive": {"expression": "(a > 0) & (b > 0)", "type": "boolean", "is_meta": True},
             ...     }
             ... )
             >>> df = vaex.from_dict({"a": [1, 2, 3], "b": [4, 5, 6]})
             >>> ds = DataSchema(numerical=["a", "b"])
             >>> data_schema, _, transformed_df = transformer.fit_transform(ds, df)
             >>> transformed_df
             #    a    b    sum    product   both_positive
@@ -66,15 +81,15 @@
             DataSchema(numerical=['a', 'b', 'sum', 'product'])
         """
         super().__init__([], cache_directory, cache_size)
         self._transformer = expressions
 
     def _fit(
         self, data_schema: DataSchema, dataframe: vaex.DataFrame
-    ) -> tuple[DataSchema, dict[str, tuple[str, DataType, bool]]]:
+    ) -> tuple[DataSchema, dict[str, ExpressionTransformerConfig]]:
         """No fitting is required for the expression transformer.
 
         Args:
             data_schema: The data schema of the DataFrame.
             dataframe: The DataFrame to fit.
 
         Returns:
@@ -90,19 +105,21 @@
             dataframe: The DataFrame to transform.
 
         Returns:
             The transformed data schema and the transformed DataFrame.
         """
         df = dataframe.copy()
         ds = data_schema.copy()
-        for feature, (expression, data_type, is_meta) in self._transformer.items():
-            logger.info(f"Creating new {data_type!r} feature {feature!r} using expression {expression!r}.")
-            df[feature] = get_column(df, expression).as_arrow()
-            if not is_meta:
-                ds.add_feature(feature, data_type)
+        for feature, config in self._transformer.items():
+            logger.info(
+                f"Creating new {config['type']!r} feature {feature!r} using expression {config['expression']!r}."
+            )
+            df[feature] = get_column(df, config["expression"]).as_arrow()
+            if not config["is_meta"]:
+                ds.add_feature(feature, config["type"])
         return ds, df
 
     def _fingerprint(self) -> Hashable:
         """Returns the fingerprint of the transformer.
 
         Returns:
             A hashable object that uniquely identifies the transformer.
```

### Comparing `mleko-4.1.0/mleko/dataset/transform/frequency_encoder_transformer.py` & `mleko-4.2.0/mleko/dataset/transform/frequency_encoder_transformer.py`

 * *Files identical despite different names*

### Comparing `mleko-4.1.0/mleko/dataset/transform/label_encoder_transformer.py` & `mleko-4.2.0/mleko/dataset/transform/label_encoder_transformer.py`

 * *Files identical despite different names*

### Comparing `mleko-4.1.0/mleko/dataset/transform/max_abs_scaler_transformer.py` & `mleko-4.2.0/mleko/dataset/transform/max_abs_scaler_transformer.py`

 * *Files identical despite different names*

### Comparing `mleko-4.1.0/mleko/dataset/transform/min_max_scaler_transformer.py` & `mleko-4.2.0/mleko/dataset/transform/min_max_scaler_transformer.py`

 * *Files identical despite different names*

### Comparing `mleko-4.1.0/mleko/model/base_model.py` & `mleko-4.2.0/mleko/model/base_model.py`

 * *Files identical despite different names*

### Comparing `mleko-4.1.0/mleko/model/lgbm_model.py` & `mleko-4.2.0/mleko/model/lgbm_model.py`

 * *Files identical despite different names*

### Comparing `mleko-4.1.0/mleko/model/tune/base_tuner.py` & `mleko-4.2.0/mleko/model/tune/base_tuner.py`

 * *Files identical despite different names*

### Comparing `mleko-4.1.0/mleko/model/tune/optuna_tuner.py` & `mleko-4.2.0/mleko/model/tune/optuna_tuner.py`

 * *Files identical despite different names*

### Comparing `mleko-4.1.0/mleko/pipeline/__init__.py` & `mleko-4.2.0/mleko/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-4.1.0/mleko/pipeline/data_container.py` & `mleko-4.2.0/mleko/pipeline/data_container.py`

 * *Files identical despite different names*

### Comparing `mleko-4.1.0/mleko/pipeline/pipeline.py` & `mleko-4.2.0/mleko/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `mleko-4.1.0/mleko/pipeline/pipeline_step.py` & `mleko-4.2.0/mleko/pipeline/pipeline_step.py`

 * *Files identical despite different names*

### Comparing `mleko-4.1.0/mleko/pipeline/steps/__init__.py` & `mleko-4.2.0/mleko/pipeline/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-4.1.0/mleko/pipeline/steps/convert_step.py` & `mleko-4.2.0/mleko/pipeline/steps/convert_step.py`

 * *Files identical despite different names*

### Comparing `mleko-4.1.0/mleko/pipeline/steps/export_step.py` & `mleko-4.2.0/mleko/pipeline/steps/export_step.py`

 * *Files identical despite different names*

### Comparing `mleko-4.1.0/mleko/pipeline/steps/feature_select_step.py` & `mleko-4.2.0/mleko/pipeline/steps/feature_select_step.py`

 * *Files identical despite different names*

### Comparing `mleko-4.1.0/mleko/pipeline/steps/filter_step.py` & `mleko-4.2.0/mleko/pipeline/steps/filter_step.py`

 * *Files identical despite different names*

### Comparing `mleko-4.1.0/mleko/pipeline/steps/ingest_step.py` & `mleko-4.2.0/mleko/pipeline/steps/ingest_step.py`

 * *Files identical despite different names*

### Comparing `mleko-4.1.0/mleko/pipeline/steps/model_step.py` & `mleko-4.2.0/mleko/pipeline/steps/model_step.py`

 * *Files identical despite different names*

### Comparing `mleko-4.1.0/mleko/pipeline/steps/split_step.py` & `mleko-4.2.0/mleko/pipeline/steps/split_step.py`

 * *Files identical despite different names*

### Comparing `mleko-4.1.0/mleko/pipeline/steps/transform_step.py` & `mleko-4.2.0/mleko/pipeline/steps/transform_step.py`

 * *Files identical despite different names*

### Comparing `mleko-4.1.0/mleko/pipeline/steps/tune_step.py` & `mleko-4.2.0/mleko/pipeline/steps/tune_step.py`

 * *Files identical despite different names*

### Comparing `mleko-4.1.0/mleko/utils/__init__.py` & `mleko-4.2.0/mleko/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-4.1.0/mleko/utils/custom_logger.py` & `mleko-4.2.0/mleko/utils/custom_logger.py`

 * *Files identical despite different names*

### Comparing `mleko-4.1.0/mleko/utils/decorators.py` & `mleko-4.2.0/mleko/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `mleko-4.1.0/mleko/utils/file_helpers.py` & `mleko-4.2.0/mleko/utils/file_helpers.py`

 * *Files identical despite different names*

### Comparing `mleko-4.1.0/mleko/utils/s3_helpers.py` & `mleko-4.2.0/mleko/utils/s3_helpers.py`

 * *Files identical despite different names*

### Comparing `mleko-4.1.0/mleko/utils/tqdm_helpers.py` & `mleko-4.2.0/mleko/utils/tqdm_helpers.py`

 * *Files identical despite different names*

### Comparing `mleko-4.1.0/mleko/utils/vaex_helpers.py` & `mleko-4.2.0/mleko/utils/vaex_helpers.py`

 * *Files identical despite different names*

### Comparing `mleko-4.1.0/pyproject.toml` & `mleko-4.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mleko"
-version = "4.1.0"
+version = "4.2.0"
 description = "ML-Ekosystem"
 authors = ["Erik Båvenstrand <erik@bavenstrand.se>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/klarna-incubator/mleko"
 repository = "https://github.com/klarna-incubator/mleko"
 documentation = "https://mleko.readthedocs.io"
```

### Comparing `mleko-4.1.0/PKG-INFO` & `mleko-4.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mleko
-Version: 4.1.0
+Version: 4.2.0
 Summary: ML-Ekosystem
 Home-page: https://github.com/klarna-incubator/mleko
 License: Apache-2.0
 Author: Erik Båvenstrand
 Author-email: erik@bavenstrand.se
 Requires-Python: >=3.8.1,<3.11.dev0
 Classifier: Development Status :: 4 - Beta
```

