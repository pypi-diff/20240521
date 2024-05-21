# Comparing `tmp/mozilla-metric-config-parser-2024.4.1.tar.gz` & `tmp/mozilla_metric_config_parser-2024.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mozilla-metric-config-parser-2024.4.1.tar", last modified: Wed Apr 10 13:23:58 2024, max compression
+gzip compressed data, was "mozilla_metric_config_parser-2024.5.1.tar", last modified: Tue May 21 16:54:18 2024, max compression
```

## Comparing `mozilla-metric-config-parser-2024.4.1.tar` & `mozilla_metric_config_parser-2024.5.1.tar`

### file list

```diff
@@ -1,60 +1,61 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 13:23:58.658162 mozilla-metric-config-parser-2024.4.1/
--rw-r--r--   0 root         (0) root         (0)    16725 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       18 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1590 2024-04-10 13:23:58.658162 mozilla-metric-config-parser-2024.4.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      279 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 13:23:58.654162 mozilla-metric-config-parser-2024.4.1/metric_config_parser/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/metric_config_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7062 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/metric_config_parser/alert.py
--rw-r--r--   0 root         (0) root         (0)     7137 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/metric_config_parser/analysis.py
--rw-r--r--   0 root         (0) root         (0)     2774 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/metric_config_parser/cli.py
--rw-r--r--   0 root         (0) root         (0)    27979 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/metric_config_parser/config.py
--rw-r--r--   0 root         (0) root         (0)     8172 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/metric_config_parser/data_source.py
--rw-r--r--   0 root         (0) root         (0)     1602 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/metric_config_parser/definition.py
--rw-r--r--   0 root         (0) root         (0)     3493 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/metric_config_parser/dimension.py
--rw-r--r--   0 root         (0) root         (0)      804 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/metric_config_parser/errors.py
--rw-r--r--   0 root         (0) root         (0)     9825 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/metric_config_parser/experiment.py
--rw-r--r--   0 root         (0) root         (0)     2619 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/metric_config_parser/exposure_signal.py
--rw-r--r--   0 root         (0) root         (0)     1143 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/metric_config_parser/function.py
--rw-r--r--   0 root         (0) root         (0)    15859 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/metric_config_parser/metric.py
--rw-r--r--   0 root         (0) root         (0)     3130 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/metric_config_parser/metric_group.py
--rw-r--r--   0 root         (0) root         (0)     6640 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/metric_config_parser/monitoring.py
--rw-r--r--   0 root         (0) root         (0)     1718 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/metric_config_parser/outcome.py
--rw-r--r--   0 root         (0) root         (0)     3386 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/metric_config_parser/parameter.py
--rw-r--r--   0 root         (0) root         (0)     3278 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/metric_config_parser/population.py
--rw-r--r--   0 root         (0) root         (0)      317 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/metric_config_parser/pre_treatment.py
--rw-r--r--   0 root         (0) root         (0)     5138 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/metric_config_parser/project.py
--rw-r--r--   0 root         (0) root         (0)     8103 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/metric_config_parser/segment.py
--rw-r--r--   0 root         (0) root         (0)     4207 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/metric_config_parser/sql.py
--rw-r--r--   0 root         (0) root         (0)      129 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/metric_config_parser/statistic.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 13:23:58.654162 mozilla-metric-config-parser-2024.4.1/metric_config_parser/templates/
--rw-r--r--   0 root         (0) root         (0)      143 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/metric_config_parser/templates/data_source_query.sql
--rw-r--r--   0 root         (0) root         (0)     2691 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/metric_config_parser/templates/metrics_query.sql
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 13:23:58.658162 mozilla-metric-config-parser-2024.4.1/metric_config_parser/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/metric_config_parser/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5118 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/metric_config_parser/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 13:23:58.658162 mozilla-metric-config-parser-2024.4.1/metric_config_parser/tests/integration/
--rw-r--r--   0 root         (0) root         (0)     6657 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/metric_config_parser/tests/integration/test_config_integration.py
--rw-r--r--   0 root         (0) root         (0)     2428 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/metric_config_parser/tests/test_alert.py
--rw-r--r--   0 root         (0) root         (0)    26303 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/metric_config_parser/tests/test_analysis.py
--rw-r--r--   0 root         (0) root         (0)    16931 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/metric_config_parser/tests/test_config.py
--rw-r--r--   0 root         (0) root         (0)    11572 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/metric_config_parser/tests/test_experiment.py
--rw-r--r--   0 root         (0) root         (0)     1581 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/metric_config_parser/tests/test_function.py
--rw-r--r--   0 root         (0) root         (0)     2866 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/metric_config_parser/tests/test_metric.py
--rw-r--r--   0 root         (0) root         (0)     8522 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/metric_config_parser/tests/test_monitoring.py
--rw-r--r--   0 root         (0) root         (0)    12162 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/metric_config_parser/tests/test_outcomes.py
--rw-r--r--   0 root         (0) root         (0)      458 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/metric_config_parser/tests/test_parameter.py
--rw-r--r--   0 root         (0) root         (0)     2035 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/metric_config_parser/tests/test_population.py
--rw-r--r--   0 root         (0) root         (0)     2808 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/metric_config_parser/tests/test_project.py
--rw-r--r--   0 root         (0) root         (0)     3322 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/metric_config_parser/tests/test_sql.py
--rw-r--r--   0 root         (0) root         (0)      575 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/metric_config_parser/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 13:23:58.658162 mozilla-metric-config-parser-2024.4.1/mozilla_metric_config_parser.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1590 2024-04-10 13:23:58.000000 mozilla-metric-config-parser-2024.4.1/mozilla_metric_config_parser.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1941 2024-04-10 13:23:58.000000 mozilla-metric-config-parser-2024.4.1/mozilla_metric_config_parser.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 13:23:58.000000 mozilla-metric-config-parser-2024.4.1/mozilla_metric_config_parser.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       70 2024-04-10 13:23:58.000000 mozilla-metric-config-parser-2024.4.1/mozilla_metric_config_parser.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      274 2024-04-10 13:23:58.000000 mozilla-metric-config-parser-2024.4.1/mozilla_metric_config_parser.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2024-04-10 13:23:58.000000 mozilla-metric-config-parser-2024.4.1/mozilla_metric_config_parser.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       85 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       67 2024-04-10 13:23:58.658162 mozilla-metric-config-parser-2024.4.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1574 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 16:54:18.806264 mozilla_metric_config_parser-2024.5.1/
+-rw-r--r--   0 root         (0) root         (0)    16725 2024-05-21 16:54:09.000000 mozilla_metric_config_parser-2024.5.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       18 2024-05-21 16:54:09.000000 mozilla_metric_config_parser-2024.5.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1590 2024-05-21 16:54:18.806264 mozilla_metric_config_parser-2024.5.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      279 2024-05-21 16:54:09.000000 mozilla_metric_config_parser-2024.5.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 16:54:18.802264 mozilla_metric_config_parser-2024.5.1/metric_config_parser/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-21 16:54:09.000000 mozilla_metric_config_parser-2024.5.1/metric_config_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7062 2024-05-21 16:54:09.000000 mozilla_metric_config_parser-2024.5.1/metric_config_parser/alert.py
+-rw-r--r--   0 root         (0) root         (0)     7185 2024-05-21 16:54:09.000000 mozilla_metric_config_parser-2024.5.1/metric_config_parser/analysis.py
+-rw-r--r--   0 root         (0) root         (0)     2774 2024-05-21 16:54:09.000000 mozilla_metric_config_parser-2024.5.1/metric_config_parser/cli.py
+-rw-r--r--   0 root         (0) root         (0)    28118 2024-05-21 16:54:09.000000 mozilla_metric_config_parser-2024.5.1/metric_config_parser/config.py
+-rw-r--r--   0 root         (0) root         (0)    10973 2024-05-21 16:54:09.000000 mozilla_metric_config_parser-2024.5.1/metric_config_parser/data_source.py
+-rw-r--r--   0 root         (0) root         (0)     1602 2024-05-21 16:54:09.000000 mozilla_metric_config_parser-2024.5.1/metric_config_parser/definition.py
+-rw-r--r--   0 root         (0) root         (0)     3493 2024-05-21 16:54:09.000000 mozilla_metric_config_parser-2024.5.1/metric_config_parser/dimension.py
+-rw-r--r--   0 root         (0) root         (0)      804 2024-05-21 16:54:09.000000 mozilla_metric_config_parser-2024.5.1/metric_config_parser/errors.py
+-rw-r--r--   0 root         (0) root         (0)     9825 2024-05-21 16:54:09.000000 mozilla_metric_config_parser-2024.5.1/metric_config_parser/experiment.py
+-rw-r--r--   0 root         (0) root         (0)     2619 2024-05-21 16:54:09.000000 mozilla_metric_config_parser-2024.5.1/metric_config_parser/exposure_signal.py
+-rw-r--r--   0 root         (0) root         (0)     1143 2024-05-21 16:54:09.000000 mozilla_metric_config_parser-2024.5.1/metric_config_parser/function.py
+-rw-r--r--   0 root         (0) root         (0)    16178 2024-05-21 16:54:09.000000 mozilla_metric_config_parser-2024.5.1/metric_config_parser/metric.py
+-rw-r--r--   0 root         (0) root         (0)     3130 2024-05-21 16:54:09.000000 mozilla_metric_config_parser-2024.5.1/metric_config_parser/metric_group.py
+-rw-r--r--   0 root         (0) root         (0)     6640 2024-05-21 16:54:09.000000 mozilla_metric_config_parser-2024.5.1/metric_config_parser/monitoring.py
+-rw-r--r--   0 root         (0) root         (0)     1718 2024-05-21 16:54:09.000000 mozilla_metric_config_parser-2024.5.1/metric_config_parser/outcome.py
+-rw-r--r--   0 root         (0) root         (0)     3386 2024-05-21 16:54:09.000000 mozilla_metric_config_parser-2024.5.1/metric_config_parser/parameter.py
+-rw-r--r--   0 root         (0) root         (0)     3374 2024-05-21 16:54:09.000000 mozilla_metric_config_parser-2024.5.1/metric_config_parser/population.py
+-rw-r--r--   0 root         (0) root         (0)      317 2024-05-21 16:54:09.000000 mozilla_metric_config_parser-2024.5.1/metric_config_parser/pre_treatment.py
+-rw-r--r--   0 root         (0) root         (0)     5138 2024-05-21 16:54:09.000000 mozilla_metric_config_parser-2024.5.1/metric_config_parser/project.py
+-rw-r--r--   0 root         (0) root         (0)     8103 2024-05-21 16:54:09.000000 mozilla_metric_config_parser-2024.5.1/metric_config_parser/segment.py
+-rw-r--r--   0 root         (0) root         (0)     5529 2024-05-21 16:54:09.000000 mozilla_metric_config_parser-2024.5.1/metric_config_parser/sql.py
+-rw-r--r--   0 root         (0) root         (0)      129 2024-05-21 16:54:09.000000 mozilla_metric_config_parser-2024.5.1/metric_config_parser/statistic.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 16:54:18.802264 mozilla_metric_config_parser-2024.5.1/metric_config_parser/templates/
+-rw-r--r--   0 root         (0) root         (0)     1727 2024-05-21 16:54:09.000000 mozilla_metric_config_parser-2024.5.1/metric_config_parser/templates/data_source_macros.j2
+-rw-r--r--   0 root         (0) root         (0)      102 2024-05-21 16:54:09.000000 mozilla_metric_config_parser-2024.5.1/metric_config_parser/templates/data_source_query.sql
+-rw-r--r--   0 root         (0) root         (0)     2750 2024-05-21 16:54:09.000000 mozilla_metric_config_parser-2024.5.1/metric_config_parser/templates/metrics_query.sql
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 16:54:18.802264 mozilla_metric_config_parser-2024.5.1/metric_config_parser/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-21 16:54:09.000000 mozilla_metric_config_parser-2024.5.1/metric_config_parser/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5118 2024-05-21 16:54:09.000000 mozilla_metric_config_parser-2024.5.1/metric_config_parser/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 16:54:18.802264 mozilla_metric_config_parser-2024.5.1/metric_config_parser/tests/integration/
+-rw-r--r--   0 root         (0) root         (0)     6657 2024-05-21 16:54:09.000000 mozilla_metric_config_parser-2024.5.1/metric_config_parser/tests/integration/test_config_integration.py
+-rw-r--r--   0 root         (0) root         (0)     2428 2024-05-21 16:54:09.000000 mozilla_metric_config_parser-2024.5.1/metric_config_parser/tests/test_alert.py
+-rw-r--r--   0 root         (0) root         (0)    26303 2024-05-21 16:54:09.000000 mozilla_metric_config_parser-2024.5.1/metric_config_parser/tests/test_analysis.py
+-rw-r--r--   0 root         (0) root         (0)    25837 2024-05-21 16:54:09.000000 mozilla_metric_config_parser-2024.5.1/metric_config_parser/tests/test_config.py
+-rw-r--r--   0 root         (0) root         (0)    11572 2024-05-21 16:54:09.000000 mozilla_metric_config_parser-2024.5.1/metric_config_parser/tests/test_experiment.py
+-rw-r--r--   0 root         (0) root         (0)     1581 2024-05-21 16:54:09.000000 mozilla_metric_config_parser-2024.5.1/metric_config_parser/tests/test_function.py
+-rw-r--r--   0 root         (0) root         (0)     2866 2024-05-21 16:54:09.000000 mozilla_metric_config_parser-2024.5.1/metric_config_parser/tests/test_metric.py
+-rw-r--r--   0 root         (0) root         (0)     8522 2024-05-21 16:54:09.000000 mozilla_metric_config_parser-2024.5.1/metric_config_parser/tests/test_monitoring.py
+-rw-r--r--   0 root         (0) root         (0)    12162 2024-05-21 16:54:09.000000 mozilla_metric_config_parser-2024.5.1/metric_config_parser/tests/test_outcomes.py
+-rw-r--r--   0 root         (0) root         (0)      458 2024-05-21 16:54:09.000000 mozilla_metric_config_parser-2024.5.1/metric_config_parser/tests/test_parameter.py
+-rw-r--r--   0 root         (0) root         (0)     2035 2024-05-21 16:54:09.000000 mozilla_metric_config_parser-2024.5.1/metric_config_parser/tests/test_population.py
+-rw-r--r--   0 root         (0) root         (0)     2808 2024-05-21 16:54:09.000000 mozilla_metric_config_parser-2024.5.1/metric_config_parser/tests/test_project.py
+-rw-r--r--   0 root         (0) root         (0)     4528 2024-05-21 16:54:09.000000 mozilla_metric_config_parser-2024.5.1/metric_config_parser/tests/test_sql.py
+-rw-r--r--   0 root         (0) root         (0)      725 2024-05-21 16:54:09.000000 mozilla_metric_config_parser-2024.5.1/metric_config_parser/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 16:54:18.806264 mozilla_metric_config_parser-2024.5.1/mozilla_metric_config_parser.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1590 2024-05-21 16:54:18.000000 mozilla_metric_config_parser-2024.5.1/mozilla_metric_config_parser.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1994 2024-05-21 16:54:18.000000 mozilla_metric_config_parser-2024.5.1/mozilla_metric_config_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 16:54:18.000000 mozilla_metric_config_parser-2024.5.1/mozilla_metric_config_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       70 2024-05-21 16:54:18.000000 mozilla_metric_config_parser-2024.5.1/mozilla_metric_config_parser.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      274 2024-05-21 16:54:18.000000 mozilla_metric_config_parser-2024.5.1/mozilla_metric_config_parser.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-21 16:54:18.000000 mozilla_metric_config_parser-2024.5.1/mozilla_metric_config_parser.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       85 2024-05-21 16:54:09.000000 mozilla_metric_config_parser-2024.5.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       67 2024-05-21 16:54:18.806264 mozilla_metric_config_parser-2024.5.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1574 2024-05-21 16:54:09.000000 mozilla_metric_config_parser-2024.5.1/setup.py
```

### Comparing `mozilla-metric-config-parser-2024.4.1/LICENSE` & `mozilla_metric_config_parser-2024.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2024.4.1/PKG-INFO` & `mozilla_metric_config_parser-2024.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mozilla-metric-config-parser
-Version: 2024.4.1
+Version: 2024.5.1
 Summary: Parses metric configuration files
 Home-page: https://github.com/mozilla/metric-config-parser
 Author: Mozilla Corporation
 Author-email: fx-data-dev@mozilla.org
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mozilla-metric-config-parser-2024.4.1/metric_config_parser/alert.py` & `mozilla_metric_config_parser-2024.5.1/metric_config_parser/alert.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2024.4.1/metric_config_parser/analysis.py` & `mozilla_metric_config_parser-2024.5.1/metric_config_parser/analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,17 +158,19 @@
 
         return ParameterDefinition(
             **{
                 "name": getattr(param_1, "name", None) or getattr(param_2, "name"),
                 "friendly_name": getattr(param_1, "friendly_name", None)
                 or getattr(param_2, "friendly_name"),
                 "description": getattr(param_1, "description", None) or param_2.description,
-                "value": {branch: branch_value for branch, branch_value in final_value.items()}
-                if isinstance(final_value, dict)
-                else final_value,
+                "value": (
+                    {branch: branch_value for branch, branch_value in final_value.items()}
+                    if isinstance(final_value, dict)
+                    else final_value
+                ),
                 "default": getattr(param_1, "default", None)
                 or default_value
                 or (dict() if isinstance(final_value, dict) else None),
                 "distinct_by_branch": getattr(param_1, "distinct_by_branch", None)
                 or param_2.distinct_by_branch,
             }
         ).validate()
