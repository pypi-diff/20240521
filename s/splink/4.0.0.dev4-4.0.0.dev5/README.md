# Comparing `tmp/splink-4.0.0.dev4.tar.gz` & `tmp/splink-4.0.0.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splink-4.0.0.dev4.tar", max compression
+gzip compressed data, was "splink-4.0.0.dev5.tar", max compression
```

## Comparing `splink-4.0.0.dev4.tar` & `splink-4.0.0.dev5.tar`

### file list

```diff
@@ -1,129 +1,146 @@
--rw-r--r--   0        0        0     1076 2024-05-17 12:06:36.526048 splink-4.0.0.dev4/LICENSE
--rw-r--r--   0        0        0    11224 2024-05-17 12:06:36.526048 splink-4.0.0.dev4/README.md
--rw-r--r--   0        0        0     3738 2024-05-17 12:06:36.674049 splink-4.0.0.dev4/pyproject.toml
--rw-r--r--   0        0        0     2076 2024-05-17 12:06:36.674049 splink-4.0.0.dev4/splink/__init__.py
--rw-r--r--   0        0        0    19195 2024-05-17 12:06:36.674049 splink-4.0.0.dev4/splink/accuracy.py
--rw-r--r--   0        0        0      350 2024-05-17 12:06:36.674049 splink-4.0.0.dev4/splink/athena/athena_helpers/athena_transforms.py
--rw-r--r--   0        0        0     2999 2024-05-17 12:06:36.674049 splink-4.0.0.dev4/splink/athena/athena_helpers/athena_utils.py
--rw-r--r--   0        0        0    23535 2024-05-17 12:06:36.674049 splink-4.0.0.dev4/splink/athena/linker.py
--rw-r--r--   0        0        0     2932 2024-05-17 12:06:36.674049 splink-4.0.0.dev4/splink/block_from_labels.py
--rw-r--r--   0        0        0    21352 2024-05-17 12:06:36.674049 splink-4.0.0.dev4/splink/blocking.py
--rw-r--r--   0        0        0      416 2024-05-17 12:06:36.674049 splink-4.0.0.dev4/splink/blocking_analysis.py
--rw-r--r--   0        0        0     1774 2024-05-17 12:06:36.674049 splink-4.0.0.dev4/splink/blocking_rule_creator.py
--rw-r--r--   0        0        0     1398 2024-05-17 12:06:36.674049 splink-4.0.0.dev4/splink/blocking_rule_creator_utils.py
--rw-r--r--   0        0        0     5992 2024-05-17 12:06:36.674049 splink-4.0.0.dev4/splink/blocking_rule_library.py
--rw-r--r--   0        0        0     2371 2024-05-17 12:06:36.674049 splink-4.0.0.dev4/splink/cache_dict_with_logging.py
--rw-r--r--   0        0        0    14938 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/charts.py
--rw-r--r--   0        0        0    14547 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/cluster_studio.py
--rw-r--r--   0        0        0     9629 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/column_expression.py
--rw-r--r--   0        0        0    16520 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/comparison.py
--rw-r--r--   0        0        0     8440 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/comparison_creator.py
--rw-r--r--   0        0        0     8940 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/comparison_helpers.py
--rw-r--r--   0        0        0    26220 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/comparison_level.py
--rw-r--r--   0        0        0     3948 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/comparison_level_composition.py
--rw-r--r--   0        0        0     5211 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/comparison_level_creator.py
--rw-r--r--   0        0        0    29966 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/comparison_level_library.py
--rw-r--r--   0        0        0     1242 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/comparison_level_sql.py
--rw-r--r--   0        0        0    24897 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/comparison_library.py
--rw-r--r--   0        0        0    24992 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/comparison_template_library.py
--rw-r--r--   0        0        0      979 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/comparison_vector_distribution.py
--rw-r--r--   0        0        0      874 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/comparison_vector_values.py
--rw-r--r--   0        0        0    17476 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/connected_components.py
--rw-r--r--   0        0        0       67 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/constants.py
--rw-r--r--   0        0        0     4693 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/cost_of_blocking_rules.py
--rw-r--r--   0        0        0    13026 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/database_api.py
--rw-r--r--   0        0        0     2487 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/databricks/enable_splink.py
--rw-r--r--   0        0        0     9801 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/datasets/__init__.py
--rw-r--r--   0        0        0      609 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/default_from_jsonschema.py
--rw-r--r--   0        0        0    16429 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/dialects.py
--rw-r--r--   0        0        0     3706 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/duckdb/database_api.py
--rw-r--r--   0        0        0     2735 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/duckdb/dataframe.py
--rw-r--r--   0        0        0     1762 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/duckdb/duckdb_helpers/duckdb_helpers.py
--rw-r--r--   0        0        0     5279 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/edge_metrics.py
--rw-r--r--   0        0        0    17045 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/em_training_session.py
--rw-r--r--   0        0        0     7922 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/estimate_u.py
--rw-r--r--   0        0        0     3226 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/exceptions.py
--rw-r--r--   0        0        0    15022 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/expectation_maximisation.py
--rw-r--r--   0        0        0      160 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/exploratory.py
--rw-r--r--   0        0        0   101742 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/files/DEPENDENCY_LICENSES.txt
--rw-r--r--   0        0        0     6779 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/files/chart_defs/accuracy_chart.json
--rw-r--r--   0        0        0     1316 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/files/chart_defs/blocking_rule_generated_comparisons.json
--rw-r--r--   0        0        0     3785 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/files/chart_defs/comparator_score_chart.json
--rw-r--r--   0        0        0     6417 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/files/chart_defs/comparator_score_threshold_chart.json
--rw-r--r--   0        0        0     2775 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/files/chart_defs/completeness.json
--rw-r--r--   0        0        0     5795 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/files/chart_defs/m_u_parameters_interactive_history.json
--rw-r--r--   0        0        0     1111 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/files/chart_defs/match_weight_histogram.json
--rw-r--r--   0        0        0     6963 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/files/chart_defs/match_weights_interactive_history.json
--rw-r--r--   0        0        0     9115 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/files/chart_defs/match_weights_waterfall.json
--rw-r--r--   0        0        0     1832 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/files/chart_defs/missingness.json
--rw-r--r--   0        0        0     2753 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/files/chart_defs/parameter_estimate_comparisons.json
--rw-r--r--   0        0        0     2660 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/files/chart_defs/phonetic_match_chart.json
--rw-r--r--   0        0        0     1654 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/files/chart_defs/precision_recall.json
--rw-r--r--   0        0        0     1125 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/files/chart_defs/probability_two_random_records_match_iteration.json
--rw-r--r--   0        0        0     2326 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/files/chart_defs/profile_data.json
--rw-r--r--   0        0        0     1805 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/files/chart_defs/roc.json
--rw-r--r--   0        0        0     9910 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/files/chart_defs/tf_adjustment_chart.json
--rw-r--r--   0        0        0    37552 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/files/chart_defs/threshold_selection_tool.json
--rw-r--r--   0        0        0     2910 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/files/chart_defs/unlinkables_chart_def.json
--rw-r--r--   0        0        0   279633 2024-05-17 12:06:36.682048 splink-4.0.0.dev4/splink/files/external_js/d3@7.8.5
--rw-r--r--   0        0        0    45883 2024-05-17 12:06:36.682048 splink-4.0.0.dev4/splink/files/external_js/stdlib.js@5.8.3
--rw-r--r--   0        0        0    66064 2024-05-17 12:06:36.682048 splink-4.0.0.dev4/splink/files/external_js/vega-embed@6.20.2
--rw-r--r--   0        0        0   256817 2024-05-17 12:06:36.682048 splink-4.0.0.dev4/splink/files/external_js/vega-lite@5.2.0
--rw-r--r--   0        0        0   501599 2024-05-17 12:06:36.686048 splink-4.0.0.dev4/splink/files/external_js/vega@5.21.0
--rw-r--r--   0        0        0   920157 2024-05-17 12:06:36.690049 splink-4.0.0.dev4/splink/files/labelling_tool/slt.js
--rw-r--r--   0        0        0     4104 2024-05-17 12:06:36.690049 splink-4.0.0.dev4/splink/files/labelling_tool/template.j2
--rw-r--r--   0        0        0    14089 2024-05-17 12:06:36.690049 splink-4.0.0.dev4/splink/files/settings_jsonschema.json
--rw-r--r--   0        0        0  1228220 2024-05-17 12:06:36.694049 splink-4.0.0.dev4/splink/files/spark_jars/scala-udf-similarity-0.1.0_classic.jar
--rw-r--r--   0        0        0   944614 2024-05-17 12:06:36.702048 splink-4.0.0.dev4/splink/files/spark_jars/scala-udf-similarity-0.1.0_spark3.3.jar
--rw-r--r--   0        0        0   949562 2024-05-17 12:06:36.706049 splink-4.0.0.dev4/splink/files/spark_jars/scala-udf-similarity-0.1.1_spark3.x.jar
--rw-r--r--   0        0        0     6506 2024-05-17 12:06:36.706049 splink-4.0.0.dev4/splink/files/splink_cluster_studio/cluster_template.j2
--rw-r--r--   0        0        0     2269 2024-05-17 12:06:36.706049 splink-4.0.0.dev4/splink/files/splink_cluster_studio/custom.css
--rw-r--r--   0        0        0     2269 2024-05-17 12:06:36.706049 splink-4.0.0.dev4/splink/files/splink_comparison_viewer/custom.css
--rw-r--r--   0        0        0     4120 2024-05-17 12:06:36.706049 splink-4.0.0.dev4/splink/files/splink_comparison_viewer/template.j2
--rw-r--r--   0        0        0   321314 2024-05-17 12:06:36.706049 splink-4.0.0.dev4/splink/files/splink_vis_utils/splink_vis_utils.js
--rw-r--r--   0        0        0      404 2024-05-17 12:06:36.706049 splink-4.0.0.dev4/splink/files/templates/single_chart_template.html
--rw-r--r--   0        0        0     9072 2024-05-17 12:06:36.706049 splink-4.0.0.dev4/splink/find_brs_with_comparison_counts_below_threshold.py
--rw-r--r--   0        0        0     1488 2024-05-17 12:06:36.706049 splink-4.0.0.dev4/splink/find_matches_to_new_records.py
--rw-r--r--   0        0        0    10088 2024-05-17 12:06:36.706049 splink-4.0.0.dev4/splink/graph_metrics.py
--rw-r--r--   0        0        0    12400 2024-05-17 12:06:36.706049 splink-4.0.0.dev4/splink/input_column.py
--rw-r--r--   0        0        0    23741 2024-05-17 12:06:36.706049 splink-4.0.0.dev4/splink/internals/blocking_analysis.py
--rw-r--r--   0        0        0     4066 2024-05-17 12:06:36.706049 splink-4.0.0.dev4/splink/internals/completeness.py
--rw-r--r--   0        0        0    11706 2024-05-17 12:06:36.706049 splink-4.0.0.dev4/splink/internals/profile_data.py
--rw-r--r--   0        0        0     3763 2024-05-17 12:06:36.706049 splink-4.0.0.dev4/splink/labelling_tool.py
--rw-r--r--   0        0        0   137958 2024-05-17 12:06:36.706049 splink-4.0.0.dev4/splink/linker.py
--rw-r--r--   0        0        0      300 2024-05-17 12:06:36.706049 splink-4.0.0.dev4/splink/logging_messages.py
--rw-r--r--   0        0        0     3191 2024-05-17 12:06:36.706049 splink-4.0.0.dev4/splink/lower_id_on_lhs.py
--rw-r--r--   0        0        0     2195 2024-05-17 12:06:36.706049 splink-4.0.0.dev4/splink/m_from_labels.py
--rw-r--r--   0        0        0     3238 2024-05-17 12:06:36.706049 splink-4.0.0.dev4/splink/m_training.py
--rw-r--r--   0        0        0     2696 2024-05-17 12:06:36.706049 splink-4.0.0.dev4/splink/m_u_records_to_parameters.py
--rw-r--r--   0        0        0      623 2024-05-17 12:06:36.706049 splink-4.0.0.dev4/splink/match_key_analysis.py
--rw-r--r--   0        0        0     2162 2024-05-17 12:06:36.706049 splink-4.0.0.dev4/splink/match_weights_histogram.py
--rw-r--r--   0        0        0     5482 2024-05-17 12:06:36.706049 splink-4.0.0.dev4/splink/misc.py
--rw-r--r--   0        0        0     7096 2024-05-17 12:06:36.706049 splink-4.0.0.dev4/splink/optimise_cost_of_brs.py
--rw-r--r--   0        0        0     2232 2024-05-17 12:06:36.706049 splink-4.0.0.dev4/splink/parse_sql.py
--rw-r--r--   0        0        0     3784 2024-05-17 12:06:36.706049 splink-4.0.0.dev4/splink/pipeline.py
--rw-r--r--   0        0        0     6487 2024-05-17 12:06:36.706049 splink-4.0.0.dev4/splink/postgres/database_api.py
--rw-r--r--   0        0        0     2379 2024-05-17 12:06:36.706049 splink-4.0.0.dev4/splink/postgres/dataframe.py
--rw-r--r--   0        0        0     7516 2024-05-17 12:06:36.706049 splink-4.0.0.dev4/splink/predict.py
--rw-r--r--   0        0        0    24963 2024-05-17 12:06:36.706049 splink-4.0.0.dev4/splink/settings.py
--rw-r--r--   0        0        0     5491 2024-05-17 12:06:36.706049 splink-4.0.0.dev4/splink/settings_creator.py
--rw-r--r--   0        0        0     9998 2024-05-17 12:06:36.706049 splink-4.0.0.dev4/splink/settings_validation/log_invalid_columns.py
--rw-r--r--   0        0        0     4694 2024-05-17 12:06:36.710049 splink-4.0.0.dev4/splink/settings_validation/settings_column_cleaner.py
--rw-r--r--   0        0        0     6613 2024-05-17 12:06:36.710049 splink-4.0.0.dev4/splink/settings_validation/settings_validation_log_strings.py
--rw-r--r--   0        0        0      797 2024-05-17 12:06:36.710049 splink-4.0.0.dev4/splink/settings_validation/valid_types.py
--rw-r--r--   0        0        0    13344 2024-05-17 12:06:36.710049 splink-4.0.0.dev4/splink/spark/database_api.py
--rw-r--r--   0        0        0     2224 2024-05-17 12:06:36.710049 splink-4.0.0.dev4/splink/spark/dataframe.py
--rw-r--r--   0        0        0     2235 2024-05-17 12:06:36.710049 splink-4.0.0.dev4/splink/spark/jar_location.py
--rw-r--r--   0        0        0     1110 2024-05-17 12:06:36.710049 splink-4.0.0.dev4/splink/spark/spark_helpers/custom_spark_dialect.py
--rw-r--r--   0        0        0     5180 2024-05-17 12:06:36.710049 splink-4.0.0.dev4/splink/splink_comparison_viewer.py
--rw-r--r--   0        0        0     6785 2024-05-17 12:06:36.710049 splink-4.0.0.dev4/splink/splink_dataframe.py
--rw-r--r--   0        0        0     4673 2024-05-17 12:06:36.710049 splink-4.0.0.dev4/splink/sql_transform.py
--rw-r--r--   0        0        0     3503 2024-05-17 12:06:36.710049 splink-4.0.0.dev4/splink/sqlite/database_api.py
--rw-r--r--   0        0        0     2267 2024-05-17 12:06:36.710049 splink-4.0.0.dev4/splink/sqlite/dataframe.py
--rw-r--r--   0        0        0    10265 2024-05-17 12:06:36.710049 splink-4.0.0.dev4/splink/term_frequencies.py
--rw-r--r--   0        0        0     1143 2024-05-17 12:06:36.710049 splink-4.0.0.dev4/splink/unique_id_concat.py
--rw-r--r--   0        0        0     1798 2024-05-17 12:06:36.710049 splink-4.0.0.dev4/splink/unlinkables.py
--rw-r--r--   0        0        0     2460 2024-05-17 12:06:36.710049 splink-4.0.0.dev4/splink/validate_jsonschema.py
--rw-r--r--   0        0        0     7428 2024-05-17 12:06:36.710049 splink-4.0.0.dev4/splink/vertically_concatenate.py
--rw-r--r--   0        0        0     5665 2024-05-17 12:06:36.710049 splink-4.0.0.dev4/splink/waterfall_chart.py
--rw-r--r--   0        0        0    12705 1970-01-01 00:00:00.000000 splink-4.0.0.dev4/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-05-21 08:29:08.391187 splink-4.0.0.dev5/LICENSE
+-rw-r--r--   0        0        0    11224 2024-05-21 08:29:08.391187 splink-4.0.0.dev5/README.md
+-rw-r--r--   0        0        0     3738 2024-05-21 08:29:08.519186 splink-4.0.0.dev5/pyproject.toml
+-rw-r--r--   0        0        0     2133 2024-05-21 08:29:08.519186 splink-4.0.0.dev5/splink/__init__.py
+-rw-r--r--   0        0        0      111 2024-05-21 08:29:08.519186 splink-4.0.0.dev5/splink/backends/spark.py
+-rw-r--r--   0        0        0       84 2024-05-21 08:29:08.519186 splink-4.0.0.dev5/splink/backends/sqlite.py
+-rw-r--r--   0        0        0      416 2024-05-21 08:29:08.519186 splink-4.0.0.dev5/splink/blocking_analysis.py
+-rw-r--r--   0        0        0      955 2024-05-21 08:29:08.519186 splink-4.0.0.dev5/splink/comparison_level_library.py
+-rw-r--r--   0        0        0      791 2024-05-21 08:29:08.519186 splink-4.0.0.dev5/splink/comparison_library.py
+-rw-r--r--   0        0        0      318 2024-05-21 08:29:08.519186 splink-4.0.0.dev5/splink/comparison_template_library.py
+-rw-r--r--   0        0        0      133 2024-05-21 08:29:08.519186 splink-4.0.0.dev5/splink/datasets.py
+-rw-r--r--   0        0        0      160 2024-05-21 08:29:08.519186 splink-4.0.0.dev5/splink/exploratory.py
+-rw-r--r--   0        0        0        0 2024-05-21 08:29:08.519186 splink-4.0.0.dev5/splink/internals/__init__.py
+-rw-r--r--   0        0        0    19364 2024-05-21 08:29:08.519186 splink-4.0.0.dev5/splink/internals/accuracy.py
+-rw-r--r--   0        0        0        0 2024-05-21 08:29:08.519186 splink-4.0.0.dev5/splink/internals/athena/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-21 08:29:08.519186 splink-4.0.0.dev5/splink/internals/athena/athena_helpers/__init__.py
+-rw-r--r--   0        0        0      350 2024-05-21 08:29:08.519186 splink-4.0.0.dev5/splink/internals/athena/athena_helpers/athena_transforms.py
+-rw-r--r--   0        0        0     3029 2024-05-21 08:29:08.519186 splink-4.0.0.dev5/splink/internals/athena/athena_helpers/athena_utils.py
+-rw-r--r--   0        0        0    23535 2024-05-21 08:29:08.519186 splink-4.0.0.dev5/splink/internals/athena/linker.py
+-rw-r--r--   0        0        0     2964 2024-05-21 08:29:08.519186 splink-4.0.0.dev5/splink/internals/block_from_labels.py
+-rw-r--r--   0        0        0    21374 2024-05-21 08:29:08.519186 splink-4.0.0.dev5/splink/internals/blocking.py
+-rw-r--r--   0        0        0    24046 2024-05-21 08:29:08.519186 splink-4.0.0.dev5/splink/internals/blocking_analysis.py
+-rw-r--r--   0        0        0     1806 2024-05-21 08:29:08.519186 splink-4.0.0.dev5/splink/internals/blocking_rule_creator.py
+-rw-r--r--   0        0        0     1447 2024-05-21 08:29:08.519186 splink-4.0.0.dev5/splink/internals/blocking_rule_creator_utils.py
+-rw-r--r--   0        0        0     6040 2024-05-21 08:29:08.519186 splink-4.0.0.dev5/splink/internals/blocking_rule_library.py
+-rw-r--r--   0        0        0     2387 2024-05-21 08:29:08.519186 splink-4.0.0.dev5/splink/internals/cache_dict_with_logging.py
+-rw-r--r--   0        0        0    15020 2024-05-21 08:29:08.519186 splink-4.0.0.dev5/splink/internals/charts.py
+-rw-r--r--   0        0        0    14713 2024-05-21 08:29:08.519186 splink-4.0.0.dev5/splink/internals/cluster_studio.py
+-rw-r--r--   0        0        0     9798 2024-05-21 08:29:08.523186 splink-4.0.0.dev5/splink/internals/column_expression.py
+-rw-r--r--   0        0        0    16582 2024-05-21 08:29:08.523186 splink-4.0.0.dev5/splink/internals/comparison.py
+-rw-r--r--   0        0        0     8473 2024-05-21 08:29:08.523186 splink-4.0.0.dev5/splink/internals/comparison_creator.py
+-rw-r--r--   0        0        0     8956 2024-05-21 08:29:08.523186 splink-4.0.0.dev5/splink/internals/comparison_helpers.py
+-rw-r--r--   0        0        0    26300 2024-05-21 08:29:08.523186 splink-4.0.0.dev5/splink/internals/comparison_level.py
+-rw-r--r--   0        0        0     3981 2024-05-21 08:29:08.523186 splink-4.0.0.dev5/splink/internals/comparison_level_composition.py
+-rw-r--r--   0        0        0     5244 2024-05-21 08:29:08.523186 splink-4.0.0.dev5/splink/internals/comparison_level_creator.py
+-rw-r--r--   0        0        0    31551 2024-05-21 08:29:08.523186 splink-4.0.0.dev5/splink/internals/comparison_level_library.py
+-rw-r--r--   0        0        0     1242 2024-05-21 08:29:08.523186 splink-4.0.0.dev5/splink/internals/comparison_level_sql.py
+-rw-r--r--   0        0        0    23732 2024-05-21 08:29:08.523186 splink-4.0.0.dev5/splink/internals/comparison_library.py
+-rw-r--r--   0        0        0    25087 2024-05-21 08:29:08.523186 splink-4.0.0.dev5/splink/internals/comparison_template_library.py
+-rw-r--r--   0        0        0      994 2024-05-21 08:29:08.523186 splink-4.0.0.dev5/splink/internals/comparison_vector_distribution.py
+-rw-r--r--   0        0        0      874 2024-05-21 08:29:08.523186 splink-4.0.0.dev5/splink/internals/comparison_vector_values.py
+-rw-r--r--   0        0        0     4172 2024-05-21 08:29:08.523186 splink-4.0.0.dev5/splink/internals/completeness.py
+-rw-r--r--   0        0        0    17556 2024-05-21 08:29:08.523186 splink-4.0.0.dev5/splink/internals/connected_components.py
+-rw-r--r--   0        0        0       67 2024-05-21 08:29:08.523186 splink-4.0.0.dev5/splink/internals/constants.py
+-rw-r--r--   0        0        0     4693 2024-05-21 08:29:08.523186 splink-4.0.0.dev5/splink/internals/cost_of_blocking_rules.py
+-rw-r--r--   0        0        0    13107 2024-05-21 08:29:08.523186 splink-4.0.0.dev5/splink/internals/database_api.py
+-rw-r--r--   0        0        0        0 2024-05-21 08:29:08.523186 splink-4.0.0.dev5/splink/internals/databricks/__init__.py
+-rw-r--r--   0        0        0     2497 2024-05-21 08:29:08.523186 splink-4.0.0.dev5/splink/internals/databricks/enable_splink.py
+-rw-r--r--   0        0        0     9801 2024-05-21 08:29:08.523186 splink-4.0.0.dev5/splink/internals/datasets/__init__.py
+-rw-r--r--   0        0        0      625 2024-05-21 08:29:08.523186 splink-4.0.0.dev5/splink/internals/default_from_jsonschema.py
+-rw-r--r--   0        0        0    16264 2024-05-21 08:29:08.523186 splink-4.0.0.dev5/splink/internals/dialects.py
+-rw-r--r--   0        0        0        0 2024-05-21 08:29:08.523186 splink-4.0.0.dev5/splink/internals/duckdb/__init__.py
+-rw-r--r--   0        0        0     3737 2024-05-21 08:29:08.523186 splink-4.0.0.dev5/splink/internals/duckdb/database_api.py
+-rw-r--r--   0        0        0     2765 2024-05-21 08:29:08.523186 splink-4.0.0.dev5/splink/internals/duckdb/dataframe.py
+-rw-r--r--   0        0        0        0 2024-05-21 08:29:08.523186 splink-4.0.0.dev5/splink/internals/duckdb/duckdb_helpers/__init__.py
+-rw-r--r--   0        0        0     1761 2024-05-21 08:29:08.523186 splink-4.0.0.dev5/splink/internals/duckdb/duckdb_helpers/duckdb_helpers.py
+-rw-r--r--   0        0        0     5360 2024-05-21 08:29:08.523186 splink-4.0.0.dev5/splink/internals/edge_metrics.py
+-rw-r--r--   0        0        0    17279 2024-05-21 08:29:08.523186 splink-4.0.0.dev5/splink/internals/em_training_session.py
+-rw-r--r--   0        0        0     8028 2024-05-21 08:29:08.523186 splink-4.0.0.dev5/splink/internals/estimate_u.py
+-rw-r--r--   0        0        0     3226 2024-05-21 08:29:08.523186 splink-4.0.0.dev5/splink/internals/exceptions.py
+-rw-r--r--   0        0        0    15167 2024-05-21 08:29:08.523186 splink-4.0.0.dev5/splink/internals/expectation_maximisation.py
+-rw-r--r--   0        0        0   101742 2024-05-21 08:29:08.523186 splink-4.0.0.dev5/splink/internals/files/DEPENDENCY_LICENSES.txt
+-rw-r--r--   0        0        0     6779 2024-05-21 08:29:08.523186 splink-4.0.0.dev5/splink/internals/files/chart_defs/accuracy_chart.json
+-rw-r--r--   0        0        0     1316 2024-05-21 08:29:08.523186 splink-4.0.0.dev5/splink/internals/files/chart_defs/blocking_rule_generated_comparisons.json
+-rw-r--r--   0        0        0     3785 2024-05-21 08:29:08.523186 splink-4.0.0.dev5/splink/internals/files/chart_defs/comparator_score_chart.json
+-rw-r--r--   0        0        0     6417 2024-05-21 08:29:08.523186 splink-4.0.0.dev5/splink/internals/files/chart_defs/comparator_score_threshold_chart.json
+-rw-r--r--   0        0        0     2775 2024-05-21 08:29:08.523186 splink-4.0.0.dev5/splink/internals/files/chart_defs/completeness.json
+-rw-r--r--   0        0        0     5795 2024-05-21 08:29:08.523186 splink-4.0.0.dev5/splink/internals/files/chart_defs/m_u_parameters_interactive_history.json
+-rw-r--r--   0        0        0     1111 2024-05-21 08:29:08.523186 splink-4.0.0.dev5/splink/internals/files/chart_defs/match_weight_histogram.json
+-rw-r--r--   0        0        0     6963 2024-05-21 08:29:08.523186 splink-4.0.0.dev5/splink/internals/files/chart_defs/match_weights_interactive_history.json
+-rw-r--r--   0        0        0     9115 2024-05-21 08:29:08.523186 splink-4.0.0.dev5/splink/internals/files/chart_defs/match_weights_waterfall.json
+-rw-r--r--   0        0        0     1832 2024-05-21 08:29:08.523186 splink-4.0.0.dev5/splink/internals/files/chart_defs/missingness.json
+-rw-r--r--   0        0        0     2753 2024-05-21 08:29:08.523186 splink-4.0.0.dev5/splink/internals/files/chart_defs/parameter_estimate_comparisons.json
+-rw-r--r--   0        0        0     2660 2024-05-21 08:29:08.523186 splink-4.0.0.dev5/splink/internals/files/chart_defs/phonetic_match_chart.json
+-rw-r--r--   0        0        0     1654 2024-05-21 08:29:08.523186 splink-4.0.0.dev5/splink/internals/files/chart_defs/precision_recall.json
+-rw-r--r--   0        0        0     1125 2024-05-21 08:29:08.523186 splink-4.0.0.dev5/splink/internals/files/chart_defs/probability_two_random_records_match_iteration.json
+-rw-r--r--   0        0        0     2326 2024-05-21 08:29:08.523186 splink-4.0.0.dev5/splink/internals/files/chart_defs/profile_data.json
+-rw-r--r--   0        0        0     1805 2024-05-21 08:29:08.523186 splink-4.0.0.dev5/splink/internals/files/chart_defs/roc.json
+-rw-r--r--   0        0        0     9910 2024-05-21 08:29:08.523186 splink-4.0.0.dev5/splink/internals/files/chart_defs/tf_adjustment_chart.json
+-rw-r--r--   0        0        0    37552 2024-05-21 08:29:08.523186 splink-4.0.0.dev5/splink/internals/files/chart_defs/threshold_selection_tool.json
+-rw-r--r--   0        0        0     2910 2024-05-21 08:29:08.523186 splink-4.0.0.dev5/splink/internals/files/chart_defs/unlinkables_chart_def.json
+-rw-r--r--   0        0        0   279633 2024-05-21 08:29:08.527186 splink-4.0.0.dev5/splink/internals/files/external_js/d3@7.8.5
+-rw-r--r--   0        0        0    45883 2024-05-21 08:29:08.527186 splink-4.0.0.dev5/splink/internals/files/external_js/stdlib.js@5.8.3
+-rw-r--r--   0        0        0    66064 2024-05-21 08:29:08.527186 splink-4.0.0.dev5/splink/internals/files/external_js/vega-embed@6.20.2
+-rw-r--r--   0        0        0   256817 2024-05-21 08:29:08.527186 splink-4.0.0.dev5/splink/internals/files/external_js/vega-lite@5.2.0
+-rw-r--r--   0        0        0   501599 2024-05-21 08:29:08.531185 splink-4.0.0.dev5/splink/internals/files/external_js/vega@5.21.0
+-rw-r--r--   0        0        0   920157 2024-05-21 08:29:08.535186 splink-4.0.0.dev5/splink/internals/files/labelling_tool/slt.js
+-rw-r--r--   0        0        0     4104 2024-05-21 08:29:08.535186 splink-4.0.0.dev5/splink/internals/files/labelling_tool/template.j2
+-rw-r--r--   0        0        0    14089 2024-05-21 08:29:08.535186 splink-4.0.0.dev5/splink/internals/files/settings_jsonschema.json
+-rw-r--r--   0        0        0  1228220 2024-05-21 08:29:08.539186 splink-4.0.0.dev5/splink/internals/files/spark_jars/scala-udf-similarity-0.1.0_classic.jar
+-rw-r--r--   0        0        0   944614 2024-05-21 08:29:08.547186 splink-4.0.0.dev5/splink/internals/files/spark_jars/scala-udf-similarity-0.1.0_spark3.3.jar
+-rw-r--r--   0        0        0   949562 2024-05-21 08:29:08.551185 splink-4.0.0.dev5/splink/internals/files/spark_jars/scala-udf-similarity-0.1.1_spark3.x.jar
+-rw-r--r--   0        0        0     6506 2024-05-21 08:29:08.551185 splink-4.0.0.dev5/splink/internals/files/splink_cluster_studio/cluster_template.j2
+-rw-r--r--   0        0        0     2269 2024-05-21 08:29:08.551185 splink-4.0.0.dev5/splink/internals/files/splink_cluster_studio/custom.css
+-rw-r--r--   0        0        0     2269 2024-05-21 08:29:08.551185 splink-4.0.0.dev5/splink/internals/files/splink_comparison_viewer/custom.css
+-rw-r--r--   0        0        0     4120 2024-05-21 08:29:08.551185 splink-4.0.0.dev5/splink/internals/files/splink_comparison_viewer/template.j2
+-rw-r--r--   0        0        0   321314 2024-05-21 08:29:08.551185 splink-4.0.0.dev5/splink/internals/files/splink_vis_utils/splink_vis_utils.js
+-rw-r--r--   0        0        0      404 2024-05-21 08:29:08.551185 splink-4.0.0.dev5/splink/internals/files/templates/single_chart_template.html
+-rw-r--r--   0        0        0     9163 2024-05-21 08:29:08.551185 splink-4.0.0.dev5/splink/internals/find_brs_with_comparison_counts_below_threshold.py
+-rw-r--r--   0        0        0     1537 2024-05-21 08:29:08.551185 splink-4.0.0.dev5/splink/internals/find_matches_to_new_records.py
+-rw-r--r--   0        0        0    10098 2024-05-21 08:29:08.551185 splink-4.0.0.dev5/splink/internals/graph_metrics.py
+-rw-r--r--   0        0        0    12432 2024-05-21 08:29:08.551185 splink-4.0.0.dev5/splink/internals/input_column.py
+-rw-r--r--   0        0        0     3883 2024-05-21 08:29:08.551185 splink-4.0.0.dev5/splink/internals/labelling_tool.py
+-rw-r--r--   0        0        0   120279 2024-05-21 08:29:08.551185 splink-4.0.0.dev5/splink/internals/linker.py
+-rw-r--r--   0        0        0      300 2024-05-21 08:29:08.551185 splink-4.0.0.dev5/splink/internals/logging_messages.py
+-rw-r--r--   0        0        0     3191 2024-05-21 08:29:08.551185 splink-4.0.0.dev5/splink/internals/lower_id_on_lhs.py
+-rw-r--r--   0        0        0     2285 2024-05-21 08:29:08.551185 splink-4.0.0.dev5/splink/internals/m_from_labels.py
+-rw-r--r--   0        0        0     3328 2024-05-21 08:29:08.551185 splink-4.0.0.dev5/splink/internals/m_training.py
+-rw-r--r--   0        0        0     2728 2024-05-21 08:29:08.551185 splink-4.0.0.dev5/splink/internals/m_u_records_to_parameters.py
+-rw-r--r--   0        0        0      623 2024-05-21 08:29:08.551185 splink-4.0.0.dev5/splink/internals/match_key_analysis.py
+-rw-r--r--   0        0        0     2178 2024-05-21 08:29:08.551185 splink-4.0.0.dev5/splink/internals/match_weights_histogram.py
+-rw-r--r--   0        0        0     5482 2024-05-21 08:29:08.551185 splink-4.0.0.dev5/splink/internals/misc.py
+-rw-r--r--   0        0        0     7112 2024-05-21 08:29:08.551185 splink-4.0.0.dev5/splink/internals/optimise_cost_of_brs.py
+-rw-r--r--   0        0        0     2248 2024-05-21 08:29:08.551185 splink-4.0.0.dev5/splink/internals/parse_sql.py
+-rw-r--r--   0        0        0     3817 2024-05-21 08:29:08.551185 splink-4.0.0.dev5/splink/internals/pipeline.py
+-rw-r--r--   0        0        0        0 2024-05-21 08:29:08.551185 splink-4.0.0.dev5/splink/internals/postgres/__init__.py
+-rw-r--r--   0        0        0     6533 2024-05-21 08:29:08.551185 splink-4.0.0.dev5/splink/internals/postgres/database_api.py
+-rw-r--r--   0        0        0     2409 2024-05-21 08:29:08.551185 splink-4.0.0.dev5/splink/internals/postgres/dataframe.py
+-rw-r--r--   0        0        0     7565 2024-05-21 08:29:08.551185 splink-4.0.0.dev5/splink/internals/predict.py
+-rw-r--r--   0        0        0    11814 2024-05-21 08:29:08.551185 splink-4.0.0.dev5/splink/internals/profile_data.py
+-rw-r--r--   0        0        0    25109 2024-05-21 08:29:08.551185 splink-4.0.0.dev5/splink/internals/settings.py
+-rw-r--r--   0        0        0     5393 2024-05-21 08:29:08.551185 splink-4.0.0.dev5/splink/internals/settings_creator.py
+-rw-r--r--   0        0        0        0 2024-05-21 08:29:08.551185 splink-4.0.0.dev5/splink/internals/settings_validation/__init__.py
+-rw-r--r--   0        0        0    10029 2024-05-21 08:29:08.551185 splink-4.0.0.dev5/splink/internals/settings_validation/log_invalid_columns.py
+-rw-r--r--   0        0        0     4739 2024-05-21 08:29:08.555185 splink-4.0.0.dev5/splink/internals/settings_validation/settings_column_cleaner.py
+-rw-r--r--   0        0        0     6613 2024-05-21 08:29:08.555185 splink-4.0.0.dev5/splink/internals/settings_validation/settings_validation_log_strings.py
+-rw-r--r--   0        0        0      797 2024-05-21 08:29:08.555185 splink-4.0.0.dev5/splink/internals/settings_validation/valid_types.py
+-rw-r--r--   0        0        0        0 2024-05-21 08:29:08.555185 splink-4.0.0.dev5/splink/internals/spark/__init__.py
+-rw-r--r--   0        0        0    13405 2024-05-21 08:29:08.555185 splink-4.0.0.dev5/splink/internals/spark/database_api.py
+-rw-r--r--   0        0        0     2255 2024-05-21 08:29:08.555185 splink-4.0.0.dev5/splink/internals/spark/dataframe.py
+-rw-r--r--   0        0        0     2255 2024-05-21 08:29:08.555185 splink-4.0.0.dev5/splink/internals/spark/jar_location.py
+-rw-r--r--   0        0        0        0 2024-05-21 08:29:08.555185 splink-4.0.0.dev5/splink/internals/spark/spark_helpers/__init__.py
+-rw-r--r--   0        0        0     1110 2024-05-21 08:29:08.555185 splink-4.0.0.dev5/splink/internals/spark/spark_helpers/custom_spark_dialect.py
+-rw-r--r--   0        0        0     5283 2024-05-21 08:29:08.555185 splink-4.0.0.dev5/splink/internals/splink_comparison_viewer.py
+-rw-r--r--   0        0        0     6817 2024-05-21 08:29:08.555185 splink-4.0.0.dev5/splink/internals/splink_dataframe.py
+-rw-r--r--   0        0        0     4673 2024-05-21 08:29:08.555185 splink-4.0.0.dev5/splink/internals/sql_transform.py
+-rw-r--r--   0        0        0        0 2024-05-21 08:29:08.555185 splink-4.0.0.dev5/splink/internals/sqlite/__init__.py
+-rw-r--r--   0        0        0     3549 2024-05-21 08:29:08.555185 splink-4.0.0.dev5/splink/internals/sqlite/database_api.py
+-rw-r--r--   0        0        0     2297 2024-05-21 08:29:08.555185 splink-4.0.0.dev5/splink/internals/sqlite/dataframe.py
+-rw-r--r--   0        0        0    10346 2024-05-21 08:29:08.555185 splink-4.0.0.dev5/splink/internals/term_frequencies.py
+-rw-r--r--   0        0        0     1159 2024-05-21 08:29:08.555185 splink-4.0.0.dev5/splink/internals/unique_id_concat.py
+-rw-r--r--   0        0        0     1830 2024-05-21 08:29:08.555185 splink-4.0.0.dev5/splink/internals/unlinkables.py
+-rw-r--r--   0        0        0     2476 2024-05-21 08:29:08.555185 splink-4.0.0.dev5/splink/internals/validate_jsonschema.py
+-rw-r--r--   0        0        0     7563 2024-05-21 08:29:08.555185 splink-4.0.0.dev5/splink/internals/vertically_concatenate.py
+-rw-r--r--   0        0        0     5697 2024-05-21 08:29:08.555185 splink-4.0.0.dev5/splink/internals/waterfall_chart.py
+-rw-r--r--   0        0        0    12705 1970-01-01 00:00:00.000000 splink-4.0.0.dev5/PKG-INFO
```

### Comparing `splink-4.0.0.dev4/LICENSE` & `splink-4.0.0.dev5/LICENSE`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev4/README.md` & `splink-4.0.0.dev5/README.md`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev4/pyproject.toml` & `splink-4.0.0.dev5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "splink"
-version = "4.0.0.dev4"
+version = "4.0.0.dev5"
 description = "Fast probabilistic data linkage at scale"
 authors = ["Robin Linacre <robinlinacre@hotmail.com>", "Sam Lindsay", "Theodore Manassis", "Tom Hepworth", "Andy Bond", "Ross Kennedy"]
 license = "MIT"
 homepage = "https://github.com/moj-analytical-services/splink"
 repository = "https://github.com/moj-analytical-services/splink"
 readme = "README.md"