```

### Comparing `mozilla-metric-config-parser-2024.4.1/metric_config_parser/cli.py` & `mozilla_metric_config_parser-2024.5.1/metric_config_parser/cli.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2024.4.1/metric_config_parser/config.py` & `mozilla_metric_config_parser-2024.5.1/metric_config_parser/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -675,18 +675,26 @@
             group_by=group_by,
             where=where,
             group_by_client_id=group_by_client_id,
             group_by_submission_date=group_by_submission_date,
         )
 
     def get_data_source_sql(
-        self, data_source: str, platform: str, where: Optional[str] = None
+        self,
+        data_source: str,
+        platform: str,
+        where: Optional[str] = None,
+        select_fields: bool = True,
     ) -> str:
         return generate_data_source_sql(
-            self, data_source=data_source, platform=platform, where=where
+            self,
+            data_source=data_source,
+            platform=platform,
+            where=where,
+            select_fields=select_fields,
         )
 
     def get_env(self) -> jinja2.Environment:
         """
         Create a Jinja2 environment that understands the SQL agg_* helpers in mozanalysis.metrics.
 
         Just a wrapper to avoid leaking temporary variables to the module scope."""
```

### Comparing `mozilla-metric-config-parser-2024.4.1/metric_config_parser/data_source.py` & `mozilla_metric_config_parser-2024.5.1/metric_config_parser/data_source.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,51 @@
-from typing import TYPE_CHECKING, Any, Dict, Optional, Union
+import fnmatch
+import re
+from enum import Enum
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Union
 
 import attr
 
 from metric_config_parser.errors import DefinitionNotFound
 
 if TYPE_CHECKING:
     from metric_config_parser.config import ConfigCollection
     from .experiment import ExperimentConfiguration
     from .definition import DefinitionSpecSub
     from .project import ProjectConfiguration
 
-from .util import converter
+from .util import converter, is_valid_slug
+
+
+class DataSourceJoinRelationship(Enum):
+    ONE_TO_ONE = "one_to_one"
+    MANY_TO_ONE = "many_to_one"
+    ONE_TO_MANY = "one_to_many"
+    MANY_TO_MANY = "many_to_many"
+
+    @staticmethod
+    def from_str(label):
+        match label:
+            case "one_to_one":
+                return DataSourceJoinRelationship.ONE_TO_ONE
+            case "many_to_one":
+                return DataSourceJoinRelationship.MANY_TO_ONE
+            case "one_to_many":
+                return DataSourceJoinRelationship.ONE_TO_MANY
+            case "many_to_many":
+                return DataSourceJoinRelationship.MANY_TO_MANY
+            case _:
+                raise NotImplementedError
+
+
+@attr.s(auto_attribs=True)
+class DataSourceJoin:
+    data_source: "DataSource"
+    relationship: Optional[DataSourceJoinRelationship]
+    on_expression: Optional[str]
 
 
 @attr.s(frozen=True, slots=True)
 class DataSource:
     """Represents a table or view, from which Metrics may be defined.
     Args:
         name (str): Name for the Data Source. Used in sanity metric
@@ -53,14 +84,16 @@
     experiments_column_type = attr.ib(default="simple", type=str)
     client_id_column = attr.ib(default="client_id", type=str)
     submission_date_column = attr.ib(default="submission_date", type=str)
     default_dataset = attr.ib(default=None, type=Optional[str])
     build_id_column = attr.ib(default="SAFE.SUBSTR(application.build_id, 0, 8)", type=str)
     friendly_name = attr.ib(default=None, type=str)
     description = attr.ib(default=None, type=str)
+    joins = attr.ib(default=None, type=List[DataSourceJoin])
+    columns_as_dimensions = attr.ib(default=False, type=bool)
 
     EXPERIMENT_COLUMN_TYPES = (None, "simple", "native", "glean")
 
     @experiments_column_type.validator
     def _check_experiments_column_type(self, attribute, value):
         if value not in self.EXPERIMENT_COLUMN_TYPES:
             raise ValueError(
@@ -97,20 +130,20 @@
     def resolve(
         self,
         spec: "DefinitionSpecSub",
         conf: Union["ExperimentConfiguration", "ProjectConfiguration"],
         configs: "ConfigCollection",
     ) -> DataSource:
         if self.name in spec.data_sources.definitions:
-            return spec.data_sources.definitions[self.name].resolve(spec)
+            return spec.data_sources.definitions[self.name].resolve(spec, conf, configs)
 
         data_source_definition = configs.get_data_source_definition(self.name, conf.app_name)
         if data_source_definition is None:
             raise DefinitionNotFound(f"No default definition for data source '{self.name}' found")
-        return data_source_definition.resolve(spec)
+        return data_source_definition.resolve(spec, conf, configs)
 
 
 converter.register_structure_hook(
     DataSourceReference, lambda obj, _type: DataSourceReference(name=obj)
 )
 
 
@@ -123,44 +156,79 @@
     experiments_column_type: Optional[str] = None
     client_id_column: Optional[str] = None
     submission_date_column: Optional[str] = None
     default_dataset: Optional[str] = None
     build_id_column: Optional[str] = None
     friendly_name: Optional[str] = None
     description: Optional[str] = None
+    joins: Optional[Dict[str, Dict[str, Any]]] = None
+    columns_as_dimensions: Optional[bool] = None
+
+    def resolve(
+        self,
+        spec: "DefinitionSpecSub",
+        conf: Union["ExperimentConfiguration", "ProjectConfiguration"],
+        configs: "ConfigCollection",
+    ) -> DataSource:
+        if not is_valid_slug(self.name):
+            # a data source name cannot include a wildcard * because if
+            # it does at this point in the code,
+            # that means it isn't defined anywhere and there's some dangling wildcard
+            raise ValueError(
+                f"Invalid identifier found in name {self.name}. "
+                + "Name must at least consist of one character, number or underscore. "
+                + "Wildcard characters are only allowed if matching slug is defined."
+            )
 
-    def resolve(self, spec: "DefinitionSpecSub") -> DataSource:
         params: Dict[str, Any] = {"name": self.name, "from_expression": self.from_expression}
         # Allow mozanalysis to infer defaults for these values:
         for k in (
             "experiments_column_type",
             "client_id_column",
             "submission_date_column",
             "default_dataset",
             "build_id_column",
             "friendly_name",
             "description",
+            "columns_as_dimensions",
         ):
             v = getattr(self, k)
             if v:
                 params[k] = v
         # experiments_column_type is a little special, though!
         # `None` is a valid value, which means there isn't any `experiments` column in the
         # data source, so mozanalysis shouldn't try to use it.
         # But mozanalysis has a different default value for that param ("simple"), and
         # TOML can't represent an explicit null. So we'll look for the string "none" and
         # transform it to the value None.
         if (self.experiments_column_type or "").lower() == "none":
             params["experiments_column_type"] = None
+
+        # resolve the data source joins
+        if self.joins and len(self.joins) > 0:
+            params["joins"] = [
+                DataSourceJoin(
+                    data_source=DataSourceReference(name=data_source).resolve(spec, conf, configs),
+                    relationship=(
+                        DataSourceJoinRelationship.from_str(join["relationship"])
+                        if "relationship" in join
+                        else None
+                    ),
+                    on_expression=join.get("on_expression", None),
+                )
+                for data_source, join in self.joins.items()
+            ]
+
         return DataSource(**params)
 
     def merge(self, other: "DataSourceDefinition"):
         """Merge with another data source definition."""
         for key in attr.fields_dict(type(self)):
-            setattr(self, key, getattr(other, key) or getattr(self, key))
+            if key != "name":
+                setattr(self, key, getattr(other, key) or getattr(self, key))
 
 
 @attr.s(auto_attribs=True)
 class DataSourcesSpec:
     """Holds data source definitions.
 
     This doesn't have a resolve() method to produce a concrete DataSourcesConfiguration