```

### Comparing `splink-4.0.0.dev4/splink/accuracy.py` & `splink-4.0.0.dev5/splink/internals/accuracy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 from __future__ import annotations
 
 from copy import deepcopy
 from typing import TYPE_CHECKING
 
-from .block_from_labels import block_from_labels
-from .blocking import BlockingRule
-from .comparison_vector_values import compute_comparison_vector_values_sql
-from .misc import calculate_cartesian
-from .pipeline import CTEPipeline
-from .predict import predict_from_comparison_vectors_sqls_using_settings
-from .splink_dataframe import SplinkDataFrame
-from .sql_transform import move_l_r_table_prefix_to_column_suffix
-from .vertically_concatenate import (
+from splink.internals.block_from_labels import block_from_labels
+from splink.internals.blocking import BlockingRule
+from splink.internals.comparison_vector_values import (
+    compute_comparison_vector_values_sql,
+)
+from splink.internals.misc import calculate_cartesian
+from splink.internals.pipeline import CTEPipeline
+from splink.internals.predict import predict_from_comparison_vectors_sqls_using_settings
+from splink.internals.splink_dataframe import SplinkDataFrame
+from splink.internals.sql_transform import move_l_r_table_prefix_to_column_suffix
+from splink.internals.vertically_concatenate import (
     compute_df_concat,
     compute_df_concat_with_tf,
 )
 
 if TYPE_CHECKING:
-    from .linker import Linker
+    from splink.internals.linker import Linker
 
 
 def truth_space_table_from_labels_with_predictions_sqls(
     threshold_actual: float = 0.5,
     match_weight_round_to_nearest: float | None = None,
     total_labels: int = None,
     positives_not_captured_by_blocking_rules_scored_as_zero: bool = True,
```

### Comparing `splink-4.0.0.dev4/splink/athena/athena_helpers/athena_utils.py` & `splink-4.0.0.dev5/splink/internals/athena/athena_helpers/athena_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import awswrangler as wr
 
-from splink.exceptions import InvalidAWSBucketOrDatabase
-from splink.misc import ensure_is_list
-from splink.splink_dataframe import SplinkDataFrame
+from splink.internals.exceptions import InvalidAWSBucketOrDatabase
+from splink.internals.misc import ensure_is_list
+from splink.internals.splink_dataframe import SplinkDataFrame
 
 
 def athena_warning_text(database_bucket_txt, do_does_grammar):
     return (
         f"\nThe supplied {database_bucket_txt} that you have requested to write to "
         f"{do_does_grammar[0]} not currently exist. \n \nCreate "
         f"{do_does_grammar[1]} either directly from within AWS, or by using "
```

### Comparing `splink-4.0.0.dev4/splink/athena/linker.py` & `splink-4.0.0.dev5/splink/internals/athena/linker.py`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev4/splink/block_from_labels.py` & `splink-4.0.0.dev5/splink/internals/block_from_labels.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
-from .lower_id_on_lhs import lower_id_to_left_hand_side
+from splink.internals.lower_id_on_lhs import lower_id_to_left_hand_side
 
 # https://stackoverflow.com/questions/39740632/python-type-hinting-without-cyclic-imports
 if TYPE_CHECKING:
-    from .linker import Linker
+    from splink.internals.linker import Linker
 
 
 def block_from_labels(
     linker: Linker, labels_table_name: str, include_clerical_match_score: bool = False
 ) -> list[dict[str, str]]:
     """Create pairwise record comparisons corresponding to the ID pairs in a labels
     table
```

### Comparing `splink-4.0.0.dev4/splink/blocking.py` & `splink-4.0.0.dev5/splink/internals/blocking.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,28 +4,28 @@
 from typing import TYPE_CHECKING, Any, List, Literal, Optional
 
 from sqlglot import parse_one
 from sqlglot.expressions import Column, Expression, Identifier, Join
 from sqlglot.optimizer.eliminate_joins import join_condition
 from sqlglot.optimizer.optimizer import optimize
 
-from .database_api import DatabaseAPISubClass
-from .exceptions import SplinkException
-from .input_column import InputColumn
-from .misc import ensure_is_list
-from .pipeline import CTEPipeline
-from .splink_dataframe import SplinkDataFrame
-from .unique_id_concat import _composite_unique_id_from_nodes_sql
-from .vertically_concatenate import vertically_concatenate_sql
+from splink.internals.database_api import DatabaseAPISubClass
+from splink.internals.exceptions import SplinkException
+from splink.internals.input_column import InputColumn
+from splink.internals.misc import ensure_is_list
+from splink.internals.pipeline import CTEPipeline
+from splink.internals.splink_dataframe import SplinkDataFrame
+from splink.internals.unique_id_concat import _composite_unique_id_from_nodes_sql
+from splink.internals.vertically_concatenate import vertically_concatenate_sql
 
 logger = logging.getLogger(__name__)
 
 # https://stackoverflow.com/questions/39740632/python-type-hinting-without-cyclic-imports
 if TYPE_CHECKING:
-    from .settings import LinkTypeLiteralType
+    from splink.internals.settings import LinkTypeLiteralType
 
 user_input_link_type_options = Literal["link_only", "link_and_dedupe", "dedupe_only"]
 
 backend_link_type_options = Literal[
     "link_only", "link_and_dedupe", "dedupe_only", "two_dataset_link_only", "self_link"
 ]
 
@@ -480,22 +480,18 @@
 
     if len(exploding_blocking_rules) == 0:
         return []
     exploded_tables = []
 
     pipeline = CTEPipeline()
 
-    source_dataset_column_name = (
-        source_dataset_input_column.name if source_dataset_input_column else None
-    )
-
     sql = vertically_concatenate_sql(
         splink_df_dict,
         salting_required=False,
-        source_dataset_column_name=source_dataset_column_name,
+        source_dataset_input_column=source_dataset_input_column,
     )
     pipeline.enqueue_sql(sql, "__splink__df_concat")
     nodes_concat = db_api.sql_pipeline_to_splink_dataframe(pipeline)
 
     input_colnames = {col.name for col in nodes_concat.columns}
 
     for br in exploding_blocking_rules:
```

### Comparing `splink-4.0.0.dev4/splink/blocking_rule_creator.py` & `splink-4.0.0.dev5/splink/internals/blocking_rule_creator.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from typing import Any, Dict, Union, final
 
-from .blocking import BlockingRule, blocking_rule_to_obj
-from .dialects import SplinkDialect
+from splink.internals.blocking import BlockingRule, blocking_rule_to_obj
+from splink.internals.dialects import SplinkDialect
 
 
 class BlockingRuleCreator(ABC):
     def __init__(
         self,
         salting_partitions: int | None = None,
         arrays_to_explode: list[str] | None = None,
```

### Comparing `splink-4.0.0.dev4/splink/blocking_rule_creator_utils.py` & `splink-4.0.0.dev5/splink/internals/blocking_rule_creator_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from __future__ import annotations
 
 from typing import Any, List, Union
 
-from .blocking import BlockingRule
-from .blocking_rule_creator import BlockingRuleCreator
+from splink.internals.blocking import BlockingRule
+from splink.internals.blocking_rule_creator import BlockingRuleCreator
+from splink.internals.misc import ensure_is_iterable
+
 from .blocking_rule_library import CustomRule
-from .misc import ensure_is_iterable
 
 
 def to_blocking_rule_creator(
     blocking_rule_creator: Union[dict[str, Any], str, BlockingRuleCreator],
 ) -> BlockingRuleCreator:
     if isinstance(blocking_rule_creator, dict):
         return CustomRule(**blocking_rule_creator)
```

### Comparing `splink-4.0.0.dev4/splink/blocking_rule_library.py` & `splink-4.0.0.dev5/splink/internals/blocking_rule_library.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 
 from typing import Any, Union, final
 
 from sqlglot import TokenError, parse_one
 
-from .blocking_rule_creator import BlockingRuleCreator
-from .column_expression import ColumnExpression
-from .dialects import SplinkDialect
+from splink.internals.blocking_rule_creator import BlockingRuleCreator
+from splink.internals.column_expression import ColumnExpression
+from splink.internals.dialects import SplinkDialect
 
 
 def _translate_sql_string(
     sqlglot_base_dialect_sql: str,
     to_sqlglot_dialect: str,
     from_sqlglot_dialect: str = None,
 ) -> str:
```

### Comparing `splink-4.0.0.dev4/splink/cache_dict_with_logging.py` & `splink-4.0.0.dev5/splink/internals/cache_dict_with_logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 from collections import UserDict
 from copy import copy
 from typing import TYPE_CHECKING
 
-from .splink_dataframe import SplinkDataFrame
+from splink.internals.splink_dataframe import SplinkDataFrame
 
 logger = logging.getLogger(__name__)
 
 if TYPE_CHECKING:
     TypedUserDict = UserDict[str, SplinkDataFrame]
 else:
     TypedUserDict = UserDict
```

### Comparing `splink-4.0.0.dev4/splink/charts.py` & `splink-4.0.0.dev5/splink/internals/charts.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 import math
 import os
 from typing import TYPE_CHECKING, Any, Dict, Union
 
 import numpy as np
 import pandas as pd
 
-from .misc import read_resource
-from .waterfall_chart import records_to_waterfall_data
+from splink.internals.misc import read_resource
+from splink.internals.waterfall_chart import records_to_waterfall_data
 
 altair_installed = True
 
 try:
     import altair as alt
 except ImportError:
     altair_installed = False
@@ -22,23 +22,23 @@
     import altair as alt
 
 # type alias:
 ChartReturnType = Union[Dict[Any, Any], alt.core.SchemaBase]
 
 
 def load_chart_definition(filename):
-    path = f"files/chart_defs/{filename}"
+    path = f"internals/files/chart_defs/{filename}"
     return json.loads(read_resource(path))
 
 
 def _load_external_libs():
     to_load = {
-        "vega-embed": "files/external_js/vega-embed@6.20.2",
-        "vega-lite": "files/external_js/vega-lite@5.2.0",
-        "vega": "files/external_js/vega@5.21.0",
+        "vega-embed": "internals/files/external_js/vega-embed@6.20.2",
+        "vega-lite": "internals/files/external_js/vega-lite@5.2.0",
+        "vega": "internals/files/external_js/vega@5.21.0",
     }
     return {k: read_resource(v) for k, v in to_load.items()}
 
 
 def altair_or_json(
     chart_dict: dict[Any, Any], as_dict: bool = False
 ) -> ChartReturnType:
@@ -80,15 +80,15 @@
         raise ValueError(
             f"The path {filename} already exists. Please provide a different path."
         )
 
     if type(chart_dict).__name__ == "VegaliteNoValidate":
         chart_dict = chart_dict.spec
 
-    template = read_resource("files/templates/single_chart_template.html")
+    template = read_resource("internals/files/templates/single_chart_template.html")
 
     fmt_dict = _load_external_libs()
 
     fmt_dict["mychart"] = json.dumps(chart_dict)
 
     with open(filename, "w", encoding="utf-8") as f:
         f.write(template.format(**fmt_dict))
```

### Comparing `splink-4.0.0.dev4/splink/cluster_studio.py` & `splink-4.0.0.dev5/splink/internals/cluster_studio.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 import json
 import os
 import random
 from typing import TYPE_CHECKING, Any, Literal, Optional
 
 from jinja2 import Template
 
-from .exceptions import SplinkException
-from .misc import EverythingEncoder, read_resource
-from .pipeline import CTEPipeline
-from .splink_dataframe import SplinkDataFrame
-from .unique_id_concat import (
+from splink.internals.exceptions import SplinkException
+from splink.internals.misc import EverythingEncoder, read_resource
+from splink.internals.pipeline import CTEPipeline
+from splink.internals.splink_dataframe import SplinkDataFrame
+from splink.internals.unique_id_concat import (
     _composite_unique_id_from_edges_sql,
     _composite_unique_id_from_nodes_sql,
 )
 
 # https://stackoverflow.com/questions/39740632/python-type-hinting-without-cyclic-imports
 if TYPE_CHECKING:
-    from .linker import Linker
+    from splink.internals.linker import Linker
 
 SamplingMethods = Literal[
     "random", "by_cluster_size", "lowest_density_clusters_by_size"
 ]
 
 
 def _quo_if_str(x):
@@ -372,15 +372,15 @@
 
     cluster_recs = df_clusters_as_records(linker, df_clustered_nodes, cluster_ids)
     df_nodes = create_df_nodes(linker, df_clustered_nodes, cluster_ids)
     nodes_recs = df_nodes.as_record_dict()
     edges_recs = df_edges_as_records(linker, df_predicted_edges, df_nodes)
 
     # Render template with cluster, nodes and edges
-    template_path = "files/splink_cluster_studio/cluster_template.j2"
+    template_path = "internals/files/splink_cluster_studio/cluster_template.j2"
     template = Template(read_resource(template_path))
 
     template_data: dict[str, Any] = {
         "raw_edge_data": json.dumps(edges_recs, cls=EverythingEncoder),
         "raw_node_data": json.dumps(nodes_recs, cls=EverythingEncoder),
         "raw_clusters_data": json.dumps(cluster_recs, cls=EverythingEncoder),
         "splink_settings": json.dumps(
@@ -393,20 +393,20 @@
         named_clusters_dict = dict(zip(cluster_ids, cluster_names))
 
         template_data["named_clusters"] = json.dumps(
             named_clusters_dict, cls=EverythingEncoder
         )
 
     files = {
-        "embed": "files/external_js/vega-embed@6.20.2",
-        "stdlib": "files/external_js/stdlib.js@5.8.3",
-        "vega": "files/external_js/vega@5.21.0",
-        "vegalite": "files/external_js/vega-lite@5.2.0",
-        "svu_text": "files/splink_vis_utils/splink_vis_utils.js",
-        "custom_css": "files/splink_cluster_studio/custom.css",
+        "embed": "internals/files/external_js/vega-embed@6.20.2",
+        "stdlib": "internals/files/external_js/stdlib.js@5.8.3",
+        "vega": "internals/files/external_js/vega@5.21.0",
+        "vegalite": "internals/files/external_js/vega-lite@5.2.0",
+        "svu_text": "internals/files/splink_vis_utils/splink_vis_utils.js",
+        "custom_css": "internals/files/splink_cluster_studio/custom.css",
     }
     for k, v in files.items():
         template_data[k] = read_resource(v)
 
     template_data["bundle_observable_notebook"] = bundle_observable_notebook
 
     rendered = template.render(**template_data)
```

### Comparing `splink-4.0.0.dev4/splink/column_expression.py` & `splink-4.0.0.dev5/splink/internals/column_expression.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 from __future__ import annotations
 
 import re
 import string
 from copy import copy
 from functools import partial
-from typing import Callable, Union
+from typing import Protocol, Union
 
 import sqlglot
 
-from .dialects import SplinkDialect
-from .input_column import SqlglotColumnTreeBuilder
-from .sql_transform import (
+from splink.internals.dialects import SplinkDialect
+from splink.internals.input_column import SqlglotColumnTreeBuilder
+from splink.internals.sql_transform import (
     add_suffix_to_all_column_identifiers,
     add_table_to_all_column_identifiers,
 )
 
 
+class ColumnExpressionOperation(Protocol):
+    def __call__(self, name: str, dialect: SplinkDialect) -> str: ...
+
+
 class ColumnExpression:
     """
     Enables transforms to be applied to a column before it's passed into a
     comparison level.
 
     Dialect agnostic.  Execution is delayed until the dialect is known.
 
@@ -36,15 +40,15 @@
     Note that this will typically be created without a dialect, and the dialect
     will later be populated when the ColumnExpression is passed via a comparison
     level creator into a linker.
     """
 
     def __init__(self, sql_expression: str, sql_dialect: SplinkDialect = None):
         self.raw_sql_expression = sql_expression
-        self.operations: list[Callable[..., str]] = []
+        self.operations: list[ColumnExpressionOperation] = []
         if sql_dialect is not None:
             self.sql_dialect: SplinkDialect = sql_dialect
 
     def _clone(self) -> "ColumnExpression":
         clone = copy(self)
         clone.operations = [op for op in self.operations]
         return clone
@@ -109,15 +113,15 @@
             dialect=dialect.sqlglot_name
         )
 
         return lower_sql.replace("___col___", name)
 
     def lower(self) -> "ColumnExpression":
         """
-        Applies a lowercase transofrom to the input expression.
+        Applies a lowercase transform to the input expression.
         """
         clone = self._clone()
         clone.operations.append(clone._lower_dialected)
         return clone
 
     def _substr_dialected(
         self, name: str, start: int, end: int, dialect: SplinkDialect
```

### Comparing `splink-4.0.0.dev4/splink/comparison.py` & `splink-4.0.0.dev5/splink/internals/comparison.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, List, Optional
 
+from splink.internals.misc import (
+    dedupe_preserving_order,
+    join_list_with_commas_final_and,
+)
+
 from .comparison_level import ComparisonLevel, _default_m_values, _default_u_values
-from .misc import dedupe_preserving_order, join_list_with_commas_final_and
 
 # https://stackoverflow.com/questions/39740632/python-type-hinting-without-cyclic-imports
 if TYPE_CHECKING:
-    from .settings import ColumnInfoSettings
+    from splink.internals.settings import ColumnInfoSettings
 
 
 class Comparison:
     """Each Comparison defines how data from one or more input columns is
     compared to assess its similarity.
 
     For example, one Comparison may represent how similarity is assessed for a
@@ -462,11 +466,11 @@
             f"ComparisonLevels:\n{comp_levels}"
         )
 
         return desc
 
     def match_weights_chart(self, as_dict=False):
         """Display a chart of comparison levels of the comparison"""
-        from .charts import comparison_match_weights_chart
+        from splink.internals.charts import comparison_match_weights_chart
 
         records = self._as_detailed_records
         return comparison_match_weights_chart(records, as_dict=as_dict)
```

### Comparing `splink-4.0.0.dev4/splink/comparison_creator.py` & `splink-4.0.0.dev5/splink/internals/comparison_creator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from typing import Any, Dict, List, Optional, Union, final
 
-from .column_expression import ColumnExpression
+from splink.internals.column_expression import ColumnExpression
+from splink.internals.exceptions import SplinkException
+
 from .comparison import Comparison
 from .comparison_level_creator import ComparisonLevelCreator
-from .exceptions import SplinkException
 
 
 class ComparisonCreator(ABC):
     DEFAULT_COL_EXP_KEY = "__default__"
 
     def __init__(
         self,
```

### Comparing `splink-4.0.0.dev4/splink/comparison_helpers.py` & `splink-4.0.0.dev5/splink/internals/comparison_helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import duckdb
 import pandas as pd
 import phonetics
 
-from .charts import (
+from splink.internals.charts import (
     _comparator_score_chart,
     _comparator_score_threshold_chart,
     _phonetic_match_chart,
 )
 
 comparator_cols_sql = """
     levenshtein({comparison1}, {comparison2}) as levenshtein_distance,
```

### Comparing `splink-4.0.0.dev4/splink/comparison_level.py` & `splink-4.0.0.dev5/splink/internals/comparison_level.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,24 +9,24 @@
 from typing import Any, Optional, Union, cast
 
 import sqlglot
 from sqlglot.expressions import Column, Identifier
 from sqlglot.optimizer.normalize import normalize
 from sqlglot.optimizer.simplify import simplify
 
-from .constants import LEVEL_NOT_OBSERVED_TEXT
-from .input_column import InputColumn
-from .misc import (
+from splink.internals.constants import LEVEL_NOT_OBSERVED_TEXT
+from splink.internals.input_column import InputColumn
+from splink.internals.misc import (
     dedupe_preserving_order,
     interpolate,
     join_list_with_commas_final_and,
     match_weight_to_bayes_factor,
 )
-from .parse_sql import get_columns_used_from_sql
-from .sql_transform import sqlglot_tree_signature
+from splink.internals.parse_sql import get_columns_used_from_sql
+from splink.internals.sql_transform import sqlglot_tree_signature
 
 logger = logging.getLogger(__name__)
 
 
 def _is_exact_match(sql_syntax_tree):
     signature = sqlglot_tree_signature(sql_syntax_tree)
```

### Comparing `splink-4.0.0.dev4/splink/comparison_level_composition.py` & `splink-4.0.0.dev5/splink/internals/comparison_level_composition.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from __future__ import annotations
 
 from typing import Any, Iterable, Union, final
 
-from .blocking import BlockingRule
+from splink.internals.blocking import BlockingRule
+from splink.internals.dialects import SplinkDialect
+
 from .comparison_creator import ComparisonLevelCreator
 from .comparison_level import ComparisonLevel
-from .dialects import SplinkDialect
 
 
 def _ensure_is_comparison_level_creator(
     cl: Union[ComparisonLevelCreator, dict[str, Any]],
 ) -> ComparisonLevelCreator:
     if isinstance(cl, dict):
         from .comparison_level_library import CustomLevel
```

### Comparing `splink-4.0.0.dev4/splink/comparison_level_creator.py` & `splink-4.0.0.dev5/splink/internals/comparison_level_creator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from inspect import signature
 from typing import Any, final
 
-from .column_expression import ColumnExpression
+from splink.internals.column_expression import ColumnExpression
+from splink.internals.dialects import SplinkDialect
+
 from .comparison_level import ComparisonLevel
-from .dialects import SplinkDialect
 
 
 class ComparisonLevelCreator(ABC):
     # off by default - only a small subset should have tf adjustments
     term_frequency_adjustments = False
 
     @abstractmethod
```

### Comparing `splink-4.0.0.dev4/splink/comparison_level_library.py` & `splink-4.0.0.dev5/splink/internals/comparison_level_library.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from __future__ import annotations
 
+from copy import copy
 from functools import wraps
-from typing import Callable, List, Literal, TypeVar, Union
+from typing import Any, Callable, List, Literal, TypeVar, Union
 
 from sqlglot import TokenError, parse_one
 
-from .column_expression import ColumnExpression
+from splink.internals.column_expression import ColumnExpression
+from splink.internals.comparison_level_sql import great_circle_distance_km_sql
+from splink.internals.dialects import SplinkDialect
 
 # import composition functions for export
 from .comparison_level_composition import And, Not, Or  # NOQA: F401
 from .comparison_level_creator import ComparisonLevelCreator
-from .comparison_level_sql import great_circle_distance_km_sql
-from .dialects import SplinkDialect
 
 # type aliases:
 T = TypeVar("T", bound=ComparisonLevelCreator)
 CreateSQLFunctionType = Callable[[T, SplinkDialect], str]
 
 
 def unsupported_splink_dialects(
@@ -166,14 +167,54 @@
     def create_label_for_charts(self) -> str:
         return (
             self.label_for_charts
             if self.label_for_charts is not None
             else self.sql_condition
         )
 
+    @staticmethod
+    def _convert_to_creator(
+        cl: Union[ComparisonLevelCreator, dict[str, Any]],
+    ) -> ComparisonLevelCreator:
+        if isinstance(cl, ComparisonLevelCreator):
+            return cl
+        if isinstance(cl, dict):
+            # TODO: swap this if we develop a more uniform approach to (de)serialising
+            cl_dict = copy(cl)
+            configurable_parameters = (
+                "is_null_level",
+                "m_probability",
+                "u_probability",
+                "tf_adjustment_column",
+                "tf_adjustment_weight",
+                "tf_minimum_u_value",
+                "label_for_charts",
+                "disable_tf_exact_match_detection",
+            )
+            # split dict in two depending whether or not entries are 'configurables'
+            configurables = {
+                key: value
+                for key, value in cl_dict.items()
+                if key in configurable_parameters
+            }
+            cl_dict = {
+                key: value
+                for key, value in cl_dict.items()
+                if key not in configurable_parameters
+            }
+
+            custom_comparison = CustomLevel(**cl_dict)
+            if configurables:
+                custom_comparison.configure(**configurables)
+            return custom_comparison
+        raise ValueError(
+            "`comparison_levels` entries must be `dict` or `ComparisonLevelCreator, "
+            f"but found type {type(cl)} for entry {cl}"
+        )
+
 
 class ExactMatchLevel(ComparisonLevelCreator):
     def __init__(
         self,
         col_name: Union[str, ColumnExpression],
         term_frequency_adjustments: bool = False,
     ):
```

### Comparing `splink-4.0.0.dev4/splink/comparison_level_sql.py` & `splink-4.0.0.dev5/splink/internals/comparison_level_sql.py`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev4/splink/comparison_library.py` & `splink-4.0.0.dev5/splink/internals/comparison_library.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from __future__ import annotations
 
-from copy import copy
 from typing import Any, Iterable, List, Optional, Union
 
-from . import comparison_level_library as cll
-from .comparison_creator import ComparisonCreator
-from .comparison_level_creator import ComparisonLevelCreator
-from .comparison_level_library import CustomLevel, DateMetricType
-from .misc import ensure_is_iterable
+from splink.internals import comparison_level_library as cll
+from splink.internals.comparison_creator import ComparisonCreator
+from splink.internals.comparison_level_creator import ComparisonLevelCreator
+from splink.internals.comparison_level_library import CustomLevel, DateMetricType
+from splink.internals.misc import ensure_is_iterable
 
 
 class CustomComparison(ComparisonCreator):
     def __init__(
         self,
         comparison_levels: List[Union[ComparisonLevelCreator, dict[str, Any]]],
         output_column_name: str = None,
@@ -32,57 +31,17 @@
         self._output_column_name = output_column_name
         self._comparison_levels = comparison_levels
         self._description = comparison_description
         # we deliberately don't call super().__init__() - all that does is set up
         # column expressions, which we do not need here as we are dealing with
         # levels directly
 
-    @staticmethod
-    def _convert_to_creator(
-        cl: Union[ComparisonLevelCreator, dict[str, Any]],
-    ) -> ComparisonLevelCreator:
-        if isinstance(cl, ComparisonLevelCreator):
-            return cl
-        if isinstance(cl, dict):
-            # TODO: swap this if we develop a more uniform approach to (de)serialising
-            cl_dict = copy(cl)
-            configurable_parameters = (
-                "is_null_level",
-                "m_probability",
-                "u_probability",
-                "tf_adjustment_column",
-                "tf_adjustment_weight",
-                "tf_minimum_u_value",
-                "label_for_charts",
-                "disable_tf_exact_match_detection",
-            )
-            # split dict in two depending whether or not entries are 'configurables'
-            configurables = {
-                key: value
-                for key, value in cl_dict.items()
-                if key in configurable_parameters
-            }
-            cl_dict = {
-                key: value
-                for key, value in cl_dict.items()
-                if key not in configurable_parameters
-            }
-
-            custom_comparison = CustomLevel(**cl_dict)
-            if configurables:
-                custom_comparison.configure(**configurables)
-            return custom_comparison
-        raise ValueError(
-            "`comparison_levels` entries must be `dict` or `ComparisonLevelCreator, "
-            f"but found type {type(cl)} for entry {cl}"
-        )
-
     def create_comparison_levels(self) -> List[ComparisonLevelCreator]:
         comparison_level_creators = [
-            self._convert_to_creator(cl) for cl in self._comparison_levels
+            CustomLevel._convert_to_creator(cl) for cl in self._comparison_levels
         ]
         return comparison_level_creators
 
     def create_description(self) -> str:
         # TODO: fleshed out default description?
         return (
             self._description
@@ -90,14 +49,22 @@
             else f"Comparison for {self._output_column_name}"
         )
 
     def create_output_column_name(self) -> Optional[str]:
         # TODO: should default logic be here? would need column-extraction logic also
         return self._output_column_name
 
+    @staticmethod
+    def _convert_to_creator(
+        comparison_creator: dict[str, Any] | ComparisonCreator,
+    ) -> ComparisonCreator:
+        if isinstance(comparison_creator, dict):
+            return CustomComparison(**comparison_creator)
+        return comparison_creator
+
 
 class ExactMatch(ComparisonCreator):
     """
     Represents a comparison of the data in `col_name` with two levels:
         - Exact match in `col_name`
         - Anything else
```

### Comparing `splink-4.0.0.dev4/splink/comparison_template_library.py` & `splink-4.0.0.dev5/splink/internals/comparison_template_library.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from __future__ import annotations
 
 from typing import List, Type, Union
 
-from . import comparison_level_library as cll
-from .column_expression import ColumnExpression
-from .comparison_creator import ComparisonCreator
-from .comparison_level_creator import ComparisonLevelCreator
-from .comparison_level_library import DateMetricType
-from .misc import ensure_is_iterable
+from splink.internals import comparison_level_library as cll
+from splink.internals.column_expression import ColumnExpression
+from splink.internals.comparison_creator import ComparisonCreator
+from splink.internals.comparison_level_creator import ComparisonLevelCreator
+from splink.internals.comparison_level_library import DateMetricType
+from splink.internals.misc import ensure_is_iterable
 
 # alternatively we could stick an inheritance layer in these, just for typing:
 _fuzzy_cll_type = Union[
     Type[cll.DamerauLevenshteinLevel],
     Type[cll.JaroLevel],
     Type[cll.JaroWinklerLevel],
     Type[cll.LevenshteinLevel],
```

### Comparing `splink-4.0.0.dev4/splink/comparison_vector_distribution.py` & `splink-4.0.0.dev5/splink/internals/comparison_vector_distribution.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 # https://stackoverflow.com/questions/39740632/python-type-hinting-without-cyclic-imports
 if TYPE_CHECKING:
-    from ..linker import Linker
+    from splink.internals.linker import Linker
 
 
 def comparison_vector_distribution_sql(linker: Linker) -> str:
     gamma_columns = [c._gamma_column_name for c in linker._settings_obj.comparisons]
     groupby_cols = " , ".join(gamma_columns)
     gam_concat = " || ',' || ".join(gamma_columns)
```

### Comparing `splink-4.0.0.dev4/splink/comparison_vector_values.py` & `splink-4.0.0.dev5/splink/internals/comparison_vector_values.py`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev4/splink/connected_components.py` & `splink-4.0.0.dev5/splink/internals/connected_components.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,24 +9,24 @@
 # https://stackoverflow.com/questions/39740632/python-type-hinting-without-cyclic-imports
 from __future__ import annotations
 
 import logging
 import time
 from typing import TYPE_CHECKING, Optional
 
-from .input_column import InputColumn
-from .pipeline import CTEPipeline
-from .splink_dataframe import SplinkDataFrame
-from .unique_id_concat import (
+from splink.internals.input_column import InputColumn
+from splink.internals.pipeline import CTEPipeline
+from splink.internals.splink_dataframe import SplinkDataFrame
+from splink.internals.unique_id_concat import (
     _composite_unique_id_from_edges_sql,
     _composite_unique_id_from_nodes_sql,
 )
 
 if TYPE_CHECKING:
-    from .linker import Linker
+    from splink.internals.linker import Linker
 
 logger = logging.getLogger(__name__)
 
 
 def _cc_create_nodes_table(linker: "Linker", generated_graph: bool = False) -> str:
     """SQL to create our connected components nodes table.
```

### Comparing `splink-4.0.0.dev4/splink/cost_of_blocking_rules.py` & `splink-4.0.0.dev5/splink/internals/cost_of_blocking_rules.py`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev4/splink/database_api.py` & `splink-4.0.0.dev5/splink/internals/database_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,23 +7,24 @@
 from abc import ABC, abstractmethod
 from collections.abc import Sequence
 from typing import Any, Dict, Generic, List, Optional, TypeVar, Union, final
 
 import sqlglot
 from pandas import DataFrame as PandasDataFrame
 
-from .cache_dict_with_logging import CacheDictWithLogging
+from splink.internals.cache_dict_with_logging import CacheDictWithLogging
+from splink.internals.logging_messages import execute_sql_logging_message_info, log_sql
+from splink.internals.misc import ascii_uid, ensure_is_list, parse_duration
+from splink.internals.pipeline import CTEPipeline
+from splink.internals.splink_dataframe import SplinkDataFrame
+
 from .dialects import (
     SplinkDialect,
 )
 from .exceptions import SplinkException
-from .logging_messages import execute_sql_logging_message_info, log_sql
-from .misc import ascii_uid, ensure_is_list, parse_duration
-from .pipeline import CTEPipeline
-from .splink_dataframe import SplinkDataFrame
 
 logger = logging.getLogger(__name__)
 
 # minimal acceptable table types
 AcceptableInputTableType = Union[
     str, PandasDataFrame, List[Dict[str, Any]], Dict[str, Any]
 ]
```

### Comparing `splink-4.0.0.dev4/splink/databricks/enable_splink.py` & `splink-4.0.0.dev5/splink/internals/databricks/enable_splink.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 
-from splink.spark.jar_location import similarity_jar_location
+from splink.internals.spark.jar_location import similarity_jar_location
 
 logger = logging.getLogger(__name__)
 
 
 def enable_splink(spark):
     """
     Enable Splink functions.
```

### Comparing `splink-4.0.0.dev4/splink/datasets/__init__.py` & `splink-4.0.0.dev5/splink/internals/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev4/splink/default_from_jsonschema.py` & `splink-4.0.0.dev5/splink/internals/default_from_jsonschema.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from copy import deepcopy
 
-from .validate_jsonschema import get_schema
+from splink.internals.validate_jsonschema import get_schema
 
 
 def default_value_from_schema(key, schema_part):
     schema = deepcopy(get_schema())
     if schema_part == "root":
         return schema["properties"][key]["default"]
```

### Comparing `splink-4.0.0.dev4/splink/dialects.py` & `splink-4.0.0.dev5/splink/internals/dialects.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from abc import ABC, abstractproperty
 from typing import TYPE_CHECKING, Type, TypeVar, final
 
 if TYPE_CHECKING:
-    from .comparison_level_library import (
+    from splink.internals.comparison_level_library import (
         AbsoluteTimeDifferenceLevel,
         ArrayIntersectLevel,
     )
 
 # equivalent to typing.Self in python >= 3.11
 Self = TypeVar("Self", bound="SplinkDialect")
 
@@ -493,16 +493,7 @@
     @property
     def sqlglot_name(self):
         return "presto"
 
     @property
     def _levenshtein_name(self):
         return "levenshtein_distance"
-
-
-_dialect_lookup = {
-    "duckdb": DuckDBDialect(),
-    "spark": SparkDialect(),
-    "sqlite": SQLiteDialect(),
-    "postgres": PostgresDialect(),
-    "athena": AthenaDialect(),
-}
```

### Comparing `splink-4.0.0.dev4/splink/duckdb/database_api.py` & `splink-4.0.0.dev5/splink/internals/duckdb/database_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 
 import logging
 from typing import Sequence, Union
 
 import duckdb
 import pandas as pd
 
-from ..database_api import AcceptableInputTableType, DatabaseAPI
-from ..dialects import (
+from splink.internals.database_api import AcceptableInputTableType, DatabaseAPI
+from splink.internals.dialects import (
     DuckDBDialect,
 )
+
 from .dataframe import DuckDBDataFrame
 from .duckdb_helpers.duckdb_helpers import (
     create_temporary_duckdb_connection,
     duckdb_load_from_file,
     validate_duckdb_connection,
 )
```

### Comparing `splink-4.0.0.dev4/splink/duckdb/dataframe.py` & `splink-4.0.0.dev5/splink/internals/duckdb/dataframe.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import logging
 import os
 from typing import TYPE_CHECKING
 
-from ..input_column import InputColumn
-from ..splink_dataframe import SplinkDataFrame
+from splink.internals.input_column import InputColumn
+from splink.internals.splink_dataframe import SplinkDataFrame
 
 logger = logging.getLogger(__name__)
 if TYPE_CHECKING:
     from .database_api import DuckDBAPI
 
 
 class DuckDBDataFrame(SplinkDataFrame):
```

### Comparing `splink-4.0.0.dev4/splink/duckdb/duckdb_helpers/duckdb_helpers.py` & `splink-4.0.0.dev5/splink/internals/duckdb/duckdb_helpers/duckdb_helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     )
 
 
 def create_temporary_duckdb_connection(self):
     """
     Create a temporary duckdb connection.
     """
-    self._temp_dir = tempfile.TemporaryDirectory(dir=".")
+    self._temp_dir = tempfile.TemporaryDirectory(dir="")
     fname = uuid.uuid4().hex[:7]
     path = os.path.join(self._temp_dir.name, f"{fname}.duckdb")
     con = duckdb.connect(database=path, read_only=False)
     return con
 
 
 def duckdb_load_from_file(path: str) -> str:
```

### Comparing `splink-4.0.0.dev4/splink/edge_metrics.py` & `splink-4.0.0.dev5/splink/internals/edge_metrics.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 from __future__ import annotations
 
 import logging
 from typing import TYPE_CHECKING
 
-from .exceptions import MissingDependencyException
-from .graph_metrics import (
+from splink.internals.graph_metrics import (
     _basic_edge_metrics_sql,
     _bridges_from_igraph_sql,
     _edges_for_igraph_sql,
     _full_bridges_sql,
     _node_mapping_table_sql,
     _truncated_edges_sql,
 )
-from .pipeline import CTEPipeline
-from .splink_dataframe import SplinkDataFrame
-from .unique_id_concat import (
+from splink.internals.pipeline import CTEPipeline
+from splink.internals.splink_dataframe import SplinkDataFrame
+from splink.internals.unique_id_concat import (
     _composite_unique_id_from_edges_sql,
 )
 
+from .exceptions import MissingDependencyException
+
 if TYPE_CHECKING:
-    from .linker import Linker
+    from splink.internals.linker import Linker
 
 logger = logging.getLogger(__name__)
 
 
 def compute_edge_metrics(
     linker: Linker,
     df_node_metrics: SplinkDataFrame,
```

### Comparing `splink-4.0.0.dev4/splink/em_training_session.py` & `splink-4.0.0.dev5/splink/internals/em_training_session.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,43 +1,46 @@
 from __future__ import annotations
 
 import logging
 from typing import TYPE_CHECKING, List
 
-from .blocking import BlockingRule, block_using_rules_sqls
-from .charts import (
+from splink.internals.blocking import BlockingRule, block_using_rules_sqls
+from splink.internals.charts import (
     m_u_parameters_interactive_history_chart,
     match_weights_interactive_history_chart,
     probability_two_random_records_match_iteration_chart,
 )
-from .comparison import Comparison
-from .comparison_level import ComparisonLevel
-from .comparison_vector_values import compute_comparison_vector_values_sql
-from .constants import LEVEL_NOT_OBSERVED_TEXT
-from .database_api import DatabaseAPISubClass
-from .exceptions import EMTrainingException
-from .expectation_maximisation import expectation_maximisation
-from .input_column import InputColumn
-from .misc import bayes_factor_to_prob, prob_to_bayes_factor
-from .parse_sql import get_columns_used_from_sql
-from .pipeline import CTEPipeline
-from .settings import (
+from splink.internals.comparison import Comparison
+from splink.internals.comparison_level import ComparisonLevel
+from splink.internals.comparison_vector_values import (
+    compute_comparison_vector_values_sql,
+)
+from splink.internals.constants import LEVEL_NOT_OBSERVED_TEXT
+from splink.internals.input_column import InputColumn
+from splink.internals.misc import bayes_factor_to_prob, prob_to_bayes_factor
+from splink.internals.parse_sql import get_columns_used_from_sql
+from splink.internals.pipeline import CTEPipeline
+from splink.internals.settings import (
     ComparisonAndLevelDict,
     CoreModelSettings,
     Settings,
     TrainingSettings,
 )
-from .vertically_concatenate import compute_df_concat_with_tf
+from splink.internals.vertically_concatenate import compute_df_concat_with_tf
+
+from .database_api import DatabaseAPISubClass
+from .exceptions import EMTrainingException
+from .expectation_maximisation import expectation_maximisation
 
 logger = logging.getLogger(__name__)
 
 # https://stackoverflow.com/questions/39740632/python-type-hinting-without-cyclic-imports
 if TYPE_CHECKING:
-    from .linker import Linker
-    from .splink_dataframe import SplinkDataFrame
+    from splink.internals.linker import Linker
+    from splink.internals.splink_dataframe import SplinkDataFrame
 
 
 class EMTrainingSession:
     """Manages training models using the Expectation Maximisation algorithm, and
     holds statistics on the evolution of parameter estimates.  Plots diagnostic charts
     """
```

### Comparing `splink-4.0.0.dev4/splink/estimate_u.py` & `splink-4.0.0.dev5/splink/internals/estimate_u.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 from __future__ import annotations
 
 import logging
 import multiprocessing
 from copy import deepcopy
 from typing import TYPE_CHECKING, List
 
-from .blocking import block_using_rules_sqls, blocking_rule_to_obj
-from .comparison_vector_values import compute_comparison_vector_values_sql
-from .expectation_maximisation import (
-    compute_new_parameters_sql,
-    compute_proportions_for_new_parameters,
+from splink.internals.blocking import block_using_rules_sqls, blocking_rule_to_obj
+from splink.internals.comparison_vector_values import (
+    compute_comparison_vector_values_sql,
 )
-from .m_u_records_to_parameters import (
+from splink.internals.m_u_records_to_parameters import (
     append_u_probability_to_comparison_level_trained_probabilities,
     m_u_records_to_lookup_dict,
 )
-from .pipeline import CTEPipeline
-from .vertically_concatenate import (
+from splink.internals.pipeline import CTEPipeline
+from splink.internals.vertically_concatenate import (
     enqueue_df_concat,
     split_df_concat_with_tf_into_two_tables_sqls,
 )
 
+from .expectation_maximisation import (
+    compute_new_parameters_sql,
+    compute_proportions_for_new_parameters,
+)
+
 # https://stackoverflow.com/questions/39740632/python-type-hinting-without-cyclic-imports
 if TYPE_CHECKING:
-    from .linker import Linker
+    from splink.internals.linker import Linker
 
 logger = logging.getLogger(__name__)
 
 
 def _rows_needed_for_n_pairs(n_pairs):
     # Number of pairs generated by cartesian product is
     # p(r) = r(r-1)/2, where r is input rows
```

### Comparing `splink-4.0.0.dev4/splink/exceptions.py` & `splink-4.0.0.dev5/splink/internals/exceptions.py`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev4/splink/expectation_maximisation.py` & `splink-4.0.0.dev5/splink/internals/expectation_maximisation.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,27 +2,28 @@
 
 import logging
 import time
 from typing import Any, List, cast
 
 import pandas as pd
 
-from .comparison import Comparison
-from .comparison_level import ComparisonLevel
-from .constants import LEVEL_NOT_OBSERVED_TEXT
-from .database_api import DatabaseAPISubClass
-from .input_column import InputColumn
-from .m_u_records_to_parameters import m_u_records_to_lookup_dict
-from .pipeline import CTEPipeline
-from .predict import (
+from splink.internals.comparison import Comparison
+from splink.internals.comparison_level import ComparisonLevel
+from splink.internals.constants import LEVEL_NOT_OBSERVED_TEXT
+from splink.internals.input_column import InputColumn
+from splink.internals.m_u_records_to_parameters import m_u_records_to_lookup_dict
+from splink.internals.pipeline import CTEPipeline
+from splink.internals.predict import (
     predict_from_agreement_pattern_counts_sqls,
     predict_from_comparison_vectors_sqls,
 )
-from .settings import CoreModelSettings, TrainingSettings
-from .splink_dataframe import SplinkDataFrame
+from splink.internals.settings import CoreModelSettings, TrainingSettings
+from splink.internals.splink_dataframe import SplinkDataFrame
+
+from .database_api import DatabaseAPISubClass
 
 logger = logging.getLogger(__name__)
 
 
 def count_agreement_patterns_sql(comparisons: List[Comparison]) -> str:
     """Count how many times each realized agreement pattern
     was observed across the blocked dataset."""
```

### Comparing `splink-4.0.0.dev4/splink/files/DEPENDENCY_LICENSES.txt` & `splink-4.0.0.dev5/splink/internals/files/DEPENDENCY_LICENSES.txt`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev4/splink/files/chart_defs/accuracy_chart.json` & `splink-4.0.0.dev5/splink/internals/files/chart_defs/accuracy_chart.json`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev4/splink/files/chart_defs/blocking_rule_generated_comparisons.json` & `splink-4.0.0.dev5/splink/internals/files/chart_defs/blocking_rule_generated_comparisons.json`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev4/splink/files/chart_defs/comparator_score_chart.json` & `splink-4.0.0.dev5/splink/internals/files/chart_defs/comparator_score_chart.json`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev4/splink/files/chart_defs/comparator_score_threshold_chart.json` & `splink-4.0.0.dev5/splink/internals/files/chart_defs/comparator_score_threshold_chart.json`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev4/splink/files/chart_defs/completeness.json` & `splink-4.0.0.dev5/splink/internals/files/chart_defs/completeness.json`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev4/splink/files/chart_defs/m_u_parameters_interactive_history.json` & `splink-4.0.0.dev5/splink/internals/files/chart_defs/m_u_parameters_interactive_history.json`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev4/splink/files/chart_defs/match_weight_histogram.json` & `splink-4.0.0.dev5/splink/internals/files/chart_defs/match_weight_histogram.json`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev4/splink/files/chart_defs/match_weights_interactive_history.json` & `splink-4.0.0.dev5/splink/internals/files/chart_defs/match_weights_interactive_history.json`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev4/splink/files/chart_defs/match_weights_waterfall.json` & `splink-4.0.0.dev5/splink/internals/files/chart_defs/match_weights_waterfall.json`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev4/splink/files/chart_defs/missingness.json` & `splink-4.0.0.dev5/splink/internals/files/chart_defs/missingness.json`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev4/splink/files/chart_defs/parameter_estimate_comparisons.json` & `splink-4.0.0.dev5/splink/internals/files/chart_defs/parameter_estimate_comparisons.json`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev4/splink/files/chart_defs/phonetic_match_chart.json` & `splink-4.0.0.dev5/splink/internals/files/chart_defs/phonetic_match_chart.json`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev4/splink/files/chart_defs/precision_recall.json` & `splink-4.0.0.dev5/splink/internals/files/chart_defs/precision_recall.json`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev4/splink/files/chart_defs/probability_two_random_records_match_iteration.json` & `splink-4.0.0.dev5/splink/internals/files/chart_defs/probability_two_random_records_match_iteration.json`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev4/splink/files/chart_defs/profile_data.json` & `splink-4.0.0.dev5/splink/internals/files/chart_defs/profile_data.json`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev4/splink/files/chart_defs/roc.json` & `splink-4.0.0.dev5/splink/internals/files/chart_defs/roc.json`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev4/splink/files/chart_defs/tf_adjustment_chart.json` & `splink-4.0.0.dev5/splink/internals/files/chart_defs/tf_adjustment_chart.json`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev4/splink/files/chart_defs/threshold_selection_tool.json` & `splink-4.0.0.dev5/splink/internals/files/chart_defs/threshold_selection_tool.json`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev4/splink/files/chart_defs/unlinkables_chart_def.json` & `splink-4.0.0.dev5/splink/internals/files/chart_defs/unlinkables_chart_def.json`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev4/splink/files/external_js/d3@7.8.5` & `splink-4.0.0.dev5/splink/internals/files/external_js/d3@7.8.5`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev4/splink/files/external_js/stdlib.js@5.8.3` & `splink-4.0.0.dev5/splink/internals/files/external_js/stdlib.js@5.8.3`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev4/splink/files/external_js/vega-embed@6.20.2` & `splink-4.0.0.dev5/splink/internals/files/external_js/vega-embed@6.20.2`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev4/splink/files/external_js/vega-lite@5.2.0` & `splink-4.0.0.dev5/splink/internals/files/external_js/vega-lite@5.2.0`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev4/splink/files/external_js/vega@5.21.0` & `splink-4.0.0.dev5/splink/internals/files/external_js/vega@5.21.0`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev4/splink/files/labelling_tool/slt.js` & `splink-4.0.0.dev5/splink/internals/files/labelling_tool/slt.js`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev4/splink/files/labelling_tool/template.j2` & `splink-4.0.0.dev5/splink/internals/files/labelling_tool/template.j2`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev4/splink/files/settings_jsonschema.json` & `splink-4.0.0.dev5/splink/internals/files/settings_jsonschema.json`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev4/splink/files/spark_jars/scala-udf-similarity-0.1.0_classic.jar` & `splink-4.0.0.dev5/splink/internals/files/spark_jars/scala-udf-similarity-0.1.0_classic.jar`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev4/splink/files/spark_jars/scala-udf-similarity-0.1.0_spark3.3.jar` & `splink-4.0.0.dev5/splink/internals/files/spark_jars/scala-udf-similarity-0.1.0_spark3.3.jar`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev4/splink/files/spark_jars/scala-udf-similarity-0.1.1_spark3.x.jar` & `splink-4.0.0.dev5/splink/internals/files/spark_jars/scala-udf-similarity-0.1.1_spark3.x.jar`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev4/splink/files/splink_cluster_studio/cluster_template.j2` & `splink-4.0.0.dev5/splink/internals/files/splink_cluster_studio/cluster_template.j2`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev4/splink/files/splink_cluster_studio/custom.css` & `splink-4.0.0.dev5/splink/internals/files/splink_cluster_studio/custom.css`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev4/splink/files/splink_comparison_viewer/custom.css` & `splink-4.0.0.dev5/splink/internals/files/splink_comparison_viewer/custom.css`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev4/splink/files/splink_comparison_viewer/template.j2` & `splink-4.0.0.dev5/splink/internals/files/splink_comparison_viewer/template.j2`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev4/splink/files/splink_vis_utils/splink_vis_utils.js` & `splink-4.0.0.dev5/splink/internals/files/splink_vis_utils/splink_vis_utils.js`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev4/splink/find_brs_with_comparison_counts_below_threshold.py` & `splink-4.0.0.dev5/splink/internals/find_brs_with_comparison_counts_below_threshold.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,25 +2,26 @@
 
 import logging
 import string
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Sequence, Set
 
 import pandas as pd
 
-from .blocking import BlockingRule
-from .blocking_rule_creator import BlockingRuleCreator
-from .blocking_rule_library import CustomRule, block_on
-from .database_api import DatabaseAPISubClass
-from .input_column import InputColumn
-from .internals.blocking_analysis import (
+from splink.internals.blocking import BlockingRule
+from splink.internals.blocking_analysis import (
     _count_comparisons_generated_from_blocking_rule,
 )
+from splink.internals.blocking_rule_creator import BlockingRuleCreator
+from splink.internals.blocking_rule_library import CustomRule, block_on
+from splink.internals.database_api import DatabaseAPISubClass
+
+from .input_column import InputColumn
 
 if TYPE_CHECKING:
-    from .linker import Linker
+    from splink.internals.linker import Linker
 logger = logging.getLogger(__name__)
 
 
 def sanitise_column_name_for_one_hot_encoding(column_name: str) -> str:
     allowed_chars = string.ascii_letters + string.digits + "_"
     sanitised_name = "".join(c for c in column_name if c in allowed_chars)
     return sanitised_name
@@ -161,16 +162,16 @@
 
     comparison_count = _count_comparisons_generated_from_blocking_rule(
         splink_df_dict=linker._input_tables_dict,
         blocking_rule=br,
         link_type=linker._settings_obj._link_type,
         db_api=linker.db_api,
         compute_post_filter_count=False,
-        source_dataset_column_name=linker._settings_obj.column_info_settings.source_dataset_column_name,
-        unique_id_column_name=linker._settings_obj.column_info_settings.unique_id_column_name,
+        source_dataset_input_column=linker._settings_obj.column_info_settings.source_dataset_input_column,
+        unique_id_input_column=linker._settings_obj.column_info_settings.unique_id_input_column,
     )["number_of_comparisons_generated_pre_filter_conditions"]
 
     already_visited.add(frozenset(current_combination))
 
     # int just to satisfy mypy
     comparison_count = int(comparison_count)
     if comparison_count > threshold:
```

### Comparing `splink-4.0.0.dev4/splink/find_matches_to_new_records.py` & `splink-4.0.0.dev5/splink/internals/find_matches_to_new_records.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
+from splink.internals.pipeline import CTEPipeline
+
 from .input_column import InputColumn
-from .pipeline import CTEPipeline
 
 if TYPE_CHECKING:
-    from .linker import Linker
-    from .splink_dataframe import SplinkDataFrame
+    from splink.internals.linker import Linker
+    from splink.internals.splink_dataframe import SplinkDataFrame
 
 
 def add_unique_id_and_source_dataset_cols_if_needed(
     linker: "Linker", new_records_df: "SplinkDataFrame", pipeline: CTEPipeline
 ) -> CTEPipeline:
     input_cols: list[InputColumn] = new_records_df.columns
     cols: list[str] = [c.unquote().name for c in input_cols]
```

### Comparing `splink-4.0.0.dev4/splink/graph_metrics.py` & `splink-4.0.0.dev5/splink/internals/graph_metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 from typing import Dict, List
 
-from splink.splink_dataframe import SplinkDataFrame
+from splink.internals.splink_dataframe import SplinkDataFrame
 
 
 def _truncated_edges_sql(
     df_predict: SplinkDataFrame,
     threshold_match_probability: float,
 ) -> Dict[str, str]:
     """
```

### Comparing `splink-4.0.0.dev4/splink/input_column.py` & `splink-4.0.0.dev5/splink/internals/input_column.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 from copy import deepcopy
 from dataclasses import dataclass, replace
 from typing import TYPE_CHECKING, Optional, Type
 
 import sqlglot
 import sqlglot.expressions as exp
 
-from .sql_transform import sqlglot_tree_signature
+from splink.internals.sql_transform import sqlglot_tree_signature
 
 if TYPE_CHECKING:
-    from .settings import ColumnInfoSettings
+    from splink.internals.settings import ColumnInfoSettings
 
 
 @dataclass(frozen=True)
 class SqlglotColumnTreeBuilder:
     """
     Builds a sqlglot expression tree representing a column or column reference
     from its arguments.
```

### Comparing `splink-4.0.0.dev4/splink/internals/blocking_analysis.py` & `splink-4.0.0.dev5/splink/internals/blocking_analysis.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,83 +2,74 @@
 
 import logging
 from typing import Any, Dict, Iterable, List, Optional, Sequence, Tuple, Union
 
 import pandas as pd
 import sqlglot
 
-from ..blocking import (
+from splink.internals.blocking import (
     BlockingRule,
     _sql_gen_where_condition,
     backend_link_type_options,
     block_using_rules_sqls,
     materialise_exploded_id_tables,
     user_input_link_type_options,
 )
-from ..blocking_rule_creator import BlockingRuleCreator
-from ..blocking_rule_creator_utils import to_blocking_rule_creator
-from ..charts import ChartReturnType, cumulative_blocking_rule_comparisons_generated
-from ..database_api import AcceptableInputTableType, DatabaseAPISubClass
-from ..input_column import InputColumn
-from ..misc import calculate_cartesian, ensure_is_iterable
-from ..pipeline import CTEPipeline
-from ..splink_dataframe import SplinkDataFrame
-from ..vertically_concatenate import (
+from splink.internals.blocking_rule_creator import BlockingRuleCreator
+from splink.internals.blocking_rule_creator_utils import to_blocking_rule_creator
+from splink.internals.charts import (
+    ChartReturnType,
+    cumulative_blocking_rule_comparisons_generated,
+)
+from splink.internals.database_api import AcceptableInputTableType, DatabaseAPISubClass
+from splink.internals.input_column import InputColumn
+from splink.internals.misc import calculate_cartesian, ensure_is_iterable
+from splink.internals.pipeline import CTEPipeline
+from splink.internals.splink_dataframe import SplinkDataFrame
+from splink.internals.vertically_concatenate import (
     split_df_concat_with_tf_into_two_tables_sqls,
     vertically_concatenate_sql,
 )
 
 logger = logging.getLogger(__name__)
 
 
 def _number_of_comparisons_generated_by_blocking_rule_post_filters_sqls(
     input_data_dict: dict[str, "SplinkDataFrame"],
     blocking_rule: "BlockingRule",
     link_type: backend_link_type_options,
     db_api: DatabaseAPISubClass,
-    unique_id_column_name: str,
-    source_dataset_column_name: Optional[str],
+    unique_id_input_column: InputColumn,
+    source_dataset_input_column: Optional[InputColumn],
 ) -> list[dict[str, str]]:
     input_dataframes = list(input_data_dict.values())
 
     two_dataset_link_only = link_type == "link_only" and len(input_dataframes) == 2
     if two_dataset_link_only:
         link_type = "two_dataset_link_only"
 
-    source_dataset_input_column, unique_id_input_column = _process_unique_id_columns(
-        unique_id_column_name,
-        source_dataset_column_name,
-        input_data_dict,
-        link_type,
-        db_api.sql_dialect.name,
-    )
+    # If it's a link_only or link_and_dedupe and no source_dataset_column_name is
+    # provided, it will have been set to a default by _process_unique_id_columns
     if source_dataset_input_column:
         unique_id_cols = [source_dataset_input_column, unique_id_input_column]
     else:
         unique_id_cols = [unique_id_input_column]
 
     where_condition = _sql_gen_where_condition(link_type, unique_id_cols)
 
-    # If it's a link_only or link_and_dedupe and no source_dataset_column_name is
-    # provided, it will have been set to a default by _process_unique_id_columns
-    if source_dataset_input_column is None:
-        source_dataset_column_name = None
-    else:
-        source_dataset_column_name = source_dataset_input_column.name
-
     sqls = []
 
     if two_dataset_link_only:
         input_tablename_l = input_dataframes[0].physical_name
         input_tablename_r = input_dataframes[1].physical_name
     else:
         sql = vertically_concatenate_sql(
             input_data_dict,
             salting_required=False,
-            source_dataset_column_name=source_dataset_column_name,
+            source_dataset_input_column=source_dataset_input_column,
         )
         sqls.append({"sql": sql, "output_table_name": "__splink__df_concat"})
 
         input_tablename_l = "__splink__df_concat"
         input_tablename_r = "__splink__df_concat"
 
     sql = f"""
@@ -108,15 +99,15 @@
     sqls = []
 
     if two_dataset_link_only:
         input_tablename_l = input_dataframes[0].physical_name
         input_tablename_r = input_dataframes[1].physical_name
     else:
         sql = vertically_concatenate_sql(
-            input_data_dict, salting_required=False, source_dataset_column_name=None
+            input_data_dict, salting_required=False, source_dataset_input_column=None
         )
         sqls.append({"sql": sql, "output_table_name": "__splink__df_concat"})
 
         input_tablename_l = "__splink__df_concat"
         input_tablename_r = "__splink__df_concat"
 
     l_cols_sel = []
@@ -204,37 +195,37 @@
     splink_df_dict: dict[str, "SplinkDataFrame"],
     link_type: backend_link_type_options,
     source_dataset_input_column: Optional[InputColumn],
     db_api: DatabaseAPISubClass,
 ) -> "SplinkDataFrame":
     pipeline = CTEPipeline()
 
-    if source_dataset_input_column:
-        source_dataset_column_name = source_dataset_input_column.name
-    else:
-        source_dataset_column_name = None
-
     sql = vertically_concatenate_sql(
         splink_df_dict,
         salting_required=False,
-        source_dataset_column_name=source_dataset_column_name,
+        source_dataset_input_column=source_dataset_input_column,
     )
     pipeline.enqueue_sql(sql, "__splink__df_concat")
 
     if link_type == "dedupe_only":
         sql = """
         select count(*) as count
         from __splink__df_concat
         """
-    else:
+    elif source_dataset_input_column is not None:
         sql = f"""
         select count(*) as count
         from __splink__df_concat
-        group by {source_dataset_column_name}
+        group by {source_dataset_input_column.name}
         """
+    else:
+        raise ValueError(
+            "If you are using link_only or link_and_dedupe, you must provide a "
+            "source_dataset_column_name"
+        )
     pipeline.enqueue_sql(sql, "__splink__df_count")
     return db_api.sql_pipeline_to_splink_dataframe(pipeline)
 
 
 def _process_unique_id_columns(
     unique_id_column_name: str,
     source_dataset_column_name: Optional[str],
@@ -293,38 +284,30 @@
 def _cumulative_comparisons_to_be_scored_from_blocking_rules(
     *,
     splink_df_dict: dict[str, "SplinkDataFrame"],
     blocking_rules: List[BlockingRule],
     link_type: backend_link_type_options,
     db_api: DatabaseAPISubClass,
     max_rows_limit: int = int(1e9),
-    unique_id_column_name: str,
-    source_dataset_column_name: Optional[str],
+    unique_id_input_column: InputColumn,
+    source_dataset_input_column: Optional[InputColumn],
 ) -> pd.DataFrame:
-    source_dataset_input_column, unique_id_input_column = _process_unique_id_columns(
-        unique_id_column_name,
-        source_dataset_column_name,
-        splink_df_dict,
-        link_type,
-        db_api.sql_dialect.name,
-    )
-
     # Check none of the blocking rules will create a vast/computationally
     # intractable number of comparisons
     for br in blocking_rules:
         # TODO: Deal properly with exlpoding rules
         count = _count_comparisons_generated_from_blocking_rule(
             splink_df_dict=splink_df_dict,
             blocking_rule=br,
             link_type=link_type,
             db_api=db_api,
             max_rows_limit=max_rows_limit,
             compute_post_filter_count=False,
-            unique_id_column_name=unique_id_column_name,
-            source_dataset_column_name=source_dataset_column_name,
+            unique_id_input_column=unique_id_input_column,
+            source_dataset_input_column=source_dataset_input_column,
         )
         count_pre_filter = count[
             "number_of_comparisons_generated_pre_filter_conditions"
         ]
 
         if float(count_pre_filter) > max_rows_limit:
             # TODO: Use a SplinkException?  Want this to give a sensible message
@@ -358,15 +341,15 @@
     )
 
     pipeline = CTEPipeline()
 
     sql = vertically_concatenate_sql(
         splink_df_dict,
         salting_required=False,
-        source_dataset_column_name=source_dataset_column_name,
+        source_dataset_input_column=source_dataset_input_column,
     )
 
     pipeline.enqueue_sql(sql, "__splink__df_concat")
 
     input_columns = [source_dataset_input_column, unique_id_input_column]
     sql_select_expr = ",".join(
         [item for c in input_columns if c is not None for item in c.l_r_names_as_l_r]
@@ -374,14 +357,19 @@
 
     blocking_input_tablename_l = "__splink__df_concat"
 
     blocking_input_tablename_r = "__splink__df_concat"
     if len(splink_df_dict) == 2 and link_type == "link_only":
         link_type = "two_dataset_link_only"
 
+    if source_dataset_input_column:
+        source_dataset_column_name = source_dataset_input_column.name
+    else:
+        source_dataset_column_name = None
+
     if link_type == "two_dataset_link_only" and source_dataset_column_name is not None:
         sqls = split_df_concat_with_tf_into_two_tables_sqls(
             "__splink__df_concat",
             source_dataset_column_name,
         )
         pipeline.enqueue_list_of_sqls(sqls)
 
@@ -457,16 +445,16 @@
     *,
     splink_df_dict: dict[str, "SplinkDataFrame"],
     blocking_rule: BlockingRule,
     link_type: backend_link_type_options,
     db_api: DatabaseAPISubClass,
     compute_post_filter_count: bool,
     max_rows_limit: int = int(1e9),
-    unique_id_column_name: str,
-    source_dataset_column_name: Optional[str],
+    unique_id_input_column: InputColumn,
+    source_dataset_input_column: Optional[InputColumn],
 ) -> dict[str, Union[int, str]]:
     # TODO: if it's an exploding blocking rule, make sure we error out
     pipeline = CTEPipeline()
     sqls = _count_comparisons_from_blocking_rule_pre_filter_conditions_sqls(
         splink_df_dict, blocking_rule, link_type, db_api
     )
     pipeline.enqueue_list_of_sqls(sqls)
@@ -490,47 +478,39 @@
 
     equi_join_conditions_joined = " AND ".join(equi_join_conditions)
 
     filter_conditions = blocking_rule._filter_conditions
     if filter_conditions == "TRUE":
         filter_conditions = ""
 
-    source_dataset_input_column, unique_id_input_column = _process_unique_id_columns(
-        unique_id_column_name,
-        source_dataset_column_name,
-        splink_df_dict,
-        link_type,
-        db_api.sql_dialect.name,
-    )
-
     if source_dataset_input_column:
         uid_for_where = [source_dataset_input_column, unique_id_input_column]
     else:
         uid_for_where = [unique_id_input_column]
 
-    join_condition_sql = _sql_gen_where_condition(link_type, uid_for_where)
+    link_type_join_condition_sql = _sql_gen_where_condition(link_type, uid_for_where)
 
     if not compute_post_filter_count:
         return {
             "number_of_comparisons_generated_pre_filter_conditions": pre_filter_total,
             "number_of_comparisons_to_be_scored_post_filter_conditions": "not computed",
             "filter_conditions_identified": filter_conditions,
             "equi_join_conditions_identified": equi_join_conditions_joined,
-            "inner_join_condition_identified": join_condition_sql,
+            "link_type_join_condition": link_type_join_condition_sql,
         }
 
     if pre_filter_total < max_rows_limit:
         pipeline = CTEPipeline()
         sqls = _number_of_comparisons_generated_by_blocking_rule_post_filters_sqls(
             splink_df_dict,
             blocking_rule,
             link_type,
             db_api,
-            unique_id_column_name,
-            source_dataset_column_name,
+            unique_id_input_column,
+            source_dataset_input_column,
         )
         pipeline.enqueue_list_of_sqls(sqls)
         post_filter_total_df = db_api.sql_pipeline_to_splink_dataframe(pipeline)
         post_filter_total = post_filter_total_df.as_record_dict()[0][
             "count_of_pairwise_comparisons_generated"
         ]
         post_filter_total_df.drop_table_from_database_and_remove_from_cache()
@@ -548,15 +528,15 @@
         )
 
     return {
         "number_of_comparisons_generated_pre_filter_conditions": pre_filter_total,
         "number_of_comparisons_to_be_scored_post_filter_conditions": post_filter_total,
         "filter_conditions_identified": filter_conditions,
         "equi_join_conditions_identified": equi_join_conditions_joined,
-        "inner_join_condition_identified": join_condition_sql,
+        "link_type_join_condition": link_type_join_condition_sql,
     }
 
 
 def count_comparisons_from_blocking_rule(
     *,
     table_or_tables: Sequence[AcceptableInputTableType],
     blocking_rule: Union[BlockingRuleCreator, str, Dict[str, Any]],
@@ -570,23 +550,31 @@
     # Ensure what's been passed in is a BlockingRuleCreator
     blocking_rule_creator = to_blocking_rule_creator(blocking_rule).get_blocking_rule(
         db_api.sql_dialect.name
     )
 
     splink_df_dict = db_api.register_multiple_tables(table_or_tables)
 
+    source_dataset_input_column, unique_id_input_column = _process_unique_id_columns(
+        unique_id_column_name,
+        source_dataset_column_name,
+        splink_df_dict,
+        link_type,
+        db_api.sql_dialect.name,
+    )
+
     return _count_comparisons_generated_from_blocking_rule(
         splink_df_dict=splink_df_dict,
         blocking_rule=blocking_rule_creator,
         link_type=link_type,
         db_api=db_api,
         compute_post_filter_count=compute_post_filter_count,
         max_rows_limit=max_rows_limit,
-        unique_id_column_name=unique_id_column_name,
-        source_dataset_column_name=source_dataset_column_name,
+        unique_id_input_column=unique_id_input_column,
+        source_dataset_input_column=source_dataset_input_column,
     )
 
 
 def cumulative_comparisons_to_be_scored_from_blocking_rules_data(
     *,
     table_or_tables: Sequence[AcceptableInputTableType],
     blocking_rules: Iterable[Union[BlockingRuleCreator, str, Dict[str, Any]]],
@@ -604,22 +592,30 @@
 
     blocking_rules_as_br: List[BlockingRule] = []
     for br in blocking_rules:
         blocking_rules_as_br.append(
             to_blocking_rule_creator(br).get_blocking_rule(db_api.sql_dialect.name)
         )
 
+    source_dataset_input_column, unique_id_input_column = _process_unique_id_columns(
+        unique_id_column_name,
+        source_dataset_column_name,
+        splink_df_dict,
+        link_type,
+        db_api.sql_dialect.name,
+    )
+
     return _cumulative_comparisons_to_be_scored_from_blocking_rules(
         splink_df_dict=splink_df_dict,
         blocking_rules=blocking_rules_as_br,
         link_type=link_type,
         db_api=db_api,
         max_rows_limit=max_rows_limit,
-        unique_id_column_name=unique_id_column_name,
-        source_dataset_column_name=source_dataset_column_name,
+        unique_id_input_column=unique_id_input_column,
+        source_dataset_input_column=source_dataset_input_column,
     )
 
 
 def cumulative_comparisons_to_be_scored_from_blocking_rules_chart(
     *,
     table_or_tables: Sequence[AcceptableInputTableType],
     blocking_rules: Iterable[Union[BlockingRuleCreator, str, Dict[str, Any]]],
@@ -637,20 +633,28 @@
 
     blocking_rules_as_br: List[BlockingRule] = []
     for br in blocking_rules:
         blocking_rules_as_br.append(
             to_blocking_rule_creator(br).get_blocking_rule(db_api.sql_dialect.name)
         )
 
+    source_dataset_input_column, unique_id_input_column = _process_unique_id_columns(
+        unique_id_column_name,
+        source_dataset_column_name,
+        splink_df_dict,
+        link_type,
+        db_api.sql_dialect.name,
+    )
+
     pd_df = _cumulative_comparisons_to_be_scored_from_blocking_rules(
         splink_df_dict=splink_df_dict,
         blocking_rules=blocking_rules_as_br,
         link_type=link_type,
         db_api=db_api,
         max_rows_limit=max_rows_limit,
-        unique_id_column_name=unique_id_column_name,
-        source_dataset_column_name=source_dataset_column_name,
+        unique_id_input_column=unique_id_input_column,
+        source_dataset_input_column=source_dataset_input_column,
     )
 
     return cumulative_blocking_rule_comparisons_generated(
         pd_df.to_dict(orient="records")
     )
```

### Comparing `splink-4.0.0.dev4/splink/internals/completeness.py` & `splink-4.0.0.dev5/splink/internals/completeness.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 from __future__ import annotations
 
 from typing import Any, List, Sequence
 
-from ..charts import (
+from splink.internals.charts import (
     ChartReturnType,
 )
-from ..charts import (
+from splink.internals.charts import (
     completeness_chart as records_to_completeness_chart,
 )
-from ..database_api import AcceptableInputTableType, DatabaseAPISubClass
-from ..input_column import InputColumn
-from ..pipeline import CTEPipeline
-from ..splink_dataframe import SplinkDataFrame
-from ..vertically_concatenate import vertically_concatenate_sql
+from splink.internals.database_api import AcceptableInputTableType, DatabaseAPISubClass
+from splink.internals.input_column import InputColumn
+from splink.internals.pipeline import CTEPipeline
+from splink.internals.splink_dataframe import SplinkDataFrame
+from splink.internals.vertically_concatenate import vertically_concatenate_sql
 
 
 def completeness_data(
     splink_df_dict: dict[str, SplinkDataFrame],
     db_api: DatabaseAPISubClass,
     cols: List[str] = None,
     table_names_for_chart: List[str] = None,
 ) -> list[dict[str, Any]]:
     pipeline = CTEPipeline()
 
     sql = vertically_concatenate_sql(
-        splink_df_dict, salting_required=False, source_dataset_column_name=None
+        splink_df_dict, salting_required=False, source_dataset_input_column=None
     )
 
     pipeline.enqueue_sql(sql, "__splink__df_concat")
 
     # In the case of a single input dataframe, a source_dataset column
     # will not have been created, create one
     first_df = next(iter(splink_df_dict.values()))
```

### Comparing `splink-4.0.0.dev4/splink/internals/profile_data.py` & `splink-4.0.0.dev5/splink/internals/profile_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 import logging
 import re
 from copy import deepcopy
 from typing import List, Optional, Sequence, Union
 
-from ..charts import ChartReturnType, altair_or_json, load_chart_definition
-from ..column_expression import ColumnExpression
-from ..database_api import AcceptableInputTableType, DatabaseAPISubClass
-from ..misc import ensure_is_list
-from ..pipeline import CTEPipeline
-from ..vertically_concatenate import vertically_concatenate_sql
+from splink.internals.charts import (
+    ChartReturnType,
+    altair_or_json,
+    load_chart_definition,
+)
+from splink.internals.column_expression import ColumnExpression
+from splink.internals.database_api import AcceptableInputTableType, DatabaseAPISubClass
+from splink.internals.misc import ensure_is_list
+from splink.internals.pipeline import CTEPipeline
+from splink.internals.vertically_concatenate import vertically_concatenate_sql
 
 logger = logging.getLogger(__name__)
 
 
 def _group_name(cols_or_expr):
     cols_or_expr = re.sub(r"[^0-9a-zA-Z_]", " ", cols_or_expr)
     cols_or_expr = re.sub(r"\s+", "_", cols_or_expr)
@@ -242,15 +246,15 @@
             values to display in the respective charts.
     """
 
     splink_df_dict = db_api.register_multiple_tables(table_or_tables)
 
     pipeline = CTEPipeline()
     sql = vertically_concatenate_sql(
-        splink_df_dict, salting_required=False, source_dataset_column_name=None
+        splink_df_dict, salting_required=False, source_dataset_input_column=None
     )
     pipeline.enqueue_sql(sql, "__splink__df_concat")
 
     input_dataframes = list(splink_df_dict.values())
 
     input_columns = input_dataframes[0].columns_escaped
```

### Comparing `splink-4.0.0.dev4/splink/labelling_tool.py` & `splink-4.0.0.dev5/splink/internals/labelling_tool.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 import os
 from typing import TYPE_CHECKING, Any
 
 import numpy as np
 import pandas as pd
 from jinja2 import Template
 
-from .misc import EverythingEncoder, read_resource
-from .pipeline import CTEPipeline
-from .splink_dataframe import SplinkDataFrame
-from .vertically_concatenate import compute_df_concat_with_tf
+from splink.internals.misc import EverythingEncoder, read_resource
+from splink.internals.pipeline import CTEPipeline
+from splink.internals.splink_dataframe import SplinkDataFrame
+from splink.internals.vertically_concatenate import compute_df_concat_with_tf
 
 # https://stackoverflow.com/questions/39740632/python-type-hinting-without-cyclic-imports
 if TYPE_CHECKING:
-    from .linker import Linker
+    from splink.internals.linker import Linker
 
 logger = logging.getLogger(__name__)
 
 
 def generate_labelling_tool_comparisons(
     linker: "Linker",
     unique_id: str,
@@ -84,21 +84,21 @@
 
     comparisons_recs = comparisons_recs.fillna(np.nan).replace(
         [np.nan, pd.NA], ["", ""]
     )
 
     comparisons_recs = comparisons_recs.to_dict(orient="records")
     # Render template with cluster, nodes and edges
-    template_path = "files/labelling_tool/template.j2"
+    template_path = "internals/files/labelling_tool/template.j2"
     template = Template(read_resource(template_path))
 
     template_data = {
-        "slt": read_resource("files/labelling_tool/slt.js"),
-        "d3": read_resource("files/external_js/d3@7.8.5"),
-        "stdlib": read_resource("files/external_js/stdlib.js@5.8.3"),
+        "slt": read_resource("internals/files/labelling_tool/slt.js"),
+        "d3": read_resource("internals/files/external_js/d3@7.8.5"),
+        "stdlib": read_resource("internals/files/external_js/stdlib.js@5.8.3"),
         "pairwise_comparison_data": json.dumps(comparisons_recs, cls=EverythingEncoder),
         "splink_settings_data": json.dumps(settings, cls=EverythingEncoder),
         "view_in_jupyter": view_in_jupyter,
         "show_splink_predictions_in_interface": show_splink_predictions_in_interface,
     }
 
     rendered = template.render(**template_data)
```

### Comparing `splink-4.0.0.dev4/splink/linker.py` & `splink-4.0.0.dev5/splink/internals/linker.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,118 +2,125 @@
 
 import json
 import logging
 import os
 from copy import copy, deepcopy
 from pathlib import Path
 from statistics import median
-from typing import Any, Dict, List, Optional, Sequence, Union
+from typing import Any, Dict, List, Literal, Optional, Sequence, Union
 
-from .accuracy import (
+from splink.internals.accuracy import (
     prediction_errors_from_label_column,
     prediction_errors_from_labels_table,
     truth_space_table_from_labels_column,
     truth_space_table_from_labels_table,
 )
-from .blocking import (
+from splink.internals.blocking import (
     BlockingRule,
     SaltedBlockingRule,
     block_using_rules_sqls,
     blocking_rule_to_obj,
     materialise_exploded_id_tables,
 )
-from .blocking_rule_creator import BlockingRuleCreator
-from .blocking_rule_creator_utils import to_blocking_rule_creator
-from .cache_dict_with_logging import CacheDictWithLogging
-from .charts import (
+from splink.internals.blocking_analysis import (
+    _cumulative_comparisons_to_be_scored_from_blocking_rules,
+)
+from splink.internals.blocking_rule_creator import BlockingRuleCreator
+from splink.internals.blocking_rule_creator_utils import to_blocking_rule_creator
+from splink.internals.cache_dict_with_logging import CacheDictWithLogging
+from splink.internals.charts import (
     ChartReturnType,
     accuracy_chart,
     match_weights_histogram,
     parameter_estimate_comparisons,
     precision_recall_chart,
     roc_chart,
     threshold_selection_tool,
     unlinkables_chart,
     waterfall_chart,
 )
-from .cluster_studio import SamplingMethods, render_splink_cluster_studio_html
-from .comparison import Comparison
-from .comparison_level import ComparisonLevel
-from .comparison_vector_distribution import (
+from splink.internals.cluster_studio import (
+    SamplingMethods,
+    render_splink_cluster_studio_html,
+)
+from splink.internals.comparison import Comparison
+from splink.internals.comparison_level import ComparisonLevel
+from splink.internals.comparison_vector_distribution import (
     comparison_vector_distribution_sql,
 )
-from .comparison_vector_values import compute_comparison_vector_values_sql
-from .connected_components import (
+from splink.internals.comparison_vector_values import (
+    compute_comparison_vector_values_sql,
+)
+from splink.internals.connected_components import (
     _cc_create_unique_id_cols,
     solve_connected_components,
 )
-from .database_api import AcceptableInputTableType, DatabaseAPISubClass
-from .dialects import SplinkDialect
-from .edge_metrics import compute_edge_metrics
-from .em_training_session import EMTrainingSession
-from .estimate_u import estimate_u_values
-from .exceptions import SplinkException
-from .find_brs_with_comparison_counts_below_threshold import (
+from splink.internals.database_api import AcceptableInputTableType, DatabaseAPISubClass
+from splink.internals.dialects import SplinkDialect
+from splink.internals.edge_metrics import compute_edge_metrics
+from splink.internals.em_training_session import EMTrainingSession
+from splink.internals.estimate_u import estimate_u_values
+from splink.internals.exceptions import SplinkException
+from splink.internals.find_brs_with_comparison_counts_below_threshold import (
     find_blocking_rules_below_threshold_comparison_count,
 )
-from .find_matches_to_new_records import add_unique_id_and_source_dataset_cols_if_needed
-from .graph_metrics import (
+from splink.internals.find_matches_to_new_records import (
+    add_unique_id_and_source_dataset_cols_if_needed,
+)
+from splink.internals.graph_metrics import (
     GraphMetricsResults,
     _node_degree_sql,
     _size_density_centralisation_sql,
 )
-from .input_column import InputColumn
-from .internals.blocking_analysis import (
-    _cumulative_comparisons_to_be_scored_from_blocking_rules,
-)
-from .labelling_tool import (
+from splink.internals.input_column import InputColumn
+from splink.internals.labelling_tool import (
     generate_labelling_tool_comparisons,
     render_labelling_tool_html,
 )
-from .m_from_labels import estimate_m_from_pairwise_labels
-from .m_training import estimate_m_values_from_label_column
-from .match_weights_histogram import histogram_data
-from .misc import (
+from splink.internals.m_from_labels import estimate_m_from_pairwise_labels
+from splink.internals.m_training import estimate_m_values_from_label_column
+from splink.internals.match_weights_histogram import histogram_data
+from splink.internals.misc import (
     ascii_uid,
     bayes_factor_to_prob,
     ensure_is_iterable,
     ensure_is_list,
     prob_to_bayes_factor,
 )
-from .optimise_cost_of_brs import suggest_blocking_rules
-from .pipeline import CTEPipeline
-from .predict import (
+from splink.internals.optimise_cost_of_brs import suggest_blocking_rules
+from splink.internals.pipeline import CTEPipeline
+from splink.internals.predict import (
     predict_from_comparison_vectors_sqls,
     predict_from_comparison_vectors_sqls_using_settings,
 )
-from .settings_creator import SettingsCreator
-from .settings_validation.log_invalid_columns import (
+from splink.internals.settings_creator import SettingsCreator
+from splink.internals.settings_validation.log_invalid_columns import (
     InvalidColumnsLogger,
     SettingsColumnCleaner,
 )
-from .settings_validation.valid_types import (
+from splink.internals.settings_validation.valid_types import (
     _validate_dialect,
 )
-from .splink_comparison_viewer import (
+from splink.internals.splink_comparison_viewer import (
     comparison_viewer_table_sqls,
     render_splink_comparison_viewer_html,
 )
-from .splink_dataframe import SplinkDataFrame
-from .term_frequencies import (
+from splink.internals.splink_dataframe import SplinkDataFrame
+from splink.internals.term_frequencies import (
     _join_new_table_to_df_concat_with_tf_sql,
     colname_to_tf_tablename,
     term_frequencies_for_single_column_sql,
     tf_adjustment_chart,
 )
-from .unique_id_concat import (
+from splink.internals.unique_id_concat import (
     _composite_unique_id_from_edges_sql,
     _composite_unique_id_from_nodes_sql,
 )
-from .unlinkables import unlinkables_data
-from .vertically_concatenate import (
+from splink.internals.unlinkables import unlinkables_data
+from splink.internals.vertically_concatenate import (
     compute_df_concat_with_tf,
     enqueue_df_concat,
     enqueue_df_concat_with_tf,
     split_df_concat_with_tf_into_two_tables_sqls,
 )
 
 logger = logging.getLogger(__name__)
@@ -1762,356 +1769,14 @@
             ```
         """
         labels_tablename = self._get_labels_tablename_from_input(
             labels_splinkdataframe_or_table_name
         )
         estimate_m_from_pairwise_labels(self, labels_tablename)
 
-    def truth_space_table_from_labels_table(
-        self,
-        labels_splinkdataframe_or_table_name: SplinkDataFrame | str,
-        threshold_actual: float = 0.5,
-        match_weight_round_to_nearest: float = None,
-    ) -> SplinkDataFrame:
-        """Generate truth statistics (false positive etc.) for each threshold value of
-        match_probability, suitable for plotting a ROC chart.
-
-        The table of labels should be in the following format, and should be registered
-        with your database:
-
-        |source_dataset_l|unique_id_l|source_dataset_r|unique_id_r|clerical_match_score|
-        |----------------|-----------|----------------|-----------|--------------------|
-        |df_1            |1          |df_2            |2          |0.99                |
-        |df_1            |1          |df_2            |3          |0.2                 |
-
-        Note that `source_dataset` and `unique_id` should correspond to the values
-        specified in the settings dict, and the `input_table_aliases` passed to the
-        `linker` object.
-
-        For `dedupe_only` links, the `source_dataset` columns can be ommitted.
-
-        Args:
-            labels_splinkdataframe_or_table_name (str | SplinkDataFrame): Name of table
-                containing labels in the database
-            threshold_actual (float, optional): Where the `clerical_match_score`
-                provided by the user is a probability rather than binary, this value
-                is used as the threshold to classify `clerical_match_score`s as binary
-                matches or non matches. Defaults to 0.5.
-            match_weight_round_to_nearest (float, optional): When provided, thresholds
-                are rounded.  When large numbers of labels are provided, this is
-                sometimes necessary to reduce the size of the ROC table, and therefore
-                the number of points plotted on the ROC chart. Defaults to None.
-
-        Examples:
-            ```py
-            labels = pd.read_csv("my_labels.csv")
-            linker.register_table(labels, "labels")
-            linker.truth_space_table_from_labels_table("labels")
-            ```
-
-        Returns:
-            SplinkDataFrame:  Table of truth statistics
-        """
-        labels_tablename = self._get_labels_tablename_from_input(
-            labels_splinkdataframe_or_table_name
-        )
-
-        self._raise_error_if_necessary_accuracy_columns_not_computed()
-        return truth_space_table_from_labels_table(
-            self,
-            labels_tablename,
-            threshold_actual=threshold_actual,
-            match_weight_round_to_nearest=match_weight_round_to_nearest,
-        )
-
-    def roc_chart_from_labels_table(
-        self,
-        labels_splinkdataframe_or_table_name: str | SplinkDataFrame,
-        threshold_actual: float = 0.5,
-        match_weight_round_to_nearest: float = None,
-    ) -> ChartReturnType:
-        """Generate a ROC chart from labelled (ground truth) data.
-
-        The table of labels should be in the following format, and should be registered
-        with your database:
-
-        |source_dataset_l|unique_id_l|source_dataset_r|unique_id_r|clerical_match_score|
-        |----------------|-----------|----------------|-----------|--------------------|
-        |df_1            |1          |df_2            |2          |0.99                |
-        |df_1            |1          |df_2            |3          |0.2                 |
-
-        Note that `source_dataset` and `unique_id` should correspond to the values
-        specified in the settings dict, and the `input_table_aliases` passed to the
-        `linker` object.
-
-        For `dedupe_only` links, the `source_dataset` columns can be ommitted.
-
-        Args:
-            labels_splinkdataframe_or_table_name (str | SplinkDataFrame): Name of table
-                containing labels in the database
-            threshold_actual (float, optional): Where the `clerical_match_score`
-                provided by the user is a probability rather than binary, this value
-                is used as the threshold to classify `clerical_match_score`s as binary
-                matches or non matches. Defaults to 0.5.
-            match_weight_round_to_nearest (float, optional): When provided, thresholds
-                are rounded.  When large numbers of labels are provided, this is
-                sometimes necessary to reduce the size of the ROC table, and therefore
-                the number of points plotted on the ROC chart. Defaults to None.
-
-        Examples:
-            === ":simple-duckdb: DuckDB"
-                ```py
-                labels = pd.read_csv("my_labels.csv")
-                linker.register_table(labels, "labels")
-                linker.roc_chart_from_labels_table("labels")
-                ```
-            === ":simple-apachespark: Spark"
-                ```py
-                labels = spark.read.csv("my_labels.csv", header=True)
-                labels.createDataFrame("labels")
-                linker.roc_chart_from_labels_table("labels")
-                ```
-
-        Returns:
-            altair.Chart: An altair chart
-        """
-        labels_tablename = self._get_labels_tablename_from_input(
-            labels_splinkdataframe_or_table_name
-        )
-
-        self._raise_error_if_necessary_accuracy_columns_not_computed()
-        df_truth_space = truth_space_table_from_labels_table(
-            self,
-            labels_tablename,
-            threshold_actual=threshold_actual,
-            match_weight_round_to_nearest=match_weight_round_to_nearest,
-        )
-        recs = df_truth_space.as_record_dict()
-        return roc_chart(recs)
-
-    def precision_recall_chart_from_labels_table(
-        self,
-        labels_splinkdataframe_or_table_name: SplinkDataFrame | str,
-        threshold_actual: float = 0.5,
-        match_weight_round_to_nearest: float = None,
-    ) -> ChartReturnType:
-        """Generate a precision-recall chart from labelled (ground truth) data.
-
-        The table of labels should be in the following format, and should be registered
-        as a table with your database:
-
-        |source_dataset_l|unique_id_l|source_dataset_r|unique_id_r|clerical_match_score|
-        |----------------|-----------|----------------|-----------|--------------------|
-        |df_1            |1          |df_2            |2          |0.99                |
-        |df_1            |1          |df_2            |3          |0.2                 |
-
-        Note that `source_dataset` and `unique_id` should correspond to the values
-        specified in the settings dict, and the `input_table_aliases` passed to the
-        `linker` object.
-
-        For `dedupe_only` links, the `source_dataset` columns can be ommitted.
-
-        Args:
-            labels_splinkdataframe_or_table_name (str | SplinkDataFrame): Name of table
-                containing labels in the database
-            threshold_actual (float, optional): Where the `clerical_match_score`
-                provided by the user is a probability rather than binary, this value
-                is used as the threshold to classify `clerical_match_score`s as binary
-                matches or non matches. Defaults to 0.5.
-            match_weight_round_to_nearest (float, optional): When provided, thresholds
-                are rounded.  When large numbers of labels are provided, this is
-                sometimes necessary to reduce the size of the ROC table, and therefore
-                the number of points plotted on the ROC chart. Defaults to None.
-        Examples:
-            ```py
-            labels = pd.read_csv("my_labels.csv")
-            linker.register_table(labels, "labels")
-            linker.precision_recall_chart_from_labels_table("labels")
-            ```
-
-        Returns:
-            altair.Chart: An altair chart
-        """
-        labels_tablename = self._get_labels_tablename_from_input(
-            labels_splinkdataframe_or_table_name
-        )
-        self._raise_error_if_necessary_accuracy_columns_not_computed()
-        df_truth_space = truth_space_table_from_labels_table(
-            self,
-            labels_tablename,
-            threshold_actual=threshold_actual,
-            match_weight_round_to_nearest=match_weight_round_to_nearest,
-        )
-        recs = df_truth_space.as_record_dict()
-        return precision_recall_chart(recs)
-
-    def accuracy_chart_from_labels_table(
-        self,
-        labels_splinkdataframe_or_table_name: SplinkDataFrame | str,
-        threshold_actual: float = 0.5,
-        match_weight_round_to_nearest: float = None,
-        add_metrics: list[str] = [],
-    ) -> ChartReturnType:
-        """Generate an accuracy measure chart from labelled (ground truth) data.
-
-        The table of labels should be in the following format, and should be registered
-        as a table with your database:
-
-        |source_dataset_l|unique_id_l|source_dataset_r|unique_id_r|clerical_match_score|
-        |----------------|-----------|----------------|-----------|--------------------|
-        |df_1            |1          |df_2            |2          |0.99                |
-        |df_1            |1          |df_2            |3          |0.2                 |
-
-        Note that `source_dataset` and `unique_id` should correspond to the values
-        specified in the settings dict, and the `input_table_aliases` passed to the
-        `linker` object.
-
-        For `dedupe_only` links, the `source_dataset` columns can be ommitted.
-
-        Args:
-            labels_splinkdataframe_or_table_name (str | SplinkDataFrame): Name of table
-                containing labels in the database
-            threshold_actual (float, optional): Where the `clerical_match_score`
-                provided by the user is a probability rather than binary, this value
-                is used as the threshold to classify `clerical_match_score`s as binary
-                matches or non matches. Defaults to 0.5.
-            match_weight_round_to_nearest (float, optional): When provided, thresholds
-                are rounded.  When large numbers of labels are provided, this is
-                sometimes necessary to reduce the size of the ROC table, and therefore
-                the number of points plotted on the chart. Defaults to None.
-            add_metrics (list(str), optional): Precision and recall metrics are always
-                included. Where provided, `add_metrics` specifies additional metrics
-                to show, with the following options:
-
-                - `"specificity"`: specificity, selectivity, true negative rate (TNR)
-                - `"npv"`: negative predictive value (NPV)
-                - `"accuracy"`: overall accuracy (TP+TN)/(P+N)
-                - `"f1"`/`"f2"`/`"f0_5"`: F-scores for \u03b2=1 (balanced), \u03b2=2
-                (emphasis on recall) and \u03b2=0.5 (emphasis on precision)
-                - `"p4"` -  an extended F1 score with specificity and NPV included
-                - `"phi"` - \u03c6 coefficient or Matthews correlation coefficient (MCC)
-        Examples:
-            === ":simple-duckdb: DuckDB"
-                ```py
-                labels = pd.read_csv("my_labels.csv")
-                linker.register_table(labels, "labels")
-                linker.accuracy_chart_from_labels_table("labels", add_metrics=["f1"])
-                ```
-            === ":simple-apachespark: Spark"
-                ```py
-                labels = spark.read.csv("my_labels.csv", header=True)
-                labels.createDataFrame("labels")
-                linker.accuracy_chart_from_labels_table("labels", add_metrics=['f1'])
-                ```
-
-        Returns:
-            altair.Chart: An altair chart
-        """
-        allowed = ["specificity", "npv", "accuracy", "f1", "f2", "f0_5", "p4", "phi"]
-
-        if not isinstance(add_metrics, list):
-            raise Exception(
-                "add_metrics must be a list containing one or more of the following:",
-                allowed,
-            )
-
-        # Silently filter out invalid entries (except case errors - e.g. ["NPV", "F1"])
-        add_metrics = list(set(map(str.lower, add_metrics)).intersection(allowed))
-
-        labels_tablename = self._get_labels_tablename_from_input(
-            labels_splinkdataframe_or_table_name
-        )
-        self._raise_error_if_necessary_accuracy_columns_not_computed()
-        df_truth_space = truth_space_table_from_labels_table(
-            self,
-            labels_tablename,
-            threshold_actual=threshold_actual,
-            match_weight_round_to_nearest=match_weight_round_to_nearest,
-        )
-        recs = df_truth_space.as_record_dict()
-        return accuracy_chart(recs, add_metrics=add_metrics)
-
-    def threshold_selection_tool_from_labels_table(
-        self,
-        labels_splinkdataframe_or_table_name: str | SplinkDataFrame,
-        threshold_actual: float = 0.5,
-        match_weight_round_to_nearest: float = None,
-        add_metrics: list[str] = [],
-    ) -> ChartReturnType:
-        """Generate an accuracy chart from labelled (ground truth) data.
-
-        The table of labels should be in the following format, and should be registered
-        as a table with your database:
-
-        |source_dataset_l|unique_id_l|source_dataset_r|unique_id_r|clerical_match_score|
-        |----------------|-----------|----------------|-----------|--------------------|
-        |df_1            |1          |df_2            |2          |0.99                |
-        |df_1            |1          |df_2            |3          |0.2                 |
-
-        Note that `source_dataset` and `unique_id` should correspond to the values
-        specified in the settings dict, and the `input_table_aliases` passed to the
-        `linker` object.
-
-        For `dedupe_only` links, the `source_dataset` columns can be ommitted.
-
-        Args:
-            labels_splinkdataframe_or_table_name (str | SplinkDataFrame): Name of table
-                containing labels in the database
-            threshold_actual (float, optional): Where the `clerical_match_score`
-                provided by the user is a probability rather than binary, this value
-                is used as the threshold to classify `clerical_match_score`s as binary
-                matches or non matches. Defaults to 0.5.
-            match_weight_round_to_nearest (float, optional): When provided, thresholds
-                are rounded.  When large numbers of labels are provided, this is
-                sometimes necessary to reduce the size of the ROC table, and therefore
-                the number of points plotted on the chart. Defaults to None.
-            add_metrics (list(str), optional): Precision and recall metrics are always
-                included. Where provided, `add_metrics` specifies additional metrics
-                to show, with the following options:
-
-                - `"specificity"`: specificity, selectivity, true negative rate (TNR)
-                - `"npv"`: negative predictive value (NPV)
-                - `"accuracy"`: overall accuracy (TP+TN)/(P+N)
-                - `"f1"`/`"f2"`/`"f0_5"`: F-scores for \u03b2=1 (balanced), \u03b2=2
-                (emphasis on recall) and \u03b2=0.5 (emphasis on precision)
-                - `"p4"` -  an extended F1 score with specificity and NPV included
-                - `"phi"` - \u03c6 coefficient or Matthews correlation coefficient (MCC)
-        Examples:
-            ```py
-            linker.accuracy_chart_from_labels_column("ground_truth", add_metrics=["f1"])
-            ```
-
-        Returns:
-            altair.Chart: An altair chart
-        """
-
-        allowed = ["specificity", "npv", "accuracy", "f1", "f2", "f0_5", "p4", "phi"]
-
-        if not isinstance(add_metrics, list):
-            raise Exception(
-                "add_metrics must be a list containing one or more of the following:",
-                allowed,
-            )
-
-        # Silently filter out invalid entries (except case errors - e.g. ["NPV", "F1"])
-        add_metrics = list(set(map(str.lower, add_metrics)).intersection(allowed))
-
-        labels_tablename = self._get_labels_tablename_from_input(
-            labels_splinkdataframe_or_table_name
-        )
-        self._raise_error_if_necessary_accuracy_columns_not_computed()
-        df_truth_space = truth_space_table_from_labels_table(
-            self,
-            labels_tablename,
-            threshold_actual=threshold_actual,
-            match_weight_round_to_nearest=match_weight_round_to_nearest,
-        )
-        recs = df_truth_space.as_record_dict()
-        return threshold_selection_tool(recs, add_metrics=add_metrics)
-
     def prediction_errors_from_labels_table(
         self,
         labels_splinkdataframe_or_table_name,
         include_false_positives=True,
         include_false_negatives=True,
         threshold=0.5,
     ):
@@ -2137,138 +1802,38 @@
             self,
             labels_tablename,
             include_false_positives,
             include_false_negatives,
             threshold,
         )
 
-    def truth_space_table_from_labels_column(
+    def accuracy_analysis_from_labels_column(
         self,
         labels_column_name: str,
+        *,
         threshold_actual: float = 0.5,
-        match_weight_round_to_nearest: float = None,
+        match_weight_round_to_nearest: float = 0.1,
+        output_type: Literal[
+            "threshold_selection", "roc", "precision_recall", "table", "accuracy"
+        ] = "threshold_selection",
+        add_metrics: List[
+            Literal[
+                "specificity",
+                "npv",
+                "accuracy",
+                "f1",
+                "f2",
+                "f0_5",
+                "p4",
+                "phi",
+            ]
+        ] = [],
         positives_not_captured_by_blocking_rules_scored_as_zero: bool = True,
-    ) -> SplinkDataFrame:
-        """Generate truth statistics (false positive etc.) for each threshold value of
-        match_probability, suitable for plotting a ROC chart.
-
-        Your labels_column_name should include the ground truth cluster (unique
-        identifier) that groups entities which are the same
-
-        Args:
-            labels_tablename (str): Name of table containing labels in the database
-            threshold_actual (float, optional): Where the `clerical_match_score`
-                provided by the user is a probability rather than binary, this value
-                is used as the threshold to classify `clerical_match_score`s as binary
-                matches or non matches. Defaults to 0.5.
-            match_weight_round_to_nearest (float, optional): When provided, thresholds
-                are rounded.  When large numbers of labels are provided, this is
-                sometimes necessary to reduce the size of the ROC table, and therefore
-                the number of points plotted on the ROC chart. Defaults to None.
-
-        Examples:
-            ```py
-            linker.truth_space_table_from_labels_column("cluster")
-            ```
-
-        Returns:
-            SplinkDataFrame:  Table of truth statistics
-        """
-
-        return truth_space_table_from_labels_column(
-            self,
-            labels_column_name,
-            threshold_actual,
-            match_weight_round_to_nearest,
-            positives_not_captured_by_blocking_rules_scored_as_zero,
-        )
-
-    def roc_chart_from_labels_column(
-        self,
-        labels_column_name: str,
-        threshold_actual: float = 0.5,
-        match_weight_round_to_nearest: float = None,
-    ) -> ChartReturnType:
-        """Generate a ROC chart from ground truth data, whereby the ground truth
-        is in a column in the input dataset called `labels_column_name`
-
-        Args:
-            labels_column_name (str): Column name containing labels in the input table
-            threshold_actual (float, optional): Where the `clerical_match_score`
-                provided by the user is a probability rather than binary, this value
-                is used as the threshold to classify `clerical_match_score`s as binary
-                matches or non matches. Defaults to 0.5.
-            match_weight_round_to_nearest (float, optional): When provided, thresholds
-                are rounded.  When large numbers of labels are provided, this is
-                sometimes necessary to reduce the size of the ROC table, and therefore
-                the number of points plotted on the ROC chart. Defaults to None.
-
-        Examples:
-            ```py
-            linker.roc_chart_from_labels_column("labels")
-            ```
-
-        Returns:
-            altair.Chart: An altair chart
-        """
-
-        df_truth_space = truth_space_table_from_labels_column(
-            self,
-            labels_column_name,
-            threshold_actual=threshold_actual,
-            match_weight_round_to_nearest=match_weight_round_to_nearest,
-        )
-        recs = df_truth_space.as_record_dict()
-        return roc_chart(recs)
-
-    def precision_recall_chart_from_labels_column(
-        self,
-        labels_column_name: str,
-        threshold_actual: float = 0.5,
-        match_weight_round_to_nearest: float = None,
-    ) -> ChartReturnType:
-        """Generate a precision-recall chart from ground truth data, whereby the ground
-        truth is in a column in the input dataset called `labels_column_name`
-
-        Args:
-            labels_column_name (str): Column name containing labels in the input table
-            threshold_actual (float, optional): Where the `clerical_match_score`
-                provided by the user is a probability rather than binary, this value
-                is used as the threshold to classify `clerical_match_score`s as binary
-                matches or non matches. Defaults to 0.5.
-            match_weight_round_to_nearest (float, optional): When provided, thresholds
-                are rounded.  When large numbers of labels are provided, this is
-                sometimes necessary to reduce the size of the ROC table, and therefore
-                the number of points plotted on the ROC chart. Defaults to None.
-        Examples:
-            ```py
-            linker.precision_recall_chart_from_labels_column("ground_truth")
-            ```
-
-        Returns:
-            altair.Chart: An altair chart
-        """
-
-        df_truth_space = truth_space_table_from_labels_column(
-            self,
-            labels_column_name,
-            threshold_actual=threshold_actual,
-            match_weight_round_to_nearest=match_weight_round_to_nearest,
-        )
-        recs = df_truth_space.as_record_dict()
-        return precision_recall_chart(recs)
-
-    def accuracy_chart_from_labels_column(
-        self,
-        labels_column_name: str,
-        threshold_actual: float = 0.5,
-        match_weight_round_to_nearest: float = None,
-        add_metrics: list[str] = [],
-    ) -> ChartReturnType:
-        """Generate an accuracy chart from ground truth data, whereby the ground
+    ) -> Union[ChartReturnType, SplinkDataFrame]:
+        """Generate an accuracy chart or table from ground truth data, where the ground
         truth is in a column in the input dataset called `labels_column_name`
 
         Args:
             labels_column_name (str): Column name containing labels in the input table
             threshold_actual (float, optional): Where the `clerical_match_score`
                 provided by the user is a probability rather than binary, this value
                 is used as the threshold to classify `clerical_match_score`s as binary
@@ -2286,53 +1851,101 @@
                 - `"accuracy"`: overall accuracy (TP+TN)/(P+N)
                 - `"f1"`/`"f2"`/`"f0_5"`: F-scores for \u03b2=1 (balanced), \u03b2=2
                 (emphasis on recall) and \u03b2=0.5 (emphasis on precision)
                 - `"p4"` -  an extended F1 score with specificity and NPV included
                 - `"phi"` - \u03c6 coefficient or Matthews correlation coefficient (MCC)
         Examples:
             ```py
-            linker.accuracy_chart_from_labels_column("ground_truth", add_metrics=["f1"])
+            linker.accuracy_analysis_from_labels_column("ground_truth", add_metrics=["f1"])
             ```
 
         Returns:
             altair.Chart: An altair chart
-        """
+        """  # noqa: E501
 
         allowed = ["specificity", "npv", "accuracy", "f1", "f2", "f0_5", "p4", "phi"]
 
         if not isinstance(add_metrics, list):
             raise Exception(
                 "add_metrics must be a list containing one or more of the following:",
                 allowed,
             )
 
-        # Silently filter out invalid entries (except case errors - e.g. ["NPV", "F1"])
-        add_metrics = list(set(map(str.lower, add_metrics)).intersection(allowed))
+        if not all(metric in allowed for metric in add_metrics):
+            raise ValueError(
+                "Invalid metric. " f"Allowed metrics are: {', '.join(allowed)}."
+            )
 
         df_truth_space = truth_space_table_from_labels_column(
             self,
             labels_column_name,
             threshold_actual=threshold_actual,
             match_weight_round_to_nearest=match_weight_round_to_nearest,
+            positives_not_captured_by_blocking_rules_scored_as_zero=positives_not_captured_by_blocking_rules_scored_as_zero,
         )
         recs = df_truth_space.as_record_dict()
-        return accuracy_chart(recs, add_metrics=add_metrics)
 
-    def threshold_selection_tool_from_labels_column(
+        if output_type == "threshold_selection":
+            return threshold_selection_tool(recs, add_metrics=add_metrics)
+        elif output_type == "accuracy":
+            return accuracy_chart(recs, add_metrics=add_metrics)
+        elif output_type == "roc":
+            return roc_chart(recs)
+        elif output_type == "precision_recall":
+            return precision_recall_chart(recs)
+        elif output_type == "table":
+            return df_truth_space
+        else:
+            raise ValueError(
+                "Invalid chart_type. Allowed chart types are: "
+                "'threshold_selection', 'roc', 'precision_recall', 'accuracy."
+            )
+
+    def accuracy_analysis_from_labels_table(
         self,
-        labels_column_name: str,
+        labels_splinkdataframe_or_table_name: str | SplinkDataFrame,
+        *,
         threshold_actual: float = 0.5,
-        match_weight_round_to_nearest: float = None,
-        add_metrics: list[str] = [],
-    ) -> ChartReturnType:
-        """Generate an accuracy chart from ground truth data, whereby the ground
-        truth is in a column in the input dataset called `labels_column_name`
+        match_weight_round_to_nearest: float = 0.1,
+        output_type: Literal[
+            "threshold_selection", "roc", "precision_recall", "table", "accuracy"
+        ] = "threshold_selection",
+        add_metrics: List[
+            Literal[
+                "specificity",
+                "npv",
+                "accuracy",
+                "f1",
+                "f2",
+                "f0_5",
+                "p4",
+                "phi",
+            ]
+        ] = [],
+    ) -> Union[ChartReturnType, SplinkDataFrame]:
+        """Generate an accuracy chart or table from labelled (ground truth) data.
+
+        The table of labels should be in the following format, and should be registered
+        as a table with your database using
+        `labels_table = linker.register_labels_table(my_df)`
+
+        |source_dataset_l|unique_id_l|source_dataset_r|unique_id_r|clerical_match_score|
+        |----------------|-----------|----------------|-----------|--------------------|
+        |df_1            |1          |df_2            |2          |0.99                |
+        |df_1            |1          |df_2            |3          |0.2                 |
+
+        Note that `source_dataset` and `unique_id` should correspond to the values
+        specified in the settings dict, and the `input_table_aliases` passed to the
+        `linker` object.
+
+        For `dedupe_only` links, the `source_dataset` columns can be ommitted.
 
         Args:
-            labels_column_name (str): Column name containing labels in the input table
+            labels_splinkdataframe_or_table_name (str | SplinkDataFrame): Name of table
+                containing labels in the database
             threshold_actual (float, optional): Where the `clerical_match_score`
                 provided by the user is a probability rather than binary, this value
                 is used as the threshold to classify `clerical_match_score`s as binary
                 matches or non matches. Defaults to 0.5.
             match_weight_round_to_nearest (float, optional): When provided, thresholds
                 are rounded.  When large numbers of labels are provided, this is
                 sometimes necessary to reduce the size of the ROC table, and therefore
@@ -2346,40 +1959,61 @@
                 - `"accuracy"`: overall accuracy (TP+TN)/(P+N)
                 - `"f1"`/`"f2"`/`"f0_5"`: F-scores for \u03b2=1 (balanced), \u03b2=2
                 (emphasis on recall) and \u03b2=0.5 (emphasis on precision)
                 - `"p4"` -  an extended F1 score with specificity and NPV included
                 - `"phi"` - \u03c6 coefficient or Matthews correlation coefficient (MCC)
         Examples:
             ```py
-            linker.accuracy_chart_from_labels_column("ground_truth", add_metrics=["f1"])
+            linker.accuracy_analysis_from_labels_table("ground_truth", add_metrics=["f1"])
             ```
 
         Returns:
             altair.Chart: An altair chart
-        """
+        """  # noqa: E501
 
         allowed = ["specificity", "npv", "accuracy", "f1", "f2", "f0_5", "p4", "phi"]
 
         if not isinstance(add_metrics, list):
             raise Exception(
                 "add_metrics must be a list containing one or more of the following:",
                 allowed,
             )
 
-        # Silently filter out invalid entries (except case errors - e.g. ["NPV", "F1"])
-        add_metrics = list(set(map(str.lower, add_metrics)).intersection(allowed))
+        if not all(metric in allowed for metric in add_metrics):
+            raise ValueError(
+                f"Invalid metric. Allowed metrics are: {', '.join(allowed)}."
+            )
 
-        df_truth_space = truth_space_table_from_labels_column(
+        labels_tablename = self._get_labels_tablename_from_input(
+            labels_splinkdataframe_or_table_name
+        )
+        self._raise_error_if_necessary_accuracy_columns_not_computed()
+        df_truth_space = truth_space_table_from_labels_table(
             self,
-            labels_column_name,
+            labels_tablename,
             threshold_actual=threshold_actual,
             match_weight_round_to_nearest=match_weight_round_to_nearest,
         )
         recs = df_truth_space.as_record_dict()
-        return threshold_selection_tool(recs, add_metrics=add_metrics)
+
+        if output_type == "threshold_selection":
+            return threshold_selection_tool(recs, add_metrics=add_metrics)
+        elif output_type == "accuracy":
+            return accuracy_chart(recs, add_metrics=add_metrics)
+        elif output_type == "roc":
+            return roc_chart(recs)
+        elif output_type == "precision_recall":
+            return precision_recall_chart(recs)
+        elif output_type == "table":
+            return df_truth_space
+        else:
+            raise ValueError(
+                "Invalid chart_type. Allowed chart types are: "
+                "'threshold_selection', 'roc', 'precision_recall', 'accuracy."
+            )
 
     def prediction_errors_from_labels_column(
         self,
         label_colname,
         include_false_positives=True,
         include_false_negatives=True,
         threshold=0.5,
@@ -2840,16 +2474,16 @@
 
         pd_df = _cumulative_comparisons_to_be_scored_from_blocking_rules(
             splink_df_dict=self._input_tables_dict,
             blocking_rules=blocking_rules,
             link_type=self._settings_obj._link_type,
             db_api=self.db_api,
             max_rows_limit=max_rows_limit,
-            unique_id_column_name=self._settings_obj.column_info_settings.unique_id_column_name,
-            source_dataset_column_name=self._settings_obj.column_info_settings.source_dataset_column_name,
+            unique_id_input_column=self._settings_obj.column_info_settings.unique_id_input_column,
+            source_dataset_input_column=self._settings_obj.column_info_settings.source_dataset_input_column,
         )
 
         records = pd_df.to_dict(orient="records")
 
         summary_record = records[-1]
         num_observed_matches = summary_record["cumulative_rows"]
         num_total_comparisons = summary_record["cartesian"]
```

### Comparing `splink-4.0.0.dev4/splink/lower_id_on_lhs.py` & `splink-4.0.0.dev5/splink/internals/lower_id_on_lhs.py`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev4/splink/m_from_labels.py` & `splink-4.0.0.dev5/splink/internals/m_from_labels.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 import logging
 
-from .block_from_labels import block_from_labels
-from .comparison_vector_values import compute_comparison_vector_values_sql
-from .expectation_maximisation import (
+from splink.internals.block_from_labels import block_from_labels
+from splink.internals.comparison_vector_values import (
+    compute_comparison_vector_values_sql,
+)
+from splink.internals.expectation_maximisation import (
     compute_new_parameters_sql,
     compute_proportions_for_new_parameters,
 )
+from splink.internals.pipeline import CTEPipeline
+from splink.internals.vertically_concatenate import compute_df_concat_with_tf
+
 from .m_u_records_to_parameters import (
     append_m_probability_to_comparison_level_trained_probabilities,
     m_u_records_to_lookup_dict,
 )
-from .pipeline import CTEPipeline
-from .vertically_concatenate import compute_df_concat_with_tf
 
 logger = logging.getLogger(__name__)
 
 
 def estimate_m_from_pairwise_labels(linker, table_name):
     pipeline = CTEPipeline()
     nodes_with_tf = compute_df_concat_with_tf(linker, pipeline)
```

### Comparing `splink-4.0.0.dev4/splink/m_training.py` & `splink-4.0.0.dev5/splink/internals/m_training.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 import logging
 from copy import deepcopy
 
-from .blocking import BlockingRule, block_using_rules_sqls
-from .comparison_vector_values import compute_comparison_vector_values_sql
-from .expectation_maximisation import (
+from splink.internals.blocking import BlockingRule, block_using_rules_sqls
+from splink.internals.comparison_vector_values import (
+    compute_comparison_vector_values_sql,
+)
+from splink.internals.expectation_maximisation import (
     compute_new_parameters_sql,
     compute_proportions_for_new_parameters,
 )
+from splink.internals.pipeline import CTEPipeline
+from splink.internals.vertically_concatenate import compute_df_concat_with_tf
+
 from .m_u_records_to_parameters import (
     append_m_probability_to_comparison_level_trained_probabilities,
     m_u_records_to_lookup_dict,
 )
-from .pipeline import CTEPipeline
-from .vertically_concatenate import compute_df_concat_with_tf
 
 logger = logging.getLogger(__name__)
 
 
 def estimate_m_values_from_label_column(linker, df_dict, label_colname):
     msg = f" Estimating m probabilities using from column {label_colname} "
     logger.info(f"{msg:-^70}")
```

### Comparing `splink-4.0.0.dev4/splink/m_u_records_to_parameters.py` & `splink-4.0.0.dev5/splink/internals/m_u_records_to_parameters.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import logging
 from typing import Any, Dict, List
 
-from .comparison_level import ComparisonLevel
-from .constants import LEVEL_NOT_OBSERVED_TEXT
+from splink.internals.comparison_level import ComparisonLevel
+from splink.internals.constants import LEVEL_NOT_OBSERVED_TEXT
 
 logger = logging.getLogger(__name__)
 
 
 def m_u_records_to_lookup_dict(
     m_u_records: List[Dict[str, Any]],
 ) -> Dict[str, Dict[int, Any]]:
```

### Comparing `splink-4.0.0.dev4/splink/match_key_analysis.py` & `splink-4.0.0.dev5/splink/internals/match_key_analysis.py`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev4/splink/match_weights_histogram.py` & `splink-4.0.0.dev5/splink/internals/match_weights_histogram.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from math import floor
 
-from .pipeline import CTEPipeline
+from splink.internals.pipeline import CTEPipeline
 
 
 def _bins(min, max, num_bins):
     bin_widths = [0.01, 0.1, 0.2, 0.25, 0.5, 1, 2, 5]
 
     rough_binwidth = (max - min) / num_bins
```

### Comparing `splink-4.0.0.dev4/splink/misc.py` & `splink-4.0.0.dev5/splink/internals/misc.py`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev4/splink/optimise_cost_of_brs.py` & `splink-4.0.0.dev5/splink/internals/optimise_cost_of_brs.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import logging
 from random import randint
 from typing import TypeVar
 
 import pandas as pd
 
-from .cost_of_blocking_rules import calculate_cost_of_combination_of_brs
+from splink.internals.cost_of_blocking_rules import calculate_cost_of_combination_of_brs
 
 logger = logging.getLogger(__name__)
 
 T = TypeVar("T")
 
 
 def localised_shuffle(lst: list[T], window_percent: float) -> list[T]:
```

### Comparing `splink-4.0.0.dev4/splink/parse_sql.py` & `splink-4.0.0.dev5/splink/internals/parse_sql.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from collections.abc import Sequence
 
 import sqlglot
 import sqlglot.expressions as exp
 from sqlglot.expressions import Bracket, Column, Lambda
 
-from .sql_transform import remove_quotes_from_identifiers
+from splink.internals.sql_transform import remove_quotes_from_identifiers
 
 
 def get_columns_used_from_sql(sql, dialect=None, retain_table_prefix=False):
     column_names = set()
     syntax_tree = sqlglot.parse_one(sql, read=dialect)
 
     for subtree in syntax_tree.find_all(exp.Column):
```

### Comparing `splink-4.0.0.dev4/splink/pipeline.py` & `splink-4.0.0.dev5/splink/internals/pipeline.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,21 +3,22 @@
 import logging
 from typing import TYPE_CHECKING, List, Optional
 
 import sqlglot
 from sqlglot.errors import ParseError
 from sqlglot.expressions import Table
 
-from .misc import ensure_is_list
+from splink.internals.misc import ensure_is_list
+
 from .splink_dataframe import SplinkDataFrame
 
 logger = logging.getLogger(__name__)
 
 if TYPE_CHECKING:
-    from .database_api import DatabaseAPISubClass
+    from splink.internals.database_api import DatabaseAPISubClass
 
 
 class CTE:
     def __init__(self, sql, output_table_name):
         self.sql = sql
         self.output_table_name = output_table_name
```

### Comparing `splink-4.0.0.dev4/splink/postgres/database_api.py` & `splink-4.0.0.dev5/splink/internals/postgres/database_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,21 +2,22 @@
 from typing import Any, List, Union
 
 import duckdb
 import pandas as pd
 from sqlalchemy import CursorResult, text
 from sqlalchemy.engine import Engine
 
-from ..database_api import DatabaseAPI
-from ..dialects import (
+from splink.internals.database_api import DatabaseAPI
+from splink.internals.dialects import (
     PostgresDialect,
 )
-from ..misc import (
+from splink.internals.misc import (
     ensure_is_list,
 )
+
 from .dataframe import PostgresDataFrame
 
 logger = logging.getLogger(__name__)
 
 
 class PostgresAPI(DatabaseAPI[CursorResult[Any]]):
     sql_dialect = PostgresDialect()
```

### Comparing `splink-4.0.0.dev4/splink/postgres/dataframe.py` & `splink-4.0.0.dev5/splink/internals/postgres/dataframe.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import logging
 from typing import TYPE_CHECKING
 
-from ..input_column import InputColumn
-from ..splink_dataframe import SplinkDataFrame
+from splink.internals.input_column import InputColumn
+from splink.internals.splink_dataframe import SplinkDataFrame
 
 logger = logging.getLogger(__name__)
 if TYPE_CHECKING:
     from .database_api import PostgresAPI
 
 
 class PostgresDataFrame(SplinkDataFrame):
```

### Comparing `splink-4.0.0.dev4/splink/predict.py` & `splink-4.0.0.dev5/splink/internals/predict.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from __future__ import annotations
 
 # This is otherwise known as the expectation step of the EM algorithm.
 import logging
 from typing import List
 
-from .comparison import Comparison
-from .input_column import InputColumn
-from .misc import prob_to_bayes_factor, prob_to_match_weight
+from splink.internals.comparison import Comparison
+from splink.internals.input_column import InputColumn
+from splink.internals.misc import prob_to_bayes_factor, prob_to_match_weight
+
 from .settings import CoreModelSettings, Settings
 
 logger = logging.getLogger(__name__)
 
 
 def predict_from_comparison_vectors_sqls_using_settings(
     settings_obj: Settings,
```

### Comparing `splink-4.0.0.dev4/splink/settings.py` & `splink-4.0.0.dev5/splink/internals/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,29 @@
 from __future__ import annotations
 
 import logging
 from copy import deepcopy
 from dataclasses import asdict, dataclass
 from typing import Any, List, Literal, Sequence, TypedDict
 
-from .blocking import BlockingRule, SaltedBlockingRule, blocking_rule_to_obj
-from .charts import m_u_parameters_chart, match_weights_chart
-from .comparison import Comparison
-from .comparison_level import ComparisonLevel
-from .input_column import InputColumn
-from .misc import dedupe_preserving_order, prob_to_bayes_factor, prob_to_match_weight
-from .parse_sql import get_columns_used_from_sql
+from splink.internals.blocking import (
+    BlockingRule,
+    SaltedBlockingRule,
+    blocking_rule_to_obj,
+)
+from splink.internals.charts import m_u_parameters_chart, match_weights_chart
+from splink.internals.comparison import Comparison
+from splink.internals.comparison_level import ComparisonLevel
+from splink.internals.input_column import InputColumn
+from splink.internals.misc import (
+    dedupe_preserving_order,
+    prob_to_bayes_factor,
+    prob_to_match_weight,
+)
+from splink.internals.parse_sql import get_columns_used_from_sql
 
 logger = logging.getLogger(__name__)
 
 
 # custom type for hinting:
 class ComparisonAndLevelDict(TypedDict):
     level: ComparisonLevel
```

### Comparing `splink-4.0.0.dev4/splink/settings_creator.py` & `splink-4.0.0.dev5/splink/internals/settings_creator.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,25 +2,20 @@
 
 import json
 from copy import deepcopy
 from dataclasses import asdict, dataclass, field
 from pathlib import Path
 from typing import Any, List, Literal, Union
 
-from .blocking_rule_creator import BlockingRuleCreator
-from .blocking_rule_creator_utils import to_blocking_rule_creator
-from .comparison_creator import ComparisonCreator
-from .comparison_library import CustomComparison
-from .settings import Settings
-
+from splink.internals.blocking_rule_creator import BlockingRuleCreator
+from splink.internals.blocking_rule_creator_utils import to_blocking_rule_creator
+from splink.internals.comparison_creator import ComparisonCreator
+from splink.internals.comparison_library import CustomComparison
 
-def to_comparison_creator(comparison_creator):
-    if isinstance(comparison_creator, dict):
-        return CustomComparison(**comparison_creator)
-    return comparison_creator
+from .settings import Settings
 
 
 @dataclass
 class SettingsCreator:
     """
     Non-dialected version of Settings.
     Responsible for authoring Settings, but not implementing anything
@@ -64,15 +59,15 @@
         Returns class as a dict where we have converted any sub-dicts into
         'creator' types
         """
         creator_dict = self._as_naive_dict()
         # we adjust dict to ensure that comparisons + blocking rules are
         # consistently of creatore types
         creator_dict["comparisons"] = [
-            to_comparison_creator(comparison_creator)
+            CustomComparison._convert_to_creator(comparison_creator)
             for comparison_creator in creator_dict["comparisons"]
         ]
         creator_dict["blocking_rules_to_generate_predictions"] = [
             to_blocking_rule_creator(blocking_rule_creator)
             for blocking_rule_creator in creator_dict[
                 "blocking_rules_to_generate_predictions"
             ]
```

### Comparing `splink-4.0.0.dev4/splink/settings_validation/log_invalid_columns.py` & `splink-4.0.0.dev5/splink/internals/settings_validation/log_invalid_columns.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 import logging
 from collections.abc import Sequence
 from typing import TYPE_CHECKING, Iterable, Protocol
 
 import sqlglot
 import sqlglot.expressions
 
-from ..comparison import Comparison
-from ..parse_sql import parse_columns_in_sql
+from splink.internals.comparison import Comparison
+from splink.internals.parse_sql import parse_columns_in_sql
+
 from .settings_column_cleaner import (
     SettingsColumnCleaner,
     clean_and_find_columns_not_in_input_dfs,
     find_columns_not_in_input_dfs,
 )
 from .settings_validation_log_strings import (
     InvalidColumnSuffixesLogGenerator,
```

### Comparing `splink-4.0.0.dev4/splink/settings_validation/settings_column_cleaner.py` & `splink-4.0.0.dev5/splink/internals/settings_validation/settings_column_cleaner.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 from copy import deepcopy
 from functools import reduce
 from operator import and_
 from typing import TYPE_CHECKING, Iterable, List, Literal, overload
 
 import sqlglot
 
-from ..input_column import InputColumn
-from ..splink_dataframe import SplinkDataFrame
+from splink.internals.input_column import InputColumn
+from splink.internals.splink_dataframe import SplinkDataFrame
 
 logger = logging.getLogger(__name__)
 
 if TYPE_CHECKING:
-    from ..settings import Settings
+    from splink.internals.settings import Settings
 
 
 def remove_suffix(c: str) -> str:
     return re.sub("_[l|r]{1}$", "", c)
 
 
 def find_columns_not_in_input_dfs(
```

### Comparing `splink-4.0.0.dev4/splink/settings_validation/settings_validation_log_strings.py` & `splink-4.0.0.dev5/splink/internals/settings_validation/settings_validation_log_strings.py`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev4/splink/settings_validation/valid_types.py` & `splink-4.0.0.dev5/splink/internals/settings_validation/valid_types.py`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev4/splink/spark/database_api.py` & `splink-4.0.0.dev5/splink/internals/spark/database_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,22 +5,23 @@
 
 import pandas as pd
 import sqlglot
 from numpy import nan
 from pyspark.sql.dataframe import DataFrame as spark_df
 from pyspark.sql.utils import AnalysisException
 
-from ..database_api import AcceptableInputTableType, DatabaseAPI
-from ..databricks.enable_splink import enable_splink
-from ..dialects import (
+from splink.internals.database_api import AcceptableInputTableType, DatabaseAPI
+from splink.internals.databricks.enable_splink import enable_splink
+from splink.internals.dialects import (
     SparkDialect,
 )
-from ..misc import (
+from splink.internals.misc import (
     major_minor_version_greater_equal_than,
 )
+
 from .dataframe import SparkDataFrame
 from .jar_location import get_scala_udfs
 
 logger = logging.getLogger(__name__)
 
 
 class SparkAPI(DatabaseAPI[spark_df]):
```

### Comparing `splink-4.0.0.dev4/splink/spark/dataframe.py` & `splink-4.0.0.dev5/splink/internals/spark/dataframe.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from __future__ import annotations
 
 import logging
 from typing import TYPE_CHECKING
 
 from pandas import DataFrame as PandasDataFrame
 
-from ..input_column import InputColumn
-from ..splink_dataframe import SplinkDataFrame
+from splink.internals.input_column import InputColumn
+from splink.internals.splink_dataframe import SplinkDataFrame
+
 from .spark_helpers.custom_spark_dialect import Dialect
 
 logger = logging.getLogger(__name__)
 
 Dialect["customspark"]
 if TYPE_CHECKING:
     from .database_api import SparkAPI
```

### Comparing `splink-4.0.0.dev4/splink/spark/jar_location.py` & `splink-4.0.0.dev5/splink/internals/spark/jar_location.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,20 +15,20 @@
 
 def similarity_jar_location():
     import splink
 
     if _spark_v_3_check():
         path = (
             splink.__file__[0:-11]
-            + "files/spark_jars/scala-udf-similarity-0.1.1_spark3.x.jar"
+            + "internals/files/spark_jars/scala-udf-similarity-0.1.1_spark3.x.jar"
         )
     else:
         path = (
             splink.__file__[0:-11]
-            + "files/spark_jars/scala-udf-similarity-0.1.0_classic.jar"
+            + "internals/files/spark_jars/scala-udf-similarity-0.1.0_classic.jar"
         )
 
     return path
 
 
 def get_scala_udfs():
     # This functions expects that either:
```

### Comparing `splink-4.0.0.dev4/splink/spark/spark_helpers/custom_spark_dialect.py` & `splink-4.0.0.dev5/splink/internals/spark/spark_helpers/custom_spark_dialect.py`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev4/splink/splink_comparison_viewer.py` & `splink-4.0.0.dev5/splink/internals/splink_comparison_viewer.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,20 +2,21 @@
 
 import json
 import os
 from typing import TYPE_CHECKING, Any
 
 from jinja2 import Template
 
-from .misc import EverythingEncoder, read_resource
+from splink.internals.misc import EverythingEncoder, read_resource
+
 from .predict import _combine_prior_and_bfs
 
 # https://stackoverflow.com/questions/39740632/python-type-hinting-without-cyclic-imports
 if TYPE_CHECKING:
-    from .linker import Linker
+    from splink.internals.linker import Linker
 
 
 def row_examples(
     linker: Linker, example_rows_per_category: int = 2
 ) -> list[dict[str, str]]:
     sqls = []
 
@@ -116,31 +117,31 @@
     overwrite: bool = False,
 ) -> str:
     # When developing the package, it can be easier to point
     # ar the script live on observable using <script src=>
     # rather than bundling the whole thing into the html
     bundle_observable_notebook = True
 
-    template_path = "files/splink_comparison_viewer/template.j2"
+    template_path = "internals/files/splink_comparison_viewer/template.j2"
     template = Template(read_resource(template_path))
 
     template_data: dict[str, Any] = {
         "comparison_vector_data": json.dumps(
             comparison_vector_data, cls=EverythingEncoder
         ),
         "splink_settings": json.dumps(splink_settings),
     }
 
     files = {
-        "embed": "files/external_js/vega-embed@6.20.2",
-        "vega": "files/external_js/vega@5.21.0",
-        "vegalite": "files/external_js/vega-lite@5.2.0",
-        "stdlib": "files/external_js/stdlib.js@5.8.3",
-        "svu_text": "files/splink_vis_utils/splink_vis_utils.js",
-        "custom_css": "files/splink_comparison_viewer/custom.css",
+        "embed": "internals/files/external_js/vega-embed@6.20.2",
+        "vega": "internals/files/external_js/vega@5.21.0",
+        "vegalite": "internals/files/external_js/vega-lite@5.2.0",
+        "stdlib": "internals/files/external_js/stdlib.js@5.8.3",
+        "svu_text": "internals/files/splink_vis_utils/splink_vis_utils.js",
+        "custom_css": "internals/files/splink_comparison_viewer/custom.css",
     }
     for k, v in files.items():
         template_data[k] = read_resource(v)
 
     template_data["bundle_observable_notebook"] = bundle_observable_notebook
 
     rendered = template.render(**template_data)
```

### Comparing `splink-4.0.0.dev4/splink/splink_dataframe.py` & `splink-4.0.0.dev5/splink/internals/splink_dataframe.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from __future__ import annotations
 
 import logging
 from abc import ABC, abstractmethod, abstractproperty
 from pathlib import Path
 from typing import TYPE_CHECKING, Any
 
-from .input_column import InputColumn
+from splink.internals.input_column import InputColumn
 
 logger = logging.getLogger(__name__)
 
 # https://stackoverflow.com/questions/39740632/python-type-hinting-without-cyclic-imports
 if TYPE_CHECKING:
-    from .database_api import DatabaseAPI
+    from splink.internals.database_api import DatabaseAPI
 
 
 class SplinkDataFrame(ABC):
     """Abstraction over dataframe to handle basic operations like retrieving data and
     retrieving column names, which need different implementations depending on whether
     it's a spark dataframe, sqlite table etc.
     Uses methods like `as_pandas_dataframe()` and `as_record_dict()` to retrieve data
```

### Comparing `splink-4.0.0.dev4/splink/sql_transform.py` & `splink-4.0.0.dev5/splink/internals/sql_transform.py`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev4/splink/sqlite/database_api.py` & `splink-4.0.0.dev5/splink/internals/sqlite/database_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import math
 import sqlite3
 from typing import Union
 
 import pandas as pd
 
-from ..database_api import DatabaseAPI
-from ..dialects import (
+from splink.internals.database_api import DatabaseAPI
+from splink.internals.dialects import (
     SQLiteDialect,
 )
-from ..exceptions import SplinkException
+from splink.internals.exceptions import SplinkException
+
 from .dataframe import SQLiteDataFrame
 
 sql_con = sqlite3.Connection
 
 
 class SQLiteAPI(DatabaseAPI[sqlite3.Cursor]):
     sql_dialect = SQLiteDialect()
```

### Comparing `splink-4.0.0.dev4/splink/sqlite/dataframe.py` & `splink-4.0.0.dev5/splink/internals/sqlite/dataframe.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import logging
 from typing import TYPE_CHECKING
 
-from ..input_column import InputColumn
-from ..splink_dataframe import SplinkDataFrame
+from splink.internals.input_column import InputColumn
+from splink.internals.splink_dataframe import SplinkDataFrame
 
 logger = logging.getLogger(__name__)
 if TYPE_CHECKING:
     from .database_api import SQLiteAPI
 
 
 def dict_factory(cursor, row):
```

### Comparing `splink-4.0.0.dev4/splink/term_frequencies.py` & `splink-4.0.0.dev5/splink/internals/term_frequencies.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,21 +5,25 @@
 import logging
 import warnings
 from typing import TYPE_CHECKING, Any
 
 from numpy import arange, ceil, floor, log2
 from pandas import concat, cut
 
-from .charts import ChartReturnType, altair_or_json, load_chart_definition
-from .input_column import InputColumn
-from .pipeline import CTEPipeline
+from splink.internals.charts import (
+    ChartReturnType,
+    altair_or_json,
+    load_chart_definition,
+)
+from splink.internals.input_column import InputColumn
+from splink.internals.pipeline import CTEPipeline
 
 # https://stackoverflow.com/questions/39740632/python-type-hinting-without-cyclic-imports
 if TYPE_CHECKING:
-    from .linker import Linker
+    from splink.internals.linker import Linker
 
 logger = logging.getLogger(__name__)
 
 
 def colname_to_tf_tablename(input_column: InputColumn) -> str:
     column_name_str = input_column.unquote().name.replace(" ", "_")
     return f"__splink__df_tf_{column_name_str}"
```

### Comparing `splink-4.0.0.dev4/splink/unique_id_concat.py` & `splink-4.0.0.dev5/splink/internals/unique_id_concat.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from .input_column import InputColumn
+from splink.internals.input_column import InputColumn
 
 CONCAT_SEPARATOR = "-__-"
 
 
 def _composite_unique_id_from_nodes_sql(
     unique_id_cols: list[InputColumn], table_prefix: str | None = None
 ) -> str:
```

### Comparing `splink-4.0.0.dev4/splink/unlinkables.py` & `splink-4.0.0.dev5/splink/internals/unlinkables.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any
 
-from .pipeline import CTEPipeline
+from splink.internals.pipeline import CTEPipeline
 
 # https://stackoverflow.com/questions/39740632/python-type-hinting-without-cyclic-imports
 if TYPE_CHECKING:
-    from .linker import Linker
+    from splink.internals.linker import Linker
 
 
 def unlinkables_data(linker: Linker) -> dict[str, Any]:
     """Generate data displaying the proportion of records that are "unlinkable"
     for a given splink score threshold and model parameters. These are records that,
     even when compared with themselves, do not contain enough information to confirm
     a match.
```

### Comparing `splink-4.0.0.dev4/splink/validate_jsonschema.py` & `splink-4.0.0.dev5/splink/internals/validate_jsonschema.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import json
 import operator
 from functools import lru_cache, reduce
 from typing import Any
 
 from jsonschema import Draft7Validator
 
-from .misc import read_resource
+from splink.internals.misc import read_resource
 
 
 @lru_cache()
 def get_schema():
     path = "files/settings_jsonschema.json"
     return json.loads(read_resource(path))
```

### Comparing `splink-4.0.0.dev4/splink/vertically_concatenate.py` & `splink-4.0.0.dev5/splink/internals/vertically_concatenate.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 from __future__ import annotations
 
 import logging
 from typing import TYPE_CHECKING, Dict
 
-from .pipeline import CTEPipeline
-from .splink_dataframe import SplinkDataFrame
+from splink.internals.input_column import InputColumn
+from splink.internals.pipeline import CTEPipeline
+from splink.internals.splink_dataframe import SplinkDataFrame
+
 from .term_frequencies import compute_all_term_frequencies_sqls
 
 logger = logging.getLogger(__name__)
 
 # https://stackoverflow.com/questions/39740632/python-type-hinting-without-cyclic-imports
 if TYPE_CHECKING:
-    from .linker import Linker
+    from splink.internals.linker import Linker
 
 
 def vertically_concatenate_sql(
     input_tables: Dict[str, SplinkDataFrame],
     salting_required: bool,
-    source_dataset_column_name: str = None,
+    source_dataset_input_column: InputColumn = None,
 ) -> str:
     """
     Using `input_tables`, create a single table with the columns and
     rows required for linking.
 
     This table will later be the basis for the generation of pairwise record comparises,
     and will also be used to generate the term frequency adjustment tables.
@@ -41,18 +43,19 @@
 
     if salting_required:
         salt_sql = ", random() as __splink_salt"
     else:
         salt_sql = ""
 
     source_dataset_column_already_exists = False
-    if source_dataset_column_name:
-        source_dataset_column_already_exists = source_dataset_column_name in [
-            c.unquote().name for c in df_obj.columns
-        ]
+    if source_dataset_input_column:
+        source_dataset_column_already_exists = (
+            source_dataset_input_column.unquote().name
+            in [c.unquote().name for c in df_obj.columns]
+        )
 
     select_columns_sql = ", ".join(columns)
     if len(input_tables) > 1:
         sqls_to_union = []
 
         for df_obj in input_tables.values():
             if source_dataset_column_already_exists:
@@ -82,20 +85,20 @@
 def enqueue_df_concat_with_tf(linker: Linker, pipeline: CTEPipeline) -> CTEPipeline:
     cache = linker._intermediate_table_cache
     if "__splink__df_concat_with_tf" in cache:
         nodes_with_tf = cache.get_with_logging("__splink__df_concat_with_tf")
         pipeline.append_input_dataframe(nodes_with_tf)
         return pipeline
 
-    sds_name = linker._settings_obj.column_info_settings.source_dataset_column_name
+    sds_ic = linker._settings_obj.column_info_settings.source_dataset_input_column
 
     sql = vertically_concatenate_sql(
         input_tables=linker._input_tables_dict,
         salting_required=linker._settings_obj.salting_required,
-        source_dataset_column_name=sds_name,
+        source_dataset_input_column=sds_ic,
     )
     pipeline.enqueue_sql(sql, "__splink__df_concat")
 
     sqls = compute_all_term_frequencies_sqls(linker, pipeline)
     pipeline.enqueue_list_of_sqls(sqls)
 
     return pipeline
@@ -104,20 +107,20 @@
 def compute_df_concat_with_tf(linker: Linker, pipeline: CTEPipeline) -> SplinkDataFrame:
     cache = linker._intermediate_table_cache
     db_api = linker.db_api
 
     if "__splink__df_concat_with_tf" in cache:
         return cache.get_with_logging("__splink__df_concat_with_tf")
 
-    sds_name = linker._settings_obj.column_info_settings.source_dataset_column_name
+    sds_ic = linker._settings_obj.column_info_settings.source_dataset_input_column
 
     sql = vertically_concatenate_sql(
         input_tables=linker._input_tables_dict,
         salting_required=linker._settings_obj.salting_required,
-        source_dataset_column_name=sds_name,
+        source_dataset_input_column=sds_ic,
     )
     pipeline.enqueue_sql(sql, "__splink__df_concat")
 
     sqls = compute_all_term_frequencies_sqls(linker, pipeline)
     pipeline.enqueue_list_of_sqls(sqls)
 
     nodes_with_tf = db_api.sql_pipeline_to_splink_dataframe(pipeline)
@@ -137,20 +140,20 @@
     # so if it exists, use it instead
     elif "__splink__df_concat_with_tf" in cache:
         nodes_with_tf = cache.get_with_logging("__splink__df_concat_with_tf")
         nodes_with_tf.templated_name = "__splink__df_concat"
         pipeline.append_input_dataframe(nodes_with_tf)
         return pipeline
 
-    sds_name = linker._settings_obj.column_info_settings.source_dataset_column_name
+    sds_ic = linker._settings_obj.column_info_settings.source_dataset_input_column
 
     sql = vertically_concatenate_sql(
         input_tables=linker._input_tables_dict,
         salting_required=linker._settings_obj.salting_required,
-        source_dataset_column_name=sds_name,
+        source_dataset_input_column=sds_ic,
     )
     pipeline.enqueue_sql(sql, "__splink__df_concat")
 
     return pipeline
 
 
 def compute_df_concat(linker: Linker, pipeline: CTEPipeline) -> SplinkDataFrame:
@@ -160,20 +163,20 @@
     if "__splink__df_concat" in cache:
         return cache.get_with_logging("__splink__df_concat")
     if "__splink__df_concat_with_tf" in cache:
         df = cache.get_with_logging("__splink__df_concat_with_tf")
         df.templated_name = "__splink__df_concat"
         return df
 
-    sds_name = linker._settings_obj.column_info_settings.source_dataset_column_name
+    sds_ic = linker._settings_obj.column_info_settings.source_dataset_input_column
 
     sql = vertically_concatenate_sql(
         input_tables=linker._input_tables_dict,
         salting_required=linker._settings_obj.salting_required,
-        source_dataset_column_name=sds_name,
+        source_dataset_input_column=sds_ic,
     )
     pipeline.enqueue_sql(sql, "__splink__df_concat")
 
     nodes_with_tf = db_api.sql_pipeline_to_splink_dataframe(pipeline)
     cache["__splink__df_concat"] = nodes_with_tf
     return nodes_with_tf
```

### Comparing `splink-4.0.0.dev4/splink/waterfall_chart.py` & `splink-4.0.0.dev5/splink/internals/waterfall_chart.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import math
 from copy import deepcopy
 from typing import Any, Dict
 
-from .comparison import Comparison
-from .misc import prob_to_bayes_factor
+from splink.internals.comparison import Comparison
+from splink.internals.misc import prob_to_bayes_factor
 
 
 def _prior_record(settings_obj):
     rec: Dict[str, Any] = {}
     rec["column_name"] = "Prior"
     rec["label_for_charts"] = "Starting match weight (prior)"
     rec["sql_condition"] = None
```

### Comparing `splink-4.0.0.dev4/PKG-INFO` & `splink-4.0.0.dev5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splink
-Version: 4.0.0.dev4
+Version: 4.0.0.dev5
 Summary: Fast probabilistic data linkage at scale
 Home-page: https://github.com/moj-analytical-services/splink
 License: MIT
 Author: Robin Linacre
 Author-email: robinlinacre@hotmail.com
 Requires-Python: >=3.8.0,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