@@ -179,20 +247,24 @@
         return cls(definitions)
 
     def merge(self, other: "DataSourcesSpec"):
         """
         Merge another datasource spec into the current one.
         The `other` DataSourcesSpec overwrites existing keys.
         """
-        seen = []
+        seen = set()
         for key, _ in self.definitions.items():
-            if key in other.definitions:
-                self.definitions[key].merge(other.definitions[key])
-            seen.append(key)
+            for other_key in other.definitions:
+                # support wildcard characters in `other`
+                other_key_regex = re.compile(fnmatch.translate(other_key))
+                if other_key_regex.fullmatch(key):
+                    self.definitions[key].merge(other.definitions[other_key])
+                    seen.add(other_key)
+            seen.add(key)
         for key, definition in other.definitions.items():
-            if key not in seen:
+            if key not in seen and is_valid_slug(key):
                 self.definitions[key] = definition
 
 
 converter.register_structure_hook(
     DataSourcesSpec, lambda obj, _type: DataSourcesSpec.from_dict(obj)
 )
```

### Comparing `mozilla-metric-config-parser-2024.4.1/metric_config_parser/definition.py` & `mozilla_metric_config_parser-2024.5.1/metric_config_parser/definition.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2024.4.1/metric_config_parser/dimension.py` & `mozilla_metric_config_parser-2024.5.1/metric_config_parser/dimension.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2024.4.1/metric_config_parser/errors.py` & `mozilla_metric_config_parser-2024.5.1/metric_config_parser/errors.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2024.4.1/metric_config_parser/experiment.py` & `mozilla_metric_config_parser-2024.5.1/metric_config_parser/experiment.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2024.4.1/metric_config_parser/exposure_signal.py` & `mozilla_metric_config_parser-2024.5.1/metric_config_parser/exposure_signal.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2024.4.1/metric_config_parser/function.py` & `mozilla_metric_config_parser-2024.5.1/metric_config_parser/function.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2024.4.1/metric_config_parser/metric.py` & `mozilla_metric_config_parser-2024.5.1/metric_config_parser/metric.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import copy
+import fnmatch
+import re
 from collections import defaultdict
 from enum import Enum
 from textwrap import dedent
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Union
 
 import attr
 import jinja2
@@ -17,15 +19,15 @@
     from .definition import DefinitionSpecSub
     from .project import ProjectConfiguration
 
 from .data_source import DataSource, DataSourceReference
 from .parameter import ParameterDefinition
 from .pre_treatment import PreTreatmentReference
 from .statistic import Statistic
-from .util import converter
+from .util import converter, is_valid_slug
 
 
 class AnalysisPeriod(Enum):
     DAY = "day"
     WEEK = "week"
     DAYS_28 = "days28"
     OVERALL = "overall"
@@ -220,17 +222,17 @@
                     f"No default definition found for referenced metric {self.name}"
                 )
             elif upstream_metrics:
                 metric = Metric(
                     name=self.name,
                     data_source=None,
                     select_expression=None,
-                    friendly_name=dedent(self.friendly_name)
-                    if self.friendly_name
-                    else self.friendly_name,
+                    friendly_name=(
+                        dedent(self.friendly_name) if self.friendly_name else self.friendly_name
+                    ),
                     description=dedent(self.description) if self.description else self.description,
                     bigger_is_better=self.bigger_is_better,
                     analysis_bases=self.analysis_bases
                     or [AnalysisBasis.ENROLLMENTS, AnalysisBasis.EXPOSURES],
                     type=self.type or "scalar",
                     category=self.category,
                     depends_on=upstream_metrics,
@@ -252,17 +254,17 @@
                 configs=configs,
             )
 
             metric = Metric(
                 name=self.name,
                 data_source=self.data_source.resolve(spec, conf, configs),
                 select_expression=select_expression,
-                friendly_name=dedent(self.friendly_name)
-                if self.friendly_name
-                else self.friendly_name,
+                friendly_name=(
+                    dedent(self.friendly_name) if self.friendly_name else self.friendly_name
+                ),
                 description=dedent(self.description) if self.description else self.description,
                 bigger_is_better=self.bigger_is_better,
                 analysis_bases=self.analysis_bases
                 or [AnalysisBasis.ENROLLMENTS, AnalysisBasis.EXPOSURES],
                 type=self.type or "scalar",
                 category=self.category,
                 depends_on=upstream_metrics,
@@ -403,18 +405,22 @@
         self.daily = other.daily + self.daily
         self.weekly = other.weekly + self.weekly
         self.days28 = other.days28 + self.days28
         self.overall = other.overall + self.overall
         self.preenrollment_weekly = other.preenrollment_weekly + self.preenrollment_weekly
         self.preenrollment_days28 = other.preenrollment_days28 + self.preenrollment_days28
 
-        seen = []
+        seen = set()
         for key, _ in self.definitions.items():
-            if key in other.definitions:
-                self.definitions[key].merge(other.definitions[key])
-            seen.append(key)
+            for other_key in other.definitions:
+                # support wildcard characters in `other`
+                other_key_regex = re.compile(fnmatch.translate(other_key))
+                if other_key_regex.fullmatch(key):
+                    self.definitions[key].merge(other.definitions[other_key])
+                    seen.add(other_key)
+            seen.add(key)
         for key, definition in other.definitions.items():
-            if key not in seen:
+            if key not in seen and is_valid_slug(key):
                 self.definitions[key] = definition
 
 
 converter.register_structure_hook(MetricsSpec, lambda obj, _type: MetricsSpec.from_dict(obj))
```

### Comparing `mozilla-metric-config-parser-2024.4.1/metric_config_parser/metric_group.py` & `mozilla_metric_config_parser-2024.5.1/metric_config_parser/metric_group.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2024.4.1/metric_config_parser/monitoring.py` & `mozilla_metric_config_parser-2024.5.1/metric_config_parser/monitoring.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2024.4.1/metric_config_parser/outcome.py` & `mozilla_metric_config_parser-2024.5.1/metric_config_parser/outcome.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2024.4.1/metric_config_parser/parameter.py` & `mozilla_metric_config_parser-2024.5.1/metric_config_parser/parameter.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2024.4.1/metric_config_parser/population.py` & `mozilla_metric_config_parser-2024.5.1/metric_config_parser/population.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,25 +50,29 @@
                 )
 
         return PopulationConfiguration(
             data_source=self.data_source.resolve(spec, conf, configs) if self.data_source else None,
             boolean_pref=self.boolean_pref
             or (conf.population.boolean_pref if conf and not conf.is_rollout else None),
             channel=self.channel or (conf.population.channel if conf else None),
-            branches=self.branches
-            if self.branches is not None
-            else (
-                [branch for branch in conf.population.branches]
-                if conf and self.boolean_pref is None and not conf.is_rollout
-                else []
+            branches=(
+                self.branches
+                if self.branches is not None
+                else (
+                    [branch for branch in conf.population.branches]
+                    if conf and self.boolean_pref is None and not conf.is_rollout
+                    else []
+                )
             ),
             monitor_entire_population=self.monitor_entire_population,
-            group_by_dimension=self.group_by_dimension.resolve(spec, conf, configs)
-            if self.group_by_dimension
-            else None,
+            group_by_dimension=(
+                self.group_by_dimension.resolve(spec, conf, configs)
+                if self.group_by_dimension
+                else None
+            ),
         )
 
     def merge(self, other: "PopulationSpec") -> None:
         """
         Merge another population spec into the current one.
 
         The `other` PopulationSpec overwrites existing keys.
```

### Comparing `mozilla-metric-config-parser-2024.4.1/metric_config_parser/project.py` & `mozilla_metric_config_parser-2024.5.1/metric_config_parser/project.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2024.4.1/metric_config_parser/segment.py` & `mozilla_metric_config_parser-2024.5.1/metric_config_parser/segment.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2024.4.1/metric_config_parser/sql.py` & `mozilla_metric_config_parser-2024.5.1/metric_config_parser/sql.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 if TYPE_CHECKING:
     from .config import ConfigCollection
 
 FILE_PATH = Path(os.path.dirname(__file__))
 METRICS_QUERY = FILE_PATH / "templates" / "metrics_query.sql"
 DATA_SOURCE_QUERY = FILE_PATH / "templates" / "data_source_query.sql"
+DATA_SOURCE_MACROS = FILE_PATH / "templates" / "data_source_macros.j2"
 
 
 def generate_metrics_sql(
     config_collection: "ConfigCollection",
     metrics: List[str],
     platform: str,
     group_by: Union[List[str], Dict[str, str]] = [],
@@ -66,38 +67,56 @@
 
     # group by should be a dictionary with the key being the alias and
     # the value the potentially nested field;
     # it can also be specified as list if all fields are top-level fields that don't need an alias
     if isinstance(group_by, list):
         group_by = {g: g for g in group_by}
 
+    macros_template = DATA_SOURCE_MACROS.read_text()
     template = METRICS_QUERY.read_text()
+
+    # using `from_string()` in Jinja doens't support include statements, so
+    # substituting them here manually
+    template = template.replace("{% include 'data_source_macros.j2' %}", macros_template)
     return (
         config_collection.get_env()
         .from_string(template)
         .render(
             **{
                 "metrics_per_data_source": metrics_per_data_source,
                 "where": where,
                 "group_by": group_by,
                 "group_by_client_id": group_by_client_id,
                 "group_by_submission_date": group_by_submission_date,
+                "data_sources": {
+                    slug: data_source
+                    for definition in config_collection.definitions
+                    for slug, data_source in definition.spec.data_sources.definitions.items()
+                    if platform == definition.platform
+                },
+                "select_fields": True,
             }
         )
     )
 
 
 def generate_data_source_sql(
     config_collection: "ConfigCollection",
     data_source: str,
     platform: str,
     where: Optional[str] = None,
+    select_fields: bool = True,
 ) -> str:
     """Generates a SQL query for the specified data source."""
     template = DATA_SOURCE_QUERY.read_text()
+    macros_template = DATA_SOURCE_MACROS.read_text()
+
+    # using `from_string()` in Jinja doens't support include statements, so
+    # substituting them here manually
+    template = template.replace("{% include 'data_source_macros.j2' %}", macros_template)
     data_source_definition = config_collection.get_data_source_definition(data_source, platform)
 
     if data_source_definition is None:
         raise ValueError(f"No valid data source definition found for {data_source}")
 
     # default parameters need to be set explicitly otherwise they'll be None
     data_source_definition.client_id_column = data_source_definition.client_id_column or "client_id"
@@ -106,11 +125,18 @@
     )
     return (
         config_collection.get_env()
         .from_string(template)
         .render(
             **{
                 "data_source": data_source_definition,
+                "data_sources": {
+                    slug: data_source
+                    for definition in config_collection.definitions
+                    for slug, data_source in definition.spec.data_sources.definitions.items()
+                    if platform == definition.platform
+                },
                 "where": where,
+                "select_fields": select_fields,
             }
         )
     )
```

### Comparing `mozilla-metric-config-parser-2024.4.1/metric_config_parser/templates/metrics_query.sql` & `mozilla_metric_config_parser-2024.5.1/metric_config_parser/templates/metrics_query.sql`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+{% include 'data_source_macros.j2' %}
+
 (
 {% for data_source_slug, data_source_info in metrics_per_data_source.items() -%}
 {{ "WITH" if loop.first else "" }} {{ data_source_slug }} AS (
     SELECT
         {% if group_by_client_id -%}
         {{ data_source_info["data_source"].client_id_column }} AS client_id,
         {% endif -%}
@@ -10,30 +12,27 @@
         {% endif -%}
         {% for dimension, dimension_sql in group_by.items() -%}
         {{ dimension_sql }} AS {{ dimension }},
         {% endfor -%}
         {% for metric in data_source_info["metrics"] -%}
         {{ metric.select_expression }} AS {{ metric.name }},
         {% endfor %}
-    FROM
-        {{ data_source_info["data_source"].from_expression }}
-    {% if where -%}
-    WHERE
-        {{ where }}
-    {% endif -%}
-    GROUP BY    
+    FROM {{ data_source_query(data_source_info["data_source"]) }}
+    {% if group_by != {} or group_by_submission_date or group_by_client_id -%}
+    GROUP BY
         {% for dimension, dimension_sql in group_by.items() -%}
         {{ dimension }}{{ "," if not loop.last or group_by_submission_date or group_by_client_id else "" }}
         {% endfor -%}
         {% if group_by_client_id -%}
         client_id{{ "," if group_by_submission_date else "" }}
         {% endif -%}
         {% if group_by_submission_date -%}
         submission_date
         {% endif %}
+    {% endif -%}
 ){{ "," if not loop.last else "" }}
 {% endfor -%}
 
 {% for data_source_slug, data_source_info in metrics_per_data_source.items() -%}
 {% if loop.first -%}
 SELECT
     {% if group_by_client_id -%}
```

### Comparing `mozilla-metric-config-parser-2024.4.1/metric_config_parser/tests/conftest.py` & `mozilla_metric_config_parser-2024.5.1/metric_config_parser/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2024.4.1/metric_config_parser/tests/integration/test_config_integration.py` & `mozilla_metric_config_parser-2024.5.1/metric_config_parser/tests/integration/test_config_integration.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2024.4.1/metric_config_parser/tests/test_alert.py` & `mozilla_metric_config_parser-2024.5.1/metric_config_parser/tests/test_alert.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2024.4.1/metric_config_parser/tests/test_analysis.py` & `mozilla_metric_config_parser-2024.5.1/metric_config_parser/tests/test_analysis.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2024.4.1/metric_config_parser/tests/test_config.py` & `mozilla_metric_config_parser-2024.5.1/metric_config_parser/tests/test_config.py`

 * *Files 21% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from metric_config_parser.config import (
     Config,
     ConfigCollection,
     DefaultConfig,
     DefinitionConfig,
     Outcome,
 )
+from metric_config_parser.data_source import DataSourceJoinRelationship
 from metric_config_parser.errors import DefinitionNotFound
 from metric_config_parser.metric import MetricLevel
 from metric_config_parser.outcome import OutcomeSpec
 
 TEST_DIR = Path(__file__).parent
 
 
@@ -499,7 +500,265 @@
         with pytest.raises(Exception):
             DefinitionConfig(
                 slug="firefox_desktop",
                 platform="firefox_desktop",
                 spec=AnalysisSpec.from_dict(toml.loads(config_str)),
                 last_modified=datetime.datetime.now(),
             )
+
+    def test_data_source_joins(self):
+        config_str = dedent(
+            """
+            [data_sources.events]
+            from_expression = "mozdata.telemetry.events"
+            experiments_column_type = "simple"
+
+            [data_sources.metrics]
+            from_expression = "mozdata.telemetry.metrics"
+            experiments_column_type = "simple"
+
+            [data_sources.baseline]
+            from_expression = "mozdata.telemetry.baseline"
+            experiments_column_type = "simple"
+
+            [data_sources.baseline.joins.metrics]
+            on_expression = "metrics.client_id = baseline.client_id"
+            relationship = "many_to_one"
+
+            [data_sources.baseline.joins.events]
+            """
+        )
+
+        definition = DefinitionConfig(
+            slug="firefox_desktop",
+            platform="firefox_desktop",
+            spec=AnalysisSpec.from_dict(toml.loads(config_str)),
+            last_modified=datetime.datetime.now(),
+        )
+        config_collection = ConfigCollection(
+            configs=[], outcomes=[], defaults=[], definitions=[definition]
+        )
+
+        data_source = config_collection.get_data_source_definition(
+            "baseline", "firefox_desktop"
+        ).resolve(definition.spec, None, config_collection)
+
+        assert len(data_source.joins) == 2
+        assert data_source.joins[0].data_source.name == "metrics"
+        assert data_source.joins[0].on_expression == "metrics.client_id = baseline.client_id"
+        assert data_source.joins[0].relationship == DataSourceJoinRelationship.MANY_TO_ONE
+
+        assert data_source.joins[1].data_source.name == "events"
+
+    def test_data_source_joins_invalid(self):
+        config_str = dedent(
+            """
+            [data_sources.baseline]
+            from_expression = "mozdata.telemetry.baseline"
+            experiments_column_type = "simple"
+
+            [data_sources.baseline.joins.non_existing]
+            relationship = "many_to_one"
+            """
+        )
+
+        definition = DefinitionConfig(
+            slug="firefox_desktop",
+            platform="firefox_desktop",
+            spec=AnalysisSpec.from_dict(toml.loads(config_str)),
+            last_modified=datetime.datetime.now(),
+        )
+        config_collection = ConfigCollection(
+            configs=[], outcomes=[], defaults=[], definitions=[definition]
+        )
+
+        with pytest.raises(Exception):
+            config_collection.get_data_source_definition("baseline", "firefox_desktop").resolve(
+                definition.spec, None, config_collection
+            )
+
+    def test_data_source_joins_circular_dependency(self):
+        config_str = dedent(
+            """
+            [data_sources.baseline]
+            from_expression = "mozdata.telemetry.baseline"
+            experiments_column_type = "simple"
+
+            [data_sources.metrics]
+            from_expression = "mozdata.telemetry.metrics"
+            experiments_column_type = "simple"
+
+            [data_sources.baseline.joins.metrics]
+
+            [data_sources.metrics.joins.baseline]
+            """
+        )
+
+        definition = DefinitionConfig(
+            slug="firefox_desktop",
+            platform="firefox_desktop",
+            spec=AnalysisSpec.from_dict(toml.loads(config_str)),
+            last_modified=datetime.datetime.now(),
+        )
+        config_collection = ConfigCollection(
+            configs=[], outcomes=[], defaults=[], definitions=[definition]
+        )
+
+        with pytest.raises(Exception):
+            config_collection.get_data_source_definition("baseline", "firefox_desktop").resolve(
+                definition.spec, None, config_collection
+            )
+
+    def test_invalid_wildcard_in_data_source(self):
+        # needs to be [data_sources.'baseline_*']
+        config_str = dedent(
+            """
+            [data_sources.baseline_*]
+            from_expression = "mozdata.search.baseline"
+            experiments_column_type = "simple"
+            """
+        )
+
+        with pytest.raises(ValueError):
+            DefinitionConfig(
+                slug="firefox_desktop",
+                platform="firefox_desktop",
+                spec=AnalysisSpec.from_dict(toml.loads(config_str)),
+                last_modified=datetime.datetime.now(),
+            )
+
+    def test_merge_with_wildcards(self):
+        config_str = dedent(
+            """
+            [metrics.test_metric]
+            select_expression = 1
+            category = "test"
+
+            [data_sources.baseline]
+            from_expression = "mozdata.search.baseline"
+            experiments_column_type = "simple"
+            """
+        )
+
+        definition = DefinitionConfig(
+            slug="firefox_desktop",
+            platform="firefox_desktop",
+            spec=AnalysisSpec.from_dict(toml.loads(config_str)),
+            last_modified=datetime.datetime.now(),
+        )
+        config_collection_1 = ConfigCollection(
+            configs=[], outcomes=[], defaults=[], definitions=[definition]
+        )
+
+        config_str = dedent(
+            """
+            [data_sources.'*']
+            experiments_column_type = "none"
+
+            [metrics.'test_*']
+            data_source = "baseline"
+            category = "test_overwrite_first"
+
+            [metrics.'test_*'.statistics.bootstrap_mean]
+
+            [metrics.'test_me*']
+            category = "test_overwrite_second"
+            """
+        )
+        definition = DefinitionConfig(
+            slug="firefox_desktop",
+            platform="firefox_desktop",
+            spec=AnalysisSpec.from_dict(toml.loads(config_str)),
+            last_modified=datetime.datetime.now(),
+        )
+        config_collection_2 = ConfigCollection(
+            configs=[], outcomes=[], defaults=[], definitions=[definition]
+        )
+
+        config_collection_1.get_metric_definition(
+            "test_metric", "firefox_desktop"
+        ).data_source is None
+        assert (
+            config_collection_1.get_data_source_definition(
+                "baseline", "firefox_desktop"
+            ).experiments_column_type
+            == "simple"
+        )
+
+        config_collection_1.merge(config_collection_2)
+        assert (
+            config_collection_1.get_data_source_definition("baseline", "firefox_desktop").name
+            == "baseline"
+        )
+        assert (
+            config_collection_1.get_data_source_definition(
+                "baseline", "firefox_desktop"
+            ).experiments_column_type
+            == "none"
+        )
+        assert config_collection_1.get_data_source_definition("*", "firefox_desktop") is None
+        assert (
+            config_collection_1.get_metric_definition(
+                "test_metric", "firefox_desktop"
+            ).data_source.name
+            == "baseline"
+        )
+        assert (
+            "bootstrap_mean"
+            in config_collection_1.get_metric_definition(
+                "test_metric", "firefox_desktop"
+            ).statistics
+        )
+        assert (
+            config_collection_1.get_metric_definition("test_metric", "firefox_desktop").category
+            == "test_overwrite_second"
+        )
+
+    def test_merge_with_wildcards_invalid(self):
+        config_str = dedent(
+            """
+            [data_sources.baseline]
+            from_expression = "mozdata.search.baseline"
+            experiments_column_type = "simple"
+            """
+        )
+
+        definition = DefinitionConfig(
+            slug="firefox_desktop",
+            platform="firefox_desktop",
+            spec=AnalysisSpec.from_dict(toml.loads(config_str)),
+            last_modified=datetime.datetime.now(),
+        )
+        config_collection_1 = ConfigCollection(
+            configs=[], outcomes=[], defaults=[], definitions=[definition]
+        )
+
+        config_str = dedent(
+            """
+            [data_sources.'invalid_*']
+            experiments_column_type = "none"
+            """
+        )
+        definition = DefinitionConfig(
+            slug="firefox_desktop",
+            platform="firefox_desktop",
+            spec=AnalysisSpec.from_dict(toml.loads(config_str)),
+            last_modified=datetime.datetime.now(),
+        )
+        config_collection_2 = ConfigCollection(
+            configs=[], outcomes=[], defaults=[], definitions=[definition]
+        )
+
+        config_collection_1.merge(config_collection_2)
+        assert (
+            config_collection_1.get_data_source_definition("baseline", "firefox_desktop").name
+            == "baseline"
+        )
+        assert (
+            config_collection_1.get_data_source_definition(
+                "baseline", "firefox_desktop"
+            ).experiments_column_type
+            == "simple"
+        )
+        assert (
+            config_collection_1.get_data_source_definition("invalid_*", "firefox_desktop") is None
+        )
```

### Comparing `mozilla-metric-config-parser-2024.4.1/metric_config_parser/tests/test_experiment.py` & `mozilla_metric_config_parser-2024.5.1/metric_config_parser/tests/test_experiment.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2024.4.1/metric_config_parser/tests/test_function.py` & `mozilla_metric_config_parser-2024.5.1/metric_config_parser/tests/test_function.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2024.4.1/metric_config_parser/tests/test_metric.py` & `mozilla_metric_config_parser-2024.5.1/metric_config_parser/tests/test_metric.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2024.4.1/metric_config_parser/tests/test_monitoring.py` & `mozilla_metric_config_parser-2024.5.1/metric_config_parser/tests/test_monitoring.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2024.4.1/metric_config_parser/tests/test_outcomes.py` & `mozilla_metric_config_parser-2024.5.1/metric_config_parser/tests/test_outcomes.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2024.4.1/metric_config_parser/tests/test_population.py` & `mozilla_metric_config_parser-2024.5.1/metric_config_parser/tests/test_population.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2024.4.1/metric_config_parser/tests/test_project.py` & `mozilla_metric_config_parser-2024.5.1/metric_config_parser/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2024.4.1/metric_config_parser/tests/test_sql.py` & `mozilla_metric_config_parser-2024.5.1/metric_config_parser/tests/test_sql.py`

 * *Files 14% similar despite different names*

```diff
@@ -88,7 +88,42 @@
 
 
 def test_data_source_not_found(config_collection):
     with pytest.raises(ValueError):
         config_collection.get_data_source_sql(
             data_source="non-existing", platform="firefox_desktop"
         )
+
+
+def test_data_source_with_join(config_collection):
+    assert (
+        config_collection.get_data_source_sql(
+            data_source="joined_baseline",
+            platform="firefox_desktop",
+            where="submission_date = '2023-01-01'",
+        )
+        == (TEST_DATA / "test_generate_data_source_with_join.expected.sql").read_text()
+    )
+
+
+def test_data_source_with_multiple_join(config_collection):
+    assert (
+        config_collection.get_data_source_sql(
+            data_source="multiple_joined_baseline",
+            platform="firefox_desktop",
+            where="submission_date = '2023-01-01'",
+        )
+        == (TEST_DATA / "test_generate_data_source_with_multi_join.expected.sql").read_text()
+    )
+
+
+def test_metric_with_joined_data_source(config_collection):
+    assert (
+        config_collection.get_metrics_sql(
+            metrics=["joined_metric"],
+            platform="firefox_desktop",
+            where="submission_date = '2023-01-01' AND normalized_channel = 'release'",
+            group_by_client_id=True,
+            group_by_submission_date=False,
+        )
+        == (TEST_DATA / "test_generate_query_with_joined_data_sources.expected.sql").read_text()
+    )
```

### Comparing `mozilla-metric-config-parser-2024.4.1/metric_config_parser/util.py` & `mozilla_metric_config_parser-2024.5.1/metric_config_parser/util.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import re
 import shutil
 import tempfile
 from contextlib import contextmanager
 from datetime import datetime
 from pathlib import Path
 from typing import Optional
 
@@ -21,7 +22,12 @@
             shutil.rmtree(name)
 
 
 def parse_date(yyyy_mm_dd: Optional[str]) -> Optional[datetime]:
     if not yyyy_mm_dd:
         return None
     return datetime.strptime(yyyy_mm_dd, "%Y-%m-%d").replace(tzinfo=pytz.utc)
+
+
+def is_valid_slug(slug: str) -> bool:
+    """Returns whether a slug name is valid."""
+    return bool(re.match(r"^[a-zA-Z0-9_]+$", slug))
```

### Comparing `mozilla-metric-config-parser-2024.4.1/mozilla_metric_config_parser.egg-info/PKG-INFO` & `mozilla_metric_config_parser-2024.5.1/mozilla_metric_config_parser.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mozilla-metric-config-parser
-Version: 2024.4.1
+Version: 2024.5.1
 Summary: Parses metric configuration files
 Home-page: https://github.com/mozilla/metric-config-parser
 Author: Mozilla Corporation
 Author-email: fx-data-dev@mozilla.org
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mozilla-metric-config-parser-2024.4.1/mozilla_metric_config_parser.egg-info/SOURCES.txt` & `mozilla_metric_config_parser-2024.5.1/mozilla_metric_config_parser.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 metric_config_parser/population.py
 metric_config_parser/pre_treatment.py
 metric_config_parser/project.py
 metric_config_parser/segment.py
 metric_config_parser/sql.py
 metric_config_parser/statistic.py
 metric_config_parser/util.py
+metric_config_parser/templates/data_source_macros.j2
 metric_config_parser/templates/data_source_query.sql
 metric_config_parser/templates/metrics_query.sql
 metric_config_parser/tests/__init__.py
 metric_config_parser/tests/conftest.py
 metric_config_parser/tests/test_alert.py
 metric_config_parser/tests/test_analysis.py
 metric_config_parser/tests/test_config.py
```

### Comparing `mozilla-metric-config-parser-2024.4.1/setup.py` & `mozilla_metric_config_parser-2024.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,9 +61,9 @@
     long_description=text_from_file("README.md"),
     long_description_content_type="text/markdown",
     python_requires=">=3.6",
     entry_points="""
         [console_scripts]
         metric-config-parser=metric_config_parser.cli:cli
     """,
-    version="2024.4.1",
+    version="2024.5.1",
 )
```

